# Comparing `tmp/horde_sdk-0.9.2.tar.gz` & `tmp/horde_sdk-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "horde_sdk-0.9.2.tar", last modified: Mon Mar 25 02:07:25 2024, max compression
+gzip compressed data, was "horde_sdk-0.9.3.tar", last modified: Fri Apr 12 00:59:16 2024, max compression
```

## Comparing `horde_sdk-0.9.2.tar` & `horde_sdk-0.9.3.tar`

### file list

```diff
@@ -1,342 +1,342 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.275485 horde_sdk-0.9.2/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.changelog
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.env.template
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.223485 horde_sdk-0.9.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.223485 horde_sdk-0.9.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.github/workflows/maintests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.github/workflows/prtests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.223485 horde_sdk-0.9.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      287 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    34503 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    42324 2024-03-25 02:07:25.275485 horde_sdk-0.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.223485 horde_sdk-0.9.2/codegen/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    62599 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/ai_horde_codegen_10072023.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/codegen_regex_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)   232106 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/swagger.json
--rw-r--r--   0 runner    (1001) docker     (127)   205944 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/codegen/swagger_openapi3.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.227485 horde_sdk-0.9.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/.pages
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/api_to_sdk_map.md
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/api_to_sdk_payload_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/api_to_sdk_response_map.json
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/build_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/examples.md
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/faq.md
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/getting_started.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.227485 horde_sdk-0.9.2/docs/horde_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/.pages
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.227485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/ai_horde_clients.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/_find_user.md
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/_stats.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_async.md
--rw-r--r--   0 runner    (1001) docker     (127)       57 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_status.md
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/base.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_async.md
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_check.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_pop.md
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_progress.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_status.md
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/generate/_submit.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/workers/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/consts.md
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/exceptions.md
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/fields.md
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/kudos.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/metadata.md
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_api/server_model_names.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/bridge_data.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.231485 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/locale_info/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/locale_info/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.md
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/model_meta.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ai_horde_worker/worker_client.md
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/consts.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/exceptions.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/generic_api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/_reflection.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/apimodels.md
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/consts.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/generic_clients.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/metadata.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/generic_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/utils/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/generic_api/utils/swagger.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/locales/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/locales/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/localize.md
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/logging.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/model_reference/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/model_reference/.pages
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/apimodels.md
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/endpoints.md
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/metadata.md
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/ratings_api/ratings_client.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/horde_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/scripts/.pages
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/scripts/write_all_payload_examples_for_tests.md
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/scripts/write_all_response_examples_for_tests.md
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/horde_sdk/utils.md
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/request_field_names_and_descriptions.json
--rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/response_field_names_and_descriptions.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.235485 horde_sdk-0.9.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.239485 horde_sdk-0.9.2/examples/ai_horde_client/
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/aihorde_dry_run_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/aihorde_manual_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/aihorde_simple_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/alchemy_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/async_aihorde_manual_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/async_aihorde_simple_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ai_horde_client/find_user.py
--rw-r--r--   0 runner    (1001) docker     (127)    43370 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/cat_in_a_hat.webp
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.239485 horde_sdk-0.9.2/examples/ratings_client/
--rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/ratings_client/ratings_api_client_example.py
--rw-r--r--   0 runner    (1001) docker     (127)   178529 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/examples/sketch_mountains_input.jpg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.239485 horde_sdk-0.9.2/horde_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.243485 horde_sdk-0.9.2/horde_sdk/ai_horde_api/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45432 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/ai_horde_clients.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.243485 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/
--rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/_find_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/_stats.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.243485 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.py
--rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_async.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_check.py
--rw-r--r--   0 runner    (1001) docker     (127)    17809 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_progress.py
--rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6952 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
--rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/kudos.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_api/server_model_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/bridge_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/locale_info/
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/locale_info/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/locale_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/model_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ai_horde_worker/worker_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)       88 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/generic_api/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/_reflection.py
--rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/apimodels.py
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)    38579 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/generic_clients.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/generic_api/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38633 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/generic_api/utils/swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)      174 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/localize.py
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.247485 horde_sdk-0.9.2/horde_sdk/model_reference/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/model_reference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/horde_sdk/ratings_api/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ratings_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ratings_api/apimodels.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ratings_api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (127)      824 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ratings_api/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)      601 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/ratings_api/ratings_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/horde_sdk/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/scripts/write_all_payload_examples_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/scripts/write_all_response_examples_for_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      635 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/horde_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.275485 horde_sdk-0.9.2/horde_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    42324 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       98 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-25 02:07:25.000000 horde_sdk-0.9.2/horde_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/requirements.dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/requirements.docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 02:07:25.275485 horde_sdk-0.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/tests/ai_horde_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_alchemy_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)    29446 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    25973 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_generate_api_calls.py
--rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_api/test_swagger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/tests/ai_horde_worker/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ai_horde_worker/test_model_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/tests/ratings_api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/ratings_api/test_init.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.251485 horde_sdk-0.9.2/tests/test_data/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/RequestErrorResponse.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.255485 horde_sdk-0.9.2/tests/test_data/ai_horde_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.259485 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_filter_id_patch.json
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_filters_put.json
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_rate_id_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_pop_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_submit_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_async_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_pop_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_submit_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_award_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_kai_user_id_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_transfer_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_operations_block_worker_ipaddr_worker_id_put.json
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_operations_ipaddr_post.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_put.json
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_sharedkey_id_patch.json
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_status_modes_put.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_teams_post.json
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_teams_team_id_patch.json
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_users_user_id_put.json
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.259485 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_production_responses/
--rw-r--r--   0 runner    (1001) docker     (127)   118737 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.271485 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_patch_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_put_201.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_filters_regex_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_202.json
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_check_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_rate_id_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_submit_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_async_post_202.json
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_submit_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_async_post_202.json
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_pop_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_submit_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_kudos_award_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_kudos_transfer_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_block_worker_ipaddr_worker_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_block_worker_ipaddr_worker_id_put_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_ipaddr_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_put_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_patch_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_models_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_totals_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_models_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_totals_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_models_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_models_model_name_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_put_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_news_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_status_performance_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_patch_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      460 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_put_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_delete_200.json
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_put_200.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.271485 horde_sdk-0.9.2/tests/test_data/ai_horde_api/production_responses/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/production_responses/_v2_interrogate_pop_post_200.json
--rw-r--r--   0 runner    (1001) docker     (127)    99142 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json
--rw-r--r--   0 runner    (1001) docker     (127)   232106 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ai_horde_api/swagger.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.271485 horde_sdk-0.9.2/tests/test_data/images/
--rw-r--r--   0 runner    (1001) docker     (127)    73791 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/images/haidra.png
--rw-r--r--   0 runner    (1001) docker     (127)   178529 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/images/sketch-mountains-input.jpg
--rw-r--r--   0 runner    (1001) docker     (127)   378244 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/images/woman_headshot_bokeh.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.219485 horde_sdk-0.9.2/tests/test_data/ratings_api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.271485 horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)    62732 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
--rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_dynamically_check_apimodels.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_ratings_api_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:25.275485 horde_sdk-0.9.2/tests/testing_result_images/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tests/testing_result_images/.results_go_here
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-03-25 02:07:18.000000 horde_sdk-0.9.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.changelog
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.env.template
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.866960 horde_sdk-0.9.3/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.866960 horde_sdk-0.9.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.github/workflows/maintests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.github/workflows/prtests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2014 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.866960 horde_sdk-0.9.3/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      287 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    34503 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    42324 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1712 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.866960 horde_sdk-0.9.3/codegen/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62599 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/ai_horde_codegen_10072023.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/codegen_regex_fixes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   232106 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/swagger.json
+-rw-r--r--   0 runner    (1001) docker     (127)   205944 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/codegen/swagger_openapi3.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.870960 horde_sdk-0.9.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/api_to_sdk_map.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/api_to_sdk_payload_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1455 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/api_to_sdk_response_map.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/build_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/examples.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/faq.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/getting_started.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.870960 horde_sdk-0.9.3/docs/horde_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/.pages
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.870960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/ai_horde_clients.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.870960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/_find_user.md
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/_stats.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.874960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_async.md
+-rw-r--r--   0 runner    (1001) docker     (127)       57 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_status.md
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/base.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.874960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_async.md
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_check.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_pop.md
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_progress.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_status.md
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/generate/_submit.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.874960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/workers/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/consts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/exceptions.md
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/fields.md
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/kudos.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/metadata.md
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_api/server_model_names.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.874960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/bridge_data.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.874960 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/locale_info/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/locale_info/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.md
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/model_meta.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ai_horde_worker/worker_client.md
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/consts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/exceptions.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/generic_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/_reflection.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/apimodels.md
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/consts.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/generic_clients.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/metadata.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/generic_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/utils/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/generic_api/utils/swagger.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/locales/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/locales/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/localize.md
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/logging.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/model_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/model_reference/.pages
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/apimodels.md
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/endpoints.md
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/metadata.md
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/ratings_api/ratings_client.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/horde_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/scripts/.pages
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/scripts/write_all_payload_examples_for_tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/scripts/write_all_response_examples_for_tests.md
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/horde_sdk/utils.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/request_field_names_and_descriptions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7314 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/response_field_names_and_descriptions.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2572 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.878960 horde_sdk-0.9.3/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.882959 horde_sdk-0.9.3/examples/ai_horde_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/aihorde_dry_run_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/aihorde_manual_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/aihorde_simple_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/alchemy_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/async_aihorde_manual_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4077 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/async_aihorde_simple_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ai_horde_client/find_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43370 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/cat_in_a_hat.webp
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.882959 horde_sdk-0.9.3/examples/ratings_client/
+-rw-r--r--   0 runner    (1001) docker     (127)     2832 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/ratings_client/ratings_api_client_example.py
+-rw-r--r--   0 runner    (1001) docker     (127)   178529 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/examples/sketch_mountains_input.jpg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.882959 horde_sdk-0.9.3/horde_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45432 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/ai_horde_clients.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/
+-rw-r--r--   0 runner    (1001) docker     (127)     3982 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9540 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/_find_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/_stats.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6635 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7027 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12031 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5736 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_check.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17809 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_pop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_progress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4908 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2217 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_submit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6867 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5215 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3061 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2313 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/kudos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_api/server_model_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.886959 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15755 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/bridge_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/locale_info/
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/locale_info/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/locale_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10192 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12732 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/model_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ai_horde_worker/worker_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/generic_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/_reflection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16111 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/apimodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38579 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/generic_clients.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/generic_api/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38633 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/generic_api/utils/swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      174 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/localize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/model_reference/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/model_reference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/ratings_api/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ratings_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8440 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ratings_api/apimodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ratings_api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (127)      824 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ratings_api/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)      601 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/ratings_api/ratings_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.890959 horde_sdk-0.9.3/horde_sdk/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/scripts/write_all_payload_examples_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/scripts/write_all_response_examples_for_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      635 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/horde_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/horde_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    42324 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14722 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       98 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-12 00:59:16.000000 horde_sdk-0.9.3/horde_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/requirements.dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/requirements.docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/ai_horde_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_alchemy_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29446 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25973 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_generate_api_calls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7857 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_dynamically_validate_against_swagger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_api/test_swagger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/ai_horde_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ai_horde_worker/test_model_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/ratings_api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/ratings_api/test_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/test_data/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/RequestErrorResponse.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.894960 horde_sdk-0.9.3/tests/test_data/ai_horde_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.898959 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_filters_filter_id_patch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_filters_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_filters_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_rate_id_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_pop_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_submit_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_async_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_pop_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_interrogate_submit_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_award_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_kai_user_id_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_kudos_transfer_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_operations_block_worker_ipaddr_worker_id_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_operations_ipaddr_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_sharedkeys_sharedkey_id_patch.json
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_status_modes_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_teams_post.json
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_teams_team_id_patch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_users_user_id_put.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.898959 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_production_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)   118737 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.910959 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_filter_id_patch_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_put_201.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_filters_regex_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_async_post_202.json
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_check_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_rate_id_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_submit_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_async_post_202.json
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_pop_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_submit_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_async_post_202.json
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_pop_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_status_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_interrogate_submit_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_kudos_award_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_kudos_transfer_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_block_worker_ipaddr_worker_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_block_worker_ipaddr_worker_id_put_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_ipaddr_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_operations_ipaddr_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_put_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_sharedkeys_sharedkey_id_patch_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_models_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_stats_img_totals_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_models_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_stats_text_totals_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_models_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_models_model_name_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_modes_put_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_news_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_status_performance_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_team_id_patch_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1477 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      460 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_put_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_delete_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_put_200.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.910959 horde_sdk-0.9.3/tests/test_data/ai_horde_api/production_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/production_responses/_v2_interrogate_pop_post_200.json
+-rw-r--r--   0 runner    (1001) docker     (127)    99142 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json
+-rw-r--r--   0 runner    (1001) docker     (127)   232106 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ai_horde_api/swagger.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.910959 horde_sdk-0.9.3/tests/test_data/images/
+-rw-r--r--   0 runner    (1001) docker     (127)    73791 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/images/haidra.png
+-rw-r--r--   0 runner    (1001) docker     (127)   178529 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/images/sketch-mountains-input.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)   378244 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/images/woman_headshot_bokeh.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.862960 horde_sdk-0.9.3/tests/test_data/ratings_api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/UserCheckResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)    62732 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5539 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/UserValidateResponse.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9872 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_dynamically_check_apimodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_ratings_api_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:16.914959 horde_sdk-0.9.3/tests/testing_result_images/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tests/testing_result_images/.results_go_here
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-12 00:59:07.000000 horde_sdk-0.9.3/tox.ini
```

### Comparing `horde_sdk-0.9.2/.changelog` & `horde_sdk-0.9.3/.changelog`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.github/workflows/codeql.yml` & `horde_sdk-0.9.3/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.github/workflows/maintests.yml` & `horde_sdk-0.9.3/.github/workflows/maintests.yml`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.github/workflows/prtests.yml` & `horde_sdk-0.9.3/.github/workflows/prtests.yml`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.github/workflows/release.yml` & `horde_sdk-0.9.3/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.gitignore` & `horde_sdk-0.9.3/.gitignore`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/.pre-commit-config.yaml` & `horde_sdk-0.9.3/.pre-commit-config.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 -   repo: https://github.com/pre-commit/pre-commit-hooks
     rev: v4.5.0
     hooks:
     -   id: check-yaml
     -   id: end-of-file-fixer
     -   id: trailing-whitespace
 -   repo: https://github.com/psf/black
-    rev: 24.2.0
+    rev: 24.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.1
+    rev: v0.3.4
     hooks:
     -    id: ruff
 -   repo: https://github.com/pre-commit/mirrors-mypy
-    rev: 'v1.8.0'
+    rev: 'v1.9.0'
     hooks:
     -   id: mypy
         additional_dependencies: [pydantic, types-requests, types-pytz, types-setuptools, types-urllib3, StrEnum]
```

### Comparing `horde_sdk-0.9.2/CONTRIBUTING.md` & `horde_sdk-0.9.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/LICENSE` & `horde_sdk-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/PKG-INFO` & `horde_sdk-0.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde_sdk
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `horde_sdk-0.9.2/README.md` & `horde_sdk-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/codegen/README.md` & `horde_sdk-0.9.3/codegen/README.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/codegen/ai_horde_codegen_10072023.py` & `horde_sdk-0.9.3/codegen/ai_horde_codegen_10072023.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/codegen/codegen_regex_fixes.py` & `horde_sdk-0.9.3/codegen/codegen_regex_fixes.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/codegen/swagger.json` & `horde_sdk-0.9.3/codegen/swagger.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/codegen/swagger_openapi3.json` & `horde_sdk-0.9.3/codegen/swagger_openapi3.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/api_to_sdk_map.md` & `horde_sdk-0.9.3/docs/api_to_sdk_map.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/api_to_sdk_payload_map.json` & `horde_sdk-0.9.3/docs/api_to_sdk_payload_map.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/api_to_sdk_response_map.json` & `horde_sdk-0.9.3/docs/api_to_sdk_response_map.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/build_docs.py` & `horde_sdk-0.9.3/docs/build_docs.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/faq.md` & `horde_sdk-0.9.3/docs/faq.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/getting_started.md` & `horde_sdk-0.9.3/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/index.md` & `horde_sdk-0.9.3/docs/index.md`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/request_field_names_and_descriptions.json` & `horde_sdk-0.9.3/docs/request_field_names_and_descriptions.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/response_field_names_and_descriptions.json` & `horde_sdk-0.9.3/docs/response_field_names_and_descriptions.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/docs/stylesheets/extra.css` & `horde_sdk-0.9.3/docs/stylesheets/extra.css`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/aihorde_dry_run_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/aihorde_dry_run_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/aihorde_manual_client_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/aihorde_manual_client_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/aihorde_simple_client_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/aihorde_simple_client_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/alchemy_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/alchemy_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/async_aihorde_manual_client_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/async_aihorde_manual_client_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/async_aihorde_simple_client_example.py` & `horde_sdk-0.9.3/examples/ai_horde_client/async_aihorde_simple_client_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ai_horde_client/find_user.py` & `horde_sdk-0.9.3/examples/ai_horde_client/find_user.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/cat_in_a_hat.webp` & `horde_sdk-0.9.3/examples/cat_in_a_hat.webp`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/ratings_client/ratings_api_client_example.py` & `horde_sdk-0.9.3/examples/ratings_client/ratings_api_client_example.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/examples/sketch_mountains_input.jpg` & `horde_sdk-0.9.3/examples/sketch_mountains_input.jpg`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/__init__.py` & `horde_sdk-0.9.3/horde_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/__init__.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/ai_horde_clients.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/ai_horde_clients.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/__init__.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/__init__.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/_find_user.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/_find_user.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/_stats.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/_stats.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_async.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_async.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_pop.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_status.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_status.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/alchemy/_submit.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/base.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/base.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_async.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_async.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_check.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_check.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_pop.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_pop.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_progress.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_progress.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_status.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_status.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/generate/_submit.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/generate/_submit.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/apimodels/workers/_workers_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from collections.abc import Iterator
-from typing import ClassVar
 
-from pydantic import AliasChoices, ConfigDict, Field, RootModel
+from pydantic import AliasChoices, Field, RootModel
 from typing_extensions import override
 
 from horde_sdk.ai_horde_api.apimodels.base import BaseAIHordeRequest
 from horde_sdk.ai_horde_api.consts import WORKER_TYPE
 from horde_sdk.ai_horde_api.endpoints import AI_HORDE_API_ENDPOINT_SUBPATH
 from horde_sdk.ai_horde_api.fields import TeamID, WorkerID
 from horde_sdk.consts import HTTPMethod
@@ -126,16 +125,14 @@
         )
 
     def __hash__(self) -> int:
         raise NotImplementedError("Hashing is not implemented for WorkerDetailItem")
 
 
 class AllWorkersDetailsResponse(HordeResponse, RootModel[list[WorkerDetailItem]]):
-    model_config: ClassVar[ConfigDict] = {}
-
     # @tazlin: The typing of __iter__ in BaseModel seems to assume that RootModel wouldn't also be a parent class.
     # without a `type: ignore``, mypy feels that this is a bad override. This is probably a sub-optimal solution
     # on my part with me hoping to come up with a more elegant path in the future.
     # TODO: fix this?
     def __iter__(self) -> Iterator[WorkerDetailItem]:  # type: ignore
         return iter(self.root)
```

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/consts.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/endpoints.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/exceptions.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/exceptions.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/fields.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/fields.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/kudos.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/kudos.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_api/metadata.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_worker/bridge_data.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_worker/bridge_data.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_worker/locale_info/bridge_data_fields.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ai_horde_worker/model_meta.py` & `horde_sdk-0.9.3/horde_sdk/ai_horde_worker/model_meta.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/consts.py` & `horde_sdk-0.9.3/horde_sdk/consts.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/_reflection.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/_reflection.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/apimodels.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/endpoints.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/generic_clients.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/generic_clients.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/metadata.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/generic_api/utils/swagger.py` & `horde_sdk-0.9.3/horde_sdk/generic_api/utils/swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/logging.py` & `horde_sdk-0.9.3/horde_sdk/logging.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ratings_api/apimodels.py` & `horde_sdk-0.9.3/horde_sdk/ratings_api/apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ratings_api/endpoints.py` & `horde_sdk-0.9.3/horde_sdk/ratings_api/endpoints.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ratings_api/metadata.py` & `horde_sdk-0.9.3/horde_sdk/ratings_api/metadata.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/ratings_api/ratings_client.py` & `horde_sdk-0.9.3/horde_sdk/ratings_api/ratings_client.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/scripts/write_all_payload_examples_for_tests.py` & `horde_sdk-0.9.3/horde_sdk/scripts/write_all_payload_examples_for_tests.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/scripts/write_all_response_examples_for_tests.py` & `horde_sdk-0.9.3/horde_sdk/scripts/write_all_response_examples_for_tests.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk/utils.py` & `horde_sdk-0.9.3/horde_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/horde_sdk.egg-info/PKG-INFO` & `horde_sdk-0.9.3/horde_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: horde_sdk
-Version: 0.9.2
+Version: 0.9.3
 Summary: A python toolkit for interacting with the horde APIs, services, and ecosystem.
 Author-email: tazlin <tazlin.on.github@gmail.com>, db0 <mail@dbzer0.com>
 License: GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `horde_sdk-0.9.2/horde_sdk.egg-info/SOURCES.txt` & `horde_sdk-0.9.3/horde_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/mkdocs.yml` & `horde_sdk-0.9.3/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/pyproject.toml` & `horde_sdk-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 [tool.setuptools.package-data]
 horde_sdk = ["py.typed", "lib.pyi"]
 tests = ["*.json"]
 
 [tool.ruff]
 line-length = 119
+exclude = ["codegen"]
+
+[tool.ruff.lint]
 select = [
   "A",
   "I",
   "E",
   "W",
   "F",
   "UP",
@@ -66,17 +69,16 @@
   "D400",
   "D404",
   "D406",
   "D407",
   "D408",
   "D409",
   "D413",]
-exclude = ["codegen"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["E402"]
 "conftest.py" = ["E402"]
 
 [tool.black]
 line-length = 119
 include = '\.pyi?$'
 exclude = '''
```

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_alchemy_api_calls.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_alchemy_api_calls.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_api_calls.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_api_calls.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_api_models.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_api_models.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_ai_horde_generate_api_calls.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_ai_horde_generate_api_calls.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_dynamically_validate_against_swagger.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_dynamically_validate_against_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_api/test_swagger.py` & `horde_sdk-0.9.3/tests/ai_horde_api/test_swagger.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/ai_horde_worker/test_model_meta.py` & `horde_sdk-0.9.3/tests/ai_horde_worker/test_model_meta.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/conftest.py` & `horde_sdk-0.9.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_async_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_pop_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_submit_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_generate_text_async_post.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_payloads/_v2_workers_worker_id_put.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_production_responses/_v2_workers_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_find_user_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_pop_post_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_delete_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_status_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_delete_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_generate_text_status_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_teams_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_users_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_users_user_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/example_responses/_v2_workers_worker_id_get_200.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/production_responses/_v2_workers_get_200_production.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ai_horde_api/swagger.json` & `horde_sdk-0.9.3/tests/test_data/ai_horde_api/swagger.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/images/haidra.png` & `horde_sdk-0.9.3/tests/test_data/images/haidra.png`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/images/sketch-mountains-input.jpg` & `horde_sdk-0.9.3/tests/test_data/images/sketch-mountains-input.jpg`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/images/woman_headshot_bokeh.png` & `horde_sdk-0.9.3/tests/test_data/images/woman_headshot_bokeh.png`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json` & `horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/ImageRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json` & `horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/UserRatingsResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_data/ratings_api/example_responses/UserValidateResponse.json` & `horde_sdk-0.9.3/tests/test_data/ratings_api/example_responses/UserValidateResponse.json`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_dynamically_check_apimodels.py` & `horde_sdk-0.9.3/tests/test_dynamically_check_apimodels.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_ratings_api_models.py` & `horde_sdk-0.9.3/tests/test_ratings_api_models.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tests/test_utils.py` & `horde_sdk-0.9.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `horde_sdk-0.9.2/tox.ini` & `horde_sdk-0.9.3/tox.ini`

 * *Files identical despite different names*

