# Comparing `tmp/fedn-0.9.3.tar.gz` & `tmp/fedn-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fedn-0.9.3.tar", last modified: Wed May 22 12:55:51 2024, max compression
+gzip compressed data, was "fedn-0.9.5.tar", last modified: Wed May 22 12:52:34 2024, max compression
```

## Comparing `fedn-0.9.3.tar` & `fedn-0.9.5.tar`

### file list

```diff
@@ -1,412 +1,159 @@
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.663931 fedn-0.9.3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11350 2023-11-21 14:46:43.000000 fedn-0.9.3/LICENSE
--rw-r--r--   0 stefan    (1000) stefan    (1000)    20324 2024-05-22 12:55:51.663931 fedn-0.9.3/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6152 2024-05-22 12:54:10.000000 fedn-0.9.3/README.rst
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      452 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.647931 fedn-0.9.3/fedn/build/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.647931 fedn-0.9.3/fedn/build/lib/
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      533 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5725 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/client_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3729 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/combiner_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1488 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/config_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      261 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/main.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1544 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/model_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2386 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/package_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1544 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/round_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9005 2024-05-08 10:15:46.000000 fedn-0.9.3/fedn/build/lib/cli/run_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1562 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/session_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2718 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1559 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/status_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/cli/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/cli/tests/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/cli/tests/tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1589 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/cli/validation_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3102 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2067 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3417 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      150 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3351 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/net/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4242 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/common/telemetry.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      453 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3140 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3500 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3421 2024-04-25 11:14:48.000000 fedn-0.9.3/fedn/build/lib/fedn/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/common/net/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4381 2024-04-29 15:30:02.000000 fedn-0.9.3/fedn/build/lib/fedn/common/telemetry.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2613 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24174 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    38098 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5186 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    19873 2024-04-26 14:34:42.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11190 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/client_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10343 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/combiner_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18235 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/model_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13598 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/package_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9335 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/round_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9284 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/session_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2131 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12614 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/status_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13391 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/validation_routes.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    33413 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6311 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6038 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      733 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-04-25 14:14:25.000000 fedn-0.9.3/fedn/build/lib/fedn/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5394 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/aggregator.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6876 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4424 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5976 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/fedopt.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    26358 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4765 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10404 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7614 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14932 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      348 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14418 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11434 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3564 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      662 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1414 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      493 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1313 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1222 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1706 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3291 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1292 2024-04-26 09:11:17.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3968 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4014 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.651931 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    30469 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1041 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/client_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/combiner_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/model_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/package_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/round_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/session_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/status_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/validation_store.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/fedn/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      526 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9845 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/dispatcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4138 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/environment.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/fedn/utils/flowercompat/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-04-25 08:28:51.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/flowercompat/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4839 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/flowercompat/client_app_adapter.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1407 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1316 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-03-01 14:47:16.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3448 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4711 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/plugins/numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15870 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6210 2024-04-29 15:17:52.000000 fedn-0.9.3/fedn/build/lib/fedn/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2480 2024-05-08 12:08:13.000000 fedn-0.9.3/fedn/build/lib/network/api/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24363 2024-05-08 12:08:24.000000 fedn-0.9.3/fedn/build/lib/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    37477 2024-05-08 12:08:34.000000 fedn-0.9.3/fedn/build/lib/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5100 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    19749 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/api/v1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11104 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/client_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10257 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/combiner_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18069 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/model_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13472 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/package_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9249 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/round_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9198 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/session_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2073 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12348 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/status_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13119 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/api/v1/validation_routes.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32985 2024-05-08 12:08:57.000000 fedn-0.9.3/fedn/build/lib/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6060 2024-05-08 12:09:36.000000 fedn-0.9.3/fedn/build/lib/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6309 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      732 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7016 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4441 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10765 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/fedopt.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    25744 2024-05-08 12:10:18.000000 fedn-0.9.3/fedn/build/lib/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4668 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10147 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7520 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14996 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      321 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14269 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11253 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3558 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/grpc/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      659 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1409 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      490 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1311 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1216 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1699 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3270 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1289 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3886 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3904 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    29643 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1022 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/client_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/combiner_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/model_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/package_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/round_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/session_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/status_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/network/storage/statestore/stores/validation_store.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      525 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9514 2024-05-08 12:07:42.000000 fedn-0.9.3/fedn/build/lib/utils/dispatcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4199 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/environment.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/utils/flowercompat/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/flowercompat/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4592 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/flowercompat/client_app_adapter.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1399 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1315 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.655931 fedn-0.9.3/fedn/build/lib/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3394 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4936 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/helpers/plugins/numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1639 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/parameters.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15222 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6213 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/build/lib/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/cli/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      533 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/cli/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5725 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/client_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3729 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/combiner_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1488 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/config_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      262 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/main.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1544 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/model_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2386 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/package_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1544 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/round_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     8115 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/run_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1562 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/session_cmd.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2718 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1559 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/status_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/cli/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/cli/tests/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2294 2023-11-21 14:46:43.000000 fedn-0.9.3/fedn/cli/tests/tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1589 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/cli/validation_cmd.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/common/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/common/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/common/certificate/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/common/certificate/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3102 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/common/certificate/certificate.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2067 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/common/certificate/certificatemanager.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3417 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/common/config.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      150 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/common/exceptions.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3351 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/common/log_config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/common/net/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/common/net/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      260 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/api/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      130 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2205 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/network/api/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    24291 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    37406 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/interface.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5029 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/network.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    19749 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/server.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14651 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/tests.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/api/v1/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      614 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11104 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/client_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10257 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/combiner_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    18069 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/v1/model_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13472 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/package_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9249 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/round_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     9198 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/v1/session_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2073 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/api/v1/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    12348 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/status_routes.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    13119 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/api/v1/validation_routes.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/clients/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      445 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/clients/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32803 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/clients/client.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5576 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/clients/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6238 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/clients/package.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      632 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/network/clients/state.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1564 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/clients/test_client.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/combiner/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      147 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/combiner/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/combiner/aggregators/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      250 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/combiner/aggregators/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6884 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/aggregators/aggregatorbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4370 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/aggregators/fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10765 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/aggregators/fedopt.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/combiner/aggregators/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1031 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/combiner/aggregators/tests/test_fedavg.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    25576 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/combiner.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/combiner/combiner_tests.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4597 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/connect.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10057 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/interfaces.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7145 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/modelservice.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14925 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/combiner/roundhandler.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      321 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/config.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/controller/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      216 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/controller/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14198 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/controller/control.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    11182 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/controller/controlbase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/grpc/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       40 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/grpc/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3558 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/grpc/auth.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    10980 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/grpc/fedn_pb2.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    32182 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/grpc/fedn_pb2_grpc.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2260 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/grpc/server.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/loadbalancer/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       96 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/loadbalancer/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      588 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/loadbalancer/firstavailable.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1338 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/loadbalancer/leastpacked.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      418 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/network/loadbalancer/loadbalancerbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1151 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/network/state.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       95 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/__init__.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/models/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      322 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/models/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1145 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/models/memorymodelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1627 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/network/storage/models/modelstorage.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3199 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/models/tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/models/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4155 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/models/tests/test_tempmodelstorage.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/s3/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      302 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/s3/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1289 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/s3/base.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3815 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/s3/miniorepository.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3833 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/s3/repository.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/statestore/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       81 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/statestore/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    29572 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/mongostatestore.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1022 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/statestore/statestorebase.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/network/storage/statestore/stores/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3337 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/client_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4286 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/combiner_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     7032 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/model_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     5190 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/package_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3054 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/round_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3552 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/session_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      174 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/shared.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3732 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/status_store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     2576 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/store.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3792 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/network/storage/statestore/stores/validation_store.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      442 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      441 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/utils/checksum.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     8994 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/dispatcher.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4128 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/environment.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/flowercompat/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       42 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/flowercompat/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4520 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/utils/flowercompat/client_app_adapter.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/helpers/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      158 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/helpers/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1399 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/helpers/helperbase.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1131 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/utils/helpers/helpers.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/helpers/plugins/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        0 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/helpers/plugins/__init__.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     3323 2024-05-14 19:51:01.000000 fedn-0.9.3/fedn/utils/helpers/plugins/androidhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     4865 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/helpers/plugins/numpyhelper.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/helpers/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1818 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/helpers/tests/test_numpyhelper.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1639 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/parameters.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    15222 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/plots.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     6036 2024-05-22 12:54:10.000000 fedn-0.9.3/fedn/utils/process.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn/utils/tests/
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1682 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/tests/test_helpers.py
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     1615 2024-05-08 09:23:36.000000 fedn-0.9.3/fedn/utils/tests/test_parameters.py
-drwxrwxr-x   0 stefan    (1000) stefan    (1000)        0 2024-05-22 12:55:51.659931 fedn-0.9.3/fedn.egg-info/
--rw-r--r--   0 stefan    (1000) stefan    (1000)    20324 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/PKG-INFO
--rw-rw-r--   0 stefan    (1000) stefan    (1000)    14291 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/SOURCES.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        1 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/dependency_links.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       44 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/entry_points.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)      211 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/requires.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)        5 2024-05-22 12:55:51.000000 fedn-0.9.3/fedn.egg-info/top_level.txt
--rw-rw-r--   0 stefan    (1000) stefan    (1000)     8242 2024-05-22 12:54:17.000000 fedn-0.9.3/pyproject.toml
--rw-rw-r--   0 stefan    (1000) stefan    (1000)       38 2024-05-22 12:55:51.663931 fedn-0.9.3/setup.cfg
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

### Comparing `fedn-0.9.3/LICENSE` & `fedn-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/PKG-INFO` & `fedn-0.9.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.3
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

### Comparing `fedn-0.9.3/README.rst` & `fedn-0.9.5/README.rst`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/__init__.py` & `fedn-0.9.5/fedn/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/cli/client_cmd.py` & `fedn-0.9.5/fedn/cli/client_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/combiner_cmd.py` & `fedn-0.9.5/fedn/cli/combiner_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/config_cmd.py` & `fedn-0.9.5/fedn/cli/config_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/model_cmd.py` & `fedn-0.9.5/fedn/cli/model_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/package_cmd.py` & `fedn-0.9.5/fedn/cli/package_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/round_cmd.py` & `fedn-0.9.5/fedn/cli/round_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/run_cmd.py` & `fedn-0.9.5/fedn/cli/run_cmd.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,28 +3,25 @@
 import uuid
 
 import click
 import yaml
 
 from fedn.common.exceptions import InvalidClientConfig
 from fedn.common.log_config import logger
-from fedn.common.telemetry import get_context, tracer
 from fedn.network.clients.client import Client
 from fedn.network.combiner.combiner import Combiner
 from fedn.utils.dispatcher import Dispatcher, _read_yaml_file
 
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
@@ -37,36 +34,18 @@
         helper = control["helper"]
     except KeyError:
         logger.error("--local-package was used, but no helper was found in --init settings file.")
         exit(-1)
     return helper
 
 
-def sanitize_config(config):
-    # List of keys to sanitize (remove or mask)
-    sensitive_keys = ["discover_host",
-                      "discover_port",
-                      "name",
-                      "token",
-                      "client_id",
-                      "preshared_cert"
-                      ]
-
-    # Create a sanitized copy of the dictionary
-    sanitized_config = {key: (config[key] if key not in sensitive_keys else "***") for key in config}
-
-    return sanitized_config
-
-
-@main.group('run')
+@main.group("run")
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
@@ -138,17 +117,15 @@
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
@@ -159,54 +136,53 @@
     :param init:
     :param logfile:
     :param hearbeat_interval
     :param reconnect_after_missed_heartbeat
     :param verbosity
     :return:
     """
-    with tracer.start_as_current_span("client_cmd") as span:
-        remote = False if local_package else True
-        config = {
-            "discover_host": discoverhost,
-            "discover_port": discoverport,
-            "token": token,
-            "name": name,
-            "client_id": client_id,
-            "remote_compute_context": remote,
-            "force_ssl": force_ssl,
-            "dry_run": dry_run,
-            "secure": secure,
-            "preshared_cert": preshared_cert,
-            "verify": verify,
-            "preferred_combiner": preferred_combiner,
-            "validator": validator,
-            "trainer": trainer,
-            "logfile": logfile,
-            "heartbeat_interval": heartbeat_interval,
-            "reconnect_after_missed_heartbeat": reconnect_after_missed_heartbeat,
-            "verbosity": verbosity,
-        }
-
-        click.echo(
-            click.style("\n*** fedn run client is deprecated and will be removed. Please use fedn client start instead. ***\n", blink=True, bold=True, fg="red")
-        )
-
-        if init:
-            apply_config(init, config)
-            click.echo(f"\nClient configuration loaded from file: {init}")
-            click.echo("Values set in file override defaults and command line arguments...\n")
+    remote = False if local_package else True
+    config = {
+        "discover_host": discoverhost,
+        "discover_port": discoverport,
+        "token": token,
+        "name": name,
+        "client_id": client_id,
+        "remote_compute_context": remote,
+        "force_ssl": force_ssl,
+        "dry_run": dry_run,
+        "secure": secure,
+        "preshared_cert": preshared_cert,
+        "verify": verify,
+        "preferred_combiner": preferred_combiner,
+        "validator": validator,
+        "trainer": trainer,
+        "logfile": logfile,
+        "heartbeat_interval": heartbeat_interval,
+        "reconnect_after_missed_heartbeat": reconnect_after_missed_heartbeat,
+        "verbosity": verbosity,
+    }
+
+    click.echo(
+        click.style("\n*** fedn run client is deprecated and will be removed. Please use fedn client start instead. ***\n", blink=True, bold=True, fg="red")
+    )
+
+    if init:
+        apply_config(init, config)
+        click.echo(f"\nClient configuration loaded from file: {init}")
+        click.echo("Values set in file override defaults and command line arguments...\n")
 
-        try:
-            validate_client_config(config)
-        except InvalidClientConfig as e:
-            click.echo(f"Error: {e}")
-            return
+    try:
+        validate_client_config(config)
+    except InvalidClientConfig as e:
+        click.echo(f"Error: {e}")
+        return
 
-        client = Client(config)
-        client.run()
+    client = Client(config)
+    client.run()
 
 
 @run_cmd.command("combiner")
 @click.option("-d", "--discoverhost", required=False, help="Hostname for discovery services (reducer).")
 @click.option("-p", "--discoverport", required=False, help="Port for discovery services (reducer).")
 @click.option("-t", "--token", required=False, help="Set token provided by reducer if enabled")
 @click.option("-n", "--name", required=False, default="combiner" + str(uuid.uuid4())[:8], help="Set name for combiner.")
@@ -215,45 +191,42 @@
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
     :param max_clients:
     :param init:
     """
-    with tracer.start_as_current_span("combiner_cmd"):
-        config = {
-            "discover_host": discoverhost,
-            "discover_port": discoverport,
-            "token": token,
-            "host": host,
-            "port": port,
-            "fqdn": fqdn,
-            "name": name,
-            "secure": secure,
-            "verify": verify,
-            "max_clients": max_clients,
-        }
-
-        click.echo(
-            click.style("\n*** fedn run combiner is deprecated and will be removed. Please use fedn combiner start instead. ***\n", blink=True, bold=True, fg="red")
-        )
-
-        if init:
-            apply_config(init, config)
-            click.echo(f"\nCombiner configuration loaded from file: {init}")
-            click.echo("Values set in file override defaults and command line arguments...\n")
+    config = {
+        "discover_host": discoverhost,
+        "discover_port": discoverport,
+        "token": token,
+        "host": host,
+        "port": port,
+        "fqdn": fqdn,
+        "name": name,
+        "secure": secure,
+        "verify": verify,
+        "max_clients": max_clients,
+    }
+
+    click.echo(
+        click.style("\n*** fedn run combiner is deprecated and will be removed. Please use fedn combiner start instead. ***\n", blink=True, bold=True, fg="red")
+    )
+
+    if init:
+        apply_config(init, config)
+        click.echo(f"\nCombiner configuration loaded from file: {init}")
+        click.echo("Values set in file override defaults and command line arguments...\n")
 
-        combiner = Combiner(config)
-        combiner.run()
+    combiner = Combiner(config)
+    combiner.run()
```

### Comparing `fedn-0.9.3/fedn/build/lib/cli/session_cmd.py` & `fedn-0.9.5/fedn/cli/session_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/shared.py` & `fedn-0.9.5/fedn/cli/shared.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/status_cmd.py` & `fedn-0.9.5/fedn/cli/status_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/cli/tests/tests.py` & `fedn-0.9.5/fedn/cli/tests/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/cli/validation_cmd.py` & `fedn-0.9.5/fedn/cli/validation_cmd.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/common/certificate/certificate.py` & `fedn-0.9.5/fedn/common/certificate/certificate.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/common/certificate/certificatemanager.py` & `fedn-0.9.5/fedn/common/certificate/certificatemanager.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/common/config.py` & `fedn-0.9.5/fedn/common/config.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/common/log_config.py` & `fedn-0.9.5/fedn/common/log_config.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/auth.py` & `fedn-0.9.5/fedn/network/api/auth.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,75 +1,73 @@
 from functools import wraps
 
 import jwt
 from flask import jsonify, request
 
-from fedn.common.config import (FEDN_AUTH_SCHEME,
-                                FEDN_AUTH_WHITELIST_URL_PREFIX,
-                                FEDN_JWT_ALGORITHM, FEDN_JWT_CUSTOM_CLAIM_KEY,
-                                FEDN_JWT_CUSTOM_CLAIM_VALUE, SECRET_KEY)
-from fedn.common.telemetry import tracer
+from fedn.common.config import (
+    FEDN_AUTH_SCHEME,
+    FEDN_AUTH_WHITELIST_URL_PREFIX,
+    FEDN_JWT_ALGORITHM,
+    FEDN_JWT_CUSTOM_CLAIM_KEY,
+    FEDN_JWT_CUSTOM_CLAIM_VALUE,
+    SECRET_KEY,
+)
 
 
-@tracer.start_as_current_span(name="check_role_claims")
 def check_role_claims(payload, role):
-    if 'role' not in payload:
+    if "role" not in payload:
         return False
-    if payload['role'] != role:
+    if payload["role"] != role:
         return False
 
     return True
 
 
-@tracer.start_as_current_span(name="check_custom_claims")
 def check_custom_claims(payload):
     if FEDN_JWT_CUSTOM_CLAIM_KEY and FEDN_JWT_CUSTOM_CLAIM_VALUE:
         if payload[FEDN_JWT_CUSTOM_CLAIM_KEY] != FEDN_JWT_CUSTOM_CLAIM_VALUE:
             return False
     return True
 
 
-@tracer.start_as_current_span(name="if_whitelisted_url_prefix")
 def if_whitelisted_url_prefix(path):
     if FEDN_AUTH_WHITELIST_URL_PREFIX and path.startswith(FEDN_AUTH_WHITELIST_URL_PREFIX):
         return True
     else:
         return False
 
 
-@tracer.start_as_current_span(name="jwt_auth_required")
 def jwt_auth_required(role=None):
     def actual_decorator(func):
         if not SECRET_KEY:
             return func
 
         @wraps(func)
         def decorated(*args, **kwargs):
             if if_whitelisted_url_prefix(request.path):
                 return func(*args, **kwargs)
-            token = request.headers.get('Authorization')
+            token = request.headers.get("Authorization")
             if not token:
-                return jsonify({'message': 'Missing token'}), 401
+                return jsonify({"message": "Missing token"}), 401
             # Get token from the header Bearer
             if token.startswith(FEDN_AUTH_SCHEME):
-                token = token.split(' ')[1]
+                token = token.split(" ")[1]
             else:
-                return jsonify({'message':
-                                f'Invalid token scheme, expected {FEDN_AUTH_SCHEME}'
-                                }), 401
+                return jsonify({"message": f"Invalid token scheme, expected {FEDN_AUTH_SCHEME}"}), 401
             try:
                 payload = jwt.decode(token, SECRET_KEY, algorithms=[FEDN_JWT_ALGORITHM])
                 if not check_role_claims(payload, role):
-                    return jsonify({'message': 'Invalid token'}), 401
+                    return jsonify({"message": "Invalid token"}), 401
                 if not check_custom_claims(payload):
-                    return jsonify({'message': 'Invalid token'}), 401
+                    return jsonify({"message": "Invalid token"}), 401
 
             except jwt.ExpiredSignatureError:
-                return jsonify({'message': 'Token expired'}), 401
+                return jsonify({"message": "Token expired"}), 401
 
             except jwt.InvalidTokenError:
-                return jsonify({'message': 'Invalid token'}), 401
+                return jsonify({"message": "Invalid token"}), 401
 
             return func(*args, **kwargs)
 
         return decorated
+
     return actual_decorator
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/client.py` & `fedn-0.9.5/fedn/network/api/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import os
 
 import requests
 
-from fedn.common.telemetry import trace_all_methods
+__all__ = ["APIClient"]
 
-__all__ = ['APIClient']
 
-
-@trace_all_methods
 class APIClient:
-    """ An API client for interacting with the statestore and controller.
+    """An API client for interacting with the statestore and controller.
 
     :param host: The host of the api server.
     :type host: str
     :param port: The port of the api server.
     :type port: int
     :param secure: Whether to use https.
     :type secure: bool
@@ -36,250 +33,248 @@
             token = os.environ.get("FEDN_AUTH_TOKEN", False)
 
         if token:
             self.headers = {"Authorization": f"{auth_scheme} {token}"}
 
     def _get_url(self, endpoint):
         if self.secure:
-            protocol = 'https'
+            protocol = "https"
         else:
-            protocol = 'http'
+            protocol = "http"
         if self.port:
-            return f'{protocol}://{self.host}:{self.port}/{endpoint}'
-        return f'{protocol}://{self.host}/{endpoint}'
+            return f"{protocol}://{self.host}:{self.port}/{endpoint}"
+        return f"{protocol}://{self.host}/{endpoint}"
 
     def _get_url_api_v1(self, endpoint):
-        return self._get_url(f'api/v1/{endpoint}')
+        return self._get_url(f"api/v1/{endpoint}")
 
     # --- Clients --- #
 
     def get_client(self, id: str):
-        """ Get a client from the statestore.
+        """Get a client from the statestore.
 
         :param id: The client id to get.
         :type id: str
         :return: Client.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'clients/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"clients/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_clients(self, n_max: int = None):
-        """ Get clients from the statestore.
+        """Get clients from the statestore.
 
         :param n_max: The maximum number of clients to get (If none all will be fetched).
         :type n_max: int
         return: Clients.
         rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('clients'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("clients/"), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_clients_count(self):
-        """ Get the number of clients in the statestore.
+        """Get the number of clients in the statestore.
 
         :return: The number of clients.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('clients/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("clients/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_client_config(self, checksum=True):
-        """ Get client config from controller. Optionally include the checksum.
+        """Get client config from controller. Optionally include the checksum.
         The config is used for clients to connect to the controller and ask for combiner assignment.
 
         :param checksum: Whether to include the checksum of the package.
         :type checksum: bool
         :return: The client configuration.
         :rtype: dict
         """
-        _params = {
-            'checksum': "true" if checksum else "false"
-        }
+        _params = {"checksum": "true" if checksum else "false"}
 
-        response = requests.get(self._get_url('get_client_config'), params=_params, verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url("get_client_config"), params=_params, verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_active_clients(self, combiner_id: str = None, n_max: int = None):
-        """ Get active clients from the statestore.
+        """Get active clients from the statestore.
 
         :param combiner_id: The combiner id to get active clients for.
         :type combiner_id: str
         :param n_max: The maximum number of clients to get (If none all will be fetched).
         :type n_max: int
         :return: Active clients.
         :rtype: dict
         """
         _params = {"status": "online"}
 
         if combiner_id:
-            _params['combiner'] = combiner_id
+            _params["combiner"] = combiner_id
 
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('clients/'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("clients/"), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     # --- Combiners --- #
 
     def get_combiner(self, id: str):
-        """ Get a combiner from the statestore.
+        """Get a combiner from the statestore.
 
         :param id: The combiner id to get.
         :type id: str
         :return: Combiner.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'combiners/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"combiners/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_combiners(self, n_max: int = None):
-        """ Get combiners in the network.
+        """Get combiners in the network.
 
         :param n_max: The maximum number of combiners to get (If none all will be fetched).
         :type n_max: int
         :return: Combiners.
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('combiners/'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("combiners/"), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_combiners_count(self):
-        """ Get the number of combiners in the statestore.
+        """Get the number of combiners in the statestore.
 
         :return: The number of combiners.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('combiners/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("combiners/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     # --- Controllers --- #
 
     def get_controller_status(self):
-        """ Get the status of the controller.
+        """Get the status of the controller.
 
         :return: The status of the controller.
         :rtype: dict
         """
-        response = requests.get(self._get_url('get_controller_status'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url("get_controller_status"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     # --- Models --- #
 
     def get_model(self, id: str):
-        """ Get a model from the statestore.
+        """Get a model from the statestore.
 
         :param id: The id (or model property) of the model to get.
         :type id: str
         :return: Model.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'models/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"models/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_models(self, session_id: str = None, n_max: int = None):
-        """ Get models from the statestore.
+        """Get models from the statestore.
 
         :param session_id: The session id to get models for. (optional)
         :type session_id: str
         :param n_max: The maximum number of models to get (If none all will be fetched).
         :type n_max: int
         :return: Models.
         :rtype: dict
         """
         _params = {}
 
         if session_id:
-            _params['session_id'] = session_id
+            _params["session_id"] = session_id
 
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('models/'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("models/"), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_models_count(self):
-        """ Get the number of models in the statestore.
+        """Get the number of models in the statestore.
 
         :return: The number of models.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('models/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("models/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_active_model(self):
-        """ Get the latest model from the statestore.
+        """Get the latest model from the statestore.
 
         :return: The latest model.
         :rtype: dict
         """
         _headers = self.headers.copy()
-        _headers['X-Limit'] = "1"
+        _headers["X-Limit"] = "1"
 
-        response = requests.get(self._get_url_api_v1('models/'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("models/"), verify=self.verify, headers=_headers)
         _json = response.json()
 
         if "result" in _json and len(_json["result"]) > 0:
             return _json["result"][0]
 
         return _json
 
     def get_model_trail(self, id: str = None, include_self: bool = True, reverse: bool = True, n_max: int = None):
-        """ Get the model trail.
+        """Get the model trail.
 
         :param id: The id (or model property) of the model to start the trail from. (optional)
         :type id: str
         :param n_max: The maximum number of models to get (If none all will be fetched).
         :type n_max: int
         :return: Models.
         :rtype: dict
@@ -290,294 +285,301 @@
                 id = model["id"]
             else:
                 return model
 
         _headers = self.headers.copy()
 
         _count: int = n_max if n_max else self.get_models_count()
-        _headers['X-Limit'] = str(_count)
-        _headers['X-Reverse'] = "true" if reverse else "false"
+        _headers["X-Limit"] = str(_count)
+        _headers["X-Reverse"] = "true" if reverse else "false"
 
         _include_self_str: str = "true" if include_self else "false"
 
-        response = requests.get(self._get_url_api_v1(f'models/{id}/ancestors?include_self={_include_self_str}'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1(f"models/{id}/ancestors?include_self={_include_self_str}"), verify=self.verify, headers=_headers)
         _json = response.json()
 
         return _json
 
     def download_model(self, id: str, path: str):
-        """ Download the model with id id.
+        """Download the model with id id.
 
         :param id: The id (or model property) of the model to download.
         :type id: str
         :param path: The path to download the model to.
         :type path: str
         :return: Message with success or failure.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'models/{id}/download'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"models/{id}/download"), verify=self.verify, headers=self.headers)
 
         if response.status_code == 200:
-
-            with open(path, 'wb') as file:
+            with open(path, "wb") as file:
                 file.write(response.content)
-            return {'success': True, 'message': 'Model downloaded successfully.'}
+            return {"success": True, "message": "Model downloaded successfully."}
         else:
-            return {'success': False, 'message': 'Failed to download model.'}
+            return {"success": False, "message": "Failed to download model."}
 
     def set_active_model(self, path):
-        """ Set the initial model in the statestore and upload to model repository.
+        """Set the initial model in the statestore and upload to model repository.
 
         :param path: The file path of the initial model to set.
         :type path: str
         :return: A dict with success or failure message.
         :rtype: dict
         """
-        with open(path, 'rb') as file:
-            response = requests.post(self._get_url('set_initial_model'), files={'file': file}, verify=self.verify, headers=self.headers)
+        with open(path, "rb") as file:
+            response = requests.post(self._get_url("set_initial_model"), files={"file": file}, verify=self.verify, headers=self.headers)
         return response.json()
 
     # --- Packages --- #
 
     def get_package(self, id: str):
-        """ Get a compute package from the statestore.
+        """Get a compute package from the statestore.
 
         :param id: The id of the compute package to get.
         :type id: str
         :return: Package.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'packages/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"packages/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_packages(self, n_max: int = None):
-        """ Get compute packages from the statestore.
+        """Get compute packages from the statestore.
 
         :param n_max: The maximum number of packages to get (If none all will be fetched).
         :type n_max: int
         :return: Packages.
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('packages/'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("packages/"), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_packages_count(self):
-        """ Get the number of compute packages in the statestore.
+        """Get the number of compute packages in the statestore.
 
         :return: The number of packages.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('packages/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("packages/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_active_package(self):
-        """ Get the (active) compute package from the statestore.
+        """Get the (active) compute package from the statestore.
 
         :return: Package.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('packages/active'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("packages/active"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_package_checksum(self):
-        """ Get the checksum of the compute package.
+        """Get the checksum of the compute package.
 
         :return: The checksum.
         :rtype: dict
         """
-        response = requests.get(self._get_url('get_package_checksum'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url("get_package_checksum"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def download_package(self, path: str):
-        """ Download the compute package.
+        """Download the compute package.
 
         :param path: The path to download the compute package to.
         :type path: str
         :return: Message with success or failure.
         :rtype: dict
         """
-        response = requests.get(self._get_url('download_package'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url("download_package"), verify=self.verify, headers=self.headers)
         if response.status_code == 200:
-            with open(path, 'wb') as file:
+            with open(path, "wb") as file:
                 file.write(response.content)
-            return {'success': True, 'message': 'Package downloaded successfully.'}
+            return {"success": True, "message": "Package downloaded successfully."}
         else:
-            return {'success': False, 'message': 'Failed to download package.'}
+            return {"success": False, "message": "Failed to download package."}
 
     def set_active_package(self, path: str, helper: str, name: str = None, description: str = None):
-        """ Set the compute package in the statestore.
+        """Set the compute package in the statestore.
 
         :param path: The file path of the compute package to set.
         :type path: str
         :param helper: The helper type to use.
         :type helper: str
         :return: A dict with success or failure message.
         :rtype: dict
         """
-        with open(path, 'rb') as file:
-            response = requests.post(self._get_url('set_package'), files={'file': file}, data={
-                                     'helper': helper, 'name': name, 'description': description}, verify=self.verify, headers=self.headers)
+        with open(path, "rb") as file:
+            response = requests.post(
+                self._get_url("set_package"),
+                files={"file": file},
+                data={"helper": helper, "name": name, "description": description},
+                verify=self.verify,
+                headers=self.headers,
+            )
 
         _json = response.json()
 
         return _json
 
     # --- Rounds --- #
 
     def get_round(self, id: str):
-        """ Get a round from the statestore.
+        """Get a round from the statestore.
 
         :param round_id: The round id to get.
         :type round_id: str
         :return: Round (config and metrics).
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'rounds/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"rounds/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_rounds(self, n_max: int = None):
-        """ Get all rounds from the statestore.
+        """Get all rounds from the statestore.
 
         :param n_max: The maximum number of rounds to get (If none all will be fetched).
         :type n_max: int
         :return: Rounds.
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('rounds/'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("rounds/"), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_rounds_count(self):
-        """ Get the number of rounds in the statestore.
+        """Get the number of rounds in the statestore.
 
         :return: The number of rounds.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('rounds/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("rounds/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     # --- Sessions --- #
 
     def get_session(self, id: str):
-        """ Get a session from the statestore.
+        """Get a session from the statestore.
 
         :param id: The session id to get.
         :type id: str
         :return: Session.
         :rtype: dict
         """
-
-        response = requests.get(self._get_url_api_v1(f'sessions/{id}'), self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"sessions/{id}"), self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_sessions(self, n_max: int = None):
-        """ Get sessions from the statestore.
+        """Get sessions from the statestore.
 
         :param n_max: The maximum number of sessions to get (If none all will be fetched).
         :type n_max: int
         :return: Sessions.
         :rtype: dict
         """
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('sessions/'), verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("sessions/"), verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_sessions_count(self):
-        """ Get the number of sessions in the statestore.
+        """Get the number of sessions in the statestore.
 
         :return: The number of sessions.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('sessions/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("sessions/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_session_status(self, id: str):
-        """ Get the status of a session.
+        """Get the status of a session.
 
         :param id: The id of the session to get.
         :type id: str
         :return: The status of the session.
         :rtype: str
         """
         session = self.get_session(id)
 
         if session and "status" in session:
             return session["status"]
 
         return "Could not retrieve session status."
 
     def session_is_finished(self, id: str):
-        """ Check if a session with id has finished.
+        """Check if a session with id has finished.
 
         :param id: The id of the session to get.
         :type id: str
         :return: True if session is finished, otherwise false.
         :rtype: bool
         """
         status = self.get_session_status(id)
         return status and status.lower() == "finished"
 
     def start_session(
-            self,
-            id: str = None,
-            aggregator: str = 'fedavg',
-            model_id:  str = None,
-            round_timeout: int = 180,
-            rounds: int = 5,
-            round_buffer_size: int = -1,
-            delete_models: bool = True,
-            validate: bool = True, helper: str = 'numpyhelper', min_clients: int = 1, requested_clients: int = 8
+        self,
+        id: str = None,
+        aggregator: str = "fedavg",
+        aggregator_kwargs: dict = None,
+        model_id: str = None,
+        round_timeout: int = 180,
+        rounds: int = 5,
+        round_buffer_size: int = -1,
+        delete_models: bool = True,
+        validate: bool = True,
+        helper: str = "numpyhelper",
+        min_clients: int = 1,
+        requested_clients: int = 8,
     ):
-        """ Start a new session.
+        """Start a new session.
 
         :param id: The session id to start.
         :type id: str
         :param aggregator: The aggregator plugin to use.
         :type aggregator: str
         :param model_id: The id of the initial model.
         :type model_id: str
@@ -596,50 +598,56 @@
         :param min_clients: The minimum number of clients required.
         :type min_clients: int
         :param requested_clients: The requested number of clients.
         :type requested_clients: int
         :return: A dict with success or failure message and session config.
         :rtype: dict
         """
-        response = requests.post(self._get_url('start_session'), json={
-            'session_id': id,
-            'aggregator': aggregator,
-            'model_id': model_id,
-            'round_timeout': round_timeout,
-            'rounds': rounds,
-            'round_buffer_size': round_buffer_size,
-            'delete_models': delete_models,
-            'validate': validate,
-            'helper': helper,
-            'min_clients': min_clients,
-            'requested_clients': requested_clients
-        }, verify=self.verify, headers=self.headers)
+        response = requests.post(
+            self._get_url("start_session"),
+            json={
+                "session_id": id,
+                "aggregator": aggregator,
+                "aggregator_kwargs": aggregator_kwargs,
+                "model_id": model_id,
+                "round_timeout": round_timeout,
+                "rounds": rounds,
+                "round_buffer_size": round_buffer_size,
+                "delete_models": delete_models,
+                "validate": validate,
+                "helper": helper,
+                "min_clients": min_clients,
+                "requested_clients": requested_clients,
+            },
+            verify=self.verify,
+            headers=self.headers,
+        )
 
         _json = response.json()
 
         return _json
 
     # --- Statuses --- #
 
     def get_status(self, id: str):
-        """ Get a status object (event) from the statestore.
+        """Get a status object (event) from the statestore.
 
         :param id: The id of the status to get.
         :type id: str
         :return: Status.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'statuses/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"statuses/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_statuses(self, session_id: str = None, event_type: str = None, sender_name: str = None, sender_role: str = None, n_max: int = None):
-        """ Get statuses from the statestore. Filter by input parameters
+        """Get statuses from the statestore. Filter by input parameters
 
         :param session_id: The session id to get statuses for.
         :type session_id: str
         :param event_type: The event type to get.
         :type event_type: str
         :param sender_name: The sender name to get.
         :type sender_name: str
@@ -662,62 +670,62 @@
 
         if sender_role:
             _params["sender.role"] = sender_role
 
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('statuses/'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("statuses/"), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_statuses_count(self):
-        """ Get the number of statuses in the statestore.
+        """Get the number of statuses in the statestore.
 
         :return: The number of statuses.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('statuses/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("statuses/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     # --- Validations --- #
 
     def get_validation(self, id: str):
-        """ Get a validation from the statestore.
+        """Get a validation from the statestore.
 
         :param id: The id of the validation to get.
         :type id: str
         :return: Validation.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1(f'validations/{id}'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1(f"validations/{id}"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
 
     def get_validations(
         self,
         session_id: str = None,
         model_id: str = None,
         correlation_id: str = None,
         sender_name: str = None,
         sender_role: str = None,
         receiver_name: str = None,
         receiver_role: str = None,
-        n_max: int = None
+        n_max: int = None,
     ):
-        """ Get validations from the statestore. Filter by input parameters.
+        """Get validations from the statestore. Filter by input parameters.
 
         :param session_id: The session id to get validations for.
         :type session_id: str
         :param model_id: The model id to get validations for.
         :type model_id: str
         :param correlation_id: The correlation id to get validations for.
         :type correlation_id: str
@@ -756,26 +764,26 @@
 
         if receiver_role:
             _params["receiver.role"] = receiver_role
 
         _headers = self.headers.copy()
 
         if n_max:
-            _headers['X-Limit'] = str(n_max)
+            _headers["X-Limit"] = str(n_max)
 
-        response = requests.get(self._get_url_api_v1('validations/'), params=_params, verify=self.verify, headers=_headers)
+        response = requests.get(self._get_url_api_v1("validations/"), params=_params, verify=self.verify, headers=_headers)
 
         _json = response.json()
 
         return _json
 
     def get_validations_count(self):
-        """ Get the number of validations in the statestore.
+        """Get the number of validations in the statestore.
 
         :return: The number of validations.
         :rtype: dict
         """
-        response = requests.get(self._get_url_api_v1('validations/count'), verify=self.verify, headers=self.headers)
+        response = requests.get(self._get_url_api_v1("validations/count"), verify=self.verify, headers=self.headers)
 
         _json = response.json()
 
         return _json
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/interface.py` & `fedn-0.9.5/fedn/network/api/interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,25 +6,22 @@
 from io import BytesIO
 
 from flask import jsonify, send_from_directory
 from werkzeug.utils import secure_filename
 
 from fedn.common.config import get_controller_config, get_network_config
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
-from fedn.network.combiner.interfaces import (CombinerInterface,
-                                              CombinerUnavailableError)
+from fedn.network.combiner.interfaces import CombinerInterface, CombinerUnavailableError
 from fedn.network.state import ReducerState, ReducerStateToString
 from fedn.utils.checksum import sha
 from fedn.utils.plots import Plot
 
 __all__ = ("API",)
 
 
-@trace_all_methods
 class API:
     """The API class is a wrapper for the statestore. It is used to expose the statestore to the network API."""
 
     def __init__(self, statestore, control):
         self.statestore = statestore
         self.control = control
         self.name = "api"
@@ -34,17 +31,15 @@
 
         ::return: The object as a dict.
         ::rtype: dict
         """
         data = {"name": self.name}
         return data
 
-    def _allowed_file_extension(
-        self, filename, ALLOWED_EXTENSIONS={"gz", "bz2", "tar", "zip", "tgz"}
-    ):
+    def _allowed_file_extension(self, filename, ALLOWED_EXTENSIONS={"gz", "bz2", "tar", "zip", "tgz"}):
         """Check if file extension is allowed.
 
         :param filename: The filename to check.
         :type filename: str
         :return: True and extension str if file extension is allowed, else False and None.
         :rtype: Tuple (bool, str)
         """
@@ -168,19 +163,18 @@
                 404,
             )
         payload = {}
         id = session_object["session_id"]
         info = session_object["session_config"][0]
         status = session_object["status"]
         payload[id] = info
-        payload['status'] = status
+        payload["status"] = status
         return jsonify(payload)
 
     def set_active_compute_package(self, id: str):
-
         success = self.statestore.set_active_compute_package(id)
 
         if not success:
             return (
                 jsonify(
                     {
                         "success": False,
@@ -196,25 +190,20 @@
         """Set the compute package in the statestore.
 
         :param file: The compute package to set.
         :type file: file
         :return: A json response with success or failure message.
         :rtype: :class:`flask.Response`
         """
-
-        if (
-            self.control.state() == ReducerState.instructing
-            or self.control.state() == ReducerState.monitoring
-        ):
+        if self.control.state() == ReducerState.instructing or self.control.state() == ReducerState.monitoring:
             return (
                 jsonify(
                     {
                         "success": False,
-                        "message": "Reducer is in instructing or monitoring state."
-                        "Cannot set compute package.",
+                        "message": "Reducer is in instructing or monitoring state." "Cannot set compute package.",
                     }
                 ),
                 400,
             )
 
         if file is None:
             return (
@@ -286,17 +275,15 @@
 
         :return: The compute package as a json response.
         :rtype: :class:`flask.Response`
         """
         result = self.statestore.get_compute_package()
         if result is None:
             return (
-                jsonify(
-                    {"success": False, "message": "No compute package found."}
-                ),
+                jsonify({"success": False, "message": "No compute package found."}),
                 404,
             )
 
         obj = {
             "id": result["id"] if "id" in result else "",
             "file_name": result["file_name"],
             "helper": result["helper"],
@@ -315,27 +302,24 @@
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
         if result is None:
             return (
-                jsonify(
-                    {"success": False, "message": "No compute packages found."}
-                ),
+                jsonify({"success": False, "message": "No compute packages found."}),
                 404,
             )
 
         active_package_id: str = None
 
         if include_active:
             active_package = self.statestore.get_compute_package()
@@ -384,49 +368,42 @@
             name, message = self._get_compute_package_name()
             if name is None:
                 return jsonify({"success": False, "message": message}), 404
         try:
             mutex = threading.Lock()
             mutex.acquire()
             # TODO: make configurable, perhaps in config.py or package.py
-            return send_from_directory(
-                "/app/client/package/", name, as_attachment=True
-            )
+            return send_from_directory("/app/client/package/", name, as_attachment=True)
         except Exception:
             try:
                 data = self.control.get_compute_package(name)
                 # TODO: make configurable, perhaps in config.py or package.py
                 file_path = os.path.join("/app/client/package/", name)
                 with open(file_path, "wb") as fh:
                     fh.write(data)
                 # TODO: make configurable, perhaps in config.py or package.py
-                return send_from_directory(
-                    "/app/client/package/", name, as_attachment=True
-                )
+                return send_from_directory("/app/client/package/", name, as_attachment=True)
             except Exception:
                 raise
         finally:
             mutex.release()
 
     def _create_checksum(self, name=None):
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
-        file_path = os.path.join(
-            "/app/client/package/", name
-        )  # TODO: make configurable, perhaps in config.py or package.py
+        file_path = os.path.join("/app/client/package/", name)  # TODO: make configurable, perhaps in config.py or package.py
         try:
             sum = str(sha(file_path))
         except FileNotFoundError:
             sum = ""
             message = "File not found."
         return True, message, sum
 
@@ -434,15 +411,14 @@
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
 
@@ -503,17 +479,15 @@
                 "meta": object["meta"],
                 "sender": object["sender"],
                 "receiver": object["receiver"],
             }
             payload[id] = info
         return jsonify(payload)
 
-    def add_combiner(
-        self, combiner_id, secure_grpc, address, remote_addr, fqdn, port
-    ):
+    def add_combiner(self, combiner_id, secure_grpc, address, remote_addr, fqdn, port):
         """Add a combiner to the network.
 
         :param combiner_id: The combiner id to add.
         :type combiner_id: str
         :param secure_grpc: Whether to use secure grpc or not.
         :type secure_grpc: bool
         :param name: The name of the combiner.
@@ -538,17 +512,15 @@
                     "message": "Conroller is not in idle state, try again later. ",
                 }
             )
         # Check if combiner already exists
         combiner = self.control.network.get_combiner(combiner_id)
         if not combiner:
             if secure_grpc == "True":
-                certificate, key = self.certificate_manager.get_or_create(
-                    address
-                ).get_keypair_raw()
+                certificate, key = self.certificate_manager.get_or_create(address).get_keypair_raw()
                 _ = base64.b64encode(certificate)
                 _ = base64.b64encode(key)
 
             else:
                 certificate = None
                 key = None
 
@@ -564,17 +536,15 @@
             )
 
             self.control.network.add_combiner(combiner_interface)
 
         # Check combiner now exists
         combiner = self.control.network.get_combiner(combiner_id)
         if not combiner:
-            return jsonify(
-                {"success": False, "message": "Combiner not added."}
-            )
+            return jsonify({"success": False, "message": "Combiner not added."})
 
         payload = {
             "success": True,
             "message": "Combiner added successfully.",
             "status": "added",
             "storage": self.statestore.get_storage_backend(),
             "statestore": self.statestore.get_config(),
@@ -621,17 +591,15 @@
                     ),
                     400,
                 )
         else:
             combiner = self.control.network.find_available_combiner()
             if combiner is None:
                 return (
-                    jsonify(
-                        {"success": False, "message": "No combiner available."}
-                    ),
+                    jsonify({"success": False, "message": "No combiner available."}),
                     400,
                 )
 
         client_config = {
             "name": client_id,
             "combiner_preferred": preferred_combiner,
             "combiner": combiner.name,
@@ -689,32 +657,28 @@
             object.seek(0)
             model = helper.load(object)
             self.control.commit(file.filename, model)
         except Exception as e:
             logger.debug(e)
             return jsonify({"success": False, "message": e})
 
-        return jsonify(
-            {"success": True, "message": "Initial model added successfully."}
-        )
+        return jsonify({"success": True, "message": "Initial model added successfully."})
 
     def get_latest_model(self):
         """Get the latest model from the statestore.
 
         :return: The initial model as a json response.
         :rtype: :class:`flask.Response`
         """
         if self.statestore.get_latest_model():
             model_id = self.statestore.get_latest_model()
             payload = {"model_id": model_id}
             return jsonify(payload)
         else:
-            return jsonify(
-                {"success": False, "message": "No initial model set."}
-            )
+            return jsonify({"success": False, "message": "No initial model set."})
 
     def set_current_model(self, model_id: str):
         """Set the active model in the statestore.
 
         :param model_id: The model id to set.
         :type model_id: str
         :return: A json response with success or failure message.
@@ -743,15 +707,14 @@
                 jsonify({"success": False, "message": "No models found."}),
                 404,
             )
 
         include_active: bool = include_active == "true"
 
         if include_active:
-
             latest_model = self.statestore.get_latest_model()
 
             arr = [
                 {
                     "committed_at": element["committed_at"],
                     "model": element["model"],
                     "session_id": element["session_id"],
@@ -799,38 +762,33 @@
         :return: The model trail for the given session as a json response.
         :rtype: :class:`flask.Response`
         """
         model_info = self.statestore.get_model_trail()
         if model_info:
             return jsonify(model_info)
         else:
-            return jsonify(
-                {"success": False, "message": "No model trail available."}
-            )
+            return jsonify({"success": False, "message": "No model trail available."})
 
     def get_model_ancestors(self, model_id: str, limit: str = None):
         """Get the model ancestors for a given model.
 
         :param model_id: The model id to get the model ancestors for.
         :type model_id: str
         :param limit: The number of ancestors to return.
         :type limit: str
         :return: The model ancestors for the given model as a json response.
         :rtype: :class:`flask.Response`
         """
         if model_id is None:
-            return jsonify(
-                {"success": False, "message": "No model id provided."}
-            )
+            return jsonify({"success": False, "message": "No model id provided."})
 
         limit: int = int(limit) if limit is not None else 10  # if limit is None, default to 10
 
         response = self.statestore.get_model_ancestors(model_id, limit)
         if response:
-
             arr: list = []
 
             for element in response:
                 obj = {
                     "model": element["model"],
                     "committed_at": element["committed_at"],
                     "session_id": element["session_id"],
@@ -838,40 +796,34 @@
                 }
                 arr.append(obj)
 
             result = {"result": arr}
 
             return jsonify(result)
         else:
-            return jsonify(
-                {"success": False, "message": "No model ancestors available."}
-            )
+            return jsonify({"success": False, "message": "No model ancestors available."})
 
     def get_model_descendants(self, model_id: str, limit: str = None):
         """Get the model descendants for a given model.
 
         :param model_id: The model id to get the model descendants for.
         :type model_id: str
         :param limit: The number of descendants to return.
         :type limit: str
         :return: The model descendants for the given model as a json response.
         :rtype: :class:`flask.Response`
         """
-
         if model_id is None:
-            return jsonify(
-                {"success": False, "message": "No model id provided."}
-            )
+            return jsonify({"success": False, "message": "No model id provided."})
 
         limit: int = int(limit) if limit is not None else 10
 
         response: list = self.statestore.get_model_descendants(model_id, limit)
 
         if response:
-
             arr: list = []
 
             for element in response:
                 obj = {
                     "model": element["model"],
                     "committed_at": element["committed_at"],
                     "session_id": element["session_id"],
@@ -879,17 +831,15 @@
                 }
                 arr.append(obj)
 
             result = {"result": arr}
 
             return jsonify(result)
         else:
-            return jsonify(
-                {"success": False, "message": "No model descendants available."}
-            )
+            return jsonify({"success": False, "message": "No model descendants available."})
 
     def get_all_rounds(self):
         """Get all rounds.
 
         :return: The rounds as json response.
         :rtype: :class:`flask.Response`
         """
@@ -909,31 +859,30 @@
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
         :rtype: :class:`flask.Response`
         """
         round_object = self.statestore.get_round(round_id)
         if round_object is None:
             return jsonify({"success": False, "message": "Round not found."})
         payload = {
-            'round_id': round_object['round_id'],
-            'combiners': round_object['combiners'],
+            "round_id": round_object["round_id"],
+            "combiners": round_object["combiners"],
         }
         return jsonify(payload)
 
     def get_client_config(self, checksum=True):
         """Get the client config.
 
         :return: The client config as json response.
@@ -956,15 +905,14 @@
 
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
@@ -983,37 +931,36 @@
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
-
             obj = {
                 "combiner": element["_id"],
                 "count": element["count"],
             }
 
             arr.append(obj)
 
         result = {"result": arr}
 
         return jsonify(result)
 
     def start_session(
         self,
         session_id,
-        aggregator='fedavg',
+        aggregator="fedavg",
+        aggregator_kwargs=None,
         model_id=None,
         rounds=5,
         round_timeout=180,
         round_buffer_size=-1,
         delete_models=True,
         validate=True,
         helper="numpyhelper",
@@ -1044,23 +991,19 @@
         :type requested_clients: int
         :return: A json response with success or failure message and session config.
         :rtype: :class:`flask.Response`
         """
         # Check if session already exists
         session = self.statestore.get_session(session_id)
         if session:
-            return jsonify(
-                {"success": False, "message": "Session already exists."}
-            )
+            return jsonify({"success": False, "message": "Session already exists."})
 
         # Check if session is running
         if self.control.state() == ReducerState.monitoring:
-            return jsonify(
-                {"success": False, "message": "A session is already running."}
-            )
+            return jsonify({"success": False, "message": "A session is already running."})
 
         # Check if compute package is set
         if not self.statestore.get_compute_package():
             return jsonify(
                 {
                     "success": False,
                     "message": "No compute package set. Set compute package before starting session.",
@@ -1106,30 +1049,29 @@
         if not model_id:
             model_id = self.statestore.get_latest_model()
 
         # Setup session config
         session_config = {
             "session_id": session_id if session_id else str(uuid.uuid4()),
             "aggregator": aggregator,
+            "aggregator_kwargs": aggregator_kwargs,
             "round_timeout": round_timeout,
             "buffer_size": round_buffer_size,
             "model_id": model_id,
             "rounds": rounds,
             "delete_models_storage": delete_models,
             "clients_required": min_clients,
             "clients_requested": requested_clients,
             "task": (""),
             "validate": validate,
             "helper_type": helper,
         }
 
         # Start session
-        threading.Thread(
-            target=self.control.session, args=(session_config,)
-        ).start()
+        threading.Thread(target=self.control.session, args=(session_config,)).start()
 
         # Return success response
         return jsonify(
             {
                 "success": True,
                 "message": "Session started successfully.",
                 "config": session_config,
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/network.py` & `fedn-0.9.5/fedn/network/api/network.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 import base64
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.combiner.interfaces import CombinerInterface
 from fedn.network.loadbalancer.leastpacked import LeastPacked
 
-__all__ = 'Network',
+__all__ = ("Network",)
 
 
-@trace_all_methods
 class Network:
-    """ FEDn network interface. This class is used to interact with the network.
-        Note: This class contain redundant code, which is not used in the current version of FEDn.
-        Some methods has been moved to :class:`fedn.network.api.interface.API`.
-         """
+    """FEDn network interface. This class is used to interact with the network.
+    Note: This class contain redundant code, which is not used in the current version of FEDn.
+    Some methods has been moved to :class:`fedn.network.api.interface.API`.
+    """
 
     def __init__(self, control, statestore, load_balancer=None):
         """ """
         self.statestore = statestore
         self.control = control
         self.id = statestore.network_id
 
         if not load_balancer:
             self.load_balancer = LeastPacked(self)
         else:
             self.load_balancer = load_balancer
 
     def get_combiner(self, name):
-        """ Get combiner by name.
+        """Get combiner by name.
 
         :param name: name of combiner
         :type name: str
         :return: The combiner instance object
         :rtype: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         """
         combiners = self.get_combiners()
         for combiner in combiners:
             if name == combiner.name:
                 return combiner
         return None
 
     def get_combiners(self):
-        """ Get all combiners in the network.
+        """Get all combiners in the network.
 
         :return: list of combiners objects
         :rtype: list(:class:`fedn.network.combiner.interfaces.CombinerInterface`)
         """
         data = self.statestore.get_combiners()
         combiners = []
         for c in data["result"]:
-            if c['certificate']:
-                cert = base64.b64decode(c['certificate'])
-                key = base64.b64decode(c['key'])
+            if c["certificate"]:
+                cert = base64.b64decode(c["certificate"])
+                key = base64.b64decode(c["key"])
             else:
                 cert = None
                 key = None
 
-            combiners.append(
-                CombinerInterface(c['parent'], c['name'], c['address'], c['fqdn'], c['port'],
-                                  certificate=cert, key=key, ip=c['ip']))
+            combiners.append(CombinerInterface(c["parent"], c["name"], c["address"], c["fqdn"], c["port"], certificate=cert, key=key, ip=c["ip"]))
 
         return combiners
 
     def add_combiner(self, combiner):
-        """ Add a new combiner to the network.
+        """Add a new combiner to the network.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         if not self.control.idle():
             logger.warning("Reducer is not idle, cannot add additional combiner.")
@@ -76,83 +72,81 @@
         if self.get_combiner(combiner.name):
             return
 
         logger.info("adding combiner {}".format(combiner.name))
         self.statestore.set_combiner(combiner.to_dict())
 
     def remove_combiner(self, combiner):
-        """ Remove a combiner from the network.
+        """Remove a combiner from the network.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         if not self.control.idle():
             logger.warning("Reducer is not idle, cannot remove combiner.")
             return
         self.statestore.delete_combiner(combiner.name)
 
     def find_available_combiner(self):
-        """ Find an available combiner in the network.
+        """Find an available combiner in the network.
 
         :return: The combiner instance object
         :rtype: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         """
         combiner = self.load_balancer.find_combiner()
         return combiner
 
     def handle_unavailable_combiner(self, combiner):
-        """ This callback is triggered if a combiner is found to be unresponsive.
+        """This callback is triggered if a combiner is found to be unresponsive.
 
         :param combiner: The combiner instance object
         :type combiner: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         :return: None
         """
         # TODO: Implement strategy to handle an unavailable combiner.
-        logger.warning("REDUCER CONTROL: Combiner {} unavailable.".format(
-            combiner.name))
+        logger.warning("REDUCER CONTROL: Combiner {} unavailable.".format(combiner.name))
 
     def add_client(self, client):
-        """ Add a new client to the network.
+        """Add a new client to the network.
 
         :param client: The client instance object
         :type client: dict
         :return: None
         """
-
-        if self.get_client(client['name']):
+        if self.get_client(client["name"]):
             return
 
-        logger.info("adding client {}".format(client['name']))
+        logger.info("adding client {}".format(client["name"]))
         self.statestore.set_client(client)
 
     def get_client(self, name):
-        """ Get client by name.
+        """Get client by name.
 
         :param name: name of client
         :type name: str
         :return: The client instance object
         :rtype: ObjectId
         """
         ret = self.statestore.get_client(name)
         return ret
 
     def update_client_data(self, client_data, status, role):
-        """ Update client status in statestore.
+        """Update client status in statestore.
 
         :param client_data: The client instance object
         :type client_data: dict
         :param status: The client status
         :type status: str
         :param role: The client role
         :type role: str
         :return: None
         """
         self.statestore.update_client_status(client_data, status, role)
 
     def get_client_info(self):
-        """ list available client in statestore.
+        """List available client in statestore.
 
         :return: list of client objects
         :rtype: list(ObjectId)
         """
         return self.statestore.list_clients()
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/server.py` & `fedn-0.9.5/fedn/network/api/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,30 @@
 import os
 
 from flask import Flask, jsonify, request
 
-from fedn.common.config import (get_controller_config, get_modelstorage_config,
-                                get_network_config, get_statestore_config)
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
-        app.register_blueprint(bp,
-                               name=f"{bp.name}_custom",
-                               url_prefix=f"{custom_url_prefix}{bp.url_prefix}")
+        app.register_blueprint(bp, name=f"{bp.name}_custom", url_prefix=f"{custom_url_prefix}{bp.url_prefix}")
 
 
-@app.route('/health', methods=["GET"])
+@app.route("/health", methods=["GET"])
 def health_check():
-    return 'OK', 200
+    return "OK", 200
 
 
 if custom_url_prefix:
     app.add_url_rule(f"{custom_url_prefix}/health", view_func=health_check, methods=["GET"])
 
 
 @app.route("/get_model_trail", methods=["GET"])
@@ -104,15 +94,14 @@
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
 
@@ -160,15 +149,14 @@
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
 
 
@@ -201,15 +189,14 @@
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
@@ -360,17 +347,15 @@
             jsonify({"success": False, "message": "Missing helper type."}),
             400,
         )
     try:
         file = request.files["file"]
     except KeyError:
         return jsonify({"success": False, "message": "Missing file."}), 400
-    return api.set_compute_package(
-        file=file, helper_type=helper_type, name=name, description=description
-    )
+    return api.set_compute_package(file=file, helper_type=helper_type, name=name, description=description)
 
 
 if custom_url_prefix:
     app.add_url_rule(f"{custom_url_prefix}/set_package", view_func=set_package, methods=["POST"])
 
 
 @app.route("/get_package", methods=["GET"])
@@ -390,22 +375,19 @@
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
 
-    return api.list_compute_packages(
-        limit=limit, skip=skip, include_active=include_active
-    )
+    return api.list_compute_packages(limit=limit, skip=skip, include_active=include_active)
 
 
 if custom_url_prefix:
     app.add_url_rule(f"{custom_url_prefix}/list_compute_packages", view_func=list_compute_packages, methods=["GET"])
 
 
 @app.route("/download_package", methods=["GET"])
@@ -599,15 +581,14 @@
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
@@ -620,15 +601,14 @@
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
@@ -643,15 +623,14 @@
 
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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/tests.py` & `fedn-0.9.5/fedn/network/api/tests.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/__init__.py` & `fedn-0.9.5/fedn/network/api/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/client_routes.py` & `fedn-0.9.5/fedn/network/api/v1/client_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, mdb
 from fedn.network.storage.statestore.stores.client_store import ClientStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("client", __name__, url_prefix=f"/api/{api_version}/clients")
 
 client_store = ClientStore(mdb, "network.clients")
 
@@ -111,17 +110,15 @@
                 message:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        clients = client_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        clients = client_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = clients["result"]
 
         response = {"count": clients["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -198,17 +195,15 @@
             properties:
                 message:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
-        clients = client_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        clients = client_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = clients["result"]
 
         response = {"count": clients["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/combiner_routes.py` & `fedn-0.9.5/fedn/network/api/v1/combiner_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, mdb
 from fedn.network.storage.statestore.stores.combiner_store import CombinerStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("combiner", __name__, url_prefix=f"/api/{api_version}/combiners")
 
 combiner_store = CombinerStore(mdb, "network.combiners")
 
@@ -103,17 +102,15 @@
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
 
         kwargs = request.args.to_dict()
 
-        combiners = combiner_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        combiners = combiner_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = combiners["result"]
 
         response = {"count": combiners["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -188,17 +185,15 @@
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
 
         kwargs = get_post_data_to_kwargs(request)
 
-        combiners = combiner_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        combiners = combiner_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = combiners["result"]
 
         response = {"count": combiners["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/model_routes.py` & `fedn-0.9.5/fedn/network/api/v1/model_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import io
 
 import numpy as np
 from flask import Blueprint, jsonify, request, send_file
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_limit,
-                                        get_post_data_to_kwargs, get_reverse,
-                                        get_typed_list_headers, mdb,
-                                        modelstorage_config)
+from fedn.network.api.v1.shared import api_version, get_limit, get_post_data_to_kwargs, get_reverse, get_typed_list_headers, mdb
+from fedn.network.api.shared import modelstorage_config
 from fedn.network.storage.s3.base import RepositoryBase
 from fedn.network.storage.s3.miniorepository import MINIORepository
 from fedn.network.storage.statestore.stores.model_store import ModelStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("model", __name__, url_prefix=f"/api/{api_version}/models")
 
@@ -108,17 +106,15 @@
                 error:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        models = model_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        models = model_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = models["result"]
 
         response = {"count": models["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -195,17 +191,15 @@
                 error:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
 
-        models = model_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        models = model_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = models["result"]
 
         response = {"count": models["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -462,15 +456,15 @@
                 properties:
                     message:
                         type: string
     """
     try:
         limit = get_limit(request.headers)
         reverse = get_reverse(request.headers)
-        include_self_param: str = request.args.get('include_self')
+        include_self_param: str = request.args.get("include_self")
 
         include_self: bool = include_self_param and include_self_param.lower() == "true"
 
         ancestors = model_store.list_ancestors(id, limit or 10, include_self=include_self, reverse=reverse, use_typing=False)
 
         response = ancestors
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/package_routes.py` & `fedn-0.9.5/fedn/network/api/v1/package_routes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, get_use_typing,
-                                        mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, get_use_typing, mdb
 from fedn.network.storage.statestore.stores.package_store import PackageStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("package", __name__, url_prefix=f"/api/{api_version}/packages")
 
 package_store = PackageStore(mdb, "control.package")
 
@@ -116,17 +114,15 @@
                     type: string
 
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        packages = package_store.list(
-            limit, skip, sort_key, sort_order, use_typing=True, **kwargs
-        )
+        packages = package_store.list(limit, skip, sort_key, sort_order, use_typing=True, **kwargs)
 
         result = [package.__dict__ for package in packages["result"]]
 
         response = {"count": packages["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -206,17 +202,15 @@
                 error:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
 
-        packages = package_store.list(
-            limit, skip, sort_key, sort_order, use_typing=True, **kwargs
-        )
+        packages = package_store.list(limit, skip, sort_key, sort_order, use_typing=True, **kwargs)
 
         result = [package.__dict__ for package in packages["result"]]
 
         response = {"count": packages["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/round_routes.py` & `fedn-0.9.5/fedn/network/api/v1/round_routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, mdb
 from fedn.network.storage.statestore.stores.round_store import RoundStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 
 bp = Blueprint("round", __name__, url_prefix=f"/api/{api_version}/rounds")
 
 round_store = RoundStore(mdb, "control.rounds")
 
@@ -91,17 +90,15 @@
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
 
         kwargs = request.args.to_dict()
 
-        rounds = round_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        rounds = round_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = rounds["result"]
 
         response = {"count": rounds["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -172,17 +169,15 @@
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
 
         kwargs = get_post_data_to_kwargs(request)
 
-        rounds = round_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        rounds = round_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = rounds["result"]
 
         response = {"count": rounds["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/session_routes.py` & `fedn-0.9.5/fedn/network/api/v1/session_routes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
+import threading
+
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, mdb
 from fedn.network.storage.statestore.stores.session_store import SessionStore
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
+from .model_routes import model_store
+from fedn.network.api.shared import control
 
 bp = Blueprint("session", __name__, url_prefix=f"/api/{api_version}/sessions")
 
 session_store = SessionStore(mdb, "control.sessions")
 
 
 @bp.route("/", methods=["GET"])
@@ -83,17 +86,15 @@
                 message:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        sessions = session_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        sessions = session_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = sessions["result"]
 
         response = {"count": sessions["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -163,17 +164,15 @@
                 message:
                     type: string
     """
     try:
         limit, skip, sort_key, sort_order, _ = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
 
-        sessions = session_store.list(
-            limit, skip, sort_key, sort_order, use_typing=False, **kwargs
-        )
+        sessions = session_store.list(limit, skip, sort_key, sort_order, use_typing=False, **kwargs)
 
         result = sessions["result"]
 
         response = {"count": sessions["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
@@ -305,7 +304,87 @@
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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/shared.py` & `fedn-0.9.5/fedn/network/api/v1/shared.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,16 @@
 from typing import Tuple
 
 import pymongo
 from pymongo.database import Database
 
-from fedn.common.config import (get_modelstorage_config, get_network_config,
-                                get_statestore_config)
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
@@ -54,17 +49,15 @@
     sort_order: str = headers.get("X-Sort-Order")
 
     limit: int = get_limit(headers)
     skip: int = get_skip(headers)
     use_typing: bool = get_use_typing(headers)
 
     if sort_order is not None:
-        sort_order = (
-            pymongo.ASCENDING if sort_order.lower() == "asc" else pymongo.DESCENDING
-        )
+        sort_order = pymongo.ASCENDING if sort_order.lower() == "asc" else pymongo.DESCENDING
     else:
         sort_order = pymongo.DESCENDING
 
     return limit, skip, sort_key, sort_order, use_typing
 
 
 def get_post_data_to_kwargs(request: object) -> dict:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/status_routes.py` & `fedn-0.9.5/fedn/network/api/v1/status_routes.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, get_use_typing,
-                                        mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, get_use_typing, mdb
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
 from fedn.network.storage.statestore.stores.status_store import StatusStore
 
 bp = Blueprint("status", __name__, url_prefix=f"/api/{api_version}/statuses")
 
 status_store = StatusStore(mdb, "control.status")
 
@@ -119,28 +117,20 @@
         schema:
             type: object
             properties:
                 message:
                     type: string
     """
     try:
-        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(
-            request.headers
-        )
+        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        statuses = status_store.list(
-            limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs
-        )
-
-        result = (
-            [status.__dict__ for status in statuses["result"]]
-            if use_typing
-            else statuses["result"]
-        )
+        statuses = status_store.list(limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs)
+
+        result = [status.__dict__ for status in statuses["result"]] if use_typing else statuses["result"]
 
         response = {"count": statuses["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
         return jsonify({"message": str(e)}), 500
 
@@ -222,28 +212,20 @@
         schema:
             type: object
             properties:
                 message:
                     type: string
     """
     try:
-        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(
-            request.headers
-        )
+        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
 
-        statuses = status_store.list(
-            limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs
-        )
-
-        result = (
-            [status.__dict__ for status in statuses["result"]]
-            if use_typing
-            else statuses["result"]
-        )
+        statuses = status_store.list(limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs)
+
+        result = [status.__dict__ for status in statuses["result"]] if use_typing else statuses["result"]
 
         response = {"count": statuses["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
         return jsonify({"message": str(e)}), 500
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/api/v1/validation_routes.py` & `fedn-0.9.5/fedn/network/api/v1/validation_routes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from flask import Blueprint, jsonify, request
 
 from fedn.network.api.auth import jwt_auth_required
-from fedn.network.api.v1.shared import (api_version, get_post_data_to_kwargs,
-                                        get_typed_list_headers, get_use_typing,
-                                        mdb)
+from fedn.network.api.v1.shared import api_version, get_post_data_to_kwargs, get_typed_list_headers, get_use_typing, mdb
 from fedn.network.storage.statestore.stores.shared import EntityNotFound
-from fedn.network.storage.statestore.stores.validation_store import \
-    ValidationStore
+from fedn.network.storage.statestore.stores.validation_store import ValidationStore
 
 bp = Blueprint("validation", __name__, url_prefix=f"/api/{api_version}/validations")
 
 validation_store = ValidationStore(mdb, "control.validations")
 
 
 @bp.route("/", methods=["GET"])
@@ -127,28 +124,20 @@
         schema:
             type: object
             properties:
                 message:
                     type: string
     """
     try:
-        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(
-            request.headers
-        )
+        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(request.headers)
         kwargs = request.args.to_dict()
 
-        validations = validation_store.list(
-            limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs
-        )
-
-        result = (
-            [validation.__dict__ for validation in validations["result"]]
-            if use_typing
-            else validations["result"]
-        )
+        validations = validation_store.list(limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs)
+
+        result = [validation.__dict__ for validation in validations["result"]] if use_typing else validations["result"]
 
         response = {"count": validations["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
         return jsonify({"message": str(e)}), 500
 
@@ -233,28 +222,20 @@
         schema:
             type: object
             properties:
                 message:
                     type: string
     """
     try:
-        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(
-            request.headers
-        )
+        limit, skip, sort_key, sort_order, use_typing = get_typed_list_headers(request.headers)
         kwargs = get_post_data_to_kwargs(request)
 
-        validations = validation_store.list(
-            limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs
-        )
-
-        result = (
-            [validation.__dict__ for validation in validations["result"]]
-            if use_typing
-            else validations["result"]
-        )
+        validations = validation_store.list(limit, skip, sort_key, sort_order, use_typing=use_typing, **kwargs)
+
+        result = [validation.__dict__ for validation in validations["result"]] if use_typing else validations["result"]
 
         response = {"count": validations["count"], "result": result}
 
         return jsonify(response), 200
     except Exception as e:
         return jsonify({"message": str(e)}), 500
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/clients/client.py` & `fedn-0.9.5/fedn/network/clients/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -18,79 +18,77 @@
 from google.protobuf.json_format import MessageToJson
 from OpenSSL import SSL
 from tenacity import retry, stop_after_attempt
 
 import fedn.network.grpc.fedn_pb2 as fedn
 import fedn.network.grpc.fedn_pb2_grpc as rpc
 from fedn.common.config import FEDN_AUTH_SCHEME, FEDN_PACKAGE_EXTRACT_DIR
-from fedn.common.log_config import (logger, set_log_level_from_string,
-                                    set_log_stream)
-from fedn.common.telemetry import trace_all_methods, tracer
+from fedn.common.log_config import logger, set_log_level_from_string, set_log_stream
 from fedn.network.clients.connect import ConnectorClient, Status
 from fedn.network.clients.package import PackageRuntime
 from fedn.network.clients.state import ClientState, ClientStateToString
-from fedn.network.combiner.modelservice import (get_tmp_path,
-                                                upload_request_generator)
+from fedn.network.combiner.modelservice import get_tmp_path, upload_request_generator
 from fedn.utils.dispatcher import Dispatcher
 from fedn.utils.helpers.helpers import get_helper
 
 CHUNK_SIZE = 1024 * 1024
-VALID_NAME_REGEX = '^[a-zA-Z0-9_-]*$'
+VALID_NAME_REGEX = "^[a-zA-Z0-9_-]*$"
 
 
-@trace_all_methods
 class GrpcAuth(grpc.AuthMetadataPlugin):
     def __init__(self, key):
         self._key = key
 
     def __call__(self, context, callback):
-        callback((('authorization', f'{FEDN_AUTH_SCHEME} {self._key}'),), None)
+        callback((("authorization", f"{FEDN_AUTH_SCHEME} {self._key}"),), None)
 
 
-@trace_all_methods
 class Client:
     """FEDn Client. Service running on client/datanodes in a federation,
     recieving and handling model update and model validation requests.
 
     :param config: A configuration dictionary containing connection information for the discovery service (controller)
         and settings governing e.g. client-combiner assignment behavior.
     :type config: dict
     """
+
     def __init__(self, config):
         """Initialize the client."""
         self.state = None
         self.error_state = False
         self._connected = False
         self._missed_heartbeat = 0
         self.config = config
         self.trace_attribs = False
-        set_log_level_from_string(config.get('verbosity', "INFO"))
-        set_log_stream(config.get('logfile', None))
+        set_log_level_from_string(config.get("verbosity", "INFO"))
+        set_log_stream(config.get("logfile", None))
 
-        self.connector = ConnectorClient(host=config['discover_host'],
-                                         port=config['discover_port'],
-                                         token=config['token'],
-                                         name=config['name'],
-                                         remote_package=config['remote_compute_context'],
-                                         force_ssl=config['force_ssl'],
-                                         verify=config['verify'],
-                                         combiner=config['preferred_combiner'],
-                                         id=config['client_id'])
+        self.connector = ConnectorClient(
+            host=config["discover_host"],
+            port=config["discover_port"],
+            token=config["token"],
+            name=config["name"],
+            remote_package=config["remote_compute_context"],
+            force_ssl=config["force_ssl"],
+            verify=config["verify"],
+            combiner=config["preferred_combiner"],
+            id=config["client_id"],
+        )
 
         # Validate client name
-        match = re.search(VALID_NAME_REGEX, config['name'])
+        match = re.search(VALID_NAME_REGEX, config["name"])
         if not match:
-            raise ValueError('Unallowed character in client name. Allowed characters: a-z, A-Z, 0-9, _, -.')
+            raise ValueError("Unallowed character in client name. Allowed characters: a-z, A-Z, 0-9, _, -.")
 
         # Folder where the client will store downloaded compute package and logs
-        self.name = config['name']
+        self.name = config["name"]
         if FEDN_PACKAGE_EXTRACT_DIR:
             self.run_path = os.path.join(os.getcwd(), FEDN_PACKAGE_EXTRACT_DIR)
         else:
-            dirname = self.name+"-"+time.strftime("%Y%m%d-%H%M%S")
+            dirname = self.name + "-" + time.strftime("%Y%m%d-%H%M%S")
             self.run_path = os.path.join(os.getcwd(), dirname)
         if not os.path.exists(self.run_path):
             os.mkdir(self.run_path)
 
         self.started_at = datetime.now()
         self.logs = []
 
@@ -100,28 +98,26 @@
         combiner_config = self.assign()
         self.connect(combiner_config)
 
         self._initialize_dispatcher(self.config)
 
         self._initialize_helper(combiner_config)
         if not self.helper:
-            logger.warning("Failed to retrieve helper class settings: {}".format(
-                combiner_config))
+            logger.warning("Failed to retrieve helper class settings: {}".format(combiner_config))
 
         self._subscribe_to_combiner(self.config)
 
         self.state = ClientState.idle
 
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
@@ -145,22 +141,22 @@
 
         :param key: The key of the metadata.
         :type key: str
         :param value: The value of the metadata.
         :type value: str
         """
         # Check if metadata exists and add if not
-        if not hasattr(self, 'metadata'):
+        if not hasattr(self, "metadata"):
             self.metadata = ()
 
         # Check if metadata key already exists and replace value if so
         for i, (k, v) in enumerate(self.metadata):
             if k == key:
                 # Replace value
-                self.metadata = self.metadata[:i] + ((key, value),) + self.metadata[i + 1:]
+                self.metadata = self.metadata[:i] + ((key, value),) + self.metadata[i + 1 :]
                 return
 
         # Set metadata using tuple concatenation
         self.metadata += ((key, value),)
 
     def _get_ssl_certificate(self, domain, port=443):
         context = SSL.Context(SSL.SSLv23_METHOD)
@@ -178,77 +174,70 @@
 
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
-        host = combiner_config['host']
+        host = combiner_config["host"]
         # Add host to gRPC metadata
-        self._add_grpc_metadata('grpc-server', host)
+        self._add_grpc_metadata("grpc-server", host)
         logger.debug("Client using metadata: {}.".format(self.metadata))
-        port = combiner_config['port']
+        port = combiner_config["port"]
         secure = False
-        if combiner_config['fqdn'] is not None:
-            host = combiner_config['fqdn']
+        if combiner_config["fqdn"] is not None:
+            host = combiner_config["fqdn"]
             # assuming https if fqdn is used
             port = 443
         logger.info(f"Initiating connection to combiner host at: {host}:{port}")
 
-        if combiner_config['certificate']:
+        if combiner_config["certificate"]:
             logger.info("Utilizing CA certificate for GRPC channel authentication.")
             secure = True
-            cert = base64.b64decode(
-                combiner_config['certificate'])  # .decode('utf-8')
+            cert = base64.b64decode(combiner_config["certificate"])  # .decode('utf-8')
             credentials = grpc.ssl_channel_credentials(root_certificates=cert)
             channel = grpc.secure_channel("{}:{}".format(host, str(port)), credentials)
         elif os.getenv("FEDN_GRPC_ROOT_CERT_PATH"):
             secure = True
             logger.info("Using root certificate from environment variable for GRPC channel.")
-            with open(os.environ["FEDN_GRPC_ROOT_CERT_PATH"], 'rb') as f:
+            with open(os.environ["FEDN_GRPC_ROOT_CERT_PATH"], "rb") as f:
                 credentials = grpc.ssl_channel_credentials(f.read())
             channel = grpc.secure_channel("{}:{}".format(host, str(port)), credentials)
-        elif self.config['secure']:
+        elif self.config["secure"]:
             secure = True
             logger.info("Using CA certificate for GRPC channel.")
             cert = self._get_ssl_certificate(host, port=port)
 
-            credentials = grpc.ssl_channel_credentials(cert.encode('utf-8'))
-            if self.config['token']:
-                token = self.config['token']
+            credentials = grpc.ssl_channel_credentials(cert.encode("utf-8"))
+            if self.config["token"]:
+                token = self.config["token"]
                 auth_creds = grpc.metadata_call_credentials(GrpcAuth(token))
                 channel = grpc.secure_channel("{}:{}".format(host, str(port)), grpc.composite_channel_credentials(credentials, auth_creds))
             else:
                 channel = grpc.secure_channel("{}:{}".format(host, str(port)), credentials)
         else:
             logger.info("Using insecure GRPC channel.")
             if port == 443:
                 port = 80
-            channel = grpc.insecure_channel("{}:{}".format(
-                host,
-                str(port)))
+            channel = grpc.insecure_channel("{}:{}".format(host, str(port)))
 
         self.channel = channel
 
         self.connectorStub = rpc.ConnectorStub(channel)
         self.combinerStub = rpc.CombinerStub(channel)
         self.modelStub = rpc.ModelServiceStub(channel)
 
-        logger.info("Successfully established {} connection to {}:{}".format("secure" if secure else "insecure",
-                                                                             host,
-                                                                             port))
+        logger.info("Successfully established {} connection to {}:{}".format("secure" if secure else "insecure", host, port))
 
-        logger.info("Using {} compute package.".format(
-            combiner_config["package"]))
+        logger.info("Using {} compute package.".format(combiner_config["package"]))
 
         self._connected = True
 
     def disconnect(self):
         """Disconnect from the combiner."""
         if not self._connected:
             logger.info("Client is not connected.")
@@ -262,102 +251,98 @@
 
         :param combiner_config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         :type combiner_config: dict
         :return:
         """
-
-        if 'helper_type' in combiner_config.keys():
-            self.helper = get_helper(combiner_config['helper_type'])
+        if "helper_type" in combiner_config.keys():
+            self.helper = get_helper(combiner_config["helper_type"])
 
     def _subscribe_to_combiner(self, config):
         """Listen to combiner message stream and start all processing threads.
 
         :param config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         """
-
         # Start sending heartbeats to the combiner.
-        threading.Thread(target=self._send_heartbeat, kwargs={
-            'update_frequency': config['heartbeat_interval']}, daemon=True).start()
+        threading.Thread(target=self._send_heartbeat, kwargs={"update_frequency": config["heartbeat_interval"]}, daemon=True).start()
 
         # Start listening for combiner training and validation messages
-        threading.Thread(
-            target=self._listen_to_task_stream, daemon=True).start()
+        threading.Thread(target=self._listen_to_task_stream, daemon=True).start()
         self._connected = True
 
         # Start processing the client message inbox
         threading.Thread(target=self.process_request, daemon=True).start()
 
     @retry(stop=stop_after_attempt(3))
     def untar_package(self, package_runtime):
-        package_runtime.unpack()
+        _, package_runpath = package_runtime.unpack()
+        return package_runpath
 
     def _initialize_dispatcher(self, config):
-        """ Initialize the dispatcher for the client.
+        """Initialize the dispatcher for the client.
 
         :param config: A configuration dictionary containing connection information for
         | the discovery service (controller) and settings governing e.g.
         | client-combiner assignment behavior.
         :type config: dict
         :return:
         """
-        if config['remote_compute_context']:
-            pr = PackageRuntime(os.getcwd(), os.getcwd())
+        if config["remote_compute_context"]:
+            pr = PackageRuntime(self.run_path)
 
             retval = None
             tries = 10
 
             while tries > 0:
                 retval = pr.download(
-                    host=config['discover_host'],
-                    port=config['discover_port'],
-                    token=config['token'],
-                    force_ssl=config['force_ssl'],
-                    secure=config['secure']
+                    host=config["discover_host"], port=config["discover_port"], token=config["token"], force_ssl=config["force_ssl"], secure=config["secure"]
                 )
                 if retval:
                     break
                 time.sleep(60)
                 logger.warning("Compute package not available. Retrying in 60 seconds. {} attempts remaining.".format(tries))
                 tries -= 1
 
             if retval:
-                if 'checksum' not in config:
+                if "checksum" not in config:
                     logger.warning("Bypassing validation of package checksum. Ensure the package source is trusted.")
                 else:
-                    checks_out = pr.validate(config['checksum'])
+                    checks_out = pr.validate(config["checksum"])
                     if not checks_out:
                         logger.critical("Validation of local package failed. Client terminating.")
                         self.error_state = True
                         return
-
+            package_runpath = ""
             if retval:
-                self.untar_package(pr)
+                package_runpath = self.untar_package(pr)
 
-            self.dispatcher = pr.dispatcher(self.run_path)
+            self.dispatcher = pr.dispatcher(package_runpath)
             try:
                 logger.info("Initiating Dispatcher with entrypoint set to: startup")
                 activate_cmd = self.dispatcher._get_or_create_python_env()
                 self.dispatcher.run_cmd("startup")
             except KeyError:
                 logger.info("No startup command found in package. Continuing.")
                 pass
             except Exception as e:
                 logger.error(f"Caught exception: {type(e).__name__}")
 
         else:
             # TODO: Deprecate
-            dispatch_config = {'entry_points':
-                               {'predict': {'command': 'python3 predict.py'},
-                                'train': {'command': 'python3 train.py'},
-                                'validate': {'command': 'python3 validate.py'}}}
-            from_path = os.path.join(os.getcwd(), 'client')
+            dispatch_config = {
+                "entry_points": {
+                    "predict": {"command": "python3 predict.py"},
+                    "train": {"command": "python3 train.py"},
+                    "validate": {"command": "python3 validate.py"},
+                }
+            }
+            from_path = os.path.join(os.getcwd(), "client")
 
             copy_tree(from_path, self.run_path)
             self.dispatcher = Dispatcher(dispatch_config, self.run_path)
         # Get or create python environment
         activate_cmd = self.dispatcher._get_or_create_python_env()
         if activate_cmd:
             logger.info("To activate the virtual environment, run: {}".format(activate_cmd))
@@ -375,15 +360,14 @@
         time_start = time.time()
         request = fedn.ModelRequest(id=id)
         request.sender.name = self.name
         request.sender.role = fedn.WORKER
 
         try:
             for part in self.modelStub.Download(request, metadata=self.metadata):
-
                 if part.status == fedn.ModelStatus.IN_PROGRESS:
                     data.write(part.data)
 
                 if part.status == fedn.ModelStatus.OK:
                     return data
 
                 if part.status == fedn.ModelStatus.FAILED:
@@ -428,55 +412,59 @@
 
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
-        self._add_grpc_metadata('client', self.name)
+        self._add_grpc_metadata("client", self.name)
 
         while self._connected:
             try:
                 for request in self.combinerStub.TaskStream(r, metadata=self.metadata):
                     if request:
                         logger.debug("Received model update request from combiner: {}.".format(request))
                     if request.sender.role == fedn.COMBINER:
                         # Process training request
-                        self.send_status("Received model update request.", log_level=fedn.Status.AUDIT,
-                                         type=fedn.StatusType.MODEL_UPDATE_REQUEST, request=request, sesssion_id=request.session_id)
+                        self.send_status(
+                            "Received model update request.",
+                            log_level=fedn.Status.AUDIT,
+                            type=fedn.StatusType.MODEL_UPDATE_REQUEST,
+                            request=request,
+                            sesssion_id=request.session_id,
+                        )
                         logger.info("Received model update request of type {} for model_id {}".format(request.type, request.model_id))
 
-                        if request.type == fedn.StatusType.MODEL_UPDATE and self.config['trainer']:
-                            self.inbox.put(('train', request))
-                        elif request.type == fedn.StatusType.MODEL_VALIDATION and self.config['validator']:
-                            self.inbox.put(('validate', request))
+                        if request.type == fedn.StatusType.MODEL_UPDATE and self.config["trainer"]:
+                            self.inbox.put(("train", request))
+                        elif request.type == fedn.StatusType.MODEL_VALIDATION and self.config["validator"]:
+                            self.inbox.put(("validate", request))
                         else:
                             logger.error("Unknown request type: {}".format(request.type))
 
             except grpc.RpcError as e:
                 # Handle gRPC errors
                 status_code = e.code()
                 if status_code == grpc.StatusCode.UNAVAILABLE:
                     logger.warning("GRPC TaskStream: server unavailable during model update request stream. Retrying.")
                     # Retry after a delay
                     time.sleep(5)
                 if status_code == grpc.StatusCode.UNAUTHENTICATED:
                     details = e.details()
-                    if details == 'Token expired':
+                    if details == "Token expired":
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
@@ -492,64 +480,62 @@
         :param model_id: The model id of the model to be updated.
         :type model_id: str
         :param session_id: The id of the current session
         :type session_id: str
         :return: The model id of the updated model, or None if the update failed. And a dict with metadata.
         :rtype: tuple
         """
-
-        self.send_status(
-            "\t Starting processing of training request for model_id {}".format(model_id), sesssion_id=session_id)
+        self.send_status("\t Starting processing of training request for model_id {}".format(model_id), sesssion_id=session_id)
         self.state = ClientState.training
 
         try:
             meta = {}
             tic = time.time()
             mdl = self.get_model_from_combiner(str(model_id))
             if mdl is None:
                 logger.error("Could not retrieve model from combiner. Aborting training request.")
                 return None, None
-            meta['fetch_model'] = time.time() - tic
+            meta["fetch_model"] = time.time() - tic
 
             inpath = self.helper.get_tmp_path()
-            with open(inpath, 'wb') as fh:
+            with open(inpath, "wb") as fh:
                 fh.write(mdl.getbuffer())
 
             outpath = self.helper.get_tmp_path()
             tic = time.time()
             # TODO: Check return status, fail gracefully
 
             self.dispatcher.run_cmd("train {} {}".format(inpath, outpath))
 
-            meta['exec_training'] = time.time() - tic
+            meta["exec_training"] = time.time() - tic
 
             tic = time.time()
             out_model = None
 
             with open(outpath, "rb") as fr:
                 out_model = io.BytesIO(fr.read())
 
             # Stream model update to combiner server
             updated_model_id = uuid.uuid4()
             self.send_model_to_combiner(out_model, str(updated_model_id))
-            meta['upload_model'] = time.time() - tic
+            meta["upload_model"] = time.time() - tic
 
             # Read the metadata file
-            with open(outpath+'-metadata', 'r') as fh:
+            with open(outpath + "-metadata", "r") as fh:
                 training_metadata = json.loads(fh.read())
-            meta['training_metadata'] = training_metadata
+            meta["training_metadata"] = training_metadata
 
             os.unlink(inpath)
             os.unlink(outpath)
-            os.unlink(outpath+'-metadata')
+            os.unlink(outpath + "-metadata")
 
         except Exception as e:
             logger.error("Could not process training request due to error: {}".format(e))
             updated_model_id = None
-            meta = {'status': 'failed', 'error': str(e)}
+            meta = {"status": "failed", "error": str(e)}
 
         self.state = ClientState.idle
 
         return updated_model_id, meta
 
     def _process_validation_request(self, model_id: str, is_inference: bool, session_id: str = None):
         """Process a validation request.
@@ -561,20 +547,19 @@
         :param session_id: The id of the current session.
         :type session_id: str
         :return: The validation metrics, or None if validation failed.
         :rtype: dict
         """
         # Figure out cmd
         if is_inference:
-            cmd = 'infer'
+            cmd = "infer"
         else:
-            cmd = 'validate'
+            cmd = "validate"
 
-        self.send_status(
-            f"Processing {cmd} request for model_id {model_id}", sesssion_id=session_id)
+        self.send_status(f"Processing {cmd} request for model_id {model_id}", sesssion_id=session_id)
         self.state = ClientState.validating
         try:
             model = self.get_model_from_combiner(str(model_id))
             if model is None:
                 logger.error("Could not retrieve model from combiner. Aborting validation request.")
                 return None
             inpath = self.helper.get_tmp_path()
@@ -596,33 +581,30 @@
             self.state = ClientState.idle
             return None
 
         self.state = ClientState.idle
         return validation
 
     def process_request(self):
-        """Process training and validation tasks. """
+        """Process training and validation tasks."""
         while True:
-
             if not self._connected:
                 return
 
             try:
                 (task_type, request) = self.inbox.get(timeout=1.0)
-                if task_type == 'train':
-
+                if task_type == "train":
                     tic = time.time()
                     self.state = ClientState.training
-                    model_id, meta = self._process_training_request(
-                        request.model_id, session_id=request.session_id)
+                    model_id, meta = self._process_training_request(request.model_id, session_id=request.session_id)
 
                     if meta is not None:
-                        processing_time = time.time()-tic
-                        meta['processing_time'] = processing_time
-                        meta['config'] = request.data
+                        processing_time = time.time() - tic
+                        meta["processing_time"] = processing_time
+                        meta["config"] = request.data
 
                     if model_id is not None:
                         # Send model update to combiner
                         update = fedn.ModelUpdate()
                         update.sender.name = self.name
                         update.sender.role = fedn.WORKER
                         update.receiver.name = request.sender.name
@@ -631,36 +613,39 @@
                         update.model_update_id = str(model_id)
                         update.timestamp = str(datetime.now())
                         update.correlation_id = request.correlation_id
                         update.meta = json.dumps(meta)
 
                         try:
                             _ = self.combinerStub.SendModelUpdate(update, metadata=self.metadata)
-                            self.send_status("Model update completed.", log_level=fedn.Status.AUDIT,
-                                             type=fedn.StatusType.MODEL_UPDATE, request=update, sesssion_id=request.session_id)
+                            self.send_status(
+                                "Model update completed.",
+                                log_level=fedn.Status.AUDIT,
+                                type=fedn.StatusType.MODEL_UPDATE,
+                                request=update,
+                                sesssion_id=request.session_id,
+                            )
                         except grpc.RpcError as e:
                             status_code = e.code()
-                            logger.error("GRPC error, {}.".format(
-                                status_code.name))
+                            logger.error("GRPC error, {}.".format(status_code.name))
                             logger.debug(e)
                         except ValueError as e:
                             logger.error("GRPC error, RPC channel closed. {}".format(e))
                             logger.debug(e)
                     else:
-                        self.send_status("Client {} failed to complete model update.",
-                                         log_level=fedn.Status.WARNING,
-                                         request=request, sesssion_id=request.session_id)
+                        self.send_status(
+                            "Client {} failed to complete model update.", log_level=fedn.Status.WARNING, request=request, sesssion_id=request.session_id
+                        )
 
                     self.state = ClientState.idle
                     self.inbox.task_done()
 
-                elif task_type == 'validate':
+                elif task_type == "validate":
                     self.state = ClientState.validating
-                    metrics = self._process_validation_request(
-                        request.model_id, False, request.session_id)
+                    metrics = self._process_validation_request(request.model_id, False, request.session_id)
 
                     if metrics is not None:
                         # Send validation
                         validation = fedn.ModelValidation()
                         validation.sender.name = self.name
                         validation.sender.role = fedn.WORKER
                         validation.receiver.name = request.sender.name
@@ -668,64 +653,69 @@
                         validation.model_id = str(request.model_id)
                         validation.data = json.dumps(metrics)
                         validation.timestamp.GetCurrentTime()
                         validation.correlation_id = request.correlation_id
                         validation.session_id = request.session_id
 
                         try:
-                            _ = self.combinerStub.SendModelValidation(
-                                validation, metadata=self.metadata)
+                            _ = self.combinerStub.SendModelValidation(validation, metadata=self.metadata)
 
                             status_type = fedn.StatusType.MODEL_VALIDATION
-                            self.send_status("Model validation completed.", log_level=fedn.Status.AUDIT,
-                                             type=status_type, request=validation, sesssion_id=request.session_id)
+                            self.send_status(
+                                "Model validation completed.", log_level=fedn.Status.AUDIT, type=status_type, request=validation, sesssion_id=request.session_id
+                            )
                         except grpc.RpcError as e:
                             status_code = e.code()
-                            logger.error("GRPC error, {}.".format(
-                                status_code.name))
+                            logger.error("GRPC error, {}.".format(status_code.name))
                             logger.debug(e)
                         except ValueError as e:
                             logger.error("GRPC error, RPC channel closed. {}".format(e))
                             logger.debug(e)
                     else:
-                        self.send_status("Client {} failed to complete model validation.".format(self.name),
-                                         log_level=fedn.Status.WARNING, request=request, sesssion_id=request.session_id)
+                        self.send_status(
+                            "Client {} failed to complete model validation.".format(self.name),
+                            log_level=fedn.Status.WARNING,
+                            request=request,
+                            sesssion_id=request.session_id,
+                        )
 
                     self.state = ClientState.idle
                     self.inbox.task_done()
             except queue.Empty:
                 pass
             except grpc.RpcError as e:
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
-            heartbeat = fedn.Heartbeat(sender=fedn.Client(
-                name=self.name, role=fedn.WORKER))
+            heartbeat = fedn.Heartbeat(sender=fedn.Client(name=self.name, role=fedn.WORKER))
             try:
                 self.connectorStub.SendHeartbeat(heartbeat, metadata=self.metadata)
                 self._missed_heartbeat = 0
             except grpc.RpcError as e:
                 status_code = e.code()
                 if status_code == grpc.StatusCode.UNAVAILABLE:
                     self._missed_heartbeat += 1
-                    logger.error("GRPC hearbeat: combiner unavailable, retrying (attempt {}/{}).".format(self._missed_heartbeat,
-                                                                                                         self.config['reconnect_after_missed_heartbeat']))
-                    if self._missed_heartbeat > self.config['reconnect_after_missed_heartbeat']:
+                    logger.error(
+                        "GRPC hearbeat: combiner unavailable, retrying (attempt {}/{}).".format(
+                            self._missed_heartbeat, self.config["reconnect_after_missed_heartbeat"]
+                        )
+                    )
+                    if self._missed_heartbeat > self.config["reconnect_after_missed_heartbeat"]:
                         self.disconnect()
                 if status_code == grpc.StatusCode.UNAUTHENTICATED:
                     details = e.details()
-                    if details == 'Token expired':
+                    if details == "Token expired":
                         logger.error("GRPC hearbeat: Token expired. Disconnecting.")
                         self.disconnect()
                         sys.exit("Unauthorized. Token expired. Please obtain a new token.")
                 logger.debug(e)
 
             time.sleep(update_frequency)
             if not self._connected:
@@ -740,15 +730,14 @@
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
@@ -758,30 +747,28 @@
         status.session_id = sesssion_id
         if type is not None:
             status.type = type
 
         if request is not None:
             status.data = MessageToJson(request)
 
-        self.logs.append(
-            "{} {} LOG LEVEL {} MESSAGE {}".format(str(datetime.now()), status.sender.name, status.log_level,
-                                                   status.status))
+        self.logs.append("{} {} LOG LEVEL {} MESSAGE {}".format(str(datetime.now()), status.sender.name, status.log_level, status.status))
         try:
             _ = self.connectorStub.SendStatus(status, metadata=self.metadata)
         except grpc.RpcError as e:
             status_code = e.code()
             if status_code == grpc.StatusCode.UNAVAILABLE:
                 logger.warning("GRPC SendStatus: server unavailable during send status.")
             if status_code == grpc.StatusCode.UNAUTHENTICATED:
                 details = e.details()
-                if details == 'Token expired':
+                if details == "Token expired":
                     logger.warning("GRPC SendStatus: Token expired.")
 
     def run(self):
-        """ Run the client. """
+        """Run the client."""
         try:
             cnt = 0
             old_state = self.state
             while True:
                 time.sleep(1)
                 if cnt == 0:
                     logger.info("Client is active, waiting for model update requests.")
@@ -791,14 +778,11 @@
                 if not self._connected:
                     logger.warning("Client lost connection to combiner. Attempting to reconnect to FEDn network.")
                     combiner_config = self.assign()
                     self.connect(combiner_config)
                     self._subscribe_to_combiner(self.config)
                     cnt = 0
                 if self.error_state:
-                    logger.error("Client in error state. Terminating.")
-                    sys.exit("Client in error state. Terminating.")
-
+                    logger.error("Client in error state. Terminiating.")
+                    sys.exit("Client in error state. Terminiating.")
         except KeyboardInterrupt:
-            with tracer.start_as_current_span("Shutting down."):
-                pass
             logger.info("Shutting down.")
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/clients/connect.py` & `fedn-0.9.5/fedn/network/clients/connect.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,33 @@
 # This file contains the Connector class for assigning client to the FEDn network via the discovery service (REST-API).
 # The Connector class is used by the Client class in fedn/network/clients/client.py.
 # Once assigned, the client will retrieve combiner assignment from the discovery service.
 # The discovery service will also add the client to the statestore.
 #
 #
 import enum
-import sys
 
 import requests
 
-from fedn.common.config import (FEDN_AUTH_REFRESH_TOKEN,
-                                FEDN_AUTH_REFRESH_TOKEN_URI, FEDN_AUTH_SCHEME,
-                                FEDN_CUSTOM_URL_PREFIX)
+from fedn.common.config import FEDN_AUTH_REFRESH_TOKEN, FEDN_AUTH_REFRESH_TOKEN_URI, FEDN_AUTH_SCHEME, FEDN_CUSTOM_URL_PREFIX
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 
 
 class Status(enum.Enum):
-    """ Enum for representing the status of a client assignment."""
+    """Enum for representing the status of a client assignment."""
+
     Unassigned = 0
     Assigned = 1
     TryAgain = 2
     UnAuthorized = 3
     UnMatchedConfig = 4
 
 
-@trace_all_methods
 class ConnectorClient:
-    """ Connector for assigning client to a combiner in the FEDn network.
+    """Connector for assigning client to a combiner in the FEDn network.
 
     :param host: host of discovery service
     :type host: str
     :param port: port of discovery service
     :type port: int
     :param token: token for authentication
     :type token: str
@@ -45,114 +41,100 @@
     :type verify: bool
     :param combiner: name of preferred combiner
     :type combiner: str
     :param id: id of client
     """
 
     def __init__(self, host, port, token, name, remote_package, force_ssl=False, verify=False, combiner=None, id=None):
-
         self.host = host
         self.port = port
         self.token = token
         self.name = name
         self.verify = verify
         self.preferred_combiner = combiner
         self.id = id
-        self.package = 'remote' if remote_package else 'local'
+        self.package = "remote" if remote_package else "local"
 
         # for https we assume a an ingress handles permanent redirect (308)
         if force_ssl:
             self.prefix = "https://"
         else:
             self.prefix = "http://"
         if self.port:
-            self.connect_string = "{}{}:{}".format(
-                self.prefix, self.host, self.port)
+            self.connect_string = "{}{}:{}".format(self.prefix, self.host, self.port)
         else:
-            self.connect_string = "{}{}".format(
-                self.prefix, self.host)
+            self.connect_string = "{}{}".format(self.prefix, self.host)
 
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
-            payload = {'client_id': self.name, 'preferred_combiner': self.preferred_combiner}
-            retval = requests.post(self.connect_string + FEDN_CUSTOM_URL_PREFIX + '/add_client',
-                                   json=payload,
-                                   verify=self.verify,
-                                   allow_redirects=True,
-                                   headers={'Authorization': f"{FEDN_AUTH_SCHEME} {self.token}"})
+            payload = {"client_id": self.name, "preferred_combiner": self.preferred_combiner}
+            retval = requests.post(
+                self.connect_string + FEDN_CUSTOM_URL_PREFIX + "/add_client",
+                json=payload,
+                verify=self.verify,
+                allow_redirects=True,
+                headers={"Authorization": f"{FEDN_AUTH_SCHEME} {self.token}"},
+            )
         except Exception as e:
-            logger.debug('***** {}'.format(e))
+            logger.debug("***** {}".format(e))
             return Status.Unassigned, {}
 
         if retval.status_code == 400:
             # Get error messange from response
-            reason = retval.json()['message']
+            reason = retval.json()["message"]
             return Status.UnMatchedConfig, reason
 
         if retval.status_code == 401:
-            if 'message' in retval.json():
-                reason = retval.json()['message']
+            if "message" in retval.json():
+                reason = retval.json()["message"]
                 logger.warning(reason)
-                if reason == 'Token expired':
+                if reason == "Token expired":
                     status_code = self.refresh_token()
                     if status_code >= 200 and status_code < 204:
                         logger.info("Token refreshed.")
                         return Status.TryAgain, reason
                     else:
                         return Status.UnAuthorized, "Could not refresh token"
             reason = "Unauthorized connection to reducer, make sure the correct token is set"
             return Status.UnAuthorized, reason
 
         if retval.status_code >= 200 and retval.status_code < 204:
-            try:
-                if retval.json()['status'] == 'retry':
-                    if 'message' in retval.json():
-                        reason = retval.json()['message']
-                    else:
-                        reason = "Reducer was not ready. Try again later."
+            if retval.json()["status"] == "retry":
+                if "message" in retval.json():
+                    reason = retval.json()["message"]
+                else:
+                    reason = "Reducer was not ready. Try again later."
 
-                    return Status.TryAgain, reason
-            except requests.exceptions.JSONDecodeError as err:
-                logger.error("Response from controller was not JSON: {}".format(err))
-                logger.error("Response was: {}".format(retval.text))
-                sys.exit(1)
-            except Exception as e:
-                logger.error("Error: {}".format(e))
-                sys.exit(1)
+                return Status.TryAgain, reason
 
-            reducer_package = retval.json()['package']
+            reducer_package = retval.json()["package"]
             if reducer_package != self.package:
-                reason = "Unmatched config of compute package between client and reducer.\n" +\
-                    "Reducer uses {} package and client uses {}.".format(
-                        reducer_package, self.package)
+                reason = "Unmatched config of compute package between client and reducer.\n" + "Reducer uses {} package and client uses {}.".format(
+                    reducer_package, self.package
+                )
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
 
-        payload = requests.post(FEDN_AUTH_REFRESH_TOKEN_URI,
-                                verify=self.verify,
-                                allow_redirects=True,
-                                json={'refresh': FEDN_AUTH_REFRESH_TOKEN})
-        self.token = payload.json()['access']
+        payload = requests.post(FEDN_AUTH_REFRESH_TOKEN_URI, verify=self.verify, allow_redirects=True, json={"refresh": FEDN_AUTH_REFRESH_TOKEN})
+        self.token = payload.json()["access"]
         return payload.status_code
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/clients/package.py` & `fedn-0.9.5/fedn/network/clients/package.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,49 +1,47 @@
 # This file contains the PackageRuntime class, which is used to download, validate and unpack compute packages.
 #
 #
 import cgi
 import os
 import tarfile
-from distutils.dir_util import copy_tree
 
 import requests
 
 from fedn.common.config import FEDN_AUTH_SCHEME, FEDN_CUSTOM_URL_PREFIX
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.utils.checksum import sha
 from fedn.utils.dispatcher import Dispatcher, _read_yaml_file
 
 
-@trace_all_methods
 class PackageRuntime:
-    """ PackageRuntime is used to download, validate and unpack compute packages.
+    """PackageRuntime is used to download, validate and unpack compute packages.
 
     :param package_path: path to compute package
     :type package_path: str
     :param package_dir: directory to unpack compute package
     :type package_dir: str
     """
 
-    def __init__(self, package_path, package_dir):
-
-        self.dispatch_config = {'entry_points':
-                                {'predict': {'command': 'python3 predict.py'},
-                                 'train': {'command': 'python3 train.py'},
-                                 'validate': {'command': 'python3 validate.py'}}}
+    def __init__(self, package_path):
+        self.dispatch_config = {
+            "entry_points": {
+                "predict": {"command": "python3 predict.py"},
+                "train": {"command": "python3 train.py"},
+                "validate": {"command": "python3 validate.py"},
+            }
+        }
 
         self.pkg_path = package_path
         self.pkg_name = None
-        self.dir = package_dir
         self.checksum = None
         self.expected_checksum = None
 
     def download(self, host, port, token, force_ssl=False, secure=False, name=None):
-        """ Download compute package from controller
+        """Download compute package from controller
 
         :param host: host of controller
         :param port: port of controller
         :param token: token for authentication
         :param name: name of package
         :return: True if download was successful, None otherwise
         :rtype: bool
@@ -56,48 +54,45 @@
         if port:
             path = f"{scheme}://{host}:{port}{FEDN_CUSTOM_URL_PREFIX}/download_package"
         else:
             path = f"{scheme}://{host}{FEDN_CUSTOM_URL_PREFIX}/download_package"
         if name:
             path = path + "?name={}".format(name)
 
-        with requests.get(path, stream=True, verify=False, headers={'Authorization': f'{FEDN_AUTH_SCHEME} {token}'}) as r:
+        with requests.get(path, stream=True, verify=False, headers={"Authorization": f"{FEDN_AUTH_SCHEME} {token}"}) as r:
             if 200 <= r.status_code < 204:
-
-                params = cgi.parse_header(
-                    r.headers.get('Content-Disposition', ''))[-1]
+                params = cgi.parse_header(r.headers.get("Content-Disposition", ""))[-1]
                 try:
-                    self.pkg_name = params['filename']
+                    self.pkg_name = params["filename"]
                 except KeyError:
                     logger.error("No package returned.")
                     return None
                 r.raise_for_status()
-                with open(os.path.join(self.pkg_path, self.pkg_name), 'wb') as f:
+                with open(os.path.join(self.pkg_path, self.pkg_name), "wb") as f:
                     for chunk in r.iter_content(chunk_size=8192):
                         f.write(chunk)
         if port:
             path = f"{scheme}://{host}:{port}{FEDN_CUSTOM_URL_PREFIX}/get_package_checksum"
         else:
             path = f"{scheme}://{host}{FEDN_CUSTOM_URL_PREFIX}/get_package_checksum"
 
         if name:
             path = path + "?name={}".format(name)
-        with requests.get(path, verify=False, headers={'Authorization': f'{FEDN_AUTH_SCHEME} {token}'}) as r:
+        with requests.get(path, verify=False, headers={"Authorization": f"{FEDN_AUTH_SCHEME} {token}"}) as r:
             if 200 <= r.status_code < 204:
-
                 data = r.json()
                 try:
-                    self.checksum = data['checksum']
+                    self.checksum = data["checksum"]
                 except Exception:
                     logger.error("Could not extract checksum.")
 
         return True
 
     def validate(self, expected_checksum):
-        """ Validate the package against the checksum provided by the controller
+        """Validate the package against the checksum provided by the controller
 
         :param expected_checksum: checksum provided by the controller
         :return: True if checksums match, False otherwise
         :rtype: bool
         """
         self.expected_checksum = expected_checksum
 
@@ -107,59 +102,59 @@
         if self.checksum == self.expected_checksum == file_checksum:
             logger.info("Package validated {}".format(self.checksum))
             return True
         else:
             return False
 
     def unpack(self):
-        """ Unpack the compute package
+        """Unpack the compute package
 
         :return: True if unpacking was successful, False otherwise
         :rtype: bool
         """
         if self.pkg_name:
             f = None
-            if self.pkg_name.endswith('tar.gz'):
-                f = tarfile.open(os.path.join(
-                    self.pkg_path, self.pkg_name), 'r:gz')
-            if self.pkg_name.endswith('.tgz'):
-                f = tarfile.open(os.path.join(
-                    self.pkg_path, self.pkg_name), 'r:gz')
-            if self.pkg_name.endswith('tar.bz2'):
-                f = tarfile.open(os.path.join(
-                    self.pkg_path, self.pkg_name), 'r:bz2')
+            if self.pkg_name.endswith("tar.gz"):
+                f = tarfile.open(os.path.join(self.pkg_path, self.pkg_name), "r:gz")
+            if self.pkg_name.endswith(".tgz"):
+                f = tarfile.open(os.path.join(self.pkg_path, self.pkg_name), "r:gz")
+            if self.pkg_name.endswith("tar.bz2"):
+                f = tarfile.open(os.path.join(self.pkg_path, self.pkg_name), "r:bz2")
         else:
-            logger.error(
-                "Failed to unpack compute package, no pkg_name set."
-                "Has the reducer been configured with a compute package?"
-            )
+            logger.error("Failed to unpack compute package, no pkg_name set." "Has the reducer been configured with a compute package?")
             return False
 
-        os.getcwd()
         try:
-            os.chdir(self.dir)
-
             if f:
-                f.extractall()
-                logger.info("Successfully extracted compute package content in {}".format(self.dir))
-                return True
+                f.extractall(self.pkg_path)
+                logger.info("Successfully extracted compute package content in {}".format(self.pkg_path))
+                # delete the tarball
+                logger.info("Deleting temporary package tarball file.")
+                f.close()
+                os.remove(os.path.join(self.pkg_path, self.pkg_name))
+                # search for file fedn.yaml in extracted package
+                for root, dirs, files in os.walk(self.pkg_path):
+                    if "fedn.yaml" in files:
+                        # Get the path to where fedn.yaml is located
+                        logger.info("Found fedn.yaml file in {}".format(root))
+                        return True, root
+
+                logger.error("No fedn.yaml file found in extracted package!")
+                return False, ""
         except Exception:
             logger.error("Error extracting files.")
-            return False
+            # delete the tarball
+            os.remove(os.path.join(self.pkg_path, self.pkg_name))
+            return False, ""
 
     def dispatcher(self, run_path):
-        """ Dispatch the compute package
+        """Dispatch the compute package
 
         :param run_path: path to dispatch the compute package
         :type run_path: str
         :return: Dispatcher object
         :rtype: :class:`fedn.utils.dispatcher.Dispatcher`
         """
-        from_path = os.path.join(os.getcwd(), 'client')
-
-        # preserve_times=False ensures compatibility with Gramine LibOS
-        copy_tree(from_path, run_path, preserve_times=False)
-
-        self.dispatch_config = _read_yaml_file(os.path.join(run_path, 'fedn.yaml'))
+        self.dispatch_config = _read_yaml_file(os.path.join(run_path, "fedn.yaml"))
         dispatcher = Dispatcher(self.dispatch_config, run_path)
 
         return dispatcher
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/clients/state.py` & `fedn-0.9.5/fedn/network/clients/state.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 from enum import Enum
 
-from fedn.common.telemetry import tracer
-
 
 class ClientState(Enum):
-    """ Enum for representing the state of a client."""
+    """Enum for representing the state of a client."""
+
     idle = 1
     training = 2
     validating = 3
 
 
-@tracer.start_as_current_span(name="ClientStateToString")
 def ClientStateToString(state):
-    """ Convert a ClientState to a string representation.
+    """Convert a ClientState to a string representation.
 
     :param state: the state to convert
     :type state: :class:`fedn.network.clients.state.ClientState`
     :return: string representation of the state
     :rtype: str
     """
     if state == ClientState.idle:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/clients/test_client.py` & `fedn-0.9.5/fedn/network/clients/test_client.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/aggregator.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/aggregatorbase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,121 +1,160 @@
+import importlib
 import json
 import queue
 from abc import ABC, abstractmethod
 
-import fedn.common.net.grpc.fedn_pb2 as fedn
-from fedn.common.telemetry import trace_all_methods
+from fedn.common.log_config import logger
 
+AGGREGATOR_PLUGIN_PATH = "fedn.network.combiner.aggregators.{}"
 
-@trace_all_methods
-class Aggregator(ABC):
-    """ Abstract class defining an aggregator. """
 
-    @abstractmethod
-    def __init__(self, id, storage, server, modelservice, control):
-        """ Initialize the aggregator.
+class AggregatorBase(ABC):
+    """ Abstract class defining an aggregator.
 
-        :param id: A reference to id of :class: `fedn.network.combiner.Combiner`
-        :type id: str
-        :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
-        :type storage: class: `fedn.common.storage.s3.s3repo.S3ModelRepository`
-        :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
-        :type server: class: `fedn.network.combiner.Combiner`
-        :param modelservice: A handle to the model service :class: `fedn.network.combiner.modelservice.ModelService`
-        :type modelservice: class: `fedn.network.combiner.modelservice.ModelService`
-        :param control: A handle to the :class: `fedn.network.combiner.round.RoundController`
-        :type control: class: `fedn.network.combiner.round.RoundController`
-        """
+    :param id: A reference to id of :class: `fedn.network.combiner.Combiner`
+    :type id: str
+    :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
+    :type storage: class: `fedn.common.storage.s3.s3repo.S3ModelRepository`
+    :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
+    :type server: class: `fedn.network.combiner.Combiner`
+    :param modelservice: A handle to the model service :class: `fedn.network.combiner.modelservice.ModelService`
+    :type modelservice: class: `fedn.network.combiner.modelservice.ModelService`
+    :param control: A handle to the :class: `fedn.network.combiner.roundhandler.RoundHandler`
+    :type control: class: `fedn.network.combiner.roundhandler.RoundHandler`
+    """
+
+    @abstractmethod
+    def __init__(self, storage, server, modelservice, round_handler):
+        """ Initialize the aggregator."""
         self.name = self.__class__.__name__
         self.storage = storage
-        self.id = id
         self.server = server
         self.modelservice = modelservice
-        self.control = control
+        self.round_handler = round_handler
         self.model_updates = queue.Queue()
 
     @abstractmethod
-    def combine_models(self, nr_expected_models=None, nr_required_models=1, helper=None, timeout=180):
+    def combine_models(self, nr_expected_models=None, nr_required_models=1, helper=None, timeout=180, delete_models=True, parameters=None):
         """Routine for combining model updates. Implemented in subclass.
 
         :param nr_expected_models: Number of expected models. If None, wait for all models.
         :type nr_expected_models: int
         :param nr_required_models: Number of required models to combine.
         :type nr_required_models: int
         :param helper: A helper object.
         :type helper: :class: `fedn.utils.plugins.helperbase.HelperBase`
         :param timeout: Timeout in seconds to wait for models to be combined.
         :type timeout: int
-        :return: A combined model.
+        :param delete_models: Delete client models after combining.
+        :type delete_models: bool
+        :param parameters: Additional key-word arguments.
+        :type parameters: dict
+        :return: The global model and metadata
+        :rtype: tuple
         """
         pass
 
     def on_model_update(self, model_update):
         """Callback when a new client model update is recieved.
-           Performs (optional) pre-processing and then puts the update id
-           on the aggregation queue. Override in subclass as needed.
 
-        :param model_update: A ModelUpdate message.
+        Performs (optional) validation and pre-processing,
+        and then puts the update id on the aggregation queue.
+        Override in subclass as needed.
+
+        :param model_update: fedn.network.grpc.fedn.proto.ModelUpdate
         :type model_id: str
         """
         try:
-            self.server.report_status("AGGREGATOR({}): callback received model update {}".format(self.name, model_update.model_update_id),
-                                      log_level=fedn.Status.INFO)
+            logger.info("AGGREGATOR({}): callback received model update {}".format(self.name, model_update.model_update_id))
 
             # Validate the update and metadata
             valid_update = self._validate_model_update(model_update)
             if valid_update:
                 # Push the model update to the processing queue
                 self.model_updates.put(model_update)
             else:
-                self.server.report_status("AGGREGATOR({}): Invalid model update, skipping.".format(self.name))
+                logger.warning("AGGREGATOR({}): Invalid model update, skipping.".format(self.name))
         except Exception as e:
-            self.server.report_status("AGGREGATOR({}): Failed to receive candidate model! {}".format(self.name, e),
-                                      log_level=fedn.Status.WARNING)
+            logger.error("AGGREGATOR({}): failed to receive model update! {}".format(self.name, e))
             pass
 
-    def on_model_validation(self, model_validation):
-        """ Callback when a new client model validation is recieved.
-            Performs (optional) pre-processing and then writes the validation
-            to the database. Override in subclass as needed.
-
-        :param validation: Dict containing validation data sent by client.
-                           Must be valid JSON.
-        :type validation: dict
-        """
-
-        # self.report_validation(validation)
-        self.server.report_status("AGGREGATOR({}): callback processed validation {}".format(self.name, model_validation.model_id),
-                                  log_level=fedn.Status.INFO)
-
     def _validate_model_update(self, model_update):
         """ Validate the model update.
 
         :param model_update: A ModelUpdate message.
         :type model_update: object
         :return: True if the model update is valid, False otherwise.
         :rtype: bool
         """
-        # TODO: Validate the metadata to check that it contains all variables assumed by the aggregator.
-        data = json.loads(model_update.meta)['training_metadata']
-        if 'num_examples' not in data.keys():
-            self.server.report_status("AGGREGATOR({}): Model validation failed, num_examples missing in metadata.".format(self.name))
+        data = json.loads(model_update.meta)["training_metadata"]
+        if "num_examples" not in data.keys():
+            logger.error("AGGREGATOR({}): Model validation failed, num_examples missing in metadata.".format(self.name))
             return False
         return True
 
-    def next_model_update(self, helper):
+    def next_model_update(self):
         """ Get the next model update from the queue.
 
         :param helper: A helper object.
         :type helper: object
-        :return: A tuple containing the model update, metadata and model id.
-        :rtype: tuple
+        :return: The model update.
+        :rtype: fedn.network.grpc.fedn.proto.ModelUpdate
         """
         model_update = self.model_updates.get(block=False)
+        return model_update
+
+    def load_model_update(self, model_update, helper):
+        """ Load the memory representation of the model update.
+
+        Load the model update paramters and the
+        associate metadata into memory.
+
+        :param model_update: The model update.
+        :type model_update: fedn.network.grpc.fedn.proto.ModelUpdate
+        :param helper: A helper object.
+        :type helper: fedn.utils.helpers.helperbase.Helper
+        :return: A tuple of (parameters, metadata)
+        :rtype: tuple
+        """
         model_id = model_update.model_update_id
-        model_next = self.control.load_model_update(helper, model_id)
+        model = self.round_handler.load_model_update(helper, model_id)
         # Get relevant metadata
-        data = json.loads(model_update.meta)['training_metadata']
-        config = json.loads(json.loads(model_update.meta)['config'])
-        data['round_id'] = config['round_id']
-
-        return model_next, data, model_id
+        metadata = json.loads(model_update.meta)
+        if "config" in metadata.keys():
+            # Used in Python client
+            config = json.loads(metadata["config"])
+        else:
+            # Used in C++ client
+            config = json.loads(model_update.config)
+        training_metadata = metadata["training_metadata"]
+        training_metadata["round_id"] = config["round_id"]
+
+        return model, training_metadata
+
+    def get_state(self):
+        """ Get the state of the aggregator's queue, including the number of model updates."""
+        state = {
+            "queue_len": self.model_updates.qsize()
+        }
+        return state
+
+
+def get_aggregator(aggregator_module_name, storage, server, modelservice, control):
+    """ Return an instance of the helper class.
+
+    :param helper_module_name: The name of the helper plugin module.
+    :type helper_module_name: str
+    :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
+    :type storage: class: `fedn.common.storage.s3.s3repo.S3ModelRepository`
+    :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
+    :type server: class: `fedn.network.combiner.Combiner`
+    :param modelservice: A handle to the model service :class: `fedn.network.combiner.modelservice.ModelService`
+    :type modelservice: class: `fedn.network.combiner.modelservice.ModelService`
+    :param control: A handle to the :class: `fedn.network.combiner.roundhandler.RoundHandler`
+    :type control: class: `fedn.network.combiner.roundhandler.RoundHandler`
+    :return: An aggregator instance.
+    :rtype: class: `fedn.combiner.aggregators.AggregatorBase`
+    """
+    aggregator_plugin = AGGREGATOR_PLUGIN_PATH.format(aggregator_module_name)
+    aggregator = importlib.import_module(aggregator_plugin)
+    return aggregator.Aggregator(storage, server, modelservice, control)
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/aggregators/fedavg.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/fedavg.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
+import traceback
+
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.combiner.aggregators.aggregatorbase import AggregatorBase
 
 
-@trace_all_methods
 class Aggregator(AggregatorBase):
-    """ Local SGD / Federated Averaging (FedAvg) aggregator. Computes a weighted mean
+    """Local SGD / Federated Averaging (FedAvg) aggregator. Computes a weighted mean
         of parameter updates.
 
     :param id: A reference to id of :class: `fedn.network.combiner.Combiner`
     :type id: str
     :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
     :type storage: class: `fedn.common.storage.s3.s3repo.S3ModelRepository`
     :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
@@ -19,77 +19,72 @@
     :param control: A handle to the :class: `fedn.network.combiner.roundhandler.RoundHandler`
     :type control: class: `fedn.network.combiner.roundhandler.RoundHandler`
 
     """
 
     def __init__(self, storage, server, modelservice, round_handler):
         """Constructor method"""
-
         super().__init__(storage, server, modelservice, round_handler)
 
         self.name = "fedavg"
 
-    def combine_models(self, helper=None, delete_models=True):
+    def combine_models(self, helper=None, delete_models=True, parameters=None):
         """Aggregate all model updates in the queue by computing an incremental
         weighted average of model parameters.
 
         :param helper: An instance of :class: `fedn.utils.helpers.helpers.HelperBase`, ML framework specific helper, defaults to None
         :type helper: class: `fedn.utils.helpers.helpers.HelperBase`, optional
         :param time_window: The time window for model aggregation, defaults to 180
         :type time_window: int, optional
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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/combiner.py` & `fedn-0.9.5/fedn/network/combiner/combiner.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,37 +8,36 @@
 import time
 import uuid
 from datetime import datetime, timedelta
 from enum import Enum
 
 import fedn.network.grpc.fedn_pb2 as fedn
 import fedn.network.grpc.fedn_pb2_grpc as rpc
-from fedn.common.log_config import (logger, set_log_level_from_string,
-                                    set_log_stream)
-from fedn.common.telemetry import trace_all_methods
+from fedn.common.log_config import logger, set_log_level_from_string, set_log_stream
 from fedn.network.combiner.connect import ConnectorCombiner, Status
 from fedn.network.combiner.modelservice import ModelService
 from fedn.network.combiner.roundhandler import RoundHandler
 from fedn.network.grpc.server import Server
 from fedn.network.storage.s3.repository import Repository
 from fedn.network.storage.statestore.mongostatestore import MongoStateStore
 
-VALID_NAME_REGEX = '^[a-zA-Z0-9_-]*$'
+VALID_NAME_REGEX = "^[a-zA-Z0-9_-]*$"
 
 
 class Role(Enum):
-    """ Enum for combiner roles. """
+    """Enum for combiner roles."""
+
     WORKER = 1
     COMBINER = 2
     REDUCER = 3
     OTHER = 4
 
 
 def role_to_proto_role(role):
-    """ Convert a Role to a proto Role.
+    """Convert a Role to a proto Role.
 
     :param role: the role to convert
     :type role: :class:`fedn.network.combiner.server.Role`
     :return: proto role
     :rtype: :class:`fedn.network.grpc.fedn_pb2.Role`
     """
     if role == Role.COMBINER:
@@ -47,52 +46,51 @@
         return fedn.WORKER
     if role == Role.REDUCER:
         return fedn.REDUCER
     if role == Role.OTHER:
         return fedn.OTHER
 
 
-@trace_all_methods
 class Combiner(rpc.CombinerServicer, rpc.ReducerServicer, rpc.ConnectorServicer, rpc.ControlServicer):
-    """ Combiner gRPC server.
+    """Combiner gRPC server.
 
     :param config: configuration for the combiner
     :type config: dict
     """
 
     def __init__(self, config):
-        """ Initialize Combiner server."""
-
-        set_log_level_from_string(config.get('verbosity', "INFO"))
-        set_log_stream(config.get('logfile', None))
+        """Initialize Combiner server."""
+        set_log_level_from_string(config.get("verbosity", "INFO"))
+        set_log_stream(config.get("logfile", None))
 
         # Client queues
         self.clients = {}
 
-        self.modelservice = ModelService()
 
         # Validate combiner name
-        match = re.search(VALID_NAME_REGEX, config['name'])
+        match = re.search(VALID_NAME_REGEX, config["name"])
         if not match:
-            raise ValueError('Unallowed character in combiner name. Allowed characters: a-z, A-Z, 0-9, _, -.')
+            raise ValueError("Unallowed character in combiner name. Allowed characters: a-z, A-Z, 0-9, _, -.")
 
-        self.id = config['name']
+        self.id = config["name"]
         self.role = Role.COMBINER
-        self.max_clients = config['max_clients']
+        self.max_clients = config["max_clients"]
 
         # Connector to announce combiner to discover service (reducer)
-        announce_client = ConnectorCombiner(host=config['discover_host'],
-                                            port=config['discover_port'],
-                                            myhost=config['host'],
-                                            fqdn=config['fqdn'],
-                                            myport=config['port'],
-                                            token=config['token'],
-                                            name=config['name'],
-                                            secure=config['secure'],
-                                            verify=config['verify'])
+        announce_client = ConnectorCombiner(
+            host=config["discover_host"],
+            port=config["discover_port"],
+            myhost=config["host"],
+            fqdn=config["fqdn"],
+            myport=config["port"],
+            token=config["token"],
+            name=config["name"],
+            secure=config["secure"],
+            verify=config["verify"],
+        )
 
         while True:
             # Announce combiner to discover service
             status, response = announce_client.announce()
             if status == Status.TryAgain:
                 logger.info(response)
                 time.sleep(5)
@@ -104,39 +102,40 @@
                 logger.info(response)
                 logger.info("Status.UnAuthorized")
                 sys.exit("Exiting: Unauthorized")
             elif status == Status.UnMatchedConfig:
                 logger.info(response)
                 logger.info("Status.UnMatchedConfig")
                 sys.exit("Exiting: Missing config")
-            else:
-                logger.info("Status.Unassigned")
-                time.sleep(5)
 
-        cert = announce_config['certificate']
-        key = announce_config['key']
+        cert = announce_config["certificate"]
+        key = announce_config["key"]
 
-        if announce_config['certificate']:
-            cert = base64.b64decode(announce_config['certificate'])  # .decode('utf-8')
-            key = base64.b64decode(announce_config['key'])  # .decode('utf-8')
+        if announce_config["certificate"]:
+            cert = base64.b64decode(announce_config["certificate"])  # .decode('utf-8')
+            key = base64.b64decode(announce_config["key"])  # .decode('utf-8')
 
         # Set up gRPC server configuration
-        grpc_config = {'port': config['port'],
-                       'secure': config['secure'],
-                       'certificate': cert,
-                       'key': key}
+        grpc_config = {"port": config["port"], "secure": config["secure"], "certificate": cert, "key": key}
 
         # Set up model repository
-        self.repository = Repository(
-            announce_config['storage']['storage_config'])
+        self.repository = Repository(announce_config["storage"]["storage_config"])
+
+        self.statestore = MongoStateStore(announce_config["statestore"]["network_id"], announce_config["statestore"]["mongo_config"])
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
 
-        self.statestore = MongoStateStore(
-            announce_config['statestore']['network_id'],
-            announce_config['statestore']['mongo_config']
-        )
         # Create gRPC server
         self.server = Server(self, self.modelservice, grpc_config)
 
         # Set up round controller
         self.round_handler = RoundHandler(self.repository, self, self.modelservice)
 
         # Start thread for round controller
@@ -145,65 +144,63 @@
         # Start thread for client status updates: TODO: Should be configurable
         threading.Thread(target=self._deamon_thread_client_status, daemon=True).start()
 
         # Start the gRPC server
         self.server.start()
 
     def __whoami(self, client, instance):
-        """ Set the client id and role in a proto message.
+        """Set the client id and role in a proto message.
 
         :param client: the client to set the id and role for
         :type client: :class:`fedn.network.grpc.fedn_pb2.Client`
         :param instance: the instance to get the id and role from
         :type instance: :class:`fedn.network.combiner.server.Combiner`
         :return: the client with id and role set
         :rtype: :class:`fedn.network.grpc.fedn_pb2.Client`
         """
         client.name = instance.id
         client.role = role_to_proto_role(instance.role)
         return client
 
     def request_model_update(self, config, clients=[]):
-        """ Ask clients to update the current global model.
+        """Ask clients to update the current global model.
 
         :param config: the model configuration to send to clients
         :type config: dict
         :param clients: the clients to send the request to
         :type clients: list
 
         """
         # The request to be added to the client queue
         request = fedn.TaskRequest()
-        request.model_id = config['model_id']
+        request.model_id = config["model_id"]
         request.correlation_id = str(uuid.uuid4())
         request.timestamp = str(datetime.now())
         request.data = json.dumps(config)
         request.type = fedn.StatusType.MODEL_UPDATE
-        request.session_id = config['session_id']
+        request.session_id = config["session_id"]
 
         request.sender.name = self.id
         request.sender.role = fedn.COMBINER
 
         if len(clients) == 0:
             clients = self.get_active_trainers()
 
         for client in clients:
             request.receiver.name = client
             request.receiver.role = fedn.WORKER
             self._put_request_to_client_queue(request, fedn.Queue.TASK_QUEUE)
 
         if len(clients) < 20:
-            logger.info("Sent model update request for model {} to clients {}".format(
-                request.model_id, clients))
+            logger.info("Sent model update request for model {} to clients {}".format(request.model_id, clients))
         else:
-            logger.info("Sent model update request for model {} to {} clients".format(
-                request.model_id, len(clients)))
+            logger.info("Sent model update request for model {} to {} clients".format(request.model_id, len(clients)))
 
     def request_model_validation(self, model_id, config, clients=[]):
-        """ Ask clients to validate the current global model.
+        """Ask clients to validate the current global model.
 
         :param model_id: the model id to validate
         :type model_id: str
         :param config: the model configuration to send to clients
         :type config: dict
         :param clients: the clients to send the request to
         :type clients: list
@@ -226,72 +223,70 @@
 
         for client in clients:
             request.receiver.name = client
             request.receiver.role = fedn.WORKER
             self._put_request_to_client_queue(request, fedn.Queue.TASK_QUEUE)
 
         if len(clients) < 20:
-            logger.info("Sent model validation request for model {} to clients {}".format(
-                request.model_id, clients))
+            logger.info("Sent model validation request for model {} to clients {}".format(request.model_id, clients))
         else:
-            logger.info("Sent model validation request for model {} to {} clients".format(
-                request.model_id, len(clients)))
+            logger.info("Sent model validation request for model {} to {} clients".format(request.model_id, len(clients)))
 
     def get_active_trainers(self):
-        """ Get a list of active trainers.
+        """Get a list of active trainers.
 
         :return: the list of active trainers
         :rtype: list
         """
         trainers = self._list_active_clients(fedn.Queue.TASK_QUEUE)
         return trainers
 
     def get_active_validators(self):
-        """ Get a list of active validators.
+        """Get a list of active validators.
 
         :return: the list of active validators
         :rtype: list
         """
         validators = self._list_active_clients(fedn.Queue.TASK_QUEUE)
         return validators
 
     def nr_active_trainers(self):
-        """ Get the number of active trainers.
+        """Get the number of active trainers.
 
         :return: the number of active trainers
         :rtype: int
         """
         return len(self.get_active_trainers())
 
     ####################################################################################################################
 
     def __join_client(self, client):
-        """ Add a client to the list of active clients.
+        """Add a client to the list of active clients.
 
         :param client: the client to add
         :type client: :class:`fedn.network.grpc.fedn_pb2.Client`
         """
         if client.name not in self.clients.keys():
             # The status is set to offline by default, and will be updated once _list_active_clients is called.
             self.clients[client.name] = {"lastseen": datetime.now(), "status": "offline"}
 
     def _subscribe_client_to_queue(self, client, queue_name):
-        """ Subscribe a client to the queue.
+        """Subscribe a client to the queue.
 
         :param client: the client to subscribe
         :type client: :class:`fedn.network.grpc.fedn_pb2.Client`
         :param queue_name: the name of the queue to subscribe to
         :type queue_name: str
         """
         self.__join_client(client)
         if queue_name not in self.clients[client.name].keys():
             self.clients[client.name][queue_name] = queue.Queue()
 
     def __get_queue(self, client, queue_name):
-        """ Get the queue for a client.
+        """Get the queue for a client.
 
         :param client: the client to get the queue for
         :type client: :class:`fedn.network.grpc.fedn_pb2.Client`
         :param queue_name: the name of the queue to get
         :type queue_name: str
         :return: the queue
         :rtype: :class:`queue.Queue`
@@ -300,29 +295,29 @@
         """
         try:
             return self.clients[client.name][queue_name]
         except KeyError:
             raise
 
     def _list_subscribed_clients(self, queue_name):
-        """ List all clients subscribed to a queue.
+        """List all clients subscribed to a queue.
 
         :param queue_name: the name of the queue
         :type queue_name: str
         :return: a list of client names
         :rtype: list
         """
         subscribed_clients = []
         for name, client in self.clients.items():
             if queue_name in client.keys():
                 subscribed_clients.append(name)
         return subscribed_clients
 
     def _list_active_clients(self, channel):
-        """ List all clients that have sent a status message in the last 10 seconds.
+        """List all clients that have sent a status message in the last 10 seconds.
 
         :param channel: the name of the channel
         :type channel: str
         :return: a list of client names
         :rtype: list
         """
         # Temporary dict to store client status
@@ -334,71 +329,64 @@
         for client in self._list_subscribed_clients(channel):
             status = self.clients[client]["status"]
             now = datetime.now()
             then = self.clients[client]["lastseen"]
             if (now - then) < timedelta(seconds=10):
                 clients["active_clients"].append(client)
                 # If client has changed status, update statestore
-                if status == "offline":
+                if status != "online":
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
-        """ Deamon thread that checks for inactive clients and updates statestore. """
+    def _deamon_thread_client_status(self, timeout=5):
+        """Deamon thread that checks for inactive clients and updates statestore."""
         while True:
             time.sleep(timeout)
             # TODO: Also update validation clients
             self._list_active_clients(fedn.Queue.TASK_QUEUE)
 
     def _put_request_to_client_queue(self, request, queue_name):
-        """ Get a client specific queue and add a request to it.
+        """Get a client specific queue and add a request to it.
         The client is identified by the request.receiver.
 
         :param request: the request to send
         :type request: :class:`fedn.network.grpc.fedn_pb2.Request`
         :param queue_name: the name of the queue to send the request to
         :type queue_name: str
         """
         try:
             q = self.__get_queue(request.receiver, queue_name)
             q.put(request)
         except Exception as e:
-            logger.error("Failed to put request to client queue {} for client {}: {}".format(
-                queue_name,
-                request.receiver.name,
-                str(e)))
+            logger.error("Failed to put request to client queue {} for client {}: {}".format(queue_name, request.receiver.name, str(e)))
             raise
 
     def _send_status(self, status):
-        """ Report a status to backend db.
+        """Report a status to backend db.
 
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
@@ -407,15 +395,15 @@
             return False
 
     #####################################################################################################################
 
     # Controller Service
 
     def Start(self, control: fedn.ControlRequest, context):
-        """ Start a round of federated learning"
+        """Start a round of federated learning"
 
         :param control: the control request
         :type control: :class:`fedn.network.grpc.fedn_pb2.ControlRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the control response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
@@ -435,15 +423,15 @@
         p = response.parameter.add()
         p.key = "job_id"
         p.value = job_id
 
         return response
 
     def SetAggregator(self, control: fedn.ControlRequest, context):
-        """ Set the active aggregator.
+        """Set the active aggregator.
 
         :param control: the control request
         :type control: :class:`fedn.network.grpc.fedn_pb2.ControlRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the control response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
@@ -452,45 +440,45 @@
         for parameter in control.parameter:
             aggregator = parameter.value
 
         status = self.round_handler.set_aggregator(aggregator)
 
         response = fedn.ControlResponse()
         if status:
-            response.message = 'Success'
+            response.message = "Success"
         else:
-            response.message = 'Failed'
+            response.message = "Failed"
 
         return response
 
     def FlushAggregationQueue(self, control: fedn.ControlRequest, context):
-        """ Flush the queue.
+        """Flush the queue.
 
         :param control: the control request
         :type control: :class:`fedn.network.grpc.fedn_pb2.ControlRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the control response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
         """
         logger.debug("grpc.Combiner.FlushAggregationQueue: Called")
         status = self._flush_model_update_queue()
 
         response = fedn.ControlResponse()
         if status:
-            response.message = 'Success'
+            response.message = "Success"
         else:
-            response.message = 'Failed'
+            response.message = "Failed"
 
         return response
 
     ##############################################################################
 
     def Stop(self, control: fedn.ControlRequest, context):
-        """ TODO: Not yet implemented.
+        """TODO: Not yet implemented.
 
         :param control: the control request
         :type control: :class:`fedn.network.grpc.fedn_pb2.ControlRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the control response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
@@ -498,15 +486,15 @@
         response = fedn.ControlResponse()
         logger.info("grpc.Combiner.Stop: Called")
         return response
 
     #####################################################################################################################
 
     def SendStatus(self, status: fedn.Status, context):
-        """ A client RPC endpoint that accepts status messages.
+        """A client RPC endpoint that accepts status messages.
 
         :param status: the status message
         :type status: :class:`fedn.network.grpc.fedn_pb2.Status`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.Response`
@@ -515,15 +503,15 @@
         self._send_status(status)
 
         response = fedn.Response()
         response.response = "Status received."
         return response
 
     def ListActiveClients(self, request: fedn.ListClientsRequest, context):
-        """ RPC endpoint that returns a ClientList containing the names of all active clients.
+        """RPC endpoint that returns a ClientList containing the names of all active clients.
             An active client has sent a status message / responded to a heartbeat
             request in the last 10 seconds.
 
         :param request: the request
         :type request: :class:`fedn.network.grpc.fedn_pb2.ListClientsRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
@@ -539,27 +527,26 @@
             logger.info("grpc.Combiner.ListActiveClients: Number active clients: {}".format(nr_active_clients))
 
         for client in active_clients:
             clients.client.append(fedn.Client(name=client, role=fedn.WORKER))
         return clients
 
     def AcceptingClients(self, request: fedn.ConnectionRequest, context):
-        """ RPC endpoint that returns a ConnectionResponse indicating whether the server
+        """RPC endpoint that returns a ConnectionResponse indicating whether the server
         is accepting clients or not.
 
         :param request: the request (unused)
         :type request: :class:`fedn.network.grpc.fedn_pb2.ConnectionRequest`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ConnectionResponse`
         """
         response = fedn.ConnectionResponse()
-        active_clients = self._list_active_clients(
-            fedn.Queue.TASK_QUEUE)
+        active_clients = self._list_active_clients(fedn.Queue.TASK_QUEUE)
 
         try:
             requested = int(self.max_clients)
             if len(active_clients) >= requested:
                 response.status = fedn.ConnectionStatus.NOT_ACCEPTING
                 return response
             if len(active_clients) < requested:
@@ -570,15 +557,15 @@
             logger.error("Combiner not properly configured! {}".format(e))
             raise
 
         response.status = fedn.ConnectionStatus.TRY_AGAIN_LATER
         return response
 
     def SendHeartbeat(self, heartbeat: fedn.Heartbeat, context):
-        """ RPC that lets clients send a hearbeat, notifying the server that
+        """RPC that lets clients send a hearbeat, notifying the server that
             the client is available.
 
         :param heartbeat: the heartbeat
         :type heartbeat: :class:`fedn.network.grpc.fedn_pb2.Heartbeat`
         :param context: the context (unused)
         :type context: :class:`grpc._server._Context`
         :return: the response
@@ -595,41 +582,42 @@
         response.sender.role = heartbeat.sender.role
         response.response = "Heartbeat received"
         return response
 
     # Combiner Service
 
     def TaskStream(self, response, context):
-        """ A server stream RPC endpoint (Update model). Messages from client stream.
+        """A server stream RPC endpoint (Update model). Messages from client stream.
 
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
-            logger.info("grpc.Combiner.TaskStream: Client connected: {}\n".format(metadata['client']))
+            logger.info("grpc.Combiner.TaskStream: Client connected: {}\n".format(metadata["client"]))
 
-        status = fedn.Status(
-            status="Client {} connecting to TaskStream.".format(client.name))
+        status = fedn.Status(status="Client {} connecting to TaskStream.".format(client.name))
         status.log_level = fedn.Status.INFO
         status.timestamp.GetCurrentTime()
 
         self.__whoami(status.sender, self)
 
-        self._subscribe_client_to_queue(
-            client, fedn.Queue.TASK_QUEUE)
+        self._subscribe_client_to_queue(client, fedn.Queue.TASK_QUEUE)
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
@@ -638,64 +626,59 @@
                 yield q.get(timeout=1.0)
             except queue.Empty:
                 pass
             except Exception as e:
                 logger.error("Error in ModelUpdateRequestStream: {}".format(e))
 
     def SendModelUpdate(self, request, context):
-        """ Send a model update response.
+        """Send a model update response.
 
         :param request: the request
         :type request: :class:`fedn.network.grpc.fedn_pb2.ModelUpdate`
         :param context: the context
         :type context: :class:`grpc._server._Context`
         :return: the response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.Response`
         """
         self.round_handler.aggregator.on_model_update(request)
 
         response = fedn.Response()
-        response.response = "RECEIVED ModelUpdate {} from client  {}".format(
-            response, response.sender.name)
+        response.response = "RECEIVED ModelUpdate {} from client  {}".format(response, response.sender.name)
         return response  # TODO Fill later
 
     def register_model_validation(self, validation):
         """Register a model validation.
 
         :param validation: the model validation
         :type validation: :class:`fedn.network.grpc.fedn_pb2.ModelValidation`
         """
-
         self.statestore.report_validation(validation)
 
     def SendModelValidation(self, request, context):
-        """ Send a model validation response.
+        """Send a model validation response.
 
         :param request: the request
         :type request: :class:`fedn.network.grpc.fedn_pb2.ModelValidation`
         :param context: the context
         :type context: :class:`grpc._server._Context`
         :return: the response
         :rtype: :class:`fedn.network.grpc.fedn_pb2.Response`
         """
         logger.info("Recieved ModelValidation from {}".format(request.sender.name))
 
         self.register_model_validation(request)
 
         response = fedn.Response()
-        response.response = "RECEIVED ModelValidation {} from client  {}".format(
-            response, response.sender.name)
+        response.response = "RECEIVED ModelValidation {} from client  {}".format(response, response.sender.name)
         return response
 
     ####################################################################################################################
 
     def run(self):
-        """ Start the server."""
-
-        logger.info("COMBINER: {} started, ready for gRPC requests.".format(
-            self.id))
+        """Start the server."""
+        logger.info("COMBINER: {} started, ready for gRPC requests.".format(self.id))
         try:
             while True:
                 signal.pause()
         except (KeyboardInterrupt, SystemExit):
             pass
         self.server.stop()
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/connect.py` & `fedn-0.9.5/fedn/network/combiner/connect.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 #
 import enum
 import os
 
 import requests
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 
 
 class Status(enum.Enum):
-    """ Enum for representing the status of a combiner announcement."""
+    """Enum for representing the status of a combiner announcement."""
+
     Unassigned = 0
     Assigned = 1
     TryAgain = 2
     UnAuthorized = 3
     UnMatchedConfig = 4
 
 
-@trace_all_methods
 class ConnectorCombiner:
-    """ Connector for annnouncing combiner to the FEDn network.
+    """Connector for annnouncing combiner to the FEDn network.
 
     :param host: host of discovery service
     :type host: str
     :param port: port of discovery service
     :type port: int
     :param myhost: host of combiner
     :type myhost: str
@@ -43,15 +42,15 @@
     :param secure: True if https is used, False if http
     :type secure: bool
     :param verify: True if certificate is verified, False if not
     :type verify: bool
     """
 
     def __init__(self, host, port, myhost, fqdn, myport, token, name, secure=False, verify=False):
-        """ Initialize the ConnectorCombiner.
+        """Initialize the ConnectorCombiner.
 
         :param host: The host of the discovery service.
         :type host: str
         :param port: The port of the discovery service.
         :type port: int
         :param myhost: The host of the combiner.
         :type myhost: str
@@ -64,71 +63,64 @@
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
-        self.token_scheme = os.environ.get('FEDN_AUTH_SCHEME', 'Bearer')
+        self.token_scheme = os.environ.get("FEDN_AUTH_SCHEME", "Bearer")
         self.name = name
         self.secure = secure
         self.verify = verify
 
         if not self.token:
-            self.token = os.environ.get('FEDN_AUTH_TOKEN', None)
+            self.token = os.environ.get("FEDN_AUTH_TOKEN", None)
 
         # for https we assume a an ingress handles permanent redirect (308)
         self.prefix = "http://"
         if port:
-            self.connect_string = "{}{}:{}".format(
-                self.prefix, self.host, self.port)
+            self.connect_string = "{}{}:{}".format(self.prefix, self.host, self.port)
         else:
-            self.connect_string = "{}{}".format(
-                self.prefix, self.host)
+            self.connect_string = "{}{}".format(self.prefix, self.host)
 
         logger.info("Setting connection string to {}".format(self.connect_string))
 
     def announce(self):
-        """
-        Announce combiner to FEDn network via discovery service (REST-API).
+        """Announce combiner to FEDn network via discovery service (REST-API).
 
         :return: Tuple with announcement Status, FEDn network configuration if sucessful, else None.
         :rtype: :class:`fedn.network.combiner.connect.Status`, str
         """
-        payload = {
-            "combiner_id": self.name,
-            "address": self.myhost,
-            "fqdn": self.fqdn,
-            "port": self.myport,
-            "secure_grpc": self.secure
-        }
-        url_prefix = os.environ.get('FEDN_CUSTOM_URL_PREFIX', '')
+        payload = {"combiner_id": self.name, "address": self.myhost, "fqdn": self.fqdn, "port": self.myport, "secure_grpc": self.secure}
+        url_prefix = os.environ.get("FEDN_CUSTOM_URL_PREFIX", "")
         try:
-            retval = requests.post(self.connect_string + url_prefix + '/add_combiner', json=payload,
-                                   verify=self.verify,
-                                   headers={'Authorization': f'{self.token_scheme} {self.token}'})
+            retval = requests.post(
+                self.connect_string + url_prefix + "/add_combiner",
+                json=payload,
+                verify=self.verify,
+                headers={"Authorization": f"{self.token_scheme} {self.token}"},
+            )
         except Exception:
             return Status.Unassigned, {}
 
         if retval.status_code == 400:
             # Get error messange from response
-            reason = retval.json()['message']
+            reason = retval.json()["message"]
             return Status.UnMatchedConfig, reason
 
         if retval.status_code == 401:
             reason = "Unauthorized connection to reducer, make sure the correct token is set"
             return Status.UnAuthorized, reason
 
         if retval.status_code >= 200 and retval.status_code < 204:
-            if retval.json()['status'] == 'retry':
-                reason = retval.json()['message']
+            if retval.json()["status"] == "retry":
+                reason = retval.json()["message"]
                 return Status.TryAgain, reason
             return Status.Assigned, retval.json()
 
         return Status.Unassigned, None
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/interfaces.py` & `fedn-0.9.5/fedn/network/combiner/interfaces.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,35 +4,33 @@
 import time
 from io import BytesIO
 
 import grpc
 
 import fedn.network.grpc.fedn_pb2 as fedn
 import fedn.network.grpc.fedn_pb2_grpc as rpc
-from fedn.common.telemetry import trace_all_methods
 
 
 class CombinerUnavailableError(Exception):
     pass
 
 
-@trace_all_methods
 class Channel:
-    """ Wrapper for a gRPC channel.
+    """Wrapper for a gRPC channel.
 
     :param address: The address for the gRPC server.
     :type address: str
     :param port: The port for connecting to the gRPC server.
     :type port: int
     :param certificate: The certificate for connecting to the gRPC server (optional)
     :type certificate: str
     """
 
     def __init__(self, address, port, certificate=None):
-        """ Create a channel.
+        """Create a channel.
 
         If a valid certificate is given, a secure channel is created, else insecure.
 
         :parameter address: The address for the gRPC server.
         :type address: str
         :parameter port: The port for connecting to the gRPC server.
         :type port: int
@@ -40,34 +38,30 @@
         :type certificate: str
         """
         self.address = address
         self.port = port
         self.certificate = certificate
 
         if self.certificate:
-            credentials = grpc.ssl_channel_credentials(
-                root_certificates=copy.deepcopy(certificate))
-            self.channel = grpc.secure_channel('{}:{}'.format(
-                self.address, str(self.port)), credentials)
+            credentials = grpc.ssl_channel_credentials(root_certificates=copy.deepcopy(certificate))
+            self.channel = grpc.secure_channel("{}:{}".format(self.address, str(self.port)), credentials)
         else:
-            self.channel = grpc.insecure_channel(
-                '{}:{}'.format(self.address, str(self.port)))
+            self.channel = grpc.insecure_channel("{}:{}".format(self.address, str(self.port)))
 
     def get_channel(self):
-        """ Get a channel.
+        """Get a channel.
 
         :return: An instance of a gRPC channel
         :rtype: :class:`grpc.Channel`
         """
         return copy.copy(self.channel)
 
 
-@trace_all_methods
 class CombinerInterface:
-    """ Interface for the Combiner (aggregation server).
+    """Interface for the Combiner (aggregation server).
         Abstraction on top of the gRPC server servicer.
 
     :param parent: The parent combiner (controller)
     :type parent: :class:`fedn.network.api.interfaces.API`
     :param name: The name of the combiner.
     :type name: str
     :param address: The address of the combiner.
@@ -83,127 +77,120 @@
     :param ip: The ip of the combiner (optional).
     :type ip: str
     :param config: The configuration of the combiner (optional).
     :type config: dict
     """
 
     def __init__(self, parent, name, address, fqdn, port, certificate=None, key=None, ip=None, config=None):
-        """ Initialize the combiner interface."""
+        """Initialize the combiner interface."""
         self.parent = parent
         self.name = name
         self.address = address
         self.fqdn = fqdn
         self.port = port
         self.certificate = certificate
         self.key = key
         self.ip = ip
 
         if not config:
-            self.config = {
-                'max_clients': 8
-            }
+            self.config = {"max_clients": 8}
         else:
             self.config = config
 
     @classmethod
     def from_json(combiner_config):
-        """ Initialize the combiner config from a json document.
+        """Initialize the combiner config from a json document.
 
         :parameter combiner_config: The combiner configuration.
         :type combiner_config: dict
         :return: An instance of the combiner interface.
         :rtype: :class:`fedn.network.combiner.interfaces.CombinerInterface`
         """
         return CombinerInterface(**combiner_config)
 
     def to_dict(self):
-        """ Export combiner configuration to a dictionary.
+        """Export combiner configuration to a dictionary.
 
         :return: A dictionary with the combiner configuration.
         :rtype: dict
         """
-
         data = {
-            'parent': self.parent,
-            'name': self.name,
-            'address': self.address,
-            'fqdn': self.fqdn,
-            'port': self.port,
-            'ip': self.ip,
-            'certificate': None,
-            'key': None,
-            'config': self.config
+            "parent": self.parent,
+            "name": self.name,
+            "address": self.address,
+            "fqdn": self.fqdn,
+            "port": self.port,
+            "ip": self.ip,
+            "certificate": None,
+            "key": None,
+            "config": self.config,
         }
 
         if self.certificate:
             cert_b64 = base64.b64encode(self.certificate)
             key_b64 = base64.b64encode(self.key)
-            data['certificate'] = str(cert_b64).split('\'')[1]
-            data['key'] = str(key_b64).split('\'')[1]
+            data["certificate"] = str(cert_b64).split("'")[1]
+            data["key"] = str(key_b64).split("'")[1]
 
         return data
 
     def to_json(self):
-        """ Export combiner configuration to json.
+        """Export combiner configuration to json.
 
         :return: A json document with the combiner configuration.
         :rtype: str
         """
         return json.dumps(self.to_dict())
 
     def get_certificate(self):
-        """ Get combiner certificate.
+        """Get combiner certificate.
 
         :return: The combiner certificate.
         :rtype: str, None if no certificate is set.
         """
         if self.certificate:
             cert_b64 = base64.b64encode(self.certificate)
-            return str(cert_b64).split('\'')[1]
+            return str(cert_b64).split("'")[1]
         else:
             return None
 
     def get_key(self):
-        """ Get combiner key.
+        """Get combiner key.
 
         :return: The combiner key.
         :rtype: str, None if no key is set.
         """
         if self.key:
             key_b64 = base64.b64encode(self.key)
-            return str(key_b64).split('\'')[1]
+            return str(key_b64).split("'")[1]
         else:
             return None
 
     def flush_model_update_queue(self):
-        """ Reset the model update queue on the combiner. """
-
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        """Reset the model update queue on the combiner."""
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ControlStub(channel)
 
         request = fedn.ControlRequest()
 
         try:
             control.FlushAggregationQueue(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
                 raise CombinerUnavailableError
             else:
                 raise
 
     def set_aggregator(self, aggregator):
-        """ Set the active aggregator module.
+        """Set the active aggregator module.
 
         :param aggregator: The name of the aggregator module.
         :type config: str
         """
-
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ControlStub(channel)
 
         request = fedn.ControlRequest()
         p = request.parameter.add()
         p.key = "aggregator"
         p.value = aggregator
 
@@ -212,23 +199,22 @@
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
                 raise CombinerUnavailableError
             else:
                 raise
 
     def submit(self, config):
-        """ Submit a compute plan to the combiner.
+        """Submit a compute plan to the combiner.
 
         :param config: The job configuration.
         :type config: dict
         :return: Server ControlResponse object.
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ControlResponse`
         """
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ControlStub(channel)
         request = fedn.ControlRequest()
         request.command = fedn.Command.START
         for k, v in config.items():
             p = request.parameter.add()
             p.key = str(k)
             p.value = str(v)
@@ -240,24 +226,22 @@
                 raise CombinerUnavailableError
             else:
                 raise
 
         return response
 
     def get_model(self, id, timeout=10):
-        """ Download a model from the combiner server.
+        """Download a model from the combiner server.
 
         :param id: The model id.
         :type id: str
         :return: A file-like object containing the model.
         :rtype: :class:`io.BytesIO`, None if the model is not available.
         """
-
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         modelservice = rpc.ModelServiceStub(channel)
 
         data = BytesIO()
         data.seek(0, 0)
 
         time_start = time.time()
 
@@ -275,21 +259,20 @@
                 return None
             if part.status == fedn.ModelStatus.UNKNOWN:
                 if time.time() - time_start > timeout:
                     return None
                 continue
 
     def allowing_clients(self):
-        """ Check if the combiner is allowing additional client connections.
+        """Check if the combiner is allowing additional client connections.
 
         :return: True if accepting, else False.
         :rtype: bool
         """
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         connector = rpc.ConnectorStub(channel)
         request = fedn.ConnectionRequest()
 
         try:
             response = connector.AcceptingClients(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
@@ -302,24 +285,23 @@
             return True
         if response.status == fedn.ConnectionStatus.TRY_AGAIN_LATER:
             return False
 
         return False
 
     def list_active_clients(self, queue=1):
-        """ List active clients.
+        """List active clients.
 
         :param queue: The channel (queue) to use (optional). Default is 1 = MODEL_UPDATE_REQUESTS channel.
             see :class:`fedn.network.grpc.fedn_pb2.Channel`
         :type channel: int
         :return: A list of active clients.
         :rtype: json
         """
-        channel = Channel(self.address, self.port,
-                          self.certificate).get_channel()
+        channel = Channel(self.address, self.port, self.certificate).get_channel()
         control = rpc.ConnectorStub(channel)
         request = fedn.ListClientsRequest()
         request.channel = queue
         try:
             response = control.ListActiveClients(request)
         except grpc.RpcError as e:
             if e.code() == grpc.StatusCode.UNAVAILABLE:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/modelservice.py` & `fedn-0.9.5/fedn/network/combiner/modelservice.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,43 +1,38 @@
 import os
 import tempfile
 from io import BytesIO
 
 import fedn.network.grpc.fedn_pb2 as fedn
 import fedn.network.grpc.fedn_pb2_grpc as rpc
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods, tracer
 from fedn.network.storage.models.tempmodelstorage import TempModelStorage
 
 CHUNK_SIZE = 1024 * 1024
 
 
-@tracer.start_as_current_span(name="upload_request_generator")
 def upload_request_generator(mdl, id):
     """Generator function for model upload requests.
 
     :param mdl: The model update object.
     :type mdl: BytesIO
     :return: A model update request.
     :rtype: fedn.ModelRequest
     """
     while True:
         b = mdl.read(CHUNK_SIZE)
         if b:
-            result = fedn.ModelRequest(
-                data=b, id=id, status=fedn.ModelStatus.IN_PROGRESS)
+            result = fedn.ModelRequest(data=b, id=id, status=fedn.ModelStatus.IN_PROGRESS)
         else:
-            result = fedn.ModelRequest(
-                id=id, data=None, status=fedn.ModelStatus.OK)
+            result = fedn.ModelRequest(id=id, data=None, status=fedn.ModelStatus.OK)
         yield result
         if not b:
             break
 
 
-@tracer.start_as_current_span(name="model_as_bytesIO")
 def model_as_bytesIO(model):
     if not isinstance(model, BytesIO):
         bt = BytesIO()
 
         written_total = 0
         for d in model.stream(32 * 1024):
             written = bt.write(d)
@@ -45,117 +40,110 @@
     else:
         bt = model
 
     bt.seek(0, 0)
     return bt
 
 
-@tracer.start_as_current_span(name="get_tmp_path")
 def get_tmp_path():
-    """ Return a temporary output path compatible with save_model, load_model. """
+    """Return a temporary output path compatible with save_model, load_model."""
     fd, path = tempfile.mkstemp()
     os.close(fd)
     return path
 
 
-@tracer.start_as_current_span(name="load_model_from_BytesIO")
 def load_model_from_BytesIO(model_bytesio, helper):
-    """ Load a model from a BytesIO object.
+    """Load a model from a BytesIO object.
     :param model_bytesio: A BytesIO object containing the model.
     :type model_bytesio: :class:`io.BytesIO`
     :param helper: The helper object for the model.
     :type helper: :class:`fedn.utils.helperbase.HelperBase`
     :return: The model object.
     :rtype: return type of helper.load
     """
     path = get_tmp_path()
-    with open(path, 'wb') as fh:
+    with open(path, "wb") as fh:
         fh.write(model_bytesio)
         fh.flush()
     model = helper.load(path)
     os.unlink(path)
     return model
 
 
-@tracer.start_as_current_span(name="serialize_model_to_BytesIO")
 def serialize_model_to_BytesIO(model, helper):
-    """ Serialize a model to a BytesIO object.
+    """Serialize a model to a BytesIO object.
 
     :param model: The model object.
     :type model: return type of helper.load
     :param helper: The helper object for the model.
     :type helper: :class:`fedn.utils.helperbase.HelperBase`
     :return: A BytesIO object containing the model.
     :rtype: :class:`io.BytesIO`
     """
     outfile_name = helper.save(model)
 
     a = BytesIO()
     a.seek(0, 0)
-    with open(outfile_name, 'rb') as f:
+    with open(outfile_name, "rb") as f:
         a.write(f.read())
     a.seek(0)
     os.unlink(outfile_name)
     return a
 
 
-@trace_all_methods
 class ModelService(rpc.ModelServiceServicer):
-    """ Service for handling download and upload of models to the server.
-
-    """
+    """Service for handling download and upload of models to the server."""
 
     def __init__(self):
         self.temp_model_storage = TempModelStorage()
 
     def exist(self, model_id):
-        """ Check if a model exists on the server.
+        """Check if a model exists on the server.
 
         :param model_id: The model id.
         :return: True if the model exists, else False.
         """
         return self.temp_model_storage.exist(model_id)
 
     def get_model(self, id):
-        """ Download model with id 'id' from server.
+        """Download model with id 'id' from server.
 
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
 
             if part.status == fedn.ModelStatus.OK:
                 return data
             if part.status == fedn.ModelStatus.FAILED:
                 return None
 
     def set_model(self, model, id):
-        """ Upload model to server.
+        """Upload model to server.
 
         :param model: A model object (BytesIO)
         :type model: :class:`io.BytesIO`
         :param id: The model id.
         :type id: str
         """
         bt = model_as_bytesIO(model)
         # TODO: Check result
         _ = self.Upload(upload_request_generator(bt, id), self)
 
     # Model Service
     def Upload(self, request_iterator, context):
-        """ RPC endpoints for uploading a model.
+        """RPC endpoints for uploading a model.
 
         :param request_iterator: The model request iterator.
         :type request_iterator: :class:`fedn.network.grpc.fedn_pb2.ModelRequest`
         :param context: The context object (unused)
         :type context: :class:`grpc._server._Context`
         :return: A model response object.
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ModelResponse`
@@ -164,46 +152,45 @@
         result = None
         for request in request_iterator:
             if request.status == fedn.ModelStatus.IN_PROGRESS:
                 self.temp_model_storage.get_ptr(request.id).write(request.data)
                 self.temp_model_storage.set_model_metadata(request.id, fedn.ModelStatus.IN_PROGRESS)
 
             if request.status == fedn.ModelStatus.OK and not request.data:
-                result = fedn.ModelResponse(id=request.id, status=fedn.ModelStatus.OK,
-                                            message="Got model successfully.")
+                result = fedn.ModelResponse(id=request.id, status=fedn.ModelStatus.OK, message="Got model successfully.")
                 # self.temp_model_storage_metadata.update({request.id: fedn.ModelStatus.OK})
                 self.temp_model_storage.set_model_metadata(request.id, fedn.ModelStatus.OK)
                 self.temp_model_storage.get_ptr(request.id).flush()
                 self.temp_model_storage.get_ptr(request.id).close()
                 return result
 
     def Download(self, request, context):
-        """ RPC endpoints for downloading a model.
+        """RPC endpoints for downloading a model.
 
         :param request: The model request object.
         :type request: :class:`fedn.network.grpc.fedn_pb2.ModelRequest`
         :param context: The context object (unused)
         :type context: :class:`grpc._server._Context`
         :return: A model response iterator.
         :rtype: :class:`fedn.network.grpc.fedn_pb2.ModelResponse`
         """
-        logger.info(f'grpc.ModelService.Download: {request.sender.role}:{request.sender.name} requested model {request.id}')
+        logger.info(f"grpc.ModelService.Download: {request.sender.role}:{request.sender.name} requested model {request.id}")
         try:
             status = self.temp_model_storage.get_model_metadata(request.id)
             if status != fedn.ModelStatus.OK:
-                logger.error(f'model file is not ready: {request.id}, status: {status}')
+                logger.error(f"model file is not ready: {request.id}, status: {status}")
                 yield fedn.ModelResponse(id=request.id, data=None, status=status)
         except Exception:
             logger.error("Error file does not exist: {}".format(request.id))
             yield fedn.ModelResponse(id=request.id, data=None, status=fedn.ModelStatus.FAILED)
 
         try:
             obj = self.temp_model_storage.get(request.id)
             if obj is None:
-                raise Exception(f'File not found: {request.id}')
+                raise Exception(f"File not found: {request.id}")
             with obj as f:
                 while True:
                     piece = f.read(CHUNK_SIZE)
                     if len(piece) == 0:
                         yield fedn.ModelResponse(id=request.id, data=None, status=fedn.ModelStatus.OK)
                         return
                     yield fedn.ModelResponse(id=request.id, data=piece, status=fedn.ModelStatus.IN_PROGRESS)
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/combiner/roundhandler.py` & `fedn-0.9.5/fedn/network/combiner/roundhandler.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,27 @@
+import ast
 import queue
 import random
 import sys
 import time
 import uuid
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.combiner.aggregators.aggregatorbase import get_aggregator
-from fedn.network.combiner.modelservice import (load_model_from_BytesIO,
-                                                serialize_model_to_BytesIO)
+from fedn.network.combiner.modelservice import load_model_from_BytesIO, serialize_model_to_BytesIO
 from fedn.utils.helpers.helpers import get_helper
+from fedn.utils.parameters import Parameters
 
 
 class ModelUpdateError(Exception):
     pass
 
 
-@trace_all_methods
 class RoundHandler:
-    """ Round handler.
+    """Round handler.
 
     The round handler processes requests from the global controller
     to produce model updates and perform model validations.
 
     :param aggregator_name: The name of the aggregator plugin module.
     :type aggregator_name: str
     :param storage: Model repository for :class: `fedn.network.combiner.Combiner`
@@ -30,16 +29,15 @@
     :param server: A handle to the Combiner class :class: `fedn.network.combiner.Combiner`
     :type server: class: `fedn.network.combiner.Combiner`
     :param modelservice: A handle to the model service :class: `fedn.network.combiner.modelservice.ModelService`
     :type modelservice: class: `fedn.network.combiner.modelservice.ModelService`
     """
 
     def __init__(self, storage, server, modelservice):
-        """ Initialize the RoundHandler."""
-
+        """Initialize the RoundHandler."""
         self.round_configs = queue.Queue()
         self.storage = storage
         self.server = server
         self.modelservice = modelservice
 
     def set_aggregator(self, aggregator):
         self.aggregator = get_aggregator(aggregator, self.storage, self.server, self.modelservice, self)
@@ -49,37 +47,35 @@
 
         :param round_config: A dict containing the round configuration (from global controller).
         :type round_config: dict
         :return: A job id (universally unique identifier) for the round.
         :rtype: str
         """
         try:
-            round_config['_job_id'] = str(uuid.uuid4())
+            round_config["_job_id"] = str(uuid.uuid4())
             self.round_configs.put(round_config)
         except Exception:
             logger.error("Failed to push round config.")
             raise
-        return round_config['_job_id']
+        return round_config["_job_id"]
 
     def load_model_update(self, helper, model_id):
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
-                logger.warning(
-                    "AGGREGATOR({}): Failed to load model!".format(self.name))
+                logger.warning("AGGREGATOR({}): Failed to load model!".format(self.name))
         else:
             raise ModelUpdateError("Failed to load model.")
 
         return model
 
     def load_model_update_str(self, model_id, retry=3):
         """Load model update object and return it as BytesIO.
@@ -104,29 +100,28 @@
                     logger.warning("Model download failed. retrying")
                     time.sleep(1)
                     model_str = self.modelservice.get_model(model_id)
 
         return model_str
 
     def waitforit(self, config, buffer_size=100, polling_interval=0.1):
-        """ Defines the policy for how long the server should wait before starting to aggregate models.
+        """Defines the policy for how long the server should wait before starting to aggregate models.
 
         The policy is as follows:
             1. Wait a maximum of time_window time until the round times out.
             2. Terminate if a preset number of model updates (buffer_size) are in the queue.
 
         :param config: The round config object
         :type config: dict
         :param buffer_size: The number of model updates to wait for before starting aggregation, defaults to 100
         :type buffer_size: int, optional
         :param polling_interval: The polling interval, defaults to 0.1
         :type polling_interval: float, optional
         """
-
-        time_window = float(config['round_timeout'])
+        time_window = float(config["round_timeout"])
 
         tt = 0.0
         while tt < time_window:
             if self.aggregator.model_updates.qsize() >= buffer_size:
                 break
 
             time.sleep(polling_interval)
@@ -138,53 +133,57 @@
         :param config: The round config object (passed to the client).
         :type config: dict
         :param clients: clients to participate in the training round
         :type clients: list
         :return: an aggregated model and associated metadata
         :rtype: model, dict
         """
-
-        logger.info(
-            "ROUNDHANDLER: Initiating training round, participating clients: {}".format(clients))
+        logger.info("ROUNDHANDLER: Initiating training round, participating clients: {}".format(clients))
 
         meta = {}
-        meta['nr_expected_updates'] = len(clients)
-        meta['nr_required_updates'] = int(config['clients_required'])
-        meta['timeout'] = float(config['round_timeout'])
+        meta["nr_expected_updates"] = len(clients)
+        meta["nr_required_updates"] = int(config["clients_required"])
+        meta["timeout"] = float(config["round_timeout"])
 
         # Request model updates from all active clients.
         self.server.request_model_update(config, clients=clients)
 
         # If buffer_size is -1 (default), the round terminates when/if all clients have completed.
-        if int(config['buffer_size']) == -1:
+        if int(config["buffer_size"]) == -1:
             buffer_size = len(clients)
         else:
-            buffer_size = int(config['buffer_size'])
+            buffer_size = int(config["buffer_size"])
 
         # Wait / block until the round termination policy has been met.
         self.waitforit(config, buffer_size=buffer_size)
 
         tic = time.time()
         model = None
         data = None
 
         try:
-            helper = get_helper(config['helper_type'])
-            logger.info("Config delete_models_storage: {}".format(config['delete_models_storage']))
-            if config['delete_models_storage'] == 'True':
+            helper = get_helper(config["helper_type"])
+            logger.info("Config delete_models_storage: {}".format(config["delete_models_storage"]))
+            if config["delete_models_storage"] == "True":
                 delete_models = True
             else:
                 delete_models = False
-            model, data = self.aggregator.combine_models(helper=helper,
-                                                         delete_models=delete_models)
+
+            if "aggregator_kwargs" in config.keys():
+                dict_parameters = ast.literal_eval(config["aggregator_kwargs"])
+                parameters = Parameters(dict_parameters)
+            else:
+                parameters = None
+
+            model, data = self.aggregator.combine_models(helper=helper, delete_models=delete_models, parameters=parameters)
         except Exception as e:
             logger.warning("AGGREGATION FAILED AT COMBINER! {}".format(e))
 
-        meta['time_combination'] = time.time() - tic
-        meta['aggregation_time'] = data
+        meta["time_combination"] = time.time() - tic
+        meta["aggregation_time"] = data
         return model, meta
 
     def _validation_round(self, config, clients, model_id):
         """Send model validation requests to clients.
 
         :param config: The round config object (passed to the client).
         :type config: dict
@@ -201,15 +200,14 @@
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
@@ -225,24 +223,23 @@
                 if tries > retry:
                     logger.error("Failed to stage model {} from storage backend!".format(model_id))
                     raise
 
         self.modelservice.set_model(model, model_id)
 
     def _assign_round_clients(self, n, type="trainers"):
-        """ Obtain a list of clients(trainers or validators) to ask for updates in this round.
+        """Obtain a list of clients(trainers or validators) to ask for updates in this round.
 
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
@@ -262,111 +259,103 @@
         :param config: The round config object.
         :type config: dict
         :param timeout: Timeout in seconds, defaults to 0.0
         :type timeout: float, optional
         :return: True if the required number of clients are available, False otherwise.
         :rtype: bool
         """
-
         active = self.server.nr_active_trainers()
-        if active >= int(config['clients_required']):
-            logger.info("Number of clients required ({0}) to start round met {1}.".format(
-                config['clients_required'], active))
+        if active >= int(config["clients_required"]):
+            logger.info("Number of clients required ({0}) to start round met {1}.".format(config["clients_required"], active))
             return True
         else:
             logger.info("Too few clients to start round.")
             return False
 
     def execute_validation_round(self, round_config):
-        """ Coordinate validation rounds as specified in config.
+        """Coordinate validation rounds as specified in config.
 
         :param round_config: The round config object.
         :type round_config: dict
         """
-        model_id = round_config['model_id']
-        logger.info(
-            "COMBINER orchestrating validation of model {}".format(model_id))
+        model_id = round_config["model_id"]
+        logger.info("COMBINER orchestrating validation of model {}".format(model_id))
         self.stage_model(model_id)
-        validators = self._assign_round_clients(
-            self.server.max_clients, type="validators")
+        validators = self._assign_round_clients(self.server.max_clients, type="validators")
         self._validation_round(round_config, validators, model_id)
 
     def execute_training_round(self, config):
-        """ Coordinates clients to execute training tasks.
+        """Coordinates clients to execute training tasks.
 
         :param config: The round config object.
         :type config: dict
         :return: metadata about the training round.
         :rtype: dict
         """
-
-        logger.info("Processing training round,  job_id {}".format(config['_job_id']))
+        logger.info("Processing training round,  job_id {}".format(config["_job_id"]))
 
         data = {}
-        data['config'] = config
-        data['round_id'] = config['round_id']
+        data["config"] = config
+        data["round_id"] = config["round_id"]
 
         # Download model to update and set in temp storage.
-        self.stage_model(config['model_id'])
+        self.stage_model(config["model_id"])
 
         clients = self._assign_round_clients(self.server.max_clients)
         model, meta = self._training_round(config, clients)
-        data['data'] = meta
+        data["data"] = meta
 
         if model is None:
-            logger.warning(
-                "\t Failed to update global model in round {0}!".format(config['round_id']))
+            logger.warning("\t Failed to update global model in round {0}!".format(config["round_id"]))
 
         if model is not None:
-            helper = get_helper(config['helper_type'])
+            helper = get_helper(config["helper_type"])
             a = serialize_model_to_BytesIO(model, helper)
             model_id = self.storage.set_model(a.read(), is_file=False)
             a.close()
-            data['model_id'] = model_id
+            data["model_id"] = model_id
 
-            logger.info(
-                "TRAINING ROUND COMPLETED. Aggregated model id: {}, Job id: {}".format(model_id, config['_job_id']))
+            logger.info("TRAINING ROUND COMPLETED. Aggregated model id: {}, Job id: {}".format(model_id, config["_job_id"]))
 
         # Delete temp model
-        self.modelservice.temp_model_storage.delete(config['model_id'])
+        self.modelservice.temp_model_storage.delete(config["model_id"])
         return data
 
     def run(self, polling_interval=1.0):
-        """ Main control loop. Execute rounds based on round config on the queue.
+        """Main control loop. Execute rounds based on round config on the queue.
 
         :param polling_interval: The polling interval in seconds for checking if a new job/config is available.
         :type polling_interval: float
         """
         try:
             while True:
                 try:
                     round_config = self.round_configs.get(block=False)
 
                     # Check that the minimum allowed number of clients are connected
                     ready = self._check_nr_round_clients(round_config)
                     round_meta = {}
 
                     if ready:
-                        if round_config['task'] == 'training':
+                        if round_config["task"] == "training":
                             tic = time.time()
                             round_meta = self.execute_training_round(round_config)
-                            round_meta['time_exec_training'] = time.time() - \
-                                tic
-                            round_meta['status'] = "Success"
-                            round_meta['name'] = self.server.id
+                            round_meta["time_exec_training"] = time.time() - tic
+                            round_meta["status"] = "Success"
+                            round_meta["name"] = self.server.id
                             self.server.statestore.set_round_combiner_data(round_meta)
-                        elif round_config['task'] == 'validation' or round_config['task'] == 'inference':
+                        elif round_config["task"] == "validation" or round_config["task"] == "inference":
                             self.execute_validation_round(round_config)
                         else:
                             logger.warning("config contains unkown task type.")
                     else:
                         round_meta = {}
-                        round_meta['status'] = "Failed"
-                        round_meta['reason'] = "Failed to meet client allocation requirements for this round config."
-                        logger.warning("{0}".format(round_meta['reason']))
+                        round_meta["status"] = "Failed"
+                        round_meta["reason"] = "Failed to meet client allocation requirements for this round config."
+                        logger.warning("{0}".format(round_meta["reason"]))
 
                     self.round_configs.task_done()
                 except queue.Empty:
                     time.sleep(polling_interval)
 
         except (KeyboardInterrupt, SystemExit):
             pass
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/controller/control.py` & `fedn-0.9.5/fedn/network/controller/control.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,15 @@
 import copy
 import datetime
 import time
 import uuid
 
-from tenacity import (retry, retry_if_exception_type, stop_after_delay,
-                      wait_random)
+from tenacity import retry, retry_if_exception_type, stop_after_delay, wait_random
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.combiner.interfaces import CombinerUnavailableError
 from fedn.network.combiner.modelservice import load_model_from_BytesIO
 from fedn.network.controller.controlbase import ControlBase
 from fedn.network.state import ReducerState
 
 
 class UnsupportedStorageBackend(Exception):
@@ -51,51 +49,102 @@
     def __init__(self, message):
         """Constructor method."""
         self.message = message
         super().__init__(self.message)
 
 
 class CombinersNotDoneException(Exception):
-    """ Exception class for when model is None """
+    """Exception class for when model is None"""
 
     def __init__(self, message):
-        """ Constructor method.
+        """Constructor method.
 
         :param message: The exception message.
         :type message: str
 
         """
         self.message = message
         super().__init__(self.message)
 
 
-@trace_all_methods
 class Control(ControlBase):
     """Controller, implementing the overall global training, validation and inference logic.
 
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
@@ -106,17 +155,17 @@
         self.create_session(config)
 
         self._state = ReducerState.monitoring
 
         last_round = int(self.get_latest_round_id())
 
         for combiner in self.network.get_combiners():
-            combiner.set_aggregator(config['aggregator'])
+            combiner.set_aggregator(config["aggregator"])
 
-        self.set_session_status(config['session_id'], 'Started')
+        self.set_session_status(config["session_id"], "Started")
         # Execute the rounds in this session
         for round in range(1, int(config["rounds"] + 1)):
             # Increment the round number
             if last_round:
                 current_round = last_round + round
             else:
                 current_round = round
@@ -127,32 +176,31 @@
                 logger.error("Failed to execute round: {0}".format(e))
 
             logger.info("Round completed with status {}".format(round_data["status"]))
 
             config["model_id"] = self.statestore.get_latest_model()
 
         # TODO: Report completion of session
-        self.set_session_status(config['session_id'], 'Finished')
+        self.set_session_status(config["session_id"], "Finished")
         self._state = ReducerState.idle
 
     def round(self, session_config, round_id):
-        """ Execute one global round.
+        """Execute one global round.
 
         : param session_config: The session config.
         : type session_config: dict
         : param round_id: The round id.
         : type round_id: str
 
         """
-
-        self.create_round({'round_id': round_id, 'status': "Pending"})
+        self.create_round({"round_id": round_id, "status": "Pending"})
 
         if len(self.network.get_combiners()) < 1:
             logger.warning("Round cannot start, no combiners connected!")
-            self.set_round_status(round_id, 'Failed')
+            self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
         # Assemble round config for this global round
         round_config = copy.deepcopy(session_config)
         round_config["rounds"] = 1
         round_config["round_id"] = round_id
         round_config["task"] = "training"
@@ -163,150 +211,143 @@
         # Get combiners that are able to participate in the round, given round_config
         participating_combiners = self.get_participating_combiners(round_config)
 
         # Check if the policy to start the round is met
         round_start = self.evaluate_round_start_policy(participating_combiners)
 
         if round_start:
-            logger.info("round start policy met, {} participating combiners.".format(
-                len(participating_combiners)))
+            logger.info("round start policy met, {} participating combiners.".format(len(participating_combiners)))
         else:
             logger.warning("Round start policy not met, skipping round!")
-            self.set_round_status(round_id, 'Failed')
+            self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
         # Ask participating combiners to coordinate model updates
         _ = self.request_model_updates(participating_combiners)
         # TODO: Check response
 
         # Wait until participating combiners have produced an updated global model,
         # or round times out.
         def do_if_round_times_out(result):
             logger.warning("Round timed out!")
 
-        @ retry(wait=wait_random(min=1.0, max=2.0),
-                stop=stop_after_delay(session_config['round_timeout']),
-                retry_error_callback=do_if_round_times_out,
-                retry=retry_if_exception_type(CombinersNotDoneException))
+        @retry(
+            wait=wait_random(min=1.0, max=2.0),
+            stop=stop_after_delay(session_config["round_timeout"]),
+            retry_error_callback=do_if_round_times_out,
+            retry=retry_if_exception_type(CombinersNotDoneException),
+        )
         def combiners_done():
-
             round = self.statestore.get_round(round_id)
-            if 'combiners' not in round:
+            if "combiners" not in round:
                 logger.info("Waiting for combiners to update model...")
                 raise CombinersNotDoneException("Combiners have not yet reported.")
 
-            if len(round['combiners']) < len(participating_combiners):
+            if len(round["combiners"]) < len(participating_combiners):
                 logger.info("Waiting for combiners to update model...")
                 raise CombinersNotDoneException("All combiners have not yet reported.")
 
             return True
 
         combiners_done()
 
         # Due to the distributed nature of the computation, there might be a
         # delay before combiners have reported the round data to the db,
         # so we need some robustness here.
-        @ retry(wait=wait_random(min=0.1, max=1.0),
-                retry=retry_if_exception_type(KeyError))
+        @retry(wait=wait_random(min=0.1, max=1.0), retry=retry_if_exception_type(KeyError))
         def check_combiners_done_reporting():
             round = self.statestore.get_round(round_id)
-            combiners = round['combiners']
+            combiners = round["combiners"]
             return combiners
 
         _ = check_combiners_done_reporting()
 
         round = self.statestore.get_round(round_id)
         round_valid = self.evaluate_round_validity_policy(round)
         if not round_valid:
             logger.error("Round failed. Invalid - evaluate_round_validity_policy: False")
-            self.set_round_status(round_id, 'Failed')
+            self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
         logger.info("Reducing combiner level models...")
         # Reduce combiner models into a new global model
         round_data = {}
         try:
             round = self.statestore.get_round(round_id)
-            model, data = self.reduce(round['combiners'])
-            round_data['reduce'] = data
+            model, data = self.reduce(round["combiners"])
+            round_data["reduce"] = data
             logger.info("Done reducing models from combiners!")
         except Exception as e:
             logger.error("Failed to reduce models from combiners, reason: {}".format(e))
-            self.set_round_status(round_id, 'Failed')
+            self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
         # Commit the new global model to the model trail
         if model is not None:
             logger.info("Committing global model to model trail...")
             tic = time.time()
             model_id = uuid.uuid4()
-            session_id = (
-                session_config["session_id"]
-                if "session_id" in session_config
-                else None
-            )
+            session_id = session_config["session_id"] if "session_id" in session_config else None
             self.commit(model_id, model, session_id)
             round_data["time_commit"] = time.time() - tic
             logger.info("Done committing global model to model trail.")
         else:
             logger.error("Failed to commit model to global model trail.")
-            self.set_round_status(round_id, 'Failed')
+            self.set_round_status(round_id, "Failed")
             return None, self.statestore.get_round(round_id)
 
-        self.set_round_status(round_id, 'Success')
+        self.set_round_status(round_id, "Success")
 
         # 4. Trigger participating combiner nodes to execute a validation round for the current model
         validate = session_config["validate"]
         if validate:
             combiner_config = copy.deepcopy(session_config)
             combiner_config["round_id"] = round_id
             combiner_config["model_id"] = self.statestore.get_latest_model()
             combiner_config["task"] = "validation"
             combiner_config["helper_type"] = self.statestore.get_helper()
 
-            validating_combiners = self.get_participating_combiners(
-                combiner_config)
+            validating_combiners = self.get_participating_combiners(combiner_config)
 
             for combiner, combiner_config in validating_combiners:
                 try:
                     logger.info("Submitting validation round to combiner {}".format(combiner))
                     combiner.submit(combiner_config)
                 except CombinerUnavailableError:
                     self._handle_unavailable_combiner(combiner)
                     pass
 
         self.set_round_data(round_id, round_data)
-        self.set_round_status(round_id, 'Finished')
+        self.set_round_status(round_id, "Finished")
         return model_id, self.statestore.get_round(round_id)
 
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
 
         for combiner in combiners:
-            name = combiner['name']
-            model_id = combiner['model_id']
+            name = combiner["name"]
+            model_id = combiner["model_id"]
 
             logger.info("Fetching model ({}) from model repository".format(model_id))
 
             try:
                 tic = time.time()
                 data = self.model_repository.get_model(model_id)
-                meta['time_fetch_model'] += (time.time() - tic)
+                meta["time_fetch_model"] += time.time() - tic
             except Exception as e:
                 logger.error("Failed to fetch model from model repository {}: {}".format(name, e))
                 data = None
 
             if data is not None:
                 try:
                     tic = time.time()
@@ -327,15 +368,14 @@
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
@@ -355,15 +395,14 @@
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
@@ -371,16 +410,15 @@
         # Setup combiner configuration
         combiner_config = copy.deepcopy(config)
         combiner_config["model_id"] = self.statestore.get_latest_model()
         combiner_config["task"] = "inference"
         combiner_config["helper_type"] = self.statestore.get_framework()
 
         # Select combiners
-        validating_combiners = self.get_participating_combiners(
-            combiner_config)
+        validating_combiners = self.get_participating_combiners(combiner_config)
 
         # Test round start policy
         round_start = self.check_round_start_policy(validating_combiners)
         if round_start:
             logger.info("Round start policy met, participating combiners {}".format(validating_combiners))
         else:
             logger.warning("Round start policy not met, skipping round!")
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/controller/controlbase.py` & `fedn-0.9.5/fedn/network/controller/controlbase.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import os
 import uuid
 from abc import ABC, abstractmethod
 from time import sleep
 
 import fedn.utils.helpers.helpers
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.api.network import Network
 from fedn.network.combiner.interfaces import CombinerUnavailableError
 from fedn.network.state import ReducerState
 from fedn.network.storage.s3.repository import Repository
 
 # Maximum number of tries to connect to statestore and retrieve storage configuration
 MAX_TRIES_BACKEND = os.getenv("MAX_TRIES_BACKEND", 10)
@@ -23,15 +22,14 @@
     pass
 
 
 class MisconfiguredHelper(Exception):
     pass
 
 
-@trace_all_methods
 class ControlBase(ABC):
     """Base class and interface for a global controller.
         Override this class to implement a global training strategy (control).
 
     :param statestore: The statestore object.
     :type statestore: :class:`fedn.network.statestore.statestorebase.StateStoreBase`
     """
@@ -59,17 +57,15 @@
                     if tries > MAX_TRIES_BACKEND:
                         raise Exception
         except Exception:
             logger.error("Failed to retrive storage configuration, exiting.")
             raise MisconfiguredStorageBackend()
 
         if storage_config["storage_type"] == "S3":
-            self.model_repository = Repository(
-                storage_config["storage_config"]
-            )
+            self.model_repository = Repository(storage_config["storage_config"])
         else:
             logger.error("Unsupported storage backend, exiting.")
             raise UnsupportedStorageBackend()
 
         if self.statestore.is_inited():
             self._state = ReducerState.idle
 
@@ -90,19 +86,15 @@
 
         :return: Helper instance.
         :rtype: :class:`fedn.utils.plugins.helperbase.HelperBase`
         """
         helper_type = self.statestore.get_helper()
         helper = fedn.utils.helpers.helpers.get_helper(helper_type)
         if not helper:
-            raise MisconfiguredHelper(
-                "Unsupported helper type {}, please configure compute_package.helper !".format(
-                    helper_type
-                )
-            )
+            raise MisconfiguredHelper("Unsupported helper type {}, please configure compute_package.helper !".format(helper_type))
         return helper
 
     def get_state(self):
         """Get the current state of the controller.
 
         :return: The current state.
         :rtype: :class:`fedn.network.state.ReducerState`
@@ -117,25 +109,21 @@
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
@@ -143,17 +131,15 @@
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
@@ -163,76 +149,72 @@
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
 
-    def create_session(self, config, status='Initialized'):
-        """ Initialize a new session in backend db. """
-
+    def create_session(self, config, status="Initialized"):
+        """Initialize a new session in backend db."""
         if "session_id" not in config.keys():
             session_id = uuid.uuid4()
             config["session_id"] = str(session_id)
         else:
             session_id = config["session_id"]
 
         self.statestore.create_session(id=session_id)
         self.statestore.set_session_config(session_id, config)
         self.statestore.set_session_status(session_id, status)
 
     def set_session_status(self, session_id, status):
-        """ Set the round round stats.
+        """Set the round round stats.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param status: The status
         :type status: str
         """
         self.statestore.set_session_status(session_id, status)
 
     def create_round(self, round_data):
-        """Initialize a new round in backend db. """
-
+        """Initialize a new round in backend db."""
         self.statestore.create_round(round_data)
 
     def set_round_data(self, round_id, round_data):
-        """ Set round data.
+        """Set round data.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_data: The status
         :type status: dict
         """
         self.statestore.set_round_data(round_id, round_data)
 
     def set_round_status(self, round_id, status):
-        """ Set the round round stats.
+        """Set the round round stats.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param status: The status
         :type status: str
         """
         self.statestore.set_round_status(round_id, status)
 
     def set_round_config(self, round_id, round_config):
-        """ Upate round in backend db.
+        """Upate round in backend db.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_config: The round configuration
         :type round_config: dict
         """
         self.statestore.set_round_config(round_id, round_config)
@@ -255,23 +237,20 @@
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
-            model_id = self.model_repository.set_model(
-                outfile_name, is_file=True
-            )
+            model_id = self.model_repository.set_model(outfile_name, is_file=True)
 
             logger.info("CONTROL: Deleting temporary model file...")
             os.unlink(outfile_name)
 
         logger.info("Committing model {} to global model trail in statestore...".format(model_id))
         self.statestore.set_latest_model(model_id, session_id)
 
@@ -290,24 +269,20 @@
             try:
                 # Current gRPC endpoint only returns active clients (both trainers and validators)
                 nr_active_clients = len(combiner.list_active_clients())
             except CombinerUnavailableError:
                 self._handle_unavailable_combiner(combiner)
                 continue
 
-            is_participating = self.evaluate_round_participation_policy(
-                combiner_round_config, nr_active_clients
-            )
+            is_participating = self.evaluate_round_participation_policy(combiner_round_config, nr_active_clients)
             if is_participating:
                 combiners.append((combiner, combiner_round_config))
         return combiners
 
-    def evaluate_round_participation_policy(
-        self, compute_plan, nr_active_clients
-    ):
+    def evaluate_round_participation_policy(self, compute_plan, nr_active_clients):
         """Evaluate policy for combiner round-participation.
         A combiner participates if it is responsive and reports enough
         active clients to participate in the round.
         """
         if int(compute_plan["clients_required"]) <= nr_active_clients:
             return True
         else:
@@ -323,38 +298,38 @@
         """
         if len(combiners) > 0:
             return True
         else:
             return False
 
     def evaluate_round_validity_policy(self, round):
-        """ Check if the round is valid.
+        """Check if the round is valid.
 
         At the end of the round, before committing a model to the global model trail,
         we check if the round validity policy has been met. This can involve
         e.g. asserting that a certain number of combiners have reported in an
         updated model, or that criteria on model performance have been met.
 
         :param round: The round object
         :rtype round: dict
         :return: True if the policy is met, otherwise False
         :rtype: bool
         """
         model_ids = []
-        for combiner in round['combiners']:
+        for combiner in round["combiners"]:
             try:
-                model_ids.append(combiner['model_id'])
+                model_ids.append(combiner["model_id"])
             except KeyError:
                 pass
 
         if len(model_ids) == 0:
             return False
 
         return True
 
     def state(self):
-        """ Get the current state of the controller.
+        """Get the current state of the controller.
 
         :return: The state
         :rype: str
         """
         return self._state
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/grpc/auth.py` & `fedn-0.9.5/fedn/network/grpc/auth.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,43 +2,41 @@
 import jwt
 
 from fedn.common.config import FEDN_AUTH_SCHEME, FEDN_JWT_ALGORITHM, SECRET_KEY
 from fedn.common.log_config import logger
 from fedn.network.api.auth import check_custom_claims
 
 ENDPOINT_ROLES_MAPPING = {
-    '/fedn.Combiner/TaskStream': ['client'],
-    '/fedn.Combiner/SendModelUpdate': ['client'],
-    '/fedn.Combiner/SendModelValidation': ['client'],
-    '/fedn.Connector/SendHeartbeat': ['client'],
-    '/fedn.Connector/SendStatus': ['client'],
-    '/fedn.ModelService/Download': ['client'],
-    '/fedn.ModelService/Upload': ['client'],
-    '/fedn.Control/Start': ['controller'],
-    '/fedn.Control/Stop': ['controller'],
-    '/fedn.Control/FlushAggregationQueue': ['controller'],
-    '/fedn.Control/SetAggregator': ['controller'],
+    "/fedn.Combiner/TaskStream": ["client"],
+    "/fedn.Combiner/SendModelUpdate": ["client"],
+    "/fedn.Combiner/SendModelValidation": ["client"],
+    "/fedn.Connector/SendHeartbeat": ["client"],
+    "/fedn.Connector/SendStatus": ["client"],
+    "/fedn.ModelService/Download": ["client"],
+    "/fedn.ModelService/Upload": ["client"],
+    "/fedn.Control/Start": ["controller"],
+    "/fedn.Control/Stop": ["controller"],
+    "/fedn.Control/FlushAggregationQueue": ["controller"],
+    "/fedn.Control/SetAggregator": ["controller"],
 }
 
 ENDPOINT_WHITELIST = [
-    '/fedn.Connector/AcceptingClients',
-    '/fedn.Connector/ListActiveClients',
-    '/fedn.Control/Start',
-    '/fedn.Control/Stop',
-    '/fedn.Control/FlushAggregationQueue',
-    '/fedn.Control/SetAggregator',
+    "/fedn.Connector/AcceptingClients",
+    "/fedn.Connector/ListActiveClients",
+    "/fedn.Control/Start",
+    "/fedn.Control/Stop",
+    "/fedn.Control/FlushAggregationQueue",
+    "/fedn.Control/SetAggregator",
 ]
 
-USER_AGENT_WHITELIST = [
-    'grpc_health_probe'
-]
+USER_AGENT_WHITELIST = ["grpc_health_probe"]
 
 
 def check_role_claims(payload, endpoint):
-    user_role = payload.get('role', '')
+    user_role = payload.get("role", "")
 
     # Perform endpoint-specific RBAC check
     allowed_roles = ENDPOINT_ROLES_MAPPING.get(endpoint)
     if allowed_roles and user_role not in allowed_roles:
         return False
     return True
 
@@ -59,37 +57,37 @@
         if not SECRET_KEY:
             return continuation(handler_call_details)
         metadata = dict(handler_call_details.invocation_metadata)
         # Pass whitelisted methods
         if handler_call_details.method in ENDPOINT_WHITELIST:
             return continuation(handler_call_details)
         # Pass if the request comes from whitelisted user agents
-        user_agent = metadata.get('user-agent').split(' ')[0]
+        user_agent = metadata.get("user-agent").split(" ")[0]
         if user_agent in USER_AGENT_WHITELIST:
             return continuation(handler_call_details)
 
-        token = metadata.get('authorization')
+        token = metadata.get("authorization")
         if token is None:
-            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, 'Token is missing')
+            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, "Token is missing")
 
         if not token.startswith(FEDN_AUTH_SCHEME):
-            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, f'Invalid token scheme, expected {FEDN_AUTH_SCHEME}')
+            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, f"Invalid token scheme, expected {FEDN_AUTH_SCHEME}")
 
-        token = token.split(' ')[1]
+        token = token.split(" ")[1]
 
         try:
             payload = jwt.decode(token, SECRET_KEY, algorithms=[FEDN_JWT_ALGORITHM])
 
             if not check_role_claims(payload, handler_call_details.method):
-                return _unary_unary_rpc_terminator(grpc.StatusCode.PERMISSION_DENIED, 'Insufficient permissions')
+                return _unary_unary_rpc_terminator(grpc.StatusCode.PERMISSION_DENIED, "Insufficient permissions")
 
             if not check_custom_claims(payload):
-                return _unary_unary_rpc_terminator(grpc.StatusCode.PERMISSION_DENIED, 'Insufficient permissions')
+                return _unary_unary_rpc_terminator(grpc.StatusCode.PERMISSION_DENIED, "Insufficient permissions")
 
             return continuation(handler_call_details)
         except jwt.InvalidTokenError:
-            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, 'Invalid token')
+            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, "Invalid token")
         except jwt.ExpiredSignatureError:
-            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, 'Token expired')
+            return _unary_unary_rpc_terminator(grpc.StatusCode.UNAUTHENTICATED, "Token expired")
         except Exception as e:
             logger.error(str(e))
             return _unary_unary_rpc_terminator(grpc.StatusCode.UNKNOWN, str(e))
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/grpc/fedn_pb2.py` & `fedn-0.9.5/fedn/network/grpc/fedn_pb2.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/grpc/fedn_pb2_grpc.py` & `fedn-0.9.5/fedn/network/grpc/fedn_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/grpc/server.py` & `fedn-0.9.5/fedn/network/grpc/server.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/loadbalancer/leastpacked.py` & `fedn-0.9.5/fedn/network/loadbalancer/leastpacked.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,33 @@
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.combiner.interfaces import CombinerUnavailableError
 from fedn.network.loadbalancer.loadbalancerbase import LoadBalancerBase
 
 
-@trace_all_methods
 class LeastPacked(LoadBalancerBase):
-    """ Load balancer that selects the combiner with the least number of attached training clients.
+    """Load balancer that selects the combiner with the least number of attached training clients.
 
     :param network: A handle to the network.
     :type network: class: `fedn.network.api.network.Network`
     """
 
     def __init__(self, network):
         super().__init__(network)
 
     def find_combiner(self):
-        """
-            Find the combiner with the least number of attached clients.
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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/state.py` & `fedn-0.9.5/fedn/network/state.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 from enum import Enum
 
-from fedn.common.telemetry import tracer
-
 
 class ReducerState(Enum):
-    """ Enum for representing the state of a reducer."""
+    """Enum for representing the state of a reducer."""
+
     setup = 1
     idle = 2
     instructing = 3
     monitoring = 4
 
 
-@tracer.start_as_current_span(name="ReducerStateToString")
 def ReducerStateToString(state):
-    """ Convert ReducerState to string.
+    """Convert ReducerState to string.
 
     :param state: The state.
     :type state: :class:`fedn.network.state.ReducerState`
     :return: The state as string.
     :rtype: str
     """
     if state == ReducerState.setup:
@@ -28,17 +26,16 @@
         return "instructing"
     if state == ReducerState.monitoring:
         return "monitoring"
 
     return "UNKNOWN"
 
 
-@tracer.start_as_current_span(name="StringToReducerState")
 def StringToReducerState(state):
-    """ Convert string to ReducerState.
+    """Convert string to ReducerState.
 
     :param state: The state as string.
     :type state: str
     :return: The state.
     :rtype: :class:`fedn.network.state.ReducerState`
     """
     if state == "setup":
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/memorymodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/memorymodelstorage.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,52 +1,43 @@
 import io
 from collections import defaultdict
 from io import BytesIO
 
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.storage.models.modelstorage import ModelStorage
 
 CHUNK_SIZE = 1024 * 1024
 
 
-@trace_all_methods
 class MemoryModelStorage(ModelStorage):
-    """ Class for in-memory storage of model artifacts.
+    """Class for in-memory storage of model artifacts.
 
     Models are stored as BytesIO objects in a dictionary.
 
     """
 
     def __init__(self):
-
         self.models = defaultdict(io.BytesIO)
         self.models_metadata = {}
 
     def exist(self, model_id):
-
         if model_id in self.models.keys():
             return True
         return False
 
     def get(self, model_id):
-
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
-
         return self.models_metadata[model_id]
 
     def set_model_metadata(self, model_id, model_metadata):
-
         self.models_metadata.update({model_id: model_metadata})
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/modelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/modelstorage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,69 @@
 from abc import ABC, abstractmethod
 
-from fedn.common.telemetry import trace_all_methods
 
-
-@trace_all_methods
 class ModelStorage(ABC):
-
     @abstractmethod
     def exist(self, model_id):
-        """ Check if model exists in storage
+        """Check if model exists in storage
 
         :param model_id: The model id
         :type model_id: str
         :return: True if model exists, False otherwise
         :rtype: bool
         """
         pass
 
     @abstractmethod
     def get(self, model_id):
-        """ Get model from storage
+        """Get model from storage
 
         :param model_id: The model id
         :type model_id: str
         :return: The model
         :rtype: object
         """
         pass
 
     @abstractmethod
     def get_model_metadata(self, model_id):
-        """ Get model metadata from storage
+        """Get model metadata from storage
 
         :param model_id: The model id
         :type model_id: str
         :return: The model metadata
         :rtype: dict
         """
         pass
 
     @abstractmethod
     def set_model_metadata(self, model_id, model_metadata):
-        """ Set model metadata in storage
+        """Set model metadata in storage
 
         :param model_id: The model id
         :type model_id: str
         :param model_metadata: The model metadata
         :type model_metadata: dict
         :return: True if successful, False otherwise
         :rtype: bool
         """
         pass
 
     @abstractmethod
     def delete(self, model_id):
-        """ Delete model from storage
+        """Delete model from storage
 
         :param model_id: The model id
         :type model_id: str
         :return: True if successful, False otherwise
         :rtype: bool
         """
         pass
 
     @abstractmethod
     def delete_all(self):
-        """ Delete all models from storage
+        """Delete all models from storage
 
         :return: True if successful, False otherwise
         :rtype: bool
         """
         pass
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/models/tempmodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/tempmodelstorage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,98 +1,86 @@
 import os
 from io import BytesIO
 
 import fedn.network.grpc.fedn_pb2 as fedn
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.storage.models.modelstorage import ModelStorage
 
 CHUNK_SIZE = 1024 * 1024
 
 
-@trace_all_methods
 class TempModelStorage(ModelStorage):
-    """ Class for managing local temporary models on file on combiners."""
+    """Class for managing local temporary models on file on combiners."""
 
     def __init__(self):
-
-        self.default_dir = os.environ.get(
-            'FEDN_MODEL_DIR', '/tmp/models')  # set default to tmp
+        self.default_dir = os.environ.get("FEDN_MODEL_DIR", "/tmp/models")  # set default to tmp
         if not os.path.exists(self.default_dir):
             os.makedirs(self.default_dir)
 
         self.models = {}
         self.models_metadata = {}
 
     def exist(self, model_id):
-
         if model_id in self.models.keys():
             return True
         return False
 
     def get(self, model_id):
-
         try:
             if self.models_metadata[model_id] != fedn.ModelStatus.OK:
                 logger.warning("File not ready! Try again")
                 return None
         except KeyError:
             logger.error("No such model has been made available yet!")
             return None
 
         obj = BytesIO()
-        with open(os.path.join(self.default_dir, str(model_id)), 'rb') as f:
+        with open(os.path.join(self.default_dir, str(model_id)), "rb") as f:
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
-            f = self.models[model_id]['file']
+            f = self.models[model_id]["file"]
         except KeyError:
             f = open(os.path.join(self.default_dir, str(model_id)), "wb")
 
-        self.models[model_id] = {'file': f}
-        return self.models[model_id]['file']
+        self.models[model_id] = {"file": f}
+        return self.models[model_id]["file"]
 
     def get_model_metadata(self, model_id):
-
         try:
             status = self.models_metadata[model_id]
         except KeyError:
             status = fedn.ModelStatus.UNKNOWN
         return status
 
     def set_model_metadata(self, model_id, model_metadata):
-
         self.models_metadata.update({model_id: model_metadata})
 
     # Delete model from disk
     def delete(self, model_id):
-
         try:
             os.remove(os.path.join(self.default_dir, str(model_id)))
             logger.info("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id))
             # Delete id from metadata and models dict
             del self.models_metadata[model_id]
             del self.models[model_id]
         except FileNotFoundError:
             logger.error("Could not delete model from disk. File not found!")
             return False
         return True
 
     # Delete all models from disk
     def delete_all(self):
-
         ids_pop = []
         for model_id in self.models.keys():
             try:
                 os.remove(os.path.join(self.default_dir, str(model_id)))
                 logger.info("TEMPMODELSTORAGE: Deleted model with id: {}".format(model_id))
                 # Add id to list of ids to pop/delete from metadata and models dict
                 ids_pop.append(model_id)
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/base.py` & `fedn-0.9.5/fedn/network/storage/s3/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,38 +2,38 @@
 
 
 class RepositoryBase(object):
     __metaclass__ = abc.ABCMeta
 
     @abc.abstractmethod
     def set_artifact(self, instance_name, instance, bucket):
-        """ Set object with name object_name
+        """Set object with name object_name
 
         :param instance_name: The name of the object
         :tyep insance_name: str
         :param instance: the object
         :param bucket: The bucket name
         :type bucket: str
         """
         raise NotImplementedError("Must be implemented by subclass")
 
     @abc.abstractmethod
     def get_artifact(self, instance_name, bucket):
-        """ Retrive object with name instance_name.
+        """Retrive object with name instance_name.
 
         :param instance_name: The name of the object to retrieve
         :type instance_name: str
         :param bucket: The bucket name
         :type bucket: str
         """
         raise NotImplementedError("Must be implemented by subclass")
 
     @abc.abstractmethod
     def get_artifact_stream(self, instance_name, bucket):
-        """ Return a stream handler for object with name instance_name.
+        """Return a stream handler for object with name instance_name.
 
         :param instance_name: The name if the object
         :type instance_name: str
         :param bucket: The bucket name
         :type bucket: str
         :return: stream handler for object instance name
         """
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/miniorepository.py` & `fedn-0.9.5/fedn/network/storage/s3/miniorepository.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,112 +1,107 @@
 import io
 
 from minio import Minio
 from minio.error import InvalidResponseError
 from urllib3.poolmanager import PoolManager
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.storage.s3.base import RepositoryBase
 
 
-@trace_all_methods
 class MINIORepository(RepositoryBase):
-    """ Class implementing Repository for MinIO. """
+    """Class implementing Repository for MinIO."""
 
     client = None
 
     def __init__(self, config):
-        """ Initialize object.
+        """Initialize object.
 
         :param config: Dictionary containing configuration for credentials and bucket names.
         :type config: dict
         """
-
         super().__init__()
         self.name = "MINIORepository"
 
-        if config['storage_secure_mode']:
-            manager = PoolManager(
-                num_pools=100, cert_reqs='CERT_NONE', assert_hostname=False)
-            self.client = Minio("{0}:{1}".format(config['storage_hostname'], config['storage_port']),
-                                access_key=config['storage_access_key'],
-                                secret_key=config['storage_secret_key'],
-                                secure=config['storage_secure_mode'], http_client=manager)
+        if config["storage_secure_mode"]:
+            manager = PoolManager(num_pools=100, cert_reqs="CERT_NONE", assert_hostname=False)
+            self.client = Minio(
+                "{0}:{1}".format(config["storage_hostname"], config["storage_port"]),
+                access_key=config["storage_access_key"],
+                secret_key=config["storage_secret_key"],
+                secure=config["storage_secure_mode"],
+                http_client=manager,
+            )
         else:
-            self.client = Minio("{0}:{1}".format(config['storage_hostname'], config['storage_port']),
-                                access_key=config['storage_access_key'],
-                                secret_key=config['storage_secret_key'],
-                                secure=config['storage_secure_mode'])
+            self.client = Minio(
+                "{0}:{1}".format(config["storage_hostname"], config["storage_port"]),
+                access_key=config["storage_access_key"],
+                secret_key=config["storage_secret_key"],
+                secure=config["storage_secure_mode"],
+            )
 
     def set_artifact(self, instance_name, instance, bucket, is_file=False):
-
         if is_file:
             self.client.fput_object(bucket, instance_name, instance)
         else:
             try:
-                self.client.put_object(
-                    bucket, instance_name, io.BytesIO(instance), len(instance))
+                self.client.put_object(bucket, instance_name, io.BytesIO(instance), len(instance))
             except Exception as e:
                 raise Exception("Could not load data into bytes {}".format(e))
 
         return True
 
     def get_artifact(self, instance_name, bucket):
-
         try:
             data = self.client.get_object(bucket, instance_name)
             return data.read()
         except Exception as e:
             raise Exception("Could not fetch data from bucket, {}".format(e))
         finally:
             data.close()
             data.release_conn()
 
     def get_artifact_stream(self, instance_name, bucket):
-
         try:
             data = self.client.get_object(bucket, instance_name)
             return data
         except Exception as e:
             raise Exception("Could not fetch data from bucket, {}".format(e))
 
     def list_artifacts(self, bucket):
-        """ List all objects in bucket.
+        """List all objects in bucket.
 
         :param bucket: Name of the bucket
         :type bucket: str
         :return: A list of object names
         """
         objects = []
         try:
             objs = self.client.list_objects(bucket)
             for obj in objs:
                 objects.append(obj.object_name)
         except Exception:
-            raise Exception(
-                "Could not list models in bucket {}".format(bucket))
+            raise Exception("Could not list models in bucket {}".format(bucket))
         return objects
 
     def delete_artifact(self, instance_name, bucket):
-        """ Delete object with name instance_name from buckets.
+        """Delete object with name instance_name from buckets.
 
         :param instance_name: The object name
         :param bucket: Buckets to delete from
         :type bucket: str
         """
-
         try:
             self.client.remove_object(bucket, instance_name)
         except InvalidResponseError as err:
-            logger.error('Could not delete artifact: {0} err: {1}'.format(instance_name, err))
+            logger.error("Could not delete artifact: {0} err: {1}".format(instance_name, err))
             pass
 
     def create_bucket(self, bucket_name):
-        """ Create a new bucket. If bucket exists, do nothing.
+        """Create a new bucket. If bucket exists, do nothing.
 
         :param bucket_name: The name of the bucket
         :type bucket_name: str
         """
         found = self.client.bucket_exists(bucket_name)
 
         if not found:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/s3/repository.py` & `fedn-0.9.5/fedn/network/storage/s3/repository.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,115 +1,106 @@
 import uuid
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.storage.s3.miniorepository import MINIORepository
 
 
-@trace_all_methods
 class Repository:
-    """ Interface for storing model objects and compute packages in S3 compatible storage. """
+    """Interface for storing model objects and compute packages in S3 compatible storage."""
 
     def __init__(self, config):
-
-        self.model_bucket = config['storage_bucket']
-        self.context_bucket = config['context_bucket']
+        self.model_bucket = config["storage_bucket"]
+        self.context_bucket = config["context_bucket"]
 
         # TODO: Make a plug-in solution
         self.client = MINIORepository(config)
 
         self.client.create_bucket(self.context_bucket)
         self.client.create_bucket(self.model_bucket)
 
     def get_model(self, model_id):
-        """ Retrieve a model with id model_id.
+        """Retrieve a model with id model_id.
 
         :param model_id: Unique identifier for model to retrive.
         :return: The model object
         """
-        logger.info("Client {} trying to get model with id: {}".format(
-            self.client.name, model_id))
+        logger.info("Client {} trying to get model with id: {}".format(self.client.name, model_id))
         return self.client.get_artifact(model_id, self.model_bucket)
 
     def get_model_stream(self, model_id):
-        """ Retrieve a stream handle to model with id model_id.
+        """Retrieve a stream handle to model with id model_id.
 
         :param model_id:
         :return: Handle to model object
         """
-        logger.info("Client {} trying to get model with id: {}".format(
-            self.client.name, model_id))
+        logger.info("Client {} trying to get model with id: {}".format(self.client.name, model_id))
         return self.client.get_artifact_stream(model_id, self.model_bucket)
 
     def set_model(self, model, is_file=True):
-        """ Upload model object.
+        """Upload model object.
 
         :param model: The model object
         :type model: BytesIO or str file name.
         :param is_file: True if model is a file name, else False
         :return: id for the uploaded object (str)
         """
         model_id = uuid.uuid4()
 
         try:
-            self.client.set_artifact(str(model_id), model,
-                                     bucket=self.model_bucket, is_file=is_file)
+            self.client.set_artifact(str(model_id), model, bucket=self.model_bucket, is_file=is_file)
         except Exception:
             logger.error("Failed to upload model with ID {} to repository.".format(model_id))
             raise
         return str(model_id)
 
     def delete_model(self, model_id):
-        """ Delete model.
+        """Delete model.
 
         :param model_id: The id of the model to delete
         :type model_id: str
         """
         try:
             self.client.delete_artifact(model_id, bucket=self.model_bucket)
         except Exception:
             logger.error("Failed to delete model {} repository.".format(model_id))
             raise
 
     def set_compute_package(self, name, compute_package, is_file=True):
-        """ Upload compute package.
+        """Upload compute package.
 
         :param name: The name of the compute package.
         :type name: str
         :param compute_package: The compute package
         :type compute_pacakge: BytesIO or str file name.
         :param is_file: True if model is a file name, else False
         """
-
         try:
-            self.client.set_artifact(str(name), compute_package,
-                                     bucket=self.context_bucket, is_file=is_file)
+            self.client.set_artifact(str(name), compute_package, bucket=self.context_bucket, is_file=is_file)
         except Exception:
             logger.error("Failed to write compute_package to repository.")
             raise
 
     def get_compute_package(self, compute_package):
-        """ Retrieve compute package from object store.
+        """Retrieve compute package from object store.
 
         :param compute_package: The name of the compute package.
         :type compute_pacakge: str
         :return: Compute package.
         """
         try:
             data = self.client.get_artifact(compute_package, bucket=self.context_bucket)
         except Exception:
             logger.error("Failed to get compute_package from repository.")
             raise
         return data
 
     def delete_compute_package(self, compute_package):
-        """ Delete a compute package from storage.
+        """Delete a compute package from storage.
 
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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/mongostatestore.py` & `fedn-0.9.5/fedn/network/storage/statestore/mongostatestore.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 import uuid
 from datetime import datetime
 
 import pymongo
 from google.protobuf.json_format import MessageToDict
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.state import ReducerStateToString, StringToReducerState
 
 
-@trace_all_methods
 class MongoStateStore:
     """Statestore implementation using MongoDB.
 
     :param network_id: The network id.
     :type network_id: str
     :param config: The statestore configuration.
     :type config: dict
@@ -59,15 +57,15 @@
             self.combiners = None
             self.clients = None
             raise
 
         self.init_index()
 
     def connect(self):
-        """ Establish client connection to MongoDB.
+        """Establish client connection to MongoDB.
 
         :param config: Dictionary containing connection strings and security credentials.
         :type config: dict
         :param network_id: Unique identifier for the FEDn network, used as db name
         :type network_id: str
         :return: MongoDB client pointing to the db corresponding to network_id
         """
@@ -123,47 +121,38 @@
         if old_state != state:
             return self.state.update_one(
                 {"state": "current_state"},
                 {"$set": {"state": ReducerStateToString(state)}},
                 True,
             )
         else:
-            logger.info(
-                "Not updating state, already in {}".format(
-                    ReducerStateToString(state)
-                )
-            )
+            logger.info("Not updating state, already in {}".format(ReducerStateToString(state)))
 
     def get_sessions(self, limit=None, skip=None, sort_key="_id", sort_order=pymongo.DESCENDING):
         """Get all sessions.
 
         :param limit: The maximum number of sessions to return.
         :type limit: int
         :param skip: The number of sessions to skip.
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
 
-            result = self.sessions.find().limit(limit).skip(skip).sort(
-                sort_key, sort_order
-            )
+            result = self.sessions.find().limit(limit).skip(skip).sort(sort_key, sort_order)
         else:
-            result = self.sessions.find().sort(
-                sort_key, sort_order
-            )
+            result = self.sessions.find().sort(sort_key, sort_order)
 
         count = self.sessions.count_documents({})
 
         return {
             "result": result,
             "count": count,
         }
@@ -181,15 +170,14 @@
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
@@ -202,17 +190,15 @@
                 "model": model_id,
                 "parent_model": parent_model,
                 "session_id": session_id,
                 "committed_at": committed_at,
             }
         )
 
-        self.model.update_one(
-            {"key": "current_model"}, {"$set": {"model": model_id}}, True
-        )
+        self.model.update_one({"key": "current_model"}, {"$set": {"model": model_id}}, True)
         self.model.update_one(
             {"key": "model_trail"},
             {
                 "$push": {
                     "model": model_id,
                     "committed_at": str(committed_at),
                 }
@@ -222,18 +208,15 @@
 
     def get_initial_model(self):
         """Return model_id for the initial model in the model trail
 
         :return: The initial model id. None if no model is found.
         :rtype: str
         """
-
-        result = self.model.find_one(
-            {"key": "model_trail"}, sort=[("committed_at", pymongo.ASCENDING)]
-        )
+        result = self.model.find_one({"key": "model_trail"}, sort=[("committed_at", pymongo.ASCENDING)])
         if result is None:
             return None
 
         try:
             model_id = result["model"]
             if model_id == "" or model_id == " ":
                 return None
@@ -262,98 +245,85 @@
     def set_current_model(self, model_id: str):
         """Set the current model in statestore.
 
         :param model_id: The model id.
         :type model_id: str
         :return:
         """
-
         try:
-
             committed_at = datetime.now()
 
             existing_model = self.model.find_one({"key": "models", "model": model_id})
 
             if existing_model is not None:
-
-                self.model.update_one(
-                    {"key": "current_model"}, {"$set": {"model": model_id, "committed_at": committed_at, "session_id": None}}, True
-                )
+                self.model.update_one({"key": "current_model"}, {"$set": {"model": model_id, "committed_at": committed_at, "session_id": None}}, True)
 
                 return True
         except Exception as e:
             logger.error("ERROR: {}".format(e))
 
         return False
 
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
-
             find = {"id": id}
             projection = {"_id": False, "key": False}
 
             doc = self.control.package.find_one(find, projection)
 
             if doc is None:
                 return False
 
             doc["key"] = "active"
 
-            self.control.package.replace_one(
-                {"key": "active"}, doc
-            )
+            self.control.package.replace_one({"key": "active"}, doc)
 
         except Exception as e:
             logger.error("ERROR: {}".format(e))
             return False
 
         return True
 
@@ -361,30 +331,27 @@
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
             "id": str(uuid.uuid4()),
         }
 
         self.control.package.update_one(
             {"key": "active"},
-            {
-                "$set": obj
-            },
+            {"$set": obj},
             True,
         )
 
         trail_obj = {**{"key": "package_trail"}, **obj}
 
         self.control.package.insert_one(trail_obj)
 
@@ -393,15 +360,14 @@
     def get_compute_package(self):
         """Get the active compute package.
 
         :return: The active compute package.
         :rtype: ObjectID
         """
         try:
-
             find = {"key": "active"}
             projection = {"key": False, "_id": False}
             ret = self.control.package.find_one(find, projection)
             return ret
         except Exception as e:
             logger.error("ERROR: {}".format(e))
             return None
@@ -416,15 +382,14 @@
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
@@ -447,34 +412,30 @@
     def set_helper(self, helper):
         """Set the active helper package in statestore.
 
         :param helper: The name of the helper package. See helper.py for available helpers.
         :type helper: str
         :return:
         """
-        self.control.package.update_one(
-            {"key": "active"}, {"$set": {"helper": helper}}, True
-        )
+        self.control.package.update_one({"key": "active"}, {"$set": {"helper": helper}}, True)
 
     def get_helper(self):
         """Get the active helper package.
 
         :return: The active helper set for the package.
         :rtype: str
         """
         ret = self.control.package.find_one({"key": "active"})
         # if local compute package used, then 'package' is None
         # if not ret:
         # get framework from round_config instead
         #    ret = self.control.config.find_one({'key': 'round_config'})
         try:
             retcheck = ret["helper"]
-            if (
-                retcheck == "" or retcheck == " "
-            ):  # ugly check for empty string
+            if retcheck == "" or retcheck == " ":  # ugly check for empty string
                 return None
             return retcheck
         except (KeyError, IndexError):
             return None
 
     def list_models(
         self,
@@ -493,37 +454,26 @@
         :param skip: The number of models to skip.
         :type skip: int
         :return: List of models.
         :rtype: list
         """
         result = None
 
-        find_option = (
-            {"key": "models"}
-            if session_id is None
-            else {"key": "models", "session_id": session_id}
-        )
+        find_option = {"key": "models"} if session_id is None else {"key": "models", "session_id": session_id}
 
         projection = {"_id": False, "key": False}
 
         if limit is not None and skip is not None:
             limit = int(limit)
             skip = int(skip)
 
-            result = (
-                self.model.find(find_option, projection)
-                .limit(limit)
-                .skip(skip)
-                .sort(sort_key, sort_order)
-            )
+            result = self.model.find(find_option, projection).limit(limit).skip(skip).sort(sort_key, sort_order)
 
         else:
-            result = self.model.find(find_option, projection).sort(
-                sort_key, sort_order
-            )
+            result = self.model.find(find_option, projection).sort(sort_key, sort_order)
 
         count = self.model.count_documents(find_option)
 
         return {
             "result": result,
             "count": count,
         }
@@ -579,15 +529,14 @@
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
@@ -623,35 +572,26 @@
         # check if kwargs is empty
 
         result = None
         count = None
         projection = {"_id": False}
 
         if not kwargs:
-            result = self.control.status.find({}, projection).sort(
-                "timestamp", pymongo.DESCENDING
-            )
+            result = self.control.status.find({}, projection).sort("timestamp", pymongo.DESCENDING)
             count = self.control.status.count_documents({})
         else:
             limit = kwargs.pop("limit", None)
             skip = kwargs.pop("skip", None)
 
             if limit is not None and skip is not None:
                 limit = int(limit)
                 skip = int(skip)
-                result = (
-                    self.control.status.find(kwargs, projection)
-                    .sort("timestamp", pymongo.DESCENDING)
-                    .limit(limit)
-                    .skip(skip)
-                )
+                result = self.control.status.find(kwargs, projection).sort("timestamp", pymongo.DESCENDING).limit(limit).skip(skip)
             else:
-                result = self.control.status.find(kwargs, projection).sort(
-                    "timestamp", pymongo.DESCENDING
-                )
+                result = self.control.status.find(kwargs, projection).sort("timestamp", pymongo.DESCENDING)
 
             count = self.control.status.count_documents(kwargs)
 
         return {
             "result": result,
             "count": count,
         }
@@ -659,46 +599,40 @@
     def get_storage_backend(self):
         """Get the storage backend.
 
         :return: The storage backend.
         :rtype: ObjectID
         """
         try:
-            ret = self.storage.find(
-                {"status": "enabled"}, projection={"_id": False}
-            )
+            ret = self.storage.find({"status": "enabled"}, projection={"_id": False})
             return ret[0]
         except (KeyError, IndexError):
             return None
 
     def set_storage_backend(self, config):
         """Set the storage backend.
 
         :param config: The storage backend configuration.
         :type config: dict
         :return:
         """
         config = copy.deepcopy(config)
         config["updated_at"] = str(datetime.now())
         config["status"] = "enabled"
-        self.storage.update_one(
-            {"storage_type": config["storage_type"]}, {"$set": config}, True
-        )
+        self.storage.update_one({"storage_type": config["storage_type"]}, {"$set": config}, True)
 
     def set_reducer(self, reducer_data):
         """Set the reducer in the statestore.
 
         :param reducer_data: dictionary of reducer config.
         :type reducer_data: dict
         :return:
         """
         reducer_data["updated_at"] = str(datetime.now())
-        self.reducer.update_one(
-            {"name": reducer_data["name"]}, {"$set": reducer_data}, True
-        )
+        self.reducer.update_one({"name": reducer_data["name"]}, {"$set": reducer_data}, True)
 
     def get_reducer(self):
         """Get reducer.config.
 
         return: reducer config.
         rtype: ObjectId
         """
@@ -734,15 +668,14 @@
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
@@ -763,19 +696,16 @@
     def set_combiner(self, combiner_data):
         """Set combiner in statestore.
 
         :param combiner_data: dictionary of combiner config
         :type combiner_data: dict
         :return:
         """
-
         combiner_data["updated_at"] = str(datetime.now())
-        self.combiners.update_one(
-            {"name": combiner_data["name"]}, {"$set": combiner_data}, True
-        )
+        self.combiners.update_one({"name": combiner_data["name"]}, {"$set": combiner_data}, True)
 
     def delete_combiner(self, combiner):
         """Delete a combiner from statestore.
 
         :param combiner: name of combiner to delete.
         :type combiner: str
         :return:
@@ -791,17 +721,15 @@
         """Set client in statestore.
 
         :param client_data: dictionary of client config.
         :type client_data: dict
         :return:
         """
         client_data["updated_at"] = str(datetime.now())
-        self.clients.update_one(
-            {"name": client_data["name"]}, {"$set": client_data}, True
-        )
+        self.clients.update_one({"name": client_data["name"]}, {"$set": client_data}, True)
 
     def get_client(self, name):
         """Get client by name.
 
         :param name: name of client to get.
         :type name: str
         :return: The client. None if not found.
@@ -823,15 +751,14 @@
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
 
@@ -860,27 +787,26 @@
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
-
-            pipeline = [
-                {"$match": {"combiner": {"$in": combiners}, "status": "online"}},
-                {"$group": {"_id": "$combiner", "count": {"$sum": 1}}},
-                {"$sort": {sort_key: sort_order, "_id": pymongo.ASCENDING}}
-            ] if combiners is not None else [
-                {"$group": {"_id": "$combiner", "count": {"$sum": 1}}},
-                {"$sort": {sort_key: sort_order, "_id": pymongo.ASCENDING}}
-            ]
+            pipeline = (
+                [
+                    {"$match": {"combiner": {"$in": combiners}, "status": "online"}},
+                    {"$group": {"_id": "$combiner", "count": {"$sum": 1}}},
+                    {"$sort": {sort_key: sort_order, "_id": pymongo.ASCENDING}},
+                ]
+                if combiners is not None
+                else [{"$group": {"_id": "$combiner", "count": {"$sum": 1}}}, {"$sort": {sort_key: sort_order, "_id": pymongo.ASCENDING}}]
+            )
 
             result = self.clients.aggregate(pipeline)
 
         except Exception as e:
             logger.error(e)
 
         return result
@@ -909,27 +835,27 @@
 
     def drop_status(self):
         """Drop the status collection."""
         if self.status:
             self.status.drop()
 
     def create_session(self, id=None):
-        """ Create a new session object.
+        """Create a new session object.
 
         :param id: The ID of the created session.
         :type id: uuid, str
 
         """
         if not id:
             id = uuid.uuid4()
-        data = {'session_id': str(id)}
+        data = {"session_id": str(id)}
         self.sessions.insert_one(data)
 
     def create_round(self, round_data):
-        """ Create a new round.
+        """Create a new round.
 
         :param round_data: Dictionary with round data.
         :type round_data: dict
         """
         # TODO: Add check if round_id already exists
         self.rounds.insert_one(round_data)
 
@@ -937,70 +863,64 @@
         """Set the session configuration.
 
         :param id: The session id
         :type id: str
         :param config: Session configuration
         :type config: dict
         """
-        self.sessions.update_one({'session_id': str(id)}, {
-            '$push': {'session_config': config}}, True)
+        self.sessions.update_one({"session_id": str(id)}, {"$push": {"session_config": config}}, True)
 
     def set_session_status(self, id, status):
         """Set session status.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_status: The status of the session.
         """
-        self.sessions.update_one({'session_id': str(id)}, {
-            '$set': {'status': status}}, True)
+        self.sessions.update_one({"session_id": str(id)}, {"$set": {"status": status}}, True)
 
     def set_round_combiner_data(self, data):
         """Set combiner round controller data.
 
         :param data: The combiner data
         :type data: dict
         """
-        self.rounds.update_one({'round_id': str(data['round_id'])}, {
-            '$push': {'combiners': data}}, True)
+        self.rounds.update_one({"round_id": str(data["round_id"])}, {"$push": {"combiners": data}}, True)
 
     def set_round_config(self, round_id, round_config):
         """Set round configuration.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_config: The round configuration
         :type round_config: dict
         """
-        self.rounds.update_one({'round_id': round_id}, {
-            '$set': {'round_config': round_config}}, True)
+        self.rounds.update_one({"round_id": round_id}, {"$set": {"round_config": round_config}}, True)
 
     def set_round_status(self, round_id, round_status):
         """Set round status.
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_status: The status of the round.
         """
-        self.rounds.update_one({'round_id': round_id}, {
-            '$set': {'status': round_status}}, True)
+        self.rounds.update_one({"round_id": round_id}, {"$set": {"status": round_status}}, True)
 
     def set_round_data(self, round_id, round_data):
         """Update round metadata
 
         :param round_id: The round unique identifier
         :type round_id: str
         :param round_data: The round metadata
         :type round_data: dict
         """
-        self.rounds.update_one({'round_id': round_id}, {
-            '$set': {'round_data': round_data}}, True)
+        self.rounds.update_one({"round_id": round_id}, {"$set": {"round_data": round_data}}, True)
 
     def update_client_status(self, clients, status):
-        """ Update client status in statestore.
+        """Update client status in statestore.
         :param client_name: The client name
         :type client_name: str
         :param status: The client status
         :type status: str
         :return: None
         """
         datetime_now = datetime.now()
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/statestorebase.py` & `fedn-0.9.5/fedn/network/storage/statestore/statestorebase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,52 +1,49 @@
 from abc import ABC, abstractmethod
 
 
 class StateStoreBase(ABC):
-    """
-
-    """
+    """ """
 
     def __init__(self):
         pass
 
     @abstractmethod
     def state(self):
-        """ Return the current state of the statestore.
-        """
+        """Return the current state of the statestore."""
         pass
 
     @abstractmethod
     def transition(self, state):
-        """ Transition the statestore to a new state.
+        """Transition the statestore to a new state.
 
         :param state: The new state.
         :type state: str
         """
         pass
 
     @abstractmethod
     def set_latest_model(self, model_id):
-        """ Set the latest model id in the statestore.
+        """Set the latest model id in the statestore.
 
         :param model_id: The model id.
         :type model_id: str
         """
         pass
 
     @abstractmethod
     def get_latest_model(self):
-        """ Get the latest model id from the statestore.
+        """Get the latest model id from the statestore.
 
         :return: The model object.
         :rtype: ObjectId
         """
         pass
 
     @abstractmethod
     def is_inited(self):
-        """ Check if the statestore is initialized.
+        """Check if the statestore is initialized.
 
         :return: True if initialized, else False.
         :rtype: bool
         """
         pass
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/client_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/client_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/combiner_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/combiner_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/model_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/model_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/package_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/package_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/round_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/round_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/session_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/validation_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/status_store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/status_store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/network/storage/statestore/stores/store.py` & `fedn-0.9.5/fedn/network/storage/statestore/stores/store.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/dispatcher.py` & `fedn-0.9.5/fedn/utils/dispatcher.py`

 * *Files 16% similar despite different names*

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
 
@@ -23,23 +22,21 @@
 import uuid
 from contextlib import contextmanager
 from pathlib import Path
 
 import yaml
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods, tracer
 from fedn.utils import PYTHON_VERSION
 from fedn.utils.environment import _PythonEnv
 from fedn.utils.process import _exec_cmd, _join_commands
 
 _IS_UNIX = os.name != "nt"
 
 
-@tracer.start_as_current_span("remove_on_error")
 @contextmanager
 def remove_on_error(path: os.PathLike, onerror=None):
     """A context manager that removes a file or directory if an exception is raised during
     execution.
     """
     try:
         yield
@@ -50,80 +47,65 @@
             if os.path.isfile(path):
                 os.remove(path)
             elif os.path.isdir(path):
                 shutil.rmtree(path)
         raise
 
 
-@tracer.start_as_current_span("_install_python")
 def _install_python(version, pyenv_root=None, capture_output=False):
     """Installs a specified version of python with pyenv and returns a path to the installed python
     binary.
     """
     raise NotImplementedError("This function is not implemented yet.")
 
 
-@tracer.start_as_current_span("_is_virtualenv_available")
 def _is_virtualenv_available():
-    """
-    Returns True if virtualenv is available, otherwise False.
+    """Returns True if virtualenv is available, otherwise False.
     """
     return shutil.which("virtualenv") is not None
 
 
-@tracer.start_as_current_span("_validate_virtualenv_is_available")
 def _validate_virtualenv_is_available():
-    """
-    Validates virtualenv is available. If not, throws an `Exception` with a brief instruction
+    """Validates virtualenv is available. If not, throws an `Exception` with a brief instruction
     on how to install virtualenv.
     """
     if not _is_virtualenv_available():
-        raise Exception(
-            "Could not find the virtualenv binary. Run `pip install virtualenv` to install "
-            "virtualenv."
-        )
+        raise Exception("Could not find the virtualenv binary. Run `pip install virtualenv` to install " "virtualenv.")
 
 
-@tracer.start_as_current_span("_get_virtualenv_extra_env_vars")
 def _get_virtualenv_extra_env_vars(env_root_dir=None):
     extra_env = {
         # PIP_NO_INPUT=1 makes pip run in non-interactive mode,
         # otherwise pip might prompt "yes or no" and ask stdin input
         "PIP_NO_INPUT": "1",
     }
     return extra_env
 
 
-@tracer.start_as_current_span("_get_python_env")
 def _get_python_env(python_env_file):
-    """
-    Parses a python environment file and returns a dictionary with the parsed content.
+    """Parses a python environment file and returns a dictionary with the parsed content.
     """
     if os.path.exists(python_env_file):
         return _PythonEnv.from_yaml(python_env_file)
 
 
-@tracer.start_as_current_span("_create_virtualenv")
-def _create_virtualenv(
-    python_bin_path, env_dir, python_env, extra_env=None, capture_output=False
-):
+def _create_virtualenv(python_bin_path, env_dir, python_env, extra_env=None, capture_output=False):
     # Created a command to activate the environment
     paths = ("bin", "activate") if _IS_UNIX else ("Scripts", "activate.bat")
     activate_cmd = env_dir.joinpath(*paths)
     activate_cmd = f"source {activate_cmd}" if _IS_UNIX else str(activate_cmd)
 
     if env_dir.exists():
         logger.info("Environment %s already exists", env_dir)
         return activate_cmd
 
     with remove_on_error(
         env_dir,
         onerror=lambda e: logger.warning(
-            "Encountered an unexpected error: %s while creating a virtualenv environment in %s, "
-            "removing the environment directory...",
+            "Encountered an unexpected error: %s while creating a virtualenv environment in %s, " "removing the environment directory...",
             repr(e),
             env_dir,
         ),
     ):
         logger.info("Creating a new environment in %s with %s", env_dir, python_bin_path)
         _exec_cmd(
             [sys.executable, "-m", "virtualenv", "--python", python_bin_path, env_dir],
@@ -131,67 +113,57 @@
         )
 
         logger.info("Installing dependencies")
         for deps in filter(None, [python_env.build_dependencies, python_env.dependencies]):
             with tempfile.TemporaryDirectory() as tmpdir:
                 tmp_req_file = f"requirements.{uuid.uuid4().hex}.txt"
                 Path(tmpdir).joinpath(tmp_req_file).write_text("\n".join(deps))
-                cmd = _join_commands(
-                    activate_cmd, f"python -m pip install --quiet -r {tmp_req_file}"
-                )
+                cmd = _join_commands(activate_cmd, f"python -m pip install -r {tmp_req_file}")
                 _exec_cmd(cmd, capture_output=capture_output, cwd=tmpdir, extra_env=extra_env)
 
     return activate_cmd
 
 
-@tracer.start_as_current_span("_read_yaml_file")
 def _read_yaml_file(file_path):
     try:
         cfg = None
-        with open(file_path, 'rb') as config_file:
-
+        with open(file_path, "rb") as config_file:
             cfg = yaml.safe_load(config_file.read())
 
     except Exception as e:
-        logger.error(
-            f"Error trying to read yaml file: {file_path}"
-        )
+        logger.error(f"Error trying to read yaml file: {file_path}")
         raise e
     return cfg
 
 
-@trace_all_methods
 class Dispatcher:
-    """ Dispatcher class for compute packages.
+    """Dispatcher class for compute packages.
 
     :param config: The configuration.
     :type config: dict
     :param dir: The directory to dispatch to.
     :type dir: str
     """
 
     def __init__(self, config, project_dir):
-        """ Initialize the dispatcher."""
+        """Initialize the dispatcher."""
         self.config = config
         self.project_dir = project_dir
         self.activate_cmd = ""
         self.python_env_path = ""
 
     def _get_or_create_python_env(self, capture_output=False, pip_requirements_override=None):
         python_env = self.config.get("python_env", "")
         if not python_env:
             logger.info("No python_env specified in the configuration, using the system Python.")
             return python_env
         else:
             python_env_path = os.path.join(self.project_dir, python_env)
             if not os.path.exists(python_env_path):
-                raise Exception(
-                    "Compute package specified python_env file %s, but no such "
-                    "file was found." % python_env_path
-                )
+                raise Exception("Compute package specified python_env file %s, but no such " "file was found." % python_env_path)
             python_env = _get_python_env(python_env_path)
 
         extra_env = _get_virtualenv_extra_env_vars()
         env_dir = Path(self.project_dir) / Path(python_env.name)
         self.python_env_path = env_dir
         try:
             python_bin_path = _install_python(python_env.python, capture_output=True)
@@ -207,18 +179,15 @@
                 env_dir,
                 python_env,
                 extra_env=extra_env,
                 capture_output=capture_output,
             )
             # Install additional dependencies specified by `requirements_override`
             if pip_requirements_override:
-                logger.info(
-                    "Installing additional dependencies specified by "
-                    f"pip_requirements_override: {pip_requirements_override}"
-                )
+                logger.info("Installing additional dependencies specified by " f"pip_requirements_override: {pip_requirements_override}")
                 cmd = _join_commands(
                     activate_cmd,
                     f"python -m pip install --quiet -U {' '.join(pip_requirements_override)}",
                 )
                 _exec_cmd(cmd, capture_output=capture_output, extra_env=extra_env)
             self.activate_cmd = activate_cmd
             return activate_cmd
@@ -228,50 +197,46 @@
                 logger.warning("Attempting to remove %s", env_dir)
                 shutil.rmtree(env_dir, ignore_errors=True)
                 msg = "Failed to remove %s" if env_dir.exists() else "Successfully removed %s"
                 logger.warning(msg, env_dir)
 
             raise
 
-    def run_cmd(self,
-                cmd_type,
-                capture_output=False,
-                extra_env=None,
-                synchronous=True,
-                stream_output=False
-                ):
-        """ Run a command.
+    def run_cmd(self, cmd_type, capture_output=False, extra_env=None, synchronous=True, stream_output=False):
+        """Run a command.
 
         :param cmd_type: The command type.
         :type cmd_type: str
         :return:
         """
         try:
-            cmdsandargs = cmd_type.split(' ')
-            entry_point = self.config['entry_points'][cmdsandargs[0]]['command']
+            cmdsandargs = cmd_type.split(" ")
+
+            entry_point = self.config["entry_points"][cmdsandargs[0]]["command"]
+
             # remove the first element,  that is not a file but a command
             args = cmdsandargs[1:]
 
             # Join entry point and arguments into a single command as a string
-            entry_point_args = ' '.join(args)
+            entry_point_args = " ".join(args)
             entry_point = f"{entry_point} {entry_point_args}"
 
             if self.activate_cmd:
                 cmd = _join_commands(self.activate_cmd, entry_point)
             else:
                 cmd = _join_commands(entry_point)
 
-            logger.info('Running command: {}'.format(cmd))
+            logger.info("Running command: {}".format(cmd))
             _exec_cmd(
                 cmd,
                 cwd=self.project_dir,
                 throw_on_error=True,
                 extra_env=extra_env,
                 capture_output=capture_output,
                 synchronous=synchronous,
                 stream_output=stream_output,
             )
 
-            logger.info('Done executing {}'.format(cmd_type))
+            logger.info("Done executing {}".format(cmd_type))
         except IndexError:
             message = "No such argument or configuration to run."
             logger.error(message)
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/environment.py` & `fedn-0.9.5/fedn/utils/environment.py`

 * *Files 15% similar despite different names*

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
 
@@ -11,48 +10,47 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import yaml
 
-from fedn.common.telemetry import trace_all_methods
 from fedn.utils import PYTHON_VERSION
 
 _REQUIREMENTS_FILE_NAME = "requirements.txt"
 _PYTHON_ENV_FILE_NAME = "python_env.yaml"
 
 
-@trace_all_methods
 class _PythonEnv:
     BUILD_PACKAGES = ("pip", "setuptools", "wheel")
 
     def __init__(self, name=None, python=None, build_dependencies=None, dependencies=None):
-        """
-        Represents environment information for FEDn compute packages.
+        """Represents environment information for FEDn compute packages.
 
         Args:
+        ----
+            name: Name of environment. If unspecified, defaults to fedn_env
             python: Python version for the environment. If unspecified, defaults to the current
                 Python version.
             build_dependencies: List of build dependencies for the environment that must
                 be installed before installing ``dependencies``. If unspecified,
                 defaults to an empty list.
             dependencies: List of dependencies for the environment. If unspecified, defaults to
                 an empty list.
+
         """
         if name is not None and not isinstance(name, str):
             raise TypeError(f"`name` must be a string but got {type(name)}")
         if python is not None and not isinstance(python, str):
             raise TypeError(f"`python` must be a string but got {type(python)}")
         if build_dependencies is not None and not isinstance(build_dependencies, list):
-            raise TypeError(
-                f"`build_dependencies` must be a list but got {type(build_dependencies)}"
-            )
+            raise TypeError(f"`build_dependencies` must be a list but got {type(build_dependencies)}")
         if dependencies is not None and not isinstance(dependencies, list):
             raise TypeError(f"`dependencies` must be a list but got {type(dependencies)}")
         self.name = name or "fedn_env"
         self.python = python or PYTHON_VERSION
         self.build_dependencies = build_dependencies or []
         self.dependencies = dependencies or []
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/flowercompat/client_app_adapter.py` & `fedn-0.9.5/fedn/utils/flowercompat/client_app_adapter.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,61 +1,65 @@
 from typing import Tuple
 
 from flwr.client import ClientApp
-from flwr.common import (Context, EvaluateIns, FitIns, GetParametersIns,
-                         Message, MessageType, MessageTypeLegacy, Metadata,
-                         NDArrays, ndarrays_to_parameters,
-                         parameters_to_ndarrays)
-from flwr.common.recordset_compat import (evaluateins_to_recordset,
-                                          fitins_to_recordset,
-                                          getparametersins_to_recordset,
-                                          recordset_to_evaluateres,
-                                          recordset_to_fitres,
-                                          recordset_to_getparametersres)
+from flwr.common import (
+    Context,
+    EvaluateIns,
+    FitIns,
+    GetParametersIns,
+    Message,
+    MessageType,
+    MessageTypeLegacy,
+    Metadata,
+    NDArrays,
+    ndarrays_to_parameters,
+    parameters_to_ndarrays,
+)
+from flwr.common.recordset_compat import (
+    evaluateins_to_recordset,
+    fitins_to_recordset,
+    getparametersins_to_recordset,
+    recordset_to_evaluateres,
+    recordset_to_fitres,
+    recordset_to_getparametersres,
+)
 
-from fedn.common.telemetry import trace_all_methods
 
-
-@trace_all_methods
 class FlwrClientAppAdapter:
     """Flwr ClientApp wrapper."""
 
     def __init__(self, app: ClientApp) -> None:
         self.app = app
 
     def init_parameters(self, partition_id: int, config: dict = {}):
         # Construct a get_parameters message for the ClientApp
-        message, context = self._construct_message(
-            MessageTypeLegacy.GET_PARAMETERS, [], partition_id, config
-        )
+        message, context = self._construct_message(MessageTypeLegacy.GET_PARAMETERS, [], partition_id, config)
         # Call client app with train message
         client_return_message = self.app(message, context)
         # return NDArrays of clients parameters
         parameters = self._parse_get_parameters_message(client_return_message)
         if len(parameters) == 0:
-            raise ValueError("The 'parameters' list is empty. Ensure your flower \
-                             client has implemented a get_parameters() function.")
+            raise ValueError(
+                "The 'parameters' list is empty. Ensure your flower \
+                             client has implemented a get_parameters() function."
+            )
         return parameters
 
     def train(self, parameters: NDArrays, partition_id: int, config: dict = {}):
         # Construct a train message for the ClientApp with given parameters
-        message, context = self._construct_message(
-            MessageType.TRAIN, parameters, partition_id, config
-        )
+        message, context = self._construct_message(MessageType.TRAIN, parameters, partition_id, config)
         # Call client app with train message
         client_return_message = self.app(message, context)
         # Parse return message
         params, num_examples = self._parse_train_message(client_return_message)
         return params, num_examples
 
     def evaluate(self, parameters: NDArrays, partition_id: int, config: dict = {}):
         # Construct an evaluate message for the ClientApp with given parameters
-        message, context = self._construct_message(
-            MessageType.EVALUATE, parameters, partition_id, config
-        )
+        message, context = self._construct_message(MessageType.EVALUATE, parameters, partition_id, config)
         # Call client app with evaluate message
         client_return_message = self.app(message, context)
         # Parse return message
         loss, accuracy = self._parse_evaluate_message(client_return_message)
         return loss, accuracy
 
     def _parse_get_parameters_message(self, message: Message) -> NDArrays:
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/helperbase.py` & `fedn-0.9.5/fedn/utils/helpers/helperbase.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,52 +1,40 @@
-import os
-import tempfile
 from abc import ABC, abstractmethod
 
 
 class HelperBase(ABC):
-    """ Abstract class defining helpers. """
+    """Abstract class defining helpers."""
 
     def __init__(self):
-        """ Initialize helper. """
-
+        """Initialize helper."""
         self.name = self.__class__.__name__
 
     @abstractmethod
     def increment_average(self, m1, m2, a, W):
-        """ Compute one increment of incremental weighted averaging.
+        """Compute one increment of incremental weighted averaging.
 
         :param m1: Current model weights in array-like format.
         :param m2: New model weights in array-like format.
         :param a: Number of examples in new model.
         :param W: Total number of examples.
         :return: Incremental weighted average of model weights.
         """
         pass
 
     @abstractmethod
     def save(self, model, path):
-        """ Serialize weights to file. The serialized model must be a single binary object.
+        """Serialize weights to file. The serialized model must be a single binary object.
 
         :param model: Weights in array-like format.
         :param path: Path to file.
 
         """
         pass
 
     @abstractmethod
     def load(self, fh):
-        """ Load weights from file or filelike.
+        """Load weights from file or filelike.
 
         :param fh: file path, filehandle, filelike.
         :return: Weights in array-like format.
         """
         pass
-
-    def get_tmp_path(self):
-        """ Return a temporary output path compatible with save_model, load_model.
-
-        :return: Path to file.
-        """
-        fd, path = tempfile.mkstemp(suffix='.npz')
-        os.close(fd)
-        return path
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/helpers.py` & `fedn-0.9.5/fedn/utils/helpers/helpers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 import importlib
 import json
 
-from fedn.common.telemetry import tracer
-
 HELPER_PLUGIN_PATH = "fedn.utils.helpers.plugins.{}"
 
 
-@tracer.start_as_current_span(name="get_helper")
 def get_helper(helper_module_name):
-    """ Return an instance of the helper class.
+    """Return an instance of the helper class.
 
     :param helper_module_name: The name of the helper plugin module.
     :type helper_module_name: str
     :return: A helper instance.
     :rtype: class: `fedn.utils.helpers.helpers.HelperBase`
     """
     helper_plugin = HELPER_PLUGIN_PATH.format(helper_module_name)
     helper = importlib.import_module(helper_plugin)
     return helper.Helper()
 
 
-@tracer.start_as_current_span("save_metadata")
 def save_metadata(metadata, filename):
-    """ Save metadata to file.
+    """Save metadata to file.
 
     :param metadata: The metadata to save.
     :type metadata: dict
     :param filename: The name of the file to save to.
     :type filename: str
     """
-    with open(filename+'-metadata', 'w') as outfile:
+    with open(filename + "-metadata", "w") as outfile:
         json.dump(metadata, outfile)
 
 
-@tracer.start_as_current_span("save_metrics")
 def save_metrics(metrics, filename):
-    """ Save metrics to file.
+    """Save metrics to file.
 
     :param metrics: The metrics to save.
     :type metrics: dict
     :param filename: The name of the file to save to.
     :type filename: str
     """
-    with open(filename, 'w') as outfile:
+    with open(filename, "w") as outfile:
         json.dump(metrics, outfile)
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/helpers/plugins/androidhelper.py` & `fedn-0.9.5/fedn/utils/helpers/plugins/androidhelper.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,28 @@
 import os
 import struct
 import tempfile
 
 import numpy as np
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.utils.helpers.helperbase import HelperBase
 
 
-@trace_all_methods
 class Helper(HelperBase):
     """FEDn helper class for android json model weights."""
 
     def __init__(self):
         """Initialize helper."""
         self.name = "androidhelper"
         super().__init__()
 
     # function to calculate an incremental weighted average of the weights
 
-    def increment_average(
-            self, model, model_next, num_examples, total_examples
-    ):
+    def increment_average(self, model, model_next, num_examples, total_examples):
         """Incremental weighted average of model weights.
 
         :param model: Current model weights.
         :type model: list of numpy arrays.
         :param model_next: New model weights.
         :type model_next: list of numpy arrays.
         :param num_examples: Number of examples in new model.
@@ -38,17 +34,15 @@
         """
         # Incremental weighted average
         w = num_examples / total_examples
 
         return (1 - w) * model + w * model_next
 
     # function to calculate an incremental weighted average of the weights using numpy.add
-    def increment_average_add(
-        self, model, model_next, num_examples, total_examples
-    ):
+    def increment_average_add(self, model, model_next, num_examples, total_examples):
         """Incremental weighted average of model weights.
 
         :param model: Current model weights.
         :type model: list of numpy arrays.
         :param model_next: New model weights.
         :type model_next: list of numpy arrays.
         :param num_examples: Number of examples in new model.
@@ -57,31 +51,29 @@
         :type total_examples: int
         :return: Incremental weighted average of model weights.
         :rtype: list of numpy arrays.
         """
         # Incremental weighted average
         w = np.add(
             model,
-            num_examples
-            * (np.array(model_next) - np.array(model))
-            / total_examples,
+            num_examples * (np.array(model_next) - np.array(model)) / total_examples,
         )
         return w
 
     def save(self, weights, path=None):
         """Serialize weights to file. The serialized model must be a single binary object.
 
         :param weights: weights in json format.
         :param path: Path to file.
         :return: Path to file.
         """
         if not path:
             path = self.get_tmp_path()
 
-        byte_array = struct.pack("f"*len(weights), *weights)
+        byte_array = struct.pack("f" * len(weights), *weights)
         with open(path, "wb") as file:
             file.write(byte_array)
 
         return path
 
     def load(self, fh):
         """Load weights from file or filelike.
@@ -92,15 +84,15 @@
         logger.debug("in android helper load")
         if isinstance(fh, str):
             with open(fh, "rb") as file:
                 byte_data = file.read()
         else:
             byte_data = fh.read()
 
-        weights = np.array(struct.unpack(f'{len(byte_data) // 4}f', byte_data))
+        weights = np.array(struct.unpack(f"{len(byte_data) // 4}f", byte_data))
 
         return weights
 
     def get_tmp_path(self):
         """Return a temporary output path compatible with save_model, load_model.
 
         :return: Path to file.
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/plots.py` & `fedn-0.9.5/fedn/utils/plots.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,91 +3,80 @@
 
 import numpy
 import plotly
 import plotly.graph_objs as go
 from plotly.subplots import make_subplots
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import trace_all_methods
 from fedn.network.storage.statestore.mongostatestore import MongoStateStore
 
 
-@trace_all_methods
 class Plot:
-    """
-
-    """
+    """ """
 
     def __init__(self, statestore):
         try:
             statestore_config = statestore.get_config()
-            statestore = MongoStateStore(
-                statestore_config['network_id'], statestore_config['mongo_config'])
+            statestore = MongoStateStore(statestore_config["network_id"], statestore_config["mongo_config"])
             self.mdb = statestore.connect()
-            self.status = self.mdb['control.status']
+            self.status = self.mdb["control.status"]
             self.round_time = self.mdb["control.round_time"]
             self.combiner_round_time = self.mdb["control.combiner_round_time"]
             self.psutil_usage = self.mdb["control.psutil_monitoring"]
             self.network_clients = self.mdb["network.clients"]
 
         except Exception as e:
             logger.error("FAILED TO CONNECT TO MONGO, {}".format(e))
             self.collection = None
             raise
 
     # plot metrics from DB
     def _scalar_metrics(self, metrics):
-        """ Extract all scalar valued metrics from a MODEL_VALIDATON. """
-
-        data = json.loads(metrics['data'])
-        data = json.loads(data['data'])
+        """Extract all scalar valued metrics from a MODEL_VALIDATON."""
+        data = json.loads(metrics["data"])
+        data = json.loads(data["data"])
 
         valid_metrics = []
         for metric, val in data.items():
             # If it can be converted to a float it is a valid, scalar metric
             try:
                 val = float(val)
                 valid_metrics.append(metric)
             except Exception:
                 pass
 
         return valid_metrics
 
     def create_table_plot(self):
+        """:return:
         """
-
-        :return:
-        """
-        metrics = self.status.find_one({'type': 'MODEL_VALIDATION'})
+        metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         if metrics is None:
             fig = go.Figure(data=[])
-            fig.update_layout(
-                title_text='No data currently available for table mean metrics')
+            fig.update_layout(title_text="No data currently available for table mean metrics")
             table = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return False
 
         valid_metrics = self._scalar_metrics(metrics)
         if valid_metrics == []:
             fig = go.Figure(data=[])
-            fig.update_layout(title_text='No scalar metrics found')
+            fig.update_layout(title_text="No scalar metrics found")
             table = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return False
 
         all_vals = []
         models = []
         for metric in valid_metrics:
             validations = {}
-            for post in self.status.find({'type': 'MODEL_VALIDATION'}):
-                e = json.loads(post['data'])
+            for post in self.status.find({"type": "MODEL_VALIDATION"}):
+                e = json.loads(post["data"])
                 try:
-                    validations[e['modelId']].append(
-                        float(json.loads(e['data'])[metric]))
+                    validations[e["modelId"]].append(float(json.loads(e["data"])[metric]))
                 except KeyError:
-                    validations[e['modelId']] = [
-                        float(json.loads(e['data'])[metric])]
+                    validations[e["modelId"]] = [float(json.loads(e["data"])[metric])]
 
             vals = []
             models = []
             for model, data in validations.items():
                 vals.append(numpy.mean(data))
                 models.append(model)
             all_vals.append(vals)
@@ -96,264 +85,239 @@
         models.reverse()
         values = [models]
 
         for vals in all_vals:
             vals.reverse()
             values.append(vals)
 
-        fig = go.Figure(data=[go.Table(
-            header=dict(values=['Model ID'] + header_vals,
-                        line_color='darkslategray',
-                        fill_color='lightskyblue',
-                        align='left'),
-
-            cells=dict(values=values,  # 2nd column
-                       line_color='darkslategray',
-                       fill_color='lightcyan',
-                       align='left'))
-        ])
+        fig = go.Figure(
+            data=[
+                go.Table(
+                    header=dict(values=["Model ID"] + header_vals, line_color="darkslategray", fill_color="lightskyblue", align="left"),
+                    cells=dict(
+                        values=values,  # 2nd column
+                        line_color="darkslategray",
+                        fill_color="lightcyan",
+                        align="left",
+                    ),
+                )
+            ]
+        )
 
-        fig.update_layout(title_text='Summary: mean metrics')
+        fig.update_layout(title_text="Summary: mean metrics")
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
-        for p in self.status.find({'type': 'MODEL_UPDATE_REQUEST'}):
-            e = json.loads(p['data'])
-            cid = e['correlationId']
-            for cc in self.status.find({'sender': p['sender'], 'type': 'MODEL_UPDATE'}):
-                da = json.loads(cc['data'])
-                if da['correlationId'] == cid:
+        for p in self.status.find({"type": "MODEL_UPDATE_REQUEST"}):
+            e = json.loads(p["data"])
+            cid = e["correlationId"]
+            for cc in self.status.find({"sender": p["sender"], "type": "MODEL_UPDATE"}):
+                da = json.loads(cc["data"])
+                if da["correlationId"] == cid:
                     cp = cc
 
-            cd = json.loads(cp['data'])
-            tr = datetime.strptime(e['timestamp'], '%Y-%m-%d %H:%M:%S.%f')
-            tu = datetime.strptime(cd['timestamp'], '%Y-%m-%d %H:%M:%S.%f')
+            cd = json.loads(cp["data"])
+            tr = datetime.strptime(e["timestamp"], "%Y-%m-%d %H:%M:%S.%f")
+            tu = datetime.strptime(cd["timestamp"], "%Y-%m-%d %H:%M:%S.%f")
             ts = tu - tr
             base.append(tr.timestamp())
             x.append(ts.total_seconds() / 60.0)
-            y.append(p['sender']['name'])
+            y.append(p["sender"]["name"])
 
-        trace_data.append(go.Bar(
-            x=y,
-            y=x,
-            marker=dict(color='royalblue'),
-            name="Training",
-        ))
+        trace_data.append(
+            go.Bar(
+                x=y,
+                y=x,
+                marker=dict(color="royalblue"),
+                name="Training",
+            )
+        )
 
         x = []
         y = []
         base = []
-        for p in self.status.find({'type': 'MODEL_VALIDATION_REQUEST'}):
-            e = json.loads(p['data'])
-            cid = e['correlationId']
-            for cc in self.status.find({'sender': p['sender'], 'type': 'MODEL_VALIDATION'}):
-                da = json.loads(cc['data'])
-                if da['correlationId'] == cid:
+        for p in self.status.find({"type": "MODEL_VALIDATION_REQUEST"}):
+            e = json.loads(p["data"])
+            cid = e["correlationId"]
+            for cc in self.status.find({"sender": p["sender"], "type": "MODEL_VALIDATION"}):
+                da = json.loads(cc["data"])
+                if da["correlationId"] == cid:
                     cp = cc
-            cd = json.loads(cp['data'])
-            tr = datetime.strptime(e['timestamp'], '%Y-%m-%d %H:%M:%S.%f')
-            tu = datetime.strptime(cd['timestamp'], '%Y-%m-%d %H:%M:%S.%f')
+            cd = json.loads(cp["data"])
+            tr = datetime.strptime(e["timestamp"], "%Y-%m-%d %H:%M:%S.%f")
+            tu = datetime.strptime(cd["timestamp"], "%Y-%m-%d %H:%M:%S.%f")
             ts = tu - tr
             base.append(tr.timestamp())
             x.append(ts.total_seconds() / 60.0)
-            y.append(p['sender']['name'])
+            y.append(p["sender"]["name"])
 
-        trace_data.append(go.Bar(
-            x=y,
-            y=x,
-            marker=dict(color='lightskyblue'),
-            name="Validation",
-        ))
+        trace_data.append(
+            go.Bar(
+                x=y,
+                y=x,
+                marker=dict(color="lightskyblue"),
+                name="Validation",
+            )
+        )
 
         layout = go.Layout(
-            barmode='stack',
+            barmode="stack",
             showlegend=True,
         )
 
         fig = go.Figure(data=trace_data, layout=layout)
-        fig.update_xaxes(title_text='Alliance/client')
-        fig.update_yaxes(title_text='Time (Min)')
-        fig.update_layout(title_text='Alliance timeline')
+        fig.update_xaxes(title_text="Alliance/client")
+        fig.update_yaxes(title_text="Time (Min)")
+        fig.update_layout(title_text="Alliance timeline")
         timeline = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return timeline
 
     def create_client_training_distribution(self):
-        """
-
-        :return:
+        """:return:
         """
         training = []
-        for p in self.status.find({'type': 'MODEL_UPDATE'}):
-            e = json.loads(p['data'])
-            meta = json.loads(e['meta'])
-            training.append(meta['exec_training'])
+        for p in self.status.find({"type": "MODEL_UPDATE"}):
+            e = json.loads(p["data"])
+            meta = json.loads(e["meta"])
+            training.append(meta["exec_training"])
 
         if not training:
             return False
         fig = go.Figure(data=go.Histogram(x=training))
-        fig.update_layout(
-            title_text='Client model training time, mean: {}'.format(numpy.mean(training)))
+        fig.update_layout(title_text="Client model training time, mean: {}".format(numpy.mean(training)))
         histogram = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return histogram
 
     def create_client_histogram_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         training = []
-        for p in self.status.find({'type': 'MODEL_UPDATE'}):
-            e = json.loads(p['data'])
-            meta = json.loads(e['meta'])
-            training.append(meta['exec_training'])
+        for p in self.status.find({"type": "MODEL_UPDATE"}):
+            e = json.loads(p["data"])
+            meta = json.loads(e["meta"])
+            training.append(meta["exec_training"])
 
         fig = go.Figure()
 
         fig.update_layout(
             template="simple_white",
             xaxis=dict(title_text="Time (s)"),
-            yaxis=dict(title_text='Number of updates'),
-            title="Mean client training time: {}".format(
-                numpy.mean(training)),
+            yaxis=dict(title_text="Number of updates"),
+            title="Mean client training time: {}".format(numpy.mean(training)),
             # showlegend=True
         )
         if not training:
             return False
 
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
-        for p in self.status.find({'type': 'MODEL_UPDATE'}):
-            e = json.loads(p['data'])
-            meta = json.loads(e['meta'])
-            upload.append(meta['upload_model'])
-            download.append(meta['fetch_model'])
-            training.append(meta['exec_training'])
-            processing.append(meta['processing_time'])
+        for p in self.status.find({"type": "MODEL_UPDATE"}):
+            e = json.loads(p["data"])
+            meta = json.loads(e["meta"])
+            upload.append(meta["upload_model"])
+            download.append(meta["fetch_model"])
+            training.append(meta["exec_training"])
+            processing.append(meta["processing_time"])
 
         fig = go.Figure()
-        fig.update_layout(
-            template="simple_white",
-            title="Mean client processing time: {}".format(
-                numpy.mean(processing)),
-            showlegend=True
-        )
+        fig.update_layout(template="simple_white", title="Mean client processing time: {}".format(numpy.mean(processing)), showlegend=True)
         if not processing:
             return False
         data = [numpy.mean(training), numpy.mean(upload), numpy.mean(download)]
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
-        for round in self.mdb['control.round'].find():
+        for round in self.mdb["control.round"].find():
             try:
-                for combiner in round['combiners']:
+                for combiner in round["combiners"]:
                     data = combiner
-                    stats = data['local_round']['1']
-                    ml = stats['aggregation_time']['time_model_load']
-                    ag = stats['aggregation_time']['time_model_aggregation']
-                    combination.append(stats['time_combination'])
-                    waiting.append(stats['time_combination'] - ml - ag)
+                    stats = data["local_round"]["1"]
+                    ml = stats["aggregation_time"]["time_model_load"]
+                    ag = stats["aggregation_time"]["time_model_aggregation"]
+                    combination.append(stats["time_combination"])
+                    waiting.append(stats["time_combination"] - ml - ag)
                     model_load.append(ml)
                     aggregation.append(ag)
             except Exception:
                 pass
 
-        labels = ['Waiting for client updates',
-                  'Aggregation', 'Loading model updates from disk']
-        val = [numpy.mean(waiting), numpy.mean(
-            aggregation), numpy.mean(model_load)]
+        labels = ["Waiting for client updates", "Aggregation", "Loading model updates from disk"]
+        val = [numpy.mean(waiting), numpy.mean(aggregation), numpy.mean(model_load)]
         fig = go.Figure()
 
-        fig.update_layout(
-            template="simple_white",
-            title="Mean combiner round time: {}".format(
-                numpy.mean(combination)),
-            showlegend=True
-        )
+        fig.update_layout(template="simple_white", title="Mean combiner round time: {}".format(numpy.mean(combination)), showlegend=True)
         if not combination:
             return False
         fig.add_trace(go.Pie(labels=labels, values=val))
         combiner_plot = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return combiner_plot
 
     def fetch_valid_metrics(self):
+        """:return:
         """
-
-        :return:
-        """
-        metrics = self.status.find_one({'type': 'MODEL_VALIDATION'})
+        metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         valid_metrics = self._scalar_metrics(metrics)
         return valid_metrics
 
     def create_box_plot(self, metric):
-        """
-
-        :param metric:
+        """:param metric:
         :return:
         """
-        metrics = self.status.find_one({'type': 'MODEL_VALIDATION'})
+        metrics = self.status.find_one({"type": "MODEL_VALIDATION"})
         if metrics is None:
             fig = go.Figure(data=[])
-            fig.update_layout(title_text='No data currently available for metric distribution over  '
-                                         'participants')
+            fig.update_layout(title_text="No data currently available for metric distribution over  " "participants")
             box = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return box
 
         valid_metrics = self._scalar_metrics(metrics)
         if valid_metrics == []:
             fig = go.Figure(data=[])
-            fig.update_layout(title_text='No scalar metrics found')
+            fig.update_layout(title_text="No scalar metrics found")
             box = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return box
 
         validations = {}
-        for post in self.status.find({'type': 'MODEL_VALIDATION'}):
-            e = json.loads(post['data'])
+        for post in self.status.find({"type": "MODEL_VALIDATION"}):
+            e = json.loads(post["data"])
             try:
-                validations[e['modelId']].append(
-                    float(json.loads(e['data'])[metric]))
+                validations[e["modelId"]].append(float(json.loads(e["data"])[metric]))
             except KeyError:
-                validations[e['modelId']] = [
-                    float(json.loads(e['data'])[metric])]
+                validations[e["modelId"]] = [float(json.loads(e["data"])[metric])]
 
         # Make sure validations are plotted in chronological order
-        model_trail = self.mdb.control.model.find_one({'key': 'model_trail'})
-        model_trail_ids = model_trail['model']
+        model_trail = self.mdb.control.model.find_one({"key": "model_trail"})
+        model_trail_ids = model_trail["model"]
         validations_sorted = []
         for model_id in model_trail_ids:
             try:
                 validations_sorted.append(validations[model_id])
             except Exception:
                 pass
 
@@ -362,117 +326,86 @@
         box = go.Figure()
 
         y = []
         for j, acc in enumerate(validations):
             # x.append(j)
             y.append(numpy.mean([float(i) for i in acc]))
             if len(acc) >= 2:
-                box.add_trace(go.Box(y=acc, name=str(j), marker_color="royalblue", showlegend=False,
-                                     boxpoints=False))
+                box.add_trace(go.Box(y=acc, name=str(j), marker_color="royalblue", showlegend=False, boxpoints=False))
             else:
-                box.add_trace(go.Scatter(
-                    x=[str(j)], y=[y[j]], showlegend=False))
+                box.add_trace(go.Scatter(x=[str(j)], y=[y[j]], showlegend=False))
 
         rounds = list(range(len(y)))
-        box.add_trace(go.Scatter(
-            x=rounds,
-            y=y,
-            name='Mean'
-        ))
-
-        box.update_xaxes(title_text='Rounds')
-        box.update_yaxes(
-            tickvals=[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
-        box.update_layout(title_text='Metric distribution over clients: {}'.format(metric),
-                          margin=dict(l=20, r=20, t=45, b=20))
+        box.add_trace(go.Scatter(x=rounds, y=y, name="Mean"))
+
+        box.update_xaxes(title_text="Rounds")
+        box.update_yaxes(tickvals=[0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0])
+        box.update_layout(title_text="Metric distribution over clients: {}".format(metric), margin=dict(l=20, r=20, t=45, b=20))
         box = json.dumps(box, cls=plotly.utils.PlotlyJSONEncoder)
         return box
 
     def create_round_plot(self):
-        """
-
-        :return:
+        """:return:
         """
         trace_data = []
-        metrics = self.round_time.find_one({'key': 'round_time'})
+        metrics = self.round_time.find_one({"key": "round_time"})
         if metrics is None:
             fig = go.Figure(data=[])
-            fig.update_layout(
-                title_text='No data currently available for round time')
+            fig.update_layout(title_text="No data currently available for round time")
             return False
 
-        for post in self.round_time.find({'key': 'round_time'}):
-            rounds = post['round']
-            traces_data = post['round_time']
-
-        trace_data.append(go.Scatter(
-            x=rounds,
-            y=traces_data,
-            mode='lines+markers',
-            name='Reducer'
-        ))
-
-        for rec in self.combiner_round_time.find({'key': 'combiner_round_time'}):
-            c_traces_data = rec['round_time']
-
-        trace_data.append(go.Scatter(
-            x=rounds,
-            y=c_traces_data,
-            mode='lines+markers',
-            name='Combiner'
-        ))
+        for post in self.round_time.find({"key": "round_time"}):
+            rounds = post["round"]
+            traces_data = post["round_time"]
+
+        trace_data.append(go.Scatter(x=rounds, y=traces_data, mode="lines+markers", name="Reducer"))
+
+        for rec in self.combiner_round_time.find({"key": "combiner_round_time"}):
+            c_traces_data = rec["round_time"]
+
+        trace_data.append(go.Scatter(x=rounds, y=c_traces_data, mode="lines+markers", name="Combiner"))
 
         fig = go.Figure(data=trace_data)
-        fig.update_xaxes(title_text='Round')
-        fig.update_yaxes(title_text='Time (s)')
-        fig.update_layout(title_text='Round time')
+        fig.update_xaxes(title_text="Round")
+        fig.update_yaxes(title_text="Time (s)")
+        fig.update_layout(title_text="Round time")
         round_t = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return round_t
 
     def create_cpu_plot(self):
+        """:return:
         """
-
-        :return:
-        """
-        metrics = self.psutil_usage.find_one({'key': 'cpu_mem_usage'})
+        metrics = self.psutil_usage.find_one({"key": "cpu_mem_usage"})
         if metrics is None:
             fig = go.Figure(data=[])
-            fig.update_layout(
-                title_text='No data currently available for MEM and CPU usage')
+            fig.update_layout(title_text="No data currently available for MEM and CPU usage")
             cpu = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
             return False
 
-        for post in self.psutil_usage.find({'key': 'cpu_mem_usage'}):
-            cpu = post['cpu']
-            mem = post['mem']
-            ps_time = post['time']
-            round = post['round']
+        for post in self.psutil_usage.find({"key": "cpu_mem_usage"}):
+            cpu = post["cpu"]
+            mem = post["mem"]
+            ps_time = post["time"]
+            round = post["round"]
 
         # Create figure with secondary y-axis
         fig = make_subplots(specs=[[{"secondary_y": True}]])
-        fig.add_trace(go.Scatter(
-            x=ps_time,
-            y=cpu,
-            mode='lines+markers',
-            name='CPU (%)'
-        ))
-
-        fig.add_trace(go.Scatter(
-            x=ps_time,
-            y=mem,
-            mode='lines+markers',
-            name='MEM (%)'
-        ))
-
-        fig.add_trace(go.Scatter(
-            x=ps_time,
-            y=round,
-            mode='lines+markers',
-            name='Round',
-        ), secondary_y=True)
+        fig.add_trace(go.Scatter(x=ps_time, y=cpu, mode="lines+markers", name="CPU (%)"))
+
+        fig.add_trace(go.Scatter(x=ps_time, y=mem, mode="lines+markers", name="MEM (%)"))
+
+        fig.add_trace(
+            go.Scatter(
+                x=ps_time,
+                y=round,
+                mode="lines+markers",
+                name="Round",
+            ),
+            secondary_y=True,
+        )
 
-        fig.update_xaxes(title_text='Date Time')
-        fig.update_yaxes(title_text='Percentage (%)')
+        fig.update_xaxes(title_text="Date Time")
+        fig.update_yaxes(title_text="Percentage (%)")
         fig.update_yaxes(title_text="Round", secondary_y=True)
-        fig.update_layout(title_text='CPU loads and memory usage')
+        fig.update_layout(title_text="CPU loads and memory usage")
         cpu = json.dumps(fig, cls=plotly.utils.PlotlyJSONEncoder)
         return cpu
```

### Comparing `fedn-0.9.3/fedn/build/lib/fedn/utils/process.py` & `fedn-0.9.5/fedn/utils/process.py`

 * *Files 10% similar despite different names*

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
 
@@ -11,20 +10,20 @@
 
 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
 """
+
 import os
 import subprocess
 import sys
 
 from fedn.common.log_config import logger
-from fedn.common.telemetry import tracer
 
 _IS_UNIX = os.name != "nt"
 
 
 class ShellCommandException(Exception):
     @classmethod
     def from_completed_process(cls, process):
@@ -43,81 +42,78 @@
                 "",
                 "STDERR:",
                 process.stderr,
             ]
         return cls("\n".join(lines))
 
 
-@tracer.start_as_current_span("_join_commands")
 def _join_commands(*commands):
     entry_point = ["bash", "-c"] if _IS_UNIX else ["cmd", "/c"]
     sep = " && " if _IS_UNIX else " & "
     return [*entry_point, sep.join(map(str, commands))]
 
 
-@tracer.start_as_current_span("_exec_cmd")
 def _exec_cmd(
     cmd,
     *,
     cwd=None,
     throw_on_error=True,
     extra_env=None,
     capture_output=True,
     synchronous=True,
     stream_output=False,
     **kwargs,
 ):
     """A convenience wrapper of `subprocess.Popen` for running a command from a Python script.
 
     Args:
+    ----
         cmd: The command to run, as a string or a list of strings.
+        cwd: The current working directory.
         throw_on_error: If True, raises an Exception if the exit code of the program is nonzero.
         extra_env: Extra environment variables to be defined when running the child process.
             If this argument is specified, `kwargs` cannot contain `env`.
         capture_output: If True, stdout and stderr will be captured and included in an exception
             message on failure; if False, these streams won't be captured.
         synchronous: If True, wait for the command to complete and return a CompletedProcess
             instance, If False, does not wait for the command to complete and return
             a Popen instance, and ignore the `throw_on_error` argument.
         stream_output: If True, stream the command's stdout and stderr to `sys.stdout`
             as a unified stream during execution.
             If False, do not stream the command's stdout and stderr to `sys.stdout`.
         kwargs: Keyword arguments (except `text`) passed to `subprocess.Popen`.
 
     Returns:
+    -------
         If synchronous is True, return a `subprocess.CompletedProcess` instance,
         otherwise return a Popen instance.
 
     """
     illegal_kwargs = set(kwargs.keys()).intersection({"text"})
     if illegal_kwargs:
         raise ValueError(f"`kwargs` cannot contain {list(illegal_kwargs)}")
 
     env = kwargs.pop("env", None)
     if extra_env is not None and env is not None:
         raise ValueError("`extra_env` and `env` cannot be used at the same time")
 
     if capture_output and stream_output:
-        raise ValueError(
-            "`capture_output=True` and `stream_output=True` cannot be specified at the same time"
-        )
+        raise ValueError("`capture_output=True` and `stream_output=True` cannot be specified at the same time")
 
     env = env if extra_env is None else {**os.environ, **extra_env}
 
     # In Python < 3.8, `subprocess.Popen` doesn't accept a command containing path-like
     # objects (e.g. `["ls", pathlib.Path("abc")]`) on Windows. To avoid this issue,
     # stringify all elements in `cmd`. Note `str(pathlib.Path("abc"))` returns 'abc'.
     if isinstance(cmd, list):
         cmd = list(map(str, cmd))
 
     if capture_output or stream_output:
         if kwargs.get("stdout") is not None or kwargs.get("stderr") is not None:
-            raise ValueError(
-                "stdout and stderr arguments may not be used with capture_output or stream_output"
-            )
+            raise ValueError("stdout and stderr arguments may not be used with capture_output or stream_output")
         kwargs["stdout"] = subprocess.PIPE
         if capture_output:
             kwargs["stderr"] = subprocess.PIPE
         elif stream_output:
             # Redirect stderr to stdout in order to combine the streams for unified printing to
             # `sys.stdout`, as documented in
             # https://docs.python.org/3/library/subprocess.html#subprocess.run
@@ -146,29 +142,27 @@
         stderr=stderr,
     )
     if throw_on_error and returncode != 0:
         raise ShellCommandException.from_completed_process(comp_process)
     return comp_process
 
 
-@tracer.start_as_current_span("run_process")
 def run_process(args, cwd):
-    """ Run a process and log the output.
+    """Run a process and log the output.
 
     :param args: The arguments to the process.
     :type args: list
     :param cwd: The current working directory.
     :type cwd: str
     :return:
     """
-    status = subprocess.Popen(
-        args, cwd=cwd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
+    status = subprocess.Popen(args, cwd=cwd, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
 
     def check_io():
-        """ Check stdout/stderr of the child process.
+        """Check stdout/stderr of the child process.
 
         :return:
         """
         while True:
             output = status.stdout.readline().decode()
             if output:
                 logger.info(output)
```

### Comparing `fedn-0.9.3/fedn/build/lib/network/combiner/aggregators/fedopt.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/fedopt.py`

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

### Comparing `fedn-0.9.3/fedn/build/lib/utils/parameters.py` & `fedn-0.9.5/fedn/utils/parameters.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/network/combiner/aggregators/tests/test_fedavg.py` & `fedn-0.9.5/fedn/network/combiner/aggregators/tests/test_fedavg.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/network/loadbalancer/firstavailable.py` & `fedn-0.9.5/fedn/network/loadbalancer/firstavailable.py`

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

### Comparing `fedn-0.9.3/fedn/network/storage/models/tests/test_tempmodelstorage.py` & `fedn-0.9.5/fedn/network/storage/models/tests/test_tempmodelstorage.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/utils/helpers/tests/test_numpyhelper.py` & `fedn-0.9.5/fedn/utils/helpers/tests/test_numpyhelper.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/utils/tests/test_helpers.py` & `fedn-0.9.5/fedn/utils/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn/utils/tests/test_parameters.py` & `fedn-0.9.5/fedn/utils/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `fedn-0.9.3/fedn.egg-info/PKG-INFO` & `fedn-0.9.5/fedn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fedn
-Version: 0.9.3
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

### Comparing `fedn-0.9.3/pyproject.toml` & `fedn-0.9.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fedn"
-version = "0.9.3"
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

