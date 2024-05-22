# Comparing `tmp/metaflow-stubs-2.11.8.tar.gz` & `tmp/metaflow-stubs-2.11.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metaflow-stubs-2.11.8.tar", last modified: Fri Mar 29 12:38:00 2024, max compression
+gzip compressed data, was "metaflow-stubs-2.11.9.tar", last modified: Fri Mar 29 22:28:02 2024, max compression
```

## Comparing `metaflow-stubs-2.11.8.tar` & `metaflow-stubs-2.11.9.tar`

### file list

```diff
@@ -1,164 +1,164 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 12:37:47.000000 metaflow-stubs-2.11.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 12:37:47.000000 metaflow-stubs-2.11.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.661055 metaflow-stubs-2.11.8/metaflow-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)   107435 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/cli.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.661055 metaflow-stubs-2.11.8/metaflow-stubs/client/
--rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/client/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/client/core.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/client/filecache.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/clone_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/flowspec.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/generated_for.txt
--rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/includefile.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.661055 metaflow-stubs-2.11.8/metaflow-stubs/metadata/
--rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/metadata/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/metadata/util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/metaflow_config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/metaflow_current.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.661055 metaflow-stubs-2.11.8/metaflow-stubs/mflog/
--rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/mflog/mflog.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/multicore_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/parameters.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.665056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.665056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/exception.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.665056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.665056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_events.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.669056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/aws_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/aws_utils.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.669056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.669056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/secrets_manager/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.669056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.673056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/azure_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/azure_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.673056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_creator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_datastore.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.673056 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/basic.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/card.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/components.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_resolver.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/component_serializer.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/exception.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/catch_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/
--rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/local.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/
--rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/debug_logger.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/debug_monitor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/environment_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/events_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/frameworks/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/frameworks/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/frameworks/pytorch.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/gs_utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/includefile_support.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.677055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/package_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/parallel_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/project_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/conda_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/conda_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/pypi_environment.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/resources_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/retry_decorator.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/storage_executor.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/tag_cli.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/plugins/timeout_decorator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/procpoll.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/pylint_wrapper.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/tagging_util.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-29 12:37:59.000000 metaflow-stubs-2.11.8/metaflow-stubs/version.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/metaflow_stubs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 12:38:00.681055 metaflow-stubs-2.11.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-29 12:37:47.000000 metaflow-stubs-2.11.8/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 12:38:00.000000 metaflow-stubs-2.11.8/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)   107435 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9145 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2908 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/cli.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/client/
+-rw-r--r--   0 runner    (1001) docker     (127)    28941 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    40806 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/core.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/client/filecache.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1090 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/clone_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3405 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10442 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/flowspec.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/generated_for.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    18152 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/includefile.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/metadata/
+-rw-r--r--   0 runner    (1001) docker     (127)    12396 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/metadata/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/metadata/util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/metaflow_config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/metaflow_current.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.446081 metaflow-stubs-2.11.9/metaflow-stubs/mflog/
+-rw-r--r--   0 runner    (1001) docker     (127)      621 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/mflog/mflog.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2369 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/multicore_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/parameters.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)     5528 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3221 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3053 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/exception.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.450081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_events.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    14340 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5800 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5870 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_utils.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4723 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3226 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/production_token.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6526 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4441 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.454081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2537 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1748 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    18088 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_creator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_datastore.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4258 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7581 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/basic.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1816 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/card.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/
+-rw-r--r--   0 runner    (1001) docker     (127)     2711 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2667 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/metadata.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3525 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     7674 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/components.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_resolver.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/component_serializer.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/exception.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1826 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/catch_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.458081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/
+-rw-r--r--   0 runner    (1001) docker     (127)    12909 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/local.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/
+-rw-r--r--   0 runner    (1001) docker     (127)    20310 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    29021 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-03-29 22:28:01.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3tail.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_logger.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_monitor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/environment_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/events_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1622 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/pytorch.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      772 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_exceptions.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_storage_client_factory.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1184 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/includefile_support.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2955 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4891 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/package_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/parallel_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/project_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2312 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      905 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_environment.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      609 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/resources_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/retry_decorator.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.462081 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/secrets_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/storage_executor.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    10363 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/tag_cli.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/plugins/timeout_decorator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/procpoll.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/pylint_wrapper.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/tagging_util.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-03-29 22:28:00.000000 metaflow-stubs-2.11.9/metaflow-stubs/version.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/metaflow_stubs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 22:28:02.466081 metaflow-stubs-2.11.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-03-29 22:27:44.000000 metaflow-stubs-2.11.9/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-29 22:28:02.000000 metaflow-stubs-2.11.9/version.py
```

### Comparing `metaflow-stubs-2.11.8/PKG-INFO` & `metaflow-stubs-2.11.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-stubs
-Version: 2.11.8
+Version: 2.11.9
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: metaflow==2.11.8
+Requires-Dist: metaflow==2.11.9
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.184463                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.911417                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
-    import metaflow.plugins.datatools.s3.s3
-    import metaflow._vendor.click.types
-    import metaflow.client.core
     import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
+    import metaflow.metaflow_current
     import typing
+    import io
+    import metaflow.events
     import metaflow.parameters
     import datetime
-    import io
-    import metaflow.metaflow_current
+    import metaflow.client.core
+    import metaflow._vendor.click.types
 FlowSpecDerived = typing.TypeVar("FlowSpecDerived", bound="FlowSpec", contravariant=False, covariant=False)
 StepFlag = typing.NewType("StepFlag", bool)
 
 CURRENT_DIRECTORY: str
 
 INFO_FILE: str
 
@@ -722,14 +722,65 @@
     -------
     Union[Callable[[FlowSpecDerived, StepFlag], None], Callable[[FlowSpecDerived, Any, StepFlag], None]]
         Function that is a Metaflow Step
     """
     ...
 
 @typing.overload
+def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+    ...
+
+@typing.overload
+def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
+    """
+    Creates a human-readable report, a Metaflow Card, after this step completes.
+    
+    Note that you may add multiple `@card` decorators in a step with different parameters.
+    
+    Parameters
+    ----------
+    type : str, default 'default'
+        Card type.
+    id : str, optional, default None
+        If multiple cards are present, use this id to identify this card.
+    options : Dict[str, Any], default {}
+        Options passed to the card. The contents depend on the card type.
+    timeout : int, default 45
+        Interrupt reporting if it takes more than this many seconds.
+    
+    
+    """
+    ...
+
+@typing.overload
 def environment(*, vars: typing.Dict[str, str] = {}) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies environment variables to be set prior to the execution of a step.
     
     Parameters
     ----------
     vars : Dict[str, str], default {}
@@ -753,63 +804,43 @@
     ----------
     vars : Dict[str, str], default {}
         Dictionary of environment variables to set.
     """
     ...
 
 @typing.overload
-def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
-    
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
+def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
     """
-    Specifies the number of times the task corresponding
-    to a step needs to be retried.
-    
-    This decorator is useful for handling transient errors, such as networking issues.
-    If your task contains operations that can't be retried safely, e.g. database updates,
-    it is advisable to annotate it with `@retry(times=0)`.
-    
-    This can be used in conjunction with the `@catch` decorator. The `@catch`
-    decorator will execute a no-op task after all retries have been exhausted,
-    ensuring that the flow execution can continue.
+    Specifies secrets to be retrieved and injected as environment variables prior to
+    the execution of a step.
     
     Parameters
     ----------
-    times : int, default 3
-        Number of times to retry this task.
-    minutes_between_retries : int, default 2
-        Number of minutes between retries.
+    sources : List[Union[str, Dict[str, Any]]], default: []
+        List of secret specs, defining how the secrets are to be retrieved
     """
     ...
 
 @typing.overload
 def resources(*, cpu: int = 1, gpu: int = 0, disk: typing.Optional[int] = None, memory: int = 4096, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies the resources needed when executing this step.
@@ -883,63 +914,14 @@
     shared_memory : int, optional, default None
         The value for the size (in MiB) of the /dev/shm volume for this step.
         This parameter maps to the `--shm-size` option in Docker.
     """
     ...
 
 @typing.overload
-def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
-    """
-    Specifies that the step will success under all circumstances.
-    
-    The decorator will create an optional artifact, specified by `var`, which
-    contains the exception raised. You can use it to detect the presence
-    of errors, indicating that all happy-path artifacts produced by the step
-    are missing.
-    
-    Parameters
-    ----------
-    var : str, optional, default None
-        Name of the artifact in which to store the caught exception.
-        If not specified, the exception is not stored.
-    print_exception : bool, default True
-        Determines whether or not the exception is printed to
-        stdout when caught.
-    """
-    ...
-
-@typing.overload
 def batch(*, cpu: int = 1, gpu: int = 0, memory: int = 4096, image: typing.Optional[str] = None, queue: str = "METAFLOW_BATCH_JOB_QUEUE", iam_role: str = "METAFLOW_ECS_S3_ACCESS_IAM_ROLE", execution_role: str = "METAFLOW_ECS_FARGATE_EXECUTION_ROLE", shared_memory: typing.Optional[int] = None, max_swap: typing.Optional[int] = None, swappiness: typing.Optional[int] = None, use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = None, inferentia: int = 0, trainium: int = None, efa: int = 0, ephemeral_storage: int = None, log_driver: typing.Optional[str] = None, log_options: typing.Optional[typing.List[str]] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on [AWS Batch](https://aws.amazon.com/batch/).
     
     Parameters
     ----------
     cpu : int, default 1
@@ -1079,200 +1061,161 @@
         List of strings containing options for the chosen log driver. The configurable values
         depend on the `log driver` chosen. Validation of these options is not supported yet.
         Example usage: ["awslogs-group:aws/batch/job"]
     """
     ...
 
 @typing.overload
-def card(*, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
+    Specifies the PyPI packages for the step.
     
-    Note that you may add multiple `@card` decorators in a step with different parameters.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def card(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def card(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, type: str = "default", id: typing.Optional[str] = None, options: typing.Dict[str, typing.Any] = {}, timeout: int = 45):
-    """
-    Creates a human-readable report, a Metaflow Card, after this step completes.
-    
-    Note that you may add multiple `@card` decorators in a step with different parameters.
-    
-    Parameters
-    ----------
-    type : str, default 'default'
-        Card type.
-    id : str, optional, default None
-        If multiple cards are present, use this id to identify this card.
-    options : Dict[str, Any], default {}
-        Options passed to the card. The contents depend on the card type.
-    timeout : int, default 45
-        Interrupt reporting if it takes more than this many seconds.
-    
-    
-    """
+def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-@typing.overload
-def secrets(*, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
     """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Specifies the PyPI packages for the step.
     
-    Parameters
-    ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
-    """
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
-    ...
-
-@typing.overload
-def secrets(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
-    ...
-
-def secrets(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, sources: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = []):
-    """
-    Specifies secrets to be retrieved and injected as environment variables prior to
-    the execution of a step.
+    Information in this decorator will augment any
+    attributes set in the `@pyi_base` flow-level decorator. Hence,
+    you can use `@pypi_base` to set packages required by all
+    steps and use `@pypi` to specify step-specific overrides.
     
     Parameters
     ----------
-    sources : List[Union[str, Dict[str, Any]]], default: []
-        List of secret specs, defining how the secrets are to be retrieved
+    packages : Dict[str, str], default: {}
+        Packages to use for this step. The key is the name of the package
+        and the value is the version to use.
+    python : str, optional, default: None
+        Version of Python to use, e.g. '3.7.4'. A default value of None implies
+        that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
 @typing.overload
-def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def retry(*, times: int = 3, minutes_between_retries: int = 2) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def retry(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
+def retry(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, times: int = 3, minutes_between_retries: int = 2):
     """
-    Specifies a timeout for your step.
-    
-    This decorator is useful if this step may hang indefinitely.
+    Specifies the number of times the task corresponding
+    to a step needs to be retried.
     
-    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
-    A timeout is considered to be an exception thrown by the step. It will cause the step to be
-    retried if needed and the exception will be caught by the `@catch` decorator, if present.
+    This decorator is useful for handling transient errors, such as networking issues.
+    If your task contains operations that can't be retried safely, e.g. database updates,
+    it is advisable to annotate it with `@retry(times=0)`.
     
-    Note that all the values specified in parameters are added together so if you specify
-    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
+    This can be used in conjunction with the `@catch` decorator. The `@catch`
+    decorator will execute a no-op task after all retries have been exhausted,
+    ensuring that the flow execution can continue.
     
     Parameters
     ----------
-    seconds : int, default 0
-        Number of seconds to wait prior to timing out.
-    minutes : int, default 0
-        Number of minutes to wait prior to timing out.
-    hours : int, default 0
-        Number of hours to wait prior to timing out.
+    times : int, default 3
+        Number of times to retry this task.
+    minutes_between_retries : int, default 2
+        Number of minutes between retries.
     """
     ...
 
 @typing.overload
-def pypi(*, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
+def catch(*, var: typing.Optional[str] = None, print_exception: bool = True) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the PyPI packages for the step.
+    Specifies that the step will success under all circumstances.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
 @typing.overload
-def pypi(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+def catch(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
     ...
 
-def pypi(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, packages: typing.Dict[str, str] = {}, python: typing.Optional[str] = None):
+def catch(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, var: typing.Optional[str] = None, print_exception: bool = True):
     """
-    Specifies the PyPI packages for the step.
+    Specifies that the step will success under all circumstances.
     
-    Information in this decorator will augment any
-    attributes set in the `@pyi_base` flow-level decorator. Hence,
-    you can use `@pypi_base` to set packages required by all
-    steps and use `@pypi` to specify step-specific overrides.
+    The decorator will create an optional artifact, specified by `var`, which
+    contains the exception raised. You can use it to detect the presence
+    of errors, indicating that all happy-path artifacts produced by the step
+    are missing.
     
     Parameters
     ----------
-    packages : Dict[str, str], default: {}
-        Packages to use for this step. The key is the name of the package
-        and the value is the version to use.
-    python : str, optional, default: None
-        Version of Python to use, e.g. '3.7.4'. A default value of None implies
-        that the version used will correspond to the version of the Python interpreter used to start the run.
+    var : str, optional, default None
+        Name of the artifact in which to store the caught exception.
+        If not specified, the exception is not stored.
+    print_exception : bool, default True
+        Determines whether or not the exception is printed to
+        stdout when caught.
     """
     ...
 
 def kubernetes(*, cpu: int = 1, memory: int = 4096, disk: int = 10240, image: typing.Optional[str] = None, image_pull_policy: str = "KUBERNETES_IMAGE_PULL_POLICY", service_account: str = "METAFLOW_KUBERNETES_SERVICE_ACCOUNT", secrets: typing.Optional[typing.List[str]] = None, namespace: str = "METAFLOW_KUBERNETES_NAMESPACE", gpu: typing.Optional[int] = None, gpu_vendor: str = "KUBERNETES_GPU_VENDOR", tolerations: typing.List[str] = [], use_tmpfs: bool = False, tmpfs_tempdir: bool = True, tmpfs_size: typing.Optional[int] = None, tmpfs_path: typing.Optional[str] = "/metaflow_temp", persistent_volume_claims: typing.Optional[typing.Dict[str, str]] = None, shared_memory: typing.Optional[int] = None) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
     Specifies that this step should execute on Kubernetes.
     
@@ -1383,111 +1326,83 @@
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables @conda.
     """
     ...
 
 @typing.overload
-def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+def timeout(*, seconds: int = 0, minutes: int = 0, hours: int = 0) -> typing.Callable[[typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]], typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]]]:
     """
-    Specifies the flow(s) that this flow depends on.
-    
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
+    Specifies a timeout for your step.
     
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
+    This decorator is useful if this step may hang indefinitely.
     
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
     Parameters
     ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
-    
-    
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
     """
     ...
 
 @typing.overload
-def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+def timeout(f: typing.Callable[[FlowSpecDerived, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, StepFlag], None]:
     ...
 
-def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
+@typing.overload
+def timeout(f: typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]) -> typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None]:
+    ...
+
+def timeout(f: typing.Union[typing.Callable[[FlowSpecDerived, StepFlag], None], typing.Callable[[FlowSpecDerived, typing.Any, StepFlag], None], None] = None, *, seconds: int = 0, minutes: int = 0, hours: int = 0):
     """
-    Specifies the flow(s) that this flow depends on.
+    Specifies a timeout for your step.
     
-    ```
-    @trigger_on_finish(flow='FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
-    ```
-    This decorator respects the @project decorator and triggers the flow
-    when upstream runs within the same namespace complete successfully
+    This decorator is useful if this step may hang indefinitely.
     
-    Additionally, you can specify project aware upstream flow dependencies
-    by specifying the fully qualified project_flow_name.
-    ```
-    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
-    ```
-    or
-    ```
-    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
-    ```
+    This can be used in conjunction with the `@retry` decorator as well as the `@catch` decorator.
+    A timeout is considered to be an exception thrown by the step. It will cause the step to be
+    retried if needed and the exception will be caught by the `@catch` decorator, if present.
     
-    You can also specify just the project or project branch (other values will be
-    inferred from the current project or project branch):
-    ```
-    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
-    ```
+    Note that all the values specified in parameters are added together so if you specify
+    60 seconds and 1 hour, the decorator will have an effective timeout of 1 hour and 1 minute.
     
-    Note that `branch` is typically one of:
-      - `prod`
-      - `user.bob`
-      - `test.my_experiment`
-      - `prod.staging`
+    Parameters
+    ----------
+    seconds : int, default 0
+        Number of seconds to wait prior to timing out.
+    minutes : int, default 0
+        Number of minutes to wait prior to timing out.
+    hours : int, default 0
+        Number of hours to wait prior to timing out.
+    """
+    ...
+
+def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies what flows belong to the same project.
+    
+    A project-specific namespace is created for all flows that
+    use the same `@project(name)`.
     
     Parameters
     ----------
-    flow : Union[str, Dict[str, str]], optional, default None
-        Upstream flow dependency for this flow.
-    flows : List[Union[str, Dict[str, str]]], default []
-        Upstream flow dependencies for this flow.
-    options : Dict[str, Any], default {}
-        Backend-specific configuration for tuning eventing behavior.
+    name : str
+        Project name. Make sure that the name is unique amongst all
+        projects that use the same production scheduler. The name may
+        contain only lowercase alphanumeric characters and underscores.
     
     
     """
     ...
 
 @typing.overload
 def trigger(*, event: typing.Union[str, typing.Dict[str, typing.Any], None] = None, events: typing.List[typing.Union[str, typing.Dict[str, typing.Any]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
@@ -1619,63 +1534,14 @@
         and the value is the version to use.
     python : str, optional, default: None
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     """
     ...
 
-@typing.overload
-def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
-@typing.overload
-def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
-    ...
-
-def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
-    """
-    Specifies the times when the flow should be run when running on a
-    production scheduler.
-    
-    Parameters
-    ----------
-    hourly : bool, default False
-        Run the workflow hourly.
-    daily : bool, default True
-        Run the workflow daily.
-    weekly : bool, default False
-        Run the workflow weekly.
-    cron : str, optional, default None
-        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
-        specified by this expression.
-    timezone : str, optional, default None
-        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
-        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
-    """
-    ...
-
 def airflow_s3_key_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, bucket_key: typing.Union[str, typing.List[str]], bucket_name: str, wildcard_match: bool, aws_conn_id: str, verify: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     The `@airflow_s3_key_sensor` decorator attaches a Airflow [S3KeySensor](https://airflow.apache.org/docs/apache-airflow-providers-amazon/stable/_api/airflow/providers/amazon/aws/sensors/s3/index.html#airflow.providers.amazon.aws.sensors.s3.S3KeySensor)
     before the start step of the flow. This decorator only works when a flow is scheduled on Airflow
     and is compiled using `airflow create`. More than one `@airflow_s3_key_sensor` can be
     added as a flow decorators. Adding more than one decorator will ensure that `start` step
     starts only after all sensors finish.
@@ -1710,56 +1576,14 @@
     aws_conn_id : str
         a reference to the s3 connection on Airflow. (Default: None)
     verify : bool
         Whether or not to verify SSL certificates for S3 connection. (Default: None)
     """
     ...
 
-def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
-    """
-    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
-    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
-    
-    Parameters
-    ----------
-    timeout : int
-        Time, in seconds before the task times out and fails. (Default: 3600)
-    poke_interval : int
-        Time in seconds that the job should wait in between each try. (Default: 60)
-    mode : str
-        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
-    exponential_backoff : bool
-        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
-    pool : str
-        the slot pool this task should run in,
-        slot pools are a way to limit concurrency for certain tasks. (Default:None)
-    soft_fail : bool
-        Set to true to mark the task as SKIPPED on failure. (Default: False)
-    name : str
-        Name of the sensor on Airflow
-    description : str
-        Description of sensor in the Airflow UI
-    external_dag_id : str
-        The dag_id that contains the task you want to wait for.
-    external_task_ids : List[str]
-        The list of task_ids that you want to wait for.
-        If None (default value) the sensor waits for the DAG. (Default: None)
-    allowed_states : List[str]
-        Iterable of allowed states, (Default: ['success'])
-    failed_states : List[str]
-        Iterable of failed or dis-allowed states. (Default: None)
-    execution_delta : datetime.timedelta
-        time difference with the previous execution to look at,
-        the default is the same logical date as the current task or DAG. (Default: None)
-    check_existence: bool
-        Set to True to check if the external task exists or check if
-        the DAG to wait for exists. (Default: True)
-    """
-    ...
-
 @typing.overload
 def conda_base(*, packages: typing.Dict[str, str] = {}, libraries: typing.Dict[str, str] = {}, python: typing.Optional[str] = None, disabled: bool = False) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
     Specifies the Conda environment for all steps of the flow.
     
     Use `@conda_base` to set common libraries required by all
     steps and use `@conda` to specify step-specific additions.
@@ -1801,29 +1625,205 @@
         Version of Python to use, e.g. '3.7.4'. A default value of None implies
         that the version used will correspond to the version of the Python interpreter used to start the run.
     disabled : bool, default False
         If set to True, disables Conda.
     """
     ...
 
-def project(*, name: str) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+@typing.overload
+def trigger_on_finish(*, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
     """
-    Specifies what flows belong to the same project.
+    Specifies the flow(s) that this flow depends on.
     
-    A project-specific namespace is created for all flows that
-    use the same `@project(name)`.
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
     
     Parameters
     ----------
-    name : str
-        Project name. Make sure that the name is unique amongst all
-        projects that use the same production scheduler. The name may
-        contain only lowercase alphanumeric characters and underscores.
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def trigger_on_finish(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def trigger_on_finish(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, flow: typing.Union[str, typing.Dict[str, str], None] = None, flows: typing.List[typing.Union[str, typing.Dict[str, str]]] = [], options: typing.Dict[str, typing.Any] = {}):
+    """
+    Specifies the flow(s) that this flow depends on.
+    
+    ```
+    @trigger_on_finish(flow='FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['FooFlow', 'BarFlow'])
+    ```
+    This decorator respects the @project decorator and triggers the flow
+    when upstream runs within the same namespace complete successfully
+    
+    Additionally, you can specify project aware upstream flow dependencies
+    by specifying the fully qualified project_flow_name.
+    ```
+    @trigger_on_finish(flow='my_project.branch.my_branch.FooFlow')
+    ```
+    or
+    ```
+    @trigger_on_finish(flows=['my_project.branch.my_branch.FooFlow', 'BarFlow'])
+    ```
+    
+    You can also specify just the project or project branch (other values will be
+    inferred from the current project or project branch):
+    ```
+    @trigger_on_finish(flow={"name": "FooFlow", "project": "my_project", "project_branch": "branch"})
+    ```
+    
+    Note that `branch` is typically one of:
+      - `prod`
+      - `user.bob`
+      - `test.my_experiment`
+      - `prod.staging`
+    
+    Parameters
+    ----------
+    flow : Union[str, Dict[str, str]], optional, default None
+        Upstream flow dependency for this flow.
+    flows : List[Union[str, Dict[str, str]]], default []
+        Upstream flow dependencies for this flow.
+    options : Dict[str, Any], default {}
+        Backend-specific configuration for tuning eventing behavior.
+    
+    
+    """
+    ...
+
+@typing.overload
+def schedule(*, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
     
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+@typing.overload
+def schedule(f: typing.Type[FlowSpecDerived]) -> typing.Type[FlowSpecDerived]:
+    ...
+
+def schedule(f: typing.Optional[typing.Type[FlowSpecDerived]] = None, *, hourly: bool = False, daily: bool = True, weekly: bool = False, cron: typing.Optional[str] = None, timezone: typing.Optional[str] = None):
+    """
+    Specifies the times when the flow should be run when running on a
+    production scheduler.
     
+    Parameters
+    ----------
+    hourly : bool, default False
+        Run the workflow hourly.
+    daily : bool, default True
+        Run the workflow daily.
+    weekly : bool, default False
+        Run the workflow weekly.
+    cron : str, optional, default None
+        Run the workflow at [a custom Cron schedule](https://docs.aws.amazon.com/eventbridge/latest/userguide/scheduled-events.html#cron-expressions)
+        specified by this expression.
+    timezone : str, optional, default None
+        Timezone on which the schedule runs (default: None). Currently supported only for Argo workflows,
+        which accepts timezones in [IANA format](https://nodatime.org/TimeZones).
+    """
+    ...
+
+def airflow_external_task_sensor(*, timeout: int, poke_interval: int, mode: str, exponential_backoff: bool, pool: str, soft_fail: bool, name: str, description: str, external_dag_id: str, external_task_ids: typing.List[str], allowed_states: typing.List[str], failed_states: typing.List[str], execution_delta: "datetime.timedelta", check_existence: bool) -> typing.Callable[[typing.Type[FlowSpecDerived]], typing.Type[FlowSpecDerived]]:
+    """
+    The `@airflow_external_task_sensor` decorator attaches a Airflow [ExternalTaskSensor](https://airflow.apache.org/docs/apache-airflow/stable/_api/airflow/sensors/external_task/index.html#airflow.sensors.external_task.ExternalTaskSensor) before the start step of the flow.
+    This decorator only works when a flow is scheduled on Airflow and is compiled using `airflow create`. More than one `@airflow_external_task_sensor` can be added as a flow decorators. Adding more than one decorator will ensure that `start` step starts only after all sensors finish.
+    
+    Parameters
+    ----------
+    timeout : int
+        Time, in seconds before the task times out and fails. (Default: 3600)
+    poke_interval : int
+        Time in seconds that the job should wait in between each try. (Default: 60)
+    mode : str
+        How the sensor operates. Options are: { poke | reschedule }. (Default: "poke")
+    exponential_backoff : bool
+        allow progressive longer waits between pokes by using exponential backoff algorithm. (Default: True)
+    pool : str
+        the slot pool this task should run in,
+        slot pools are a way to limit concurrency for certain tasks. (Default:None)
+    soft_fail : bool
+        Set to true to mark the task as SKIPPED on failure. (Default: False)
+    name : str
+        Name of the sensor on Airflow
+    description : str
+        Description of sensor in the Airflow UI
+    external_dag_id : str
+        The dag_id that contains the task you want to wait for.
+    external_task_ids : List[str]
+        The list of task_ids that you want to wait for.
+        If None (default value) the sensor waits for the DAG. (Default: None)
+    allowed_states : List[str]
+        Iterable of allowed states, (Default: ['success'])
+    failed_states : List[str]
+        Iterable of failed or dis-allowed states. (Default: None)
+    execution_delta : datetime.timedelta
+        time difference with the previous execution to look at,
+        the default is the same logical date as the current task or DAG. (Default: None)
+    check_existence: bool
+        Set to True to check if the external task exists or check if
+        the DAG to wait for exists. (Default: True)
     """
     ...
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/cards.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/cards.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.209571                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.937079                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.basic
-    import typing
-    import metaflow.plugins.cards.card_client
     import metaflow
-    import metaflow.plugins.cards.card_modules.card
+    import typing
+    import metaflow.plugins.cards.card_modules.basic
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
+    import metaflow.plugins.cards.card_client
 
 def get_cards(task: typing.Union[str, "metaflow.Task"], id: typing.Optional[str] = None, type: typing.Optional[str] = None, follow_resumed: bool = True) -> metaflow.plugins.cards.card_client.CardContainer:
     """
     Get cards related to a `Task`.
     
     Note that `get_cards` resolves the cards contained by the task, but it doesn't actually
     retrieve them from the datastore. Actual card contents are retrieved lazily either when
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/cli.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.216434                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.943055                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/client/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/client/__init__.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.212765                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.940233                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.client.core
+    import datetime
     import typing
     import metaflow.events
-    import datetime
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/client/core.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/client/core.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.195327                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.922677                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow
+    import metaflow.metaflow_current
+    import typing
+    import metaflow.exception
     import metaflow.events
-    import tarfile
     import metaflow.client.core
-    import typing
     import datetime
-    import metaflow.exception
-    import metaflow
-    import metaflow.metaflow_current
+    import tarfile
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/client/filecache.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/client/filecache.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.217495                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.944136                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/clone_util.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/clone_util.pyi`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.213254                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.940759                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaDatum(tuple, metaclass=type):
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/events.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/events.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.197821                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.925117                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
     import metaflow
+    import metaflow.events
 
 TYPE_CHECKING: bool
 
 class MetaflowEvent(tuple, metaclass=type):
     @staticmethod
     def __new__(_cls, name, id, timestamp, type):
         """
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/exception.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/exception.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.185579                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.912556                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/flowspec.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/flowspec.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.197093                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.924344                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.unbounded_foreach
     import metaflow.datastore.inputs
     import typing
-    import metaflow.parameters
-    import metaflow.unbounded_foreach
     import metaflow.exception
+    import metaflow.parameters
 
 class DelayedEvaluationParameter(object, metaclass=type):
     def __init__(self, name, field, fun):
         ...
     def __call__(self, return_str = False):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/includefile.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/includefile.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.207375                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.934714                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
-    import metaflow._vendor.click.types
     import typing
-    import metaflow.parameters
     import io
+    import metaflow.parameters
+    import metaflow._vendor.click.types
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/metadata/metadata.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/metadata/metadata.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.238983                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.966396                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metadata.metadata
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/metaflow_config.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/metaflow_config.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.186894                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.913832                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/metaflow_current.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/metaflow_current.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.298833                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.023084                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
-    import metaflow.plugins.cards.component_serializer
-    import typing
     import metaflow
     import metaflow.metaflow_current
+    import metaflow.plugins.cards.component_serializer
+    import typing
+    import metaflow.events
 
 TYPE_CHECKING: bool
 
 TEMPDIR: str
 
 class Parallel(tuple, metaclass=type):
     @staticmethod
@@ -238,27 +238,14 @@
         Returns
         -------
         CardComponentCollector
             The or one of the cards attached to this step.
         """
         ...
     @property
-    def trigger(self) -> "metaflow.events.Trigger":
-        """
-        (only in the presence of the @trigger_on_finish, or @trigger decorators)
-        
-        Returns `Trigger` if the current run is triggered by an event
-        
-        Returns
-        -------
-        Trigger
-            `Trigger` if triggered by an event
-        """
-        ...
-    @property
     def project_name(self) -> str:
         """
         (only in the presence of the @project decorator)
         
         The name of the project assigned to this flow, i.e. `X` in `@project(name=X)`.
         
         Returns
@@ -317,11 +304,24 @@
         
         Returns
         -------
         bool
             True if the flow is deployed with `--production`.
         """
         ...
+    @property
+    def trigger(self) -> "metaflow.events.Trigger":
+        """
+        (only in the presence of the @trigger, or @trigger_on_finish decorators)
+        
+        Returns `Trigger` if the current run is triggered by an event
+        
+        Returns
+        -------
+        Trigger
+            `Trigger` if triggered by an event
+        """
+        ...
     ...
 
 current: Current
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/mflog/mflog.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/mflog/mflog.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.239385                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.966795                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import datetime
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/multicore_utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/multicore_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.187410                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.914344                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import typing
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/parameters.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/parameters.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.188886                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.915738                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
-    import metaflow.exception
     import metaflow._vendor.click.types
+    import metaflow.exception
     import typing
 
 class ParameterFieldFailed(metaflow.exception.MetaflowException, metaclass=type):
     def __init__(self, name, field):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.199796                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.927203                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.unbounded_foreach
+    import metaflow.plugins.cards.card_modules.card
 
 CLIS_DESC: list
 
 class InternalTestUnboundedForeachInput(metaflow.unbounded_foreach.UnboundedForeachInput, metaclass=type):
     def __init__(self, iterable):
         ...
     def __iter__(self):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.260336                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.980715                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow._vendor.click.types
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.261540                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.981934                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
     import metaflow.exception
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.257933                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.978279                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/airflow_utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/airflow_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.257468                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.977803                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 TASK_ID_XCOM_KEY: str
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/exception.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/exception.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.258235                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.978549                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/__init__.pyi`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.258512                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.978822                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.airflow.sensors.base_sensor
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/base_sensor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.291407                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.007423                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/external_task_sensor.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.292247                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.007905                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/airflow/sensors/s3_sensor.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.293028                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.008335                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.exception
     import metaflow.plugins.airflow.sensors.base_sensor
+    import metaflow.exception
+    import metaflow.decorators
 
 class AirflowSensorDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     def serialize_operator_args(self):
         """
         Subclasses will parse the decorator arguments to
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.268540                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.995703                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_events.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_events.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.266878                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.993898                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.273966                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.001234                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
     import metaflow._vendor.click.types
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.275973                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.003195                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
     import metaflow.metaflow_current
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/argo/argo_workflows_decorator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.267844                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.994990                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.events
+    import metaflow
     import metaflow.metaflow_current
     import metaflow.decorators
-    import metaflow
+    import metaflow.events
 
 current: metaflow.metaflow_current.Current
 
 class Trigger(object, metaclass=type):
     def __init__(self, _meta = None):
         ...
     @classmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/aws_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.240796                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.982847                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 cached_aws_sandbox_creds: None
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/aws_utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/aws_utils.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.240410                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.982460                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.281603                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.011553                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_cli.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.283263                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.013252                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.280344                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.010263                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/batch/batch_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.282555                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.012478                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ResourcesDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     ...
 
 def get_run_time_limit_for_task(step_decos):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/secrets_manager/aws_secrets_manager_secrets_provider.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.289811                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.019609                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
-    import metaflow.exception
     import metaflow.plugins.secrets
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/dynamo_db_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.283530                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.013514                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 SFN_DYNAMO_DB_TABLE: None
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/event_bridge_client.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.284816                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.014547                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class EventBridgeClient(object, metaclass=type):
     def __init__(self, name):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/schedule_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/environment_decorator.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.284205                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.945820                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class ScheduleDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.287731                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.017517                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_cli.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.289304                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.019097                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.parameters
     import metaflow.metaflow_current
-    import metaflow.exception
     import metaflow.decorators
+    import metaflow.exception
 
 JSONType: metaflow.parameters.JSONTypeClass
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_client.pyi`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.285195                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.014929                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 AWS_SANDBOX_ENABLED: bool
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/aws/step_functions/step_functions_decorator.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.284007                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.014009                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/azure_exceptions.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_exceptions.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.277028                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.004706                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/azure_utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/azure_utils.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.277639                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.005224                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/blob_service_client_factory.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.278063                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.005646                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/azure/includefile_support.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/azure/includefile_support.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.232579                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.959997                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_cli.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.252132                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.975418                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import typing
+    import metaflow.exception
     import metaflow.client.core
     import datetime
     import metaflow.parameters
-    import typing
-    import metaflow.exception
 
 class Task(metaflow.client.core.MetaflowObject, metaclass=type):
     def __init__(self, *args, **kwargs):
         ...
     @property
     def metadata(self) -> typing.List[metaflow.client.core.Metadata]:
         """
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_client.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.234529                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.961948                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow
     import metaflow.plugins.cards.card_client
     import metaflow.exception
-    import metaflow
 
 TYPE_CHECKING: bool
 
 CARD_SUFFIX: str
 
 def resolve_paths_from_task(flow_datastore, pathspec = None, type = None, hash = None, card_id = None):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_creator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_creator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.246927                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.970143                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_datastore.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_datastore.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.248757                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.971977                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_decorator.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.247823                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.971043                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class CardComponentCollector(object, metaclass=type):
     def __init__(self, logger = None, card_creator = None):
         ...
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.244100                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.967391                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/basic.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/basic.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.227664                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.955015                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow
     import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.basic
-    import metaflow
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/card.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/card.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.235027                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.962441                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/__init__.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.290671                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.006776                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def main(template, data = None, **kwargs):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/main.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.296025                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.021710                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def render(template = "", data = {}, partials_path = ".", partials_ext = "mustache", partials_dict = {}, padding = "", def_ldel = "{{", def_rdel = "}}", scopes = None, warn = False, keep = False):
     """
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/renderer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.295270                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.021255                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 linesep: str
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/chevron/tokenizer.pyi`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.294430                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.020783                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class ChevronError(SyntaxError, metaclass=type):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/components.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/components.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.237459                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.964790                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import typing
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.basic
 
 class LogComponent(metaflow.plugins.cards.card_modules.basic.DefaultComponent, metaclass=type):
     def __init__(self, data = None):
         ...
     def render(self):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/convert_to_native_type.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.278542                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.006095                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class TypeResolvedObject(tuple, metaclass=type):
     @staticmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/renderer_tools.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.278767                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.006326                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.cards.card_modules.basic
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_modules/test_cards.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.229120                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.956478                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow
+    import metaflow.plugins.cards.card_modules.card
 
 class MetaflowCard(object, metaclass=type):
     def __init__(self, options = {}, components = [], graph = None):
         ...
     def render(self, task: "metaflow.Task") -> str:
         """
         Produce custom card contents in HTML.
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/card_resolver.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/card_resolver.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.249366                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.972610                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class CardDatastore(object, metaclass=type):
     @classmethod
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/component_serializer.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/component_serializer.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.246624                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.969836                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.cards.card_modules.card
     import metaflow.plugins.cards.card_modules.components
+    import metaflow.plugins.cards.card_modules.card
     import metaflow.exception
     import metaflow.plugins.cards.card_modules.basic
 
 class MetaflowCardComponent(object, metaclass=type):
     @property
     def component_id(self):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/cards/exception.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/cards/exception.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.244799                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.968100                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/catch_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/catch_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.219919                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.950078                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
     import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.221954                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.948860                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/local.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/local.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.231994                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.959424                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/__init__.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.243499                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.985692                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.plugins.datatools.s3.s3
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.203789                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.931185                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.plugins.datatools.s3.s3
     import metaflow.datastore.inputs
+    import metaflow.plugins.datatools.s3.s3
+    import metaflow.metaflow_current
     import typing
     import metaflow.exception
     import io
-    import metaflow.metaflow_current
 
 TYPE_CHECKING: bool
 
 class FlowSpec(object, metaclass=type):
     def __init__(self, use_cli = True):
         """
         Construct a FlowSpec
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3tail.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3tail.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.290268                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.020024                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 def aws_retry(f):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/datatools/s3/s3util.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/datatools/s3/s3util.pyi`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.231340                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.958770                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/debug_logger.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_logger.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.224705                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.952171                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.event_logger
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/debug_monitor.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/debug_monitor.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.224988                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.952458                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.monitor
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/environment_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/retry_decorator.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,28 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.218336                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.949464                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
 
-class EnvironmentDecorator(metaflow.decorators.StepDecorator, metaclass=type):
-    def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
+class MetaflowException(Exception, metaclass=type):
+    def __init__(self, msg = "", lineno = None):
+        ...
+    def __str__(self):
+        ...
+    ...
+
+MAX_ATTEMPTS: int
+
+class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
+        ...
+    def step_task_retry_count(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/events_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/project_decorator.pyi`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.223399                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.950856                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
-
-current: metaflow.metaflow_current.Current
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
-        ...
-    ...
+current: metaflow.metaflow_current.Current
+
+VALID_NAME_RE: str
+
+VALID_NAME_LEN: int
 
-class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
+def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
+    ...
+
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/frameworks/pytorch.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/frameworks/pytorch.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.239878                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.003673                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.plugins.parallel_decorator
+    import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class ParallelDecorator(metaflow.decorators.StepDecorator, metaclass=type):
     def __init__(self, attributes = None, statically_defined = False):
         ...
     def runtime_step_cli(self, cli_args, retry_count, max_user_code_retries, ubf_context):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/gs_exceptions.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/__init__.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,22 +1,18 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.276388                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.949148                                        #
 ##################################################################################
 
 from __future__ import annotations
 
-import typing
-if typing.TYPE_CHECKING:
-    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
-    ...
+MAGIC_FILE: str
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/gs_utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_utils.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.276763                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.004422                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/gcp/includefile_support.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/includefile_support.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.233158                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.960608                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.264313                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.991316                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_current
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_cli.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.266399                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.993416                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.exception
+    import metaflow.decorators
     import metaflow._vendor.click.types
 
 class JSONTypeClass(metaflow._vendor.click.types.ParamType, metaclass=type):
     def convert(self, value, param, ctx):
         ...
     def __str__(self):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_client.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.263089                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.990192                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_decorator.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.265400                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.992398                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
-    import metaflow.metaflow_current
     import metaflow.exception
+    import metaflow.metaflow_current
+    import metaflow.decorators
 
 current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/kubernetes/kubernetes_job.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.262459                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.989578                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/parallel_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/parallel_decorator.pyi`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.219307                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.946493                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/project_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/events_decorator.pyi`

 * *Files 23% similar despite different names*

```diff
@@ -1,36 +1,34 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.223800                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.951252                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.metaflow_current
+    import metaflow.decorators
+
+current: metaflow.metaflow_current.Current
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-current: metaflow.metaflow_current.Current
-
-VALID_NAME_RE: str
-
-VALID_NAME_LEN: int
+class TriggerDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
+        ...
+    ...
 
-class ProjectDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
-    def flow_init(self, flow, graph, environment, flow_datastore, metadata, logger, echo, options):
+class TriggerOnFinishDecorator(metaflow.decorators.FlowDecorator, metaclass=type):
+    def flow_init(self, flow_name, graph, environment, flow_datastore, metadata, logger, echo, options):
         ...
     def get_top_level_options(self):
         ...
     ...
 
-def format_name(flow_name, project_name, deploy_prod, given_branch, user_name):
-    ...
-
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/pylint_wrapper.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,18 +1,31 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.222634                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.941612                                        #
 ##################################################################################
 
 from __future__ import annotations
 
+import typing
+if typing.TYPE_CHECKING:
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAGIC_FILE: str
+class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class PyLint(object, metaclass=type):
+    def __init__(self, fname):
+        ...
+    def has_pylint(self):
+        ...
+    def run(self, logger = None, warnings = False, pylint_config = []):
+        ...
+    ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/conda_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_decorator.pyi`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.254228                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.986763                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/conda_environment.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/conda_environment.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.255715                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.988133                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_environment
     import abc
     import metaflow.exception
-    import metaflow.metaflow_environment
     import io
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/pypi_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_decorator.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.253521                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.986033                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/pypi_environment.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/pypi_environment.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.256208                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.988664                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.metaflow_environment
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/pypi/utils.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/pypi/utils.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.254604                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.987137                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/resources_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/resources_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.218780                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.946635                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/retry_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/timeout_decorator.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,39 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.218639                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.947332                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
+    import metaflow.exception
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-MAX_ATTEMPTS: int
+UBF_CONTROL: str
 
-class RetryDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+class TimeoutException(metaflow.exception.MetaflowException, metaclass=type):
+    ...
+
+class TimeoutDecorator(metaflow.decorators.StepDecorator, metaclass=type):
+    def __init__(self, *args, **kwargs):
+        ...
     def step_init(self, flow, graph, step, decos, environment, flow_datastore, logger):
         ...
-    def step_task_retry_count(self):
+    def task_pre_step(self, step_name, task_datastore, metadata, run_id, task_id, flow, graph, retry_count, max_user_code_retries, ubf_context, inputs):
         ...
+    def task_post_step(self, step_name, flow, graph, retry_count, max_user_code_retries):
+        ...
+    ...
+
+def get_run_time_limit_for_task(step_decos):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/__init__.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,21 +1,30 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.222391                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.976503                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
+    import metaflow.plugins.secrets
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
         ...
     ...
 
+class InlineSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
+    def get_secret_as_dict(self, secret_id, options = {}, role = None):
+        """
+        Intended to be used for testing purposes only.
+        """
+        ...
+    ...
+
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/inline_secrets_provider.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/__init__.pyi`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,21 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.253224                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.946073                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import abc
-    import metaflow.plugins.secrets
 
 class SecretsProvider(abc.ABC, metaclass=abc.ABCMeta):
     def get_secret_as_dict(self, secret_id, options = {}, role = None) -> typing.Dict[str, str]:
         """
         Retrieve the secret from secrets backend, and return a dictionary of
         environment variables.
         """
         ...
     ...
 
-class InlineSecretsProvider(metaflow.plugins.secrets.SecretsProvider, metaclass=abc.ABCMeta):
-    def get_secret_as_dict(self, secret_id, options = {}, role = None):
-        """
-        Intended to be used for testing purposes only.
-        """
-        ...
-    ...
-
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/secrets/secrets_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/secrets/secrets_decorator.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.252933                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.976213                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.decorators
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/storage_executor.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/storage_executor.pyi`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.224310                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.951779                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/tag_cli.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/tag_cli.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.230840                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.958278                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
+    import metaflow.metaflow_current
+    import metaflow.exception
     import metaflow.events
     import metaflow.client.core
     import datetime
-    import metaflow.exception
-    import metaflow.metaflow_current
 
 def namespace(ns: typing.Optional[str]) -> typing.Optional[str]:
     """
     Switch namespace to the one provided.
     
     This call has a global effect. No objects outside this namespace
     will be accessible. To access all objects regardless of namespaces,
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/test_unbounded_foreach_decorator.pyi`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.218145                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.945489                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
-    import metaflow.decorators
     import metaflow.unbounded_foreach
+    import metaflow.decorators
 
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/procpoll.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/procpoll.pyi`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.214643                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.941266                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.procpoll
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/pylint_wrapper.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/plugins/gcp/gs_exceptions.pyi`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.214997                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:01.004068                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
@@ -13,19 +13,10 @@
 class MetaflowException(Exception, metaclass=type):
     def __init__(self, msg = "", lineno = None):
         ...
     def __str__(self):
         ...
     ...
 
-class PyLintWarn(metaflow.exception.MetaflowException, metaclass=type):
-    ...
-
-class PyLint(object, metaclass=type):
-    def __init__(self, fname):
-        ...
-    def has_pylint(self):
-        ...
-    def run(self, logger = None, warnings = False, pylint_config = []):
-        ...
+class MetaflowGSPackageError(metaflow.exception.MetaflowException, metaclass=type):
     ...
```

### Comparing `metaflow-stubs-2.11.8/metaflow-stubs/tagging_util.pyi` & `metaflow-stubs-2.11.9/metaflow-stubs/tagging_util.pyi`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ##################################################################################
 #                       Auto-generated Metaflow stub file                        #
-# MF version: 2.11.8                                                             #
-# Generated on 2024-03-29T12:37:59.189268                                        #
+# MF version: 2.11.9                                                             #
+# Generated on 2024-03-29T22:28:00.916120                                        #
 ##################################################################################
 
 from __future__ import annotations
 
 import typing
 if typing.TYPE_CHECKING:
     import metaflow.exception
```

### Comparing `metaflow-stubs-2.11.8/metaflow_stubs.egg-info/PKG-INFO` & `metaflow-stubs-2.11.9/metaflow_stubs.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metaflow-stubs
-Version: 2.11.8
+Version: 2.11.9
 Summary: Metaflow Stubs: Stubs for the metaflow package
 Author: Metaflow Developers
 Author-email: help@metaflow.org
 License: Apache Software License
 Project-URL: Source, https://github.com/Netflix/metaflow
 Project-URL: Issues, https://github.com/Netflix/metaflow/issues
 Project-URL: Documentation, https://docs.metaflow.org
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.7.0
 Description-Content-Type: text/markdown
-Requires-Dist: metaflow==2.11.8
+Requires-Dist: metaflow==2.11.9
 
 # Metaflow Stubs
 
 This package contains stub files for `metaflow` and thus offers type hints for various editors (such as `VSCode`) and language servers (such as `Pylance`).
 
 ## Installation
```

### Comparing `metaflow-stubs-2.11.8/metaflow_stubs.egg-info/SOURCES.txt` & `metaflow-stubs-2.11.9/metaflow_stubs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metaflow-stubs-2.11.8/setup.py` & `metaflow-stubs-2.11.9/setup.py`

 * *Files identical despite different names*

