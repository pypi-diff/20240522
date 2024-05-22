# Comparing `tmp/microsoft_kiota_abstractions-1.3.1.tar.gz` & `tmp/microsoft_kiota_abstractions-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microsoft_kiota_abstractions-1.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "microsoft_kiota_abstractions-1.3.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `microsoft_kiota_abstractions-1.3.1.tar` & `microsoft_kiota_abstractions-1.3.2.tar`

### file list

```diff
@@ -1,83 +1,84 @@
--rw-r--r--   0        0        0       82 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/CODEOWNERS
--rw-r--r--   0        0        0      534 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      605 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      314 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/dependabot.yml
--rw-r--r--   0        0        0     2617 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/policies/resourceManagement.yml
--rw-r--r--   0        0        0      514 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/pull_request_template.md
--rw-r--r--   0        0        0      792 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/workflows/auto-merge-dependabot.yml
--rw-r--r--   0        0        0     1351 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/workflows/build.yml
--rw-r--r--   0        0        0     2538 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0        0        0     1324 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/workflows/conflicting-pr-label.yml
--rw-r--r--   0        0        0     1380 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.github/workflows/publish.yml
--rw-r--r--   0        0        0     1799 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.gitignore
--rw-r--r--   0        0        0    15931 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/.pylintrc
--rw-r--r--   0        0        0     4148 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/CHANGELOG.md
--rw-r--r--   0        0        0      444 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1141 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/LICENSE
--rw-r--r--   0        0        0      335 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/Makefile
--rw-r--r--   0        0        0     2515 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/README.md
--rw-r--r--   0        0        0     2757 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/SECURITY.md
--rw-r--r--   0        0        0     1244 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/SUPPORT.md
--rw-r--r--   0        0        0      119 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/__init__.py
--rw-r--r--   0        0        0       23 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/_version.py
--rw-r--r--   0        0        0     3566 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/api_client_builder.py
--rw-r--r--   0        0        0      656 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/api_error.py
--rw-r--r--   0        0        0      673 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/__init__.py
--rw-r--r--   0        0        0     1306 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/access_token_provider.py
--rw-r--r--   0        0        0     2120 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/allowed_hosts_validator.py
--rw-r--r--   0        0        0     1094 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/anonymous_authentication_provider.py
--rw-r--r--   0        0        0     2745 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/api_key_authentication_provider.py
--rw-r--r--   0        0        0      959 2024-03-05 10:03:19.424862 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/authentication_provider.py
--rw-r--r--   0        0        0     2127 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
--rw-r--r--   0        0        0     1432 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/base_request_builder.py
--rw-r--r--   0        0        0     1092 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/base_request_configuration.py
--rw-r--r--   0        0        0      648 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/default_query_parameters.py
--rw-r--r--   0        0        0      453 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/get_path_parameters.py
--rw-r--r--   0        0        0     6263 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/headers_collection.py
--rw-r--r--   0        0        0      529 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/method.py
--rw-r--r--   0        0        0     5823 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/multipart_body.py
--rw-r--r--   0        0        0      938 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/native_response_handler.py
--rw-r--r--   0        0        0     5758 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/request_adapter.py
--rw-r--r--   0        0        0    12541 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/request_information.py
--rw-r--r--   0        0        0      313 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/request_option.py
--rw-r--r--   0        0        0      965 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/response_handler.py
--rw-r--r--   0        0        0      734 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/__init__.py
--rw-r--r--   0        0        0      374 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/additional_data_holder.py
--rw-r--r--   0        0        0      182 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/composed_type_wrapper.py
--rw-r--r--   0        0        0     1006 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parsable.py
--rw-r--r--   0        0        0      642 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parsable_factory.py
--rw-r--r--   0        0        0     5850 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node.py
--rw-r--r--   0        0        0      876 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_factory.py
--rw-r--r--   0        0        0     1947 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_factory_registry.py
--rw-r--r--   0        0        0      949 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_helper.py
--rw-r--r--   0        0        0     2774 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_proxy_factory.py
--rw-r--r--   0        0        0     9849 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer.py
--rw-r--r--   0        0        0      898 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_factory.py
--rw-r--r--   0        0        0     2025 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py
--rw-r--r--   0        0        0     3532 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0      528 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/__init__.py
--rw-r--r--   0        0        0     1162 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backed_model.py
--rw-r--r--   0        0        0     4599 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store.py
--rw-r--r--   0        0        0      741 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_factory.py
--rw-r--r--   0        0        0     2239 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_factory_singleton.py
--rw-r--r--   0        0        0     1327 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_parse_node_factory.py
--rw-r--r--   0        0        0     2119 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
--rw-r--r--   0        0        0     8499 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/in_memory_backing_store.py
--rw-r--r--   0        0        0      697 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/in_memory_backing_store_factory.py
--rw-r--r--   0        0        0      899 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/kiota_abstractions/utils.py
--rw-r--r--   0        0        0     1263 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/pyproject.toml
--rw-r--r--   0        0        0     1209 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/requirements-dev.txt
--rw-r--r--   0        0        0        0 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/authentication/__init__.py
--rw-r--r--   0        0        0     2281 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/authentication/test_api_key_authentication_provider.py
--rw-r--r--   0        0        0     1051 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/authentication/test_base_bearer_token_authentication.py
--rw-r--r--   0        0        0     6002 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/conftest.py
--rw-r--r--   0        0        0        0 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/store/__init__.py
--rw-r--r--   0        0        0     1262 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/store/test_backed_model.py
--rw-r--r--   0        0        0     3140 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/store/test_backing_store_factory_singleton.py
--rw-r--r--   0        0        0    10860 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/store/test_in_memory_backing_store.py
--rw-r--r--   0        0        0     2052 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/test_base_request_builder.py
--rw-r--r--   0        0        0     2318 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/test_multipart_body.py
--rw-r--r--   0        0        0     6398 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/test_request_header.py
--rw-r--r--   0        0        0     8188 2024-03-05 10:03:19.428861 microsoft_kiota_abstractions-1.3.1/tests/test_request_information.py
--rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0       82 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/CODEOWNERS
+-rw-r--r--   0        0        0      534 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      605 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      314 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/dependabot.yml
+-rw-r--r--   0        0        0     2617 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/policies/resourceManagement.yml
+-rw-r--r--   0        0        0      514 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/pull_request_template.md
+-rw-r--r--   0        0        0      792 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/workflows/auto-merge-dependabot.yml
+-rw-r--r--   0        0        0     1351 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/workflows/build.yml
+-rw-r--r--   0        0        0     2538 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0        0        0     1324 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/workflows/conflicting-pr-label.yml
+-rw-r--r--   0        0        0     1380 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.github/workflows/publish.yml
+-rw-r--r--   0        0        0     1799 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.gitignore
+-rw-r--r--   0        0        0    15931 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/.pylintrc
+-rw-r--r--   0        0        0     4359 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/CHANGELOG.md
+-rw-r--r--   0        0        0      444 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1141 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/LICENSE
+-rw-r--r--   0        0        0      335 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/Makefile
+-rw-r--r--   0        0        0     2515 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/README.md
+-rw-r--r--   0        0        0     2757 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/SECURITY.md
+-rw-r--r--   0        0        0     1244 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/SUPPORT.md
+-rw-r--r--   0        0        0      119 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/__init__.py
+-rw-r--r--   0        0        0       23 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/_version.py
+-rw-r--r--   0        0        0     3566 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/api_client_builder.py
+-rw-r--r--   0        0        0      656 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/api_error.py
+-rw-r--r--   0        0        0      673 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/__init__.py
+-rw-r--r--   0        0        0     1306 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/access_token_provider.py
+-rw-r--r--   0        0        0     2120 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/allowed_hosts_validator.py
+-rw-r--r--   0        0        0     1094 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/anonymous_authentication_provider.py
+-rw-r--r--   0        0        0     2745 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/api_key_authentication_provider.py
+-rw-r--r--   0        0        0      959 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/authentication_provider.py
+-rw-r--r--   0        0        0     2127 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py
+-rw-r--r--   0        0        0     1432 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/base_request_builder.py
+-rw-r--r--   0        0        0     1138 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/base_request_configuration.py
+-rw-r--r--   0        0        0      648 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/default_query_parameters.py
+-rw-r--r--   0        0        0      453 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/get_path_parameters.py
+-rw-r--r--   0        0        0     6263 2024-03-26 10:36:16.851614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/headers_collection.py
+-rw-r--r--   0        0        0      529 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/method.py
+-rw-r--r--   0        0        0     5823 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/multipart_body.py
+-rw-r--r--   0        0        0      938 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/native_response_handler.py
+-rw-r--r--   0        0        0     5758 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/request_adapter.py
+-rw-r--r--   0        0        0    12541 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/request_information.py
+-rw-r--r--   0        0        0      313 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/request_option.py
+-rw-r--r--   0        0        0      965 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/response_handler.py
+-rw-r--r--   0        0        0      734 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/__init__.py
+-rw-r--r--   0        0        0      374 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/additional_data_holder.py
+-rw-r--r--   0        0        0      182 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/composed_type_wrapper.py
+-rw-r--r--   0        0        0     1006 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parsable.py
+-rw-r--r--   0        0        0      642 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parsable_factory.py
+-rw-r--r--   0        0        0     5850 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node.py
+-rw-r--r--   0        0        0      876 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_factory.py
+-rw-r--r--   0        0        0     1947 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_factory_registry.py
+-rw-r--r--   0        0        0      949 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_helper.py
+-rw-r--r--   0        0        0     2774 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_proxy_factory.py
+-rw-r--r--   0        0        0     9849 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer.py
+-rw-r--r--   0        0        0      898 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_factory.py
+-rw-r--r--   0        0        0     2025 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_factory_registry.py
+-rw-r--r--   0        0        0     3532 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0      528 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/__init__.py
+-rw-r--r--   0        0        0     1162 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backed_model.py
+-rw-r--r--   0        0        0     4599 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store.py
+-rw-r--r--   0        0        0      741 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_factory.py
+-rw-r--r--   0        0        0     2239 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_factory_singleton.py
+-rw-r--r--   0        0        0     1327 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_parse_node_factory.py
+-rw-r--r--   0        0        0     2119 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py
+-rw-r--r--   0        0        0     8499 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/in_memory_backing_store.py
+-rw-r--r--   0        0        0      697 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/in_memory_backing_store_factory.py
+-rw-r--r--   0        0        0      899 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/kiota_abstractions/utils.py
+-rw-r--r--   0        0        0     1263 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1209 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/requirements-dev.txt
+-rw-r--r--   0        0        0        0 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/authentication/__init__.py
+-rw-r--r--   0        0        0     2281 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/authentication/test_api_key_authentication_provider.py
+-rw-r--r--   0        0        0     1051 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/authentication/test_base_bearer_token_authentication.py
+-rw-r--r--   0        0        0     6002 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/store/__init__.py
+-rw-r--r--   0        0        0     1262 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/store/test_backed_model.py
+-rw-r--r--   0        0        0     3140 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/store/test_backing_store_factory_singleton.py
+-rw-r--r--   0        0        0    10860 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/store/test_in_memory_backing_store.py
+-rw-r--r--   0        0        0     2052 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/test_base_request_builder.py
+-rw-r--r--   0        0        0      530 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/test_base_request_configuration.py
+-rw-r--r--   0        0        0     2318 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/test_multipart_body.py
+-rw-r--r--   0        0        0     6398 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/test_request_header.py
+-rw-r--r--   0        0        0     8188 2024-03-26 10:36:16.855614 microsoft_kiota_abstractions-1.3.2/tests/test_request_information.py
+-rw-r--r--   0        0        0     3437 1970-01-01 00:00:00.000000 microsoft_kiota_abstractions-1.3.2/PKG-INFO
```

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/ISSUE_TEMPLATE/bug_report.md` & `microsoft_kiota_abstractions-1.3.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/ISSUE_TEMPLATE/feature_request.md` & `microsoft_kiota_abstractions-1.3.2/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/policies/resourceManagement.yml` & `microsoft_kiota_abstractions-1.3.2/.github/policies/resourceManagement.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/pull_request_template.md` & `microsoft_kiota_abstractions-1.3.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/workflows/auto-merge-dependabot.yml` & `microsoft_kiota_abstractions-1.3.2/.github/workflows/auto-merge-dependabot.yml`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     runs-on: ubuntu-latest
 
     if: ${{ github.actor == 'dependabot[bot]' }}
 
     steps:
       - name: Dependabot metadata
         id: metadata
-        uses: dependabot/fetch-metadata@v1.6.0
+        uses: dependabot/fetch-metadata@v2.0.0
         with:
           github-token: "${{ secrets.GITHUB_TOKEN }}"
 
       - name: Enable auto-merge for Dependabot PRs
         # Only if version bump is not a major version change
         if: ${{steps.metadata.outputs.update-type != 'version-update:semver-major'}}
         run: gh pr merge --auto --merge "$PR_URL"
```

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/workflows/build.yml` & `microsoft_kiota_abstractions-1.3.2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/workflows/codeql-analysis.yml` & `microsoft_kiota_abstractions-1.3.2/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/workflows/conflicting-pr-label.yml` & `microsoft_kiota_abstractions-1.3.2/.github/workflows/conflicting-pr-label.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.github/workflows/publish.yml` & `microsoft_kiota_abstractions-1.3.2/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.gitignore` & `microsoft_kiota_abstractions-1.3.2/.gitignore`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/.pylintrc` & `microsoft_kiota_abstractions-1.3.2/.pylintrc`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/CHANGELOG.md` & `microsoft_kiota_abstractions-1.3.2/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [1.3.2] - 2024-03-25
+
+### Added
+
+### Changed
+
+- Moved DeprecationWarning to __post_init__ of BaseRequestConfiguration. [microsoft/kiota#250](https://github.com/microsoft/kiota-abstractions-python/pull/250)
+
+
 ## [1.3.1] - 2024-03-05
 
 ### Added
 
 ### Changed
 
 - Fixed a bug with serialization of parsable multipart body due to unsubscriptable argument type.
```

### Comparing `microsoft_kiota_abstractions-1.3.1/LICENSE` & `microsoft_kiota_abstractions-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/README.md` & `microsoft_kiota_abstractions-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/SECURITY.md` & `microsoft_kiota_abstractions-1.3.2/SECURITY.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/SUPPORT.md` & `microsoft_kiota_abstractions-1.3.2/SUPPORT.md`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/api_client_builder.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/api_client_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/api_error.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/api_error.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/__init__.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/access_token_provider.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/access_token_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/allowed_hosts_validator.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/allowed_hosts_validator.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/anonymous_authentication_provider.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/anonymous_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/api_key_authentication_provider.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/api_key_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/authentication_provider.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/authentication/base_bearer_token_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/base_request_builder.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/base_request_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/base_request_configuration.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/base_request_configuration.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,11 +24,13 @@
     options: Optional[List[RequestOption]] = None
     # Request query parameters
     query_parameters: Optional[QueryParameters] = None
 
 
 @dataclass
 class BaseRequestConfiguration(RequestConfiguration):
-    warn(
-        "BaseRequestConfiguration is deprecated. Use RequestConfiguration class instead.",
-        DeprecationWarning
-    )
+
+    def __post_init__(self):
+        warn(
+            "BaseRequestConfiguration is deprecated. Use RequestConfiguration class instead.",
+            DeprecationWarning
+        )
```

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/default_query_parameters.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/default_query_parameters.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/headers_collection.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/headers_collection.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/method.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/method.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/multipart_body.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/multipart_body.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/native_response_handler.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/native_response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/request_adapter.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/request_adapter.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/request_information.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/response_handler.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/response_handler.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/__init__.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parsable.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parsable.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parsable_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parsable_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_factory_registry.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_helper.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_helper.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/parse_node_proxy_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/parse_node_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_factory_registry.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_factory_registry.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/serialization/serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/serialization/serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/__init__.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/__init__.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backed_model.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backed_model.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_factory_singleton.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_factory_singleton.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_parse_node_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_parse_node_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/backing_store_serialization_writer_proxy_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/in_memory_backing_store.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/store/in_memory_backing_store_factory.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/store/in_memory_backing_store_factory.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/kiota_abstractions/utils.py` & `microsoft_kiota_abstractions-1.3.2/kiota_abstractions/utils.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/pyproject.toml` & `microsoft_kiota_abstractions-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/requirements-dev.txt` & `microsoft_kiota_abstractions-1.3.2/requirements-dev.txt`

 * *Files 9% similar despite different names*

```diff
@@ -22,31 +22,31 @@
 
 isort==5.13.2
 
 lazy-object-proxy==1.10.0 ; python_version >= '3.7'
 
 mccabe==0.7.0 ; python_version >= '3.6'
 
-mypy==1.8.0
+mypy==1.9.0
 
 mypy-extensions==1.0.0 ; python_version >= '3.5'
 
-packaging==23.2 ; python_version >= '3.7'
+packaging==24.0 ; python_version >= '3.7'
 
 platformdirs==4.2.0 ; python_version >= '3.7'
 
 pluggy==1.4.0 ; python_version >= '3.6'
 
 pylint==3.1.0
 
-pytest==8.0.2
+pytest==8.1.1
 
-pytest-asyncio==0.23.5
+pytest-asyncio==0.23.6
 
-pytest-mock==3.12.0
+pytest-mock==3.14.0
 
 requests==2.31.0
 
 toml==0.10.2
 
 tomli==2.0.1 ; python_version < '3.11'
 
@@ -58,12 +58,12 @@
 
 urllib3==2.2.1 ; python_version >= '3.7'
 
 wrapt==1.15.0 ; python_version < '3.11'
 
 yapf==0.40.2
 
-std-uritemplate==0.0.54
+std-uritemplate==0.0.55
 
 opentelemetry-api==1.23.0
 
 opentelemetry-sdk==1.23.0
```

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/authentication/test_api_key_authentication_provider.py` & `microsoft_kiota_abstractions-1.3.2/tests/authentication/test_api_key_authentication_provider.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/authentication/test_base_bearer_token_authentication.py` & `microsoft_kiota_abstractions-1.3.2/tests/authentication/test_base_bearer_token_authentication.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/conftest.py` & `microsoft_kiota_abstractions-1.3.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/store/test_backed_model.py` & `microsoft_kiota_abstractions-1.3.2/tests/store/test_backed_model.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/store/test_backing_store_factory_singleton.py` & `microsoft_kiota_abstractions-1.3.2/tests/store/test_backing_store_factory_singleton.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/store/test_in_memory_backing_store.py` & `microsoft_kiota_abstractions-1.3.2/tests/store/test_in_memory_backing_store.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/test_base_request_builder.py` & `microsoft_kiota_abstractions-1.3.2/tests/test_base_request_builder.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/test_multipart_body.py` & `microsoft_kiota_abstractions-1.3.2/tests/test_multipart_body.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/test_request_header.py` & `microsoft_kiota_abstractions-1.3.2/tests/test_request_header.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/tests/test_request_information.py` & `microsoft_kiota_abstractions-1.3.2/tests/test_request_information.py`

 * *Files identical despite different names*

### Comparing `microsoft_kiota_abstractions-1.3.1/PKG-INFO` & `microsoft_kiota_abstractions-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microsoft-kiota-abstractions
-Version: 1.3.1
+Version: 1.3.2
 Summary: Core abstractions for kiota generated libraries in Python
 Keywords: kiota,openAPI,Microsoft,Graph
 Author-email: Microsoft <graphtooling+python@microsoft.com>
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

