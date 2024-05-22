# Comparing `tmp/asyncflows-0.0.0.tar.gz` & `tmp/asyncflows-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asyncflows-0.0.0.tar", max compression
+gzip compressed data, was "asyncflows-0.1.3.tar", max compression
```

## Comparing `asyncflows-0.0.0.tar` & `asyncflows-0.1.3.tar`

### file list

```diff
@@ -1,4 +1,97 @@
--rw-r--r--   0        0        0       13 2024-02-29 23:44:29.635354 asyncflows-0.0.0/README.md
--rw-r--r--   0        0        0        0 2024-02-29 23:43:43.549064 asyncflows-0.0.0/asyncflows/__init__.py
--rw-r--r--   0        0        0      270 2024-02-29 23:44:16.117606 asyncflows-0.0.0/pyproject.toml
--rw-r--r--   0        0        0      353 1970-01-01 00:00:00.000000 asyncflows-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4019 2024-05-22 14:49:22.081858 asyncflows-0.1.3/LICENSE
+-rw-r--r--   0        0        0    32228 2024-05-22 21:28:30.252337 asyncflows-0.1.3/README.md
+-rw-r--r--   0        0        0      215 2024-05-22 14:47:42.260962 asyncflows-0.1.3/asyncflows/__init__.py
+-rw-r--r--   0        0        0      721 2024-05-22 14:46:03.753765 asyncflows-0.1.3/asyncflows/actions/__init__.py
+-rw-r--r--   0        0        0     6399 2024-05-22 14:47:42.261515 asyncflows-0.1.3/asyncflows/actions/base.py
+-rw-r--r--   0        0        0     1867 2024-05-22 14:48:15.151039 asyncflows-0.1.3/asyncflows/actions/execute_db_statement.py
+-rw-r--r--   0        0        0     1385 2024-05-22 14:49:22.057325 asyncflows-0.1.3/asyncflows/actions/extract_list.py
+-rw-r--r--   0        0        0     1982 2024-05-22 18:55:04.922974 asyncflows-0.1.3/asyncflows/actions/extract_pdf_text.py
+-rw-r--r--   0        0        0     1428 2024-05-22 14:47:42.368774 asyncflows-0.1.3/asyncflows/actions/extract_xml_tag.py
+-rw-r--r--   0        0        0     1168 2024-05-22 14:48:15.151258 asyncflows-0.1.3/asyncflows/actions/get_db_schema.py
+-rw-r--r--   0        0        0      582 2024-05-22 14:47:42.261922 asyncflows-0.1.3/asyncflows/actions/get_url.py
+-rw-r--r--   0        0        0      860 2024-05-22 14:47:42.317491 asyncflows-0.1.3/asyncflows/actions/ocr.py
+-rw-r--r--   0        0        0    13123 2024-05-22 21:28:30.269737 asyncflows-0.1.3/asyncflows/actions/prompt.py
+-rw-r--r--   0        0        0     1297 2024-05-22 14:47:42.262400 asyncflows-0.1.3/asyncflows/actions/score.py
+-rw-r--r--   0        0        0     4309 2024-05-22 18:55:04.923294 asyncflows-0.1.3/asyncflows/actions/transformer.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755456 asyncflows-0.1.3/asyncflows/actions/utils/__init__.py
+-rw-r--r--   0        0        0     5351 2024-05-22 21:28:30.270167 asyncflows-0.1.3/asyncflows/actions/utils/prompt_context.py
+-rw-r--r--   0        0        0     3678 2024-05-22 14:49:22.043426 asyncflows-0.1.3/asyncflows/asyncflows.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.755962 asyncflows-0.1.3/asyncflows/examples/__init__.py
+-rw-r--r--   0        0        0   287615 2024-05-22 18:55:04.925115 asyncflows-0.1.3/asyncflows/examples/books/Alice's Adventures in Wonderland, by Lewis Carroll.pdf
+-rw-r--r--   0        0        0     1533 2024-05-22 18:55:04.925408 asyncflows-0.1.3/asyncflows/examples/chatbot.py
+-rw-r--r--   0        0        0     3083 2024-05-22 21:28:30.270775 asyncflows-0.1.3/asyncflows/examples/chatbot.yaml
+-rw-r--r--   0        0        0      716 2024-05-22 14:47:42.404980 asyncflows-0.1.3/asyncflows/examples/debono.py
+-rw-r--r--   0        0        0     3348 2024-05-22 18:55:04.926345 asyncflows-0.1.3/asyncflows/examples/debono.yaml
+-rw-r--r--   0        0        0      699 2024-05-22 14:47:42.405239 asyncflows-0.1.3/asyncflows/examples/get_page_title.py
+-rw-r--r--   0        0        0      423 2024-05-22 18:55:04.926679 asyncflows-0.1.3/asyncflows/examples/get_page_title.yaml
+-rw-r--r--   0        0        0   294692 2024-05-22 14:49:22.077191 asyncflows-0.1.3/asyncflows/examples/hello_world.ipynb
+-rw-r--r--   0        0        0      651 2024-05-22 14:47:42.405500 asyncflows-0.1.3/asyncflows/examples/hello_world.py
+-rw-r--r--   0        0        0      260 2024-05-22 18:55:04.927091 asyncflows-0.1.3/asyncflows/examples/hello_world.yaml
+-rw-r--r--   0        0        0     1309 2024-05-22 18:55:04.927602 asyncflows-0.1.3/asyncflows/examples/rag.py
+-rw-r--r--   0        0        0     1070 2024-05-22 21:29:57.720543 asyncflows-0.1.3/asyncflows/examples/rag.yaml
+-rw-r--r--   0        0        0      280 2024-05-22 14:46:03.758066 asyncflows-0.1.3/asyncflows/examples/recipes/caprese.md
+-rw-r--r--   0        0        0      380 2024-05-22 14:46:03.758468 asyncflows-0.1.3/asyncflows/examples/recipes/chana_masala.md
+-rw-r--r--   0        0        0      329 2024-05-22 14:46:03.758593 asyncflows-0.1.3/asyncflows/examples/recipes/coconut_soup.md
+-rw-r--r--   0        0        0      413 2024-05-22 14:46:03.758715 asyncflows-0.1.3/asyncflows/examples/recipes/gazpacho.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.758850 asyncflows-0.1.3/asyncflows/examples/recipes/guacamole.md
+-rw-r--r--   0        0        0      375 2024-05-22 14:46:03.758989 asyncflows-0.1.3/asyncflows/examples/recipes/hummus.md
+-rw-r--r--   0        0        0      326 2024-05-22 14:46:03.759115 asyncflows-0.1.3/asyncflows/examples/recipes/miso_soup.md
+-rw-r--r--   0        0        0      331 2024-05-22 14:46:03.759255 asyncflows-0.1.3/asyncflows/examples/recipes/omelette.md
+-rw-r--r--   0        0        0      327 2024-05-22 14:46:03.759525 asyncflows-0.1.3/asyncflows/examples/recipes/stir_fry.md
+-rw-r--r--   0        0        0      321 2024-05-22 14:46:03.759651 asyncflows-0.1.3/asyncflows/examples/recipes/yogurt_parfait.md
+-rw-r--r--   0        0        0     1105 2024-05-22 14:47:42.413403 asyncflows-0.1.3/asyncflows/examples/sql_rag.py
+-rw-r--r--   0        0        0     1541 2024-05-22 18:55:04.928130 asyncflows-0.1.3/asyncflows/examples/sql_rag.yaml
+-rw-r--r--   0        0        0     1198 2024-05-22 21:28:30.271238 asyncflows-0.1.3/asyncflows/examples/text_style_transfer.py
+-rw-r--r--   0        0        0      505 2024-05-22 21:28:30.271418 asyncflows-0.1.3/asyncflows/examples/text_style_transfer.yaml
+-rw-r--r--   0        0        0     1890 2024-05-22 14:46:03.761643 asyncflows-0.1.3/asyncflows/log_config.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.761683 asyncflows-0.1.3/asyncflows/models/__init__.py
+-rw-r--r--   0        0        0      204 2024-05-22 14:46:03.761990 asyncflows-0.1.3/asyncflows/models/blob.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.762029 asyncflows-0.1.3/asyncflows/models/config/__init__.py
+-rw-r--r--   0        0        0     3639 2024-05-22 14:49:41.998538 asyncflows-0.1.3/asyncflows/models/config/action.py
+-rw-r--r--   0        0        0     2681 2024-05-22 14:46:03.762355 asyncflows-0.1.3/asyncflows/models/config/common.py
+-rw-r--r--   0        0        0     1115 2024-05-22 14:49:41.998821 asyncflows-0.1.3/asyncflows/models/config/flow.py
+-rw-r--r--   0        0        0     2422 2024-05-22 21:28:30.271703 asyncflows-0.1.3/asyncflows/models/config/model.py
+-rw-r--r--   0        0        0     5075 2024-05-22 14:49:41.999198 asyncflows-0.1.3/asyncflows/models/config/transform.py
+-rw-r--r--   0        0        0     5022 2024-05-22 14:49:22.058252 asyncflows-0.1.3/asyncflows/models/config/value_declarations.py
+-rw-r--r--   0        0        0     3303 2024-05-22 14:49:22.058580 asyncflows-0.1.3/asyncflows/models/file.py
+-rw-r--r--   0        0        0      700 2024-05-22 14:47:42.230677 asyncflows-0.1.3/asyncflows/models/primitives.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.763641 asyncflows-0.1.3/asyncflows/repos/__init__.py
+-rw-r--r--   0        0        0    20233 2024-05-22 14:46:03.764021 asyncflows-0.1.3/asyncflows/repos/blob_repo.py
+-rw-r--r--   0        0        0     4421 2024-05-22 14:46:03.764605 asyncflows-0.1.3/asyncflows/repos/cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764679 asyncflows-0.1.3/asyncflows/scripts/__init__.py
+-rw-r--r--   0        0        0     4943 2024-05-22 14:49:41.999576 asyncflows-0.1.3/asyncflows/scripts/generate_config_schema.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.764985 asyncflows-0.1.3/asyncflows/services/__init__.py
+-rw-r--r--   0        0        0    38289 2024-05-22 14:49:22.059469 asyncflows-0.1.3/asyncflows/services/action_service.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765630 asyncflows-0.1.3/asyncflows/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.765743 asyncflows-0.1.3/asyncflows/tests/action_tests/__init__.py
+-rw-r--r--   0        0        0      724 2024-05-22 14:48:15.166644 asyncflows-0.1.3/asyncflows/tests/action_tests/test_execute_db_statement.py
+-rw-r--r--   0        0        0     1260 2024-05-22 14:47:42.369030 asyncflows-0.1.3/asyncflows/tests/action_tests/test_extract_xml_tag.py
+-rw-r--r--   0        0        0      683 2024-05-22 14:48:15.166773 asyncflows-0.1.3/asyncflows/tests/action_tests/test_get_db_schema.py
+-rw-r--r--   0        0        0     7949 2024-05-22 21:28:30.271910 asyncflows-0.1.3/asyncflows/tests/action_tests/test_prompt.py
+-rw-r--r--   0        0        0     1902 2024-05-22 14:46:03.766510 asyncflows-0.1.3/asyncflows/tests/action_tests/test_transformers.py
+-rw-r--r--   0        0        0    11472 2024-05-22 18:55:04.928549 asyncflows-0.1.3/asyncflows/tests/conftest.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.766988 asyncflows-0.1.3/asyncflows/tests/repos/__init__.py
+-rw-r--r--   0        0        0     8319 2024-05-22 14:46:03.767510 asyncflows-0.1.3/asyncflows/tests/repos/test_blob_repo.py
+-rw-r--r--   0        0        0     6567 2024-05-22 14:46:03.767743 asyncflows-0.1.3/asyncflows/tests/repos/test_cache_repo.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.767812 asyncflows-0.1.3/asyncflows/tests/resources/__init__.py
+-rw-r--r--   0        0        0     5737 2024-05-22 14:47:42.263059 asyncflows-0.1.3/asyncflows/tests/resources/actions.py
+-rw-r--r--   0        0        0     4075 2024-05-22 14:47:42.287921 asyncflows-0.1.3/asyncflows/tests/resources/testing_actions.yaml
+-rw-r--r--   0        0        0    26138 2024-05-22 14:47:42.323379 asyncflows-0.1.3/asyncflows/tests/test_action_service.py
+-rw-r--r--   0        0        0     6172 2024-05-22 14:47:42.263271 asyncflows-0.1.3/asyncflows/tests/test_async_utils.py
+-rw-r--r--   0        0        0    11747 2024-05-22 18:55:04.928969 asyncflows-0.1.3/asyncflows/tests/test_config.py
+-rw-r--r--   0        0        0     2053 2024-05-22 14:48:15.167483 asyncflows-0.1.3/asyncflows/tests/test_run_examples.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:46:03.769749 asyncflows-0.1.3/asyncflows/utils/__init__.py
+-rw-r--r--   0        0        0     9747 2024-05-22 14:49:22.060097 asyncflows-0.1.3/asyncflows/utils/async_utils.py
+-rw-r--r--   0        0        0      676 2024-05-22 14:46:03.770301 asyncflows-0.1.3/asyncflows/utils/cache_utils.py
+-rw-r--r--   0        0        0     8592 2024-05-22 18:55:04.929288 asyncflows-0.1.3/asyncflows/utils/config_utils.py
+-rw-r--r--   0        0        0      725 2024-05-22 14:47:42.393837 asyncflows-0.1.3/asyncflows/utils/db_utils.py
+-rw-r--r--   0        0        0     1320 2024-05-22 14:46:03.771069 asyncflows-0.1.3/asyncflows/utils/jinja_utils.py
+-rw-r--r--   0        0        0     1482 2024-05-22 14:46:03.771192 asyncflows-0.1.3/asyncflows/utils/redis_utils.py
+-rw-r--r--   0        0        0     2686 2024-05-22 14:46:03.771325 asyncflows-0.1.3/asyncflows/utils/request_utils.py
+-rw-r--r--   0        0        0      382 2024-05-22 14:46:03.771449 asyncflows-0.1.3/asyncflows/utils/secret_utils.py
+-rw-r--r--   0        0        0      479 2024-05-22 14:46:03.771565 asyncflows-0.1.3/asyncflows/utils/sentinel_utils.py
+-rw-r--r--   0        0        0      451 2024-05-22 14:46:03.771681 asyncflows-0.1.3/asyncflows/utils/singleton_utils.py
+-rw-r--r--   0        0        0     3333 2024-05-22 14:47:42.303806 asyncflows-0.1.3/asyncflows/utils/transformers_utils.py
+-rw-r--r--   0        0        0     2507 2024-05-22 14:46:03.772050 asyncflows-0.1.3/asyncflows/utils/type_utils.py
+-rw-r--r--   0        0        0     2547 2024-05-22 21:28:30.273329 asyncflows-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0    34339 1970-01-01 00:00:00.000000 asyncflows-0.1.3/PKG-INFO
```

