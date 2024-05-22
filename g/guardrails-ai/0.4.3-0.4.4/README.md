# Comparing `tmp/guardrails_ai-0.4.3.tar.gz` & `tmp/guardrails_ai-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "guardrails_ai-0.4.3.tar", max compression
+gzip compressed data, was "guardrails_ai-0.4.4.tar", max compression
```

## Comparing `guardrails_ai-0.4.3.tar` & `guardrails_ai-0.4.4.tar`

### file list

```diff
@@ -1,134 +1,137 @@
--rw-r--r--   0        0        0    11357 2024-04-10 01:03:46.759287 guardrails_ai-0.4.3/LICENSE
--rw-r--r--   0        0        0     7671 2024-04-10 01:03:46.759287 guardrails_ai-0.4.3/README.md
--rw-r--r--   0        0        0      675 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/__init__.py
--rw-r--r--   0        0        0     1628 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/api_client.py
--rw-r--r--   0        0        0        0 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/__init__.py
--rw-r--r--   0        0        0     7243 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/text2sql.py
--rw-r--r--   0        0        0      783 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/applications/text2sql.rail
--rw-r--r--   0        0        0      288 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/__init__.py
--rw-r--r--   0        0        0     1694 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/credentials.py
--rw-r--r--   0        0        0      156 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/__init__.py
--rw-r--r--   0        0        0     1450 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/serializeable.py
--rw-r--r--   0        0        0     2826 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/generic/stack.py
--rw-r--r--   0        0        0      346 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/__init__.py
--rw-r--r--   0        0        0    15186 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/call.py
--rw-r--r--   0        0        0      936 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/call_inputs.py
--rw-r--r--   0        0        0     1737 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/inputs.py
--rw-r--r--   0        0        0     8287 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/iteration.py
--rw-r--r--   0        0        0     4281 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/history/outputs.py
--rw-r--r--   0        0        0      128 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/input_type.py
--rw-r--r--   0        0        0       76 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/output_type.py
--rw-r--r--   0        0        0     3335 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/classes/validation_outcome.py
--rw-r--r--   0        0        0      324 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/__init__.py
--rw-r--r--   0        0        0     2420 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/configure.py
--rw-r--r--   0        0        0       41 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/guardrails.py
--rw-r--r--   0        0        0      189 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/__init__.py
--rw-r--r--   0        0        0       54 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/console.py
--rw-r--r--   0        0        0     6757 2024-04-10 01:03:46.875288 guardrails_ai-0.4.3/guardrails/cli/hub/create_validator.py
--rw-r--r--   0        0        0       42 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/hub.py
--rw-r--r--   0        0        0     9899 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/install.py
--rw-r--r--   0        0        0     1706 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/hub/submit.py
--rw-r--r--   0        0        0      425 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/logger.py
--rw-r--r--   0        0        0       61 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/__init__.py
--rw-r--r--   0        0        0      907 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/auth.py
--rw-r--r--   0        0        0     5006 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/hub_client.py
--rw-r--r--   0        0        0     1841 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/server/module_manifest.py
--rw-r--r--   0        0        0     1067 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/cli/validate.py
--rw-r--r--   0        0        0      226 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/constants/__init__.py
--rw-r--r--   0        0        0     8367 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/constants.xml
--rw-r--r--   0        0        0    19090 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/datatypes.py
--rw-r--r--   0        0        0     8898 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/document_store.py
--rw-r--r--   0        0        0     7092 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/embedding.py
--rw-r--r--   0        0        0      512 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/errors/__init__.py
--rw-r--r--   0        0        0    52741 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/guard.py
--rw-r--r--   0        0        0       96 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/hub/__init__.py
--rw-r--r--   0        0        0    29727 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/llm_providers.py
--rw-r--r--   0        0        0     2738 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/logger.py
--rw-r--r--   0        0        0      245 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/logging_utils.py
--rw-r--r--   0        0        0      114 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/namespace_template.py
--rw-r--r--   0        0        0      115 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/__init__.py
--rw-r--r--   0        0        0     3946 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/base_prompt.py
--rw-r--r--   0        0        0     1411 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/instructions.py
--rw-r--r--   0        0        0      894 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/prompt/prompt.py
--rw-r--r--   0        0        0    11267 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/rail.py
--rw-r--r--   0        0        0      339 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/__init__.py
--rw-r--r--   0        0        0    15370 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/async_runner.py
--rw-r--r--   0        0        0    21453 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/runner.py
--rw-r--r--   0        0        0     9662 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/stream_runner.py
--rw-r--r--   0        0        0      441 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/run/utils.py
--rw-r--r--   0        0        0      257 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/__init__.py
--rw-r--r--   0        0        0    18617 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/json_schema.py
--rw-r--r--   0        0        0     5708 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/schema.py
--rw-r--r--   0        0        0     9467 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/schema/string_schema.py
--rw-r--r--   0        0        0     1953 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/stores/context.py
--rw-r--r--   0        0        0      168 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/__init__.py
--rw-r--r--   0        0        0       88 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/args.py
--rw-r--r--   0        0        0      472 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/casting_utils.py
--rw-r--r--   0        0        0     1555 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/constants.py
--rw-r--r--   0        0        0      236 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/dataclass.py
--rw-r--r--   0        0        0     4924 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/docs_utils.py
--rw-r--r--   0        0        0      274 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/exception_utils.py
--rw-r--r--   0        0        0     4435 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/hub_telemetry_utils.py
--rw-r--r--   0        0        0    11220 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/json_utils.py
--rw-r--r--   0        0        0       89 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/kwargs.py
--rw-r--r--   0        0        0      288 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/llm_response.py
--rw-r--r--   0        0        0     3244 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/logs_utils.py
--rw-r--r--   0        0        0     4903 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/misc.py
--rw-r--r--   0        0        0      337 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/on_fail.py
--rw-r--r--   0        0        0     1077 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/__init__.py
--rw-r--r--   0        0        0     1390 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/base.py
--rw-r--r--   0        0        0     2792 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/streaming_utils.py
--rw-r--r--   0        0        0    10818 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/v0.py
--rw-r--r--   0        0        0    11107 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/openai_utils/v1.py
--rw-r--r--   0        0        0     2497 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/parsing_utils.py
--rw-r--r--   0        0        0      757 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/__init__.py
--rw-r--r--   0        0        0    18102 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v1.py
--rw-r--r--   0        0        0    17654 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v2.py
--rw-r--r--   0        0        0     7721 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/reask_utils.py
--rw-r--r--   0        0        0     1247 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/safe_get.py
--rw-r--r--   0        0        0     4013 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/sql_utils.py
--rw-r--r--   0        0        0    10841 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/telemetry_utils.py
--rw-r--r--   0        0        0     1488 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/validator_utils.py
--rw-r--r--   0        0        0      507 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/utils/xml_utils.py
--rw-r--r--   0        0        0    18967 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validator_base.py
--rw-r--r--   0        0        0    16056 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validator_service.py
--rw-r--r--   0        0        0     3946 2024-04-10 01:03:46.879288 guardrails_ai-0.4.3/guardrails/validators/__init__.py
--rw-r--r--   0        0        0     1425 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/bug_free_python.py
--rw-r--r--   0        0        0     1703 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/bug_free_sql.py
--rw-r--r--   0        0        0     5567 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/competitor_check.py
--rw-r--r--   0        0        0     7037 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/detect_secrets.py
--rw-r--r--   0        0        0     1857 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/endpoint_is_reachable.py
--rw-r--r--   0        0        0     1373 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/ends_with.py
--rw-r--r--   0        0        0     1884 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/exclude_sql_predicates.py
--rw-r--r--   0        0        0     5533 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/extracted_summary_sentences_match.py
--rw-r--r--   0        0        0     4778 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/extractive_summary.py
--rw-r--r--   0        0        0     3869 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/is_high_quality_translation.py
--rw-r--r--   0        0        0     1540 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/is_profanity_free.py
--rw-r--r--   0        0        0     1091 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/lower_case.py
--rw-r--r--   0        0        0    10671 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/on_topic.py
--rw-r--r--   0        0        0     1204 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/one_line.py
--rw-r--r--   0        0        0     5160 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/pii_filter.py
--rw-r--r--   0        0        0    24837 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/provenance.py
--rw-r--r--   0        0        0     1755 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/pydantic_field_validator.py
--rw-r--r--   0        0        0     3304 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/qa_relevance_llm_eval.py
--rw-r--r--   0        0        0     1784 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/reading_time.py
--rw-r--r--   0        0        0     2455 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/regex_match.py
--rw-r--r--   0        0        0     3075 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/remove_redundant_sentences.py
--rw-r--r--   0        0        0     4572 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/saliency_check.py
--rw-r--r--   0        0        0     3438 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/similar_to_document.py
--rw-r--r--   0        0        0     6425 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/similar_to_list.py
--rw-r--r--   0        0        0     1654 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/sql_column_presence.py
--rw-r--r--   0        0        0     7376 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/toxic_language.py
--rw-r--r--   0        0        0     1422 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/two_words.py
--rw-r--r--   0        0        0     1091 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/upper_case.py
--rw-r--r--   0        0        0     1452 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_choices.py
--rw-r--r--   0        0        0     3198 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_length.py
--rw-r--r--   0        0        0     1946 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_range.py
--rw-r--r--   0        0        0     1407 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/valid_url.py
--rw-r--r--   0        0        0      808 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validators/validators.py
--rw-r--r--   0        0        0    15075 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/validatorsattr.py
--rw-r--r--   0        0        0       93 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/__init__.py
--rw-r--r--   0        0        0     2996 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/base.py
--rw-r--r--   0        0        0     3338 2024-04-10 01:03:46.883288 guardrails_ai-0.4.3/guardrails/vectordb/faiss.py
--rw-r--r--   0        0        0     3488 2024-04-10 01:03:46.887288 guardrails_ai-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    11005 1970-01-01 00:00:00.000000 guardrails_ai-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 20:20:44.169649 guardrails_ai-0.4.4/LICENSE
+-rw-r--r--   0        0        0     7671 2024-05-22 20:20:44.169649 guardrails_ai-0.4.4/README.md
+-rw-r--r--   0        0        0      739 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/__init__.py
+-rw-r--r--   0        0        0     1628 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/api_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/applications/__init__.py
+-rw-r--r--   0        0        0     7271 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/applications/text2sql.py
+-rw-r--r--   0        0        0      783 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/applications/text2sql.rail
+-rw-r--r--   0        0        0    17077 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/async_guard.py
+-rw-r--r--   0        0        0      288 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/__init__.py
+-rw-r--r--   0        0        0     2504 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/credentials.py
+-rw-r--r--   0        0        0      156 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/generic/__init__.py
+-rw-r--r--   0        0        0     1450 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/generic/serializeable.py
+-rw-r--r--   0        0        0     2826 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/generic/stack.py
+-rw-r--r--   0        0        0      346 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/__init__.py
+-rw-r--r--   0        0        0    15189 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/call.py
+-rw-r--r--   0        0        0      936 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/call_inputs.py
+-rw-r--r--   0        0        0     1737 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/inputs.py
+-rw-r--r--   0        0        0     8288 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/iteration.py
+-rw-r--r--   0        0        0     4281 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/history/outputs.py
+-rw-r--r--   0        0        0      128 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/input_type.py
+-rw-r--r--   0        0        0       76 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/output_type.py
+-rw-r--r--   0        0        0     3335 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/classes/validation_outcome.py
+-rw-r--r--   0        0        0      324 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/__init__.py
+-rw-r--r--   0        0        0     3124 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/configure.py
+-rw-r--r--   0        0        0       41 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/guardrails.py
+-rw-r--r--   0        0        0      233 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/hub/__init__.py
+-rw-r--r--   0        0        0       54 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/hub/console.py
+-rw-r--r--   0        0        0     6776 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/hub/create_validator.py
+-rw-r--r--   0        0        0       42 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/hub/hub.py
+-rw-r--r--   0        0        0     8728 2024-05-22 20:20:44.285649 guardrails_ai-0.4.4/guardrails/cli/hub/install.py
+-rw-r--r--   0        0        0     1706 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/hub/submit.py
+-rw-r--r--   0        0        0     3820 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/hub/uninstall.py
+-rw-r--r--   0        0        0     2782 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/hub/utils.py
+-rw-r--r--   0        0        0      427 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/logger.py
+-rw-r--r--   0        0        0       61 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/server/__init__.py
+-rw-r--r--   0        0        0      907 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/server/auth.py
+-rw-r--r--   0        0        0     5444 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/server/hub_client.py
+-rw-r--r--   0        0        0     1841 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/server/module_manifest.py
+-rw-r--r--   0        0        0     1067 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/cli/validate.py
+-rw-r--r--   0        0        0      226 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/constants/__init__.py
+-rw-r--r--   0        0        0     8367 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/constants.xml
+-rw-r--r--   0        0        0    19090 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/datatypes.py
+-rw-r--r--   0        0        0     8868 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/document_store.py
+-rw-r--r--   0        0        0     7092 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/embedding.py
+-rw-r--r--   0        0        0      512 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/errors/__init__.py
+-rw-r--r--   0        0        0    56044 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/guard.py
+-rw-r--r--   0        0        0       96 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/hub/__init__.py
+-rw-r--r--   0        0        0    29728 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/llm_providers.py
+-rw-r--r--   0        0        0     2738 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/logger.py
+-rw-r--r--   0        0        0      245 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/logging_utils.py
+-rw-r--r--   0        0        0      114 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/namespace_template.py
+-rw-r--r--   0        0        0      115 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/prompt/__init__.py
+-rw-r--r--   0        0        0     3947 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/prompt/base_prompt.py
+-rw-r--r--   0        0        0     1412 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/prompt/instructions.py
+-rw-r--r--   0        0        0      895 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/prompt/prompt.py
+-rw-r--r--   0        0        0    11268 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/rail.py
+-rw-r--r--   0        0        0      339 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/run/__init__.py
+-rw-r--r--   0        0        0    15370 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/run/async_runner.py
+-rw-r--r--   0        0        0    21453 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/run/runner.py
+-rw-r--r--   0        0        0     9662 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/run/stream_runner.py
+-rw-r--r--   0        0        0      441 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/run/utils.py
+-rw-r--r--   0        0        0      257 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/schema/__init__.py
+-rw-r--r--   0        0        0    18617 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/schema/json_schema.py
+-rw-r--r--   0        0        0     5708 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/schema/schema.py
+-rw-r--r--   0        0        0     9467 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/schema/string_schema.py
+-rw-r--r--   0        0        0     1953 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/stores/context.py
+-rw-r--r--   0        0        0      168 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/__init__.py
+-rw-r--r--   0        0        0       88 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/args.py
+-rw-r--r--   0        0        0      472 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/casting_utils.py
+-rw-r--r--   0        0        0     1555 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/constants.py
+-rw-r--r--   0        0        0      236 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/dataclass.py
+-rw-r--r--   0        0        0     4924 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/docs_utils.py
+-rw-r--r--   0        0        0      274 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/exception_utils.py
+-rw-r--r--   0        0        0     4435 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/hub_telemetry_utils.py
+-rw-r--r--   0        0        0    11221 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/json_utils.py
+-rw-r--r--   0        0        0       89 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/kwargs.py
+-rw-r--r--   0        0        0      288 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/llm_response.py
+-rw-r--r--   0        0        0     3244 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/logs_utils.py
+-rw-r--r--   0        0        0     4901 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/misc.py
+-rw-r--r--   0        0        0      337 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/on_fail.py
+-rw-r--r--   0        0        0     1077 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/openai_utils/__init__.py
+-rw-r--r--   0        0        0     1390 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/openai_utils/base.py
+-rw-r--r--   0        0        0     2792 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/openai_utils/streaming_utils.py
+-rw-r--r--   0        0        0    10818 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/openai_utils/v0.py
+-rw-r--r--   0        0        0    11107 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/openai_utils/v1.py
+-rw-r--r--   0        0        0     2497 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/parsing_utils.py
+-rw-r--r--   0        0        0      757 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/__init__.py
+-rw-r--r--   0        0        0    18154 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/v1.py
+-rw-r--r--   0        0        0    17705 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/v2.py
+-rw-r--r--   0        0        0     7722 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/reask_utils.py
+-rw-r--r--   0        0        0     1247 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/safe_get.py
+-rw-r--r--   0        0        0     3997 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/sql_utils.py
+-rw-r--r--   0        0        0    10827 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/telemetry_utils.py
+-rw-r--r--   0        0        0     1485 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/validator_utils.py
+-rw-r--r--   0        0        0      507 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/utils/xml_utils.py
+-rw-r--r--   0        0        0    18967 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/validator_base.py
+-rw-r--r--   0        0        0    16002 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/validator_service.py
+-rw-r--r--   0        0        0     3947 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/validators/__init__.py
+-rw-r--r--   0        0        0     1425 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/validators/bug_free_python.py
+-rw-r--r--   0        0        0     1703 2024-05-22 20:20:44.289649 guardrails_ai-0.4.4/guardrails/validators/bug_free_sql.py
+-rw-r--r--   0        0        0     5567 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/competitor_check.py
+-rw-r--r--   0        0        0     7037 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/detect_secrets.py
+-rw-r--r--   0        0        0     1857 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/endpoint_is_reachable.py
+-rw-r--r--   0        0        0     1373 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/ends_with.py
+-rw-r--r--   0        0        0     1884 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/exclude_sql_predicates.py
+-rw-r--r--   0        0        0     5533 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/extracted_summary_sentences_match.py
+-rw-r--r--   0        0        0     4778 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/extractive_summary.py
+-rw-r--r--   0        0        0     3869 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/is_high_quality_translation.py
+-rw-r--r--   0        0        0     1540 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/is_profanity_free.py
+-rw-r--r--   0        0        0     1091 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/lower_case.py
+-rw-r--r--   0        0        0    10671 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/on_topic.py
+-rw-r--r--   0        0        0     1204 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/one_line.py
+-rw-r--r--   0        0        0     5160 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/pii_filter.py
+-rw-r--r--   0        0        0    24837 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/provenance.py
+-rw-r--r--   0        0        0     1755 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/pydantic_field_validator.py
+-rw-r--r--   0        0        0     3304 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/qa_relevance_llm_eval.py
+-rw-r--r--   0        0        0     1784 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/reading_time.py
+-rw-r--r--   0        0        0     2455 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/regex_match.py
+-rw-r--r--   0        0        0     3075 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/remove_redundant_sentences.py
+-rw-r--r--   0        0        0     4572 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/saliency_check.py
+-rw-r--r--   0        0        0     3438 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/similar_to_document.py
+-rw-r--r--   0        0        0     6425 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/similar_to_list.py
+-rw-r--r--   0        0        0     1654 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/sql_column_presence.py
+-rw-r--r--   0        0        0     7376 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/toxic_language.py
+-rw-r--r--   0        0        0     1422 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/two_words.py
+-rw-r--r--   0        0        0     1091 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/upper_case.py
+-rw-r--r--   0        0        0     1452 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/valid_choices.py
+-rw-r--r--   0        0        0     3198 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/valid_length.py
+-rw-r--r--   0        0        0     1946 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/valid_range.py
+-rw-r--r--   0        0        0     1407 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/valid_url.py
+-rw-r--r--   0        0        0      808 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validators/validators.py
+-rw-r--r--   0        0        0    15075 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/validatorsattr.py
+-rw-r--r--   0        0        0       93 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/vectordb/__init__.py
+-rw-r--r--   0        0        0     2996 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/vectordb/base.py
+-rw-r--r--   0        0        0     3316 2024-05-22 20:20:44.293649 guardrails_ai-0.4.4/guardrails/vectordb/faiss.py
+-rw-r--r--   0        0        0     3394 2024-05-22 20:20:44.297649 guardrails_ai-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    11037 1970-01-01 00:00:00.000000 guardrails_ai-0.4.4/PKG-INFO
```

### Comparing `guardrails_ai-0.4.3/LICENSE` & `guardrails_ai-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/README.md` & `guardrails_ai-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/__init__.py` & `guardrails_ai-0.4.4/guardrails/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # Set up __init__.py so that users can do from guardrails import Response, Schema, etc.
 
 from guardrails.guard import Guard
+from guardrails.async_guard import AsyncGuard
 from guardrails.llm_providers import PromptCallableBase
 from guardrails.logging_utils import configure_logging
 from guardrails.prompt import Instructions, Prompt
 from guardrails.rail import Rail
 from guardrails.utils import constants, docs_utils
 from guardrails.validator_base import OnFailAction, Validator, register_validator
 
 __all__ = [
     "Guard",
+    "AsyncGuard",
     "PromptCallableBase",
     "Rail",
     "Validator",
     "OnFailAction",
     "register_validator",
     "constants",
     "docs_utils",
```

### Comparing `guardrails_ai-0.4.3/guardrails/api_client.py` & `guardrails_ai-0.4.4/guardrails/api_client.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/applications/text2sql.py` & `guardrails_ai-0.4.4/guardrails/applications/text2sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
             rail_spec_str = f.read()
 
         # Substitute the parameters in the rail specification.
         if rail_params is not None:
             rail_spec_str = Template(rail_spec_str).safe_substitute(**rail_params)
 
         guard = Guard.from_rail_string(rail_spec_str)
-        guard.reask_prompt = reask_prompt
+        guard.rail.output_schema.reask_prompt_template = reask_prompt
 
         return guard
 
     def _create_docstore_with_examples(
         self,
         examples: Optional[Dict],
         embedding: Type[EmbeddingBase],
```

### Comparing `guardrails_ai-0.4.3/guardrails/applications/text2sql.rail` & `guardrails_ai-0.4.4/guardrails/applications/text2sql.rail`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/generic/serializeable.py` & `guardrails_ai-0.4.4/guardrails/classes/generic/serializeable.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/generic/stack.py` & `guardrails_ai-0.4.4/guardrails/classes/generic/stack.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/history/call.py` & `guardrails_ai-0.4.4/guardrails/classes/history/call.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,16 @@
         #   2. There's nothing to merge
         #   3. The output is a top level ReAsk (i.e. SkeletonReAsk or NonParseableReask)
         #   4. The output is a string
         if (
             self.inputs.full_schema_reask
             or number_of_iterations < 2
             or isinstance(
-                self.iterations.last.validation_response, ReAsk  # type: ignore
+                self.iterations.last.validation_response,  # type: ignore
+                ReAsk,  # type: ignore
             )
             or isinstance(self.iterations.last.validation_response, str)  # type: ignore
         ):
             return self.iterations.last.validation_response  # type: ignore
 
         current_index = 1
         # We've already established that there are iterations,
@@ -406,17 +407,15 @@
                 :-1
             ]
             validated_outcome_panel = Panel(
                 pretty_repr(self.guarded_output),
                 title="Validated Output",
                 style="on #F0FFF0",
             )
-            tree.children[
-                -1
-            ].label.renderable._renderables = previous_panels + (  # type: ignore
+            tree.children[-1].label.renderable._renderables = previous_panels + (  # type: ignore
                 validated_outcome_panel,
             )
 
         return tree
 
     def __str__(self) -> str:
         return pretty_repr(self)
```

### Comparing `guardrails_ai-0.4.3/guardrails/classes/history/call_inputs.py` & `guardrails_ai-0.4.4/guardrails/classes/history/call_inputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/history/inputs.py` & `guardrails_ai-0.4.4/guardrails/classes/history/inputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/history/iteration.py` & `guardrails_ai-0.4.4/guardrails/classes/history/iteration.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         OneOf: pass, fail, error, not run
         """
         return self.outputs.status
 
     @property
     def rich_group(self) -> Group:
         def create_msg_history_table(
-            msg_history: Optional[List[Dict[str, Prompt]]]
+            msg_history: Optional[List[Dict[str, Prompt]]],
         ) -> Union[str, Table]:
             if msg_history is None:
                 return "No message history."
             table = Table(show_lines=True)
             table.add_column("Role", justify="right", no_wrap=True)
             table.add_column("Content")
```

### Comparing `guardrails_ai-0.4.3/guardrails/classes/history/outputs.py` & `guardrails_ai-0.4.4/guardrails/classes/history/outputs.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/classes/validation_outcome.py` & `guardrails_ai-0.4.4/guardrails/classes/validation_outcome.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/cli/configure.py` & `guardrails_ai-0.4.4/guardrails/classes/credentials.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,78 +1,68 @@
+import logging
 import os
-import sys
-import uuid
+from dataclasses import dataclass
 from os.path import expanduser
 from typing import Optional
 
-import typer
+from guardrails.classes.generic.serializeable import Serializeable
 
-from guardrails.cli.guardrails import guardrails
-from guardrails.cli.logger import LEVELS, logger
-from guardrails.cli.server.hub_client import AuthenticationError, get_auth
-
-
-def save_configuration_file(token: str, no_metrics: bool) -> None:
-    home = expanduser("~")
-    guardrails_rc = os.path.join(home, ".guardrailsrc")
-    with open(guardrails_rc, "w") as rc_file:
-        lines = [
-            f"id={str(uuid.uuid4())}{os.linesep}",
-            f"token={token}{os.linesep}",
-            f"no_metrics={str(no_metrics).lower()}",
-        ]
-        rc_file.writelines(lines)
-        rc_file.close()
-
-
-@guardrails.command()
-def configure(
-    token: Optional[str] = typer.Option(
-        help="Your Guardrails Hub auth token.", hide_input=True, default=""
-    ),
-    no_metrics: Optional[str] = typer.Option(
-        help="Opt out of anonymous metrics collection.", default=False
-    ),
-):
-    """Set the global configuration for the Guardrails CLI and Hub."""
-    try:
-        notice_message = """
-
-    You can find your token at https://hub.guardrailsai.com/tokens
-    """
-        logger.log(level=LEVELS.get("NOTICE"), msg=notice_message)  # type: ignore
-        if not token:
-            token = typer.prompt("Token", hide_input=True)
-        logger.info("Configuring...")
-        save_configuration_file(token, no_metrics)  # type: ignore
-
-        logger.info("Validating credentials...")
-        get_auth()
-        success_message = """
-
-    Login successful.
-
-    Get started by installing our RegexMatch validator:
-    https://hub.guardrailsai.com/validator/guardrails_ai/regex_match
-
-    You can install it by running:
-    guardrails hub install hub://guardrails/regex_match
-
-    Find more validators at https://hub.guardrailsai.com
-    """
-        logger.log(level=LEVELS.get("SUCCESS"), msg=success_message)  # type: ignore
-    except AuthenticationError as auth_error:
-        logger.error(auth_error)
-        logger.error(
-            """
-            Check that your token is correct and try again.
-
-            If you don't have your token credentials you can find them here:
-
-            https://hub.guardrailsai.com/tokens
-            """
-        )
-        sys.exit(1)
-    except Exception as e:
-        logger.error("An unexpected error occurred!")
-        logger.error(e)
-        sys.exit(1)
+
+@dataclass
+class Credentials(Serializeable):
+    id: Optional[str] = None
+    token: Optional[str] = None
+    no_metrics: Optional[bool] = False
+    enable_metrics: Optional[bool] = True
+
+    @staticmethod
+    def _to_bool(value: str) -> Optional[bool]:
+        if value.lower() == "true":
+            return True
+        if value.lower() == "false":
+            return False
+        return None
+
+    @staticmethod
+    def from_rc_file(logger: Optional[logging.Logger] = None) -> "Credentials":
+        try:
+            if not logger:
+                logger = logging.getLogger()
+            home = expanduser("~")
+            guardrails_rc = os.path.join(home, ".guardrailsrc")
+            with open(guardrails_rc) as rc_file:
+                lines = rc_file.readlines()
+                filtered_lines = list(filter(lambda l: l.strip(), lines))
+                creds = {}
+                for line in filtered_lines:
+                    line_content = line.split("=", 1)
+                    if len(line_content) != 2:
+                        logger.warn(
+                            """
+                            Invalid line found in .guardrailsrc file!
+                            All lines in this file should follow the format: key=value
+                            Ignoring line contents...
+                            """
+                        )
+                        logger.debug(f".guardrailsrc file location: {guardrails_rc}")
+                    else:
+                        key, value = line_content
+                        key = key.strip()
+                        value = value.strip()
+                        if key == "no_metrics" or key == "enable_metrics":
+                            value = Credentials._to_bool(value)
+
+                        creds[key] = value
+
+                rc_file.close()
+
+                # backfill no_metrics, handle defaults
+                # remove in 0.5.0
+                no_metrics_val = creds.pop("no_metrics", None)
+                if no_metrics_val is not None and creds.get("enable_metrics") is None:
+                    creds["enable_metrics"] = not no_metrics_val
+
+                creds_dict = Credentials.from_dict(creds)
+                return creds_dict
+
+        except FileNotFoundError:
+            return Credentials.from_dict({})  # type: ignore
```

### Comparing `guardrails_ai-0.4.3/guardrails/cli/hub/create_validator.py` & `guardrails_ai-0.4.4/guardrails/cli/hub/create_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: E501
 import os
 from datetime import date
 from string import Template
 
 import typer
 from pydash import pascal_case, snake_case
```

### Comparing `guardrails_ai-0.4.3/guardrails/cli/hub/install.py` & `guardrails_ai-0.4.4/guardrails/cli/hub/install.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,27 @@
-import json
+from contextlib import contextmanager
 import os
 import subprocess
 import sys
-from email.parser import BytesHeaderParser
 from string import Template
-from typing import List, Literal, Union
+from typing import List, Literal
 
 import typer
-from pydash.strings import snake_case
 
 from guardrails.classes.generic import Stack
 from guardrails.cli.hub.hub import hub_command
 from guardrails.cli.logger import LEVELS, logger
 from guardrails.cli.server.hub_client import get_validator_manifest
 from guardrails.cli.server.module_manifest import ModuleManifest
 
+from guardrails.cli.hub.utils import pip_process
+from guardrails.cli.hub.utils import get_site_packages_location
+from guardrails.cli.hub.utils import get_org_and_package_dirs
+from guardrails.cli.hub.utils import get_hub_directory
+
 from .console import console
 
 
 def removesuffix(string: str, suffix: str) -> str:
     if sys.version_info.minor >= 9:
         return string.removesuffix(suffix)  # type: ignore
     else:
@@ -27,77 +30,14 @@
         return string
 
 
 string_format: Literal["string"] = "string"
 json_format: Literal["json"] = "json"
 
 
-def pip_process(
-    action: str,
-    package: str = "",
-    flags: List[str] = [],
-    format: Union[Literal["string"], Literal["json"]] = string_format,
-) -> Union[str, dict]:
-    try:
-        logger.debug(f"running pip {action} {' '.join(flags)} {package}")
-        command = [sys.executable, "-m", "pip", action]
-        command.extend(flags)
-        if package:
-            command.append(package)
-        output = subprocess.check_output(command)
-        logger.debug(f"decoding output from pip {action} {package}")
-        if format == json_format:
-            parsed = BytesHeaderParser().parsebytes(output)
-            try:
-                return json.loads(str(parsed))
-            except Exception:
-                logger.debug(
-                    f"json parse exception in decoding output from pip {action} {package}. Falling back to accumulating the byte stream",  # noqa
-                )
-            accumulator = {}
-            for key, value in parsed.items():
-                accumulator[key] = value
-            return accumulator
-        return str(output.decode())
-    except subprocess.CalledProcessError as exc:
-        logger.error(
-            (
-                f"Failed to {action} {package}\n"
-                f"Exit code: {exc.returncode}\n"
-                f"stdout: {exc.output}"
-            )
-        )
-        sys.exit(1)
-    except Exception as e:
-        logger.error(
-            f"An unexpected exception occurred while try to {action} {package}!",
-            e,
-        )
-        sys.exit(1)
-
-
-def get_site_packages_location():
-    output = pip_process("show", "pip", format=json_format)
-    pip_location = output["Location"]  # type: ignore
-    return pip_location
-
-
-def get_org_and_package_dirs(manifest: ModuleManifest) -> List[str]:
-    org_name = manifest.namespace
-    package_name = manifest.package_name
-    org = snake_case(org_name if len(org_name) > 1 else "")
-    package = snake_case(package_name if len(package_name) > 1 else package_name)
-    return list(filter(None, [org, package]))
-
-
-def get_hub_directory(manifest: ModuleManifest, site_packages: str) -> str:
-    org_package = get_org_and_package_dirs(manifest)
-    return os.path.join(site_packages, "guardrails", "hub", *org_package)
-
-
 # NOTE: I don't like this but don't see another way without
 #  shimming the init file with all hub validators
 def add_to_hub_inits(manifest: ModuleManifest, site_packages: str):
     org_package = get_org_and_package_dirs(manifest)
     exports: List[str] = manifest.exports or []
     sorted_exports = sorted(exports, reverse=True)
     module_name = manifest.module_name
@@ -191,27 +131,35 @@
 
     if branch is not None:
         git_url = f"{git_url}@{branch}"
 
     return git_url
 
 
-def install_hub_module(module_manifest: ModuleManifest, site_packages: str):
+def install_hub_module(
+    module_manifest: ModuleManifest, site_packages: str, quiet: bool = False
+):
     install_url = get_install_url(module_manifest)
     install_directory = get_hub_directory(module_manifest, site_packages)
 
+    pip_flags = [f"--target={install_directory}", "--no-deps"]
+    if quiet:
+        pip_flags.append("-q")
+
     # Install validator module in namespaced directory under guardrails.hub
-    download_output = pip_process(
-        "install", install_url, [f"--target={install_directory}", "--no-deps", "-q"]
-    )
-    logger.info(download_output)
+    download_output = pip_process("install", install_url, pip_flags, quiet=quiet)
+    if not quiet:
+        logger.info(download_output)
 
     # Install validator module's dependencies in normal site-packages directory
     inspect_output = pip_process(
-        "inspect", flags=[f"--path={install_directory}"], format=json_format
+        "inspect",
+        flags=[f"--path={install_directory}"],
+        format=json_format,
+        quiet=quiet,
     )
 
     # throw if inspect_output is a string. Mostly for pyright
     if isinstance(inspect_output, str):
         logger.error("Failed to inspect the installed package!")
         sys.exit(1)
 
@@ -224,74 +172,93 @@
     requirements = filter(lambda dep: "extra" not in dep, dependencies)
     for req in requirements:
         req_info = Stack(*req.split(" "))
         name = req_info.at(0, "").strip()  # type: ignore
         versions = req_info.at(1, "").strip("()")  # type: ignore
         if name:
             install_spec = name if not versions else f"{name}{versions}"
-            dep_install_output = pip_process("install", install_spec)
-            logger.info(dep_install_output)
+            dep_install_output = pip_process("install", install_spec, quiet=quiet)
+            if not quiet:
+                logger.info(dep_install_output)
 
 
 @hub_command.command()
 def install(
     package_uri: str = typer.Argument(
-        help="URI to the package to install. Example: hub://guardrails/regex_match."
+        help="URI to the package to install.\
+Example: hub://guardrails/regex_match."
+    ),
+    quiet: bool = typer.Option(
+        False,
+        "--quiet",
+        help="Run the command in quiet mode to reduce output verbosity.",
     ),
 ):
+    verbose_printer = console.print
+    quiet_printer = console.print if not quiet else lambda x: None
     """Install a validator from the Hub."""
     if not package_uri.startswith("hub://"):
         logger.error("Invalid URI!")
         sys.exit(1)
 
-    console.print(f"\nInstalling {package_uri}...\n")
+    installing_msg = f"Installing {package_uri}..."
     logger.log(
-        level=LEVELS.get("SPAM"), msg=f"Installing {package_uri}..."  # type: ignore
+        level=LEVELS.get("SPAM"),  # type: ignore
+        msg=installing_msg,
     )
+    verbose_printer(installing_msg)
 
     # Validation
     module_name = package_uri.replace("hub://", "")
 
+    @contextmanager
+    def do_nothing_context(*args, **kwargs):
+        try:
+            yield
+        finally:
+            pass
+
+    loader = console.status if not quiet else do_nothing_context
+
     # Prep
-    with console.status("Fetching manifest", spinner="bouncingBar"):
+    fetch_manifest_msg = "Fetching manifest"
+    with loader(fetch_manifest_msg, spinner="bouncingBar"):
         module_manifest = get_validator_manifest(module_name)
         site_packages = get_site_packages_location()
 
     # Install
-    with console.status("Downloading dependencies", spinner="bouncingBar"):
-        install_hub_module(module_manifest, site_packages)
+    dl_deps_msg = "Downloading dependencies"
+    with loader(dl_deps_msg, spinner="bouncingBar"):
+        install_hub_module(module_manifest, site_packages, quiet=quiet)
 
     # Post-install
-    with console.status("Running post-install setup", spinner="bouncingBar"):
+    post_msg = "Running post-install setup"
+    with loader(post_msg, spinner="bouncingBar"):
         run_post_install(module_manifest, site_packages)
         add_to_hub_inits(module_manifest, site_packages)
 
-    success_message_cli = Template(
-        """✅Successfully installed ${module_name}!
-
-[bold]Import validator:[/bold]
-from guardrails.hub import ${export}
+    logger.info("Installation complete")
 
-[bold]Get more info:[/bold]
-https://hub.guardrailsai.com/validator/${id}
-"""
+    verbose_printer(f"✅Successfully installed {module_name}!\n\n")
+    success_message_cli = Template(
+        "[bold]Import validator:[/bold]\n"
+        "from guardrails.hub import ${export}\n\n"
+        "[bold]Get more info:[/bold]\n"
+        "https://hub.guardrailsai.com/validator/${id}\n"
     ).safe_substitute(
         module_name=package_uri,
         id=module_manifest.id,
         export=module_manifest.exports[0],
     )
     success_message_logger = Template(
-        """✅Successfully installed ${module_name}!
-
-Import validator:
-from guardrails.hub import ${export}
-
-Get more info:
-https://hub.guardrailsai.com/validator/${id}
-"""
+        "✅Successfully installed ${module_name}!\n\n"
+        "Import validator:\n"
+        "from guardrails.hub import ${export}\n\n"
+        "Get more info:\n"
+        "https://hub.guardrailsai.com/validator/${id}\n"
     ).safe_substitute(
         module_name=package_uri,
         id=module_manifest.id,
         export=module_manifest.exports[0],
     )
-    console.print(success_message_cli)  # type: ignore
+    quiet_printer(success_message_cli)  # type: ignore
     logger.log(level=LEVELS.get("SPAM"), msg=success_message_logger)  # type: ignore
```

### Comparing `guardrails_ai-0.4.3/guardrails/cli/hub/submit.py` & `guardrails_ai-0.4.4/guardrails/cli/hub/submit.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/cli/server/auth.py` & `guardrails_ai-0.4.4/guardrails/cli/server/auth.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/cli/server/hub_client.py` & `guardrails_ai-0.4.4/guardrails/cli/server/hub_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,31 +6,41 @@
 from jwt import JWT
 from jwt.exceptions import JWTDecodeError
 
 from guardrails.classes.credentials import Credentials
 from guardrails.cli.logger import logger
 from guardrails.cli.server.module_manifest import ModuleManifest
 
-TOKEN_EXPIRED_MESSAGE = (
-    "Your token has expired. Please run `guardrails configure` to update your token."
-)
-TOKEN_INVALID_MESSAGE = (
-    "Your token is invalid. Please run `guardrails configure` to update your token."
-)
+FIND_NEW_TOKEN = "You can find a new token at https://hub.guardrailsai.com/tokens"
+
+TOKEN_EXPIRED_MESSAGE = f"""Your token has expired. Please run `guardrails configure`\
+to update your token.
+{FIND_NEW_TOKEN}"""
+TOKEN_INVALID_MESSAGE = f"""Your token is invalid. Please run `guardrails configure`\
+to update your token.
+{FIND_NEW_TOKEN}"""
 
 validator_hub_service = "https://so4sg4q4pb.execute-api.us-east-1.amazonaws.com"
 validator_manifest_endpoint = Template(
     "validator-manifests/${namespace}/${validator_name}"
 )
 
 
 class AuthenticationError(Exception):
     pass
 
 
+class ExpiredTokenError(Exception):
+    pass
+
+
+class InvalidTokenError(Exception):
+    pass
+
+
 class HttpError(Exception):
     status: int
     message: str
 
 
 def fetch(url: str, token: Optional[str], anonymousUserId: Optional[str]):
     try:
@@ -76,17 +86,17 @@
     # check for jwt expiration
     if token:
         try:
             JWT().decode(token, do_verify=False)
         except JWTDecodeError as e:
             # if the error message includes "Expired", then the token is expired
             if "Expired" in str(e):
-                raise Exception(TOKEN_EXPIRED_MESSAGE)
+                raise ExpiredTokenError(TOKEN_EXPIRED_MESSAGE)
             else:
-                raise Exception(TOKEN_INVALID_MESSAGE)
+                raise InvalidTokenError(TOKEN_INVALID_MESSAGE)
     return token
 
 
 def fetch_module(module_name: str) -> ModuleManifest:
     creds = Credentials.from_rc_file(logger)
     token = get_jwt_token(creds)
 
@@ -101,14 +111,17 @@
         if not module_manifest:
             logger.error(f"Failed to install hub://{module_name}")
             sys.exit(1)
         return module_manifest
     except HttpError:
         logger.error(f"Failed to install hub://{module_name}")
         sys.exit(1)
+    except (ExpiredTokenError, InvalidTokenError) as e:
+        logger.error(AuthenticationError(e))
+        sys.exit(1)
     except Exception as e:
         logger.error("An unexpected error occurred!", e)
         sys.exit(1)
 
 
 # GET /auth
 def get_auth():
@@ -118,14 +131,16 @@
         auth_url = f"{validator_hub_service}/auth"
         response = fetch(auth_url, token, creds.id)
         if not response:
             raise AuthenticationError("Failed to authenticate!")
     except HttpError as http_error:
         logger.error(http_error)
         raise AuthenticationError("Failed to authenticate!")
+    except (ExpiredTokenError, InvalidTokenError) as e:
+        raise AuthenticationError(e)
     except Exception as e:
         logger.error("An unexpected error occurred!", e)
         raise AuthenticationError("Failed to authenticate!")
 
 
 def post_validator_submit(package_name: str, content: str):
     try:
```

### Comparing `guardrails_ai-0.4.3/guardrails/cli/server/module_manifest.py` & `guardrails_ai-0.4.4/guardrails/cli/server/module_manifest.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/cli/validate.py` & `guardrails_ai-0.4.4/guardrails/cli/validate.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/constants.xml` & `guardrails_ai-0.4.4/guardrails/constants.xml`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/datatypes.py` & `guardrails_ai-0.4.4/guardrails/datatypes.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/document_store.py` & `guardrails_ai-0.4.4/guardrails/document_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,16 +48,15 @@
 class DocumentStoreBase(ABC):
     """Abstract class for a store that can store text, and metadata from
     documents.
 
     The store can be queried by text for similar documents.
     """
 
-    def __init__(self, vector_db: VectorDBBase, path: Optional[str] = None):
-        ...
+    def __init__(self, vector_db: VectorDBBase, path: Optional[str] = None): ...
 
     @abstractmethod
     def add_document(self, document: Document) -> None:
         """Adds a document to the store.
 
         Args:
             document: Document object to be added
@@ -178,17 +177,15 @@
 
     Base = declarative_base()
 
     class RealSqlDocument(Base):
         __tablename__ = "documents"
 
         id: Mapped[int] = mapped_column(primary_key=True)  # type: ignore
-        page_num: Mapped[int] = mapped_column(
-            sqlalchemy.Integer, primary_key=True
-        )  # type: ignore
+        page_num: Mapped[int] = mapped_column(sqlalchemy.Integer, primary_key=True)  # type: ignore
         text: Mapped[str] = mapped_column(sqlalchemy.String)  # type: ignore
         meta: Mapped[dict] = mapped_column(sqlalchemy.PickleType)  # type: ignore
         vector_index: Mapped[int] = mapped_column(sqlalchemy.Integer)  # type: ignore
 
     class RealSQLMetadataStore:
         def __init__(self, path: Optional[str] = None):
             conn = f"sqlite:///{path}" if path is not None else "sqlite://"
```

### Comparing `guardrails_ai-0.4.3/guardrails/embedding.py` & `guardrails_ai-0.4.4/guardrails/embedding.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/errors/__init__.py` & `guardrails_ai-0.4.4/guardrails/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/guard.py` & `guardrails_ai-0.4.4/guardrails/guard.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,28 +18,28 @@
     Tuple,
     Type,
     Union,
     cast,
     overload,
 )
 
-from guardrails_api_client.models import AnyObject
-from guardrails_api_client.models import Guard as GuardModel
 from guardrails_api_client.models import (
+    AnyObject,
+    Guard as GuardModel,
     History,
     HistoryEvent,
     ValidatePayload,
     ValidationOutput,
 )
 from guardrails_api_client.types import UNSET
 from langchain_core.messages import BaseMessage
 from langchain_core.runnables import Runnable, RunnableConfig
 from pydantic import BaseModel
 from pydantic.version import VERSION as PYDANTIC_VERSION
-from typing_extensions import deprecated
+from typing_extensions import deprecated  # type: ignore
 
 from guardrails.api_client import GuardrailsApiClient
 from guardrails.classes import OT, InputType, ValidationOutcome
 from guardrails.classes.credentials import Credentials
 from guardrails.classes.generic import Stack
 from guardrails.classes.history import Call
 from guardrails.classes.history.call_inputs import CallInputs
@@ -127,15 +127,15 @@
 
         credentials = Credentials.from_rc_file(logger)
 
         # Get unique id of user from credentials
         self._user_id = credentials.id or ""
 
         # Get metrics opt-out from credentials
-        self._disable_tracer = credentials.no_metrics
+        self._disable_tracer = not credentials.enable_metrics
 
         # Get id of guard object (that is unique)
         self._guard_id = id(self)  # id of guard object; not the class
 
         # Initialize Hub Telemetry singleton and get the tracer
         #  if it is not disabled
         if not self._disable_tracer:
@@ -156,74 +156,124 @@
                         name=self.name
                     )
                 )
             self._api_client = GuardrailsApiClient(api_key=api_key)
             self.upsert_guard()
 
     @property
+    @deprecated(
+        """'Guard.prompt_schema' is deprecated and will be removed in \
+versions 0.5.x and beyond."""
+    )
     def prompt_schema(self) -> Optional[StringSchema]:
         """Return the input schema."""
         return self.rail.prompt_schema
 
     @property
+    @deprecated(
+        """'Guard.instructions_schema' is deprecated and will be removed in \
+versions 0.5.x and beyond."""
+    )
     def instructions_schema(self) -> Optional[StringSchema]:
         """Return the input schema."""
         return self.rail.instructions_schema
 
     @property
+    @deprecated(
+        """'Guard.msg_history_schema' is deprecated and will be removed in \
+versions 0.5.x and beyond."""
+    )
     def msg_history_schema(self) -> Optional[StringSchema]:
         """Return the input schema."""
         return self.rail.msg_history_schema
 
     @property
+    @deprecated(
+        """'Guard.output_schema' is deprecated and will be removed in \
+versions 0.5.x and beyond."""
+    )
     def output_schema(self) -> Schema:
         """Return the output schema."""
         return self.rail.output_schema
 
     @property
+    @deprecated(
+        """'Guard.instructions' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.instructions' instead."""
+    )
     def instructions(self) -> Optional[Instructions]:
         """Return the instruction-prompt."""
         return self.rail.instructions
 
     @property
+    @deprecated(
+        """'Guard.prompt' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.prompt' instead."""
+    )
     def prompt(self) -> Optional[Prompt]:
         """Return the prompt."""
         return self.rail.prompt
 
     @property
+    @deprecated(
+        """'Guard.raw_prompt' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.prompt' instead."""
+    )
     def raw_prompt(self) -> Optional[Prompt]:
         """Return the prompt, alias for `prompt`."""
-        return self.prompt
+        return self.rail.prompt
 
     @property
+    @deprecated(
+        """'Guard.base_prompt' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.prompt' instead."""
+    )
     def base_prompt(self) -> Optional[str]:
         """Return the base prompt i.e. prompt.source."""
-        if self.prompt is None:
+        if self.rail.prompt is None:
             return None
-        return self.prompt.source
+        return self.rail.prompt.source
 
     @property
+    @deprecated(
+        """'Guard.reask_prompt' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.reask_prompts' instead."""
+    )
     def reask_prompt(self) -> Optional[Prompt]:
         """Return the reask prompt."""
-        return self.output_schema.reask_prompt_template
+        return self.rail.output_schema.reask_prompt_template
 
     @reask_prompt.setter
+    @deprecated(
+        """'Guard.reask_prompt' is deprecated and will be removed in \
+versions 0.5.x and beyond. Pass 'reask_prompt' in the initializer \
+    method instead: e.g. 'Guard.from_pydantic'."""
+    )
     def reask_prompt(self, reask_prompt: Optional[str]):
         """Set the reask prompt."""
-        self.output_schema.reask_prompt_template = reask_prompt
+        self.rail.output_schema.reask_prompt_template = reask_prompt
 
     @property
+    @deprecated(
+        """'Guard.reask_instructions' is deprecated and will be removed in \
+versions 0.5.x and beyond. Use 'Guard.history.last.reask_instructions' instead."""
+    )
     def reask_instructions(self) -> Optional[Instructions]:
         """Return the reask prompt."""
-        return self.output_schema.reask_instructions_template
+        return self.rail.output_schema.reask_instructions_template
 
     @reask_instructions.setter
+    @deprecated(
+        """'Guard.reask_instructions' is deprecated and will be removed in \
+versions 0.5.x and beyond. Pass 'reask_instructions' in the initializer \
+    method instead: e.g. 'Guard.from_pydantic'."""
+    )
     def reask_instructions(self, reask_instructions: Optional[str]):
         """Set the reask prompt."""
-        self.output_schema.reask_instructions_template = reask_instructions
+        self.rail.output_schema.reask_instructions_template = reask_instructions
 
     def configure(
         self,
         num_reasks: Optional[int] = None,
     ):
         """Configure the Guard."""
         self.num_reasks = (
@@ -463,32 +513,30 @@
         instructions: Optional[str] = None,
         msg_history: Optional[List[Dict]] = None,
         metadata: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         stream: Optional[bool] = False,
         *args,
         **kwargs,
-    ) -> Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]]:
-        ...
+    ) -> Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]]: ...
 
     @overload
     def __call__(
         self,
         llm_api: Callable[[Any], Awaitable[Any]],
         prompt_params: Optional[Dict] = None,
         num_reasks: Optional[int] = None,
         prompt: Optional[str] = None,
         instructions: Optional[str] = None,
         msg_history: Optional[List[Dict]] = None,
         metadata: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
-    ) -> Awaitable[ValidationOutcome[OT]]:
-        ...
+    ) -> Awaitable[ValidationOutcome[OT]]: ...
 
     def __call__(
         self,
         llm_api: Union[Callable, Callable[[Any], Awaitable[Any]]],
         prompt_params: Optional[Dict] = None,
         num_reasks: Optional[int] = None,
         prompt: Optional[str] = None,
@@ -498,16 +546,15 @@
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
     ) -> Union[
         Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]],
         Awaitable[ValidationOutcome[OT]],
     ]:
-        """Call the LLM and validate the output. Pass an async LLM API to
-        return a coroutine.
+        """Call the LLM and validate the output.
 
         Args:
             llm_api: The LLM API to call
                      (e.g. openai.Completion.create or openai.Completion.acreate)
             prompt_params: The parameters to pass to the prompt.format() method.
             num_reasks: The max times to re-ask the LLM for invalid output.
             prompt: The prompt to use for the LLM.
@@ -532,33 +579,40 @@
             instructions: Optional[str] = None,
             msg_history: Optional[List[Dict]] = None,
             metadata: Optional[Dict] = None,
             full_schema_reask: Optional[bool] = None,
             *args,
             **kwargs,
         ):
+            llm_api_str = (
+                f"{llm_api.__module__}.{llm_api.__name__}" if llm_api else "None"
+            )
             if metadata is None:
                 metadata = {}
             if full_schema_reask is None:
                 full_schema_reask = self.base_model is not None
             if prompt_params is None:
                 prompt_params = {}
 
             if not self._disable_tracer:
                 # Create a new span for this guard call
                 self._hub_telemetry.create_new_span(
                     span_name="/guard_call",
                     attributes=[
                         ("guard_id", self._guard_id),
                         ("user_id", self._user_id),
-                        ("llm_api", llm_api.__name__ if llm_api else "None"),
-                        ("custom_reask_prompt", self.reask_prompt is not None),
+                        ("llm_api", llm_api_str),
+                        (
+                            "custom_reask_prompt",
+                            self.rail.output_schema.reask_prompt_template is not None,
+                        ),
                         (
                             "custom_reask_instructions",
-                            self.reask_instructions is not None,
+                            self.rail.output_schema.reask_instructions_template
+                            is not None,
                         ),
                     ],
                     is_parent=True,  # It will have children
                     has_parent=False,  # Has no parents
                 )
 
             set_call_kwargs(kwargs)
@@ -568,17 +622,19 @@
             self.configure(num_reasks)
             if self.num_reasks is None:
                 raise RuntimeError(
                     "`num_reasks` is `None` after calling `configure()`. "
                     "This should never happen."
                 )
 
-            input_prompt = prompt or (self.prompt._source if self.prompt else None)
+            input_prompt = prompt or (
+                self.rail.prompt._source if self.rail.prompt else None
+            )
             input_instructions = instructions or (
-                self.instructions._source if self.instructions else None
+                self.rail.instructions._source if self.rail.instructions else None
             )
             call_inputs = CallInputs(
                 llm_api=llm_api,
                 prompt=input_prompt,
                 instructions=input_instructions,
                 msg_history=msg_history,
                 prompt_params=prompt_params,
@@ -601,15 +657,16 @@
                     prompt_params=prompt_params,
                     full_schema_reask=full_schema_reask,
                     call_log=call_log,
                     *args,
                     **kwargs,
                 )
 
-            # If the LLM API is async, return a coroutine
+            # If the LLM API is async, return a coroutine. This will be deprecated soon.
+
             if asyncio.iscoroutinefunction(llm_api):
                 return self._call_async(
                     llm_api,
                     prompt_params=prompt_params,
                     num_reasks=self.num_reasks,
                     prompt=prompt,
                     instructions=instructions,
@@ -661,16 +718,16 @@
         msg_history: Optional[List[Dict]],
         metadata: Dict,
         full_schema_reask: bool,
         call_log: Call,
         *args,
         **kwargs,
     ) -> Union[ValidationOutcome[OT], Iterable[ValidationOutcome[OT]]]:
-        instructions_obj = instructions or self.instructions
-        prompt_obj = prompt or self.prompt
+        instructions_obj = instructions or self.rail.instructions
+        prompt_obj = prompt or self.rail.prompt
         msg_history_obj = msg_history or []
         if prompt_obj is None:
             if msg_history is not None and not len(msg_history_obj):
                 raise RuntimeError(
                     "You must provide a prompt if msg_history is empty. "
                     "Alternatively, you can provide a prompt in the Schema constructor."
                 )
@@ -679,45 +736,51 @@
         if kwargs.get("stream", False):
             # If stream is True, use StreamRunner
             runner = StreamRunner(
                 instructions=instructions_obj,
                 prompt=prompt_obj,
                 msg_history=msg_history_obj,
                 api=get_llm_ask(llm_api, *args, **kwargs),
-                prompt_schema=self.prompt_schema,
-                instructions_schema=self.instructions_schema,
-                msg_history_schema=self.msg_history_schema,
-                output_schema=self.output_schema,
+                prompt_schema=self.rail.prompt_schema,
+                instructions_schema=self.rail.instructions_schema,
+                msg_history_schema=self.rail.msg_history_schema,
+                output_schema=self.rail.output_schema,
                 num_reasks=num_reasks,
                 metadata=metadata,
                 base_model=self.base_model,
                 full_schema_reask=full_schema_reask,
                 disable_tracer=self._disable_tracer,
             )
             return runner(call_log=call_log, prompt_params=prompt_params)
         else:
             # Otherwise, use Runner
             runner = Runner(
                 instructions=instructions_obj,
                 prompt=prompt_obj,
                 msg_history=msg_history_obj,
                 api=get_llm_ask(llm_api, *args, **kwargs),
-                prompt_schema=self.prompt_schema,
-                instructions_schema=self.instructions_schema,
-                msg_history_schema=self.msg_history_schema,
-                output_schema=self.output_schema,
+                prompt_schema=self.rail.prompt_schema,
+                instructions_schema=self.rail.instructions_schema,
+                msg_history_schema=self.rail.msg_history_schema,
+                output_schema=self.rail.output_schema,
                 num_reasks=num_reasks,
                 metadata=metadata,
                 base_model=self.base_model,
                 full_schema_reask=full_schema_reask,
                 disable_tracer=self._disable_tracer,
             )
             call = runner(call_log=call_log, prompt_params=prompt_params)
             return ValidationOutcome[OT].from_guard_history(call)
 
+    @deprecated(
+        """Async methods within Guard are deprecated and will be removed in 0.5.x.
+        Instead, please use `AsyncGuard() or pass in a synchronous llm api.""",
+        category=FutureWarning,
+        stacklevel=2,
+    )
     async def _call_async(
         self,
         llm_api: Callable[[Any], Awaitable[Any]],
         prompt_params: Dict,
         num_reasks: int,
         prompt: Optional[str],
         instructions: Optional[str],
@@ -742,33 +805,33 @@
                                or just the incorrect values.
                                Defaults to `True` if a base model is provided,
                                `False` otherwise.
 
         Returns:
             The raw text output from the LLM and the validated output.
         """
-        instructions_obj = instructions or self.instructions
-        prompt_obj = prompt or self.prompt
+        instructions_obj = instructions or self.rail.instructions
+        prompt_obj = prompt or self.rail.prompt
         msg_history_obj = msg_history or []
         if prompt_obj is None:
             if msg_history_obj is not None and not len(msg_history_obj):
                 raise RuntimeError(
                     "You must provide a prompt if msg_history is empty. "
                     "Alternatively, you can provide a prompt in the RAIL spec."
                 )
 
         runner = AsyncRunner(
             instructions=instructions_obj,
             prompt=prompt_obj,
             msg_history=msg_history_obj,
             api=get_async_llm_ask(llm_api, *args, **kwargs),
-            prompt_schema=self.prompt_schema,
-            instructions_schema=self.instructions_schema,
-            msg_history_schema=self.msg_history_schema,
-            output_schema=self.output_schema,
+            prompt_schema=self.rail.prompt_schema,
+            instructions_schema=self.rail.instructions_schema,
+            msg_history_schema=self.rail.msg_history_schema,
+            output_schema=self.rail.output_schema,
             num_reasks=num_reasks,
             metadata=metadata,
             base_model=self.base_model,
             full_schema_reask=full_schema_reask,
             disable_tracer=self._disable_tracer,
         )
         call = await runner.async_run(call_log=call_log, prompt_params=prompt_params)
@@ -807,44 +870,41 @@
         metadata: Optional[Dict] = None,
         llm_api: None = None,
         num_reasks: Optional[int] = None,
         prompt_params: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
-    ) -> ValidationOutcome[OT]:
-        ...
+    ) -> ValidationOutcome[OT]: ...
 
     @overload
     def parse(
         self,
         llm_output: str,
         metadata: Optional[Dict] = None,
         llm_api: Callable[[Any], Awaitable[Any]] = ...,
         num_reasks: Optional[int] = None,
         prompt_params: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
-    ) -> Awaitable[ValidationOutcome[OT]]:
-        ...
+    ) -> Awaitable[ValidationOutcome[OT]]: ...
 
     @overload
     def parse(
         self,
         llm_output: str,
         metadata: Optional[Dict] = None,
         llm_api: Optional[Callable] = None,
         num_reasks: Optional[int] = None,
         prompt_params: Optional[Dict] = None,
         full_schema_reask: Optional[bool] = None,
         *args,
         **kwargs,
-    ) -> ValidationOutcome[OT]:
-        ...
+    ) -> ValidationOutcome[OT]: ...
 
     def parse(
         self,
         llm_output: str,
         metadata: Optional[Dict] = None,
         llm_api: Optional[Callable] = None,
         num_reasks: Optional[int] = None,
@@ -877,29 +937,36 @@
             llm_api: Optional[Callable] = None,
             num_reasks: Optional[int] = None,
             prompt_params: Optional[Dict] = None,
             full_schema_reask: Optional[bool] = None,
             *args,
             **kwargs,
         ):
+            llm_api_str = (
+                f"{llm_api.__module__}.{llm_api.__name__}" if llm_api else "None"
+            )
             final_num_reasks = (
                 num_reasks if num_reasks is not None else 0 if llm_api is None else None
             )
 
             if not self._disable_tracer:
                 self._hub_telemetry.create_new_span(
                     span_name="/guard_parse",
                     attributes=[
                         ("guard_id", self._guard_id),
                         ("user_id", self._user_id),
-                        ("llm_api", llm_api.__name__ if llm_api else "None"),
-                        ("custom_reask_prompt", self.reask_prompt is not None),
+                        ("llm_api", llm_api_str),
+                        (
+                            "custom_reask_prompt",
+                            self.rail.output_schema.reask_prompt_template is not None,
+                        ),
                         (
                             "custom_reask_instructions",
-                            self.reask_instructions is not None,
+                            self.rail.output_schema.reask_instructions_template
+                            is not None,
                         ),
                     ],
                     is_parent=True,  # It will have children
                     has_parent=False,  # Has no parents
                 )
 
             self.configure(final_num_reasks)
@@ -913,17 +980,17 @@
             metadata = metadata or {}
             prompt_params = prompt_params or {}
 
             set_call_kwargs(kwargs)
             set_tracer(self._tracer)
             set_tracer_context(self._tracer_context)
 
-            input_prompt = self.prompt._source if self.prompt else None
+            input_prompt = self.rail.prompt._source if self.rail.prompt else None
             input_instructions = (
-                self.instructions._source if self.instructions else None
+                self.rail.instructions._source if self.rail.instructions else None
             )
             call_inputs = CallInputs(
                 llm_api=llm_api,
                 llm_output=llm_output,
                 prompt=input_prompt,
                 instructions=input_instructions,
                 prompt_params=prompt_params,
@@ -1014,29 +1081,35 @@
             The validated response.
         """
         runner = Runner(
             instructions=kwargs.pop("instructions", None),
             prompt=kwargs.pop("prompt", None),
             msg_history=kwargs.pop("msg_history", None),
             api=get_llm_ask(llm_api, *args, **kwargs) if llm_api else None,
-            prompt_schema=self.prompt_schema,
-            instructions_schema=self.instructions_schema,
-            msg_history_schema=self.msg_history_schema,
-            output_schema=self.output_schema,
+            prompt_schema=self.rail.prompt_schema,
+            instructions_schema=self.rail.instructions_schema,
+            msg_history_schema=self.rail.msg_history_schema,
+            output_schema=self.rail.output_schema,
             num_reasks=num_reasks,
             metadata=metadata,
             output=llm_output,
             base_model=self.base_model,
             full_schema_reask=full_schema_reask,
             disable_tracer=self._disable_tracer,
         )
         call = runner(call_log=call_log, prompt_params=prompt_params)
 
         return ValidationOutcome[OT].from_guard_history(call)
 
+    @deprecated(
+        """Async methods within Guard are deprecated and will be removed in 0.5.x.
+        Instead, please use `AsyncGuard() or pass in a synchronous llm api.""",
+        category=FutureWarning,
+        stacklevel=2,
+    )
     async def _async_parse(
         self,
         llm_output: str,
         metadata: Dict,
         llm_api: Optional[Callable[[Any], Awaitable[Any]]],
         num_reasks: int,
         prompt_params: Dict,
@@ -1056,18 +1129,18 @@
             The validated response.
         """
         runner = AsyncRunner(
             instructions=kwargs.pop("instructions", None),
             prompt=kwargs.pop("prompt", None),
             msg_history=kwargs.pop("msg_history", None),
             api=get_async_llm_ask(llm_api, *args, **kwargs) if llm_api else None,
-            prompt_schema=self.prompt_schema,
-            instructions_schema=self.instructions_schema,
-            msg_history_schema=self.msg_history_schema,
-            output_schema=self.output_schema,
+            prompt_schema=self.rail.prompt_schema,
+            instructions_schema=self.rail.instructions_schema,
+            msg_history_schema=self.rail.msg_history_schema,
+            output_schema=self.rail.output_schema,
             num_reasks=num_reasks,
             metadata=metadata,
             output=llm_output,
             base_model=self.base_model,
             full_schema_reask=full_schema_reask,
             disable_tracer=self._disable_tracer,
         )
@@ -1190,22 +1263,20 @@
         else:
             raise ValueError(
                 """Invalid value for `on`. Must be one of the following:
                 'output', 'prompt', 'instructions', 'msg_history'."""
             )
 
     @overload
-    def use(self, validator: Validator, *, on: str = "output") -> "Guard":
-        ...
+    def use(self, validator: Validator, *, on: str = "output") -> "Guard": ...
 
     @overload
     def use(
         self, validator: Type[Validator], *args, on: str = "output", **kwargs
-    ) -> "Guard":
-        ...
+    ) -> "Guard": ...
 
     def use(
         self,
         validator: Union[Validator, Type[Validator]],
         *args,
         on: str = "output",
         **kwargs,
@@ -1223,28 +1294,26 @@
             on: The part of the LLM request to validate. Defaults to "output".
         """
         hydrated_validator = get_validator(validator, *args, **kwargs)
         self.__add_validator(hydrated_validator, on=on)
         return self
 
     @overload
-    def use_many(self, *validators: Validator, on: str = "output") -> "Guard":
-        ...
+    def use_many(self, *validators: Validator, on: str = "output") -> "Guard": ...
 
     @overload
     def use_many(
         self,
         *validators: Tuple[
             Type[Validator],
             Optional[Union[List[Any], Dict[str, Any]]],
             Optional[Dict[str, Any]],
         ],
         on: str = "output",
-    ) -> "Guard":
-        ...
+    ) -> "Guard": ...
 
     def use_many(
         self,
         *validators: Union[
             Validator,
             Tuple[
                 Type[Validator],
@@ -1272,19 +1341,25 @@
     def validate(self, llm_output: str, *args, **kwargs) -> ValidationOutcome[str]:
         if (
             not self.rail
             or self.rail.output_schema.root_datatype.validators != self._validators
         ):
             self.rail = Rail.from_string_validators(
                 validators=self._validators,
-                prompt=self.prompt.source if self.prompt else None,
-                instructions=self.instructions.source if self.instructions else None,
-                reask_prompt=self.reask_prompt.source if self.reask_prompt else None,
-                reask_instructions=self.reask_instructions.source
-                if self.reask_instructions
+                prompt=self.rail.prompt.source if self.rail.prompt else None,
+                instructions=(
+                    self.rail.instructions.source if self.rail.instructions else None
+                ),
+                reask_prompt=(
+                    self.rail.output_schema.reask_prompt_template.source
+                    if self.rail.output_schema.reask_prompt_template
+                    else None
+                ),
+                reask_instructions=self.rail.output_schema.reask_instructions_template.source
+                if self.rail.output_schema.reask_instructions_template
                 else None,
             )
 
         return self.parse(llm_output=llm_output, *args, **kwargs)
 
     # No call support for this until
     # https://github.com/guardrails-ai/guardrails/pull/525 is merged
```

### Comparing `guardrails_ai-0.4.3/guardrails/llm_providers.py` & `guardrails_ai-0.4.4/guardrails/llm_providers.py`

 * *Files 0% similar despite different names*

```diff
@@ -942,15 +942,15 @@
     return issubclass(type(model), OpenAIModel) or issubclass(
         type(model), AsyncOpenAIModel
     )
 
 
 # FIXME: Update with newly supported LLMs
 def get_llm_api_enum(
-    llm_api: Callable[[Any], Awaitable[Any]]
+    llm_api: Callable[[Any], Awaitable[Any]],
 ) -> Optional[ValidatePayloadLlmApi]:
     # TODO: Distinguish between v1 and v2
     if llm_api == get_static_openai_create_func():
         return ValidatePayloadLlmApi.OPENAI_COMPLETION_CREATE
     elif llm_api == get_static_openai_chat_create_func():
         return ValidatePayloadLlmApi.OPENAI_CHATCOMPLETION_CREATE
     elif llm_api == get_static_openai_acreate_func():
```

### Comparing `guardrails_ai-0.4.3/guardrails/logger.py` & `guardrails_ai-0.4.4/guardrails/logger.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/prompt/base_prompt.py` & `guardrails_ai-0.4.4/guardrails/prompt/base_prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for representing a prompt entry."""
+
 import re
 from string import Template
 from typing import Optional
 
 import regex
 
 from guardrails.namespace_template import NamespaceTemplate
```

### Comparing `guardrails_ai-0.4.3/guardrails/prompt/instructions.py` & `guardrails_ai-0.4.4/guardrails/prompt/instructions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Instructions to the LLM, to be passed in the prompt."""
+
 from string import Template
 
 from guardrails.utils.parsing_utils import get_template_variables
 
 from .base_prompt import BasePrompt
```

### Comparing `guardrails_ai-0.4.3/guardrails/prompt/prompt.py` & `guardrails_ai-0.4.4/guardrails/prompt/prompt.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """The LLM prompt."""
+
 from string import Template
 
 from guardrails.utils.parsing_utils import get_template_variables
 
 from .base_prompt import BasePrompt
```

### Comparing `guardrails_ai-0.4.3/guardrails/rail.py` & `guardrails_ai-0.4.4/guardrails/rail.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Rail class."""
+
 import warnings
 from dataclasses import dataclass
 from typing import Any, Dict, List, Optional, Sequence, Type, Union
 
 from lxml import etree as ET
 from pydantic import BaseModel
```

### Comparing `guardrails_ai-0.4.3/guardrails/run/async_runner.py` & `guardrails_ai-0.4.4/guardrails/run/async_runner.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/run/runner.py` & `guardrails_ai-0.4.4/guardrails/run/runner.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/run/stream_runner.py` & `guardrails_ai-0.4.4/guardrails/run/stream_runner.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/schema/json_schema.py` & `guardrails_ai-0.4.4/guardrails/schema/json_schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/schema/schema.py` & `guardrails_ai-0.4.4/guardrails/schema/schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/schema/string_schema.py` & `guardrails_ai-0.4.4/guardrails/schema/string_schema.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/stores/context.py` & `guardrails_ai-0.4.4/guardrails/stores/context.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/constants.py` & `guardrails_ai-0.4.4/guardrails/utils/constants.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/docs_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/docs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/hub_telemetry_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/hub_telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/json_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/json_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,15 +247,15 @@
             prune_extra_keys=prune_extra_keys,
             coerce_types=coerce_types,
             validate_subschema=validate_subschema,
         )
 
 
 def generate_type_skeleton_from_schema(
-    schema: Union[Object, ListDataType]
+    schema: Union[Object, ListDataType],
 ) -> Placeholder:
     """Generate a JSON skeleton from an XML schema."""
 
     def _recurse_schema(schema: DataType):
         if isinstance(schema, Object):
             return DictPlaceholder(
                 children={
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/logs_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/logs_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/misc.py` & `guardrails_ai-0.4.4/guardrails/utils/misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
         # Save the validated response.
         validated_output = logs.guarded_output
         with open(
             os.path.join(artifact_dir, f"validated_response_{on_fail_type}{ext}.py"),
             "w",
         ) as f:
-            f.write("# flake8: noqa: E501\n")
+            f.write("# ruff: noqa: E501\n")
 
             reasks, _ = gather_reasks(validated_output)
             if len(reasks):
                 f.write("from guardrails.utils.reask_utils import ReAsk\n")
 
             validated_output_repr = pretty_repr(validated_output, max_string=None)
             f.write(f"\nVALIDATED_OUTPUT = {validated_output_repr}")
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/openai_utils/__init__.py` & `guardrails_ai-0.4.4/guardrails/utils/openai_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/openai_utils/base.py` & `guardrails_ai-0.4.4/guardrails/utils/openai_utils/base.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/openai_utils/streaming_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/openai_utils/streaming_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/openai_utils/v0.py` & `guardrails_ai-0.4.4/guardrails/utils/openai_utils/v0.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/openai_utils/v1.py` & `guardrails_ai-0.4.4/guardrails/utils/openai_utils/v1.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/parsing_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/parsing_utils.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/__init__.py` & `guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v1.py` & `guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/v1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Utilities for working with Pydantic models."""
+
 import typing
 import warnings
 from copy import deepcopy
 from datetime import date, time
 from enum import Enum
 from typing import (
     Any,
@@ -109,15 +110,17 @@
 
     if isinstance(type_annotation, ModelField):
         type_annotation = type_annotation.annotation
 
     # Strip a Union type annotation to the first non-None type
     if get_origin(type_annotation) == Union:
         non_none_type_annotation = [
-            t for t in get_args(type_annotation) if t != type(None)  # noqa E721
+            t
+            for t in get_args(type_annotation)
+            if t != type(None)  # noqa E721
         ]
         if len(non_none_type_annotation) == 1:
             return non_none_type_annotation[0]
         return type_annotation
 
     return type_annotation
 
@@ -307,15 +310,15 @@
     #     value_type = find_models_in_type(value)
     #     root_model.__annotations__[key] = value_type
 
     return copy
 
 
 def convert_pydantic_model_to_openai_fn(
-    model: Union[Type[BaseModel], Type[List[Type[BaseModel]]]]
+    model: Union[Type[BaseModel], Type[List[Type[BaseModel]]]],
 ) -> Dict:
     """Convert a Pydantic BaseModel to an OpenAI function.
 
     Args:
         model: The Pydantic BaseModel to convert.
 
     Returns:
@@ -455,22 +458,22 @@
             discriminator = field.discriminator_key or "discriminator"
             choice_children = {}
             for case in typing.get_args(field.type_):
                 case_discriminator_type = case.__fields__[discriminator].type_
                 assert typing.get_origin(case_discriminator_type) is typing.Literal
                 assert len(typing.get_args(case_discriminator_type)) == 1
                 discriminator_value = typing.get_args(case_discriminator_type)[0]
-                choice_children[
-                    discriminator_value
-                ] = convert_pydantic_model_to_datatype(
-                    case,
-                    datatype=CaseDataType,
-                    name=discriminator_value,
-                    strict=strict,
-                    excluded_fields=[discriminator],
+                choice_children[discriminator_value] = (
+                    convert_pydantic_model_to_datatype(
+                        case,
+                        datatype=CaseDataType,
+                        name=discriminator_value,
+                        strict=strict,
+                        excluded_fields=[discriminator],
+                    )
                 )
             children[field_name] = pydantic_field_to_datatype(
                 Choice,
                 field,
                 children=choice_children,
                 strict=strict,
                 discriminator_key=discriminator,
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/pydantic_utils/v2.py` & `guardrails_ai-0.4.4/guardrails/utils/pydantic_utils/v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
             return True
     except TypeError:
         pass
     return False
 
 
 def convert_pydantic_model_to_openai_fn(
-    model: Union[Type[BaseModel], Type[List[Type[BaseModel]]]]
+    model: Union[Type[BaseModel], Type[List[Type[BaseModel]]]],
 ) -> Dict:
     """Convert a Pydantic BaseModel to an OpenAI function.
 
     Args:
         model: The Pydantic BaseModel to convert.
 
     Returns:
@@ -294,15 +294,17 @@
 
     if isinstance(type_annotation, FieldInfo):
         type_annotation = type_annotation.annotation
 
     # Strip a Union type annotation to the first non-None type
     if typing.get_origin(type_annotation) == Union:
         non_none_type_annotation = [
-            t for t in get_args(type_annotation) if t != type(None)  # noqa E721
+            t
+            for t in get_args(type_annotation)
+            if t != type(None)  # noqa E721
         ]
         if len(non_none_type_annotation) == 1:
             return non_none_type_annotation[0]
         return type_annotation
 
     return type_annotation
 
@@ -420,22 +422,22 @@
 
             choice_children = {}
             for case in typing.get_args(field.annotation):
                 case_discriminator_type = case.model_fields[discriminator].annotation
                 assert typing.get_origin(case_discriminator_type) is typing.Literal
                 assert len(typing.get_args(case_discriminator_type)) == 1
                 discriminator_value = typing.get_args(case_discriminator_type)[0]
-                choice_children[
-                    discriminator_value
-                ] = convert_pydantic_model_to_datatype(
-                    case,
-                    datatype=CaseDataType,
-                    name=discriminator_value,
-                    strict=strict,
-                    excluded_fields=[discriminator],
+                choice_children[discriminator_value] = (
+                    convert_pydantic_model_to_datatype(
+                        case,
+                        datatype=CaseDataType,
+                        name=discriminator_value,
+                        strict=strict,
+                        excluded_fields=[discriminator],
+                    )
                 )
             children[field_name] = pydantic_field_to_datatype(
                 Choice,
                 field,
                 children=choice_children,
                 strict=strict,
                 discriminator_key=discriminator,
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/reask_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/reask_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 class NonParseableReAsk(ReAsk):
     pass
 
 
 def gather_reasks(
-    validated_output: Optional[Union[str, Dict, List, ReAsk]]
+    validated_output: Optional[Union[str, Dict, List, ReAsk]],
 ) -> Tuple[List[ReAsk], Union[Dict, List, None]]:
     """Traverse output and gather all ReAsk objects.
 
     Args:
         validated_output (Union[str, Dict, ReAsk], optional): The output of a model.
             Each value can be a ReAsk, a list, a dictionary, or a single value.
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/safe_get.py` & `guardrails_ai-0.4.4/guardrails/utils/safe_get.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/utils/sql_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/sql_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,18 @@
 class SQLDriver(ABC):
     """Abstract class for SQL drivers.
 
     The expose common functionality for validating SQL queries.
     """
 
     @abstractmethod
-    def validate_sql(self, query: str) -> List[str]:
-        ...
+    def validate_sql(self, query: str) -> List[str]: ...
 
     @abstractmethod
-    def get_schema(self) -> str:
-        ...
+    def get_schema(self) -> str: ...
 
 
 class SimpleSqlDriver(SQLDriver):
     """Simple SQL driver which uses sqlvalidator to validate SQL queries.
 
     Does not understands dialects and is not connected to a database.
     """
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/telemetry_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/telemetry_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,17 +73,15 @@
         "registered_name",
         "value_before_validation",
         "validation_result",
         "value_after_validation",
         "start_time",
         "end_time",
         "instance_id",
-    )(
-        validator_log
-    )
+    )(validator_log)
     result = (
         validation_result.outcome
         if hasattr(validation_result, "outcome")
         and validation_result.outcome is not None
         else "unknown"
     )
     result_type = get_result_type(
```

### Comparing `guardrails_ai-0.4.3/guardrails/utils/validator_utils.py` & `guardrails_ai-0.4.4/guardrails/utils/validator_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-# flake8: noqa
+# ruff: noqa
 """This module contains the constants and utils used by the validator.py."""
 
-
 from typing import Any, Dict, List, Optional, Tuple, Type, Union
 
 from guardrails.utils.safe_get import safe_get
 from guardrails.validator_base import Validator
 
 PROVENANCE_V1_PROMPT = """Instruction:
 As an Attribution Validator, you task is to verify whether the following contexts support the claim:
```

### Comparing `guardrails_ai-0.4.3/guardrails/validator_base.py` & `guardrails_ai-0.4.4/guardrails/validator_base.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validator_service.py` & `guardrails_ai-0.4.4/guardrails/validator_service.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,16 +122,14 @@
             property_path=property_path,
         )
         iteration.outputs.validator_logs.append(validator_logs)
 
         start_time = datetime.now()
         result = self.execute_validator(validator, value, metadata)
         end_time = datetime.now()
-
-        result = validator.validate(value, metadata)
         if result is None:
             result = PassResult()
 
         validator_logs.validation_result = result
         validator_logs.start_time = start_time
         validator_logs.end_time = end_time
         # If we ever re-use validator instances across multiple properties,
```

### Comparing `guardrails_ai-0.4.3/guardrails/validators/__init__.py` & `guardrails_ai-0.4.4/guardrails/validators/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """This module contains the validators for the Guardrails framework.
 
 The name with which a validator is registered is the name that is used
 in the `RAIL` spec to specify formatters.
 """
+
 from warnings import warn
 
 from guardrails.validator_base import (
     FailResult,
     PassResult,
     ValidationResult,
     Validator,
```

### Comparing `guardrails_ai-0.4.3/guardrails/validators/bug_free_python.py` & `guardrails_ai-0.4.4/guardrails/validators/bug_free_python.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/bug_free_sql.py` & `guardrails_ai-0.4.4/guardrails/validators/bug_free_sql.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/competitor_check.py` & `guardrails_ai-0.4.4/guardrails/validators/competitor_check.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/detect_secrets.py` & `guardrails_ai-0.4.4/guardrails/validators/detect_secrets.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/endpoint_is_reachable.py` & `guardrails_ai-0.4.4/guardrails/validators/endpoint_is_reachable.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/ends_with.py` & `guardrails_ai-0.4.4/guardrails/validators/ends_with.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/exclude_sql_predicates.py` & `guardrails_ai-0.4.4/guardrails/validators/exclude_sql_predicates.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/extracted_summary_sentences_match.py` & `guardrails_ai-0.4.4/guardrails/validators/extracted_summary_sentences_match.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/extractive_summary.py` & `guardrails_ai-0.4.4/guardrails/validators/extractive_summary.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/is_high_quality_translation.py` & `guardrails_ai-0.4.4/guardrails/validators/is_high_quality_translation.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/is_profanity_free.py` & `guardrails_ai-0.4.4/guardrails/validators/is_profanity_free.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/lower_case.py` & `guardrails_ai-0.4.4/guardrails/validators/lower_case.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/on_topic.py` & `guardrails_ai-0.4.4/guardrails/validators/on_topic.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/one_line.py` & `guardrails_ai-0.4.4/guardrails/validators/one_line.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/pii_filter.py` & `guardrails_ai-0.4.4/guardrails/validators/pii_filter.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/provenance.py` & `guardrails_ai-0.4.4/guardrails/validators/provenance.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/pydantic_field_validator.py` & `guardrails_ai-0.4.4/guardrails/validators/pydantic_field_validator.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/qa_relevance_llm_eval.py` & `guardrails_ai-0.4.4/guardrails/validators/qa_relevance_llm_eval.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/reading_time.py` & `guardrails_ai-0.4.4/guardrails/validators/reading_time.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/regex_match.py` & `guardrails_ai-0.4.4/guardrails/validators/regex_match.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/remove_redundant_sentences.py` & `guardrails_ai-0.4.4/guardrails/validators/remove_redundant_sentences.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/saliency_check.py` & `guardrails_ai-0.4.4/guardrails/validators/saliency_check.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/similar_to_document.py` & `guardrails_ai-0.4.4/guardrails/validators/similar_to_document.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/similar_to_list.py` & `guardrails_ai-0.4.4/guardrails/validators/similar_to_list.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/sql_column_presence.py` & `guardrails_ai-0.4.4/guardrails/validators/sql_column_presence.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/toxic_language.py` & `guardrails_ai-0.4.4/guardrails/validators/toxic_language.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/two_words.py` & `guardrails_ai-0.4.4/guardrails/validators/two_words.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/upper_case.py` & `guardrails_ai-0.4.4/guardrails/validators/upper_case.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/valid_choices.py` & `guardrails_ai-0.4.4/guardrails/validators/valid_choices.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/valid_length.py` & `guardrails_ai-0.4.4/guardrails/validators/valid_length.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/valid_range.py` & `guardrails_ai-0.4.4/guardrails/validators/valid_range.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/valid_url.py` & `guardrails_ai-0.4.4/guardrails/validators/valid_url.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validators/validators.py` & `guardrails_ai-0.4.4/guardrails/validators/validators.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/validatorsattr.py` & `guardrails_ai-0.4.4/guardrails/validatorsattr.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/vectordb/base.py` & `guardrails_ai-0.4.4/guardrails/vectordb/base.py`

 * *Files identical despite different names*

### Comparing `guardrails_ai-0.4.3/guardrails/vectordb/faiss.py` & `guardrails_ai-0.4.4/guardrails/vectordb/faiss.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,17 +83,15 @@
         self, vector: List[float], k: int, threshold: float
     ) -> List[int]:
         import numpy as np
 
         # Call faiss range search and get all the vectors with a score >= threshold
         # FIXME is this correct usage of `range_search`?
         #  Arguments missing for parameters "radius", "result"
-        _, dist, indexes = self._index.range_search(
-            np.array([vector]), threshold
-        )  # type: ignore
+        _, dist, indexes = self._index.range_search(np.array([vector]), threshold)  # type: ignore
 
         if len(indexes) == 0:
             return []
 
         sorted_indices = np.argsort(dist)
         sorted_indexes = indexes[sorted_indices]
         return sorted_indexes.tolist()[:k]
```

### Comparing `guardrails_ai-0.4.3/pyproject.toml` & `guardrails_ai-0.4.4/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [tool.poetry]
 name = "guardrails-ai"
-version = "0.4.3"
+version = "0.4.4"
 description = "Adding guardrails to large language models."
 authors = ["Guardrails AI <contact@guardrailsai.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 packages = [
     { include = "guardrails", from = "." }
 ]
 
 [tool.poetry.scripts]
 guardrails = "guardrails.cli:cli"
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
 lxml = "^4.9.3"
-openai = "<2"
+openai = "^1.30.1"
 rich = "^13.6.0"
 pydantic = ">=1.10.9, <3.0"
 typer = {extras = ["all"], version = "^0.9.0"}
 griffe = "^0.36.9"
 tenacity = ">=8.1.0"
 regex = "^2023.10.3"
 rstr = "^3.2.2"
 typing-extensions = "^4.8.0"
 python-dateutil = "^2.8.2"
-tiktoken = "^0.5.1"
+tiktoken = ">=0.5.1"
 
 sqlvalidator = {version = "^0.0.20", optional = true}
 sqlalchemy = {version = ">=2.0.9", optional = true}
 sqlglot = {version = "^19.0.3", optional = true}
 thefuzz = {version = "^0.20.0", optional = true}
 nltk = {version = "^3.8.1", optional = true}
 faiss-cpu = {version = "^1.7.4", optional = true}
 numpy = {version = ">=1.24", optional = true}
 alt-profanity-check = {version = "^1.3.1", optional = true}
 detect-secrets = {version = "^1.4.0", optional = true}
-litellm = {version = "^1.34.38", optional = true}
+litellm = {version = "^1.37.14", optional = true}
 manifest-ml = {version = "^0.1.8", optional = true}
 transformers = {version = "^4.36.0", optional = true}
 presidio_analyzer = {version = "^2.2.33", optional = true}
 presidio_anonymizer = {version = "^2.2.33", optional = true}
 spacy-transformers = {version = "^1.3.4", optional = true}
 anthropic = {version = "^0.7.2", optional = true}
 torch = {version = "^2.1.1", optional = true}
@@ -54,16 +54,15 @@
 opentelemetry-exporter-otlp-proto-grpc = "1.20.0"
 opentelemetry-exporter-otlp-proto-http = "1.20.0"
 langchain-core = "^0.1.18"
 coloredlogs = "^15.0.1"
 requests = "^2.31.0"
 guardrails-api-client = "^0.1.1"
 jwt = "^1.3.1"
-
-
+pip = ">=22"
 
 [tool.poetry.extras]
 sql = ["sqlvalidator", "sqlalchemy", "sqlglot"]
 summary = ["thefuzz", "nltk"]
 vectordb = ["faiss-cpu", "numpy"]
 profanity = ["alt-profanity-check"]
 detect-secrets = ["detect-secrets"]
@@ -76,25 +75,23 @@
 anthropic = ["anthropic"]
 docs-build = ["nbdoc", "docspec_python", "pydoc-markdown"]
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
-black = "^23.0.0"
-isort = ">=5.12.0"
-flake8 = ">=3.8.4"
 docformatter = ">=1.4"
 pytest-cov = ">=2.10.1"
 pre-commit = ">=2.9.3"
 twine = "^4.0.2"
 pytest-mock = "^3.12.0"
 pypdfium2 = "^4.23.1"
 pyright = "1.1.334"
 lxml-stubs = "^0.4.0"
+ruff = ">=0.4.1"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
 mkdocs = "^1.5.3"
 mkdocstrings = {extras = ["python"], version = "^0.23.0"}
@@ -109,14 +106,10 @@
 [[tool.poetry.source]]
 name = "PyPI"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
-[tool.isort]
-multi_line_output = 3
-include_trailing_comma = true
-force_grid_wrap = 0
-use_parentheses = true
-ensure_newline_before_comments = true
-line_length = 88
+[tool.ruff.lint]
+select = ["E4", "E7", "E9", "F", "E501"]
+ignore = ["E731", "E203", "E741"]
```

### Comparing `guardrails_ai-0.4.3/PKG-INFO` & `guardrails_ai-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: guardrails-ai
-Version: 0.4.3
+Version: 0.4.4
 Summary: Adding guardrails to large language models.
 License: Apache-2.0
 Author: Guardrails AI
 Author-email: contact@guardrailsai.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -32,24 +32,25 @@
 Requires-Dist: docspec_python (==2.2.1) ; extra == "docs-build"
 Requires-Dist: faiss-cpu (>=1.7.4,<2.0.0) ; extra == "vectordb"
 Requires-Dist: griffe (>=0.36.9,<0.37.0)
 Requires-Dist: guardrails-api-client (>=0.1.1,<0.2.0)
 Requires-Dist: huggingface_hub (>=0.19.3,<0.20.0) ; extra == "high-quality-translation"
 Requires-Dist: jwt (>=1.3.1,<2.0.0)
 Requires-Dist: langchain-core (>=0.1.18,<0.2.0)
-Requires-Dist: litellm (>=1.34.38,<2.0.0) ; extra == "litellm"
+Requires-Dist: litellm (>=1.37.14,<2.0.0) ; extra == "litellm"
 Requires-Dist: lxml (>=4.9.3,<5.0.0)
 Requires-Dist: manifest-ml (>=0.1.8,<0.2.0) ; extra == "manifest"
 Requires-Dist: nbdoc (>=0.0.82,<0.0.83) ; extra == "docs-build"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "summary"
 Requires-Dist: numpy (>=1.24) ; extra == "vectordb"
-Requires-Dist: openai (<2)
+Requires-Dist: openai (>=1.30.1,<2.0.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-grpc (==1.20.0)
 Requires-Dist: opentelemetry-exporter-otlp-proto-http (==1.20.0)
 Requires-Dist: opentelemetry-sdk (==1.20.0)
+Requires-Dist: pip (>=22)
 Requires-Dist: presidio_analyzer (>=2.2.33,<3.0.0) ; extra == "pii"
 Requires-Dist: presidio_anonymizer (>=2.2.33,<3.0.0) ; extra == "pii"
 Requires-Dist: pydantic (>=1.10.9,<3.0)
 Requires-Dist: pydash (>=7.0.6,<8.0.0)
 Requires-Dist: pydoc-markdown (==4.8.2) ; extra == "docs-build"
 Requires-Dist: python-dateutil (>=2.8.2,<3.0.0)
 Requires-Dist: regex (>=2023.10.3,<2024.0.0)
@@ -58,15 +59,15 @@
 Requires-Dist: rstr (>=3.2.2,<4.0.0)
 Requires-Dist: spacy-transformers (>=1.3.4,<2.0.0) ; extra == "competitor-check"
 Requires-Dist: sqlalchemy (>=2.0.9) ; extra == "sql"
 Requires-Dist: sqlglot (>=19.0.3,<20.0.0) ; extra == "sql"
 Requires-Dist: sqlvalidator (>=0.0.20,<0.0.21) ; extra == "sql"
 Requires-Dist: tenacity (>=8.1.0)
 Requires-Dist: thefuzz (>=0.20.0,<0.21.0) ; extra == "summary"
-Requires-Dist: tiktoken (>=0.5.1,<0.6.0)
+Requires-Dist: tiktoken (>=0.5.1)
 Requires-Dist: torch (>=2.1.1,<3.0.0) ; extra == "toxic-language"
 Requires-Dist: transformers (>=4.36.0,<5.0.0) ; extra == "toxic-language"
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Requires-Dist: typing-extensions (>=4.8.0,<5.0.0)
 Requires-Dist: unbabel-comet (>=2.2.1,<3.0.0) ; extra == "high-quality-translation"
 Description-Content-Type: text/markdown
```

