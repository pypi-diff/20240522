# Comparing `tmp/tecton-0.9.3.tar.gz` & `tmp/tecton-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tecton-0.9.3.tar", last modified: Fri May 10 18:29:52 2024, max compression
+gzip compressed data, was "tecton-0.9.4.tar", last modified: Fri May 17 00:28:00 2024, max compression
```

## Comparing `tecton-0.9.3.tar` & `tecton-0.9.4.tar`

### file list

```diff
@@ -1,675 +1,675 @@
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.228607 tecton-0.9.3/
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-05-10 18:29:48.000000 tecton-0.9.3/MANIFEST.in
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-05-10 18:29:52.228607 tecton-0.9.3/PKG-INFO
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-05-10 18:29:48.000000 tecton-0.9.3/README.md
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.160602 tecton-0.9.3/protoc_gen_openapiv2/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/protoc_gen_openapiv2/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.160602 tecton-0.9.3/protoc_gen_openapiv2/options/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/protoc_gen_openapiv2/options/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-05-10 18:29:48.000000 tecton-0.9.3/protoc_gen_openapiv2/options/annotations_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-05-10 18:29:48.000000 tecton-0.9.3/protoc_gen_openapiv2/options/openapiv2_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-05-10 18:29:52.228607 tecton-0.9.3/setup.cfg
--rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2590 2024-05-10 18:29:48.000000 tecton-0.9.3/setup.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.164602 tecton-0.9.3/tecton/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_gen_version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.168603 tecton-0.9.3/tecton/_internals/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/analytics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/athena_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/data_frame_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/delete_keys_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/display.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/env_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29291 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/find_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/ingest_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/ingestion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/materialization_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/metadata_service.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.168603 tecton-0.9.3/tecton/_internals/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/metadata_service_impl/auth_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/metadata_service_impl/request_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/metadata_service_impl/service_modules.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/mock_source_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1357 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/offline_store_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/pandas_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/query_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20864 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/querytree_api.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.168603 tecton-0.9.3/tecton/_internals/repo/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/repo/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/repo/function_serialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18229 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/run_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/sdk_decorators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/secret_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/snowflake_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7214 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2996 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/tecton_pydantic.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.168603 tecton-0.9.3/tecton/_internals/tests/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/tests/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      342 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/tests/test_spark_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_internals/validations_api.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/_stamp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/aggregation_functions.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.168603 tecton-0.9.3/tecton/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26054 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/access_control.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/api_key.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/auth.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/cli.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/cli_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/command.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/completion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/engine.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/engine_renderer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32013 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/environment.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8982 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/environment_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/error_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/pex_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/printer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/repo.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9759 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/repo_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5011 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/service_account.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/user.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/workspace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/cli/workspace_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/fco_listers.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.172603 tecton-0.9.3/tecton/framework/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/base_tecton_object.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   119859 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/configs.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29108 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/data_frame.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    40898 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13976 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/dataset.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/entity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2641 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    42636 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/feature_service.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   229521 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/feature_view.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/filtered_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/repo_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/transformation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/validation_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/framework/workspace.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.172603 tecton-0.9.3/tecton/identities/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/identities/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/identities/api_keys.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/identities/credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/identities/okta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/pytest_tecton.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/run_api_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/snowflake_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/tecton_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/types.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.172603 tecton-0.9.3/tecton/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.172603 tecton-0.9.3/tecton/vendor/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.176603 tecton-0.9.3/tecton/vendor/dill/dill/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/__diff.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/_objects.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/detect.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/info.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/objtypes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/pointers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/settings.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/dill/dill/temp.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.176603 tecton-0.9.3/tecton/vendor/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.176603 tecton-0.9.3/tecton/vendor/pyspark/py4j/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/clientserver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/finalizer.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/java_collections.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/protocol.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/signals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/py4j/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.180604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/_globals.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/accumulators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/broadcast.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.180604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/daemon.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/files.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/find_spark_home.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/install.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/java_gateway.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/join.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.180604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/base.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/fpm.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/image.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.180604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/shared.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/regression.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/stat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/tuning.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/wrapper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/classification.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/clustering.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/common.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/feature.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/fpm.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/linalg/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/random.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/regression.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/profiler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/pyspark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/rdd.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/rddsampler.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.184604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/information.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/profile.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/requests.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/resultiterable.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/shell.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/shuffle.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.188604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.188604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/avro/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/catalog.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/column.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/dataframe.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/group.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.188604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21251 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/readwriter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/streaming.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/udf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/window.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/statcounter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/storagelevel.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.188604 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/dstream.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/listener.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/taskcontext.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/traceback_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/util.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/pyspark/pyspark/worker.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/vendor_dill.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/vendor/vendor_pyspark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton/version.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.164602 tecton-0.9.3/tecton.egg-info/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/PKG-INFO
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23011 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/SOURCES.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/dependency_links.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/entry_points.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1128 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/requires.txt
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-05-10 18:29:50.000000 tecton-0.9.3/tecton.egg-info/top_level.txt
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.192604 tecton-0.9.3/tecton_athena/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/athena_session.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/data_catalog_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5708 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/odfv_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.192604 tecton-0.9.3/tecton_athena/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.192604 tecton-0.9.3/tecton_athena/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/create_table.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_athena/templates_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.196605 tecton-0.9.3/tecton_core/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/_gen_version.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/aggregation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/arrow.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/aws_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/compute_mode.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    24797 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/conf.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/data_types.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3981 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/duckdb_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.196605 tecton-0.9.3/tecton_core/embeddings/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/embeddings/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/embeddings/config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/fco_container.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27600 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/feature_definition_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/feature_set_config.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/feature_view_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/filter_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/function_deserialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/http.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/id_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/iterators.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/materialization_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.196605 tecton-0.9.3/tecton_core/metadata_service_impl/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/base_stub.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/error_lib.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/http_client.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/providers.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/response.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/service_calls.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/metadata_service_impl/trace.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20281 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/online_serving_index.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7766 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/pipeline_common.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    56183 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/compaction_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/dialect.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/query/duckdb/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/duckdb/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10983 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/duckdb/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/duckdb/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/duckdb/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/errors.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/executor_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/executor_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/node_interface.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7303 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/node_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   126322 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/query/pandas/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21975 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/pipeline_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/sql.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pandas/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/pipeline_sql_builder.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/prefixed_uri_resolver.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4204 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/query_tree_compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21774 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/query_tree_executor.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/rewrite.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/query/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/snowflake/compute.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query/sql_compat.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/query_consts.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/repo_file_handler.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/request_context.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/schema.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    11989 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/schema_validation.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/snowflake_context.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/specs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/data_source_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/entity_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/feature_service_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    43407 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/feature_view_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/tecton_object_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/time_window_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/transformation_spec.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/specs/utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/time_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/vendor/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/queue.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.200605 tecton-0.9.3/tecton_core/vendor/treelib/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/exceptions.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/misc.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/plugins.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/treelib/tree.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_core/vendor/vendor_treelib.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23147 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/batch_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_materialization/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/common/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/common/job_metadata_aws.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/common/job_metadata_gcp.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/common/task_params.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/consumption.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/delta_maintenance.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/entity_deletion.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/job_metadata.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/materialization_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_materialization/ray/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/batch_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/delta.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/feature_export.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/ingest_materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/job_status.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/materialization.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/materialization_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/ray/nodes.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_materialization/remote_host/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/remote_host/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/remote_host/pyspark_remote_host.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/secrets.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_materialization/stream_materialization.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_proto/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_proto/amplitude/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/amplitude/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/amplitude/amplitude_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/amplitude/client_logging_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_proto/api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/api/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.204605 tecton-0.9.3/tecton_proto/api/featureservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/api/featureservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/api/featureservice/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/api/featureservice/feature_service_request_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.208606 tecton-0.9.3/tecton_proto/args/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/basic_info_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/data_source_config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    21536 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/diff_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/diff_test_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/fco_args_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    41778 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/pipeline_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/repo_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/user_defined_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/version_constraints_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/args/virtual_data_source_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.208606 tecton-0.9.3/tecton_proto/auditlog/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auditlog/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auditlog/metadata_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.208606 tecton-0.9.3/tecton_proto/auth/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/acl_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/authorization_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/principal_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/resource_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/resource_role_assignments_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/auth/service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.208606 tecton-0.9.3/tecton_proto/canary/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/canary/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/canary/type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/canary/update_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.208606 tecton-0.9.3/tecton_proto/cli/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/cli/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/cli/repo_diff_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.212606 tecton-0.9.3/tecton_proto/common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/aggregation_function_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/analytics_options_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/aws_credentials_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/column_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/compute_mode_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/container_image_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/data_source_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/data_type_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/fco_locator_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/framework_version_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/id_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/pair_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/schema_container_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/secret_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/spark_schema_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/common/time_window_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.212606 tecton-0.9.3/tecton_proto/consumption/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/consumption/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/consumption/consumption_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/data/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/batch_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/entity_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/fco_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/fco_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/feature_service_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/feature_store_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    20207 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/feature_view_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/freshness_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/fv_materialization_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/hive_metastore_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/internal_spark_cluster_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/materialization_roles_allowlists_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/materialization_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/odfv_compute_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/onboarding_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/principal_group_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/remote_compute_environment_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/remote_spark_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/saved_feature_data_frame_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/serving_status_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/state_update_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/stream_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/summary_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/tecton_api_key_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/transformation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/user_deployment_settings_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/user_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/virtual_data_source_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/data/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/databricks_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/dbfs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/execution_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/instance_profiles_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/jobs_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/libraries_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/permissions_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/scim_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/secrets_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/databricks_api/workspace_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/dataobs/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/expectation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/metric_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/validation_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/validation_task_params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/dataobs/validation_task_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/feature_server/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/feature_server/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/feature_server/configuration/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/feature_server/configuration/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/materialization/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/job_metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/materialization_states_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/materialization_task_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/params_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materialization/spark_cluster_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/materializationjobservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materializationjobservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.216606 tecton-0.9.3/tecton_proto/metadataservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/metadataservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/metadataservice/http_over_grpc_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)   121489 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/metadataservice/metadata_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/offlinestore/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/offlinestore/__init__.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/offlinestore/delta/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/offlinestore/delta/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/offlinestore/delta/metadata_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/online_store/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store/feature_value_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store/status_entry_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/online_store_writer/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store_writer/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store_writer/config_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/online_store_writer/copier_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/remoteenvironmentservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/remoteenvironmentservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/secrets/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/secrets/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/secrets/secrets_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/snowflake/location_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/snowflake/snowflake_credentials_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/spark_api/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_api/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_api/error_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_api/jobs_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/spark_common/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_common/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_common/clusters_pb2.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/spark_common/libraries_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/testhelperservice/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/testhelperservice/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/testhelperservice/test_helper_service_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_proto/validation/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/validation/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_proto/validation/validator_pb2.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.220607 tecton-0.9.3/tecton_snowflake/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.224607 tecton-0.9.3/tecton_snowflake/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/dataframe_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    13676 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/nodes.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/queries.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/rewrite.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/snowflake_type_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33774 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/sql_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.224607 tecton-0.9.3/tecton_snowflake/templates/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/copier_macro.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/create_temp_table_for_bfv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/data_source.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/delete_orphaned_schemas.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/delete_staged_files.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/historical_features.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/historical_features_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/materialization_tile.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/materialized_feature_view.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/offline_materialization_macros.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/online_store_copier.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/run_full_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/run_partial_aggregation.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/time_limit.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates/transformation_pipeline.sql
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/templates_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_snowflake/utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.228607 tecton-0.9.3/tecton_spark/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/aggregation_plans.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/data_observability.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/data_source_credentials.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    35732 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/data_source_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/errors_spark.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/feature_view_spark_utils.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.228607 tecton-0.9.3/tecton_spark/jars/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/jars/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/jars/class_loader.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/jars/tecton-udfs-spark-3.jar
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7182 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/materialization_plan.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    27440 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/offline_store.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    15491 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/partial_aggregations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    33450 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/pipeline_helper.py
-drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:52.228607 tecton-0.9.3/tecton_spark/query/
--rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/__init__.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/data_source.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/filter.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/join.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/node.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     7583 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/pipeline.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/projection.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/query/translate.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)    17838 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/schema_derivation_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/schema_spark_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/spark_helper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/spark_schema_wrapper.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     5028 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/time_utils.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      880 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/type_annotations.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/udf_jar.py
--rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-05-10 18:29:48.000000 tecton-0.9.3/tecton_spark/udfs.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.379806 tecton-0.9.4/
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)      206 2024-05-17 00:27:54.000000 tecton-0.9.4/MANIFEST.in
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-05-17 00:28:00.379806 tecton-0.9.4/PKG-INFO
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     3143 2024-05-17 00:27:54.000000 tecton-0.9.4/README.md
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.251796 tecton-0.9.4/protoc_gen_openapiv2/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/protoc_gen_openapiv2/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.251796 tecton-0.9.4/protoc_gen_openapiv2/options/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/protoc_gen_openapiv2/options/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-05-17 00:27:54.000000 tecton-0.9.4/protoc_gen_openapiv2/options/annotations_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18717 2024-05-17 00:27:54.000000 tecton-0.9.4/protoc_gen_openapiv2/options/openapiv2_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       38 2024-05-17 00:28:00.379806 tecton-0.9.4/setup.cfg
+-rwxr-xr-x   0 nobody   (65534) nogroup  (65534)     2590 2024-05-17 00:27:54.000000 tecton-0.9.4/setup.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.251796 tecton-0.9.4/tecton/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6026 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_gen_version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.259796 tecton-0.9.4/tecton/_internals/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10733 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/analytics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2279 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/athena_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1168 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/data_frame_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6558 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/delete_keys_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8122 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/display.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      930 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/env_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29291 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      881 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/find_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3193 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/ingest_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2359 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/ingestion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12345 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/materialization_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/metadata_service.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.259796 tecton-0.9.4/tecton/_internals/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      492 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/metadata_service_impl/auth_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1870 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/metadata_service_impl/request_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      615 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/metadata_service_impl/service_modules.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/mock_source_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2098 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/offline_store_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1037 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/pandas_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16160 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/query_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20864 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/querytree_api.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.259796 tecton-0.9.4/tecton/_internals/repo/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/repo/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11416 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/repo/function_serialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12059 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18229 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/run_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13055 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/sdk_decorators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2059 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/secret_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7119 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/snowflake_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7214 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2996 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5615 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/tecton_pydantic.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.259796 tecton-0.9.4/tecton/_internals/tests/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/tests/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      342 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/tests/test_spark_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7071 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3769 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14505 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4985 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/_internals/validations_api.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      322 2024-05-17 00:27:55.000000 tecton-0.9.4/tecton/_stamp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3067 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/aggregation_functions.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.267797 tecton-0.9.4/tecton/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26054 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/access_control.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1583 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/api_key.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3083 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/auth.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5469 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/cli.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8462 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/cli_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5967 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/command.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2027 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/completion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18539 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/engine.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1323 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/engine_renderer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32013 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/environment.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8982 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/environment_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7691 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/error_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3759 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      515 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/pex_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1786 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/printer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5135 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/repo.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9759 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7739 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/repo_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5011 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5824 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/service_account.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5620 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2403 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/user.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4917 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/workspace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2711 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/cli/workspace_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2450 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/fco_listers.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.271797 tecton-0.9.4/tecton/framework/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6920 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/base_tecton_object.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   119859 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/configs.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29108 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/data_frame.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    40898 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13976 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/dataset.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7683 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/entity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2641 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    42636 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/feature_service.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   229521 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/feature_view.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3854 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/filtered_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4922 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/repo_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21258 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/transformation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2071 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2091 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/validation_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22520 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/framework/workspace.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.275797 tecton-0.9.4/tecton/identities/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/identities/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1521 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/identities/api_keys.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14640 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/identities/credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12333 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/identities/okta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2374 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/pytest_tecton.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      381 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/run_api_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      709 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/snowflake_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2747 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/tecton_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6326 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/types.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.275797 tecton-0.9.4/tecton/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.275797 tecton-0.9.4/tecton/vendor/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.279798 tecton-0.9.4/tecton/vendor/dill/dill/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7211 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/__diff.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3634 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54753 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20428 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/_objects.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11822 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/detect.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7444 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/info.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      755 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/objtypes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4467 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/pointers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      719 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/settings.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44906 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8238 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/dill/dill/temp.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.279798 tecton-0.9.4/tecton/vendor/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.283798 tecton-0.9.4/tecton/vendor/pyspark/py4j/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      111 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    26941 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/clientserver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2329 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4306 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/finalizer.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18289 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/java_collections.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    96550 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14805 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/protocol.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4361 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/signals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       23 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/py4j/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.287799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4777 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2282 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/_globals.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9940 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/accumulators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7386 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/broadcast.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.287799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      201 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30084 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29668 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      354 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7831 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    54613 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7619 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/daemon.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1891 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/files.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3969 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/find_spark_home.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6654 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/install.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10025 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/java_gateway.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3994 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/join.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.291799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1530 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10846 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/base.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126616 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    62498 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4294 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    34149 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   212823 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17053 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/fpm.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4603 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8092 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/image.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.295799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39791 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.295799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18532 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9556 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22295 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/shared.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13656 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23213 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    91533 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/regression.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    18317 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/stat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13108 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57402 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/tuning.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22016 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15371 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/wrapper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.299799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1372 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28695 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/classification.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    39889 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/clustering.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4976 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/common.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20443 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28134 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/feature.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7028 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/fpm.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.299799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/linalg/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    46744 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    57731 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19517 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/random.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12101 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    32842 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/regression.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.299799 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1969 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1309 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14081 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1289 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2301 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    25342 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21149 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5755 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/profiler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.303800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.303800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/pyspark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/pyspark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   109373 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/rdd.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4250 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/rddsampler.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.303800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1317 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1590 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/information.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7097 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/profile.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10946 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/requests.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1224 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/resultiterable.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20586 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2473 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/shell.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27959 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/shuffle.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.307800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2590 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.307800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/avro/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      809 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5993 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12110 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/catalog.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29664 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/column.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2999 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23884 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    99829 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/dataframe.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   157099 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10681 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/group.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.311800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      959 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21251 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28130 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14683 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3806 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12308 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6324 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13225 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2745 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    77056 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/readwriter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    31188 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    69121 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/streaming.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    55203 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20068 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/udf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6976 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12863 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/window.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5149 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/statcounter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3756 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2785 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/storagelevel.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.311800 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1007 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16448 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27879 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/dstream.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5436 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2333 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/listener.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5614 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9189 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/taskcontext.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2679 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/traceback_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11623 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/util.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       20 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27875 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/pyspark/pyspark/worker.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1334 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/vendor_dill.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1448 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/vendor/vendor_pyspark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1154 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton/version.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.255796 tecton-0.9.4/tecton.egg-info/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3952 2024-05-17 00:27:57.000000 tecton-0.9.4/tecton.egg-info/PKG-INFO
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23011 2024-05-17 00:27:58.000000 tecton-0.9.4/tecton.egg-info/SOURCES.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        1 2024-05-17 00:27:57.000000 tecton-0.9.4/tecton.egg-info/dependency_links.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       96 2024-05-17 00:27:58.000000 tecton-0.9.4/tecton.egg-info/entry_points.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1128 2024-05-17 00:27:58.000000 tecton-0.9.4/tecton.egg-info/requires.txt
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      120 2024-05-17 00:27:58.000000 tecton-0.9.4/tecton.egg-info/top_level.txt
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.311800 tecton-0.9.4/tecton_athena/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14977 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/athena_session.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8797 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/data_catalog_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5708 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/odfv_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.311800 tecton-0.9.4/tecton_athena/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2381 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17721 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.315801 tecton-0.9.4/tecton_athena/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/create_table.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      267 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9544 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      672 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3975 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      503 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1046 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      277 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      656 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_athena/templates_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.323801 tecton-0.9.4/tecton_core/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)       17 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/_gen_version.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13149 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/aggregation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1598 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/arrow.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1956 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/aws_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3464 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/compute_mode.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    24797 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/conf.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7234 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/data_types.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3981 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/duckdb_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.323801 tecton-0.9.4/tecton_core/embeddings/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/embeddings/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/embeddings/config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7404 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5113 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/fco_container.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    27600 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/feature_definition_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9838 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/feature_set_config.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      749 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/feature_view_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      302 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/filter_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2507 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/function_deserialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      739 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/http.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      616 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/id_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      546 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/iterators.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7440 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/materialization_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.327802 tecton-0.9.4/tecton_core/metadata_service_impl/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      195 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/base_stub.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2665 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/error_lib.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3488 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/http_client.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      901 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/providers.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1990 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/response.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2273 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/service_calls.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      206 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/metadata_service_impl/trace.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20605 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1427 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/online_serving_index.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7766 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/pipeline_common.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.327802 tecton-0.9.4/tecton_core/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    22026 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    56183 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5286 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/compaction_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      179 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/dialect.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.327802 tecton-0.9.4/tecton_core/query/duckdb/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/duckdb/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13489 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/duckdb/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7820 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/duckdb/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      714 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/duckdb/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1526 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/errors.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      746 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/executor_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/executor_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10749 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/node_interface.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7332 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/node_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   126322 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.331802 tecton-0.9.4/tecton_core/query/pandas/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3556 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4033 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21975 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6169 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/pipeline_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5054 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      192 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/sql.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1948 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pandas/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5944 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/pipeline_sql_builder.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      786 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/prefixed_uri_resolver.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4433 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/query_tree_compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21933 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/query_tree_executor.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      227 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/rewrite.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.331802 tecton-0.9.4/tecton_core/query/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    12630 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/snowflake/compute.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20202 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query/sql_compat.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3294 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/query_consts.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5280 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/repo_file_handler.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      867 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/request_context.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3149 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/schema.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    11989 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5597 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/schema_validation.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1063 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2126 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/snowflake_context.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.331802 tecton-0.9.4/tecton_core/specs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      777 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    44686 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/data_source_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1457 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/entity_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5460 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/feature_service_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    43407 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/feature_view_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4440 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/tecton_object_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9179 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/time_window_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2440 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/transformation_spec.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4952 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/specs/utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9725 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/time_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.331802 tecton-0.9.4/tecton_core/vendor/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9361 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/queue.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.331802 tecton-0.9.4/tecton_core/vendor/treelib/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1594 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      943 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/exceptions.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1575 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/misc.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9595 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1265 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/plugins.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37469 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/treelib/tree.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1275 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_core/vendor/vendor_treelib.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.335802 tecton-0.9.4/tecton_materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      718 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23147 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/batch_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.335802 tecton-0.9.4/tecton_materialization/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2835 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/common/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5803 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/common/job_metadata_aws.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2222 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/common/job_metadata_gcp.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2693 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/common/task_params.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4811 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/consumption.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1070 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/delta_maintenance.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3731 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/entity_deletion.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5200 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5090 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7159 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/job_metadata.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9316 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7780 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/materialization_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.335802 tecton-0.9.4/tecton_materialization/ray/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5242 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/batch_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    23853 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/delta.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5973 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/feature_export.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5009 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/ingest_materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6869 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/job_status.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10181 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/materialization.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4190 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/materialization_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3172 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/ray/nodes.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.335802 tecton-0.9.4/tecton_materialization/remote_host/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/remote_host/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20100 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/remote_host/pyspark_remote_host.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1996 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/secrets.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6666 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_materialization/stream_materialization.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.335802 tecton-0.9.4/tecton_proto/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.339803 tecton-0.9.4/tecton_proto/amplitude/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/amplitude/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4642 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/amplitude/amplitude_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3093 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/amplitude/client_logging_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.339803 tecton-0.9.4/tecton_proto/api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/api/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.339803 tecton-0.9.4/tecton_proto/api/featureservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/api/featureservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    81835 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/api/featureservice/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9573 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/api/featureservice/feature_service_request_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.339803 tecton-0.9.4/tecton_proto/args/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2864 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/basic_info_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1897 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/data_source_config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    21536 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3996 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/diff_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6990 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/diff_test_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3059 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2415 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/fco_args_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5172 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    41778 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6092 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/pipeline_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1694 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/repo_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4704 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1637 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/user_defined_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1893 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/version_constraints_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8163 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/args/virtual_data_source_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.339803 tecton-0.9.4/tecton_proto/auditlog/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auditlog/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2716 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auditlog/metadata_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.343803 tecton-0.9.4/tecton_proto/auth/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1422 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/acl_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    29023 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/authorization_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3224 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/principal_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6551 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/resource_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/resource_role_assignments_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3058 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/auth/service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.343803 tecton-0.9.4/tecton_proto/canary/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/canary/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1208 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/canary/type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2195 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/canary/update_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.343803 tecton-0.9.4/tecton_proto/cli/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/cli/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3075 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/cli/repo_diff_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.343803 tecton-0.9.4/tecton_proto/common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3459 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/aggregation_function_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1717 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/analytics_options_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1823 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/aws_credentials_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1672 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/column_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1336 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/compute_mode_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1934 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/container_image_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1373 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/data_source_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2431 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/data_type_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1735 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/fco_locator_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1286 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/framework_version_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1725 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/id_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1150 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/pair_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1368 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/schema_container_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2819 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1518 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/secret_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1381 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/spark_schema_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2183 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/common/time_window_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.347803 tecton-0.9.4/tecton_proto/consumption/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/consumption/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5600 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/consumption/consumption_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.347803 tecton-0.9.4/tecton_proto/data/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7900 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/batch_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2313 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/entity_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2848 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/fco_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2916 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/fco_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5025 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/feature_service_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1487 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/feature_store_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    20207 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/feature_view_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2121 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/freshness_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4810 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/fv_materialization_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1366 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/hive_metastore_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1975 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/internal_spark_cluster_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1683 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/materialization_roles_allowlists_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5831 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/materialization_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1752 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/odfv_compute_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/onboarding_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2614 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/principal_group_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6827 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/remote_compute_environment_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15757 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/remote_spark_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3468 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/saved_feature_data_frame_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4545 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/serving_status_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10895 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/state_update_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4799 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/stream_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1828 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/summary_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2349 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/tecton_api_key_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2795 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/transformation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10456 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/user_deployment_settings_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1650 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/user_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3433 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/virtual_data_source_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2355 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/data/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.351803 tecton-0.9.4/tecton_proto/databricks_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8276 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1889 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/dbfs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1276 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3593 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/execution_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1501 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/instance_profiles_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8112 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/jobs_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1912 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/libraries_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2911 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/permissions_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1253 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/scim_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2391 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/secrets_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2613 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/databricks_api/workspace_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.351803 tecton-0.9.4/tecton_proto/dataobs/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2490 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2553 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/expectation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3691 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/metric_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5748 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/validation_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3723 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/validation_task_params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4629 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/dataobs/validation_task_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.351803 tecton-0.9.4/tecton_proto/feature_server/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/feature_server/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.351803 tecton-0.9.4/tecton_proto/feature_server/configuration/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/feature_server/configuration/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    19997 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.355804 tecton-0.9.4/tecton_proto/materialization/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     9821 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/job_metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2610 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/materialization_states_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14634 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/materialization_task_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8173 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/params_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2752 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materialization/spark_cluster_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.355804 tecton-0.9.4/tecton_proto/materializationjobservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materializationjobservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    16111 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.355804 tecton-0.9.4/tecton_proto/metadataservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/metadataservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2776 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/metadataservice/http_over_grpc_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)   121631 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/metadataservice/metadata_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.355804 tecton-0.9.4/tecton_proto/offlinestore/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/offlinestore/__init__.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.355804 tecton-0.9.4/tecton_proto/offlinestore/delta/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/offlinestore/delta/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1570 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/offlinestore/delta/metadata_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6554 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/online_store/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5408 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store/feature_value_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1306 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store/status_entry_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/online_store_writer/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store_writer/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2401 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store_writer/config_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5522 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/online_store_writer/copier_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/remoteenvironmentservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/remoteenvironmentservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13213 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/secrets/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/secrets/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10485 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/secrets/secrets_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1246 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/snowflake/location_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1392 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/snowflake/snowflake_credentials_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.359804 tecton-0.9.4/tecton_proto/spark_api/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_api/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1195 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_api/error_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7388 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_api/jobs_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.363804 tecton-0.9.4/tecton_proto/spark_common/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_common/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7786 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_common/clusters_pb2.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2386 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/spark_common/libraries_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.363804 tecton-0.9.4/tecton_proto/testhelperservice/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/testhelperservice/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3516 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/testhelperservice/test_helper_service_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.363804 tecton-0.9.4/tecton_proto/validation/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/validation/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     4609 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_proto/validation/validator_pb2.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.363804 tecton-0.9.4/tecton_snowflake/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30085 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.367805 tecton-0.9.4/tecton_snowflake/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10160 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/dataframe_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    13676 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/nodes.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6314 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/queries.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      741 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/rewrite.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3704 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     8392 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2246 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/snowflake_type_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33774 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/sql_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.371805 tecton-0.9.4/tecton_snowflake/templates/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1025 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/copier_macro.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      396 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/create_temp_table_for_bfv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      363 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/create_temp_table_for_bwafv.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      255 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/data_source.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1248 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/delete_orphaned_schemas.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      698 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/delete_staged_files.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3069 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/historical_features.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7892 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/historical_features_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1795 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/materialization_tile.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2575 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/materialized_feature_view.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      937 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/offline_materialization_macros.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      126 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/online_store_copier.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6777 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/run_full_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      583 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/run_partial_aggregation.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      569 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/time_limit.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      213 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates/transformation_pipeline.sql
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      806 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/templates_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      249 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_snowflake/utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.375805 tecton-0.9.4/tecton_spark/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      808 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    30278 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/aggregation_plans.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2263 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/data_observability.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      926 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/data_source_credentials.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    35732 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/data_source_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      425 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/errors_spark.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     6470 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/feature_view_spark_utils.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.375805 tecton-0.9.4/tecton_spark/jars/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/jars/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2633 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/jars/class_loader.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)  1794322 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/jars/tecton-udfs-spark-3.jar
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7182 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/materialization_plan.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    28400 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/offline_store.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    15491 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/partial_aggregations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    33450 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/pipeline_helper.py
+drwxr-xr-x   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:28:00.379806 tecton-0.9.4/tecton_spark/query/
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)        0 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/__init__.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3356 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/data_source.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10751 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/filter.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    37167 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/join.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1515 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/node.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     7583 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/pipeline.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    14752 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/projection.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    10712 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/query/translate.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)    17838 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/schema_derivation_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5434 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/schema_spark_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     2317 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/spark_helper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     1697 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/spark_schema_wrapper.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     5028 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/time_utils.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      880 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/type_annotations.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)      393 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/udf_jar.py
+-rw-r--r--   0 nobody   (65534) nogroup  (65534)     3257 2024-05-17 00:27:54.000000 tecton-0.9.4/tecton_spark/udfs.py
```

### Comparing `tecton-0.9.3/PKG-INFO` & `tecton-0.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.3/README.md` & `tecton-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/protoc_gen_openapiv2/options/annotations_pb2.py` & `tecton-0.9.4/protoc_gen_openapiv2/options/annotations_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/protoc_gen_openapiv2/options/openapiv2_pb2.py` & `tecton-0.9.4/protoc_gen_openapiv2/options/openapiv2_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/setup.py` & `tecton-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,14 @@
     author_email='support@tecton.ai',
     url='https://tecton.ai',
     license='Tecton Proprietary',
     include_package_data=True,
     description='Tecton Python SDK',
     entry_points={'console_scripts': ['tecton=tecton.cli.cli:main'], 'pytest11': ['pytest_tecton=tecton.pytest_tecton']},
     name='tecton',
-    version='0.9.3',
+    version='0.9.4',
     long_description=long_description,
     long_description_content_type='text/markdown',
     install_requires=['attrs>=21.3.0', 'boto3', 'googleapis-common-protos<2,>=1.57.0', 'jinja2~=3.0', 'numpy~=1.16', 'pathspec', 'pendulum~=2.1', 'protobuf>=3.20.0', 'pypika~=0.48.9', 'pytimeparse', 'pandas>=1.0', 'texttable', 'requests', 'colorama~=0.4', 'tqdm~=4.41', 'yaspin<3,>=0.16', 'typing-extensions~=4.1', 'pygments>=2.7.4', 'pytest', 'click~=8.0', 'typeguard~=2.0', 'sqlparse', 'semantic_version', 'pyarrow<15,>=8', 'pydantic<3,>=1.10.13', 'pyyaml', 'setuptools', 'pip', 'pex~=2.1'],
     extras_require={'databricks-connect': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect9': ['databricks-connect[sql]~=9.1.23'], 'databricks-connect10': ['databricks-connect[sql]~=10.4.12'], 'databricks-connect11': ['databricks-connect[sql]~=11.3.12'], 'pyspark': ['pyspark[sql]~=3.2.1'], 'pyspark3': ['pyspark[sql]~=3.2.1'], 'pyspark3.1': ['pyspark[sql]~=3.1.2'], 'pyspark3.2': ['pyspark[sql]~=3.2.1'], 'pyspark3.3': ['pyspark[sql]~=3.3.2'], 'rift': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0'], 'rift-materialization': ['duckdb==0.10.0', 'deltalake~=0.15', 'pyarrow>=11.0.0', 'snowflake-connector-python[pandas]~=3.6', 'snowflake-snowpark-python[pandas]~=1.0', 'pydantic<2', 'urllib3<1.27'], 'snowflake': ['snowflake-snowpark-python[pandas]~=1.0'], 'athena': ['awswrangler~=3.0'], 'materialization': ['statsd==3.3.0', 'urllib3<2.0.0']},
     packages=packages,
 )
```

### Comparing `tecton-0.9.3/tecton/__init__.py` & `tecton-0.9.4/tecton/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/analytics.py` & `tecton-0.9.4/tecton/_internals/analytics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/athena_api.py` & `tecton-0.9.4/tecton/_internals/athena_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/data_frame_helper.py` & `tecton-0.9.4/tecton/_internals/data_frame_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/delete_keys_api.py` & `tecton-0.9.4/tecton/_internals/delete_keys_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/display.py` & `tecton-0.9.4/tecton/_internals/display.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/env_utils.py` & `tecton-0.9.4/tecton/_internals/env_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/errors.py` & `tecton-0.9.4/tecton/_internals/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/find_spark.py` & `tecton-0.9.4/tecton/_internals/find_spark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/ingest_utils.py` & `tecton-0.9.4/tecton/_internals/ingest_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/ingestion.py` & `tecton-0.9.4/tecton/_internals/ingestion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/materialization_api.py` & `tecton-0.9.4/tecton/_internals/materialization_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/metadata_service.py` & `tecton-0.9.4/tecton/_internals/metadata_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/metadata_service_impl/request_lib.py` & `tecton-0.9.4/tecton/_internals/metadata_service_impl/request_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/metadata_service_impl/service_modules.py` & `tecton-0.9.4/tecton/_internals/metadata_service_impl/service_modules.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/mock_source_utils.py` & `tecton-0.9.4/tecton/_internals/mock_source_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/offline_store_credentials.py` & `tecton-0.9.4/tecton/_internals/offline_store_credentials.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,20 +7,34 @@
 from tecton_core.offline_store import S3Options
 from tecton_core.offline_store import S3OptionsSource
 from tecton_proto.common.id_pb2 import Id
 from tecton_proto.metadataservice.metadata_service_pb2 import GetOfflineStoreCredentialsRequest
 
 
 class MDSOfflineStoreOptionsProvider(OfflineStoreOptionsProvider):
-    def get_s3_options(self, feature_view_id: Id) -> Optional[S3Options]:
+    def get_s3_options_for_feature_view(self, feature_view_id: Id) -> Optional[S3Options]:
         if conf.get_bool("USE_LOCAL_OFFLINE_STORE_CREDENTIALS"):
             return None
-        response = metadata_service.instance().GetOfflineStoreCredentials(
-            GetOfflineStoreCredentialsRequest(feature_view_id=feature_view_id)
+        request = GetOfflineStoreCredentialsRequest(feature_view_id=feature_view_id)
+        response = metadata_service.instance().GetOfflineStoreCredentials(request)
+        if not response.HasField("aws"):
+            return None
+        return S3Options(
+            access_key_id=response.aws.access_key_id,
+            secret_access_key=response.aws.secret_access_key,
+            session_token=response.aws.session_token,
+            region=conf.get_or_raise("CLUSTER_REGION"),
+            options_source=S3OptionsSource.MDS,
         )
+
+    def get_s3_options_for_data_source(self, data_source_id: Id) -> Optional[S3Options]:
+        if conf.get_bool("USE_LOCAL_OFFLINE_STORE_CREDENTIALS"):
+            return None
+        request = GetOfflineStoreCredentialsRequest(data_source_id=data_source_id)
+        response = metadata_service.instance().GetOfflineStoreCredentials(request)
         if not response.HasField("aws"):
             return None
         return S3Options(
             access_key_id=response.aws.access_key_id,
             secret_access_key=response.aws.secret_access_key,
             session_token=response.aws.session_token,
             region=conf.get_or_raise("CLUSTER_REGION"),
```

### Comparing `tecton-0.9.3/tecton/_internals/pandas_compat.py` & `tecton-0.9.4/tecton/_internals/pandas_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/query_helper.py` & `tecton-0.9.4/tecton/_internals/query_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/querytree_api.py` & `tecton-0.9.4/tecton/_internals/querytree_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/repo/function_serialization.py` & `tecton-0.9.4/tecton/_internals/repo/function_serialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/rewrite.py` & `tecton-0.9.4/tecton/_internals/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/run_api.py` & `tecton-0.9.4/tecton/_internals/run_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/sdk_decorators.py` & `tecton-0.9.4/tecton/_internals/sdk_decorators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/secret_resolver.py` & `tecton-0.9.4/tecton/_internals/secret_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/snowflake_api.py` & `tecton-0.9.4/tecton/_internals/snowflake_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/spark_api.py` & `tecton-0.9.4/tecton/_internals/spark_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/spark_utils.py` & `tecton-0.9.4/tecton/_internals/spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/tecton_pydantic.py` & `tecton-0.9.4/tecton/_internals/tecton_pydantic.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/time_utils.py` & `tecton-0.9.4/tecton/_internals/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/type_utils.py` & `tecton-0.9.4/tecton/_internals/type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/utils.py` & `tecton-0.9.4/tecton/_internals/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/_internals/validations_api.py` & `tecton-0.9.4/tecton/_internals/validations_api.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/aggregation_functions.py` & `tecton-0.9.4/tecton/aggregation_functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/access_control.py` & `tecton-0.9.4/tecton/cli/access_control.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/api_key.py` & `tecton-0.9.4/tecton/cli/api_key.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/auth.py` & `tecton-0.9.4/tecton/cli/auth.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/cli.py` & `tecton-0.9.4/tecton/cli/cli.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/cli_utils.py` & `tecton-0.9.4/tecton/cli/cli_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/command.py` & `tecton-0.9.4/tecton/cli/command.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/completion.py` & `tecton-0.9.4/tecton/cli/completion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/engine.py` & `tecton-0.9.4/tecton/cli/engine.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/engine_renderer.py` & `tecton-0.9.4/tecton/cli/engine_renderer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/environment.py` & `tecton-0.9.4/tecton/cli/environment.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/environment_utils.py` & `tecton-0.9.4/tecton/cli/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/error_utils.py` & `tecton-0.9.4/tecton/cli/error_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/materialization.py` & `tecton-0.9.4/tecton/cli/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/pex_wrapper.py` & `tecton-0.9.4/tecton/cli/pex_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/printer.py` & `tecton-0.9.4/tecton/cli/printer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/repo.py` & `tecton-0.9.4/tecton/cli/repo.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/repo_config.py` & `tecton-0.9.4/tecton/cli/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/repo_utils.py` & `tecton-0.9.4/tecton/cli/repo_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/secrets.py` & `tecton-0.9.4/tecton/cli/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/service_account.py` & `tecton-0.9.4/tecton/cli/service_account.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/test.py` & `tecton-0.9.4/tecton/cli/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/user.py` & `tecton-0.9.4/tecton/cli/user.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/workspace.py` & `tecton-0.9.4/tecton/cli/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/cli/workspace_utils.py` & `tecton-0.9.4/tecton/cli/workspace_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/fco_listers.py` & `tecton-0.9.4/tecton/fco_listers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/base_tecton_object.py` & `tecton-0.9.4/tecton/framework/base_tecton_object.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/configs.py` & `tecton-0.9.4/tecton/framework/configs.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/data_frame.py` & `tecton-0.9.4/tecton/framework/data_frame.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/data_source.py` & `tecton-0.9.4/tecton/framework/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/dataset.py` & `tecton-0.9.4/tecton/framework/dataset.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/entity.py` & `tecton-0.9.4/tecton/framework/entity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/feature.py` & `tecton-0.9.4/tecton/framework/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/feature_service.py` & `tecton-0.9.4/tecton/framework/feature_service.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/feature_view.py` & `tecton-0.9.4/tecton/framework/feature_view.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/filtered_source.py` & `tecton-0.9.4/tecton/framework/filtered_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/repo_config.py` & `tecton-0.9.4/tecton/framework/repo_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/transformation.py` & `tecton-0.9.4/tecton/framework/transformation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/utils.py` & `tecton-0.9.4/tecton/framework/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/validation_mode.py` & `tecton-0.9.4/tecton/framework/validation_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/framework/workspace.py` & `tecton-0.9.4/tecton/framework/workspace.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/identities/api_keys.py` & `tecton-0.9.4/tecton/identities/api_keys.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/identities/credentials.py` & `tecton-0.9.4/tecton/identities/credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/identities/okta.py` & `tecton-0.9.4/tecton/identities/okta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/pytest_tecton.py` & `tecton-0.9.4/tecton/pytest_tecton.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/snowflake_context.py` & `tecton-0.9.4/tecton/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/tecton_context.py` & `tecton-0.9.4/tecton/tecton_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/types.py` & `tecton-0.9.4/tecton/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/__diff.py` & `tecton-0.9.4/tecton/vendor/dill/dill/__diff.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/__init__.py` & `tecton-0.9.4/tecton/vendor/dill/dill/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/_dill.py` & `tecton-0.9.4/tecton/vendor/dill/dill/_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/_objects.py` & `tecton-0.9.4/tecton/vendor/dill/dill/_objects.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/detect.py` & `tecton-0.9.4/tecton/vendor/dill/dill/detect.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/info.py` & `tecton-0.9.4/tecton/vendor/dill/dill/info.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/objtypes.py` & `tecton-0.9.4/tecton/vendor/dill/dill/objtypes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/pointers.py` & `tecton-0.9.4/tecton/vendor/dill/dill/pointers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/settings.py` & `tecton-0.9.4/tecton/vendor/dill/dill/settings.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/source.py` & `tecton-0.9.4/tecton/vendor/dill/dill/source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/dill/dill/temp.py` & `tecton-0.9.4/tecton/vendor/dill/dill/temp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/clientserver.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/clientserver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/compat.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/finalizer.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/finalizer.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/java_collections.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/java_collections.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/java_gateway.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/protocol.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/protocol.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/py4j/signals.py` & `tecton-0.9.4/tecton/vendor/pyspark/py4j/signals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/_globals.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/_globals.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/accumulators.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/accumulators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/broadcast.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/broadcast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/cloudpickle/cloudpickle_fast.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/conf.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/context.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/daemon.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/daemon.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/files.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/files.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/find_spark_home.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/find_spark_home.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/install.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/install.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/java_gateway.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/java_gateway.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/join.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/base.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/base.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/classification.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/clustering.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/common.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/evaluation.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/feature.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/fpm.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/functions.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/image.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/image.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/_shared_params_code_gen.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/param/shared.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/param/shared.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/pipeline.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/recommendation.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/regression.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/stat.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/stat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/tree.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/tuning.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/tuning.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/util.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/ml/wrapper.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/ml/wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/classification.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/classification.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/clustering.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/clustering.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/common.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/evaluation.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/evaluation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/feature.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/feature.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/fpm.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/fpm.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/linalg/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/linalg/distributed.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/random.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/random.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/recommendation.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/recommendation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/regression.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/regression.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/KernelDensity.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/_statistics.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/distribution.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/stat/test.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/stat/test.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/tree.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/mllib/util.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/mllib/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/profiler.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/profiler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/python/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/rdd.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/rdd.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/rddsampler.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/rddsampler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/information.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/information.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/profile.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/profile.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/resource/requests.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/resource/requests.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/resultiterable.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/resultiterable.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/serializers.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/shell.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/shell.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/shuffle.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/shuffle.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/avro/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/avro/functions.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/avro/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/catalog.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/catalog.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/column.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/column.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/conf.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/context.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/dataframe.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/dataframe.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/functions.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/group.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/group.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/conversion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/functions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/group_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/map_ops.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/serializers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/typehints.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/types.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/pandas/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/readwriter.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/readwriter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/session.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/streaming.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/streaming.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/types.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/udf.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/udf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/utils.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/sql/window.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/sql/window.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/statcounter.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/statcounter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/status.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/storagelevel.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/storagelevel.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/__init__.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/context.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/dstream.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/dstream.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/kinesis.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/kinesis.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/listener.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/listener.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/streaming/util.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/streaming/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/taskcontext.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/taskcontext.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/traceback_utils.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/traceback_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/util.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/util.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/pyspark/pyspark/worker.py` & `tecton-0.9.4/tecton/vendor/pyspark/pyspark/worker.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/vendor_dill.py` & `tecton-0.9.4/tecton/vendor/vendor_dill.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/vendor/vendor_pyspark.py` & `tecton-0.9.4/tecton/vendor/vendor_pyspark.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton/version.py` & `tecton-0.9.4/tecton/version.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton.egg-info/PKG-INFO` & `tecton-0.9.4/tecton.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tecton
-Version: 0.9.3
+Version: 0.9.4
 Summary: Tecton Python SDK
 Home-page: https://tecton.ai
 Author: Tecton, Inc.
 Author-email: support@tecton.ai
 License: Tecton Proprietary
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `tecton-0.9.3/tecton.egg-info/SOURCES.txt` & `tecton-0.9.4/tecton.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton.egg-info/requires.txt` & `tecton-0.9.4/tecton.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/athena_session.py` & `tecton-0.9.4/tecton_athena/athena_session.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/data_catalog_helper.py` & `tecton-0.9.4/tecton_athena/data_catalog_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/odfv_helper.py` & `tecton-0.9.4/tecton_athena/odfv_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/query/translate.py` & `tecton-0.9.4/tecton_athena/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/sql_helper.py` & `tecton-0.9.4/tecton_athena/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates/create_table.sql` & `tecton-0.9.4/tecton_athena/templates/create_table.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates/historical_features.sql` & `tecton-0.9.4/tecton_athena/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates/materialization_tile.sql` & `tecton-0.9.4/tecton_athena/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates/run_full_aggregation.sql` & `tecton-0.9.4/tecton_athena/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates/time_limit.sql` & `tecton-0.9.4/tecton_athena/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_athena/templates_utils.py` & `tecton-0.9.4/tecton_athena/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/aggregation_utils.py` & `tecton-0.9.4/tecton_core/aggregation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/arrow.py` & `tecton-0.9.4/tecton_core/arrow.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/aws_credentials.py` & `tecton-0.9.4/tecton_core/aws_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/compute_mode.py` & `tecton-0.9.4/tecton_core/compute_mode.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/conf.py` & `tecton-0.9.4/tecton_core/conf.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/data_types.py` & `tecton-0.9.4/tecton_core/data_types.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/duckdb_context.py` & `tecton-0.9.4/tecton_core/duckdb_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/errors.py` & `tecton-0.9.4/tecton_core/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/fco_container.py` & `tecton-0.9.4/tecton_core/fco_container.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/feature_definition_wrapper.py` & `tecton-0.9.4/tecton_core/feature_definition_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/feature_set_config.py` & `tecton-0.9.4/tecton_core/feature_set_config.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/feature_view_utils.py` & `tecton-0.9.4/tecton_core/feature_view_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/function_deserialization.py` & `tecton-0.9.4/tecton_core/function_deserialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/http.py` & `tecton-0.9.4/tecton_core/http.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/id_helper.py` & `tecton-0.9.4/tecton_core/id_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/iterators.py` & `tecton-0.9.4/tecton_core/iterators.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/materialization_context.py` & `tecton-0.9.4/tecton_core/materialization_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/metadata_service_impl/error_lib.py` & `tecton-0.9.4/tecton_core/metadata_service_impl/error_lib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/metadata_service_impl/http_client.py` & `tecton-0.9.4/tecton_core/metadata_service_impl/http_client.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/metadata_service_impl/providers.py` & `tecton-0.9.4/tecton_core/metadata_service_impl/providers.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/metadata_service_impl/response.py` & `tecton-0.9.4/tecton_core/metadata_service_impl/response.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/metadata_service_impl/service_calls.py` & `tecton-0.9.4/tecton_core/metadata_service_impl/service_calls.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/offline_store.py` & `tecton-0.9.4/tecton_core/offline_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -278,15 +278,18 @@
             opts["AWS_SESSION_TOKEN"] = self.session_token
         if self.region:
             opts["AWS_REGION"] = self.region
         return opts
 
 
 class OfflineStoreOptionsProvider:
-    def get_s3_options(self, feature_view_id: Id) -> Optional[S3Options]:
+    def get_s3_options_for_feature_view(self, feature_view_id: Id) -> Optional[S3Options]:
+        return
+
+    def get_s3_options_for_data_source(self, data_source_id: Id) -> Optional[S3Options]:
         return
 
 
 class BotoOfflineStoreOptionsProvider(OfflineStoreOptionsProvider):
     """deltalake's built-in S3 auth is implemented by a Rust library which doesn't support the full range of AWS
     auth configurations supported by boto, which can be surprising to users used to boto's options. This class
     following does a fully-featured auth using boto instead of depending on Rust.
@@ -326,26 +329,31 @@
         return S3Options(
             access_key_id=credentials["AccessKeyId"],
             secret_access_key=credentials["SecretAccessKey"],
             session_token=credentials["SessionToken"],
             options_source=S3OptionsSource.LOCAL,
         )
 
-    def get_s3_options(self, feature_view_id: Id) -> Optional[S3Options]:
+    def get_s3_options_for_feature_view(self, feature_view_id: Id) -> Optional[S3Options]:
+        return BotoOfflineStoreOptionsProvider.static_options()
+
+    def get_s3_options_for_data_source(self, data_source_id: Id) -> Optional[S3Options]:
         return BotoOfflineStoreOptionsProvider.static_options()
 
 
 DEFAULT_OPTIONS_PROVIDERS = [BotoOfflineStoreOptionsProvider()]
 
 
 def get_s3_options_for_fd(
     fd: FeatureDefinitionWrapper, options_providers: Iterable[OfflineStoreOptionsProvider]
 ) -> S3Options:
     fvid = id_helper.IdHelper.from_string(fd.id)
-    options = next(filter(lambda o: o is not None, (p.get_s3_options(fvid) for p in options_providers)), None)
+    options = next(
+        filter(lambda o: o is not None, (p.get_s3_options_for_feature_view(fvid) for p in options_providers)), None
+    )
     if options is None:
         msg = f"Unable to retrieve S3 store credentials for feature view {fd.name}."
         raise ValueError(msg)
 
     return options
```

### Comparing `tecton-0.9.3/tecton_core/online_serving_index.py` & `tecton-0.9.4/tecton_core/online_serving_index.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/pipeline_common.py` & `tecton-0.9.4/tecton_core/pipeline_common.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/aggregation_plans.py` & `tecton-0.9.4/tecton_core/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/builder.py` & `tecton-0.9.4/tecton_core/query/builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/compaction_utils.py` & `tecton-0.9.4/tecton_core/query/compaction_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/duckdb/compute.py` & `tecton-0.9.4/tecton_core/query/duckdb/compute.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import dataclasses
 import logging
 import re
+import time
 import typing
+from typing import Iterable
 from typing import Optional
 from typing import Union
 
 import attrs
 
 
 try:
@@ -18,32 +20,36 @@
     raise RuntimeError(msg)
 import pandas as pd
 import pyarrow
 import pyarrow.dataset
 import pyarrow.fs
 import pyarrow.json
 import sqlparse
+from deltalake import DeltaTable
 from duckdb import DuckDBPyConnection
 
 from tecton_core import conf
+from tecton_core import id_helper
 from tecton_core.duckdb_context import DuckDBContext
 from tecton_core.errors import TectonValidationError
 from tecton_core.offline_store import BotoOfflineStoreOptionsProvider
+from tecton_core.offline_store import OfflineStoreOptionsProvider
 from tecton_core.query.dialect import Dialect
 from tecton_core.query.errors import SQLCompilationError
 from tecton_core.query.errors import UserCodeError
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.nodes import DataSourceScanNode
 from tecton_core.query.query_tree_compute import ComputeMonitor
 from tecton_core.query.query_tree_compute import SQLCompute
 from tecton_core.schema import Schema
 from tecton_core.schema_validation import CastError
 from tecton_core.schema_validation import tecton_schema_to_arrow_schema
 from tecton_core.secrets import SecretResolver
 from tecton_core.specs import FileSourceSpec
+from tecton_core.specs import PushTableSourceSpec
 from tecton_core.time_utils import get_timezone_aware_datetime
 from tecton_proto.data import batch_data_source_pb2
 
 
 @dataclasses.dataclass
 class _Cause:
     type_name: str
@@ -66,18 +72,21 @@
 
 
 @attrs.define
 class DuckDBCompute(SQLCompute):
     session: "DuckDBPyConnection"
     is_debug: bool = attrs.field(init=False)
     created_views: typing.List[str] = attrs.field(init=False)
+    offline_store_options: Iterable[OfflineStoreOptionsProvider] = ()
 
     @staticmethod
-    def from_context() -> "DuckDBCompute":
-        return DuckDBCompute(session=DuckDBContext.get_instance().get_connection())
+    def from_context(offline_store_options: Iterable[OfflineStoreOptionsProvider] = ()) -> "DuckDBCompute":
+        return DuckDBCompute(
+            session=DuckDBContext.get_instance().get_connection(), offline_store_options=offline_store_options
+        )
 
     def __attrs_post_init__(self):
         self.is_debug = conf.get_bool("DUCKDB_DEBUG")
         self.created_views = []
 
     def run_sql(
         self,
@@ -149,90 +158,135 @@
     def register_temp_table_from_data_source(
         self,
         table_name: str,
         ds: DataSourceScanNode,
         secret_resolver: Optional[SecretResolver] = None,
         monitor: Optional[ComputeMonitor] = None,
     ) -> None:
-        assert isinstance(ds.ds.batch_source, (FileSourceSpec,)), "DuckDB compute supports only File data sources"
-
-        batch_source_spec = ds.ds.batch_source
-        file_uri = batch_source_spec.uri
-        timestamp_field = batch_source_spec.timestamp_field
-
-        # ToDo: log loading progress via ComputeMonitor
-        schema = Schema(ds.ds.schema.tecton_schema) if ds.ds.schema else None
-        arrow_schema = tecton_schema_to_arrow_schema(schema) if schema else None
-        if batch_source_spec.timestamp_format:
-            # replace timestamp column type with string,
-            # we will convert timestamp with DuckDB (see below)
-            timestamp_pos = arrow_schema.names.index(timestamp_field)
-            arrow_schema = arrow_schema.set(timestamp_pos, pyarrow.field(timestamp_field, pyarrow.string()))
-
-        proto_format = batch_source_spec.file_format
-        if proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_CSV:
-            arrow_format = "csv"
-        elif proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_JSON:
-            arrow_format = "json"
-        elif proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_PARQUET:
-            arrow_format = "parquet"
-        else:
-            raise ValueError(batch_data_source_pb2.FileDataSourceFormat.Name(batch_source_spec.file_format))
-
-        fs, path = pyarrow.fs.FileSystem.from_uri(file_uri)
-        if isinstance(fs, pyarrow.fs.S3FileSystem):
-            options = BotoOfflineStoreOptionsProvider.static_options()
-            if options is not None:
-                fs = pyarrow.fs.S3FileSystem(
-                    access_key=options.access_key_id,
-                    secret_key=options.secret_access_key,
-                    session_token=options.session_token,
-                    # When created via Filesystem.from_uri, the bucket region will be autodetected. This constructor
-                    # does not have a bucket from which it can detect the region, so we need to copy it over from the
-                    # previous instance.
-                    region=fs.region,
-                )
-
-        # There seems to be a bug in Arrow related to the explicit schema:
-        # when we pass an explicit schema to `dataset` and both resolution and timezone in the timestamp column
-        # don't match the schema in parquet files - filters that are pushed down by DuckDB will not work.
-        # It is very likely that we will not guess both resolution and timezone correctly.
-        # So we won't pass schema for now.
-        arrow_schema = arrow_schema if arrow_format != "parquet" else None
-        file_ds = pyarrow.dataset.dataset(source=path, schema=arrow_schema, filesystem=fs, format=arrow_format)
-        if batch_source_spec.post_processor:
-            reader = pyarrow.RecordBatchReader.from_batches(file_ds.schema, file_ds.to_batches())
-            input_df = reader.read_pandas()
-            try:
-                processed_df = batch_source_spec.post_processor(input_df)
-            except Exception as exc:
-                msg = "Post processor function of data source " f"('{ds.ds.name}') " f"failed with exception"
-                raise UserCodeError(msg) from exc
+        assert isinstance(
+            ds.ds.batch_source,
+            (
+                FileSourceSpec,
+                PushTableSourceSpec,
+            ),
+        ), "DuckDB compute supports only File and Push Table data sources"
+        if isinstance(ds.ds.batch_source, FileSourceSpec):
+            batch_source_spec = ds.ds.batch_source
+            file_uri = batch_source_spec.uri
+            timestamp_field = batch_source_spec.timestamp_field
+
+            # ToDo: log loading progress via ComputeMonitor
+            schema = Schema(ds.ds.schema.tecton_schema) if ds.ds.schema else None
+            arrow_schema = tecton_schema_to_arrow_schema(schema) if schema else None
+            if batch_source_spec.timestamp_format:
+                # replace timestamp column type with string,
+                # we will convert timestamp with DuckDB (see below)
+                timestamp_pos = arrow_schema.names.index(timestamp_field)
+                arrow_schema = arrow_schema.set(timestamp_pos, pyarrow.field(timestamp_field, pyarrow.string()))
+
+            proto_format = batch_source_spec.file_format
+            if proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_CSV:
+                arrow_format = "csv"
+            elif proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_JSON:
+                arrow_format = "json"
+            elif proto_format == batch_data_source_pb2.FILE_DATA_SOURCE_FORMAT_PARQUET:
+                arrow_format = "parquet"
             else:
-                relation = self.session.from_df(processed_df)
-        else:
-            relation = self.session.from_arrow(file_ds)
+                raise ValueError(batch_data_source_pb2.FileDataSourceFormat.Name(batch_source_spec.file_format))
 
-        column_types = dict(zip(relation.columns, relation.dtypes))
-        if ds.start_time:
-            if column_types[timestamp_field] == duckdb.typing.TIMESTAMP_TZ:
-                start_time = get_timezone_aware_datetime(ds.start_time)
+            fs, path = pyarrow.fs.FileSystem.from_uri(file_uri)
+            if isinstance(fs, pyarrow.fs.S3FileSystem):
+                options = BotoOfflineStoreOptionsProvider.static_options()
+                if options is not None:
+                    fs = pyarrow.fs.S3FileSystem(
+                        access_key=options.access_key_id,
+                        secret_key=options.secret_access_key,
+                        session_token=options.session_token,
+                        # When created via Filesystem.from_uri, the bucket region will be autodetected. This constructor
+                        # does not have a bucket from which it can detect the region, so we need to copy it over from the
+                        # previous instance.
+                        region=fs.region,
+                    )
+
+            # There seems to be a bug in Arrow related to the explicit schema:
+            # when we pass an explicit schema to `dataset` and both resolution and timezone in the timestamp column
+            # don't match the schema in parquet files - filters that are pushed down by DuckDB will not work.
+            # It is very likely that we will not guess both resolution and timezone correctly.
+            # So we won't pass schema for now.
+            arrow_schema = arrow_schema if arrow_format != "parquet" else None
+            file_ds = pyarrow.dataset.dataset(source=path, schema=arrow_schema, filesystem=fs, format=arrow_format)
+            if batch_source_spec.post_processor:
+                reader = pyarrow.RecordBatchReader.from_batches(file_ds.schema, file_ds.to_batches())
+                input_df = reader.read_pandas()
+                try:
+                    processed_df = batch_source_spec.post_processor(input_df)
+                except Exception as exc:
+                    msg = "Post processor function of data source " f"('{ds.ds.name}') " f"failed with exception"
+                    raise UserCodeError(msg) from exc
+                else:
+                    relation = self.session.from_df(processed_df)
             else:
-                start_time = ds.start_time.replace(tzinfo=None)
-            relation = relation.filter(f"\"{timestamp_field}\" >= '{start_time}'")
-        if ds.end_time:
-            if column_types[timestamp_field] == duckdb.typing.TIMESTAMP_TZ:
-                end_time = get_timezone_aware_datetime(ds.end_time)
-            else:
-                end_time = ds.end_time.replace(tzinfo=None)
-            relation = relation.filter(f"\"{timestamp_field}\" < '{end_time}'")
+                relation = self.session.from_arrow(file_ds)
+
+            column_types = dict(zip(relation.columns, relation.dtypes))
 
-        if batch_source_spec.timestamp_format:
-            conversion_exp = f"strptime(\"{timestamp_field}\", '{batch_source_spec.timestamp_format}')"
-            relation = relation.select(f'* REPLACE({conversion_exp} AS "{timestamp_field}")')
+            if ds.start_time:
+                if column_types[timestamp_field] == duckdb.typing.TIMESTAMP_TZ:
+                    start_time = get_timezone_aware_datetime(ds.start_time)
+                else:
+                    start_time = ds.start_time.replace(tzinfo=None)
+                relation = relation.filter(f"\"{timestamp_field}\" >= '{start_time}'")
+            if ds.end_time:
+                if column_types[timestamp_field] == duckdb.typing.TIMESTAMP_TZ:
+                    end_time = get_timezone_aware_datetime(ds.end_time)
+                else:
+                    end_time = ds.end_time.replace(tzinfo=None)
+                relation = relation.filter(f"\"{timestamp_field}\" < '{end_time}'")
+
+            if batch_source_spec.timestamp_format:
+                conversion_exp = f"strptime(\"{timestamp_field}\", '{batch_source_spec.timestamp_format}')"
+                relation = relation.select(f'* REPLACE({conversion_exp} AS "{timestamp_field}")')
+
+        elif isinstance(ds.ds.batch_source, PushTableSourceSpec):
+            ds_id = id_helper.IdHelper.from_string(ds.ds.id)
+            creds = next(
+                filter(
+                    lambda o: o is not None,
+                    (p.get_s3_options_for_data_source(ds_id) for p in self.offline_store_options),
+                ),
+                None,
+            )
+            if not creds:
+                msg = f"Unable to retrieve S3 store credentials for data source {ds.ds.name}"
+                raise Exception(msg)
+            storage_options = {
+                "AWS_ACCESS_KEY_ID": creds.access_key_id,
+                "AWS_SECRET_ACCESS_KEY": creds.secret_access_key,
+                "AWS_SESSION_TOKEN": creds.session_token,
+                "AWS_S3_LOCKING_PROVIDER": "dynamodb",
+                "AWS_REGION": conf.get_or_raise("CLUSTER_REGION"),
+            }
+            saved_error = None
+            for _ in range(20):
+                try:
+                    table = DeltaTable(
+                        table_uri=ds.ds.batch_source.ingested_data_location, storage_options=storage_options
+                    )
+                    break
+                except OSError as e:
+                    saved_error = e
+                    time.sleep(0.1)
+            else:
+                msg = "Failed to read from S3"
+                raise TimeoutError(msg) from saved_error
+            df = table.to_pyarrow_dataset()
+            relation = self.session.from_arrow(df)
+        else:
+            msg = "DuckDB compute supports only File data sources and Push Table data sources"
+            raise Exception(msg)
 
         relation.create_view(table_name)
         self.created_views.append(table_name)
 
     def load_table(self, table_name: str, expected_output_schema: Optional[Schema] = None) -> pyarrow.RecordBatchReader:
         return self.run_sql(
             f"select * from {table_name}", return_dataframe=True, expected_output_schema=expected_output_schema
```

### Comparing `tecton-0.9.3/tecton_core/query/duckdb/nodes.py` & `tecton-0.9.4/tecton_core/query/duckdb/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/duckdb/rewrite.py` & `tecton-0.9.4/tecton_core/query/duckdb/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/errors.py` & `tecton-0.9.4/tecton_core/query/errors.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/executor_params.py` & `tecton-0.9.4/tecton_core/query/executor_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/executor_utils.py` & `tecton-0.9.4/tecton_core/query/executor_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/node_interface.py` & `tecton-0.9.4/tecton_core/query/node_interface.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/node_utils.py` & `tecton-0.9.4/tecton_core/query/node_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
     encountered_dialects = set()
 
     def _extract_dialect_from_ds(node: DataSourceScanNode) -> None:
         nonlocal encountered_dialects
         batch_source = node.ds.batch_source
         if isinstance(batch_source, specs.PandasBatchSourceSpec):
             encountered_dialects.add(tecton_core.query.dialect.Dialect.PANDAS)
-        elif isinstance(batch_source, specs.FileSourceSpec):
+        elif isinstance(batch_source, (specs.FileSourceSpec, specs.PushTableSourceSpec)):
             encountered_dialects.add(tecton_core.query.dialect.Dialect.DUCKDB)
         elif isinstance(batch_source, specs.SnowflakeSourceSpec):
             encountered_dialects.add(tecton_core.query.dialect.Dialect.SNOWFLAKE)
         else:
             msg = f"Unexpected data source type encountered: {batch_source.__class__}"
             raise Exception(msg)
```

### Comparing `tecton-0.9.3/tecton_core/query/nodes.py` & `tecton-0.9.4/tecton_core/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/compute.py` & `tecton-0.9.4/tecton_core/query/pandas/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/node.py` & `tecton-0.9.4/tecton_core/query/pandas/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/nodes.py` & `tecton-0.9.4/tecton_core/query/pandas/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/pipeline_helper.py` & `tecton-0.9.4/tecton_core/query/pandas/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/rewrite.py` & `tecton-0.9.4/tecton_core/query/pandas/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pandas/translate.py` & `tecton-0.9.4/tecton_core/query/pandas/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/pipeline_sql_builder.py` & `tecton-0.9.4/tecton_core/query/pipeline_sql_builder.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/prefixed_uri_resolver.py` & `tecton-0.9.4/tecton_core/query/prefixed_uri_resolver.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/query_tree_compute.py` & `tecton-0.9.4/tecton_core/query/query_tree_compute.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import contextlib
 import logging
 from abc import ABC
 from abc import abstractmethod
 from typing import Callable
+from typing import Iterable
 from typing import Optional
 from typing import Union
 
 import attrs
 import pandas as pd
 import pyarrow
 
+from tecton_core.offline_store import OfflineStoreOptionsProvider
 from tecton_core.query.dialect import Dialect
 from tecton_core.query.node_interface import NodeRef
 from tecton_core.query.nodes import DataSourceScanNode
 from tecton_core.schema import Schema
 from tecton_core.secrets import SecretResolver
 
 
@@ -38,29 +40,32 @@
 class SQLCompute(QueryTreeCompute, contextlib.AbstractContextManager):
     """
     Base class for compute backed by a SQL engine (e.g. Snowflake and DuckDB).
     """
 
     @staticmethod
     def for_dialect(
-        dialect: Dialect, qt_root: Optional[NodeRef] = None, secret_resolver: Optional[SecretResolver] = None
+        dialect: Dialect,
+        qt_root: Optional[NodeRef] = None,
+        secret_resolver: Optional[SecretResolver] = None,
+        offline_store_options: Iterable[OfflineStoreOptionsProvider] = (),
     ) -> "SQLCompute":
         # Conditional imports are used so that optional dependencies such as the Snowflake connector are only imported
         # if they're needed for a query
         if dialect == Dialect.SNOWFLAKE:
             from tecton_core.query.snowflake.compute import SnowflakeCompute
             from tecton_core.query.snowflake.compute import create_snowflake_connection
 
             if SnowflakeCompute.is_context_initialized():
                 return SnowflakeCompute.from_context()
             return SnowflakeCompute.for_connection(create_snowflake_connection(qt_root, secret_resolver))
         if dialect == Dialect.DUCKDB:
             from tecton_core.query.duckdb.compute import DuckDBCompute
 
-            return DuckDBCompute.from_context()
+            return DuckDBCompute.from_context(offline_store_options=offline_store_options)
         if dialect == Dialect.PANDAS:
             from tecton_core.query.pandas.compute import PandasCompute
 
             return PandasCompute.from_context()
 
     @abstractmethod
     def get_dialect(self) -> Dialect:
```

### Comparing `tecton-0.9.3/tecton_core/query/query_tree_executor.py` & `tecton-0.9.4/tecton_core/query/query_tree_executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -210,15 +210,20 @@
         for name, staging_node in staging_nodes_to_process.items():
             data_source_node_ref = staging_node.input_node
             data_source_node = data_source_node_ref.node
 
             # No data source dialect will be returned for MockedDataSource
             dialect = get_data_source_dialect(data_source_node_ref) or Dialect.DUCKDB
             with self._monitor_stage("Reading Data Source", dialect=dialect) as monitor:
-                compute = SQLCompute.for_dialect(dialect, qt_root, secret_resolver=self.secret_resolver)
+                compute = SQLCompute.for_dialect(
+                    dialect,
+                    qt_root,
+                    secret_resolver=self.secret_resolver,
+                    offline_store_options=self.offline_store_options_providers,
+                )
 
                 assert isinstance(data_source_node, (DataSourceScanNode, MockDataSourceScanNode))
 
                 if not isinstance(data_source_node, MockDataSourceScanNode):
                     compute.register_temp_table_from_data_source(name, data_source_node, self.secret_resolver, monitor)
                     if dialect == get_pipeline_dialect(qt_root) and dialect != Dialect.PANDAS:
                         # No need to export from compute, it will be shared between stages
```

### Comparing `tecton-0.9.3/tecton_core/query/snowflake/compute.py` & `tecton-0.9.4/tecton_core/query/snowflake/compute.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query/sql_compat.py` & `tecton-0.9.4/tecton_core/query/sql_compat.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/query_consts.py` & `tecton-0.9.4/tecton_core/query_consts.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/repo_file_handler.py` & `tecton-0.9.4/tecton_core/repo_file_handler.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/request_context.py` & `tecton-0.9.4/tecton_core/request_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/schema.py` & `tecton-0.9.4/tecton_core/schema.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/schema_derivation_utils.py` & `tecton-0.9.4/tecton_core/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/schema_validation.py` & `tecton-0.9.4/tecton_core/schema_validation.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/secrets.py` & `tecton-0.9.4/tecton_core/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/snowflake_context.py` & `tecton-0.9.4/tecton_core/snowflake_context.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/__init__.py` & `tecton-0.9.4/tecton_core/specs/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/data_source_spec.py` & `tecton-0.9.4/tecton_core/specs/data_source_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/entity_spec.py` & `tecton-0.9.4/tecton_core/specs/entity_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/feature_service_spec.py` & `tecton-0.9.4/tecton_core/specs/feature_service_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/feature_view_spec.py` & `tecton-0.9.4/tecton_core/specs/feature_view_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/tecton_object_spec.py` & `tecton-0.9.4/tecton_core/specs/tecton_object_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/time_window_spec.py` & `tecton-0.9.4/tecton_core/specs/time_window_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/transformation_spec.py` & `tecton-0.9.4/tecton_core/specs/transformation_spec.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/specs/utils.py` & `tecton-0.9.4/tecton_core/specs/utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/time_utils.py` & `tecton-0.9.4/tecton_core/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/queue.py` & `tecton-0.9.4/tecton_core/vendor/queue.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/__init__.py` & `tecton-0.9.4/tecton_core/vendor/treelib/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/exceptions.py` & `tecton-0.9.4/tecton_core/vendor/treelib/exceptions.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/misc.py` & `tecton-0.9.4/tecton_core/vendor/treelib/misc.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/node.py` & `tecton-0.9.4/tecton_core/vendor/treelib/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/plugins.py` & `tecton-0.9.4/tecton_core/vendor/treelib/plugins.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/treelib/tree.py` & `tecton-0.9.4/tecton_core/vendor/treelib/tree.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_core/vendor/vendor_treelib.py` & `tecton-0.9.4/tecton_core/vendor/vendor_treelib.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/__init__.py` & `tecton-0.9.4/tecton_materialization/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/batch_materialization.py` & `tecton-0.9.4/tecton_materialization/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/common/job_metadata.py` & `tecton-0.9.4/tecton_materialization/common/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/common/job_metadata_aws.py` & `tecton-0.9.4/tecton_materialization/common/job_metadata_aws.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/common/job_metadata_gcp.py` & `tecton-0.9.4/tecton_materialization/common/job_metadata_gcp.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/common/task_params.py` & `tecton-0.9.4/tecton_materialization/common/task_params.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/consumption.py` & `tecton-0.9.4/tecton_materialization/consumption.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/delta_maintenance.py` & `tecton-0.9.4/tecton_materialization/delta_maintenance.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/entity_deletion.py` & `tecton-0.9.4/tecton_materialization/entity_deletion.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/feature_export.py` & `tecton-0.9.4/tecton_materialization/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ingest_materialization.py` & `tecton-0.9.4/tecton_materialization/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/job_metadata.py` & `tecton-0.9.4/tecton_materialization/job_metadata.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/materialization.py` & `tecton-0.9.4/tecton_materialization/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/materialization_utils.py` & `tecton-0.9.4/tecton_materialization/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/batch_materialization.py` & `tecton-0.9.4/tecton_materialization/ray/batch_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/delta.py` & `tecton-0.9.4/tecton_materialization/ray/delta.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/feature_export.py` & `tecton-0.9.4/tecton_materialization/ray/feature_export.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/ingest_materialization.py` & `tecton-0.9.4/tecton_materialization/ray/ingest_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/job_status.py` & `tecton-0.9.4/tecton_materialization/ray/job_status.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/materialization.py` & `tecton-0.9.4/tecton_materialization/ray/materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/materialization_utils.py` & `tecton-0.9.4/tecton_materialization/ray/materialization_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/ray/nodes.py` & `tecton-0.9.4/tecton_materialization/ray/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/remote_host/pyspark_remote_host.py` & `tecton-0.9.4/tecton_materialization/remote_host/pyspark_remote_host.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/secrets.py` & `tecton-0.9.4/tecton_materialization/secrets.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_materialization/stream_materialization.py` & `tecton-0.9.4/tecton_materialization/stream_materialization.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/amplitude/amplitude_pb2.py` & `tecton-0.9.4/tecton_proto/amplitude/amplitude_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/amplitude/client_logging_pb2.py` & `tecton-0.9.4/tecton_proto/amplitude/client_logging_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/api/featureservice/feature_service_pb2.py` & `tecton-0.9.4/tecton_proto/api/featureservice/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/api/featureservice/feature_service_request_pb2.py` & `tecton-0.9.4/tecton_proto/api/featureservice/feature_service_request_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/basic_info_pb2.py` & `tecton-0.9.4/tecton_proto/args/basic_info_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/data_source_config_pb2.py` & `tecton-0.9.4/tecton_proto/args/data_source_config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/data_source_pb2.py` & `tecton-0.9.4/tecton_proto/args/data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/diff_options_pb2.py` & `tecton-0.9.4/tecton_proto/args/diff_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/diff_test_pb2.py` & `tecton-0.9.4/tecton_proto/args/diff_test_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/entity_pb2.py` & `tecton-0.9.4/tecton_proto/args/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/fco_args_pb2.py` & `tecton-0.9.4/tecton_proto/args/fco_args_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/feature_service_pb2.py` & `tecton-0.9.4/tecton_proto/args/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/feature_view_pb2.py` & `tecton-0.9.4/tecton_proto/args/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/pipeline_pb2.py` & `tecton-0.9.4/tecton_proto/args/pipeline_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/repo_metadata_pb2.py` & `tecton-0.9.4/tecton_proto/args/repo_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/transformation_pb2.py` & `tecton-0.9.4/tecton_proto/args/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/user_defined_function_pb2.py` & `tecton-0.9.4/tecton_proto/args/user_defined_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/version_constraints_pb2.py` & `tecton-0.9.4/tecton_proto/args/version_constraints_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/args/virtual_data_source_pb2.py` & `tecton-0.9.4/tecton_proto/args/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auditlog/metadata_pb2.py` & `tecton-0.9.4/tecton_proto/auditlog/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/acl_pb2.py` & `tecton-0.9.4/tecton_proto/auth/acl_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/authorization_service_pb2.py` & `tecton-0.9.4/tecton_proto/auth/authorization_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/principal_pb2.py` & `tecton-0.9.4/tecton_proto/auth/principal_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/resource_pb2.py` & `tecton-0.9.4/tecton_proto/auth/resource_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/resource_role_assignments_pb2.py` & `tecton-0.9.4/tecton_proto/auth/resource_role_assignments_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/auth/service_pb2.py` & `tecton-0.9.4/tecton_proto/auth/service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/canary/type_pb2.py` & `tecton-0.9.4/tecton_proto/canary/type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/canary/update_pb2.py` & `tecton-0.9.4/tecton_proto/canary/update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/cli/repo_diff_pb2.py` & `tecton-0.9.4/tecton_proto/cli/repo_diff_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/aggregation_function_pb2.py` & `tecton-0.9.4/tecton_proto/common/aggregation_function_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/analytics_options_pb2.py` & `tecton-0.9.4/tecton_proto/common/analytics_options_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/aws_credentials_pb2.py` & `tecton-0.9.4/tecton_proto/common/aws_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/column_type_pb2.py` & `tecton-0.9.4/tecton_proto/common/column_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/compute_mode_pb2.py` & `tecton-0.9.4/tecton_proto/common/compute_mode_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/container_image_pb2.py` & `tecton-0.9.4/tecton_proto/common/container_image_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/data_source_type_pb2.py` & `tecton-0.9.4/tecton_proto/common/data_source_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/data_type_pb2.py` & `tecton-0.9.4/tecton_proto/common/data_type_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/fco_locator_pb2.py` & `tecton-0.9.4/tecton_proto/common/fco_locator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/framework_version_pb2.py` & `tecton-0.9.4/tecton_proto/common/framework_version_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/id_pb2.py` & `tecton-0.9.4/tecton_proto/common/id_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/pair_pb2.py` & `tecton-0.9.4/tecton_proto/common/pair_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/schema_container_pb2.py` & `tecton-0.9.4/tecton_proto/common/schema_container_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/schema_pb2.py` & `tecton-0.9.4/tecton_proto/common/schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/secret_pb2.py` & `tecton-0.9.4/tecton_proto/common/secret_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/spark_schema_pb2.py` & `tecton-0.9.4/tecton_proto/common/spark_schema_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/common/time_window_pb2.py` & `tecton-0.9.4/tecton_proto/common/time_window_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/consumption/consumption_pb2.py` & `tecton-0.9.4/tecton_proto/consumption/consumption_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/batch_data_source_pb2.py` & `tecton-0.9.4/tecton_proto/data/batch_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/entity_pb2.py` & `tecton-0.9.4/tecton_proto/data/entity_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/fco_metadata_pb2.py` & `tecton-0.9.4/tecton_proto/data/fco_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/fco_pb2.py` & `tecton-0.9.4/tecton_proto/data/fco_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/feature_service_pb2.py` & `tecton-0.9.4/tecton_proto/data/feature_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/feature_store_pb2.py` & `tecton-0.9.4/tecton_proto/data/feature_store_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/feature_view_pb2.py` & `tecton-0.9.4/tecton_proto/data/feature_view_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/freshness_status_pb2.py` & `tecton-0.9.4/tecton_proto/data/freshness_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/fv_materialization_pb2.py` & `tecton-0.9.4/tecton_proto/data/fv_materialization_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/hive_metastore_pb2.py` & `tecton-0.9.4/tecton_proto/data/hive_metastore_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/internal_spark_cluster_status_pb2.py` & `tecton-0.9.4/tecton_proto/data/internal_spark_cluster_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/materialization_roles_allowlists_pb2.py` & `tecton-0.9.4/tecton_proto/data/materialization_roles_allowlists_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/materialization_status_pb2.py` & `tecton-0.9.4/tecton_proto/data/materialization_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/odfv_compute_pb2.py` & `tecton-0.9.4/tecton_proto/data/odfv_compute_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/onboarding_pb2.py` & `tecton-0.9.4/tecton_proto/data/onboarding_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/principal_group_pb2.py` & `tecton-0.9.4/tecton_proto/data/principal_group_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/remote_compute_environment_pb2.py` & `tecton-0.9.4/tecton_proto/data/remote_compute_environment_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/remote_spark_pb2.py` & `tecton-0.9.4/tecton_proto/data/remote_spark_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/saved_feature_data_frame_pb2.py` & `tecton-0.9.4/tecton_proto/data/saved_feature_data_frame_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/serving_status_pb2.py` & `tecton-0.9.4/tecton_proto/data/serving_status_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/state_update_pb2.py` & `tecton-0.9.4/tecton_proto/data/state_update_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/stream_data_source_pb2.py` & `tecton-0.9.4/tecton_proto/data/stream_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/summary_pb2.py` & `tecton-0.9.4/tecton_proto/data/summary_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/tecton_api_key_pb2.py` & `tecton-0.9.4/tecton_proto/data/tecton_api_key_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/transformation_pb2.py` & `tecton-0.9.4/tecton_proto/data/transformation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/user_deployment_settings_pb2.py` & `tecton-0.9.4/tecton_proto/data/user_deployment_settings_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/user_pb2.py` & `tecton-0.9.4/tecton_proto/data/user_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/virtual_data_source_pb2.py` & `tecton-0.9.4/tecton_proto/data/virtual_data_source_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/data/workspace_pb2.py` & `tecton-0.9.4/tecton_proto/data/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/clusters_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/dbfs_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/dbfs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/error_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/execution_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/execution_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/instance_profiles_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/instance_profiles_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/jobs_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/libraries_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/permissions_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/permissions_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/scim_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/scim_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/secrets_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/secrets_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/databricks_api/workspace_pb2.py` & `tecton-0.9.4/tecton_proto/databricks_api/workspace_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/config_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/expectation_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/expectation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/metric_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/metric_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/validation_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/validation_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/validation_task_params_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/validation_task_params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/dataobs/validation_task_pb2.py` & `tecton-0.9.4/tecton_proto/dataobs/validation_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py` & `tecton-0.9.4/tecton_proto/feature_server/configuration/feature_server_configuration_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materialization/job_metadata_pb2.py` & `tecton-0.9.4/tecton_proto/materialization/job_metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materialization/materialization_states_pb2.py` & `tecton-0.9.4/tecton_proto/materialization/materialization_states_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materialization/materialization_task_pb2.py` & `tecton-0.9.4/tecton_proto/materialization/materialization_task_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materialization/params_pb2.py` & `tecton-0.9.4/tecton_proto/materialization/params_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materialization/spark_cluster_pb2.py` & `tecton-0.9.4/tecton_proto/materialization/spark_cluster_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/materializationjobservice/materialization_job_service_pb2.py` & `tecton-0.9.4/tecton_proto/materializationjobservice/materialization_job_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/metadataservice/http_over_grpc_pb2.py` & `tecton-0.9.4/tecton_proto/metadataservice/http_over_grpc_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/metadataservice/metadata_service_pb2.py` & `tecton-0.9.4/tecton_proto/metadataservice/metadata_service_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 from tecton_proto.dataobs import metric_pb2 as tecton__proto_dot_dataobs_dot_metric__pb2
 from tecton_proto.dataobs import validation_pb2 as tecton__proto_dot_dataobs_dot_validation__pb2
 from tecton_proto.materialization import job_metadata_pb2 as tecton__proto_dot_materialization_dot_job__metadata__pb2
 from tecton_proto.materialization import spark_cluster_pb2 as tecton__proto_dot_materialization_dot_spark__cluster__pb2
 from tecton_proto.validation import validator_pb2 as tecton__proto_dot_validation_dot_validator__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a$tecton_proto/args/feature_view.proto\x1a$tecton_proto/auditlog/metadata.proto\x1a!tecton_proto/auth/principal.proto\x1a\x1ftecton_proto/auth/service.proto\x1a)tecton_proto/common/aws_credentials.proto\x1a%tecton_proto/common/fco_locator.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/common/spark_schema.proto\x1a\x1etecton_proto/data/entity.proto\x1a\x1btecton_proto/data/fco.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a.tecton_proto/data/materialization_status.proto\x1a\"tecton_proto/data/onboarding.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a&tecton_proto/data/serving_status.proto\x1a$tecton_proto/data/state_update.proto\x1a\x1ftecton_proto/data/summary.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\x1a\x1ctecton_proto/data/user.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a/tecton_proto/materialization/job_metadata.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\x1a\'tecton_proto/validation/validator.proto\"\x90\x01\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x1e\n\ncomparison\x18\x03 \x01(\x03R\ncomparison\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\xbd\x01\n\x15ValidationResultToken\x12\x43\n\x0fvalidation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12\x34\n\tresult_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08resultId\x12)\n\x10\x65xpectation_name\x18\x03 \x01(\tR\x0f\x65xpectationName\"\xd3\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"\xaf\x01\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x0finclude_deleted\x18\x02 \x01(\x08R\x0eincludeDeleted\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\xac\x07\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12I\n\x08statuses\x18\x03 \x03(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\x08statuses\x12`\n\x16last_task_state_change\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x13lastTaskStateChange\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n$include_update_materialization_flags\x18\x0c \x01(\x08R!includeUpdateMaterializationFlags\x12#\n\rwrites_online\x18\r \x01(\x08R\x0cwritesOnline\x12%\n\x0ewrites_offline\x18\x0e \x01(\x08R\rwritesOffline\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"j\n\x14GetJobDetailsRequest\x12R\n\x19tecton_managed_attempt_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x16tectonManagedAttemptId\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xb5\x05\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12K\n\ttaskState\x18\x02 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12-\n\x12manually_triggered\x18\t \x01(\x08R\x11manuallyTriggered\x12O\n\x16last_task_state_change\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13lastTaskStateChange\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\x83\x05\n\x12TaskAttemptDetails\x12\x30\n\x07task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x02 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12L\n\ntask_state\x18\x03 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12V\n\x0e\x61ttempt_status\x18\x04 \x01(\x0b\x32/.tecton_proto.data.MaterializationAttemptStatusR\rattemptStatus\x12P\n\x0brun_details\x18\x05 \x01(\x0b\x32/.tecton_proto.materialization.TectonManagedInfoR\nrunDetails\x12K\n\x0e\x63luster_config\x18\x06 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigR\rclusterConfig\x12H\n\x12\x66\x65\x61ture_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\x12!\n\x0c\x61nyscale_url\x18\t \x01(\tR\x0b\x61nyscaleUrl\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xb4\x01\n\x15GetJobDetailsResponse\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12Y\n\x0f\x61ttempt_details\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.TaskAttemptDetailsR\x0e\x61ttemptDetails\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"t\n!RestartMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\"\xa1\x01\n\"RestartMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\x12V\n\x1bnew_materialization_task_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x18newMaterializationTaskId\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"F\n\x12SparkClusterConfig\x12\x1a\n\x08original\x18\x01 \x01(\tR\x08original\x12\x14\n\x05\x66inal\x18\x02 \x01(\tR\x05\x66inal\"\xc4\x01\n\x16GetSparkConfigResponse\x12S\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0b\x62\x61tchConfig\x12U\n\rstream_config\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\xca\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xf3\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x04 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\xd0\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xe8\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"\xa2\x01\n\tModelInfo\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12(\n\x10model_public_uri\x18\x03 \x01(\tR\x0emodelPublicUri\x12.\n\x13metadata_public_uri\x18\x04 \x01(\tR\x11metadataPublicUri\"+\n\x11ListModelsRequest\x12\x16\n\x06\x66ilter\x18\x01 \x01(\tR\x06\x66ilter\"U\n\x12ListModelsResponse\x12?\n\x06models\x18\x01 \x03(\x0b\x32\'.tecton_proto.metadataservice.ModelInfoR\x06models\")\n\x13GetModelInfoRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\"^\n\x14GetModelInfoResponse\x12\x46\n\nmodel_info\x18\x01 \x01(\x0b\x32\'.tecton_proto.metadataservice.ModelInfoR\tmodelInfo\"Z\n\x17\x46indFcoWorkspaceRequest\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xaa\x02\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\x12+\n\x11suppress_warnings\x18\x06 \x01(\x08R\x10suppressWarnings\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xd6\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\x12+\n\x11suppress_warnings\x18\x06 \x01(\x08R\x10suppressWarnings\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\xa5\x01\n\x16\x43reateWorkspaceRequest\x12.\n\x0eworkspace_name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\rworkspaceName\x12U\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"?\n\x16\x44\x65leteWorkspaceRequest\x12%\n\tworkspace\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"d\n\x13\x43reateApiKeyRequest\x12)\n\x0b\x64\x65scription\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12\"\n\x08is_admin\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07isAdmin\"Z\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"G\n\x13\x44\x65leteApiKeyRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\xf6\x01\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12@\n\ncreated_by\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\tcreatedBy\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAtJ\x04\x08\x05\x10\x06\"e\n\x1b\x43reateServiceAccountRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\"\xf9\x01\n\x1c\x43reateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\xa4\x01\n\x1bUpdateServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\"\xe0\x01\n\x1cUpdateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"6\n\x1b\x44\x65leteServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\"D\n\x18\x43reateClusterUserRequest\x12(\n\x0blogin_email\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\nloginEmail\"!\n\x19\x43reateClusterUserResponseJ\x04\x08\x01\x10\x02\"<\n\x18\x44\x65leteClusterUserRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\"!\n\x19\x44\x65leteClusterUserResponseJ\x04\x08\x01\x10\x02\"\x8f\x02\n\x18\x43lusterUserActionRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\x12\x41\n\x17resend_activation_email\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x15resendActivationEmail\x12*\n\x0bunlock_user\x18\x03 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\nunlockUser\x12*\n\x0bgrant_admin\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\ngrantAdmin\x12,\n\x0crevoke_admin\x18\x05 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"!\n\x19\x43lusterUserActionResponseJ\x04\x08\x01\x10\x02\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xbf\x02\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x33\n\x15online_join_keys_path\x18\x02 \x01(\tH\x00R\x12onlineJoinKeysPath\x12<\n\x1aonline_join_keys_full_path\x18\x06 \x01(\tH\x00R\x16onlineJoinKeysFullPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offlineB\n\n\x08location\"1\n\x16\x44\x65leteEntitiesResponse\x12\x17\n\x07job_ids\x18\x01 \x03(\tR\x06jobIds\"\xfd\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"\\\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02*\x12\x41\x43TION_LIST_TABLES*\x17\x41\x43TION_GET_TABLE_SCHEMA\"\xe1\x01\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06resultJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\xc9\x01\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboardingJ\x04\x08\x01\x10\x02\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\xaf\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\x12\x1a\n\x05limit\x18\x06 \x01(\x05:\x04\x35\x30\x30\x30R\x05limit\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x80\x04\n!GetFeatureValidationResultRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12\x39\n\x19\x66ilter_feature_view_names\x18\x04 \x03(\tR\x16\x66ilterFeatureViewNames\x12\x38\n\x18\x66ilter_expectation_names\x18\x05 \x03(\tR\x16\x66ilterExpectationNames\x12[\n\x13\x66ilter_result_types\x18\x06 \x03(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x11\x66ilterResultTypes\x12O\n\npagination\x18\x07 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xb9\x01\n\"GetFeatureValidationResultResponse\x12\x41\n\x07results\x18\x02 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\x12P\n\npagination\x18\x03 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\xa1\x01\n\x1e\x46\x65\x61tureServerAutoScalingConfig\x12!\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07\x65nabled\x12-\n\x0emin_node_count\x18\x02 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0cminNodeCount\x12-\n\x0emax_node_count\x18\x03 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0cmaxNodeCount\"\x1f\n\x1dGetFeatureServerConfigRequest\"\xa0\x02\n\x1eGetFeatureServerConfigResponse\x12+\n\x0c\x63urrentCount\x18\x01 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63urrentCount\x12/\n\x0e\x61vailableCount\x18\x02 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0e\x61vailableCount\x12+\n\x0c\x64\x65siredCount\x18\x03 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x64\x65siredCount\x12s\n\x11\x61utoScalingConfig\x18\x04 \x01(\x0b\x32<.tecton_proto.metadataservice.FeatureServerAutoScalingConfigB\x07\xea\x99\xbd\x46\x02\x08\x02R\x11\x61utoScalingConfig\"\xb3\x01\n\x1dSetFeatureServerConfigRequest\x12\x1d\n\x05\x63ount\x18\x01 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x05\x63ount\x12s\n\x11\x61utoScalingConfig\x18\x02 \x01(\x0b\x32<.tecton_proto.metadataservice.FeatureServerAutoScalingConfigB\x07\xea\x99\xbd\x46\x02\x08\x02R\x11\x61utoScalingConfig\"d\n!GetOfflineStoreCredentialsRequest\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\"[\n\"GetOfflineStoreCredentialsResponse\x12\x35\n\x03\x61ws\x18\x01 \x01(\x0b\x32#.tecton_proto.common.AwsCredentialsR\x03\x61ws*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\xee\x96\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xad\x01\n\rGetJobDetails\x12\x32.tecton_proto.metadataservice.GetJobDetailsRequest\x1a\x33.tecton_proto.metadataservice.GetJobDetailsResponse\"3\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/job-details:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe5\x01\n\x1aRestartMaterializationTask\x12?.tecton_proto.metadataservice.RestartMaterializationTaskRequest\x1a@.tecton_proto.metadataservice.RestartMaterializationTaskResponse\"D\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/restart-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xd6\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\"S\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x1b*\x19tecton/platform#read_only\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf7\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"n\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/query-state-update-response:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xce\x01\xa2\xbc\xe6\xc0\x05&*$tecton/organization#create_workspace\xa2\xbc\xe6\xc0\x05P2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x63reate_workspace\x1a\x01\x31\x12\xb5\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"T\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x64\x65lete_workspace\x1a\x01\x31\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xbd\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x9a\x02\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x63reate_service_account\x1a\x01\x31\x12\xc4\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\";\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xa5\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16update_service_account\x1a\x01\x31\x12\xa5\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x64\x65lete_service_account\x1a\x01\x31\x12\x8e\x02\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"\x96\x01\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xa2\xbc\xe6\xc0\x05\x44\x32\x42\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x63reate_api_key\x1a\x01\x31\x12\xb2\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"W\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x64\x65lete_api_key\x1a\x01\x31\x12|\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xff\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x63reate_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x64\x65lete_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x61\x63\x63ount_user_action\x1a\x01\x31\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\x91\x02\n\x1aGetFeatureValidationResult\x12?.tecton_proto.metadataservice.GetFeatureValidationResultRequest\x1a@.tecton_proto.metadataservice.GetFeatureValidationResultResponse\"p\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-feature-validation-result:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa4\x02\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"\x8e\x01\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\xf2\x99\xbd\x46 \x08\x01\x12\x19set_feature_server_config\x1a\x01\x31\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_user\x12\xe6\x01\n\x1aGetOfflineStoreCredentials\x12?.tecton_proto.metadataservice.GetOfflineStoreCredentialsRequest\x1a@.tecton_proto.metadataservice.GetOfflineStoreCredentialsResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-offline-store-credentials:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc9\x01\n\nListModels\x12/.tecton_proto.metadataservice.ListModelsRequest\x1a\x30.tecton_proto.metadataservice.ListModelsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/list-models:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xd2\x01\n\x0cGetModelInfo\x12\x31.tecton_proto.metadataservice.GetModelInfoRequest\x1a\x32.tecton_proto.metadataservice.GetModelInfoResponse\"[\x82\xd3\xe4\x93\x02(\"#/v1/metadata-service/get-model-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organizationBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n3tecton_proto/metadataservice/metadata_service.proto\x12\x1ctecton_proto.metadataservice\x1a\x1cgoogle/api/annotations.proto\x1a\x1egoogle/protobuf/duration.proto\x1a\x1bgoogle/protobuf/empty.proto\x1a google/protobuf/field_mask.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a&tecton_proto/amplitude/amplitude.proto\x1a+tecton_proto/amplitude/client_logging.proto\x1a$tecton_proto/args/feature_view.proto\x1a$tecton_proto/auditlog/metadata.proto\x1a!tecton_proto/auth/principal.proto\x1a\x1ftecton_proto/auth/service.proto\x1a)tecton_proto/common/aws_credentials.proto\x1a%tecton_proto/common/fco_locator.proto\x1a\x1ctecton_proto/common/id.proto\x1a&tecton_proto/common/spark_schema.proto\x1a\x1etecton_proto/data/entity.proto\x1a\x1btecton_proto/data/fco.proto\x1a\'tecton_proto/data/feature_service.proto\x1a$tecton_proto/data/feature_view.proto\x1a(tecton_proto/data/freshness_status.proto\x1a&tecton_proto/data/hive_metastore.proto\x1a\x35tecton_proto/data/internal_spark_cluster_status.proto\x1a.tecton_proto/data/materialization_status.proto\x1a\"tecton_proto/data/onboarding.proto\x1a\x30tecton_proto/data/saved_feature_data_frame.proto\x1a&tecton_proto/data/serving_status.proto\x1a$tecton_proto/data/state_update.proto\x1a\x1ftecton_proto/data/summary.proto\x1a&tecton_proto/data/tecton_api_key.proto\x1a&tecton_proto/data/transformation.proto\x1a\x1ctecton_proto/data/user.proto\x1a\x30tecton_proto/data/user_deployment_settings.proto\x1a+tecton_proto/data/virtual_data_source.proto\x1a!tecton_proto/data/workspace.proto\x1a&tecton_proto/dataobs/expectation.proto\x1a!tecton_proto/dataobs/metric.proto\x1a%tecton_proto/dataobs/validation.proto\x1a/tecton_proto/materialization/job_metadata.proto\x1a\x30tecton_proto/materialization/spark_cluster.proto\x1a\'tecton_proto/validation/validator.proto\"\x90\x01\n\nJobsKeySet\x12\x39\n\nupdated_at\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tupdatedAt\x12\x1e\n\ncomparison\x18\x03 \x01(\x03R\ncomparison\x12\'\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\"\xd0\x01\n\x11PaginationRequest\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x19\n\x08sort_key\x18\x03 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x04 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\x12\x1d\n\npage_token\x18\x05 \x01(\tR\tpageToken\"\xf0\x01\n\x12PaginationResponse\x12\x12\n\x04page\x18\x01 \x01(\rR\x04page\x12\x19\n\x08per_page\x18\x02 \x01(\rR\x07perPage\x12\x14\n\x05total\x18\x03 \x01(\rR\x05total\x12&\n\x0fnext_page_token\x18\x04 \x01(\tR\rnextPageToken\x12\x19\n\x08sort_key\x18\x05 \x01(\tR\x07sortKey\x12R\n\x0esort_direction\x18\x06 \x01(\x0e\x32+.tecton_proto.metadataservice.SortDirectionR\rsortDirection\"\xbd\x01\n\x15ValidationResultToken\x12\x43\n\x0fvalidation_time\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0evalidationTime\x12\x34\n\tresult_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x08resultId\x12)\n\x10\x65xpectation_name\x18\x03 \x01(\tR\x0f\x65xpectationName\"\xd3\x01\n\x18GetFeatureServiceRequest\x12+\n\x11service_reference\x18\x02 \x01(\tR\x10serviceReference\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x01\x10\x02J\x04\x08\x05\x10\x06\"a\n\x19GetFeatureServiceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"<\n\x1cGetAllFeatureServicesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"m\n\x1dGetAllFeatureServicesResponse\x12L\n\x10\x66\x65\x61ture_services\x18\x01 \x03(\x0b\x32!.tecton_proto.data.FeatureServiceR\x0f\x66\x65\x61tureServices\"\xc7\x01\n\x1fGetFeatureServiceSummaryRequest\x12G\n\x12\x66\x65\x61ture_service_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x32\n\x14\x66\x65\x61ture_service_name\x18\x02 \x01(\tH\x00R\x12\x66\x65\x61tureServiceName\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\t\n\x07locator\"\x8c\x01\n GetFeatureServiceSummaryResponse\x12\x43\n\rgeneral_items\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.SummaryItemR\x0cgeneralItems\x12#\n\rvariant_names\x18\x03 \x03(\tR\x0cvariantNames\"f\n\"GetVirtualDataSourceSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"e\n#GetVirtualDataSourceSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"c\n\x1fGetTransformationSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"b\n GetTransformationSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"[\n\x17GetEntitySummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"Z\n\x18GetEntitySummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"\xd9\x01\n\x17GetServingStatusRequest\x12G\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0e\n\x0crequest_type\"\xd6\x01\n\x1eGetFVServingStatusForFSRequest\x12\x45\n\x12\x66\x65\x61ture_service_id\x18\x02 \x02(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61tureServiceId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12O\n\npagination\x18\x04 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xe7\x01\n\x1fGetFVServingStatusForFSResponse\x12r\n\x1b\x66ull_serving_status_summary\x18\x01 \x01(\x0b\x32\x33.tecton_proto.data.FullFeatureServiceServingSummaryR\x18\x66ullServingStatusSummary\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"y\n\x18GetServingStatusResponse\x12]\n\x16serving_status_summary\x18\x05 \x01(\x0b\x32\'.tecton_proto.data.ServingStatusSummaryR\x14servingStatusSummary\"=\n\x1dGetAllFeatureFreshnessRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"s\n\x1eGetAllFeatureFreshnessResponse\x12Q\n\x12\x66reshness_statuses\x18\x01 \x03(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x11\x66reshnessStatuses\"^\n\x1aGetFeatureFreshnessRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"l\n\x1bGetFeatureFreshnessResponse\x12M\n\x10\x66reshness_status\x18\x01 \x01(\x0b\x32\".tecton_proto.data.FreshnessStatusR\x0f\x66reshnessStatus\"\xaf\x01\n\x1fGetMaterializationStatusRequest\x12\x45\n\x12\x66\x65\x61ture_package_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x10\x66\x65\x61turePackageId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x0finclude_deleted\x18\x02 \x01(\x08R\x0eincludeDeleted\"\x83\x01\n GetMaterializationStatusResponse\x12_\n\x16materialization_status\x18\x01 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"V\n2GetAllMaterializationStatusInLiveWorkspacesRequest\x12 \n\x0c\x63ut_off_days\x18\x01 \x01(\x05R\ncutOffDays\"4\n\nCountRange\x12\x14\n\x05start\x18\x01 \x01(\rR\x05start\x12\x10\n\x03\x65nd\x18\x02 \x01(\rR\x03\x65nd\"m\n\rDurationRange\x12/\n\x05start\x18\x01 \x01(\x0b\x32\x19.google.protobuf.DurationR\x05start\x12+\n\x03\x65nd\x18\x02 \x01(\x0b\x32\x19.google.protobuf.DurationR\x03\x65nd\"o\n\rDateTimeRange\x12\x30\n\x05start\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x05start\x12,\n\x03\x65nd\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x03\x65nd\"\xac\x07\n\x0eGetJobsRequest\x12\x1e\n\nworkspaces\x18\x01 \x03(\tR\nworkspaces\x12#\n\rfeature_views\x18\x02 \x03(\tR\x0c\x66\x65\x61tureViews\x12I\n\x08statuses\x18\x03 \x03(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\x08statuses\x12`\n\x16last_task_state_change\x18\x06 \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x13lastTaskStateChange\x12\x43\n\ttask_type\x18\x04 \x03(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12K\n\x0cnum_attempts\x18\x05 \x01(\x0b\x32(.tecton_proto.metadataservice.CountRangeR\x0bnumAttempts\x12-\n\x12manually_triggered\x18\x07 \x01(\x08R\x11manuallyTriggered\x12G\n\x08\x64uration\x18\x08 \x01(\x0b\x32+.tecton_proto.metadataservice.DurationRangeR\x08\x64uration\x12Y\n\x12\x66\x65\x61ture_start_time\x18\n \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x10\x66\x65\x61tureStartTime\x12U\n\x10\x66\x65\x61ture_end_time\x18\x0b \x01(\x0b\x32+.tecton_proto.metadataservice.DateTimeRangeR\x0e\x66\x65\x61tureEndTime\x12O\n$include_update_materialization_flags\x18\x0c \x01(\x08R!includeUpdateMaterializationFlags\x12#\n\rwrites_online\x18\r \x01(\x08R\x0cwritesOnline\x12%\n\x0ewrites_offline\x18\x0e \x01(\x08R\rwritesOffline\x12O\n\npagination\x18\t \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"j\n\x14GetJobDetailsRequest\x12R\n\x19tecton_managed_attempt_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x16tectonManagedAttemptId\"\xc5\x01\n FeatureViewMaterializationStatus\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\"\xb5\x05\n\x10TaskWithAttempts\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12K\n\ttaskState\x18\x02 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12_\n\x16materialization_status\x18\x03 \x01(\x0b\x32(.tecton_proto.data.MaterializationStatusR\x15materializationStatus\x12\x30\n\x07task_id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x08 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12-\n\x12manually_triggered\x18\t \x01(\x08R\x11manuallyTriggered\x12O\n\x16last_task_state_change\x18\n \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13lastTaskStateChange\x12*\n\x11\x66\x65\x61ture_view_name\x18\x05 \x01(\tR\x0f\x66\x65\x61tureViewName\x12H\n\x12\x66\x65\x61ture_start_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\"\x83\x05\n\x12TaskAttemptDetails\x12\x30\n\x07task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06taskId\x12\x43\n\ttask_type\x18\x02 \x01(\x0e\x32&.tecton_proto.materialization.TaskTypeR\x08taskType\x12L\n\ntask_state\x18\x03 \x01(\x0e\x32-.tecton_proto.data.MaterializationStatusStateR\ttaskState\x12V\n\x0e\x61ttempt_status\x18\x04 \x01(\x0b\x32/.tecton_proto.data.MaterializationAttemptStatusR\rattemptStatus\x12P\n\x0brun_details\x18\x05 \x01(\x0b\x32/.tecton_proto.materialization.TectonManagedInfoR\nrunDetails\x12K\n\x0e\x63luster_config\x18\x06 \x01(\x0b\x32$.tecton_proto.args.RiftClusterConfigR\rclusterConfig\x12H\n\x12\x66\x65\x61ture_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x66\x65\x61tureStartTime\x12\x44\n\x10\x66\x65\x61ture_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x66\x65\x61tureEndTime\x12!\n\x0c\x61nyscale_url\x18\t \x01(\tR\x0b\x61nyscaleUrl\"\xc5\x01\n3GetAllMaterializationStatusInLiveWorkspacesResponse\x12\x8d\x01\n#feature_view_materialization_status\x18\x01 \x03(\x0b\x32>.tecton_proto.metadataservice.FeatureViewMaterializationStatusR featureViewMaterializationStatus\"\xc1\x01\n\x0fGetJobsResponse\x12\\\n\x11tasksWithAttempts\x18\x01 \x03(\x0b\x32..tecton_proto.metadataservice.TaskWithAttemptsR\x11tasksWithAttempts\x12P\n\npagination\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xb4\x01\n\x15GetJobDetailsResponse\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12Y\n\x0f\x61ttempt_details\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.TaskAttemptDetailsR\x0e\x61ttemptDetails\"\xa0\x01\n$ForceRetryMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\x12\'\n\x0f\x61llow_overwrite\x18\x02 \x01(\x08R\x0e\x61llowOverwrite\"L\n%ForceRetryMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\"t\n!RestartMaterializationTaskRequest\x12O\n\x17materialization_task_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x15materializationTaskId\"\xa1\x01\n\"RestartMaterializationTaskResponse\x12#\n\rerror_message\x18\x01 \x01(\tR\x0c\x65rrorMessage\x12V\n\x1bnew_materialization_task_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x18newMaterializationTaskId\".\n\x0eGetFcosRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"W\n\x0fGetFcosResponse\x12\x44\n\rfco_container\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"a\n\x15GetSparkConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"F\n\x12SparkClusterConfig\x12\x1a\n\x08original\x18\x01 \x01(\tR\x08original\x12\x14\n\x05\x66inal\x18\x02 \x01(\tR\x05\x66inal\"\xc4\x01\n\x16GetSparkConfigResponse\x12S\n\x0c\x62\x61tch_config\x18\x01 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0b\x62\x61tchConfig\x12U\n\rstream_config\x18\x02 \x01(\x0b\x32\x30.tecton_proto.metadataservice.SparkClusterConfigR\x0cstreamConfig\"t\n(GetMetricAndExpectationDefinitionRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xe4\x02\n)GetMetricAndExpectationDefinitionResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x36\n\x07metrics\x18\x03 \x03(\x0b\x32\x1c.tecton_proto.dataobs.MetricR\x07metrics\x12[\n\x14\x66\x65\x61ture_expectations\x18\x04 \x03(\x0b\x32(.tecton_proto.dataobs.FeatureExpectationR\x13\x66\x65\x61tureExpectations\x12X\n\x13metric_expectations\x18\x05 \x03(\x0b\x32\'.tecton_proto.dataobs.MetricExpectationR\x12metricExpectations\"\xca\x01\n\x15GetFeatureViewRequest\x12+\n\x11version_specifier\x18\x01 \x01(\tR\x10versionSpecifier\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\'\n\x02id\x18\x04 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckJ\x04\x08\x05\x10\x06\"^\n\x16GetFeatureViewResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"`\n\x1cGetFeatureViewSummaryRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\"_\n\x1dGetFeatureViewSummaryResponse\x12>\n\x0b\x66\x63o_summary\x18\x01 \x01(\x0b\x32\x1d.tecton_proto.data.FcoSummaryR\nfcoSummary\"R\n\x18QueryFeatureViewsRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceJ\x04\x08\x05\x10\x06\"a\n\x19QueryFeatureViewsResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"{\n4GetMaterializingFeatureViewsInLiveWorkspacesResponse\x12\x43\n\rfeature_views\x18\x01 \x03(\x0b\x32\x1e.tecton_proto.data.FeatureViewR\x0c\x66\x65\x61tureViews\"\xf3\x01\n\x1bGetVirtualDataSourceRequest\x12N\n\x16virtual_data_source_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x13virtualDataSourceId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x04 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"d\n\x1cGetVirtualDataSourceResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"?\n\x1fGetAllVirtualDataSourcesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n GetAllVirtualDataSourcesResponse\x12V\n\x14virtual_data_sources\x18\x01 \x03(\x0b\x32$.tecton_proto.data.VirtualDataSourceR\x12virtualDataSources\"\xd0\x01\n\x10GetEntityRequest\x12\x36\n\tentity_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x08\x65ntityId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"Y\n\x11GetEntityResponse\x12\x44\n\rfco_container\x18\x02 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainer\"5\n\x15GetAllEntitiesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"O\n\x16GetAllEntitiesResponse\x12\x35\n\x08\x65ntities\x18\x01 \x03(\x0b\x32\x19.tecton_proto.data.EntityR\x08\x65ntities\"\xe8\x01\n\x18GetTransformationRequest\x12\x46\n\x11transformation_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10transformationId\x12\x14\n\x04name\x18\x02 \x01(\tH\x00R\x04name\x12\x1c\n\tworkspace\x18\x04 \x01(\tR\tworkspace\x12\x37\n\x18run_object_version_check\x18\x06 \x01(\x08R\x15runObjectVersionCheckB\x11\n\x0fidentifier_typeJ\x04\x08\x05\x10\x06\"g\n\x19GetTransformationResponse\x12\x44\n\rfco_container\x18\x03 \x01(\x0b\x32\x1f.tecton_proto.data.FcoContainerR\x0c\x66\x63oContainerJ\x04\x08\x01\x10\x02\"<\n\x1cGetAllTransformationsRequest\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"r\n\x1dGetAllTransformationsResponse\x12K\n\x0ftransformations\x18\x02 \x03(\x0b\x32!.tecton_proto.data.TransformationR\x0ftransformationsJ\x04\x08\x01\x10\x02\"\xa2\x01\n\tModelInfo\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12(\n\x10model_public_uri\x18\x03 \x01(\tR\x0emodelPublicUri\x12.\n\x13metadata_public_uri\x18\x04 \x01(\tR\x11metadataPublicUri\"+\n\x11ListModelsRequest\x12\x16\n\x06\x66ilter\x18\x01 \x01(\tR\x06\x66ilter\"U\n\x12ListModelsResponse\x12?\n\x06models\x18\x01 \x03(\x0b\x32\'.tecton_proto.metadataservice.ModelInfoR\x06models\")\n\x13GetModelInfoRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\"^\n\x14GetModelInfoResponse\x12\x46\n\nmodel_info\x18\x01 \x01(\x0b\x32\'.tecton_proto.metadataservice.ModelInfoR\tmodelInfo\"Z\n\x17\x46indFcoWorkspaceRequest\x12?\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\rfeatureViewId\"8\n\x18\x46indFcoWorkspaceResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"z\n\x17IngestClientLogsRequest\x12_\n\x15sdk_method_invocation\x18\x01 \x01(\x0b\x32+.tecton_proto.amplitude.SDKMethodInvocationR\x13sdkMethodInvocation\"v\n\x16IngestAnalyticsRequest\x12>\n\x06\x65vents\x18\x01 \x03(\x0b\x32&.tecton_proto.amplitude.AmplitudeEventR\x06\x65vents\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xbf\x01\n\x15NewStateUpdateRequest\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\"\xaa\x02\n\x17NewStateUpdateRequestV2\x12?\n\x07request\x18\x01 \x01(\x0b\x32%.tecton_proto.data.StateUpdateRequestR\x07request\x12\x31\n\x15\x62locking_dry_run_mode\x18\x02 \x01(\x08R\x12\x62lockingDryRunMode\x12\x32\n\x15\x65nable_eager_response\x18\x03 \x01(\x08R\x13\x65nableEagerResponse\x12\x19\n\x08no_color\x18\x04 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x05 \x01(\x08R\njsonOutput\x12+\n\x11suppress_warnings\x18\x06 \x01(\x08R\x10suppressWarnings\"\xe7\x01\n\x16NewStateUpdateResponse\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12]\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x36.tecton_proto.metadataservice.QueryStateUpdateResponseR\reagerResponse\"\xeb\x01\n\x18NewStateUpdateResponseV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12:\n\x1asigned_url_for_repo_upload\x18\x02 \x01(\tR\x16signedUrlForRepoUpload\x12_\n\x0e\x65\x61ger_response\x18\x03 \x01(\x0b\x32\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2R\reagerResponse\"k\n\x17QueryStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\xd6\x01\n\x19QueryStateUpdateRequestV2\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\x12\x19\n\x08no_color\x18\x03 \x01(\x08R\x07noColor\x12\x1f\n\x0bjson_output\x18\x04 \x01(\x08R\njsonOutput\x12+\n\x11suppress_warnings\x18\x06 \x01(\x08R\x10suppressWarnings\"\xd4\x02\n\x18QueryStateUpdateResponse\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x31\n\x14recreates_suppressed\x18\x07 \x01(\x08R\x13recreatesSuppressed\x12P\n\x11validation_result\x18\x04 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x39\n\ndiff_items\x18\x05 \x03(\x0b\x32\x1a.tecton_proto.data.FcoDiffR\tdiffItems\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\"\xe9\x02\n\x1aQueryStateUpdateResponseV2\x12\x14\n\x05ready\x18\x01 \x01(\x08R\x05ready\x12\x18\n\x07success\x18\x02 \x01(\x08R\x07success\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\x12\x32\n\x15latest_status_message\x18\x06 \x01(\tR\x13latestStatusMessage\x12R\n\x11validation_errors\x18\x08 \x01(\x0b\x32#.tecton_proto.data.ValidationResultH\x00R\x10validationErrors\x12_\n\x16successful_plan_output\x18\t \x01(\x0b\x32\'.tecton_proto.data.SuccessfulPlanOutputH\x00R\x14successfulPlanOutputB\n\n\x08responseJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06J\x04\x08\x07\x10\x08\"T\n GetStateUpdatePlanSummaryRequest\x12\x30\n\x07plan_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x06planId\"b\n!GetStateUpdatePlanSummaryResponse\x12=\n\x04plan\x18\x01 \x01(\x0b\x32).tecton_proto.data.StateUpdatePlanSummaryR\x04plan\"p\n\x17\x41pplyStateUpdateRequest\x12\x32\n\x08state_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x07stateId\x12!\n\napplied_by\x18\x02 \x01(\tB\x02\x18\x01R\tappliedBy\"\x1a\n\x18\x41pplyStateUpdateResponse\"\xb2\x01\n\x12GetConfigsResponse\x12^\n\nkey_values\x18\x01 \x03(\x0b\x32?.tecton_proto.metadataservice.GetConfigsResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"\xc2\x01\n\x1aGetGlobalsForWebUIResponse\x12\x66\n\nkey_values\x18\x01 \x03(\x0b\x32G.tecton_proto.metadataservice.GetGlobalsForWebUIResponse.KeyValuesEntryR\tkeyValues\x1a<\n\x0eKeyValuesEntry\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x14\n\x05value\x18\x02 \x01(\tR\x05value:\x02\x38\x01\"N\n\x18GetStateUpdateLogRequest\x12\x14\n\x05limit\x18\x01 \x01(\x05R\x05limit\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"Z\n\x19GetStateUpdateLogResponse\x12=\n\x07\x65ntries\x18\x01 \x03(\x0b\x32#.tecton_proto.data.StateUpdateEntryR\x07\x65ntries\"R\n\x15GetRestoreInfoRequest\x12\x1b\n\tcommit_id\x18\x01 \x01(\tR\x08\x63ommitId\x12\x1c\n\tworkspace\x18\x02 \x01(\tR\tworkspace\"\x96\x01\n\x16GetRestoreInfoResponse\x12>\n\x1csigned_url_for_repo_download\x18\x01 \x01(\tR\x18signedUrlForRepoDownload\x12\x1b\n\tcommit_id\x18\x02 \x01(\tR\x08\x63ommitId\x12\x1f\n\x0bsdk_version\x18\x03 \x01(\tR\nsdkVersion\"\xa5\x01\n\x16\x43reateWorkspaceRequest\x12.\n\x0eworkspace_name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\rworkspaceName\x12U\n\x0c\x63\x61pabilities\x18\x03 \x01(\x0b\x32(.tecton_proto.data.WorkspaceCapabilitiesB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63\x61pabilitiesJ\x04\x08\x01\x10\x02\"?\n\x16\x44\x65leteWorkspaceRequest\x12%\n\tworkspace\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\tworkspace\"2\n\x17IntrospectApiKeyRequest\x12\x17\n\x07\x61pi_key\x18\x01 \x01(\tR\x06\x61piKey\"\xcb\x01\n\x18IntrospectApiKeyResponse\x12\'\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x02id\x12 \n\x0b\x64\x65scription\x18\x02 \x01(\tR\x0b\x64\x65scription\x12\x1d\n\ncreated_by\x18\x03 \x01(\tR\tcreatedBy\x12\x16\n\x06\x61\x63tive\x18\x04 \x01(\x08R\x06\x61\x63tive\x12\x19\n\x08is_admin\x18\x05 \x01(\x08R\x07isAdmin\x12\x12\n\x04name\x18\x06 \x01(\tR\x04name\"d\n\x13\x43reateApiKeyRequest\x12)\n\x0b\x64\x65scription\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12\"\n\x08is_admin\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07isAdmin\"Z\n\x14\x43reateApiKeyResponse\x12\x10\n\x03key\x18\x01 \x01(\tR\x03key\x12\x30\n\x02id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"G\n\x13\x44\x65leteApiKeyRequest\x12\x30\n\x02id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"?\n\x12ListApiKeysRequest\x12)\n\x10include_archived\x18\x01 \x01(\x08R\x0fincludeArchived\"Q\n\x13ListApiKeysResponse\x12:\n\x08\x61pi_keys\x18\x01 \x03(\x0b\x32\x1f.tecton_proto.data.TectonApiKeyR\x07\x61piKeys\"\xf6\x01\n\x0eServiceAccount\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x12\n\x04name\x18\x02 \x01(\tR\x04name\x12 \n\x0b\x64\x65scription\x18\x03 \x01(\tR\x0b\x64\x65scription\x12\x1b\n\tis_active\x18\x04 \x01(\x08R\x08isActive\x12@\n\ncreated_by\x18\x06 \x01(\x0b\x32!.tecton_proto.auth.PrincipalBasicR\tcreatedBy\x12\x39\n\ncreated_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAtJ\x04\x08\x05\x10\x06\"e\n\x1b\x43reateServiceAccountRequest\x12\x1b\n\x04name\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\"\xf9\x01\n\x1c\x43reateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x17\n\x07\x61pi_key\x18\x05 \x01(\tR\x06\x61piKey\x12\x39\n\ncreated_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"E\n\x19GetServiceAccountsRequest\x12\x16\n\x06search\x18\x01 \x01(\tR\x06search\x12\x10\n\x03ids\x18\x02 \x03(\tR\x03ids\"u\n\x1aGetServiceAccountsResponse\x12W\n\x10service_accounts\x18\x01 \x03(\x0b\x32,.tecton_proto.metadataservice.ServiceAccountR\x0fserviceAccounts\"\xa4\x01\n\x1bUpdateServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\"\xe0\x01\n\x1cUpdateServiceAccountResponse\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\x12\x1b\n\x04name\x18\x02 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x04name\x12)\n\x0b\x64\x65scription\x18\x03 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0b\x64\x65scription\x12$\n\tis_active\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x08isActive\x12\x39\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tcreatedAt\"6\n\x1b\x44\x65leteServiceAccountRequest\x12\x17\n\x02id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x02id\"\x1e\n\x1c\x44\x65leteServiceAccountResponse\"\x17\n\x15ListWorkspacesRequest\"V\n\x16ListWorkspacesResponse\x12<\n\nworkspaces\x18\x01 \x03(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\nworkspaces\"<\n\x13GetWorkspaceRequest\x12%\n\x0eworkspace_name\x18\x01 \x01(\tR\rworkspaceName\"R\n\x14GetWorkspaceResponse\x12:\n\tworkspace\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.data.WorkspaceR\tworkspace\"\x93\x03\n\"CreateSavedFeatureDataFrameRequest\x12\x12\n\x04name\x18\x01 \x01(\tR\x04name\x12\x1c\n\tworkspace\x18\x07 \x01(\tR\tworkspace\x12G\n\x12\x66\x65\x61ture_package_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61turePackageId\x12G\n\x12\x66\x65\x61ture_service_id\x18\x03 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x10\x66\x65\x61tureServiceId\x12\x31\n\x15join_key_column_names\x18\x04 \x03(\tR\x12joinKeyColumnNames\x12\x32\n\x15timestamp_column_name\x18\x05 \x01(\tR\x13timestampColumnName\x12\x38\n\x06schema\x18\x06 \x01(\x0b\x32 .tecton_proto.common.SparkSchemaR\x06schemaB\x08\n\x06source\"\x87\x01\n#CreateSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"{\n#ArchiveSavedFeatureDataFrameRequest\x12T\n\x1asaved_feature_dataframe_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x17savedFeatureDataframeId\"&\n$ArchiveSavedFeatureDataFrameResponse\"\xe7\x01\n\x1fGetSavedFeatureDataFrameRequest\x12\x41\n\x1csaved_feature_dataframe_name\x18\x01 \x01(\tH\x00R\x19savedFeatureDataframeName\x12V\n\x1asaved_feature_dataframe_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x17savedFeatureDataframeId\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspaceB\x0b\n\treference\"\xa5\x01\n\x1bGetClusterAdminInfoResponse\x12&\n\x0f\x63\x61ller_is_admin\x18\x01 \x01(\x08R\rcallerIsAdmin\x12-\n\x05users\x18\x02 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x05users\x12/\n\x06\x61\x64mins\x18\x03 \x03(\x0b\x32\x17.tecton_proto.data.UserR\x06\x61\x64mins\"D\n\x18\x43reateClusterUserRequest\x12(\n\x0blogin_email\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\nloginEmail\"!\n\x19\x43reateClusterUserResponseJ\x04\x08\x01\x10\x02\"<\n\x18\x44\x65leteClusterUserRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\"!\n\x19\x44\x65leteClusterUserResponseJ\x04\x08\x01\x10\x02\"\x8f\x02\n\x18\x43lusterUserActionRequest\x12 \n\x07okta_id\x18\x01 \x01(\tB\x07\xea\x99\xbd\x46\x02\x08\x02R\x06oktaId\x12\x41\n\x17resend_activation_email\x18\x02 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x15resendActivationEmail\x12*\n\x0bunlock_user\x18\x03 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\nunlockUser\x12*\n\x0bgrant_admin\x18\x04 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\ngrantAdmin\x12,\n\x0crevoke_admin\x18\x05 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02H\x00R\x0brevokeAdminB\x08\n\x06\x61\x63tion\"!\n\x19\x43lusterUserActionResponseJ\x04\x08\x01\x10\x02\"\x84\x01\n GetSavedFeatureDataFrameResponse\x12`\n\x17saved_feature_dataframe\x18\x01 \x01(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x15savedFeatureDataframe\"C\n#GetAllSavedFeatureDataFramesRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\x8a\x01\n$GetAllSavedFeatureDataFramesResponse\x12\x62\n\x18saved_feature_dataframes\x18\x01 \x03(\x0b\x32(.tecton_proto.data.SavedFeatureDataFrameR\x16savedFeatureDataframes\"\x9c\x01\n\x16IngestDataframeRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\x12\x17\n\x07\x64\x66_path\x18\x02 \x01(\tR\x06\x64\x66Path\x12\x1c\n\tworkspace\x18\x03 \x01(\tR\tworkspace\"\x19\n\x17IngestDataframeResponse\"o\n GetNewIngestDataframeInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"t\n!GetNewIngestDataframeInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x36\n\x18signed_url_for_df_upload\x18\x02 \x01(\tR\x14signedUrlForDfUpload\"\x88\x01\n!GetUserDeploymentSettingsResponse\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\"\xc5\x01\n#UpdateUserDeploymentSettingsRequest\x12\x63\n\x18user_deployment_settings\x18\x01 \x01(\x0b\x32).tecton_proto.data.UserDeploymentSettingsR\x16userDeploymentSettings\x12\x39\n\nfield_mask\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.FieldMaskR\tfieldMask\"e\n$UpdateUserDeploymentSettingsResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\"n\n%GetInternalSparkClusterStatusResponse\x12\x45\n\x06status\x18\x01 \x01(\x0b\x32-.tecton_proto.data.InternalSparkClusterStatusR\x06status\"k\n\x1cGetDeleteEntitiesInfoRequest\x12K\n\x15\x66\x65\x61ture_definition_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdR\x13\x66\x65\x61tureDefinitionId\"\xca\x01\n\x1dGetDeleteEntitiesInfoResponse\x12\x17\n\x07\x64\x66_path\x18\x01 \x01(\tR\x06\x64\x66Path\x12\x43\n\x1fsigned_url_for_df_upload_online\x18\x03 \x01(\tR\x1asignedUrlForDfUploadOnline\x12\x45\n signed_url_for_df_upload_offline\x18\x04 \x01(\tR\x1bsignedUrlForDfUploadOfflineJ\x04\x08\x02\x10\x03\"\xbf\x02\n\x15\x44\x65leteEntitiesRequest\x12@\n\x0b\x66\x63o_locator\x18\x01 \x01(\x0b\x32\x1f.tecton_proto.common.FcoLocatorR\nfcoLocator\x12\x33\n\x15online_join_keys_path\x18\x02 \x01(\tH\x00R\x12onlineJoinKeysPath\x12<\n\x1aonline_join_keys_full_path\x18\x06 \x01(\tH\x00R\x16onlineJoinKeysFullPath\x12\x33\n\x16offline_join_keys_path\x18\x03 \x01(\tR\x13offlineJoinKeysPath\x12\x16\n\x06online\x18\x04 \x01(\x08R\x06online\x12\x18\n\x07offline\x18\x05 \x01(\x08R\x07offlineB\n\n\x08location\"1\n\x16\x44\x65leteEntitiesResponse\x12\x17\n\x07job_ids\x18\x01 \x03(\tR\x06jobIds\"\xfd\x01\n\x16GetHiveMetadataRequest\x12S\n\x06\x61\x63tion\x18\x01 \x01(\x0e\x32;.tecton_proto.metadataservice.GetHiveMetadataRequest.ActionR\x06\x61\x63tion\x12\x1a\n\x08\x64\x61tabase\x18\x02 \x01(\tR\x08\x64\x61tabase\x12\x14\n\x05table\x18\x03 \x01(\tR\x05table\"\\\n\x06\x41\x63tion\x12\x19\n\x15\x41\x43TION_LIST_DATABASES\x10\x00\"\x04\x08\x01\x10\x01\"\x04\x08\x02\x10\x02*\x12\x41\x43TION_LIST_TABLES*\x17\x41\x43TION_GET_TABLE_SCHEMA\"\xe1\x01\n\x17GetHiveMetadataResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12#\n\rerror_message\x18\x02 \x01(\tR\x0c\x65rrorMessage\x12\x41\n\tdatabases\x18\x03 \x01(\x0b\x32!.tecton_proto.data.ListHiveResultH\x00R\tdatabases\x12.\n\x13\x64\x65\x62ug_error_message\x18\x06 \x01(\tR\x11\x64\x65\x62ugErrorMessageB\x08\n\x06resultJ\x04\x08\x04\x10\x05J\x04\x08\x05\x10\x06\"\x95\x01\n\x17ValidateLocalFcoRequest\x12Y\n\x12validation_request\x18\x01 \x01(\x0b\x32*.tecton_proto.validation.ValidationRequestR\x11validationRequest\x12\x1f\n\x0bsdk_version\x18\x02 \x01(\tR\nsdkVersion\"\x9c\x01\n\x18ValidateLocalFcoResponse\x12\x18\n\x07success\x18\x01 \x01(\x08R\x07success\x12P\n\x11validation_result\x18\x02 \x01(\x0b\x32#.tecton_proto.data.ValidationResultR\x10validationResult\x12\x14\n\x05\x65rror\x18\x03 \x01(\tR\x05\x65rror\":\n\x1aGetOnboardingStatusRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\"\xc9\x01\n\x1bGetOnboardingStatusResponse\x12N\n\x0esetup_platform\x18\x03 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\rsetupPlatform\x12T\n\x11\x66inish_onboarding\x18\x02 \x01(\x0e\x32\'.tecton_proto.data.OnboardingStatusEnumR\x10\x66inishOnboardingJ\x04\x08\x01\x10\x02\"\x92\x01\n\"GetDataPlatformSetupStatusResponse\x12&\n\x0esetupCompleted\x18\x01 \x01(\x08R\x0esetupCompleted\x12\x44\n\x05tasks\x18\x02 \x03(\x0b\x32..tecton_proto.data.DataPlatformSetupTaskStatusR\x05tasks\"i\n\x1dGetObservabilityConfigRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\"\xa5\x01\n\x1eGetObservabilityConfigResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x39\n\x19is_dataobs_metric_enabled\x18\x03 \x01(\x08R\x16isDataobsMetricEnabled\"\xaf\x02\n\x12QueryMetricRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12\x39\n\nstart_time\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\tstartTime\x12\x35\n\x08\x65nd_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x07\x65ndTime\x12\x1a\n\x05limit\x18\x06 \x01(\x05:\x04\x35\x30\x30\x30R\x05limit\"\xf5\x03\n\x13QueryMetricResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12*\n\x11\x66\x65\x61ture_view_name\x18\x02 \x01(\tR\x0f\x66\x65\x61tureViewName\x12\x41\n\x0bmetric_type\x18\x03 \x01(\x0e\x32 .tecton_proto.dataobs.MetricTypeR\nmetricType\x12V\n\x1ametric_data_point_interval\x18\x05 \x01(\x0b\x32\x19.google.protobuf.DurationR\x17metricDataPointInterval\x12H\n\x12\x61ligned_start_time\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x10\x61lignedStartTime\x12\x44\n\x10\x61ligned_end_time\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x0e\x61lignedEndTime\x12\x46\n\x0bmetric_data\x18\x04 \x03(\x0b\x32%.tecton_proto.dataobs.MetricDataPointR\nmetricData\x12!\n\x0c\x63olumn_names\x18\x06 \x03(\tR\x0b\x63olumnNames\"\x80\x04\n!GetFeatureValidationResultRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12\x39\n\x19\x66ilter_feature_view_names\x18\x04 \x03(\tR\x16\x66ilterFeatureViewNames\x12\x38\n\x18\x66ilter_expectation_names\x18\x05 \x03(\tR\x16\x66ilterExpectationNames\x12[\n\x13\x66ilter_result_types\x18\x06 \x03(\x0e\x32+.tecton_proto.dataobs.ExpectationResultEnumR\x11\x66ilterResultTypes\x12O\n\npagination\x18\x07 \x01(\x0b\x32/.tecton_proto.metadataservice.PaginationRequestR\npagination\"\xb9\x01\n\"GetFeatureValidationResultResponse\x12\x41\n\x07results\x18\x02 \x03(\x0b\x32\'.tecton_proto.dataobs.ExpectationResultR\x07results\x12P\n\npagination\x18\x03 \x01(\x0b\x32\x30.tecton_proto.metadataservice.PaginationResponseR\npagination\"\xde\x01\n\"GetFeatureValidationSummaryRequest\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\"\xba\x02\n#GetFeatureValidationSummaryResponse\x12\x1c\n\tworkspace\x18\x01 \x01(\tR\tworkspace\x12N\n\x15validation_start_time\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x13validationStartTime\x12J\n\x13validation_end_time\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.TimestampR\x11validationEndTime\x12Y\n\x11workspace_summary\x18\x04 \x01(\x0b\x32,.tecton_proto.dataobs.WorkspaceResultSummaryR\x10workspaceSummary\"6\n\x0eGetUserRequest\x12\x0e\n\x02id\x18\x01 \x01(\tR\x02id\x12\x14\n\x05\x65mail\x18\x02 \x01(\tR\x05\x65mail\"C\n\x0fGetUserResponse\x12\x30\n\x04user\x18\x01 \x01(\x0b\x32\x1c.tecton_proto.auth.UserBasicR\x04user\"\xa1\x01\n\x1e\x46\x65\x61tureServerAutoScalingConfig\x12!\n\x07\x65nabled\x18\x01 \x01(\x08\x42\x07\xea\x99\xbd\x46\x02\x08\x02R\x07\x65nabled\x12-\n\x0emin_node_count\x18\x02 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0cminNodeCount\x12-\n\x0emax_node_count\x18\x03 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0cmaxNodeCount\"\x1f\n\x1dGetFeatureServerConfigRequest\"\xa0\x02\n\x1eGetFeatureServerConfigResponse\x12+\n\x0c\x63urrentCount\x18\x01 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x63urrentCount\x12/\n\x0e\x61vailableCount\x18\x02 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0e\x61vailableCount\x12+\n\x0c\x64\x65siredCount\x18\x03 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x0c\x64\x65siredCount\x12s\n\x11\x61utoScalingConfig\x18\x04 \x01(\x0b\x32<.tecton_proto.metadataservice.FeatureServerAutoScalingConfigB\x07\xea\x99\xbd\x46\x02\x08\x02R\x11\x61utoScalingConfig\"\xb3\x01\n\x1dSetFeatureServerConfigRequest\x12\x1d\n\x05\x63ount\x18\x01 \x01(\rB\x07\xea\x99\xbd\x46\x02\x08\x02R\x05\x63ount\x12s\n\x11\x61utoScalingConfig\x18\x02 \x01(\x0b\x32<.tecton_proto.metadataservice.FeatureServerAutoScalingConfigB\x07\xea\x99\xbd\x46\x02\x08\x02R\x11\x61utoScalingConfig\"\xb5\x01\n!GetOfflineStoreCredentialsRequest\x12\x41\n\x0f\x66\x65\x61ture_view_id\x18\x01 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\rfeatureViewId\x12?\n\x0e\x64\x61ta_source_id\x18\x02 \x01(\x0b\x32\x17.tecton_proto.common.IdH\x00R\x0c\x64\x61taSourceIdB\x0c\n\nidentifier\"[\n\"GetOfflineStoreCredentialsResponse\x12\x35\n\x03\x61ws\x18\x01 \x01(\x0b\x32#.tecton_proto.common.AwsCredentialsR\x03\x61ws*>\n\rSortDirection\x12\x10\n\x0cSORT_UNKNOWN\x10\x00\x12\x0c\n\x08SORT_ASC\x10\x01\x12\r\n\tSORT_DESC\x10\x02\x32\xee\x96\x01\n\x0fMetadataService\x12\xec\x01\n\x11GetFeatureService\x12\x36.tecton_proto.metadataservice.GetFeatureServiceRequest\x1a\x37.tecton_proto.metadataservice.GetFeatureServiceResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-feature-service:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfd\x01\n\x15GetAllFeatureServices\x12:.tecton_proto.metadataservice.GetAllFeatureServicesRequest\x1a;.tecton_proto.metadataservice.GetAllFeatureServicesResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-all-feature-services:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x98\x02\n\x18GetFeatureServiceSummary\x12=.tecton_proto.metadataservice.GetFeatureServiceSummaryRequest\x1a>.tecton_proto.metadataservice.GetFeatureServiceSummaryResponse\"}\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/get-feature-service-summary:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\xf7\x01\n\x10GetServingStatus\x12\x35.tecton_proto.metadataservice.GetServingStatusRequest\x1a\x36.tecton_proto.metadataservice.GetServingStatusResponse\"t\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-serving-status:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x96\x02\n\x17GetFVServingStatusForFS\x12<.tecton_proto.metadataservice.GetFVServingStatusForFSRequest\x1a=.tecton_proto.metadataservice.GetFVServingStatusForFSResponse\"~\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-fv-serving-status-for-fs:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x16GetAllFeatureFreshness\x12;.tecton_proto.metadataservice.GetAllFeatureFreshnessRequest\x1a<.tecton_proto.metadataservice.GetAllFeatureFreshnessResponse\"{\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-all-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05<\x1a\r\x08\x01\x12\tworkspace*+tecton/workspace#read_materialization_state\x12\x90\x02\n\x13GetFeatureFreshness\x12\x38.tecton_proto.metadataservice.GetFeatureFreshnessRequest\x1a\x39.tecton_proto.metadataservice.GetFeatureFreshnessResponse\"\x83\x01\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-feature-freshness:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xdd\x01\n\x18GetMaterializationStatus\x12=.tecton_proto.metadataservice.GetMaterializationStatusRequest\x1a>.tecton_proto.metadataservice.GetMaterializationStatusResponse\"B\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-service/get-materialization-status:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xac\x02\n+GetAllMaterializationStatusInLiveWorkspaces\x12P.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesRequest\x1aQ.tecton_proto.metadataservice.GetAllMaterializationStatusInLiveWorkspacesResponse\"X\x82\xd3\xe4\x93\x02J\"E/v1/metadata-service/get-all-materialization-status-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x94\x01\n\x07GetJobs\x12,.tecton_proto.metadataservice.GetJobsRequest\x1a-.tecton_proto.metadataservice.GetJobsResponse\",\x82\xd3\xe4\x93\x02\x1e\"\x19/v1/metadata-service/jobs:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xad\x01\n\rGetJobDetails\x12\x32.tecton_proto.metadataservice.GetJobDetailsRequest\x1a\x33.tecton_proto.metadataservice.GetJobDetailsResponse\"3\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/job-details:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xf2\x01\n\x1d\x46orceRetryMaterializationTask\x12\x42.tecton_proto.metadataservice.ForceRetryMaterializationTaskRequest\x1a\x43.tecton_proto.metadataservice.ForceRetryMaterializationTaskResponse\"H\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/force-retry-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe5\x01\n\x1aRestartMaterializationTask\x12?.tecton_proto.metadataservice.RestartMaterializationTaskRequest\x1a@.tecton_proto.metadataservice.RestartMaterializationTaskResponse\"D\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/restart-materialization-task:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xe0\x01\n\x0eGetSparkConfig\x12\x33.tecton_proto.metadataservice.GetSparkConfigRequest\x1a\x34.tecton_proto.metadataservice.GetSparkConfigResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-spark-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xae\x02\n!GetMetricAndExpectationDefinition\x12\x46.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionRequest\x1aG.tecton_proto.metadataservice.GetMetricAndExpectationDefinitionResponse\"x\x82\xd3\xe4\x93\x02?\":/v1/metadata-service/get-metric-and-expectation-definition:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetFeatureView\x12\x33.tecton_proto.metadataservice.GetFeatureViewRequest\x1a\x34.tecton_proto.metadataservice.GetFeatureViewResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-feature-view:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf0\x01\n,GetMaterializingFeatureViewsInLiveWorkspaces\x12\x16.google.protobuf.Empty\x1aR.tecton_proto.metadataservice.GetMaterializingFeatureViewsInLiveWorkspacesResponse\"T\x82\xd3\xe4\x93\x02\x46\"A/v1/metadata-service/get-materializing-features-in-live-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xec\x01\n\x11QueryFeatureViews\x12\x36.tecton_proto.metadataservice.QueryFeatureViewsRequest\x1a\x37.tecton_proto.metadataservice.QueryFeatureViewsResponse\"f\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/query-feature-views:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x99\x02\n\x15GetFeatureViewSummary\x12:.tecton_proto.metadataservice.GetFeatureViewSummaryRequest\x1a;.tecton_proto.metadataservice.GetFeatureViewSummaryResponse\"\x86\x01\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-package/get-feature-view-summary:\x01*\xa2\xbc\xe6\xc0\x05H\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*+tecton/workspace#read_materialization_state\x12\xf9\x01\n\x14GetVirtualDataSource\x12\x39.tecton_proto.metadataservice.GetVirtualDataSourceRequest\x1a:.tecton_proto.metadataservice.GetVirtualDataSourceResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-virtual-data-source:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8a\x02\n\x18GetAllVirtualDataSources\x12=.tecton_proto.metadataservice.GetAllVirtualDataSourcesRequest\x1a>.tecton_proto.metadataservice.GetAllVirtualDataSourcesResponse\"o\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-all-virtual-data-sources:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x90\x01\n\x10IngestClientLogs\x12\x35.tecton_proto.metadataservice.IngestClientLogsRequest\x1a\x16.google.protobuf.Empty\"-\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xbe\x01\n\x0fIngestAnalytics\x12\x34.tecton_proto.metadataservice.IngestAnalyticsRequest\x1a\x16.google.protobuf.Empty\"]\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/ingest-analytics:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa2\x02\n\x1bGetVirtualDataSourceSummary\x12@.tecton_proto.metadataservice.GetVirtualDataSourceSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetVirtualDataSourceSummaryResponse\"~\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/get-virtual-data-source-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xc3\x01\n\x07GetFcos\x12,.tecton_proto.metadataservice.GetFcosRequest\x1a-.tecton_proto.metadataservice.GetFcosResponse\"[\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-fcos:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xa1\x01\n\tGetEntity\x12..tecton_proto.metadataservice.GetEntityRequest\x1a/.tecton_proto.metadataservice.GetEntityResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xe0\x01\n\x0eGetAllEntities\x12\x33.tecton_proto.metadataservice.GetAllEntitiesRequest\x1a\x34.tecton_proto.metadataservice.GetAllEntitiesResponse\"c\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/get-all-entities:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf4\x01\n\x10GetEntitySummary\x12\x35.tecton_proto.metadataservice.GetEntitySummaryRequest\x1a\x36.tecton_proto.metadataservice.GetEntitySummaryResponse\"q\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-package/get-entity-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xeb\x01\n\x11GetTransformation\x12\x36.tecton_proto.metadataservice.GetTransformationRequest\x1a\x37.tecton_proto.metadataservice.GetTransformationResponse\"e\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/get-transformation:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xfc\x01\n\x15GetAllTransformations\x12:.tecton_proto.metadataservice.GetAllTransformationsRequest\x1a;.tecton_proto.metadataservice.GetAllTransformationsResponse\"j\x82\xd3\xe4\x93\x02\x31\",/v1/metadata-service/get-all-transformations:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x94\x02\n\x18GetTransformationSummary\x12=.tecton_proto.metadataservice.GetTransformationSummaryRequest\x1a>.tecton_proto.metadataservice.GetTransformationSummaryResponse\"y\x82\xd3\xe4\x93\x02\x34\"//v1/metadata-package/get-transformation-summary:\x01*\xa2\xbc\xe6\xc0\x05\x39\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace*\x1ctecton/workspace#read_config\x12\xd6\x01\n\x10\x46indFcoWorkspace\x12\x35.tecton_proto.metadataservice.FindFcoWorkspaceRequest\x1a\x36.tecton_proto.metadataservice.FindFcoWorkspaceResponse\"S\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/find-fco-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x1b*\x19tecton/platform#read_only\x12\xb8\x01\n\x0eNewStateUpdate\x12\x33.tecton_proto.metadataservice.NewStateUpdateRequest\x1a\x34.tecton_proto.metadataservice.NewStateUpdateResponse\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xbe\x01\n\x10NewStateUpdateV2\x12\x35.tecton_proto.metadataservice.NewStateUpdateRequestV2\x1a\x36.tecton_proto.metadataservice.NewStateUpdateResponseV2\";\xa2\xbc\xe6\xc0\x05\x35\x1a\x15\x08\x01\x12\x11request.workspace*\x1ctecton/workspace#create_plan\x12\xb8\x01\n\x10ValidateLocalFco\x12\x35.tecton_proto.metadataservice.ValidateLocalFcoRequest\x1a\x36.tecton_proto.metadataservice.ValidateLocalFcoResponse\"5\xa2\xbc\xe6\xc0\x05/*-tecton/organization#validate_notebook_objects\x12\xb6\x01\n\x10QueryStateUpdate\x12\x35.tecton_proto.metadataservice.QueryStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.QueryStateUpdateResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xf7\x01\n\x12QueryStateUpdateV2\x12\x37.tecton_proto.metadataservice.QueryStateUpdateRequestV2\x1a\x38.tecton_proto.metadataservice.QueryStateUpdateResponseV2\"n\x82\xd3\xe4\x93\x02\x35\"0/v1/metadata-service/query-state-update-response:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x8b\x01\n\x10\x41pplyStateUpdate\x12\x35.tecton_proto.metadataservice.ApplyStateUpdateRequest\x1a\x36.tecton_proto.metadataservice.ApplyStateUpdateResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb0\x01\n\nGetConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/get-configs:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xcb\x01\n\x12GetGlobalsForWebUI\x12\x16.google.protobuf.Empty\x1a\x38.tecton_proto.metadataservice.GetGlobalsForWebUIResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-globals-for-web-ui:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x98\x01\n\x0fGetLoginConfigs\x12\x16.google.protobuf.Empty\x1a\x30.tecton_proto.metadataservice.GetConfigsResponse\";\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-login-configs:\x01*\xa2\xbc\xe6\xc0\x05\x04\x08\x01\x10\x01\x12?\n\x03Nop\x12\x16.google.protobuf.Empty\x1a\x16.google.protobuf.Empty\"\x08\xa2\xbc\xe6\xc0\x05\x02\x10\x01\x12\xe3\x01\n\x19GetStateUpdatePlanSummary\x12>.tecton_proto.metadataservice.GetStateUpdatePlanSummaryRequest\x1a?.tecton_proto.metadataservice.GetStateUpdatePlanSummaryResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-state-update-plan-summary:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xed\x01\n\x11GetStateUpdateLog\x12\x36.tecton_proto.metadataservice.GetStateUpdateLogRequest\x1a\x37.tecton_proto.metadataservice.GetStateUpdateLogResponse\"g\x82\xd3\xe4\x93\x02.\")/v1/metadata-service/get-state-update-log:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x01\n\x0eGetRestoreInfo\x12\x33.tecton_proto.metadataservice.GetRestoreInfoRequest\x1a\x34.tecton_proto.metadataservice.GetRestoreInfoResponse\"3\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xb0\x02\n\x0f\x43reateWorkspace\x12\x34.tecton_proto.metadataservice.CreateWorkspaceRequest\x1a\x16.google.protobuf.Empty\"\xce\x01\xa2\xbc\xe6\xc0\x05&*$tecton/organization#create_workspace\xa2\xbc\xe6\xc0\x05P2N\n\x1b\x63\x61pabilities.materializable\x12\x04true\x1a)tecton/organization#create_workspace_live\x82\xd3\xe4\x93\x02*\"%/v1/metadata-service/create-workspace:\x01*\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x63reate_workspace\x1a\x01\x31\x12\xb5\x01\n\x0f\x44\x65leteWorkspace\x12\x34.tecton_proto.metadataservice.DeleteWorkspaceRequest\x1a\x16.google.protobuf.Empty\"T\xa2\xbc\xe6\xc0\x05\x32\x1a\r\x08\x01\x12\tworkspace*!tecton/workspace#delete_workspace\xf2\x99\xbd\x46\x17\x08\x01\x12\x10\x64\x65lete_workspace\x1a\x01\x31\x12\xb4\x01\n\x0eListWorkspaces\x12\x33.tecton_proto.metadataservice.ListWorkspacesRequest\x1a\x34.tecton_proto.metadataservice.ListWorkspacesResponse\"7\x82\xd3\xe4\x93\x02)\"$/v1/metadata-service/list-workspaces:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xdf\x01\n\x0cGetWorkspace\x12\x31.tecton_proto.metadataservice.GetWorkspaceRequest\x1a\x32.tecton_proto.metadataservice.GetWorkspaceResponse\"h\x82\xd3\xe4\x93\x02\'\"\"/v1/metadata-service/get-workspace:\x01*\xa2\xbc\xe6\xc0\x05\x35\x1a\x12\x08\x01\x12\x0eworkspace_name*\x1ftecton/workspace#read_workspace\x12\xbd\x01\n\x10IntrospectApiKey\x12\x35.tecton_proto.metadataservice.IntrospectApiKeyRequest\x1a\x36.tecton_proto.metadataservice.IntrospectApiKeyResponse\":\x82\xd3\xe4\x93\x02,\"\'/v1/metadata-service/introspect-api-key:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\x9a\x02\n\x14\x43reateServiceAccount\x12\x39.tecton_proto.metadataservice.CreateServiceAccountRequest\x1a:.tecton_proto.metadataservice.CreateServiceAccountResponse\"\x8a\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/create-service-account:\x01*\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x63reate_service_account\x1a\x01\x31\x12\xc4\x01\n\x12GetServiceAccounts\x12\x37.tecton_proto.metadataservice.GetServiceAccountsRequest\x1a\x38.tecton_proto.metadataservice.GetServiceAccountsResponse\";\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/get-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xa5\x02\n\x14UpdateServiceAccount\x12\x39.tecton_proto.metadataservice.UpdateServiceAccountRequest\x1a:.tecton_proto.metadataservice.UpdateServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/update-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16update_service_account\x1a\x01\x31\x12\xa5\x02\n\x14\x44\x65leteServiceAccount\x12\x39.tecton_proto.metadataservice.DeleteServiceAccountRequest\x1a:.tecton_proto.metadataservice.DeleteServiceAccountResponse\"\x95\x01\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/delete-service-account:\x01*\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x1d\x08\x01\x12\x16\x64\x65lete_service_account\x1a\x01\x31\x12\x8e\x02\n\x0c\x43reateApiKey\x12\x31.tecton_proto.metadataservice.CreateApiKeyRequest\x1a\x32.tecton_proto.metadataservice.CreateApiKeyResponse\"\x96\x01\xa2\xbc\xe6\xc0\x05,**tecton/organization#create_service_account\xa2\xbc\xe6\xc0\x05\x44\x32\x42\n\x08is_admin\x12\x04true\x1a\x30tecton/organization#create_service_account_admin\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x63reate_api_key\x1a\x01\x31\x12\xb2\x01\n\x0c\x44\x65leteApiKey\x12\x31.tecton_proto.metadataservice.DeleteApiKeyRequest\x1a\x16.google.protobuf.Empty\"W\xa2\xbc\xe6\xc0\x05\x37\x1a\x06\x08\x02\x12\x02id*-tecton/service_account#manage_service_account\xf2\x99\xbd\x46\x15\x08\x01\x12\x0e\x64\x65lete_api_key\x1a\x01\x31\x12|\n\x0bListApiKeys\x12\x30.tecton_proto.metadataservice.ListApiKeysRequest\x1a\x31.tecton_proto.metadataservice.ListApiKeysResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xda\x01\n\x1b\x43reateSavedFeatureDataFrame\x12@.tecton_proto.metadataservice.CreateSavedFeatureDataFrameRequest\x1a\x41.tecton_proto.metadataservice.CreateSavedFeatureDataFrameResponse\"6\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#update_dataset\x12\xaf\x01\n\x1c\x41rchiveSavedFeatureDataFrame\x12\x41.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameRequest\x1a\x42.tecton_proto.metadataservice.ArchiveSavedFeatureDataFrameResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xcf\x01\n\x18GetSavedFeatureDataFrame\x12=.tecton_proto.metadataservice.GetSavedFeatureDataFrameRequest\x1a>.tecton_proto.metadataservice.GetSavedFeatureDataFrameResponse\"4\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\x9b\x02\n\x1cGetAllSavedFeatureDataFrames\x12\x41.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesRequest\x1a\x42.tecton_proto.metadataservice.GetAllSavedFeatureDataFramesResponse\"t\x82\xd3\xe4\x93\x02:\"5/v1/metadata-service/get-all-saved-feature-dataframes:\x01*\xa2\xbc\xe6\xc0\x05.\x1a\r\x08\x01\x12\tworkspace*\x1dtecton/workspace#read_dataset\x12\xa6\x01\n\x19GetNewIngestDataframeInfo\x12>.tecton_proto.metadataservice.GetNewIngestDataframeInfoRequest\x1a?.tecton_proto.metadataservice.GetNewIngestDataframeInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xb7\x01\n\x0fIngestDataframe\x12\x34.tecton_proto.metadataservice.IngestDataframeRequest\x1a\x35.tecton_proto.metadataservice.IngestDataframeResponse\"7\xa2\xbc\xe6\xc0\x05\x31\x1a\r\x08\x01\x12\tworkspace* tecton/workspace#ingest_features\x12\xcd\x01\n\x13GetClusterAdminInfo\x12\x16.google.protobuf.Empty\x1a\x39.tecton_proto.metadataservice.GetClusterAdminInfoResponse\"c\x82\xd3\xe4\x93\x02\x30\"+/v1/metadata-service/get-cluster-admin-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xff\x01\n\x11\x43reateClusterUser\x12\x36.tecton_proto.metadataservice.CreateClusterUserRequest\x1a\x37.tecton_proto.metadataservice.CreateClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/create-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#create_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x63reate_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x44\x65leteClusterUser\x12\x36.tecton_proto.metadataservice.DeleteClusterUserRequest\x1a\x37.tecton_proto.metadataservice.DeleteClusterUserResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/delete-cluster-user:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x64\x65lete_account_user\x1a\x01\x31\x12\xff\x01\n\x11\x43lusterUserAction\x12\x36.tecton_proto.metadataservice.ClusterUserActionRequest\x1a\x37.tecton_proto.metadataservice.ClusterUserActionResponse\"y\x82\xd3\xe4\x93\x02-\"(/v1/metadata-service/cluster-user-action:\x01*\xa2\xbc\xe6\xc0\x05!*\x1ftecton/organization#manage_user\xf2\x99\xbd\x46\x1a\x08\x01\x12\x13\x61\x63\x63ount_user_action\x1a\x01\x31\x12\xdf\x01\n\x19GetUserDeploymentSettings\x12\x16.google.protobuf.Empty\x1a?.tecton_proto.metadataservice.GetUserDeploymentSettingsResponse\"i\x82\xd3\xe4\x93\x02\x36\"1/v1/metadata-service/get-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9c\x02\n\x1cUpdateUserDeploymentSettings\x12\x41.tecton_proto.metadataservice.UpdateUserDeploymentSettingsRequest\x1a\x42.tecton_proto.metadataservice.UpdateUserDeploymentSettingsResponse\"u\x82\xd3\xe4\x93\x02\x39\"4/v1/metadata-service/update-user-deployment-settings:\x01*\xa2\xbc\xe6\xc0\x05\x30*.tecton/organization#manage_deployment_settings\x12\xec\x01\n\x1dGetInternalSparkClusterStatus\x12\x16.google.protobuf.Empty\x1a\x43.tecton_proto.metadataservice.GetInternalSparkClusterStatusResponse\"n\x82\xd3\xe4\x93\x02;\"6/v1/metadata-service/get-internal-spark-cluster-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x9a\x01\n\x15GetDeleteEntitiesInfo\x12:.tecton_proto.metadataservice.GetDeleteEntitiesInfoRequest\x1a;.tecton_proto.metadataservice.GetDeleteEntitiesInfoResponse\"\x08\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc0\x01\n\x0e\x44\x65leteEntities\x12\x33.tecton_proto.metadataservice.DeleteEntitiesRequest\x1a\x34.tecton_proto.metadataservice.DeleteEntitiesResponse\"C\xa2\xbc\xe6\xc0\x05=\x1a\x19\x08\x01\x12\x15\x66\x63o_locator.workspace* tecton/workspace#delete_features\x12\xde\x01\n\x0fGetHiveMetadata\x12\x34.tecton_proto.metadataservice.GetHiveMetadataRequest\x1a\x35.tecton_proto.metadataservice.GetHiveMetadataResponse\"^\x82\xd3\xe4\x93\x02+\"&/v1/metadata-service/get-hive-metadata:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xf7\x01\n\x13GetOnboardingStatus\x12\x38.tecton_proto.metadataservice.GetOnboardingStatusRequest\x1a\x39.tecton_proto.metadataservice.GetOnboardingStatusResponse\"k\x82\xd3\xe4\x93\x02/\"*/v1/metadata-service/get-onboarding-status:\x01*\xa2\xbc\xe6\xc0\x05\x30\x1a\r\x08\x01\x12\tworkspace*\x1ftecton/workspace#read_workspace\x12\xe3\x01\n\x1aGetDataPlatformSetupStatus\x12\x16.google.protobuf.Empty\x1a@.tecton_proto.metadataservice.GetDataPlatformSetupStatusResponse\"k\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-data-platform-setup-status:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\x80\x02\n\x16GetObservabilityConfig\x12;.tecton_proto.metadataservice.GetObservabilityConfigRequest\x1a<.tecton_proto.metadataservice.GetObservabilityConfigResponse\"k\x82\xd3\xe4\x93\x02\x32\"-/v1/metadata-service/get-observability-config:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\xd3\x01\n\x0bQueryMetric\x12\x30.tecton_proto.metadataservice.QueryMetricRequest\x1a\x31.tecton_proto.metadataservice.QueryMetricResponse\"_\x82\xd3\xe4\x93\x02&\"!/v1/metadata-service/query-metric:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_config\x12\x95\x02\n\x1bGetFeatureValidationSummary\x12@.tecton_proto.metadataservice.GetFeatureValidationSummaryRequest\x1a\x41.tecton_proto.metadataservice.GetFeatureValidationSummaryResponse\"q\x82\xd3\xe4\x93\x02\x38\"3/v1/metadata-service/get-feature-validation-summary:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\x91\x02\n\x1aGetFeatureValidationResult\x12?.tecton_proto.metadataservice.GetFeatureValidationResultRequest\x1a@.tecton_proto.metadataservice.GetFeatureValidationResultResponse\"p\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-feature-validation-result:\x01*\xa2\xbc\xe6\xc0\x05-\x1a\r\x08\x01\x12\tworkspace*\x1ctecton/workspace#read_metric\x12\xfb\x01\n\x16GetFeatureServerConfig\x12;.tecton_proto.metadataservice.GetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"f\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/get-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xa4\x02\n\x16SetFeatureServerConfig\x12;.tecton_proto.metadataservice.SetFeatureServerConfigRequest\x1a<.tecton_proto.metadataservice.GetFeatureServerConfigResponse\"\x8e\x01\x82\xd3\xe4\x93\x02\x33\"./v1/metadata-service/set-feature-server-config:\x01*\xa2\xbc\xe6\xc0\x05**(tecton/organization#scale_feature_server\xf2\x99\xbd\x46 \x08\x01\x12\x19set_feature_server_config\x1a\x01\x31\x12\xb5\x01\n\x07GetUser\x12,.tecton_proto.metadataservice.GetUserRequest\x1a-.tecton_proto.metadataservice.GetUserResponse\"M\x82\xd3\xe4\x93\x02\"\"\x1d/v1/metadata-service/get-user:\x01*\xa2\xbc\xe6\xc0\x05\x1f*\x1dtecton/organization#list_user\x12\xe6\x01\n\x1aGetOfflineStoreCredentials\x12?.tecton_proto.metadataservice.GetOfflineStoreCredentialsRequest\x1a@.tecton_proto.metadataservice.GetOfflineStoreCredentialsResponse\"E\x82\xd3\xe4\x93\x02\x37\"2/v1/metadata-service/get-offline-store-credentials:\x01*\xa2\xbc\xe6\xc0\x05\x02@\x01\x12\xc9\x01\n\nListModels\x12/.tecton_proto.metadataservice.ListModelsRequest\x1a\x30.tecton_proto.metadataservice.ListModelsResponse\"X\x82\xd3\xe4\x93\x02%\" /v1/metadata-service/list-models:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organization\x12\xd2\x01\n\x0cGetModelInfo\x12\x31.tecton_proto.metadataservice.GetModelInfoRequest\x1a\x32.tecton_proto.metadataservice.GetModelInfoResponse\"[\x82\xd3\xe4\x93\x02(\"#/v1/metadata-service/get-model-info:\x01*\xa2\xbc\xe6\xc0\x05\'*%tecton/organization#read_organizationBg\n\x1a\x63om.tecton.metadataserviceB\x14MetadataServiceProtoP\x01Z1github.com/tecton-ai/tecton_proto/metadataservice')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tecton_proto.metadataservice.metadata_service_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\032com.tecton.metadataserviceB\024MetadataServiceProtoP\001Z1github.com/tecton-ai/tecton_proto/metadataservice'
@@ -309,16 +309,16 @@
   _METADATASERVICE.methods_by_name['GetUser']._serialized_options = b'\202\323\344\223\002\"\"\035/v1/metadata-service/get-user:\001*\242\274\346\300\005\037*\035tecton/organization#list_user'
   _METADATASERVICE.methods_by_name['GetOfflineStoreCredentials']._options = None
   _METADATASERVICE.methods_by_name['GetOfflineStoreCredentials']._serialized_options = b'\202\323\344\223\0027\"2/v1/metadata-service/get-offline-store-credentials:\001*\242\274\346\300\005\002@\001'
   _METADATASERVICE.methods_by_name['ListModels']._options = None
   _METADATASERVICE.methods_by_name['ListModels']._serialized_options = b'\202\323\344\223\002%\" /v1/metadata-service/list-models:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
   _METADATASERVICE.methods_by_name['GetModelInfo']._options = None
   _METADATASERVICE.methods_by_name['GetModelInfo']._serialized_options = b'\202\323\344\223\002(\"#/v1/metadata-service/get-model-info:\001*\242\274\346\300\005\'*%tecton/organization#read_organization'
-  _SORTDIRECTION._serialized_start=27230
-  _SORTDIRECTION._serialized_end=27292
+  _SORTDIRECTION._serialized_start=27312
+  _SORTDIRECTION._serialized_end=27374
   _JOBSKEYSET._serialized_start=1641
   _JOBSKEYSET._serialized_end=1785
   _PAGINATIONREQUEST._serialized_start=1788
   _PAGINATIONREQUEST._serialized_end=1996
   _PAGINATIONRESPONSE._serialized_start=1999
   _PAGINATIONRESPONSE._serialized_end=2239
   _VALIDATIONRESULTTOKEN._serialized_start=2242
@@ -647,14 +647,14 @@
   _FEATURESERVERAUTOSCALINGCONFIG._serialized_end=26527
   _GETFEATURESERVERCONFIGREQUEST._serialized_start=26529
   _GETFEATURESERVERCONFIGREQUEST._serialized_end=26560
   _GETFEATURESERVERCONFIGRESPONSE._serialized_start=26563
   _GETFEATURESERVERCONFIGRESPONSE._serialized_end=26851
   _SETFEATURESERVERCONFIGREQUEST._serialized_start=26854
   _SETFEATURESERVERCONFIGREQUEST._serialized_end=27033
-  _GETOFFLINESTORECREDENTIALSREQUEST._serialized_start=27035
-  _GETOFFLINESTORECREDENTIALSREQUEST._serialized_end=27135
-  _GETOFFLINESTORECREDENTIALSRESPONSE._serialized_start=27137
-  _GETOFFLINESTORECREDENTIALSRESPONSE._serialized_end=27228
-  _METADATASERVICE._serialized_start=27296
-  _METADATASERVICE._serialized_end=46606
+  _GETOFFLINESTORECREDENTIALSREQUEST._serialized_start=27036
+  _GETOFFLINESTORECREDENTIALSREQUEST._serialized_end=27217
+  _GETOFFLINESTORECREDENTIALSRESPONSE._serialized_start=27219
+  _GETOFFLINESTORECREDENTIALSRESPONSE._serialized_end=27310
+  _METADATASERVICE._serialized_start=27378
+  _METADATASERVICE._serialized_end=46688
 # @@protoc_insertion_point(module_scope)
```

### Comparing `tecton-0.9.3/tecton_proto/offlinestore/delta/metadata_pb2.py` & `tecton-0.9.4/tecton_proto/offlinestore/delta/metadata_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/offlinestore/delta/transaction_writer_pb2.py` & `tecton-0.9.4/tecton_proto/offlinestore/delta/transaction_writer_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/online_store/feature_value_pb2.py` & `tecton-0.9.4/tecton_proto/online_store/feature_value_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/online_store/status_entry_pb2.py` & `tecton-0.9.4/tecton_proto/online_store/status_entry_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/online_store_writer/config_pb2.py` & `tecton-0.9.4/tecton_proto/online_store_writer/config_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/online_store_writer/copier_pb2.py` & `tecton-0.9.4/tecton_proto/online_store_writer/copier_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py` & `tecton-0.9.4/tecton_proto/remoteenvironmentservice/remote_environment_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/secrets/secrets_service_pb2.py` & `tecton-0.9.4/tecton_proto/secrets/secrets_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/snowflake/location_pb2.py` & `tecton-0.9.4/tecton_proto/snowflake/location_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/snowflake/snowflake_credentials_pb2.py` & `tecton-0.9.4/tecton_proto/snowflake/snowflake_credentials_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/spark_api/error_pb2.py` & `tecton-0.9.4/tecton_proto/spark_api/error_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/spark_api/jobs_pb2.py` & `tecton-0.9.4/tecton_proto/spark_api/jobs_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/spark_common/clusters_pb2.py` & `tecton-0.9.4/tecton_proto/spark_common/clusters_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/spark_common/libraries_pb2.py` & `tecton-0.9.4/tecton_proto/spark_common/libraries_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/testhelperservice/test_helper_service_pb2.py` & `tecton-0.9.4/tecton_proto/testhelperservice/test_helper_service_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_proto/validation/validator_pb2.py` & `tecton-0.9.4/tecton_proto/validation/validator_pb2.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/pipeline_helper.py` & `tecton-0.9.4/tecton_snowflake/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/aggregation_plans.py` & `tecton-0.9.4/tecton_snowflake/query/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/dataframe_helper.py` & `tecton-0.9.4/tecton_snowflake/query/dataframe_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/nodes.py` & `tecton-0.9.4/tecton_snowflake/query/nodes.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/queries.py` & `tecton-0.9.4/tecton_snowflake/query/queries.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/rewrite.py` & `tecton-0.9.4/tecton_snowflake/query/rewrite.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/query/translate.py` & `tecton-0.9.4/tecton_snowflake/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/schema_derivation_utils.py` & `tecton-0.9.4/tecton_snowflake/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/snowflake_type_utils.py` & `tecton-0.9.4/tecton_snowflake/snowflake_type_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/sql_helper.py` & `tecton-0.9.4/tecton_snowflake/sql_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/copier_macro.sql` & `tecton-0.9.4/tecton_snowflake/templates/copier_macro.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/delete_orphaned_schemas.sql` & `tecton-0.9.4/tecton_snowflake/templates/delete_orphaned_schemas.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/delete_staged_files.sql` & `tecton-0.9.4/tecton_snowflake/templates/delete_staged_files.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/historical_features.sql` & `tecton-0.9.4/tecton_snowflake/templates/historical_features.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/historical_features_macros.sql` & `tecton-0.9.4/tecton_snowflake/templates/historical_features_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/materialization_tile.sql` & `tecton-0.9.4/tecton_snowflake/templates/materialization_tile.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/materialized_feature_view.sql` & `tecton-0.9.4/tecton_snowflake/templates/materialized_feature_view.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/offline_materialization_macros.sql` & `tecton-0.9.4/tecton_snowflake/templates/offline_materialization_macros.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/run_full_aggregation.sql` & `tecton-0.9.4/tecton_snowflake/templates/run_full_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/run_partial_aggregation.sql` & `tecton-0.9.4/tecton_snowflake/templates/run_partial_aggregation.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates/time_limit.sql` & `tecton-0.9.4/tecton_snowflake/templates/time_limit.sql`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_snowflake/templates_utils.py` & `tecton-0.9.4/tecton_snowflake/templates_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/__init__.py` & `tecton-0.9.4/tecton_spark/__init__.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/aggregation_plans.py` & `tecton-0.9.4/tecton_spark/aggregation_plans.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/data_observability.py` & `tecton-0.9.4/tecton_spark/data_observability.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/data_source_credentials.py` & `tecton-0.9.4/tecton_spark/data_source_credentials.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/data_source_helper.py` & `tecton-0.9.4/tecton_spark/data_source_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/feature_view_spark_utils.py` & `tecton-0.9.4/tecton_spark/feature_view_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/jars/class_loader.py` & `tecton-0.9.4/tecton_spark/jars/class_loader.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/jars/tecton-udfs-spark-3.jar` & `tecton-0.9.4/tecton_spark/jars/tecton-udfs-spark-3.jar`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/materialization_plan.py` & `tecton-0.9.4/tecton_spark/materialization_plan.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/offline_store.py` & `tecton-0.9.4/tecton_spark/offline_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -315,14 +315,29 @@
         SPARK_GCS_DELTA_LOGSTORE_CLASS,
     ]:
         return True
     msg = f"Configuration is not safe for concurrent writes: {configs}"
     raise AssertionError(msg)
 
 
+def _is_dbr_version_greater_than_or_equal_to_14(spark: SparkSession) -> bool:
+    # Return False if not on Databricks.
+    if DBRICKS_RUNTIME_VERSION not in os.environ:
+        return False
+
+    dbr_version = os.environ.get(DBRICKS_RUNTIME_VERSION)
+
+    major_version = dbr_version.split(".")[0]  # "11.3" -> "11"
+    try:
+        return int(major_version) >= 14
+    except ValueError:
+        exception_msg = f'DBR Version from "os.environ":{dbr_version} is incorrect.'
+        raise ValueError(exception_msg)
+
+
 class DeltaWriter(OfflineStoreWriter):
     """DeltaLake implementation of OfflineStoreWriter"""
 
     def __init__(
         self,
         params: OfflineStoreWriterParams,
         spark: SparkSession,
@@ -471,15 +486,21 @@
             self._metadata_writer.set_table_property(
                 self._params.s3_path, "delta.compatibility.symlinkFormatManifest.enabled", "true"
             )
 
     @_with_delta_retries
     def _append_dataframe(self, df: DataFrame) -> None:
         _assert_safe_delta_write_configuration(self._spark)
-        df.write.partitionBy(TIME_PARTITION).format("delta").mode("append").save(self._params.s3_path)
+        df_writer = df.write.partitionBy(TIME_PARTITION).format("delta").mode("append")
+        # For DBR 14+, Deletion Vectors are auto-enabled.
+        # Refer to this section on why we must disable deletion vectors:
+        # https://www.notion.so/tecton/RFC-Support-DLT-Table-as-Data-Source-7ddf14a8ace04b03ba91b2e3f7db03bf?pvs=4#f520cb9f406d4c6f9fc743dc4f399607
+        if _is_dbr_version_greater_than_or_equal_to_14(self._spark):
+            df_writer.option("delta.enableDeletionVectors", "false")
+        df_writer.save(self._params.s3_path)
 
     def _timestamp_to_partition_column(self, df: DataFrame) -> Column:
         # For some insane reason from_unixtime returns a timestamp in the session timezone, so it's pretty annoying to
         # convert a unix time to a formatted UTC timestamp unless the session is set to UTC. This only runs in
         # materialization so we can just assert that that's the case.
         tz = df.sql_ctx.sparkSession.conf.get("spark.sql.session.timeZone")
         if tz not in {"UTC", "Etc/UTC", "GMT"}:
```

### Comparing `tecton-0.9.3/tecton_spark/partial_aggregations.py` & `tecton-0.9.4/tecton_spark/partial_aggregations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/pipeline_helper.py` & `tecton-0.9.4/tecton_spark/pipeline_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/data_source.py` & `tecton-0.9.4/tecton_spark/query/data_source.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/filter.py` & `tecton-0.9.4/tecton_spark/query/filter.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/join.py` & `tecton-0.9.4/tecton_spark/query/join.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/node.py` & `tecton-0.9.4/tecton_spark/query/node.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/pipeline.py` & `tecton-0.9.4/tecton_spark/query/pipeline.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/projection.py` & `tecton-0.9.4/tecton_spark/query/projection.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/query/translate.py` & `tecton-0.9.4/tecton_spark/query/translate.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/schema_derivation_utils.py` & `tecton-0.9.4/tecton_spark/schema_derivation_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/schema_spark_utils.py` & `tecton-0.9.4/tecton_spark/schema_spark_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/spark_helper.py` & `tecton-0.9.4/tecton_spark/spark_helper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/spark_schema_wrapper.py` & `tecton-0.9.4/tecton_spark/spark_schema_wrapper.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/time_utils.py` & `tecton-0.9.4/tecton_spark/time_utils.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/type_annotations.py` & `tecton-0.9.4/tecton_spark/type_annotations.py`

 * *Files identical despite different names*

### Comparing `tecton-0.9.3/tecton_spark/udfs.py` & `tecton-0.9.4/tecton_spark/udfs.py`

 * *Files identical despite different names*

