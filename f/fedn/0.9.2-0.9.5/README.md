# Comparing `tmp/fedn-0.9.2.tar.gz` & `tmp/fedn-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedn-0.9.2.tar", last modified: Wed May  8 11:26:14 2024, max compression
+gzip compressed data, was "fedn-0.9.5.tar", last modified: Wed May 22 12:52:34 2024, max compression
```

## Comparing `fedn-0.9.2.tar` & `fedn-0.9.5.tar`

### file list

```diff
@@ -1,157 +1,159 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.168154 fedn-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-08 11:26:10.000000 fedn-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-08 11:26:14.168154 fedn-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6152 2024-05-08 11:26:10.000000 fedn-0.9.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.144154 fedn-0.9.2/fedn/
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.148154 fedn-0.9.2/fedn/cli/
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5725 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/client_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/combiner_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/config_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/model_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2386 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/package_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/round_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/run_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/session_cmd.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/status_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.148154 fedn-0.9.2/fedn/cli/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/tests/tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/cli/validation_cmd.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.148154 fedn-0.9.2/fedn/common/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.152154 fedn-0.9.2/fedn/common/certificate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3102 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/certificate/certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2067 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/certificate/certificatemanager.py
--rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3351 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/log_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.152154 fedn-0.9.2/fedn/common/net/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/common/net/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.152154 fedn-0.9.2/fedn/network/
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.152154 fedn-0.9.2/fedn/network/api/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    24291 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    37406 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     5029 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/network.py
--rw-r--r--   0 runner    (1001) docker     (127)    19749 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/api/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/client_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/combiner_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    18069 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/model_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/package_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/round_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9198 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/session_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/status_routes.py
--rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/api/v1/validation_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/clients/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    32803 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     5576 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     6238 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/package.py
--rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/state.py
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/clients/test_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/combiner/
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/combiner/aggregators/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/aggregators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/aggregators/fedavg.py
--rw-r--r--   0 runner    (1001) docker     (127)    10765 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/aggregators/fedopt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/combiner/aggregators/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/aggregators/tests/test_fedavg.py
--rw-r--r--   0 runner    (1001) docker     (127)    25576 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/combiner.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/combiner_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)    10057 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/interfaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     7145 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/modelservice.py
--rw-r--r--   0 runner    (1001) docker     (127)    14925 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/combiner/roundhandler.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.156154 fedn-0.9.2/fedn/network/controller/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14198 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/controller/control.py
--rw-r--r--   0 runner    (1001) docker     (127)    11182 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/controller/controlbase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/grpc/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/grpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/grpc/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/grpc/fedn_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/grpc/fedn_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/grpc/server.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/loadbalancer/
--rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/loadbalancer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/loadbalancer/firstavailable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/loadbalancer/leastpacked.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/loadbalancer/loadbalancerbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/storage/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/storage/models/
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/models/memorymodelstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/models/modelstorage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/models/tempmodelstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/storage/models/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/models/tests/test_tempmodelstorage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/storage/s3/
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/s3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/s3/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/s3/miniorepository.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/s3/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.160154 fedn-0.9.2/fedn/network/storage/statestore/
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29572 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/mongostatestore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/statestorebase.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.164154 fedn-0.9.2/fedn/network/storage/statestore/stores/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/client_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     4286 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/combiner_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/model_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     5190 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/package_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3054 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/round_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/session_store.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/status_store.py
--rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/store.py
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/network/storage/statestore/stores/validation_store.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.164154 fedn-0.9.2/fedn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/checksum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8994 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     4128 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.164154 fedn-0.9.2/fedn/utils/flowercompat/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/flowercompat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/flowercompat/client_app_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.164154 fedn-0.9.2/fedn/utils/helpers/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/helperbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.168154 fedn-0.9.2/fedn/utils/helpers/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/plugins/androidhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     4865 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/plugins/numpyhelper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.168154 fedn-0.9.2/fedn/utils/helpers/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/helpers/tests/test_numpyhelper.py
--rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    15222 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/plots.py
--rw-r--r--   0 runner    (1001) docker     (127)     6036 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/process.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.168154 fedn-0.9.2/fedn/utils/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-08 11:26:10.000000 fedn-0.9.2/fedn/utils/tests/test_parameters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 11:26:14.168154 fedn-0.9.2/fedn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20324 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-08 11:26:14.000000 fedn-0.9.2/fedn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-05-08 11:26:10.000000 fedn-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 11:26:14.168154 fedn-0.9.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11350 2024-05-22 12:52:30.000000 fedn-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    20572 2024-05-22 12:52:34.419967 fedn-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6400 2024-05-22 12:52:30.000000 fedn-0.9.5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.395967 fedn-0.9.5/fedn/
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.399967 fedn-0.9.5/fedn/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5707 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/client_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3712 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/combiner_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/config_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/model_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/package_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/round_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8091 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/run_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1551 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/session_cmd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/status_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.399967 fedn-0.9.5/fedn/cli/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/tests/tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/cli/validation_cmd.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.399967 fedn-0.9.5/fedn/common/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.399967 fedn-0.9.5/fedn/common/certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3048 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/certificate/certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2025 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/certificate/certificatemanager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3417 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3339 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/log_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.399967 fedn-0.9.5/fedn/common/net/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/common/net/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.403967 fedn-0.9.5/fedn/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.403967 fedn-0.9.5/fedn/network/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24290 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37381 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19307 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      523 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14651 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.407967 fedn-0.9.5/fedn/network/api/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/client_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10257 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/combiner_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18104 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/model_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13472 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/package_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/round_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11741 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/session_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12348 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/status_routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13119 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/api/v1/validation_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.407967 fedn-0.9.5/fedn/network/clients/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32804 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5558 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/clients/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.407967 fedn-0.9.5/fedn/network/combiner/
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/combiner/aggregators/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/aggregators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6884 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/aggregators/aggregatorbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4325 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/aggregators/fedavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10762 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/aggregators/fedopt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/combiner/aggregators/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/aggregators/tests/test_fedavg.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26124 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/combiner.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/combiner_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4587 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10053 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/interfaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7144 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/modelservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14917 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/combiner/roundhandler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15979 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/controller/control.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11139 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/controller/controlbase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/grpc/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/grpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/grpc/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10980 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/grpc/fedn_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32182 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/grpc/fedn_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/grpc/server.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/loadbalancer/
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/loadbalancer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/loadbalancer/firstavailable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/loadbalancer/leastpacked.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/loadbalancer/loadbalancerbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/storage/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/models/memorymodelstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1627 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/models/modelstorage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3189 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/models/tempmodelstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.411967 fedn-0.9.5/fedn/network/storage/models/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/models/tests/test_tempmodelstorage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.415967 fedn-0.9.5/fedn/network/storage/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/s3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/s3/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3813 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/s3/miniorepository.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3831 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/s3/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.415967 fedn-0.9.5/fedn/network/storage/statestore/
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29556 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/mongostatestore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/statestorebase.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.415967 fedn-0.9.5/fedn/network/storage/statestore/stores/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3360 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/client_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4309 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/combiner_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7055 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/model_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5213 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/package_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/round_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/session_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3755 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/status_store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/store.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3815 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/network/storage/statestore/stores/validation_store.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/checksum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8978 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4118 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/flowercompat/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/flowercompat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4520 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/flowercompat/client_app_adapter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/helperbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/helpers/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3323 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/plugins/androidhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/plugins/binaryhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6461 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/plugins/numpyhelper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/helpers/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/helpers/tests/test_numpyhelper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1639 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15121 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/plots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6035 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/process.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn/utils/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-22 12:52:30.000000 fedn-0.9.5/fedn/utils/tests/test_parameters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:34.419967 fedn-0.9.5/fedn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20572 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4361 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 12:52:34.000000 fedn-0.9.5/fedn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     7379 2024-05-22 12:52:30.000000 fedn-0.9.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:52:34.419967 fedn-0.9.5/setup.cfg
```

### Comparing `fedn-0.9.2/LICENSE` & `fedn-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/PKG-INFO` & `fedn-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.2
+Version: 0.9.5
 Summary: Scaleout Federated Learning
 Author-email: Scaleout Systems AB <contact@scaleoutsystems.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -284,15 +284,21 @@
 
 -  Secure deployment of server-side / control-plane on Kubernetes.
 -  UI with dashboards for orchestrating experiments and visualizing results
 -  Team features - collaborate with other users in shared project workspaces. 
 -  Features for the trusted-third party: Manage access to the FL network, FL clients and training progress.
 -  REST API for handling experiments/jobs. 
 -  View and export logging and tracing information. 
--  Public cloud, dedicated cloud and on-premise deployment options. 
+-  Public cloud, dedicated cloud and on-premise deployment options.
+
+Available clients:
+
+- Python client (this repository)
+- C++ client (`FEDn C++ client <https://github.com/scaleoutsystems/fedn-cpp-client>`__)
+- Android Kotlin client (`FEDn Kotlin client <https://github.com/scaleoutsystems/fedn-android-client>`__)
 
 
 Getting started
 ============================
 
 Get started with FEDn in two steps:
```

### Comparing `fedn-0.9.2/README.rst` & `fedn-0.9.5/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,21 @@
 
 -  Secure deployment of server-side / control-plane on Kubernetes.
 -  UI with dashboards for orchestrating experiments and visualizing results
 -  Team features - collaborate with other users in shared project workspaces. 
 -  Features for the trusted-third party: Manage access to the FL network, FL clients and training progress.
 -  REST API for handling experiments/jobs. 
 -  View and export logging and tracing information. 
--  Public cloud, dedicated cloud and on-premise deployment options. 
+-  Public cloud, dedicated cloud and on-premise deployment options.
+
+Available clients:
+
+- Python client (this repository)
+- C++ client (`FEDn C++ client <https://github.com/scaleoutsystems/fedn-cpp-client>`__)
+- Android Kotlin client (`FEDn Kotlin client <https://github.com/scaleoutsystems/fedn-android-client>`__)
 
 
 Getting started
 ============================
 
 Get started with FEDn in two steps:
```

### Comparing `fedn-0.9.2/fedn/cli/__init__.py` & `fedn-0.9.5/fedn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/cli/client_cmd.py` & `fedn-0.9.5/fedn/cli/client_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,44 +11,40 @@
 
 
 def validate_client_config(config):
     """Validate client configuration.
 
     :param config: Client config (dict).
     """
-
     try:
         if config["discover_host"] is None or config["discover_host"] == "":
             raise InvalidClientConfig("Missing required configuration: discover_host")
         if "discover_port" not in config.keys():
             config["discover_port"] = None
     except Exception:
         raise InvalidClientConfig("Could not load config from file. Check config")
 
 
 @main.group("client")
 @click.pass_context
 def client_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @client_cmd.command("list")
 @click.pass_context
 def list_clients(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of clients
     - result: list of clients
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="clients")
     headers = {}
@@ -110,17 +106,15 @@
     trainer,
     init,
     logfile,
     heartbeat_interval,
     reconnect_after_missed_heartbeat,
     verbosity,
 ):
-    """
-
-    :param ctx:
+    """:param ctx:
     :param discoverhost:
     :param discoverport:
     :param token:
     :param name:
     :param client_id:
     :param remote:
     :param dry_run:
```

### Comparing `fedn-0.9.2/fedn/cli/combiner_cmd.py` & `fedn-0.9.5/fedn/cli/combiner_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, apply_config, get_api_url, get_token, print_response
 
 
 @main.group("combiner")
 @click.pass_context
 def combiner_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @combiner_cmd.command("start")
 @click.option("-d", "--discoverhost", required=False, help="Hostname for discovery services (reducer).")
 @click.option("-p", "--discoverport", required=False, help="Port for discovery services (reducer).")
@@ -29,17 +27,15 @@
 @click.option("-f", "--fqdn", required=False, default=None, help="Set fully qualified domain name")
 @click.option("-s", "--secure", is_flag=True, help="Enable SSL/TLS encrypted gRPC channels.")
 @click.option("-v", "--verify", is_flag=True, help="Verify SSL/TLS for REST discovery service (reducer)")
 @click.option("-c", "--max_clients", required=False, default=30, help="The maximal number of client connections allowed.")
 @click.option("-in", "--init", required=False, default=None, help="Path to configuration file to (re)init combiner.")
 @click.pass_context
 def start_cmd(ctx, discoverhost, discoverport, token, name, host, port, fqdn, secure, verify, max_clients, init):
-    """
-
-    :param ctx:
+    """:param ctx:
     :param discoverhost:
     :param discoverport:
     :param token:
     :param name:
     :param hostname:
     :param port:
     :param secure:
@@ -72,16 +68,15 @@
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @combiner_cmd.command("list")
 @click.pass_context
 def list_combiners(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of combiners
     - result: list of combiners
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="combiners")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/config_cmd.py` & `fedn-0.9.5/fedn/cli/config_cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,16 +17,15 @@
     {"name": "FEDN_PACKAGE_EXTRACT_DIR", "description": "The directory to extract packages to."},
 ]
 
 
 @main.group("config", invoke_without_command=True)
 @click.pass_context
 def config_cmd(ctx):
-    """
-    - Configuration commands for the FEDn CLI.
+    """- Configuration commands for the FEDn CLI.
     """
     if ctx.invoked_subcommand is None:
         click.echo("\n--- FEDn Cli Configuration ---\n")
         click.echo("Current configuration:\n")
 
         for env in envs:
             name = env["name"]
```

### Comparing `fedn-0.9.2/fedn/cli/model_cmd.py` & `fedn-0.9.5/fedn/cli/model_cmd.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("model")
 @click.pass_context
 def model_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @model_cmd.command("list")
 @click.pass_context
 def list_models(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of models
     - result: list of models
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="models")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/package_cmd.py` & `fedn-0.9.5/fedn/cli/package_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,17 +9,15 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("package")
 @click.pass_context
 def package_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @package_cmd.command("create")
 @click.option("-p", "--path", required=True, help="Path to package directory containing fedn.yaml")
 @click.option("-n", "--name", required=False, default="package.tgz", help="Name of package tarball")
@@ -47,16 +45,15 @@
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @package_cmd.command("list")
 @click.pass_context
 def list_packages(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of packages
     - result: list of packages
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="packages")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/round_cmd.py` & `fedn-0.9.5/fedn/cli/round_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("round")
 @click.pass_context
 def round_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @round_cmd.command("list")
 @click.pass_context
 def list_rounds(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of rounds
     - result: list of rounds
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="rounds")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/run_cmd.py` & `fedn-0.9.5/fedn/cli/run_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,17 +13,15 @@
 
 from .client_cmd import validate_client_config
 from .main import main
 from .shared import apply_config
 
 
 def get_statestore_config_from_file(init):
-    """
-
-    :param init:
+    """:param init:
     :return:
     """
     with open(init, "r") as file:
         try:
             settings = dict(yaml.safe_load(file))
             return settings
         except yaml.YAMLError as e:
@@ -39,17 +37,15 @@
         exit(-1)
     return helper
 
 
 @main.group("run")
 @click.pass_context
 def run_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @run_cmd.command("build")
 @click.option("-p", "--path", required=True, help="Path to package directory containing fedn.yaml")
 @click.pass_context
@@ -121,17 +117,15 @@
     trainer,
     init,
     logfile,
     heartbeat_interval,
     reconnect_after_missed_heartbeat,
     verbosity,
 ):
-    """
-
-    :param ctx:
+    """:param ctx:
     :param discoverhost:
     :param discoverport:
     :param token:
     :param name:
     :param client_id:
     :param remote:
     :param dry_run:
@@ -197,17 +191,15 @@
 @click.option("-f", "--fqdn", required=False, default=None, help="Set fully qualified domain name")
 @click.option("-s", "--secure", is_flag=True, help="Enable SSL/TLS encrypted gRPC channels.")
 @click.option("-v", "--verify", is_flag=True, help="Verify SSL/TLS for REST discovery service (reducer)")
 @click.option("-c", "--max_clients", required=False, default=30, help="The maximal number of client connections allowed.")
 @click.option("-in", "--init", required=False, default=None, help="Path to configuration file to (re)init combiner.")
 @click.pass_context
 def combiner_cmd(ctx, discoverhost, discoverport, token, name, host, port, fqdn, secure, verify, max_clients, init):
-    """
-
-    :param ctx:
+    """:param ctx:
     :param discoverhost:
     :param discoverport:
     :param token:
     :param name:
     :param hostname:
     :param port:
     :param secure:
```

### Comparing `fedn-0.9.2/fedn/cli/session_cmd.py` & `fedn-0.9.5/fedn/cli/session_cmd.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("session")
 @click.pass_context
 def session_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @session_cmd.command("list")
 @click.pass_context
 def list_sessions(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of sessions
     - result: list of sessions
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="sessions")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/shared.py` & `fedn-0.9.5/fedn/cli/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,16 +61,15 @@
 
 def get_client_package_dir(path: str) -> str:
     return path or os.environ.get("FEDN_PACKAGE_DIR", None)
 
 
 # Print response from api (list of entities)
 def print_response(response, entity_name: str):
-    """
-    Prints the api response to the cli.
+    """Prints the api response to the cli.
     :param response:
         type: array
         description: list of entities
     :param entity_name:
         type: string
         description: name of entity
     return: None
```

### Comparing `fedn-0.9.2/fedn/cli/status_cmd.py` & `fedn-0.9.5/fedn/cli/status_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("status")
 @click.pass_context
 def status_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @status_cmd.command("list")
 @click.pass_context
 def list_statuses(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of statuses
     - result: list of statuses
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="statuses")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/cli/tests/tests.py` & `fedn-0.9.5/fedn/cli/tests/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/cli/validation_cmd.py` & `fedn-0.9.5/fedn/cli/validation_cmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,31 +4,28 @@
 from .main import main
 from .shared import CONTROLLER_DEFAULTS, get_api_url, get_token, print_response
 
 
 @main.group("validation")
 @click.pass_context
 def validation_cmd(ctx):
-    """
-
-    :param ctx:
+    """:param ctx:
     """
     pass
 
 
 @click.option("-p", "--protocol", required=False, default=CONTROLLER_DEFAULTS["protocol"], help="Communication protocol of controller (api)")
 @click.option("-H", "--host", required=False, default=CONTROLLER_DEFAULTS["host"], help="Hostname of controller (api)")
 @click.option("-P", "--port", required=False, default=CONTROLLER_DEFAULTS["port"], help="Port of controller (api)")
 @click.option("-t", "--token", required=False, help="Authentication token")
 @click.option("--n_max", required=False, help="Number of items to list")
 @validation_cmd.command("list")
 @click.pass_context
 def list_validations(ctx, protocol: str, host: str, port: str, token: str = None, n_max: int = None):
-    """
-    Return:
+    """Return:
     ------
     - count: number of validations
     - result: list of validations
 
     """
     url = get_api_url(protocol=protocol, host=host, port=port, endpoint="validations")
     headers = {}
```

### Comparing `fedn-0.9.2/fedn/common/certificate/certificate.py` & `fedn-0.9.5/fedn/common/certificate/certificate.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 
 from OpenSSL import crypto
 
 from fedn.common.log_config import logger
 
 
 class Certificate:
-    """
-    Utility to generate unsigned certificates.
+    """Utility to generate unsigned certificates.
 
     """
 
     CERT_NAME = "cert.pem"
     KEY_NAME = "key.pem"
     BITS = 2048
 
@@ -33,16 +32,15 @@
             self.name = name
         else:
             self.name = str(uuid.uuid4())
 
     def gen_keypair(
         self,
     ):
-        """
-        Generate keypair.
+        """Generate keypair.
 
         """
         key = crypto.PKey()
         key.generate_key(crypto.TYPE_RSA, 2048)
         cert = crypto.X509()
         cert.get_subject().C = "SE"
         cert.get_subject().ST = "Stockholm"
@@ -61,50 +59,42 @@
         with open(self.key_path, "wb") as keyfile:
             keyfile.write(crypto.dump_privatekey(crypto.FILETYPE_PEM, key))
 
         with open(self.cert_path, "wb") as certfile:
             certfile.write(crypto.dump_certificate(crypto.FILETYPE_PEM, cert))
 
     def set_keypair_raw(self, certificate, privatekey):
-        """
-
-        :param certificate:
+        """:param certificate:
         :param privatekey:
         """
         with open(self.key_path, "wb") as keyfile:
             keyfile.write(crypto.dump_privatekey(crypto.FILETYPE_PEM, privatekey))
 
         with open(self.cert_path, "wb") as certfile:
             certfile.write(crypto.dump_certificate(crypto.FILETYPE_PEM, certificate))
 
     def get_keypair_raw(self):
-        """
-
-        :return:
+        """:return:
         """
         with open(self.key_path, "rb") as keyfile:
             key_buf = keyfile.read()
         with open(self.cert_path, "rb") as certfile:
             cert_buf = certfile.read()
         return copy.deepcopy(cert_buf), copy.deepcopy(key_buf)
 
     def get_key(self):
-        """
-
-        :return:
+        """:return:
         """
         with open(self.key_path, "rb") as keyfile:
             key_buf = keyfile.read()
         key = crypto.load_privatekey(crypto.FILETYPE_PEM, key_buf)
         return key
 
     def get_cert(self):
-        """
-
-        :return:
+        """:return:
         """
         with open(self.cert_path, "rb") as certfile:
             cert_buf = certfile.read()
         cert = crypto.load_certificate(crypto.FILETYPE_PEM, cert_buf)
         return cert
 
     def __str__(self):
```

### Comparing `fedn-0.9.2/fedn/common/certificate/certificatemanager.py` & `fedn-0.9.5/fedn/common/certificate/certificatemanager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import os
 
 from .certificate import Certificate
 
 
 class CertificateManager:
-    """
-    Utility to handle certificates for both Reducer and Combiner services.
+    """Utility to handle certificates for both Reducer and Combiner services.
 
     """
 
     def __init__(self, directory):
         self.directory = directory
         self.certificates = []
         self.allowed = dict()
         self.load_all()
 
     def get_or_create(self, name):
-        """
-        Look for an existing certificate, if not found, generate a self-signed certificate based on name.
+        """Look for an existing certificate, if not found, generate a self-signed certificate based on name.
 
         :param name: The name used when issuing the certificate.
         :return: A certificate
         :rtype: str
         """
         search = self.find(name)
         if search:
@@ -29,43 +27,39 @@
         else:
             cert = Certificate(self.directory, name=name, cert_name=name + "-cert.pem", key_name=name + "-key.pem")
             cert.gen_keypair()
             self.certificates.append(cert)
             return cert
 
     def add(self, certificate):
-        """
-        Add certificate to certificate list.
+        """Add certificate to certificate list.
 
         :param certificate:
         :return: Success status (True, False)
         :rtype: Boolean
         """
         if not self.find(certificate.name):
             self.certificates.append(certificate)
             return True
         return False
 
     def load_all(self):
-        """
-        Load all certificates and add to certificates list.
+        """Load all certificates and add to certificates list.
 
         """
         for filename in sorted(os.listdir(self.directory)):
             if filename.endswith("cert.pem"):
                 name = filename.split("-")[0]
                 key_name = name + "-key.pem"
 
                 c = Certificate(self.directory, name=name, cert_name=filename, key_name=key_name)
                 self.certificates.append(c)
 
     def find(self, name):
-        """
-
-        :param name: Name of certificate
+        """:param name: Name of certificate
         :return: certificate if successful, else None
         """
         for cert in self.certificates:
             if cert.name == name:
                 return cert
         for cert in self.allowed:
             if cert.name == name:
```

### Comparing `fedn-0.9.2/fedn/common/config.py` & `fedn-0.9.5/fedn/common/config.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/common/log_config.py` & `fedn-0.9.5/fedn/common/log_config.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,16 +58,15 @@
 
     http_handler = StudioHTTPHandler(host=REMOTE_LOG_SERVER, url=REMOTE_LOG_PATH, method="POST", token=remote_token)
     http_handler.setLevel(rloglevel)
     logger.addHandler(http_handler)
 
 
 def set_log_level_from_string(level_str):
-    """
-    Set the log level based on a string input.
+    """Set the log level based on a string input.
     """
     # Mapping of string representation to logging constants
     level_mapping = {
         "CRITICAL": logging.CRITICAL,
         "ERROR": logging.ERROR,
         "WARNING": logging.WARNING,
         "INFO": logging.INFO,
@@ -81,16 +80,15 @@
         raise ValueError(f"Invalid log level: {level_str}")
 
     # Set the log level
     logger.setLevel(level)
 
 
 def set_log_stream(log_file):
-    """
-    Redirect the log stream to a specified file, if log_file is set.
+    """Redirect the log stream to a specified file, if log_file is set.
     """
     if not log_file:
         return
 
     # Remove existing handlers
     for h in logger.handlers[:]:
         logger.removeHandler(h)
```

### Comparing `fedn-0.9.2/fedn/network/api/auth.py` & `fedn-0.9.5/fedn/network/api/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/client.py` & `fedn-0.9.5/fedn/network/api/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -493,15 +493,14 @@
         """Get a session from the statestore.
 
         :param id: The session id to get.
         :type id: str
         :return: Session.
         :rtype: dict
         """
-
         response = requests.get(self._get_url_api_v1(f"sessions/{id}"), self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_sessions(self, n_max: int = None):
```

### Comparing `fedn-0.9.2/fedn/network/api/interface.py` & `fedn-0.9.5/fedn/network/api/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -190,15 +190,14 @@
         """Set the compute package in the statestore.
 
         :param file: The compute package to set.
         :type file: file
         :return: A json response with success or failure message.
         :rtype: :class:`flask.Response`
         """
-
         if self.control.state() == ReducerState.instructing or self.control.state() == ReducerState.monitoring:
             return (
                 jsonify(
                     {
                         "success": False,
                         "message": "Reducer is in instructing or monitoring state." "Cannot set compute package.",
                     }
@@ -303,15 +302,14 @@
         :param skip: The number of compute packages to skip.
         :type skip: str
         :param include_active: Whether to include the active compute package or not.
         :type include_active: str
         :return: All compute packages as a json response.
         :rtype: :class:`flask.Response`
         """
-
         if limit is not None and skip is not None:
             limit = int(limit)
             skip = int(skip)
 
         include_active: bool = include_active == "true"
 
         result = self.statestore.list_compute_packages(limit, skip)
@@ -393,15 +391,14 @@
         """Create the checksum of the compute package.
 
         :param name: The name of the compute package.
         :type name: str
         :return: Success or failure boolean, message and the checksum.
         :rtype: bool, str, str
         """
-
         if name is None:
             name, message = self._get_compute_package_name()
             if name is None:
                 return False, message, ""
         file_path = os.path.join("/app/client/package/", name)  # TODO: make configurable, perhaps in config.py or package.py
         try:
             sum = str(sha(file_path))
@@ -414,15 +411,14 @@
         """Get the checksum of the compute package.
 
         :param name: The name of the compute package.
         :type name: str
         :return: The checksum as a json object.
         :rtype: :py:class:`flask.Response`
         """
-
         success, message, sum = self._create_checksum(name)
         if not success:
             return jsonify({"success": False, "message": message}), 404
         payload = {"checksum": sum}
 
         return jsonify(payload)
 
@@ -812,15 +808,14 @@
         :param model_id: The model id to get the model descendants for.
         :type model_id: str
         :param limit: The number of descendants to return.
         :type limit: str
         :return: The model descendants for the given model as a json response.
         :rtype: :class:`flask.Response`
         """
-
         if model_id is None:
             return jsonify({"success": False, "message": "No model id provided."})
 
         limit: int = int(limit) if limit is not None else 10
 
         response: list = self.statestore.get_model_descendants(model_id, limit)
 
@@ -864,16 +859,15 @@
                 combiners = None
 
             info = {
                 "reducer": reducer,
                 "combiners": combiners,
             }
             payload[id] = info
-        else:
-            return jsonify(payload)
+        return jsonify(payload)
 
     def get_round(self, round_id):
         """Get a round.
 
         :param round_id: The round id to get.
         :type round_id: str
         :return: The round as json response.
@@ -911,15 +905,14 @@
 
     def get_plot_data(self, feature=None):
         """Get plot data.
 
         :return: The plot data as json response.
         :rtype: :py:class:`flask.Response`
         """
-
         plot = Plot(self.control.statestore)
 
         try:
             valid_metrics = plot.fetch_valid_metrics()
             feature = feature or valid_metrics[0]
             box_plot = plot.create_box_plot(feature)
         except Exception as e:
@@ -938,15 +931,14 @@
         """Get combiners data.
 
         :param combiners: The combiners to get data for.
         :type combiners: list
         :return: The combiners data as json response.
         :rtype: :py:class:`flask.Response`
         """
-
         response = self.statestore.list_combiners_data(combiners)
 
         arr = []
 
         # order list by combiner name
         for element in response:
             obj = {
```

### Comparing `fedn-0.9.2/fedn/network/api/network.py` & `fedn-0.9.5/fedn/network/api/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
     def add_client(self, client):
         """Add a new client to the network.
 
         :param client: The client instance object
         :type client: dict
         :return: None
         """
-
         if self.get_client(client["name"]):
             return
 
         logger.info("adding client {}".format(client["name"]))
         self.statestore.set_client(client)
 
     def get_client(self, name):
```

### Comparing `fedn-0.9.2/fedn/network/api/server.py` & `fedn-0.9.5/fedn/network/api/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,17 @@
 import os
 
 from flask import Flask, jsonify, request
 
-from fedn.common.config import get_controller_config, get_modelstorage_config, get_network_config, get_statestore_config
+from fedn.common.config import get_controller_config
 from fedn.network.api.auth import jwt_auth_required
 from fedn.network.api.interface import API
 from fedn.network.api.v1 import _routes
-from fedn.network.controller.control import Control
-from fedn.network.storage.statestore.mongostatestore import MongoStateStore
+from fedn.network.api.shared import statestore, control
 
-statestore_config = get_statestore_config()
-network_id = get_network_config()
-modelstorage_config = get_modelstorage_config()
-statestore = MongoStateStore(network_id, statestore_config["mongo_config"])
-statestore.set_storage_backend(modelstorage_config)
-control = Control(statestore=statestore)
 
 custom_url_prefix = os.environ.get("FEDN_CUSTOM_URL_PREFIX", False)
 api = API(statestore, control)
 app = Flask(__name__)
 for bp in _routes:
     app.register_blueprint(bp)
     if custom_url_prefix:
@@ -101,15 +94,14 @@
     limit: The maximum number of models to return.
     type: limit: int
     param: skip: The number of models to skip.
     type: skip: int
     Returns:
         _type_: json
     """
-
     session_id = request.args.get("session_id", None)
     limit = request.args.get("limit", None)
     skip = request.args.get("skip", None)
     include_active = request.args.get("include_active", None)
 
     return api.get_models(session_id, limit, skip, include_active)
 
@@ -157,15 +149,14 @@
 @app.route("/list_clients", methods=["GET"])
 @jwt_auth_required(role="admin")
 def list_clients():
     """Get all clients from the statestore.
     return: All clients as a json object.
     rtype: json
     """
-
     limit = request.args.get("limit", None)
     skip = request.args.get("skip", None)
     status = request.args.get("status", None)
 
     return api.get_clients(limit, skip, status)
 
 
@@ -198,15 +189,14 @@
 @app.route("/list_combiners", methods=["GET"])
 @jwt_auth_required(role="admin")
 def list_combiners():
     """Get all combiners in the network.
     return: All combiners as a json object.
     rtype: json
     """
-
     limit = request.args.get("limit", None)
     skip = request.args.get("skip", None)
 
     return api.get_all_combiners(limit, skip)
 
 
 if custom_url_prefix:
@@ -385,15 +375,14 @@
 @app.route("/list_compute_packages", methods=["GET"])
 @jwt_auth_required(role="admin")
 def list_compute_packages():
     """Get the compute package from the statestore.
     return: The compute package as a json object.
     rtype: json
     """
-
     limit = request.args.get("limit", None)
     skip = request.args.get("skip", None)
     include_active = request.args.get("include_active", None)
 
     return api.list_compute_packages(limit=limit, skip=skip, include_active=include_active)
 
 
@@ -592,15 +581,14 @@
 @app.route("/add_client", methods=["POST"])
 @jwt_auth_required(role="client")
 def add_client():
     """Add a client to the network.
     return: The response from control.
     rtype: json
     """
-
     json_data = request.get_json()
     remote_addr = request.remote_addr
     try:
         response = api.add_client(**json_data, remote_addr=remote_addr)
     except TypeError as e:
         return jsonify({"success": False, "message": str(e)}), 400
     return response
@@ -613,15 +601,14 @@
 @app.route("/list_combiners_data", methods=["POST"])
 @jwt_auth_required(role="admin")
 def list_combiners_data():
     """List data from combiners.
     return: The response from control.
     rtype: json
     """
-
     json_data = request.get_json()
 
     # expects a list of combiner names (strings) in an array
     combiners = json_data.get("combiners", None)
 
     try:
         response = api.list_combiners_data(combiners)
@@ -636,15 +623,14 @@
 
 @app.route("/get_plot_data", methods=["GET"])
 @jwt_auth_required(role="admin")
 def get_plot_data():
     """Get plot data from the statestore.
     rtype: json
     """
-
     try:
         feature = request.args.get("feature", None)
         response = api.get_plot_data(feature=feature)
     except TypeError as e:
         return jsonify({"success": False, "message": str(e)}), 400
     return response
```

### Comparing `fedn-0.9.2/fedn/network/api/tests.py` & `fedn-0.9.5/fedn/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/__init__.py` & `fedn-0.9.5/fedn/network/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/client_routes.py` & `fedn-0.9.5/fedn/network/api/v1/client_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/combiner_routes.py` & `fedn-0.9.5/fedn/network/api/v1/combiner_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/model_routes.py` & `fedn-0.9.5/fedn/network/api/v1/model_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import io
 
 import numpy as np
 from flask import Blueprint, jsonify, request, send_file
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import api_version, get_limit, get_post_data_to_kwargs, get_reverse, get_typed_list_headers, mdb, modelstorage_config
+from fedn.network.api.v1.shared import api_version, get_limit, get_post_data_to_kwargs, get_reverse, get_typed_list_headers, mdb
+from fedn.network.api.shared import modelstorage_config
 from fedn.network.storage.s3.base import RepositoryBase
 from fedn.network.storage.s3.miniorepository import MINIORepository
 from fedn.network.storage.statestore.stores.model_store import ModelStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("model", __name__, url_prefix=f"/api/{api_version}/models")
```

### Comparing `fedn-0.9.2/fedn/network/api/v1/package_routes.py` & `fedn-0.9.5/fedn/network/api/v1/package_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/round_routes.py` & `fedn-0.9.5/fedn/network/api/v1/round_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/session_routes.py` & `fedn-0.9.5/fedn/network/api/v1/session_routes.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,17 @@
+import threading
+
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
 from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, mdb
 from fedn.network.storage.statestore.stores.session_store import SessionStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
+from .model_routes import model_store
+from fedn.network.api.shared import control
 
 bp = Blueprint("session", __name__, url_prefix=f"/api/{api_version}/sessions")
 
 session_store = SessionStore(mdb, "control.sessions")
 
 
 @bp.route("/", methods=["GET"])
@@ -300,7 +304,87 @@
         response = session
 
         return jsonify(response), 200
     except EntityNotFound as e:
         return jsonify({"message": str(e)}), 404
     except Exception as e:
         return jsonify({"message": str(e)}), 500
+
+
+@bp.route("/", methods=["POST"])
+@jwt_auth_required(role="admin")
+def post():
+    """Create session
+    Creates a new session based on the provided data.
+    ---
+    tags:
+        - Sessions
+    parameters:
+      - name: session
+        in: body
+        required: true
+        schema:
+          type: object
+          properties:
+            session_id:
+              type: string
+            session_config:
+              type: object
+    responses:
+        201:
+            description: The created session
+            schema:
+                $ref: '#/definitions/Session'
+        500:
+            description: An error occurred
+            schema:
+                type: object
+                properties:
+                    message:
+                        type: string
+    """
+    try:
+        data = request.json if request.headers["Content-Type"] == "application/json" else request.form.to_dict()
+        successful, result = session_store.add(data)
+        response = result
+        status_code: int = 201 if successful else 400
+
+        return jsonify(response), status_code
+    except Exception as e:
+        return jsonify({"message": str(e)}), 500
+
+
+@bp.route("/start", methods=["POST"])
+@jwt_auth_required(role="admin")
+def start_session():
+    """Start a new session.
+    param: session_id: The session id to start.
+    type: session_id: str
+    param: rounds: The number of rounds to run.
+    type: rounds: int
+    """
+    try:
+        data = request.json if request.headers["Content-Type"] == "application/json" else request.form.to_dict()
+        session_id: str = data.get("session_id")
+        rounds: int = data.get("rounds", "")
+
+        if not session_id or session_id == "":
+            return jsonify({"message": "Session ID is required"}), 400
+
+        if not rounds or rounds == "":
+            return jsonify({"message": "Rounds is required"}), 400
+
+        if not isinstance(rounds, int):
+            return jsonify({"message": "Rounds must be an integer"}), 400
+
+        session = session_store.get(session_id, use_typing=False)
+
+        session_config = session["session_config"]
+        model_id = session_config["model_id"]
+
+        _ = model_store.get(model_id, use_typing=False)
+
+        threading.Thread(target=control.start_session, args=(session_id, rounds)).start()
+
+        return jsonify({"message": "Session started"}), 200
+    except Exception as e:
+        return jsonify({"message": str(e)}), 500
```

### Comparing `fedn-0.9.2/fedn/network/api/v1/shared.py` & `fedn-0.9.5/fedn/network/api/v1/shared.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 from typing import Tuple
 
 import pymongo
 from pymongo.database import Database
 
-from fedn.common.config import get_modelstorage_config, get_network_config, get_statestore_config
+from fedn.network.api.shared import statestore_config, network_id
 
 api_version = "v1"
 
-statestore_config = get_statestore_config()
-modelstorage_config = get_modelstorage_config()
-network_id = get_network_config()
-
 mc = pymongo.MongoClient(**statestore_config["mongo_config"])
 mc.server_info()
 mdb: Database = mc[network_id]
 
 
 def is_positive_integer(s):
     return s is not None and s.isdigit() and int(s) > 0
```

### Comparing `fedn-0.9.2/fedn/network/api/v1/status_routes.py` & `fedn-0.9.5/fedn/network/api/v1/status_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/api/v1/validation_routes.py` & `fedn-0.9.5/fedn/network/api/v1/validation_routes.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/clients/client.py` & `fedn-0.9.5/fedn/network/clients/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,14 @@
 
     def assign(self):
         """Contacts the controller and asks for combiner assignment.
 
         :return: A configuration dictionary containing connection information for combiner.
         :rtype: dict
         """
-
         logger.info("Initiating assignment request.")
         while True:
             status, response = self.connector.assign()
             if status == Status.TryAgain:
                 logger.warning(response)
                 logger.info("Assignment request failed. Retrying in 5 seconds.")
                 time.sleep(5)
@@ -175,18 +174,17 @@
 
     def connect(self, combiner_config):
         """Connect to combiner.
 
         :param combiner_config: connection information for the combiner.
         :type combiner_config: dict
         """
-
         if self._connected:
             logger.info("Client is already attached. ")
-            return None
+            return
 
         # TODO use the combiner_config['certificate'] for setting up secure comms'
         host = combiner_config["host"]
         # Add host to gRPC metadata
         self._add_grpc_metadata("grpc-server", host)
         logger.debug("Client using metadata: {}.".format(self.metadata))
         port = combiner_config["port"]
@@ -253,26 +251,24 @@
 
         :param combiner_config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         :type combiner_config: dict
         :return:
         """
-
         if "helper_type" in combiner_config.keys():
             self.helper = get_helper(combiner_config["helper_type"])
 
     def _subscribe_to_combiner(self, config):
         """Listen to combiner message stream and start all processing threads.
 
         :param config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         """
-
         # Start sending heartbeats to the combiner.
         threading.Thread(target=self._send_heartbeat, kwargs={"update_frequency": config["heartbeat_interval"]}, daemon=True).start()
 
         # Start listening for combiner training and validation messages
         threading.Thread(target=self._listen_to_task_stream, daemon=True).start()
         self._connected = True
 
@@ -416,15 +412,14 @@
 
     def _listen_to_task_stream(self):
         """Subscribe to the model update request stream.
 
         :return: None
         :rtype: None
         """
-
         r = fedn.ClientAvailableMessage()
         r.sender.name = self.name
         r.sender.role = fedn.WORKER
         # Add client to metadata
         self._add_grpc_metadata("client", self.name)
 
         while self._connected:
@@ -457,19 +452,19 @@
                     logger.warning("GRPC TaskStream: server unavailable during model update request stream. Retrying.")
                     # Retry after a delay
                     time.sleep(5)
                 if status_code == grpc.StatusCode.UNAUTHENTICATED:
                     details = e.details()
                     if details == "Token expired":
                         logger.warning("GRPC TaskStream: Token expired. Reconnecting.")
-                        self.detach()
+                        self.disconnect()
 
                 if status_code == grpc.StatusCode.CANCELLED:
-                    # Expected if the client is detached
-                    logger.critical("GRPC TaskStream: Client detached from combiner. Atempting to reconnect.")
+                    # Expected if the client is disconnected
+                    logger.critical("GRPC TaskStream: Client disconnected from combiner. Trying to reconnect.")
 
                 else:
                     # Log the error and continue
                     logger.error(f"GRPC TaskStream: An error occurred during model update request stream: {e}")
 
             except Exception as ex:
                 # Handle other exceptions
@@ -485,15 +480,14 @@
         :param model_id: The model id of the model to be updated.
         :type model_id: str
         :param session_id: The id of the current session
         :type session_id: str
         :return: The model id of the updated model, or None if the update failed. And a dict with metadata.
         :rtype: tuple
         """
-
         self.send_status("\t Starting processing of training request for model_id {}".format(model_id), sesssion_id=session_id)
         self.state = ClientState.training
 
         try:
             meta = {}
             tic = time.time()
             mdl = self.get_model_from_combiner(str(model_id))
@@ -692,15 +686,15 @@
                 logger.critical(f"GRPC process_request: An error occurred during process request: {e}")
 
     def _send_heartbeat(self, update_frequency=2.0):
         """Send a heartbeat to the combiner.
 
         :param update_frequency: The frequency of the heartbeat in seconds.
         :type update_frequency: float
-        :return: None if the client is detached.
+        :return: None if the client is disconnected.
         :rtype: None
         """
         while True:
             heartbeat = fedn.Heartbeat(sender=fedn.Client(name=self.name, role=fedn.WORKER))
             try:
                 self.connectorStub.SendHeartbeat(heartbeat, metadata=self.metadata)
                 self._missed_heartbeat = 0
@@ -736,15 +730,14 @@
         :param log_level: The log level of the message.
         :type log_level: fedn.Status.INFO, fedn.Status.WARNING, fedn.Status.ERROR
         :param type: The type of the message.
         :type type: str
         :param request: The request message.
         :type request: fedn.Request
         """
-
         if not self._connected:
             logger.info("SendStatus: Client disconnected.")
             return
 
         status = fedn.Status()
         status.timestamp.GetCurrentTime()
         status.sender.name = self.name
```

### Comparing `fedn-0.9.2/fedn/network/clients/connect.py` & `fedn-0.9.5/fedn/network/clients/connect.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,16 +63,15 @@
             self.connect_string = "{}{}:{}".format(self.prefix, self.host, self.port)
         else:
             self.connect_string = "{}{}".format(self.prefix, self.host)
 
         logger.info("Setting connection string to {}.".format(self.connect_string))
 
     def assign(self):
-        """
-        Connect client to FEDn network discovery service, ask for combiner assignment.
+        """Connect client to FEDn network discovery service, ask for combiner assignment.
 
         :return: Tuple with assingment status, combiner connection information if sucessful, else None.
         :rtype: tuple(:class:`fedn.network.clients.connect.Status`, str)
         """
         try:
             retval = None
             payload = {"client_id": self.name, "preferred_combiner": self.preferred_combiner}
@@ -123,16 +122,15 @@
                 return Status.UnMatchedConfig, reason
 
             return Status.Assigned, retval.json()
 
         return Status.Unassigned, None
 
     def refresh_token(self):
-        """
-        Refresh client token.
+        """Refresh client token.
 
         :return: Tuple with assingment status, combiner connection information if sucessful, else None.
         :rtype: tuple(:class:`fedn.network.clients.connect.Status`, str)
         """
         if not FEDN_AUTH_REFRESH_TOKEN_URI or not FEDN_AUTH_REFRESH_TOKEN:
             logger.error("No refresh token URI/Token set, cannot refresh token.")
             return 401
```

### Comparing `fedn-0.9.2/fedn/network/clients/package.py` & `fedn-0.9.5/fedn/network/clients/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
         try:
             if f:
                 f.extractall(self.pkg_path)
                 logger.info("Successfully extracted compute package content in {}".format(self.pkg_path))
                 # delete the tarball
                 logger.info("Deleting temporary package tarball file.")
+                f.close()
                 os.remove(os.path.join(self.pkg_path, self.pkg_name))
                 # search for file fedn.yaml in extracted package
                 for root, dirs, files in os.walk(self.pkg_path):
                     if "fedn.yaml" in files:
                         # Get the path to where fedn.yaml is located
                         logger.info("Found fedn.yaml file in {}".format(root))
                         return True, root
@@ -149,12 +150,11 @@
         """Dispatch the compute package
 
         :param run_path: path to dispatch the compute package
         :type run_path: str
         :return: Dispatcher object
         :rtype: :class:`fedn.utils.dispatcher.Dispatcher`
         """
-
         self.dispatch_config = _read_yaml_file(os.path.join(run_path, "fedn.yaml"))
         dispatcher = Dispatcher(self.dispatch_config, run_path)
 
         return dispatcher
```

### Comparing `fedn-0.9.2/fedn/network/clients/state.py` & `fedn-0.9.5/fedn/network/clients/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/clients/test_client.py` & `fedn-0.9.5/fedn/network/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/combiner/aggregators/aggregatorbase.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/aggregatorbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,16 +82,16 @@
         """ Validate the model update.
 
         :param model_update: A ModelUpdate message.
         :type model_update: object
         :return: True if the model update is valid, False otherwise.
         :rtype: bool
         """
-        data = json.loads(model_update.meta)['training_metadata']
-        if 'num_examples' not in data.keys():
+        data = json.loads(model_update.meta)["training_metadata"]
+        if "num_examples" not in data.keys():
             logger.error("AGGREGATOR({}): Model validation failed, num_examples missing in metadata.".format(self.name))
             return False
         return True
 
     def next_model_update(self):
         """ Get the next model update from the queue.
 
@@ -116,29 +116,29 @@
         :return: A tuple of (parameters, metadata)
         :rtype: tuple
         """
         model_id = model_update.model_update_id
         model = self.round_handler.load_model_update(helper, model_id)
         # Get relevant metadata
         metadata = json.loads(model_update.meta)
-        if 'config' in metadata.keys():
+        if "config" in metadata.keys():
             # Used in Python client
-            config = json.loads(metadata['config'])
+            config = json.loads(metadata["config"])
         else:
             # Used in C++ client
             config = json.loads(model_update.config)
-        training_metadata = metadata['training_metadata']
-        training_metadata['round_id'] = config['round_id']
+        training_metadata = metadata["training_metadata"]
+        training_metadata["round_id"] = config["round_id"]
 
         return model, training_metadata
 
     def get_state(self):
         """ Get the state of the aggregator's queue, including the number of model updates."""
         state = {
-            'queue_len': self.model_updates.qsize()
+            "queue_len": self.model_updates.qsize()
         }
         return state
 
 
 def get_aggregator(aggregator_module_name, storage, server, modelservice, control):
     """ Return an instance of the helper class.
```

### Comparing `fedn-0.9.2/fedn/network/combiner/aggregators/fedavg.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/fedavg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
+import traceback
+
 from fedn.common.log_config import logger
 from fedn.network.combiner.aggregators.aggregatorbase import AggregatorBase
 
 
 class Aggregator(AggregatorBase):
-    """ Local SGD / Federated Averaging (FedAvg) aggregator. Computes a weighted mean
+    """Local SGD / Federated Averaging (FedAvg) aggregator. Computes a weighted mean
         of parameter updates.
 
     :param id: A reference to id of :class: `fedn.network.combiner.Combiner`
     :type id: str
     :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
     :type storage: class: `fedn.common.storage.s3.s3repo.S3ModelRepository`
     :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
@@ -17,15 +19,14 @@
     :param control: A handle to the :class: `fedn.network.combiner.roundhandler.RoundHandler`
     :type control: class: `fedn.network.combiner.roundhandler.RoundHandler`
 
     """
 
     def __init__(self, storage, server, modelservice, round_handler):
         """Constructor method"""
-
         super().__init__(storage, server, modelservice, round_handler)
 
         self.name = "fedavg"
 
     def combine_models(self, helper=None, delete_models=True, parameters=None):
         """Aggregate all model updates in the queue by computing an incremental
         weighted average of model parameters.
@@ -37,57 +38,53 @@
         :param max_nr_models: The maximum number of updates aggregated, defaults to 100
         :type max_nr_models: int, optional
         :param delete_models: Delete models from storage after aggregation, defaults to True
         :type delete_models: bool, optional
         :return: The global model and metadata
         :rtype: tuple
         """
-
         data = {}
-        data['time_model_load'] = 0.0
-        data['time_model_aggregation'] = 0.0
+        data["time_model_load"] = 0.0
+        data["time_model_aggregation"] = 0.0
 
         model = None
         nr_aggregated_models = 0
         total_examples = 0
 
-        logger.info(
-            "AGGREGATOR({}): Aggregating model updates... ".format(self.name))
+        logger.info("AGGREGATOR({}): Aggregating model updates... ".format(self.name))
 
         while not self.model_updates.empty():
             try:
                 # Get next model from queue
                 logger.info("AGGREGATOR({}): Getting next model update from queue.".format(self.name))
                 model_update = self.next_model_update()
 
                 # Load model parameters and metadata
                 logger.info("AGGREGATOR({}): Loading model metadata {}.".format(self.name, model_update.model_update_id))
                 model_next, metadata = self.load_model_update(model_update, helper)
 
-                logger.info(
-                    "AGGREGATOR({}): Processing model update {}, metadata: {}  ".format(self.name, model_update.model_update_id, metadata))
+                logger.info("AGGREGATOR({}): Processing model update {}, metadata: {}  ".format(self.name, model_update.model_update_id, metadata))
 
                 # Increment total number of examples
-                total_examples += metadata['num_examples']
+                total_examples += metadata["num_examples"]
 
                 if nr_aggregated_models == 0:
                     model = model_next
                 else:
-                    model = helper.increment_average(
-                        model, model_next, metadata['num_examples'], total_examples)
+                    model = helper.increment_average(model, model_next, metadata["num_examples"], total_examples)
 
                 nr_aggregated_models += 1
                 # Delete model from storage
                 if delete_models:
                     self.modelservice.temp_model_storage.delete(model_update.model_update_id)
-                    logger.info(
-                        "AGGREGATOR({}): Deleted model update {} from storage.".format(self.name, model_update.model_update_id))
+                    logger.info("AGGREGATOR({}): Deleted model update {} from storage.".format(self.name, model_update.model_update_id))
                 self.model_updates.task_done()
             except Exception as e:
-                logger.error(
-                    "AGGREGATOR({}): Error encoutered while processing model update {}, skipping this update.".format(self.name, e))
+                tb = traceback.format_exc()
+                logger.error(f"AGGREGATOR({self.name}): Error encoutered while processing model update: {e}")
+                logger.error(tb)
                 self.model_updates.task_done()
 
-        data['nr_aggregated_models'] = nr_aggregated_models
+        data["nr_aggregated_models"] = nr_aggregated_models
 
         logger.info("AGGREGATOR({}): Aggregation completed, aggregated {} models.".format(self.name, nr_aggregated_models))
         return model, data
```

### Comparing `fedn-0.9.2/fedn/network/combiner/aggregators/fedopt.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/fedopt.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,41 +51,40 @@
         :param delete_models: Delete models from storage after aggregation, defaults to True
         :type delete_models: bool, optional
         :param parameters: Aggregator hyperparameters.
         :type parameters: `fedn.utils.parmeters.Parameters`, optional
         :return: The global model and metadata
         :rtype: tuple
         """
-
         data = {}
-        data['time_model_load'] = 0.0
-        data['time_model_aggregation'] = 0.0
+        data["time_model_load"] = 0.0
+        data["time_model_aggregation"] = 0.0
 
         # Define parameter schema
         parameter_schema = {
-            'serveropt': str,
-            'learning_rate': float,
-            'beta1': float,
-            'beta2': float,
-            'tau': float,
+            "serveropt": str,
+            "learning_rate": float,
+            "beta1": float,
+            "beta2": float,
+            "tau": float,
         }
 
         try:
             parameters.validate(parameter_schema)
         except InvalidParameterError as e:
             logger.error("Aggregator {} recieved invalid parameters. Reason {}".format(self.name, e))
             return None, data
 
         # Default hyperparameters. Note that these may need fine tuning.
         default_parameters = {
-            'serveropt': 'adam',
-            'learning_rate': 1e-3,
-            'beta1': 0.9,
-            'beta2': 0.99,
-            'tau': 1e-4,
+            "serveropt": "adam",
+            "learning_rate": 1e-3,
+            "beta1": 0.9,
+            "beta2": 0.99,
+            "tau": 1e-4,
         }
 
         # Validate parameters
         if parameters:
             try:
                 parameters.validate(parameter_schema)
             except InvalidParameterError as e:
@@ -115,47 +114,47 @@
                 # Load model paratmeters and metadata
                 model_next, metadata = self.load_model_update(model_update, helper)
 
                 logger.info(
                     "AGGREGATOR({}): Processing model update {}".format(self.name, model_update.model_update_id))
 
                 # Increment total number of examples
-                total_examples += metadata['num_examples']
+                total_examples += metadata["num_examples"]
 
                 if nr_aggregated_models == 0:
                     model_old = self.round_handler.load_model_update(helper, model_update.model_id)
                     pseudo_gradient = helper.subtract(model_next, model_old)
                 else:
                     pseudo_gradient_next = helper.subtract(model_next, model_old)
                     pseudo_gradient = helper.increment_average(
-                        pseudo_gradient, pseudo_gradient_next, metadata['num_examples'], total_examples)
+                        pseudo_gradient, pseudo_gradient_next, metadata["num_examples"], total_examples)
 
                 nr_aggregated_models += 1
                 # Delete model from storage
                 if delete_models:
                     self.modelservice.temp_model_storage.delete(model_update.model_update_id)
                     logger.info(
                         "AGGREGATOR({}): Deleted model update {} from storage.".format(self.name, model_update.model_update_id))
                 self.model_updates.task_done()
             except Exception as e:
                 logger.error(
                     "AGGREGATOR({}): Error encoutered while processing model update {}, skipping this update.".format(self.name, e))
                 self.model_updates.task_done()
 
-        if parameters['serveropt'] == 'adam':
+        if parameters["serveropt"] == "adam":
             model = self.serveropt_adam(helper, pseudo_gradient, model_old, parameters)
-        elif parameters['serveropt'] == 'yogi':
+        elif parameters["serveropt"] == "yogi":
             model = self.serveropt_yogi(helper, pseudo_gradient, model_old, parameters)
-        elif parameters['serveropt'] == 'adagrad':
+        elif parameters["serveropt"] == "adagrad":
             model = self.serveropt_adagrad(helper, pseudo_gradient, model_old, parameters)
         else:
             logger.error("Unsupported server optimizer passed to FedOpt.")
             return None, data
 
-        data['nr_aggregated_models'] = nr_aggregated_models
+        data["nr_aggregated_models"] = nr_aggregated_models
 
         logger.info("AGGREGATOR({}): Aggregation completed, aggregated {} models.".format(self.name, nr_aggregated_models))
         return model, data
 
     def serveropt_adam(self, helper, pseudo_gradient, model_old, parameters):
         """ Server side optimization, FedAdam.
 
@@ -166,18 +165,18 @@
         :param model_old: The current global model.
         :type model_old: As defined in helper.
         :param parameters: Hyperparamters for the aggregator.
         :type parameters: dict
         :return: new model weights.
         :rtype: as defined by helper.
         """
-        beta1 = parameters['beta1']
-        beta2 = parameters['beta2']
-        learning_rate = parameters['learning_rate']
-        tau = parameters['tau']
+        beta1 = parameters["beta1"]
+        beta2 = parameters["beta2"]
+        learning_rate = parameters["learning_rate"]
+        tau = parameters["tau"]
 
         if not self.v:
             self.v = helper.ones(pseudo_gradient, math.pow(tau, 2))
 
         if not self.m:
             self.m = helper.multiply(pseudo_gradient, [(1.0-beta1)]*len(pseudo_gradient))
         else:
@@ -202,19 +201,18 @@
         :param model_old: The current global model.
         :type model_old: As defined in helper.
         :param parameters: Hyperparamters for the aggregator.
         :type parameters: dict
         :return: new model weights.
         :rtype: as defined by helper.
         """
-
-        beta1 = parameters['beta1']
-        beta2 = parameters['beta2']
-        learning_rate = parameters['learning_rate']
-        tau = parameters['tau']
+        beta1 = parameters["beta1"]
+        beta2 = parameters["beta2"]
+        learning_rate = parameters["learning_rate"]
+        tau = parameters["tau"]
 
         if not self.v:
             self.v = helper.ones(pseudo_gradient, math.pow(tau, 2))
 
         if not self.m:
             self.m = helper.multiply(pseudo_gradient, [(1.0-beta1)]*len(pseudo_gradient))
         else:
@@ -241,18 +239,17 @@
         :param model_old: The current global model.
         :type model_old: As defined in helper.
         :param parameters: Hyperparamters for the aggregator.
         :type parameters: dict
         :return: new model weights.
         :rtype: as defined by helper.
         """
-
-        beta1 = parameters['beta1']
-        learning_rate = parameters['learning_rate']
-        tau = parameters['tau']
+        beta1 = parameters["beta1"]
+        learning_rate = parameters["learning_rate"]
+        tau = parameters["tau"]
 
         if not self.v:
             self.v = helper.ones(pseudo_gradient, math.pow(tau, 2))
 
         if not self.m:
             self.m = helper.multiply(pseudo_gradient, [(1.0-beta1)]*len(pseudo_gradient))
         else:
```

### Comparing `fedn-0.9.2/fedn/network/combiner/aggregators/tests/test_fedavg.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/tests/test_fedavg.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/combiner/combiner.py` & `fedn-0.9.5/fedn/network/combiner/combiner.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,22 +55,20 @@
 
     :param config: configuration for the combiner
     :type config: dict
     """
 
     def __init__(self, config):
         """Initialize Combiner server."""
-
         set_log_level_from_string(config.get("verbosity", "INFO"))
         set_log_stream(config.get("logfile", None))
 
         # Client queues
         self.clients = {}
 
-        self.modelservice = ModelService()
 
         # Validate combiner name
         match = re.search(VALID_NAME_REGEX, config["name"])
         if not match:
             raise ValueError("Unallowed character in combiner name. Allowed characters: a-z, A-Z, 0-9, _, -.")
 
         self.id = config["name"]
@@ -119,14 +117,25 @@
         # Set up gRPC server configuration
         grpc_config = {"port": config["port"], "secure": config["secure"], "certificate": cert, "key": key}
 
         # Set up model repository
         self.repository = Repository(announce_config["storage"]["storage_config"])
 
         self.statestore = MongoStateStore(announce_config["statestore"]["network_id"], announce_config["statestore"]["mongo_config"])
+
+        # Fetch all clients previously connected to the combiner
+        # If a client and a combiner goes down at the same time,
+        # the client will be stuck listed as "online" in the statestore.
+        # Set the status to offline for previous clients.
+        previous_clients = self.statestore.clients.find({"combiner": config["name"]})
+        for client in previous_clients:
+            self.statestore.set_client({"name": client["name"], "status": "offline"})
+
+        self.modelservice = ModelService()
+
         # Create gRPC server
         self.server = Server(self, self.modelservice, grpc_config)
 
         # Set up round controller
         self.round_handler = RoundHandler(self.repository, self, self.modelservice)
 
         # Start thread for round controller
@@ -323,28 +332,26 @@
             then = self.clients[client]["lastseen"]
             if (now - then) < timedelta(seconds=10):
                 clients["active_clients"].append(client)
                 # If client has changed status, update statestore
                 if status != "online":
                     self.clients[client]["status"] = "online"
                     clients["update_active_clients"].append(client)
-            else:
-                # If client has changed status, update statestore
-                if status == "online":
-                    self.clients[client]["status"] = "offline"
-                    clients["update_offline_clients"].append(client)
+            elif status != "offline":
+                self.clients[client]["status"] = "offline"
+                clients["update_offline_clients"].append(client)
         # Update statestore with client status
         if len(clients["update_active_clients"]) > 0:
             self.statestore.update_client_status(clients["update_active_clients"], "online")
         if len(clients["update_offline_clients"]) > 0:
             self.statestore.update_client_status(clients["update_offline_clients"], "offline")
 
         return clients["active_clients"]
 
-    def _deamon_thread_client_status(self, timeout=10):
+    def _deamon_thread_client_status(self, timeout=5):
         """Deamon thread that checks for inactive clients and updates statestore."""
         while True:
             time.sleep(timeout)
             # TODO: Also update validation clients
             self._list_active_clients(fedn.Queue.TASK_QUEUE)
 
     def _put_request_to_client_queue(self, request, queue_name):
@@ -365,23 +372,21 @@
 
     def _send_status(self, status):
         """Report a status to backend db.
 
         :param status: the status to report
         :type status: :class:`fedn.network.grpc.fedn_pb2.Status`
         """
-
         self.statestore.report_status(status)
 
     def _flush_model_update_queue(self):
         """Clear the model update queue (aggregator).
 
         :return: True if successful, else False
         """
-
         q = self.round_handler.aggregator.model_updates
         try:
             with q.mutex:
                 q.queue.clear()
                 q.all_tasks_done.notify_all()
                 q.unfinished_tasks = 0
             return True
@@ -584,15 +589,14 @@
         """A server stream RPC endpoint (Update model). Messages from client stream.
 
         :param response: the response
         :type response: :class:`fedn.network.grpc.fedn_pb2.ModelUpdateRequest`
         :param context: the context
         :type context: :class:`grpc._server._Context`
         """
-
         client = response.sender
         metadata = context.invocation_metadata()
         if metadata:
             metadata = dict(metadata)
             logger.info("grpc.Combiner.TaskStream: Client connected: {}\n".format(metadata["client"]))
 
         status = fedn.Status(status="Client {} connecting to TaskStream.".format(client.name))
@@ -602,14 +606,18 @@
         self.__whoami(status.sender, self)
 
         self._subscribe_client_to_queue(client, fedn.Queue.TASK_QUEUE)
         q = self.__get_queue(client, fedn.Queue.TASK_QUEUE)
 
         self._send_status(status)
 
+        # Set client status to online
+        self.clients[client.name]["status"] = "online"
+        self.statestore.set_client({"name": client.name, "status": "online"})
+
         # Keep track of the time context has been active
         start_time = time.time()
         while context.is_active():
             # Check if the context has been active for more than 10 seconds
             if time.time() - start_time > 10:
                 self.clients[client.name]["lastseen"] = datetime.now()
                 # Reset the start time
@@ -639,15 +647,14 @@
 
     def register_model_validation(self, validation):
         """Register a model validation.
 
         :param validation: the model validation
         :type validation: :class:`fedn.network.grpc.fedn_pb2.ModelValidation`
         """
-
         self.statestore.report_validation(validation)
 
     def SendModelValidation(self, request, context):
         """Send a model validation response.
 
         :param request: the request
         :type request: :class:`fedn.network.grpc.fedn_pb2.ModelValidation`
@@ -664,15 +671,14 @@
         response.response = "RECEIVED ModelValidation {} from client  {}".format(response, response.sender.name)
         return response
 
     ####################################################################################################################
 
     def run(self):
         """Start the server."""
-
         logger.info("COMBINER: {} started, ready for gRPC requests.".format(self.id))
         try:
             while True:
                 signal.pause()
         except (KeyboardInterrupt, SystemExit):
             pass
         self.server.stop()
```

### Comparing `fedn-0.9.2/fedn/network/combiner/connect.py` & `fedn-0.9.5/fedn/network/combiner/connect.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,15 +63,14 @@
         :param name: The name of the combiner.
         :type name: str
         :param secure: Use https for the connection to the discovery service.
         :type secure: bool
         :param verify: Verify the connection to the discovery service.
         :type verify: bool
         """
-
         self.host = host
         self.fqdn = fqdn
         self.port = port
         self.myhost = myhost
         self.myport = myport
         self.token = token
         self.token_scheme = os.environ.get("FEDN_AUTH_SCHEME", "Bearer")
@@ -88,16 +87,15 @@
             self.connect_string = "{}{}:{}".format(self.prefix, self.host, self.port)
         else:
             self.connect_string = "{}{}".format(self.prefix, self.host)
 
         logger.info("Setting connection string to {}".format(self.connect_string))
 
     def announce(self):
-        """
-        Announce combiner to FEDn network via discovery service (REST-API).
+        """Announce combiner to FEDn network via discovery service (REST-API).
 
         :return: Tuple with announcement Status, FEDn network configuration if sucessful, else None.
         :rtype: :class:`fedn.network.combiner.connect.Status`, str
         """
         payload = {"combiner_id": self.name, "address": self.myhost, "fqdn": self.fqdn, "port": self.myport, "secure_grpc": self.secure}
         url_prefix = os.environ.get("FEDN_CUSTOM_URL_PREFIX", "")
         try:
```

### Comparing `fedn-0.9.2/fedn/network/combiner/interfaces.py` & `fedn-0.9.5/fedn/network/combiner/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,14 @@
 
     def to_dict(self):
         """Export combiner configuration to a dictionary.
 
         :return: A dictionary with the combiner configuration.
         :rtype: dict
         """
-
         data = {
             "parent": self.parent,
             "name": self.name,
             "address": self.address,
             "fqdn": self.fqdn,
             "port": self.port,
             "ip": self.ip,
@@ -164,15 +163,14 @@
             key_b64 = base64.b64encode(self.key)
             return str(key_b64).split("'")[1]
         else:
             return None
 
     def flush_model_update_queue(self):
         """Reset the model update queue on the combiner."""
-
         channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ControlStub(channel)
 
         request = fedn.ControlRequest()
 
         try:
             control.FlushAggregationQueue(request)
@@ -184,15 +182,14 @@
 
     def set_aggregator(self, aggregator):
         """Set the active aggregator module.
 
         :param aggregator: The name of the aggregator module.
         :type config: str
         """
-
         channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ControlStub(channel)
 
         request = fedn.ControlRequest()
         p = request.parameter.add()
         p.key = "aggregator"
         p.value = aggregator
@@ -236,15 +233,14 @@
         """Download a model from the combiner server.
 
         :param id: The model id.
         :type id: str
         :return: A file-like object containing the model.
         :rtype: :class:`io.BytesIO`, None if the model is not available.
         """
-
         channel = Channel(self.address, self.port, self.certificate).get_channel()
         modelservice = rpc.ModelServiceStub(channel)
 
         data = BytesIO()
         data.seek(0, 0)
 
         time_start = time.time()
```

### Comparing `fedn-0.9.2/fedn/network/combiner/modelservice.py` & `fedn-0.9.5/fedn/network/combiner/modelservice.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,14 @@
         """Download model with id 'id' from server.
 
         :param id: The model id.
         :type id: str
         :return: A BytesIO object containing the model.
         :rtype: :class:`io.BytesIO`, None if model does not exist.
         """
-
         data = BytesIO()
         data.seek(0, 0)
 
         parts = self.Download(fedn.ModelRequest(id=id), self)
         for part in parts:
             if part.status == fedn.ModelStatus.IN_PROGRESS:
                 data.write(part.data)
```

### Comparing `fedn-0.9.2/fedn/network/combiner/roundhandler.py` & `fedn-0.9.5/fedn/network/combiner/roundhandler.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     :type server: class: `fedn.network.combiner.Combiner`
     :param modelservice: A handle to the model service :class: `fedn.network.combiner.modelservice.ModelService`
     :type modelservice: class: `fedn.network.combiner.modelservice.ModelService`
     """
 
     def __init__(self, storage, server, modelservice):
         """Initialize the RoundHandler."""
-
         self.round_configs = queue.Queue()
         self.storage = storage
         self.server = server
         self.modelservice = modelservice
 
     def set_aggregator(self, aggregator):
         self.aggregator = get_aggregator(aggregator, self.storage, self.server, self.modelservice, self)
@@ -63,15 +62,14 @@
         """Load model update with id model_id into its memory representation.
 
         :param helper: An instance of :class: `fedn.utils.helpers.helpers.HelperBase`
         :type helper: class: `fedn.utils.helpers.helpers.HelperBase`
         :param model_id: The ID of the model update, UUID in str format
         :type model_id: str
         """
-
         model_str = self.load_model_update_str(model_id)
         if model_str:
             try:
                 model = load_model_from_BytesIO(model_str.getbuffer(), helper)
             except IOError:
                 logger.warning("AGGREGATOR({}): Failed to load model!".format(self.name))
         else:
@@ -115,15 +113,14 @@
         :param config: The round config object
         :type config: dict
         :param buffer_size: The number of model updates to wait for before starting aggregation, defaults to 100
         :type buffer_size: int, optional
         :param polling_interval: The polling interval, defaults to 0.1
         :type polling_interval: float, optional
         """
-
         time_window = float(config["round_timeout"])
 
         tt = 0.0
         while tt < time_window:
             if self.aggregator.model_updates.qsize() >= buffer_size:
                 break
 
@@ -136,15 +133,14 @@
         :param config: The round config object (passed to the client).
         :type config: dict
         :param clients: clients to participate in the training round
         :type clients: list
         :return: an aggregated model and associated metadata
         :rtype: model, dict
         """
-
         logger.info("ROUNDHANDLER: Initiating training round, participating clients: {}".format(clients))
 
         meta = {}
         meta["nr_expected_updates"] = len(clients)
         meta["nr_required_updates"] = int(config["clients_required"])
         meta["timeout"] = float(config["round_timeout"])
 
@@ -204,15 +200,14 @@
         :param model_id: ID of the model update object to stage.
         :type model_id: str
         :param timeout_retry: Sleep before retrying download again(sec), defaults to 3
         :type timeout_retry: int, optional
         :param retry: Number of retries, defaults to 2
         :type retry: int, optional
         """
-
         # If the model is already in memory at the server we do not need to do anything.
         if self.modelservice.temp_model_storage.exist(model_id):
             logger.info("Model already exists in memory, skipping model staging.")
             return
         logger.info("Model Staging, fetching model from storage...")
         # If not, download it and stage it in memory at the combiner.
         tries = 0
@@ -237,15 +232,14 @@
         :param n: Size of a random set taken from active trainers(clients), if n > "active trainers" all is used
         :type n: int
         :param type: type of clients, either "trainers" or "validators", defaults to "trainers"
         :type type: str, optional
         :return: Set of clients
         :rtype: list
         """
-
         if type == "validators":
             clients = self.server.get_active_validators()
         elif type == "trainers":
             clients = self.server.get_active_trainers()
         else:
             logger.error("(ERROR): {} is not a supported type of client".format(type))
             raise
@@ -265,15 +259,14 @@
         :param config: The round config object.
         :type config: dict
         :param timeout: Timeout in seconds, defaults to 0.0
         :type timeout: float, optional
         :return: True if the required number of clients are available, False otherwise.
         :rtype: bool
         """
-
         active = self.server.nr_active_trainers()
         if active >= int(config["clients_required"]):
             logger.info("Number of clients required ({0}) to start round met {1}.".format(config["clients_required"], active))
             return True
         else:
             logger.info("Too few clients to start round.")
             return False
@@ -294,15 +287,14 @@
         """Coordinates clients to execute training tasks.
 
         :param config: The round config object.
         :type config: dict
         :return: metadata about the training round.
         :rtype: dict
         """
-
         logger.info("Processing training round,  job_id {}".format(config["_job_id"]))
 
         data = {}
         data["config"] = config
         data["round_id"] = config["round_id"]
 
         # Download model to update and set in temp storage.
```

### Comparing `fedn-0.9.2/fedn/network/controller/control.py` & `fedn-0.9.5/fedn/network/controller/control.py`

 * *Files 9% similar despite different names*

```diff
@@ -71,28 +71,80 @@
 
     :param statestore: A StateStorage instance.
     :type statestore: class: `fedn.network.statestorebase.StateStorageBase`
     """
 
     def __init__(self, statestore):
         """Constructor method."""
-
         super().__init__(statestore)
         self.name = "DefaultControl"
 
+    def start_session(self, session_id: str, rounds: int):
+        if self._state == ReducerState.instructing:
+            logger.info("Controller already in INSTRUCTING state. A session is in progress.")
+            return
+
+        if not self.statestore.get_latest_model():
+            logger.warning("No model in model chain, please provide a seed model!")
+            return
+
+        self._state = ReducerState.instructing
+
+        session = self.statestore.get_session(session_id)
+
+        if not session:
+            logger.error("Session not found.")
+            return
+
+        session_config = session["session_config"]
+
+        if not session_config or not isinstance(session_config, dict):
+            logger.error("Session not properly configured.")
+            return
+
+        self._state = ReducerState.monitoring
+
+        last_round = int(self.get_latest_round_id())
+
+        aggregator = session_config["aggregator"]
+
+        session_config["session_id"] = session_id
+
+        for combiner in self.network.get_combiners():
+            combiner.set_aggregator(aggregator)
+
+        self.set_session_status(session_id, "Started")
+
+        for round in range(1, rounds + 1):
+            if last_round:
+                current_round = last_round + round
+            else:
+                current_round = round
+
+            try:
+                _, round_data = self.round(session_config, str(current_round))
+            except TypeError as e:
+                logger.error("Failed to execute round: {0}".format(e))
+
+            logger.info("Round completed with status {}".format(round_data["status"]))
+
+            session_config["model_id"] = self.statestore.get_latest_model()
+
+        self.set_session_status(session_id, "Finished")
+        self._state = ReducerState.idle
+
     def session(self, config):
         """Execute a new training session. A session consists of one
             or several global rounds. All rounds in the same session
             have the same round_config.
 
         :param config: The session config.
         :type config: dict
 
         """
-
         if self._state == ReducerState.instructing:
             logger.info("Controller already in INSTRUCTING state. A session is in progress.")
             return
 
         if not self.statestore.get_latest_model():
             logger.warning("No model in model chain, please provide a seed model!")
             return
@@ -136,15 +188,14 @@
 
         : param session_config: The session config.
         : type session_config: dict
         : param round_id: The round id.
         : type round_id: str
 
         """
-
         self.create_round({"round_id": round_id, "status": "Pending"})
 
         if len(self.network.get_combiners()) < 1:
             logger.warning("Round cannot start, no combiners connected!")
             self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
@@ -271,15 +322,14 @@
 
     def reduce(self, combiners):
         """Combine updated models from Combiner nodes into one global model.
 
         : param combiners: dict of combiner names(key) and model IDs(value) to reduce
         : type combiners: dict
         """
-
         meta = {}
         meta["time_fetch_model"] = 0.0
         meta["time_load_model"] = 0.0
         meta["time_aggregate_model"] = 0.0
 
         i = 1
         model = None
@@ -318,15 +368,14 @@
         return model, meta
 
     def infer_instruct(self, config):
         """Main entrypoint for executing the inference compute plan.
 
         : param config: configuration for the inference round
         """
-
         # Check/set instucting state
         if self.__state == ReducerState.instructing:
             logger.info("Already set in INSTRUCTING state")
             return
         self.__state = ReducerState.instructing
 
         # Check for a model chain
@@ -346,15 +395,14 @@
         self.__state = ReducerState.idle
 
     def inference_round(self, config):
         """Execute an inference round.
 
         : param config: configuration for the inference round
         """
-
         # Init meta
         round_data = {}
 
         # Check for at least one combiner in statestore
         if len(self.network.get_combiners()) < 1:
             logger.warning("No combiners connected!")
             return round_data
```

### Comparing `fedn-0.9.2/fedn/network/controller/controlbase.py` & `fedn-0.9.5/fedn/network/controller/controlbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,25 +109,21 @@
         """
         if self._state == ReducerState.idle:
             return True
         else:
             return False
 
     def get_model_info(self):
-        """
-
-        :return:
+        """:return:
         """
         return self.statestore.get_model_trail()
 
     # TODO: remove use statestore.get_events() instead
     def get_events(self):
-        """
-
-        :return:
+        """:return:
         """
         return self.statestore.get_events()
 
     def get_latest_round_id(self):
         last_round = self.statestore.get_latest_round()
         if not last_round:
             return 0
@@ -135,17 +131,15 @@
             return last_round["round_id"]
 
     def get_latest_round(self):
         round = self.statestore.get_latest_round()
         return round
 
     def get_compute_package_name(self):
-        """
-
-        :return:
+        """:return:
         """
         definition = self.statestore.get_compute_package()
         if definition:
             try:
                 package_name = definition["storage_file_name"]
                 return package_name
             except (IndexError, KeyError):
@@ -155,29 +149,26 @@
             return None
 
     def set_compute_package(self, filename, path):
         """Persist the configuration for the compute package."""
         self.model_repository.set_compute_package(filename, path)
 
     def get_compute_package(self, compute_package=""):
-        """
-
-        :param compute_package:
+        """:param compute_package:
         :return:
         """
         if compute_package == "":
             compute_package = self.get_compute_package_name()
         if compute_package:
             return self.model_repository.get_compute_package(compute_package)
         else:
             return None
 
     def create_session(self, config, status="Initialized"):
         """Initialize a new session in backend db."""
-
         if "session_id" not in config.keys():
             session_id = uuid.uuid4()
             config["session_id"] = str(session_id)
         else:
             session_id = config["session_id"]
 
         self.statestore.create_session(id=session_id)
@@ -192,15 +183,14 @@
         :param status: The status
         :type status: str
         """
         self.statestore.set_session_status(session_id, status)
 
     def create_round(self, round_data):
         """Initialize a new round in backend db."""
-
         self.statestore.create_round(round_data)
 
     def set_round_data(self, round_id, round_data):
         """Set round data.
 
         :param round_id: The round unique identifier
         :type round_id: str
@@ -247,15 +237,14 @@
         :param model_id: Unique identifier for the model to commit.
         :type model_id: str (uuid)
         :param model: The model object to commit
         :type model: BytesIO
         :param session_id: Unique identifier for the session
         :type session_id: str
         """
-
         helper = self.get_helper()
         if model is not None:
             logger.info("Saving model file temporarily to disk...")
             outfile_name = helper.save(model)
             logger.info("CONTROL: Uploading model to Minio...")
             model_id = self.model_repository.set_model(outfile_name, is_file=True)
```

### Comparing `fedn-0.9.2/fedn/network/grpc/auth.py` & `fedn-0.9.5/fedn/network/grpc/auth.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/grpc/fedn_pb2.py` & `fedn-0.9.5/fedn/network/grpc/fedn_pb2.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/grpc/fedn_pb2_grpc.py` & `fedn-0.9.5/fedn/network/grpc/fedn_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/grpc/server.py` & `fedn-0.9.5/fedn/network/grpc/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from concurrent import futures
 
 import grpc
 from grpc_health.v1 import health, health_pb2_grpc
 
 import fedn.network.grpc.fedn_pb2_grpc as rpc
-from fedn.common.log_config import (logger, set_log_level_from_string,
-                                    set_log_stream)
+from fedn.common.log_config import logger, set_log_level_from_string, set_log_stream
 from fedn.network.grpc.auth import JWTInterceptor
 
 
 class Server:
     """ Class for configuring and launching the gRPC server."""
 
     def __init__(self, servicer, modelservicer, config):
 
-        set_log_level_from_string(config.get('verbosity', "INFO"))
-        set_log_stream(config.get('logfile', None))
+        set_log_level_from_string(config.get("verbosity", "INFO"))
+        set_log_stream(config.get("logfile", None))
 
         self.server = grpc.server(futures.ThreadPoolExecutor(max_workers=350), interceptors=[JWTInterceptor()])
         self.certificate = None
         self.health_servicer = health.HealthServicer()
 
         if isinstance(servicer, rpc.CombinerServicer):
             rpc.add_CombinerServicer_to_server(servicer, self.server)
@@ -30,23 +29,23 @@
         if isinstance(modelservicer, rpc.ModelServiceServicer):
             rpc.add_ModelServiceServicer_to_server(modelservicer, self.server)
         if isinstance(servicer, rpc.CombinerServicer):
             rpc.add_ControlServicer_to_server(servicer, self.server)
 
         health_pb2_grpc.add_HealthServicer_to_server(self.health_servicer, self.server)
 
-        if config['secure']:
+        if config["secure"]:
             logger.info(f'Creating secure gRPCS server using certificate: {config["certificate"]}')
             server_credentials = grpc.ssl_server_credentials(
-                ((config['key'], config['certificate'],),))
+                ((config["key"], config["certificate"],),))
             self.server.add_secure_port(
-                '[::]:' + str(config['port']), server_credentials)
+                "[::]:" + str(config["port"]), server_credentials)
         else:
             logger.info("Creating gRPC server")
-            self.server.add_insecure_port('[::]:' + str(config['port']))
+            self.server.add_insecure_port("[::]:" + str(config["port"]))
 
     def start(self):
         """ Start the gRPC server."""
         logger.info("gRPC Server started")
         self.server.start()
 
     def stop(self):
```

### Comparing `fedn-0.9.2/fedn/network/loadbalancer/firstavailable.py` & `fedn-0.9.5/fedn/network/loadbalancer/firstavailable.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,12 +9,11 @@
     """
 
     def __init__(self, network):
         super().__init__(network)
 
     def find_combiner(self):
         """Find the first available combiner."""
-
         for combiner in self.network.get_combiners():
             if combiner.allowing_clients():
                 return combiner
         return None
```

### Comparing `fedn-0.9.2/fedn/network/loadbalancer/leastpacked.py` & `fedn-0.9.5/fedn/network/loadbalancer/leastpacked.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,29 +9,25 @@
     :type network: class: `fedn.network.api.network.Network`
     """
 
     def __init__(self, network):
         super().__init__(network)
 
     def find_combiner(self):
-        """
-        Find the combiner with the least number of attached clients.
+        """Find the combiner with the least number of attached clients.
 
         """
         min_clients = None
         selected_combiner = None
 
         for combiner in self.network.get_combiners():
             try:
                 if combiner.allowing_clients():
                     # Using default default Channel = 1, MODEL_UPDATE_REQUESTS
                     nr_active_clients = len(combiner.list_active_clients())
-                    if not min_clients:
-                        min_clients = nr_active_clients
-                        selected_combiner = combiner
-                    elif nr_active_clients < min_clients:
+                    if not min_clients or nr_active_clients < min_clients:
                         min_clients = nr_active_clients
                         selected_combiner = combiner
             except CombinerUnavailableError:
                 pass
 
         return selected_combiner
```

### Comparing `fedn-0.9.2/fedn/network/state.py` & `fedn-0.9.5/fedn/network/state.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/storage/models/memorymodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/memorymodelstorage.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,17 +27,15 @@
         obj = self.models[model_id]
         obj.seek(0, 0)
         # Have to copy object to not mix up the file pointers when sending... fix in better way.
         obj = BytesIO(obj.read())
         return obj
 
     def get_ptr(self, model_id):
-        """
-
-        :param model_id:
+        """:param model_id:
         :return:
         """
         return self.models[model_id]
 
     def get_model_metadata(self, model_id):
         return self.models_metadata[model_id]
```

### Comparing `fedn-0.9.2/fedn/network/storage/models/modelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/modelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/storage/models/tempmodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/tempmodelstorage.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,17 +37,15 @@
         with open(os.path.join(self.default_dir, str(model_id)), "rb") as f:
             obj.write(f.read())
 
         obj.seek(0, 0)
         return obj
 
     def get_ptr(self, model_id):
-        """
-
-        :param model_id:
+        """:param model_id:
         :return:
         """
         try:
             f = self.models[model_id]["file"]
         except KeyError:
             f = open(os.path.join(self.default_dir, str(model_id)), "wb")
```

### Comparing `fedn-0.9.2/fedn/network/storage/models/tests/test_tempmodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/tests/test_tempmodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/storage/s3/base.py` & `fedn-0.9.5/fedn/network/storage/s3/base.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/storage/s3/miniorepository.py` & `fedn-0.9.5/fedn/network/storage/s3/miniorepository.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 
     def __init__(self, config):
         """Initialize object.
 
         :param config: Dictionary containing configuration for credentials and bucket names.
         :type config: dict
         """
-
         super().__init__()
         self.name = "MINIORepository"
 
         if config["storage_secure_mode"]:
             manager = PoolManager(num_pools=100, cert_reqs="CERT_NONE", assert_hostname=False)
             self.client = Minio(
                 "{0}:{1}".format(config["storage_hostname"], config["storage_port"]),
@@ -87,15 +86,14 @@
     def delete_artifact(self, instance_name, bucket):
         """Delete object with name instance_name from buckets.
 
         :param instance_name: The object name
         :param bucket: Buckets to delete from
         :type bucket: str
         """
-
         try:
             self.client.remove_object(bucket, instance_name)
         except InvalidResponseError as err:
             logger.error("Could not delete artifact: {0} err: {1}".format(instance_name, err))
             pass
 
     def create_bucket(self, bucket_name):
```

### Comparing `fedn-0.9.2/fedn/network/storage/s3/repository.py` & `fedn-0.9.5/fedn/network/storage/s3/repository.py`

 * *Files 0% similar despite different names*

```diff
@@ -69,15 +69,14 @@
 
         :param name: The name of the compute package.
         :type name: str
         :param compute_package: The compute package
         :type compute_pacakge: BytesIO or str file name.
         :param is_file: True if model is a file name, else False
         """
-
         try:
             self.client.set_artifact(str(name), compute_package, bucket=self.context_bucket, is_file=is_file)
         except Exception:
             logger.error("Failed to write compute_package to repository.")
             raise
 
     def get_compute_package(self, compute_package):
@@ -96,13 +95,12 @@
 
     def delete_compute_package(self, compute_package):
         """Delete a compute package from storage.
 
         :param compute_package: The name of the compute_package
         :type compute_package: str
         """
-
         try:
             self.client.delete_artifact(compute_package, bucket=[self.context_bucket])
         except Exception:
             logger.error("Failed to delete compute_package from repository.")
             raise
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/mongostatestore.py` & `fedn-0.9.5/fedn/network/storage/statestore/mongostatestore.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,14 @@
         :type skip: int
         :param sort_key: The key to sort by.
         :type sort_key: str
         :param sort_order: The sort order.
         :type sort_order: pymongo.ASCENDING or pymongo.DESCENDING
         :return: Dictionary of sessions in result (array of session objects) and count.
         """
-
         result = None
 
         if limit is not None and skip is not None:
             limit = int(limit)
             skip = int(skip)
 
             result = self.sessions.find().limit(limit).skip(skip).sort(sort_key, sort_order)
@@ -171,15 +170,14 @@
     def set_latest_model(self, model_id, session_id=None):
         """Set the latest model id.
 
         :param model_id: The model id.
         :type model_id: str
         :return:
         """
-
         committed_at = datetime.now()
         current_model = self.model.find_one({"key": "current_model"})
         parent_model = None
 
         # if session_id is set the it means the model is generated from a session
         # and we need to set the parent model
         # if not the model is uploaded by the user and we don't need to set the parent model
@@ -210,15 +208,14 @@
 
     def get_initial_model(self):
         """Return model_id for the initial model in the model trail
 
         :return: The initial model id. None if no model is found.
         :rtype: str
         """
-
         result = self.model.find_one({"key": "model_trail"}, sort=[("committed_at", pymongo.ASCENDING)])
         if result is None:
             return None
 
         try:
             model_id = result["model"]
             if model_id == "" or model_id == " ":
@@ -248,15 +245,14 @@
     def set_current_model(self, model_id: str):
         """Set the current model in statestore.
 
         :param model_id: The model id.
         :type model_id: str
         :return:
         """
-
         try:
             committed_at = datetime.now()
 
             existing_model = self.model.find_one({"key": "models", "model": model_id})
 
             if existing_model is not None:
                 self.model.update_one({"key": "current_model"}, {"$set": {"model": model_id, "committed_at": committed_at, "session_id": None}}, True)
@@ -269,58 +265,53 @@
 
     def get_latest_round(self):
         """Get the id of the most recent round.
 
         :return: The id of the most recent round.
         :rtype: ObjectId
         """
-
         return self.rounds.find_one(sort=[("_id", pymongo.DESCENDING)])
 
     def get_round(self, id):
         """Get round with id.
 
         :param id: id of round to get
         :type id: int
         :return: round with id, reducer and combiners
         :rtype: ObjectId
         """
-
         return self.rounds.find_one({"round_id": str(id)})
 
     def get_rounds(self):
         """Get all rounds.
 
         :return: All rounds.
         :rtype: ObjectId
         """
-
         return self.rounds.find()
 
     def get_validations(self, **kwargs):
         """Get validations from the database.
 
         :param kwargs: query to filter validations
         :type kwargs: dict
         :return: validations matching query
         :rtype: ObjectId
         """
-
         result = self.control.validations.find(kwargs)
         return result
 
     def set_active_compute_package(self, id: str):
         """Set the active compute package in statestore.
 
         :param id: The id of the compute package (not document _id).
         :type id: str
         :return: True if successful.
         :rtype: bool
         """
-
         try:
             find = {"id": id}
             projection = {"_id": False, "key": False}
 
             doc = self.control.package.find_one(find, projection)
 
             if doc is None:
@@ -340,15 +331,14 @@
         """Set the active compute package in statestore.
 
         :param file_name: The file_name of the compute package.
         :type file_name: str
         :return: True if successful.
         :rtype: bool
         """
-
         obj = {
             "file_name": file_name,
             "storage_file_name": storage_file_name,
             "helper": helper_type,
             "committed_at": datetime.now(),
             "name": name,
             "description": description,
@@ -392,15 +382,14 @@
         :param sort_key: The key to sort by.
         :type sort_key: str
         :param sort_order: The sort order.
         :type sort_order: pymongo.ASCENDING or pymongo.DESCENDING
         :return: Dictionary of compute packages in result and count.
         :rtype: dict
         """
-
         result = None
         count = None
 
         find_option = {"key": "package_trail"}
         projection = {"key": False, "_id": False}
 
         try:
@@ -540,15 +529,14 @@
         :param model_id: The model id.
         :type model_id: str
         :param limit: The maximum number of descendants to return.
         :type limit: int
         :return: List of model descendants.
         :rtype: list
         """
-
         model: object = self.model.find_one({"key": "models", "model": model_id})
         current_model_id: str = model["model"] if model is not None else None
         result: list = []
 
         for _ in range(limit):
             if current_model_id is None:
                 break
@@ -680,15 +668,14 @@
         :param sort_order: The sort order.
         :type sort_order: pymongo.ASCENDING or pymongo.DESCENDING
         :param projection: The projection.
         :type projection: dict
         :return: Dictionary of combiners in result and count.
         :rtype: dict
         """
-
         result = None
         count = None
 
         try:
             if limit is not None and skip is not None:
                 limit = int(limit)
                 skip = int(skip)
@@ -709,15 +696,14 @@
     def set_combiner(self, combiner_data):
         """Set combiner in statestore.
 
         :param combiner_data: dictionary of combiner config
         :type combiner_data: dict
         :return:
         """
-
         combiner_data["updated_at"] = str(datetime.now())
         self.combiners.update_one({"name": combiner_data["name"]}, {"$set": combiner_data}, True)
 
     def delete_combiner(self, combiner):
         """Delete a combiner from statestore.
 
         :param combiner: name of combiner to delete.
@@ -765,15 +751,14 @@
         :type limit: int
         :param skip: The number of clients to skip.
         :type skip: int
         :param status:  online | offline
         :type status: str
         :param sort_key: The key to sort by.
         """
-
         result = None
         count = None
 
         try:
             find = {} if status is None else {"status": status}
             projection = {"_id": False, "updated_at": False}
 
@@ -802,15 +787,14 @@
         :param sort_key: The key to sort by.
         :type sort_key: str
         :param sort_order: The sort order.
         :type sort_order: pymongo.ASCENDING or pymongo.DESCENDING
         :return: list of combiner data.
         :rtype: list(ObjectId)
         """
-
         result = None
 
         try:
             pipeline = (
                 [
                     {"$match": {"combiner": {"$in": combiners}, "status": "online"}},
                     {"$group": {"_id": "$combiner", "count": {"$sum": 1}}},
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/statestorebase.py` & `fedn-0.9.5/fedn/network/storage/statestore/statestorebase.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/client_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/client_store.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
 
@@ -14,24 +14,24 @@
         self.combiner = combiner
         self.combiner_preferred = combiner_preferred
         self.ip = ip
         self.status = status
         self.updated_at = updated_at
         self.last_seen = last_seen
 
-    def from_dict(data: dict) -> 'Client':
+    def from_dict(data: dict) -> "Client":
         return Client(
-            id=str(data['_id']),
-            name=data['name'] if 'name' in data else None,
-            combiner=data['combiner'] if 'combiner' in data else None,
-            combiner_preferred=data['combiner_preferred'] if 'combiner_preferred' in data else None,
-            ip=data['ip'] if 'ip' in data else None,
-            status=data['status'] if 'status' in data else None,
-            updated_at=data['updated_at'] if 'updated_at' in data else None,
-            last_seen=data['last_seen'] if 'last_seen' in data else None
+            id=str(data["_id"]),
+            name=data["name"] if "name" in data else None,
+            combiner=data["combiner"] if "combiner" in data else None,
+            combiner_preferred=data["combiner_preferred"] if "combiner_preferred" in data else None,
+            ip=data["ip"] if "ip" in data else None,
+            status=data["status"] if "status" in data else None,
+            updated_at=data["updated_at"] if "updated_at" in data else None,
+            last_seen=data["last_seen"] if "last_seen" in data else None
         )
 
 
 class ClientStore(Store[Client]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
@@ -45,15 +45,15 @@
         """
         response = super().get(id, use_typing=use_typing)
         return Client.from_dict(response) if use_typing else response
 
     def update(self, id: str, item: Client) -> bool:
         raise NotImplementedError("Update not implemented for ClientStore")
 
-    def add(self, item: Client) -> bool:
+    def add(self, item: Client)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for ClientStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for ClientStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Client]]:
         """List entities
@@ -70,15 +70,15 @@
         param kwargs: Additional query parameters
             type: dict
             example: {"key": "models"}
         return: A dictionary with the count and the result
         """
         response = super().list(limit, skip, sort_key or "last_seen", sort_order, use_typing=use_typing, **kwargs)
 
-        result = [Client.from_dict(item) for item in response['result']] if use_typing else response['result']
+        result = [Client.from_dict(item) for item in response["result"]] if use_typing else response["result"]
 
         return {
             "count": response["count"],
             "result": result
         }
 
     def count(self, **kwargs) -> int:
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/combiner_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/combiner_store.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from bson import ObjectId
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
@@ -34,28 +34,28 @@
         self.ip = ip
         self.key = key
         self.parent = parent
         self.port = port
         self.status = status
         self.updated_at = updated_at
 
-    def from_dict(data: dict) -> 'Combiner':
+    def from_dict(data: dict) -> "Combiner":
         return Combiner(
-            id=str(data['_id']),
-            name=data['name'] if 'name' in data else None,
-            address=data['address'] if 'address' in data else None,
-            certificate=data['certificate'] if 'certificate' in data else None,
-            config=data['config'] if 'config' in data else None,
-            fqdn=data['fqdn'] if 'fqdn' in data else None,
-            ip=data['ip'] if 'ip' in data else None,
-            key=data['key'] if 'key' in data else None,
-            parent=data['parent'] if 'parent' in data else None,
-            port=data['port'] if 'port' in data else None,
-            status=data['status'] if 'status' in data else None,
-            updated_at=data['updated_at'] if 'updated_at' in data else None
+            id=str(data["_id"]),
+            name=data["name"] if "name" in data else None,
+            address=data["address"] if "address" in data else None,
+            certificate=data["certificate"] if "certificate" in data else None,
+            config=data["config"] if "config" in data else None,
+            fqdn=data["fqdn"] if "fqdn" in data else None,
+            ip=data["ip"] if "ip" in data else None,
+            key=data["key"] if "key" in data else None,
+            parent=data["parent"] if "parent" in data else None,
+            port=data["port"] if "port" in data else None,
+            status=data["status"] if "status" in data else None,
+            updated_at=data["updated_at"] if "updated_at" in data else None
         )
 
 
 class CombinerStore(Store[Combiner]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
@@ -66,27 +66,27 @@
             description: The id of the entity, can be either the id or the name (property)
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entity
         """
         if ObjectId.is_valid(id):
             id_obj = ObjectId(id)
-            document = self.database[self.collection].find_one({'_id': id_obj})
+            document = self.database[self.collection].find_one({"_id": id_obj})
         else:
-            document = self.database[self.collection].find_one({'name': id})
+            document = self.database[self.collection].find_one({"name": id})
 
         if document is None:
             raise EntityNotFound(f"Entity with (id | name) {id} not found")
 
         return Combiner.from_dict(document) if use_typing else from_document(document)
 
     def update(self, id: str, item: Combiner) -> bool:
         raise NotImplementedError("Update not implemented for CombinerStore")
 
-    def add(self, item: Combiner) -> bool:
+    def add(self, item: Combiner)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for CombinerStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for CombinerStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Combiner]]:
         """List entities
@@ -103,15 +103,15 @@
         param kwargs: Additional query parameters
             type: dict
             example: {"key": "models"}
         return: A dictionary with the count and the result
         """
         response = super().list(limit, skip, sort_key or "updated_at", sort_order, use_typing=use_typing, **kwargs)
 
-        result = [Combiner.from_dict(item) for item in response['result']] if use_typing else response['result']
+        result = [Combiner.from_dict(item) for item in response["result"]] if use_typing else response["result"]
 
         return {
             "count": response["count"],
             "result": result
         }
 
     def count(self, **kwargs) -> int:
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/model_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/model_store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from bson import ObjectId
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
@@ -15,22 +15,22 @@
         self.id = id
         self.key = key
         self.model = model
         self.parent_model = parent_model
         self.session_id = session_id
         self.committed_at = committed_at
 
-    def from_dict(data: dict) -> 'Model':
+    def from_dict(data: dict) -> "Model":
         return Model(
-            id=str(data['_id']),
-            key=data['key'] if 'key' in data else None,
-            model=data['model'] if 'model' in data else None,
-            parent_model=data['parent_model'] if 'parent_model' in data else None,
-            session_id=data['session_id'] if 'session_id' in data else None,
-            committed_at=data['committed_at'] if 'committed_at' in data else None
+            id=str(data["_id"]),
+            key=data["key"] if "key" in data else None,
+            model=data["model"] if "model" in data else None,
+            parent_model=data["parent_model"] if "parent_model" in data else None,
+            session_id=data["session_id"] if "session_id" in data else None,
+            committed_at=data["committed_at"] if "committed_at" in data else None
         )
 
 
 class ModelStore(Store[Model]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
@@ -42,29 +42,29 @@
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entity
         """
         kwargs = {"key": "models"}
         if ObjectId.is_valid(id):
             id_obj = ObjectId(id)
-            kwargs['_id'] = id_obj
+            kwargs["_id"] = id_obj
         else:
-            kwargs['model'] = id
+            kwargs["model"] = id
 
         document = self.database[self.collection].find_one(kwargs)
 
         if document is None:
             raise EntityNotFound(f"Entity with (id | model) {id} not found")
 
         return Model.from_dict(document) if use_typing else from_document(document)
 
     def update(self, id: str, item: Model) -> bool:
         raise NotImplementedError("Update not implemented for ModelStore")
 
-    def add(self, item: Model) -> bool:
+    def add(self, item: Model)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for ModelStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for ModelStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Model]]:
         """List entities
@@ -79,21 +79,21 @@
         param use_typing: Whether to return the entities as typed objects or as dicts
             type: bool
         param kwargs: Additional query parameters
             type: dict
             example: {"key": "models"}
         return: A dictionary with the count and the result
         """
-        kwargs['key'] = "models"
+        kwargs["key"] = "models"
 
         response = super().list(limit, skip, sort_key or "committed_at", sort_order, use_typing=use_typing, **kwargs)
 
-        result = [Model.from_dict(item) for item in response['result']] if use_typing else response['result']
+        result = [Model.from_dict(item) for item in response["result"]] if use_typing else response["result"]
         return {
-            "count": response['count'],
+            "count": response["count"],
             "result": result
         }
 
     def list_descendants(self, id: str, limit: int, use_typing: bool = False) -> List[Model]:
         """List descendants
         param id: The id of the entity
             type: str
@@ -103,17 +103,17 @@
         param use_typing: Whether to return the entities as typed objects or as dicts
             type: bool
         return: A list of entities
         """
         kwargs = {"key": "models"}
         if ObjectId.is_valid(id):
             id_obj = ObjectId(id)
-            kwargs['_id'] = id_obj
+            kwargs["_id"] = id_obj
         else:
-            kwargs['model'] = id
+            kwargs["model"] = id
 
         model: object = self.database[self.collection].find_one(kwargs)
 
         if model is None:
             raise EntityNotFound(f"Entity with (id | model) {id} not found")
 
         current_model_id: str = model["model"]
@@ -146,17 +146,17 @@
         param use_typing: Whether to return the entities as typed objects or as dicts
             type: bool
         return: A list of entities
         """
         kwargs = {"key": "models"}
         if ObjectId.is_valid(id):
             id_obj = ObjectId(id)
-            kwargs['_id'] = id_obj
+            kwargs["_id"] = id_obj
         else:
-            kwargs['model'] = id
+            kwargs["model"] = id
 
         model: object = self.database[self.collection].find_one(kwargs)
 
         if model is None:
             raise EntityNotFound(f"Entity with (id | model) {id} not found")
 
         current_model_id: str = model["parent_model"]
@@ -187,9 +187,9 @@
     def count(self, **kwargs) -> int:
         """Count entities
         param kwargs: Additional query parameters
             type: dict
             example: {"key": "models"}
         return: The count (int)
         """
-        kwargs['key'] = "models"
+        kwargs["key"] = "models"
         return super().count(**kwargs)
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/package_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/package_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from datetime import datetime
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
 from .shared import EntityNotFound, from_document
@@ -28,29 +28,29 @@
         self.file_name = file_name
         self.helper = helper
         self.id = id
         self.name = name
         self.storage_file_name = storage_file_name
         self.active = active
 
-    def from_dict(data: dict, active_package: dict) -> 'Package':
+    def from_dict(data: dict, active_package: dict) -> "Package":
         active = False
         if active_package:
             if "id" in active_package and "id" in data:
                 active = active_package["id"] == data["id"]
 
         return Package(
-            id=data['id'] if 'id' in data else None,
-            key=data['key'] if 'key' in data else None,
-            committed_at=data['committed_at'] if 'committed_at' in data else None,
-            description=data['description'] if 'description' in data else None,
-            file_name=data['file_name'] if 'file_name' in data else None,
-            helper=data['helper'] if 'helper' in data else None,
-            name=data['name'] if 'name' in data else None,
-            storage_file_name=data['storage_file_name'] if 'storage_file_name' in data else None,
+            id=data["id"] if "id" in data else None,
+            key=data["key"] if "key" in data else None,
+            committed_at=data["committed_at"] if "committed_at" in data else None,
+            description=data["description"] if "description" in data else None,
+            file_name=data["file_name"] if "file_name" in data else None,
+            helper=data["helper"] if "helper" in data else None,
+            name=data["name"] if "name" in data else None,
+            storage_file_name=data["storage_file_name"] if "storage_file_name" in data else None,
             active=active
         )
 
 
 class PackageStore(Store[Package]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
@@ -62,43 +62,43 @@
             description: The id of the entity, can be either the id or the model (property)
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
             description: Whether to return the entities as typed objects or as dicts.
             If True, and active property will be set based on the active package.
         return: The entity
         """
-        document = self.database[self.collection].find_one({'id': id})
+        document = self.database[self.collection].find_one({"id": id})
 
         if document is None:
             raise EntityNotFound(f"Entity with id {id} not found")
 
         if not use_typing:
             return from_document(document)
 
-        response_active = self.database[self.collection].find_one({'key': 'active'})
+        response_active = self.database[self.collection].find_one({"key": "active"})
 
         return Package.from_dict(document, response_active)
 
     def get_active(self, use_typing: bool = False) -> Package:
         """Get the active entity
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entity
         """
-        response = self.database[self.collection].find_one({'key': 'active'})
+        response = self.database[self.collection].find_one({"key": "active"})
 
         if response is None:
             raise EntityNotFound(f"Entity with id {id} not found")
 
         return Package.from_dict(response, response) if use_typing else from_document(response)
 
     def update(self, id: str, item: Package) -> bool:
         raise NotImplementedError("Update not implemented for PackageStore")
 
-    def add(self, item: Package) -> bool:
+    def add(self, item: Package)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for PackageStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for PackageStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Package]]:
         """List entities
@@ -119,17 +119,17 @@
             example: {"key": "models"}
         return: A dictionary with the count and the result
         """
         kwargs["key"] = "package_trail"
 
         response = super().list(limit, skip, sort_key or "committed_at", sort_order, use_typing=True, **kwargs)
 
-        response_active = self.database[self.collection].find_one({'key': 'active'})
+        response_active = self.database[self.collection].find_one({"key": "active"})
 
-        result = [Package.from_dict(item, response_active) for item in response['result']]
+        result = [Package.from_dict(item, response_active) for item in response["result"]]
 
         return {
             "count": response["count"],
             "result": result
         }
 
     def count(self, **kwargs) -> int:
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/round_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/round_store.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
 
@@ -11,22 +11,22 @@
         self.id = id
         self.round_id = round_id
         self.status = status
         self.round_config = round_config
         self.combiners = combiners
         self.round_data = round_data
 
-    def from_dict(data: dict) -> 'Round':
+    def from_dict(data: dict) -> "Round":
         return Round(
-            id=str(data['_id']),
-            round_id=data['round_id'] if 'round_id' in data else None,
-            status=data['status'] if 'status' in data else None,
-            round_config=data['round_config'] if 'round_config' in data else None,
-            combiners=data['combiners'] if 'combiners' in data else None,
-            round_data=data['round_data'] if 'round_data' in data else None
+            id=str(data["_id"]),
+            round_id=data["round_id"] if "round_id" in data else None,
+            status=data["status"] if "status" in data else None,
+            round_config=data["round_config"] if "round_config" in data else None,
+            combiners=data["combiners"] if "combiners" in data else None,
+            round_data=data["round_data"] if "round_data" in data else None
         )
 
 
 class RoundStore(Store[Round]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
@@ -40,15 +40,15 @@
         """
         response = super().get(id, use_typing=use_typing)
         return Round.from_dict(response) if use_typing else response
 
     def update(self, id: str, item: Round) -> bool:
         raise NotImplementedError("Update not implemented for RoundStore")
 
-    def add(self, item: Round) -> bool:
+    def add(self, item: Round)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for RoundStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for RoundStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Round]]:
         """List entities
@@ -66,13 +66,13 @@
             description: The order to sort by
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entities
         """
         response = super().list(limit, skip, sort_key or "round_id", sort_order, use_typing=use_typing, **kwargs)
 
-        result = [Round.from_dict(item) for item in response['result']] if use_typing else response['result']
+        result = [Round.from_dict(item) for item in response["result"]] if use_typing else response["result"]
 
         return {
             "count": response["count"],
             "result": result
         }
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/session_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/validation_store.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,90 +1,96 @@
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
-from bson import ObjectId
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
-from .shared import EntityNotFound, from_document
 
-
-class Session:
-    def __init__(self, id: str, session_id: str, status: str, session_config: dict = None):
+class Validation:
+    def __init__(
+            self,
+            id: str,
+            model_id: str,
+            data: str,
+            correlation_id: str,
+            timestamp: str,
+            session_id: str,
+            meta: str,
+            sender: dict = None,
+            receiver: dict = None
+    ):
         self.id = id
+        self.model_id = model_id
+        self.data = data
+        self.correlation_id = correlation_id
+        self.timestamp = timestamp
         self.session_id = session_id
-        self.status = status
-        self.session_config = session_config
-
-    def from_dict(data: dict) -> 'Session':
-        return Session(
-            id=str(data['_id']),
-            session_id=data['session_id'] if 'session_id' in data else None,
-            status=data['status'] if 'status' in data else None,
-            session_config=data['session_config'] if 'session_config' in data else None
+        self.meta = meta
+        self.sender = sender
+        self.receiver = receiver
+
+    def from_dict(data: dict) -> "Validation":
+        return Validation(
+            id=str(data["_id"]),
+            model_id=data["modelId"] if "modelId" in data else None,
+            data=data["data"] if "data" in data else None,
+            correlation_id=data["correlationId"] if "correlationId" in data else None,
+            timestamp=data["timestamp"] if "timestamp" in data else None,
+            session_id=data["sessionId"] if "sessionId" in data else None,
+            meta=data["meta"] if "meta" in data else None,
+            sender=data["sender"] if "sender" in data else None,
+            receiver=data["receiver"] if "receiver" in data else None
         )
 
 
-class SessionStore(Store[Session]):
+class ValidationStore(Store[Validation]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
-    def get(self, id: str, use_typing: bool = False) -> Session:
+    def get(self, id: str, use_typing: bool = False) -> Validation:
         """Get an entity by id
         param id: The id of the entity
             type: str
-            description: The id of the entity, can be either the id or the session_id (property)
+            description: The id of the entity, can be either the id or the validation (property)
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entity
         """
-        if ObjectId.is_valid(id):
-            id_obj = ObjectId(id)
-            document = self.database[self.collection].find_one({'_id': id_obj})
-        else:
-            document = self.database[self.collection].find_one({'session_id': id})
-
-        if document is None:
-            raise EntityNotFound(f"Entity with (id | session_id) {id} not found")
-
-        return Session.from_dict(document) if use_typing else from_document(document)
+        response = super().get(id, use_typing=use_typing)
+        return Validation.from_dict(response) if use_typing else response
 
-    def update(self, id: str, item: Session) -> bool:
-        raise NotImplementedError("Update not implemented for SessionStore")
+    def update(self, id: str, item: Validation) -> bool:
+        raise NotImplementedError("Update not implemented for ValidationStore")
 
-    def add(self, item: Session) -> bool:
-        raise NotImplementedError("Add not implemented for SessionStore")
+    def add(self, item: Validation)-> Tuple[bool, Any]:
+        raise NotImplementedError("Add not implemented for ValidationStore")
 
     def delete(self, id: str) -> bool:
-        raise NotImplementedError("Delete not implemented for SessionStore")
+        raise NotImplementedError("Delete not implemented for ValidationStore")
 
-    def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Session]]:
+    def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Validation]]:
         """List entities
         param limit: The maximum number of entities to return
             type: int
             description: The maximum number of entities to return
         param skip: The number of entities to skip
             type: int
             description: The number of entities to skip
         param sort_key: The key to sort by
             type: str
             description: The key to sort by
         param sort_order: The order to sort by
             type: pymongo.DESCENDING
             description: The order to sort by
-        param use_typing: Whether to return the entity as a typed object or as a dict
+        param use_typing: Whether to return the entities as typed objects or as dicts
             type: bool
-            description: Whether to return the entities as typed objects or as dicts.
-        param kwargs: Additional query parameters
-            type: dict
-            description: Additional query parameters
-        return: The entities
+            description: Whether to return the entities as typed objects or as dicts
+        return: A dictionary with the count and a list of entities
         """
-        response = super().list(limit, skip, sort_key or "session_id", sort_order, use_typing=use_typing, **kwargs)
-
-        result = [Session.from_dict(item) for item in response['result']] if use_typing else response['result']
+        response = super().list(limit, skip, sort_key or "timestamp", sort_order, use_typing=use_typing, **kwargs)
 
+        result = [Validation.from_dict(item) for item in response["result"]] if use_typing else response["result"]
         return {
             "count": response["count"],
             "result": result
         }
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/status_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/status_store.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List
+from typing import Any, Dict, List, Tuple
 
 import pymongo
 from pymongo.database import Database
 
 from fedn.network.storage.statestore.stores.store import Store
 
 
@@ -27,26 +27,26 @@
         self.data = data
         self.correlation_id = correlation_id
         self.type = type
         self.extra = extra
         self.session_id = session_id
         self.sender = sender
 
-    def from_dict(data: dict) -> 'Status':
+    def from_dict(data: dict) -> "Status":
         return Status(
-            id=str(data['_id']),
-            status=data['status'] if 'status' in data else None,
-            timestamp=data['timestamp'] if 'timestamp' in data else None,
-            log_level=data['logLevel'] if 'logLevel' in data else None,
-            data=data['data'] if 'data' in data else None,
-            correlation_id=data['correlationId'] if 'correlationId' in data else None,
-            type=data['type'] if 'type' in data else None,
-            extra=data['extra'] if 'extra' in data else None,
-            session_id=data['sessionId'] if 'sessionId' in data else None,
-            sender=data['sender'] if 'sender' in data else None
+            id=str(data["_id"]),
+            status=data["status"] if "status" in data else None,
+            timestamp=data["timestamp"] if "timestamp" in data else None,
+            log_level=data["logLevel"] if "logLevel" in data else None,
+            data=data["data"] if "data" in data else None,
+            correlation_id=data["correlationId"] if "correlationId" in data else None,
+            type=data["type"] if "type" in data else None,
+            extra=data["extra"] if "extra" in data else None,
+            session_id=data["sessionId"] if "sessionId" in data else None,
+            sender=data["sender"] if "sender" in data else None
         )
 
 
 class StatusStore(Store[Status]):
     def __init__(self, database: Database, collection: str):
         super().__init__(database, collection)
 
@@ -61,15 +61,15 @@
         """
         response = super().get(id, use_typing=use_typing)
         return Status.from_dict(response) if use_typing else response
 
     def update(self, id: str, item: Status) -> bool:
         raise NotImplementedError("Update not implemented for StatusStore")
 
-    def add(self, item: Status) -> bool:
+    def add(self, item: Status)-> Tuple[bool, Any]:
         raise NotImplementedError("Add not implemented for StatusStore")
 
     def delete(self, id: str) -> bool:
         raise NotImplementedError("Delete not implemented for StatusStore")
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[Status]]:
         """List entities
@@ -87,10 +87,10 @@
             description: The order to sort by
         param use_typing: Whether to return the entities as typed objects or as dicts
             type: bool
             description: Whether to return the entities as typed objects or as dicts.
         """
         response = super().list(limit, skip, sort_key or "timestamp", sort_order, use_typing=use_typing, **kwargs)
 
-        result = [Status.from_dict(item) for item in response['result']] if use_typing else response['result']
+        result = [Status.from_dict(item) for item in response["result"]] if use_typing else response["result"]
 
-        return {'count': response['count'], 'result': result}
+        return {"count": response["count"], "result": result}
```

### Comparing `fedn-0.9.2/fedn/network/storage/statestore/stores/store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/store.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from typing import Dict, Generic, List, TypeVar
+from typing import Any, Dict, Generic, List, Tuple, TypeVar
 
 import pymongo
 from bson import ObjectId
 from pymongo.database import Database
 
 from .shared import EntityNotFound, from_document
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class Store(Generic[T]):
     def __init__(self, database: Database, collection: str):
         self.database = database
         self.collection = collection
 
@@ -19,26 +19,32 @@
         param id: The id of the entity
             type: str
         param use_typing: Whether to return the entity as a typed object or as a dict
             type: bool
         return: The entity
         """
         id_obj = ObjectId(id)
-        document = self.database[self.collection].find_one({'_id': id_obj})
+        document = self.database[self.collection].find_one({"_id": id_obj})
 
         if document is None:
             raise EntityNotFound(f"Entity with id {id} not found")
 
         return from_document(document) if not use_typing else document
 
     def update(self, id: str, item: T) -> bool:
         pass
 
-    def add(self, item: T) -> bool:
-        pass
+    def add(self, item: T) -> Tuple[bool, Any]:
+        try:
+            result = self.database[self.collection].insert_one(item)
+            id = result.inserted_id
+            document = self.database[self.collection].find_one({"_id": id})
+            return True, from_document(document)
+        except Exception as e:
+            return False, str(e)
 
     def delete(self, id: str) -> bool:
         pass
 
     def list(self, limit: int, skip: int, sort_key: str, sort_order=pymongo.DESCENDING, use_typing: bool = False, **kwargs) -> Dict[int, List[T]]:
         """List entities
         param limit: The maximum number of entities to return
```

### Comparing `fedn-0.9.2/fedn/utils/dispatcher.py` & `fedn-0.9.5/fedn/utils/dispatcher.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
+"""Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
 with modifications made by Scaleout Systems AB.
 Copyright (c) 2018 Databricks, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -56,23 +55,21 @@
     """Installs a specified version of python with pyenv and returns a path to the installed python
     binary.
     """
     raise NotImplementedError("This function is not implemented yet.")
 
 
 def _is_virtualenv_available():
-    """
-    Returns True if virtualenv is available, otherwise False.
+    """Returns True if virtualenv is available, otherwise False.
     """
     return shutil.which("virtualenv") is not None
 
 
 def _validate_virtualenv_is_available():
-    """
-    Validates virtualenv is available. If not, throws an `Exception` with a brief instruction
+    """Validates virtualenv is available. If not, throws an `Exception` with a brief instruction
     on how to install virtualenv.
     """
     if not _is_virtualenv_available():
         raise Exception("Could not find the virtualenv binary. Run `pip install virtualenv` to install " "virtualenv.")
 
 
 def _get_virtualenv_extra_env_vars(env_root_dir=None):
@@ -81,16 +78,15 @@
         # otherwise pip might prompt "yes or no" and ask stdin input
         "PIP_NO_INPUT": "1",
     }
     return extra_env
 
 
 def _get_python_env(python_env_file):
-    """
-    Parses a python environment file and returns a dictionary with the parsed content.
+    """Parses a python environment file and returns a dictionary with the parsed content.
     """
     if os.path.exists(python_env_file):
         return _PythonEnv.from_yaml(python_env_file)
 
 
 def _create_virtualenv(python_bin_path, env_dir, python_env, extra_env=None, capture_output=False):
     # Created a command to activate the environment
```

### Comparing `fedn-0.9.2/fedn/utils/environment.py` & `fedn-0.9.5/fedn/utils/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
+"""Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
 with modifications made by Scaleout Systems AB.
 Copyright (c) 2018 Databricks, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
 
@@ -24,16 +23,15 @@
 _PYTHON_ENV_FILE_NAME = "python_env.yaml"
 
 
 class _PythonEnv:
     BUILD_PACKAGES = ("pip", "setuptools", "wheel")
 
     def __init__(self, name=None, python=None, build_dependencies=None, dependencies=None):
-        """
-        Represents environment information for FEDn compute packages.
+        """Represents environment information for FEDn compute packages.
 
         Args:
         ----
             name: Name of environment. If unspecified, defaults to fedn_env
             python: Python version for the environment. If unspecified, defaults to the current
                 Python version.
             build_dependencies: List of build dependencies for the environment that must
```

### Comparing `fedn-0.9.2/fedn/utils/flowercompat/client_app_adapter.py` & `fedn-0.9.5/fedn/utils/flowercompat/client_app_adapter.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/helpers/helperbase.py` & `fedn-0.9.5/fedn/utils/helpers/helperbase.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,15 @@
-import os
-import tempfile
 from abc import ABC, abstractmethod
 
 
 class HelperBase(ABC):
     """Abstract class defining helpers."""
 
     def __init__(self):
         """Initialize helper."""
-
         self.name = self.__class__.__name__
 
     @abstractmethod
     def increment_average(self, m1, m2, a, W):
         """Compute one increment of incremental weighted averaging.
 
         :param m1: Current model weights in array-like format.
@@ -37,16 +34,7 @@
     def load(self, fh):
         """Load weights from file or filelike.
 
         :param fh: file path, filehandle, filelike.
         :return: Weights in array-like format.
         """
         pass
-
-    def get_tmp_path(self):
-        """Return a temporary output path compatible with save_model, load_model.
-
-        :return: Path to file.
-        """
-        fd, path = tempfile.mkstemp(suffix=".npz")
-        os.close(fd)
-        return path
```

### Comparing `fedn-0.9.2/fedn/utils/helpers/helpers.py` & `fedn-0.9.5/fedn/utils/helpers/helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/helpers/plugins/androidhelper.py` & `fedn-0.9.5/fedn/utils/helpers/plugins/androidhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/helpers/tests/test_numpyhelper.py` & `fedn-0.9.5/fedn/utils/helpers/tests/test_numpyhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/parameters.py` & `fedn-0.9.5/fedn/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/plots.py` & `fedn-0.9.5/fedn/utils/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,14 @@
             logger.error("FAILED TO CONNECT TO MONGO, {}".format(e))
             self.collection = None
             raise
 
     # plot metrics from DB
     def _scalar_metrics(self, metrics):
         """Extract all scalar valued metrics from a MODEL_VALIDATON."""
-
         data = json.loads(metrics["data"])
         data = json.loads(data["data"])
 
         valid_metrics = []
         for metric, val in data.items():
             # If it can be converted to a float it is a valid, scalar metric
             try:
@@ -44,17 +43,15 @@
                 valid_metrics.append(metric)
             except Exception:
                 pass
 
         return valid_metrics
 
     def create_table_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         if metrics is None:
             fig = go.Figure(data=[])
             fig.update_layout(title_text="No data currently available for table mean metrics")
             table = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return False
@@ -107,17 +104,15 @@
         )
 
         fig.update_layout(title_text="Summary: mean metrics")
         table = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return table
 
     def create_timeline_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         trace_data = []
         x = []
         y = []
         base = []
         for p in self.status.find({"type": "MODEL_UPDATE_REQUEST"}):
             e = json.loads(p["data"])
@@ -180,17 +175,15 @@
         fig.update_xaxes(title_text="Alliance/client")
         fig.update_yaxes(title_text="Time (Min)")
         fig.update_layout(title_text="Alliance timeline")
         timeline = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return timeline
 
     def create_client_training_distribution(self):
-        """
-
-        :return:
+        """:return:
         """
         training = []
         for p in self.status.find({"type": "MODEL_UPDATE"}):
             e = json.loads(p["data"])
             meta = json.loads(e["meta"])
             training.append(meta["exec_training"])
 
@@ -198,17 +191,15 @@
             return False
         fig = go.Figure(data=go.Histogram(x=training))
         fig.update_layout(title_text="Client model training time, mean: {}".format(numpy.mean(training)))
         histogram = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return histogram
 
     def create_client_histogram_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         training = []
         for p in self.status.find({"type": "MODEL_UPDATE"}):
             e = json.loads(p["data"])
             meta = json.loads(e["meta"])
             training.append(meta["exec_training"])
 
@@ -226,17 +217,15 @@
 
         fig.add_trace(go.Histogram(x=training))
 
         histogram_plot = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return histogram_plot
 
     def create_client_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         processing = []
         upload = []
         download = []
         training = []
         for p in self.status.find({"type": "MODEL_UPDATE"}):
             e = json.loads(p["data"])
@@ -254,17 +243,15 @@
         labels = ["Training execution", "Model upload (to combiner)", "Model download (from combiner)"]
         fig.add_trace(go.Pie(labels=labels, values=data))
 
         client_plot = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return client_plot
 
     def create_combiner_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         waiting = []
         aggregation = []
         model_load = []
         combination = []
         for round in self.mdb["control.round"].find():
             try:
@@ -288,26 +275,22 @@
         if not combination:
             return False
         fig.add_trace(go.Pie(labels=labels, values=val))
         combiner_plot = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return combiner_plot
 
     def fetch_valid_metrics(self):
-        """
-
-        :return:
+        """:return:
         """
         metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         valid_metrics = self._scalar_metrics(metrics)
         return valid_metrics
 
     def create_box_plot(self, metric):
-        """
-
-        :param metric:
+        """:param metric:
         :return:
         """
         metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         if metrics is None:
             fig = go.Figure(data=[])
             fig.update_layout(title_text="No data currently available for metric distribution over  " "participants")
             box = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
@@ -357,17 +340,15 @@
         box.update_xaxes(title_text="Rounds")
         box.update_yaxes(tickvals=[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
         box.update_layout(title_text="Metric distribution over clients: {}".format(metric), margin=dict(l=20, r=20, t=45, b=20))
         box = json.dumps(box, cls=plotly.utils.PlotlyJSONEncoder)
         return box
 
     def create_round_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         trace_data = []
         metrics = self.round_time.find_one({"key": "round_time"})
         if metrics is None:
             fig = go.Figure(data=[])
             fig.update_layout(title_text="No data currently available for round time")
             return False
@@ -387,17 +368,15 @@
         fig.update_xaxes(title_text="Round")
         fig.update_yaxes(title_text="Time (s)")
         fig.update_layout(title_text="Round time")
         round_t = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return round_t
 
     def create_cpu_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         metrics = self.psutil_usage.find_one({"key": "cpu_mem_usage"})
         if metrics is None:
             fig = go.Figure(data=[])
             fig.update_layout(title_text="No data currently available for MEM and CPU usage")
             cpu = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return False
```

### Comparing `fedn-0.9.2/fedn/utils/process.py` & `fedn-0.9.5/fedn/utils/process.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-"""
-Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
+"""Portions of this code are derived from the Apache 2.0 licensed project mlflow (https://mlflow.org/).,
 with modifications made by Scaleout Systems AB.
 Copyright (c) 2018 Databricks, Inc.
 
 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at
```

### Comparing `fedn-0.9.2/fedn/utils/tests/test_helpers.py` & `fedn-0.9.5/fedn/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn/utils/tests/test_parameters.py` & `fedn-0.9.5/fedn/utils/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.2/fedn.egg-info/PKG-INFO` & `fedn-0.9.5/fedn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.2
+Version: 0.9.5
 Summary: Scaleout Federated Learning
 Author-email: Scaleout Systems AB <contact@scaleoutsystems.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -284,15 +284,21 @@
 
 -  Secure deployment of server-side / control-plane on Kubernetes.
 -  UI with dashboards for orchestrating experiments and visualizing results
 -  Team features - collaborate with other users in shared project workspaces. 
 -  Features for the trusted-third party: Manage access to the FL network, FL clients and training progress.
 -  REST API for handling experiments/jobs. 
 -  View and export logging and tracing information. 
--  Public cloud, dedicated cloud and on-premise deployment options. 
+-  Public cloud, dedicated cloud and on-premise deployment options.
+
+Available clients:
+
+- Python client (this repository)
+- C++ client (`FEDn C++ client <https://github.com/scaleoutsystems/fedn-cpp-client>`__)
+- Android Kotlin client (`FEDn Kotlin client <https://github.com/scaleoutsystems/fedn-android-client>`__)
 
 
 Getting started
 ============================
 
 Get started with FEDn in two steps:
```

### Comparing `fedn-0.9.2/fedn.egg-info/SOURCES.txt` & `fedn-0.9.5/fedn.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 fedn/network/state.py
 fedn/network/api/__init__.py
 fedn/network/api/auth.py
 fedn/network/api/client.py
 fedn/network/api/interface.py
 fedn/network/api/network.py
 fedn/network/api/server.py
+fedn/network/api/shared.py
 fedn/network/api/tests.py
 fedn/network/api/v1/__init__.py
 fedn/network/api/v1/client_routes.py
 fedn/network/api/v1/combiner_routes.py
 fedn/network/api/v1/model_routes.py
 fedn/network/api/v1/package_routes.py
 fedn/network/api/v1/round_routes.py
@@ -115,11 +116,12 @@
 fedn/utils/flowercompat/__init__.py
 fedn/utils/flowercompat/client_app_adapter.py
 fedn/utils/helpers/__init__.py
 fedn/utils/helpers/helperbase.py
 fedn/utils/helpers/helpers.py
 fedn/utils/helpers/plugins/__init__.py
 fedn/utils/helpers/plugins/androidhelper.py
+fedn/utils/helpers/plugins/binaryhelper.py
 fedn/utils/helpers/plugins/numpyhelper.py
 fedn/utils/helpers/tests/test_numpyhelper.py
 fedn/utils/tests/test_helpers.py
 fedn/utils/tests/test_parameters.py
```

### Comparing `fedn-0.9.2/pyproject.toml` & `fedn-0.9.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fedn"
-version = "0.9.2"
+version = "0.9.5"
 description = "Scaleout Federated Learning"
 authors = [{ name = "Scaleout Systems AB", email = "contact@scaleoutsystems.com" }]
 readme = "README.rst"
 license = {file="LICENSE"}
 keywords = [
     "Scaleout",
     "FEDn",
@@ -173,29 +173,16 @@
   "PLW2901", # `for` loop variable `val` overwritten by assignment target
   "D419", # Docstring is empty
   "C416", # Unnecessary `list` comprehension (rewrite using `list()`)
   "SIM102", # Use a single `if` statement instead of nested `if` statements
   "PLW1508", # Invalid type for environment variable default; expected `str` or `None`
   "B007", # Loop control variable `v` not used within loop body
   "N806", # Variable `X_test` in function should be lowercase
-  
-  # solved with --fix
-  "Q000", # [*] Single quotes found but double quotes preferred
-  "D212", # [*] Multi-line docstring summary should start at the first line
-  "D213", # [*] Multi-line docstring summary should start at the second line
-  "D202", # [*] No blank lines allowed after function docstring (found 1)
-  "D209", # [*] Multi-line docstring closing quotes should be on a separate line
-  "D204", # [*] 1 blank line required after class docstring
-  "SIM114", # [*] Combine `if` branches using logical `or` operator
-  "D208", # [*] Docstring is over-indented
-  "I001", # [*] Import block is un-sorted or un-formatted
   "SIM103", # Return the condition directly
-  "PLR5501", # [*] Use `elif` instead of `else` then `if`, to reduce indentation
-  "RET501", # [*] Do not explicitly `return None` in function if it is the only possible return value
-  "PLW0120", # [*] `else` clause on loop without a `break` statement; remove the `else` and dedent its contents
+  "I001", # [*] Import block is un-sorted or un-formatted
 
   # unsafe?
   "S104", # Possible binding to all interfaces
   
   "S311", # Standard pseudo-random generators are not suitable for cryptographic purposes
   "S501", # Probable use of `requests` call with `verify=False` disabling SSL certificate checks
   "S108", # Probable insecure usage of temporary file or directory: "/tmp/models"
```

