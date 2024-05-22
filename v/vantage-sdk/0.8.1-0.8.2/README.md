# Comparing `tmp/vantage_sdk-0.8.1.tar.gz` & `tmp/vantage_sdk-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vantage_sdk-0.8.1.tar", max compression
+gzip compressed data, was "vantage_sdk-0.8.2.tar", max compression
```

## Comparing `vantage_sdk-0.8.1.tar` & `vantage_sdk-0.8.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.8.1/LICENSE
--rw-r--r--   0        0        0     3974 2024-05-14 15:00:04.643283 vantage_sdk-0.8.1/README.md
--rw-r--r--   0        0        0     2551 2024-05-21 16:24:37.163466 vantage_sdk-0.8.1/docs/api.md
--rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163636 vantage_sdk-0.8.1/docs/index.md
--rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163767 vantage_sdk-0.8.1/docs/installation.md
--rw-r--r--   0        0        0        9 2024-05-21 16:24:37.163900 vantage_sdk-0.8.1/docs/usage.md
--rw-r--r--   0        0        0     3017 2024-05-21 16:24:37.166299 vantage_sdk-0.8.1/pyproject.toml
--rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.8.1/tests/__init__.py
--rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.8.1/tests/data/documents.jsonl
--rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.8.1/tests/data/hello_world.parquet
--rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.8.1/tests/integration_tests/.env-example
--rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.8.1/tests/integration_tests/__init__.py
--rw-r--r--   0        0        0    10571 2024-05-14 15:00:04.643899 vantage_sdk-0.8.1/tests/integration_tests/conftest.py
--rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.8.1/tests/integration_tests/test_account.py
--rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.8.1/tests/integration_tests/test_api_keys.py
--rw-r--r--   0        0        0    12709 2024-05-14 15:00:04.644178 vantage_sdk-0.8.1/tests/integration_tests/test_collection.py
--rw-r--r--   0        0        0     4219 2024-05-14 15:00:04.644424 vantage_sdk-0.8.1/tests/integration_tests/test_documents.py
--rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.8.1/tests/integration_tests/test_search.py
--rw-r--r--   0        0        0      671 2024-05-21 16:24:37.166553 vantage_sdk-0.8.1/vantage_sdk/__init__.py
--rw-r--r--   0        0        0    66145 2024-05-21 16:24:37.167025 vantage_sdk-0.8.1/vantage_sdk/client.py
--rw-r--r--   0        0        0      239 2024-05-14 15:00:04.645361 vantage_sdk-0.8.1/vantage_sdk/config.py
--rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.8.1/vantage_sdk/core/__init__.py
--rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.8.1/vantage_sdk/core/base.py
--rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.8.1/vantage_sdk/core/exceptions.py
--rw-r--r--   0        0        0     4268 2024-05-14 15:00:04.645589 vantage_sdk-0.8.1/vantage_sdk/core/http/__init__.py
--rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.8.1/vantage_sdk/core/http/api/__init__.py
--rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.8.1/vantage_sdk/core/http/api/account_management_api.py
--rw-r--r--   0        0        0    75134 2024-05-14 15:00:04.645955 vantage_sdk-0.8.1/vantage_sdk/core/http/api/collection_management_api.py
--rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.8.1/vantage_sdk/core/http/api/documents_api.py
--rw-r--r--   0        0        0    57753 2024-05-14 15:00:04.646292 vantage_sdk-0.8.1/vantage_sdk/core/http/api/external_api_keys_api.py
--rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.8.1/vantage_sdk/core/http/api/search_api.py
--rw-r--r--   0        0        0    22624 2024-05-14 15:00:04.646500 vantage_sdk-0.8.1/vantage_sdk/core/http/api/vantage_api_keys_api.py
--rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.8.1/vantage_sdk/core/http/api_client.py
--rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.8.1/vantage_sdk/core/http/api_response.py
--rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.8.1/vantage_sdk/core/http/configuration.py
--rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.8.1/vantage_sdk/core/http/exceptions.py
--rw-r--r--   0        0        0     3384 2024-05-14 15:00:04.646724 vantage_sdk-0.8.1/vantage_sdk/core/http/models/__init__.py
--rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account.py
--rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_modifiable.py
--rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_read_only.py
--rw-r--r--   0        0        0     7946 2024-05-14 15:00:04.646949 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection.py
--rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_immutable.py
--rw-r--r--   0        0        0     4445 2024-05-14 15:00:04.647162 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_modifiable.py
--rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_read_only.py
--rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_upload_url.py
--rw-r--r--   0        0        0     6297 2024-05-14 15:00:04.647434 vantage_sdk-0.8.1/vantage_sdk/core/http/models/create_collection_request.py
--rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.8.1/vantage_sdk/core/http/models/document_batch.py
--rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.8.1/vantage_sdk/core/http/models/embedding_search_query.py
--rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key.py
--rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_modifiable.py
--rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_read_only.py
--rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties.py
--rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_collection.py
--rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
--rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_filter.py
--rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_pagination.py
--rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_sort.py
--rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these.py
--rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these_these_inner.py
--rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_these_query.py
--rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_this_query.py
--rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result.py
--rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result_results_inner.py
--rw-r--r--   0        0        0     3445 2024-05-14 15:00:04.647571 vantage_sdk-0.8.1/vantage_sdk/core/http/models/secondary_external_account.py
--rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.8.1/vantage_sdk/core/http/models/semantic_search_query.py
--rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.8.1/vantage_sdk/core/http/models/vantage_api_key.py
--rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.8.1/vantage_sdk/core/http/models/weighted_field_values.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.8.1/vantage_sdk/core/http/py.typed
--rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.8.1/vantage_sdk/core/http/rest.py
--rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.8.1/vantage_sdk/core/management/__init__.py
--rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.8.1/vantage_sdk/core/management/management.py
--rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.8.1/vantage_sdk/core/search/__init__.py
--rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.8.1/vantage_sdk/core/search/search.py
--rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.8.1/vantage_sdk/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.8.1/vantage_sdk/model/__init__.py
--rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.8.1/vantage_sdk/model/account.py
--rw-r--r--   0        0        0     2563 2024-05-14 15:00:04.647772 vantage_sdk-0.8.1/vantage_sdk/model/collection.py
--rw-r--r--   0        0        0     1670 2024-05-14 15:00:04.647963 vantage_sdk-0.8.1/vantage_sdk/model/document.py
--rw-r--r--   0        0        0      910 2024-05-14 15:00:04.648235 vantage_sdk-0.8.1/vantage_sdk/model/keys.py
--rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.8.1/vantage_sdk/model/search.py
--rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 vantage_sdk-0.8.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-22 15:20:18.752197 vantage_sdk-0.8.2/LICENSE
+-rw-r--r--   0        0        0     3974 2024-05-22 17:47:33.287400 vantage_sdk-0.8.2/README.md
+-rw-r--r--   0        0        0     2552 2024-05-22 17:47:33.288287 vantage_sdk-0.8.2/docs/api.md
+-rw-r--r--   0        0        0        9 2024-05-22 17:47:33.288430 vantage_sdk-0.8.2/docs/index.md
+-rw-r--r--   0        0        0        9 2024-05-22 17:47:33.288529 vantage_sdk-0.8.2/docs/installation.md
+-rw-r--r--   0        0        0        9 2024-05-22 17:47:33.288619 vantage_sdk-0.8.2/docs/usage.md
+-rw-r--r--   0        0        0     3017 2024-05-22 18:09:56.412216 vantage_sdk-0.8.2/pyproject.toml
+-rw-r--r--   0        0        0       41 2024-01-22 15:20:18.753683 vantage_sdk-0.8.2/tests/__init__.py
+-rw-r--r--   0        0        0    70399 2024-04-25 01:26:48.217409 vantage_sdk-0.8.2/tests/data/documents.jsonl
+-rw-r--r--   0        0        0     2971 2024-04-25 01:26:48.217491 vantage_sdk-0.8.2/tests/data/hello_world.parquet
+-rw-r--r--   0        0        0      777 2024-04-25 01:26:48.217595 vantage_sdk-0.8.2/tests/integration_tests/.env-example
+-rw-r--r--   0        0        0        0 2024-01-26 19:13:09.644916 vantage_sdk-0.8.2/tests/integration_tests/__init__.py
+-rw-r--r--   0        0        0    10571 2024-05-22 17:47:33.291290 vantage_sdk-0.8.2/tests/integration_tests/conftest.py
+-rw-r--r--   0        0        0     3027 2024-04-25 01:26:48.217838 vantage_sdk-0.8.2/tests/integration_tests/test_account.py
+-rw-r--r--   0        0        0    10983 2024-04-25 01:26:48.217894 vantage_sdk-0.8.2/tests/integration_tests/test_api_keys.py
+-rw-r--r--   0        0        0    12709 2024-05-22 17:47:33.291581 vantage_sdk-0.8.2/tests/integration_tests/test_collection.py
+-rw-r--r--   0        0        0     4219 2024-05-22 17:47:33.291792 vantage_sdk-0.8.2/tests/integration_tests/test_documents.py
+-rw-r--r--   0        0        0     9132 2024-04-25 01:26:48.218158 vantage_sdk-0.8.2/tests/integration_tests/test_search.py
+-rw-r--r--   0        0        0      671 2024-05-22 18:09:56.412449 vantage_sdk-0.8.2/vantage_sdk/__init__.py
+-rw-r--r--   0        0        0    66101 2024-05-22 18:09:56.412860 vantage_sdk-0.8.2/vantage_sdk/client.py
+-rw-r--r--   0        0        0      239 2024-05-14 15:00:04.645361 vantage_sdk-0.8.2/vantage_sdk/config.py
+-rw-r--r--   0        0        0       43 2024-04-25 01:26:48.218648 vantage_sdk-0.8.2/vantage_sdk/core/__init__.py
+-rw-r--r--   0        0        0     6471 2024-04-25 01:26:48.218733 vantage_sdk-0.8.2/vantage_sdk/core/base.py
+-rw-r--r--   0        0        0     1628 2024-04-25 01:26:48.218805 vantage_sdk-0.8.2/vantage_sdk/core/exceptions.py
+-rw-r--r--   0        0        0     4268 2024-05-14 15:00:04.645589 vantage_sdk-0.8.2/vantage_sdk/core/http/__init__.py
+-rw-r--r--   0        0        0      515 2024-04-25 01:26:48.219014 vantage_sdk-0.8.2/vantage_sdk/core/http/api/__init__.py
+-rw-r--r--   0        0        0    22934 2024-04-25 01:26:48.219174 vantage_sdk-0.8.2/vantage_sdk/core/http/api/account_management_api.py
+-rw-r--r--   0        0        0    75134 2024-05-14 15:00:04.645955 vantage_sdk-0.8.2/vantage_sdk/core/http/api/collection_management_api.py
+-rw-r--r--   0        0        0    15180 2024-04-25 01:26:48.219450 vantage_sdk-0.8.2/vantage_sdk/core/http/api/documents_api.py
+-rw-r--r--   0        0        0    57753 2024-05-14 15:00:04.646292 vantage_sdk-0.8.2/vantage_sdk/core/http/api/external_api_keys_api.py
+-rw-r--r--   0        0        0    54428 2024-04-25 01:26:48.219739 vantage_sdk-0.8.2/vantage_sdk/core/http/api/search_api.py
+-rw-r--r--   0        0        0    22624 2024-05-14 15:00:04.646500 vantage_sdk-0.8.2/vantage_sdk/core/http/api/vantage_api_keys_api.py
+-rw-r--r--   0        0        0    24948 2024-04-25 01:26:48.219980 vantage_sdk-0.8.2/vantage_sdk/core/http/api_client.py
+-rw-r--r--   0        0        0      678 2024-04-25 01:26:48.220043 vantage_sdk-0.8.2/vantage_sdk/core/http/api_response.py
+-rw-r--r--   0        0        0    15524 2024-04-25 01:26:48.220150 vantage_sdk-0.8.2/vantage_sdk/core/http/configuration.py
+-rw-r--r--   0        0        0     6369 2024-04-25 01:26:48.220244 vantage_sdk-0.8.2/vantage_sdk/core/http/exceptions.py
+-rw-r--r--   0        0        0     3384 2024-05-14 15:00:04.646724 vantage_sdk-0.8.2/vantage_sdk/core/http/models/__init__.py
+-rw-r--r--   0        0        0     2951 2024-04-25 01:26:48.220414 vantage_sdk-0.8.2/vantage_sdk/core/http/models/account.py
+-rw-r--r--   0        0        0     2735 2024-04-25 01:26:48.220567 vantage_sdk-0.8.2/vantage_sdk/core/http/models/account_modifiable.py
+-rw-r--r--   0        0        0     2812 2024-04-25 01:26:48.220678 vantage_sdk-0.8.2/vantage_sdk/core/http/models/account_read_only.py
+-rw-r--r--   0        0        0     7946 2024-05-14 15:00:04.646949 vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection.py
+-rw-r--r--   0        0        0     4615 2024-04-25 01:26:48.220877 vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_immutable.py
+-rw-r--r--   0        0        0     4445 2024-05-14 15:00:04.647162 vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_modifiable.py
+-rw-r--r--   0        0        0     4316 2024-04-25 01:26:48.221041 vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_read_only.py
+-rw-r--r--   0        0        0     3698 2024-04-25 01:26:48.221096 vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_upload_url.py
+-rw-r--r--   0        0        0     6297 2024-05-14 15:00:04.647434 vantage_sdk-0.8.2/vantage_sdk/core/http/models/create_collection_request.py
+-rw-r--r--   0        0        0     2962 2024-04-25 01:26:48.221270 vantage_sdk-0.8.2/vantage_sdk/core/http/models/document_batch.py
+-rw-r--r--   0        0        0     5971 2024-04-25 01:26:48.221347 vantage_sdk-0.8.2/vantage_sdk/core/http/models/embedding_search_query.py
+-rw-r--r--   0        0        0     4350 2024-04-25 01:26:48.221399 vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key.py
+-rw-r--r--   0        0        0     3383 2024-04-25 01:26:48.221449 vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key_modifiable.py
+-rw-r--r--   0        0        0     3673 2024-04-25 01:26:48.221506 vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key_read_only.py
+-rw-r--r--   0        0        0     5819 2024-04-25 01:26:48.221570 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties.py
+-rw-r--r--   0        0        0     3146 2024-04-25 01:26:48.221626 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_collection.py
+-rw-r--r--   0        0        0     4596 2024-04-25 01:26:48.221687 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py
+-rw-r--r--   0        0        0     2809 2024-04-25 01:26:48.221743 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_filter.py
+-rw-r--r--   0        0        0     2859 2024-04-25 01:26:48.221799 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_pagination.py
+-rw-r--r--   0        0        0     3657 2024-04-25 01:26:48.221873 vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_sort.py
+-rw-r--r--   0        0        0     3282 2024-04-25 01:26:48.221935 vantage_sdk-0.8.2/vantage_sdk/core/http/models/ml_these.py
+-rw-r--r--   0        0        0     3326 2024-04-25 01:26:48.221996 vantage_sdk-0.8.2/vantage_sdk/core/http/models/ml_these_these_inner.py
+-rw-r--r--   0        0        0     6474 2024-04-25 01:26:48.222076 vantage_sdk-0.8.2/vantage_sdk/core/http/models/more_like_these_query.py
+-rw-r--r--   0        0        0     5932 2024-04-25 01:26:48.222130 vantage_sdk-0.8.2/vantage_sdk/core/http/models/more_like_this_query.py
+-rw-r--r--   0        0        0     3721 2024-04-25 01:26:48.222195 vantage_sdk-0.8.2/vantage_sdk/core/http/models/search_result.py
+-rw-r--r--   0        0        0     2870 2024-04-25 01:26:48.222242 vantage_sdk-0.8.2/vantage_sdk/core/http/models/search_result_results_inner.py
+-rw-r--r--   0        0        0     3445 2024-05-14 15:00:04.647571 vantage_sdk-0.8.2/vantage_sdk/core/http/models/secondary_external_account.py
+-rw-r--r--   0        0        0     5912 2024-04-25 01:26:48.222361 vantage_sdk-0.8.2/vantage_sdk/core/http/models/semantic_search_query.py
+-rw-r--r--   0        0        0     4093 2024-04-25 01:26:48.222442 vantage_sdk-0.8.2/vantage_sdk/core/http/models/vantage_api_key.py
+-rw-r--r--   0        0        0     3003 2024-04-25 01:26:48.222499 vantage_sdk-0.8.2/vantage_sdk/core/http/models/weighted_field_values.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.222520 vantage_sdk-0.8.2/vantage_sdk/core/http/py.typed
+-rw-r--r--   0        0        0    10169 2024-04-25 01:26:48.222607 vantage_sdk-0.8.2/vantage_sdk/core/http/rest.py
+-rw-r--r--   0        0        0       95 2024-04-25 01:26:48.222695 vantage_sdk-0.8.2/vantage_sdk/core/management/__init__.py
+-rw-r--r--   0        0        0     1727 2024-04-25 01:26:48.222760 vantage_sdk-0.8.2/vantage_sdk/core/management/management.py
+-rw-r--r--   0        0        0       79 2024-04-25 01:26:48.222849 vantage_sdk-0.8.2/vantage_sdk/core/search/__init__.py
+-rw-r--r--   0        0        0      232 2024-04-25 01:26:48.222901 vantage_sdk-0.8.2/vantage_sdk/core/search/search.py
+-rw-r--r--   0        0        0      559 2024-04-25 01:26:48.222952 vantage_sdk-0.8.2/vantage_sdk/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-25 01:26:48.223004 vantage_sdk-0.8.2/vantage_sdk/model/__init__.py
+-rw-r--r--   0        0        0      187 2024-04-25 01:26:48.223071 vantage_sdk-0.8.2/vantage_sdk/model/account.py
+-rw-r--r--   0        0        0     2563 2024-05-14 15:00:04.647772 vantage_sdk-0.8.2/vantage_sdk/model/collection.py
+-rw-r--r--   0        0        0     1670 2024-05-22 17:47:33.292494 vantage_sdk-0.8.2/vantage_sdk/model/document.py
+-rw-r--r--   0        0        0      910 2024-05-14 15:00:04.648235 vantage_sdk-0.8.2/vantage_sdk/model/keys.py
+-rw-r--r--   0        0        0     1193 2024-04-25 01:26:48.223288 vantage_sdk-0.8.2/vantage_sdk/model/search.py
+-rw-r--r--   0        0        0     6150 1970-01-01 00:00:00.000000 vantage_sdk-0.8.2/PKG-INFO
```

### Comparing `vantage_sdk-0.8.1/LICENSE` & `vantage_sdk-0.8.2/LICENSE`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/README.md` & `vantage_sdk-0.8.2/README.md`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/docs/api.md` & `vantage_sdk-0.8.2/docs/api.md`

 * *Files 0% similar despite different names*

```diff
@@ -79,8 +79,8 @@
         docstring_style: numpy
         docstring_section_style: table
         merge_init_into_class: true
         show_docstring_attributes: true
         show_docstring_classes: true
         show_docstring_examples: true
         show_submodules: true
-        show_if_no_docstring: true
+        show_if_no_docstring: false
```

### Comparing `vantage_sdk-0.8.1/pyproject.toml` & `vantage_sdk-0.8.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool]
 [tool.poetry]
 name = "vantage-sdk"
-version = "0.8.1"
+version = "0.8.2"
 description = "Vantage Python SDK."
 authors = ["Vantage <none@vantage.com>"]
 readme = "README.md"
 repository = "https://github.com/VantageDiscovery/vantage-sdk-python"
 documentation = "https://docs.vantagediscovery.com/docs/concepts"
 classifiers=[
     'Programming Language :: Python :: 3.10',
@@ -116,15 +116,15 @@
     "D107"
 ]
 
 [tool.mypy]
 exclude = "vantage_sdk/core/http"
 
 [bumpver]
-current_version = "0.8.1"
+current_version = "0.8.2"
 version_pattern = "MAJOR.MINOR.PATCH"
 
 [bumpver.file_patterns]
 "pyproject.toml" = [
     'version = "{version}"',
 ]
 "vantage_sdk/__init__.py" = [
```

### Comparing `vantage_sdk-0.8.1/tests/data/documents.jsonl` & `vantage_sdk-0.8.2/tests/data/documents.jsonl`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/data/hello_world.parquet` & `vantage_sdk-0.8.2/tests/data/hello_world.parquet`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/.env-example` & `vantage_sdk-0.8.2/tests/integration_tests/.env-example`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/conftest.py` & `vantage_sdk-0.8.2/tests/integration_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/test_account.py` & `vantage_sdk-0.8.2/tests/integration_tests/test_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/test_api_keys.py` & `vantage_sdk-0.8.2/tests/integration_tests/test_api_keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/test_collection.py` & `vantage_sdk-0.8.2/tests/integration_tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/test_documents.py` & `vantage_sdk-0.8.2/tests/integration_tests/test_documents.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/tests/integration_tests/test_search.py` & `vantage_sdk-0.8.2/tests/integration_tests/test_search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/__init__.py` & `vantage_sdk-0.8.2/vantage_sdk/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     SearchResult,
     SearchResultItem,
 )
 
 
 __author__ = """Vantage"""
 __email__ = 'none@vantage.com'
-__version__ = '0.8.1'
+__version__ = '0.8.2'
 __all__ = [
     "VantageClient",
     "Collection",
     "CollectionUploadURL",
     "Account",
     "VantageAPIKey",
     "ExternalAPIKey",
```

### Comparing `vantage_sdk-0.8.1/vantage_sdk/client.py` & `vantage_sdk-0.8.2/vantage_sdk/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -328,15 +328,15 @@
 
         Returns
         -------
         Account
             An updated Account object reflecting the changes made.
 
         Notes
-        --------
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         account_modifiable = AccountModifiable(account_name=account_name)
 
         result = self.management_api.account_api.update_account(
             account_id=account_id or self.account_id,
@@ -367,14 +367,16 @@
             Defaults to None.
 
         Returns
         -------
         List[VantageAPIKey]
             A list of VantageAPIKey objects, each representing a Vantage API key associated with the account.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         keys = self.management_api.vantage_api_keys_api.get_vantage_api_keys(
             account_id=account_id or self.account_id,
         )
 
@@ -403,14 +405,16 @@
             Defaults to None.
 
         Returns
         -------
         VantageAPIKey
             A VantageAPIKey object containing the details of the requested API key.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         key = self.management_api.vantage_api_keys_api.get_vantage_api_key(
             account_id=account_id or self.account_id,
             vantage_api_key_id=vantage_api_key_id,
         )
@@ -439,14 +443,16 @@
             Defaults to None.
 
         Returns
         -------
         List[ExternalAPIKey]
             A list of ExternalAPIKey objects, each representing an external API key associated with the account.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         keys = self.management_api.external_api_keys_api.get_external_api_keys(
             account_id=account_id or self.account_id,
         )
         return [
@@ -477,14 +483,16 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the details of the requested external API key.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         key = self.management_api.external_api_keys_api.get_external_api_key(
             account_id=account_id or self.account_id,
             external_key_id=external_key_id,
         )
@@ -519,14 +527,16 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the details of the newly created API key.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         external_api_key_modifiable = ExternalAPIKeyModifiable(
             llm_provider=llm_provider, llm_secret=llm_secret
         )
 
@@ -568,14 +578,16 @@
             Defaults to None.
 
         Returns
         -------
         ExternalAPIKey
             An ExternalAPIKey object containing the updated details of the external API key.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         external_api_key_modifiable = ExternalAPIKeyModifiable(
             llm_provider=llm_provider, llm_secret=llm_secret
         )
 
@@ -607,14 +619,16 @@
         external_key_id : str
             The unique identifier of the external API key to be deleted.
         account_id : Optional[str], optional
             The unique identifier of the account to which the external API key is associated.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.external_api_keys_api.delete_external_api_key(
             account_id=account_id or self.account_id,
             external_key_id=external_key_id,
         )
@@ -741,14 +755,16 @@
             Defaults to None.
 
         Returns
         -------
         List[Collection]
             A list of Collection objects, each representing a collection associated with the account.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         collections = self.management_api.collection_api.list_collections(
             account_id=account_id or self.account_id
         )
 
@@ -782,14 +798,16 @@
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object containing the details of the specified collection.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         collection = self.management_api.collection_api.get_collection(
             collection_id=collection_id,
             account_id=account_id or self.account_id,
         )
@@ -820,14 +838,16 @@
             HuggingFaceCollection, both of which create and use Vantage-managed embeddings.
 
         Returns
         -------
         Collection
             A Collection object representing the newly created collection.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         if (
             hasattr(collection, "secondary_external_accounts")
             and collection.secondary_external_accounts is not None
         ):
@@ -896,14 +916,16 @@
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object representing the updated collection.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         collection = self.management_api.collection_api.get_collection(
             collection_id=collection_id,
             account_id=account_id or self.account_id,
         )
@@ -961,14 +983,16 @@
             Defaults to None.
 
         Returns
         -------
         Collection
             A Collection object representing the collection that was deleted.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.collection_api.delete_collection(
             collection_id=collection_id,
             account_id=account_id if account_id else self.account_id,
         )
@@ -1102,24 +1126,19 @@
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
-        collection = self.get_collection(collection_id=collection_id)
-
-        if collection.user_provided_embeddings:
-            raise ValueError(
-                "Semantic search is not possible on a collection of user-provided embeddings (UPE)."
-            )
-
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
             accuracy,
             page,
             page_count,
@@ -1204,14 +1223,16 @@
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
@@ -1299,14 +1320,16 @@
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results similar to the specified document.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
@@ -1394,14 +1417,16 @@
             Defaults to None.
 
         Returns
         -------
         SearchResult
             An object containing the search results similar to the specified document.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/search-api) for more details and examples.
         """
 
         vantage_api_key = self._vantage_api_key_check(vantage_api_key)
 
         search_properties = self._prepare_search_query(
             collection_id,
@@ -1579,14 +1604,17 @@
             either VantageManagedEmbeddingsDocument or UserProvidedEmbeddingsDocument,
             depending on the collection's type.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
+
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
         if not documents:
             raise ValueError("Documents object can't be empty.")
 
         collection = self.get_collection(
             collection_id=collection_id,
@@ -1632,14 +1660,16 @@
         batch_identifier : Optional[str], optional
             An optional identifier provided by the user to track the batch of document uploads.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         self.management_api.documents_api.upload_documents(
             body=documents_jsonl,
             account_id=account_id if account_id else self.account_id,
             collection_id=collection_id,
@@ -1668,14 +1698,16 @@
         batch_identifier : Optional[str], optional
             An optional identifier provided by the user to track the batch of document uploads.
         account_id : Optional[str], optional
             The account ID to which the collection belongs.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         if not exists(jsonl_file_path):
             raise FileNotFoundError(f"File \"{jsonl_file_path}\" not found.")
 
         file = open(jsonl_file_path, "rb")
@@ -1691,15 +1723,14 @@
         self,
         collection_id: str,
         parquet_file_path: str,
         account_id: Optional[str] = None,
     ) -> int:
         """
         Upserts embeddings from a parquet file to a collection.
-        This upsert method is available for user-provided embeddings collections only.
 
         Parameters
         ----------
         collection_id : str
             The unique identifier of the collection
             embeddings are being uploaded to.
         parquet_file_path : str, optional
@@ -1710,24 +1741,19 @@
             Defaults to None
 
         Returns
         -------
         int
             HTTP status of upload execution.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
-        collection = self.get_collection(collection_id=collection_id)
-
-        if not collection.user_provided_embeddings:
-            raise ValueError(
-                "Upsert using parquet file is available only for user-provided embeddings (UPE) collections."
-            )
-
         if not exists(parquet_file_path):
             raise FileNotFoundError(f"File \"{parquet_file_path}\" not found.")
         file_name = ntpath.basename(parquet_file_path)
 
         if not parquet_file_path.endswith(".parquet"):
             raise ValueError("File mast be a parquet file.")
 
@@ -1762,14 +1788,16 @@
         document_ids : List[str]
             A list of document IDs that need to be deleted from the collection.
         account_id : Optional[str], optional
             The account identifier under which the collection exists.
             If not provided, the instance's account ID is used.
             Defaults to None.
 
+        Notes
+        -----
         Visit our [documentation](https://docs.vantagediscovery.com/docs/management-api) for more details and examples.
         """
 
         documents_to_delete = [
             {"id": id, "operation": "delete"} for id in document_ids
         ]
```

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/base.py` & `vantage_sdk-0.8.2/vantage_sdk/core/base.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/exceptions.py` & `vantage_sdk-0.8.2/vantage_sdk/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/__init__.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/__init__.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/account_management_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/account_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/collection_management_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/collection_management_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/documents_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/documents_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/external_api_keys_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/external_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/search_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/search_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api/vantage_api_keys_api.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api/vantage_api_keys_api.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api_client.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api_client.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/api_response.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/api_response.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/configuration.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/configuration.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/exceptions.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/__init__.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/__init__.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_modifiable.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/account_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/account_read_only.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/account_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_immutable.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_immutable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_modifiable.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_read_only.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/collection_upload_url.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/collection_upload_url.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/create_collection_request.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/create_collection_request.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/document_batch.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/document_batch.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/embedding_search_query.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/embedding_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_modifiable.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key_modifiable.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/external_api_key_read_only.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/external_api_key_read_only.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_collection.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_field_value_weighting.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_filter.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_filter.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_pagination.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_pagination.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/global_search_properties_sort.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/global_search_properties_sort.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/ml_these.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/ml_these_these_inner.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/ml_these_these_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_these_query.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/more_like_these_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/more_like_this_query.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/more_like_this_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/search_result.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/search_result_results_inner.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/search_result_results_inner.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/secondary_external_account.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/secondary_external_account.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/semantic_search_query.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/semantic_search_query.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/vantage_api_key.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/vantage_api_key.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/models/weighted_field_values.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/models/weighted_field_values.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/http/rest.py` & `vantage_sdk-0.8.2/vantage_sdk/core/http/rest.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/core/management/management.py` & `vantage_sdk-0.8.2/vantage_sdk/core/management/management.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/exceptions.py` & `vantage_sdk-0.8.2/vantage_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/model/collection.py` & `vantage_sdk-0.8.2/vantage_sdk/model/collection.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/model/document.py` & `vantage_sdk-0.8.2/vantage_sdk/model/document.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/model/keys.py` & `vantage_sdk-0.8.2/vantage_sdk/model/keys.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/vantage_sdk/model/search.py` & `vantage_sdk-0.8.2/vantage_sdk/model/search.py`

 * *Files identical despite different names*

### Comparing `vantage_sdk-0.8.1/PKG-INFO` & `vantage_sdk-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vantage-sdk
-Version: 0.8.1
+Version: 0.8.2
 Summary: Vantage Python SDK.
 Home-page: https://github.com/VantageDiscovery/vantage-sdk-python
 Author: Vantage
 Author-email: none@vantage.com
 Requires-Python: >=3.10
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
```

