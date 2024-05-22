# Comparing `tmp/cohere-5.5.0.tar.gz` & `tmp/cohere-5.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cohere-5.5.0.tar", max compression
+gzip compressed data, was "cohere-5.5.1.tar", max compression
```

## Comparing `cohere-5.5.0.tar` & `cohere-5.5.1.tar`

### file list

```diff
@@ -1,181 +1,182 @@
--rw-r--r--   0        0        0     1062 2024-05-14 14:20:55.077003 cohere-5.5.0/LICENSE
--rw-r--r--   0        0        0     2359 2024-05-14 14:20:55.077003 cohere-5.5.0/README.md
--rw-r--r--   0        0        0      716 2024-05-14 14:20:55.085003 cohere-5.5.0/pyproject.toml
--rw-r--r--   0        0        0     8381 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/__init__.py
--rw-r--r--   0        0        0   225270 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/base_client.py
--rw-r--r--   0        0        0     9142 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/bedrock_client.py
--rw-r--r--   0        0        0    19723 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/client.py
--rw-r--r--   0        0        0       22 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/config.py
--rw-r--r--   0        0        0       65 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/connectors/__init__.py
--rw-r--r--   0        0        0    50609 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/connectors/client.py
--rw-r--r--   0        0        0     1006 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/__init__.py
--rw-r--r--   0        0        0      426 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/api_error.py
--rw-r--r--   0        0        0     2226 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/client_wrapper.py
--rw-r--r--   0        0        0     1047 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/datetime_utils.py
--rw-r--r--   0        0        0     1480 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/file.py
--rw-r--r--   0        0        0     5059 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/http_client.py
--rw-r--r--   0        0        0     3742 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/jsonable_encoder.py
--rw-r--r--   0        0        0      329 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/pydantic_utilities.py
--rw-r--r--   0        0        0      330 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/remove_none_from_dict.py
--rw-r--r--   0        0        0     1420 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/request_options.py
--rw-r--r--   0        0        0     7123 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/core/unchecked_base_model.py
--rw-r--r--   0        0        0      419 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/__init__.py
--rw-r--r--   0        0        0    35730 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/client.py
--rw-r--r--   0        0        0      578 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/__init__.py
--rw-r--r--   0        0        0     1002 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/datasets_create_response.py
--rw-r--r--   0        0        0     1402 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
--rw-r--r--   0        0        0      959 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/datasets_get_response.py
--rw-r--r--   0        0        0     1057 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/datasets_get_usage_response.py
--rw-r--r--   0        0        0      998 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/datasets/types/datasets_list_response.py
--rw-r--r--   0        0        0      159 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/embed_jobs/__init__.py
--rw-r--r--   0        0        0    31897 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/embed_jobs/client.py
--rw-r--r--   0        0        0      187 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/embed_jobs/types/__init__.py
--rw-r--r--   0        0        0      169 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
--rw-r--r--   0        0        0      159 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/environment.py
--rw-r--r--   0        0        0      617 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/__init__.py
--rw-r--r--   0        0        0      248 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/bad_request_error.py
--rw-r--r--   0        0        0      247 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/forbidden_error.py
--rw-r--r--   0        0        0      252 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/internal_server_error.py
--rw-r--r--   0        0        0      246 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/not_found_error.py
--rw-r--r--   0        0        0      290 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/service_unavailable_error.py
--rw-r--r--   0        0        0      326 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/too_many_requests_error.py
--rw-r--r--   0        0        0      284 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/errors/unauthorized_error.py
--rw-r--r--   0        0        0      953 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/__init__.py
--rw-r--r--   0        0        0    62155 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/client.py
--rw-r--r--   0        0        0      905 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/__init__.py
--rw-r--r--   0        0        0     1343 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/__init__.py
--rw-r--r--   0        0        0     1475 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/base_model.py
--rw-r--r--   0        0        0      305 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/base_type.py
--rw-r--r--   0        0        0     1175 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
--rw-r--r--   0        0        0      140 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
--rw-r--r--   0        0        0     1083 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/error.py
--rw-r--r--   0        0        0     1400 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/event.py
--rw-r--r--   0        0        0     2357 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/finetuned_model.py
--rw-r--r--   0        0        0     1171 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
--rw-r--r--   0        0        0     1823 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/hyperparameters.py
--rw-r--r--   0        0        0     1489 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_events_response.py
--rw-r--r--   0        0        0     1532 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
--rw-r--r--   0        0        0     1463 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
--rw-r--r--   0        0        0     1577 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/settings.py
--rw-r--r--   0        0        0      402 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/status.py
--rw-r--r--   0        0        0      193 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/strategy.py
--rw-r--r--   0        0        0     1390 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py
--rw-r--r--   0        0        0     1177 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
--rw-r--r--   0        0        0      811 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/manually_maintained/cache.py
--rw-r--r--   0        0        0     3015 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/manually_maintained/tokenizers.py
--rw-r--r--   0        0        0       65 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/models/__init__.py
--rw-r--r--   0        0        0    13859 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/models/client.py
--rw-r--r--   0        0        0      730 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/overrides.py
--rw-r--r--   0        0        0        0 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/py.typed
--rw-r--r--   0        0        0    10564 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/__init__.py
--rw-r--r--   0        0        0     1260 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/api_meta.py
--rw-r--r--   0        0        0     1011 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/api_meta_api_version.py
--rw-r--r--   0        0        0     1434 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/api_meta_billed_units.py
--rw-r--r--   0        0        0     1177 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/api_meta_tokens.py
--rw-r--r--   0        0        0      168 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/auth_token_type.py
--rw-r--r--   0        0        0     1929 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/chat_citation.py
--rw-r--r--   0        0        0     1127 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/chat_citation_generation_event.py
--rw-r--r--   0        0        0     1861 2024-05-14 14:20:55.085003 cohere-5.5.0/src/cohere/types/chat_connector.py
--rw-r--r--   0        0        0     1297 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_data_metrics.py
--rw-r--r--   0        0        0      117 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_document.py
--rw-r--r--   0        0        0     1652 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_message.py
--rw-r--r--   0        0        0      170 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_request_citation_quality.py
--rw-r--r--   0        0        0     1708 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_request_connectors_search_options.py
--rw-r--r--   0        0        0      189 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_request_prompt_truncation.py
--rw-r--r--   0        0        0     1180 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_search_queries_generation_event.py
--rw-r--r--   0        0        0     1247 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_search_query.py
--rw-r--r--   0        0        0     1653 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_search_result.py
--rw-r--r--   0        0        0     1055 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_search_result_connector.py
--rw-r--r--   0        0        0     1417 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_search_results_event.py
--rw-r--r--   0        0        0     1861 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_end_event.py
--rw-r--r--   0        0        0      225 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_end_event_finish_reason.py
--rw-r--r--   0        0        0      893 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_event.py
--rw-r--r--   0        0        0      176 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_request_citation_quality.py
--rw-r--r--   0        0        0     1714 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_request_connectors_search_options.py
--rw-r--r--   0        0        0      195 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_request_prompt_truncation.py
--rw-r--r--   0        0        0     1102 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_stream_start_event.py
--rw-r--r--   0        0        0     1068 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_text_generation_event.py
--rw-r--r--   0        0        0     1040 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/chat_tool_calls_generation_event.py
--rw-r--r--   0        0        0     1005 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/check_api_key_response.py
--rw-r--r--   0        0        0     1004 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_data_metrics.py
--rw-r--r--   0        0        0      971 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_example.py
--rw-r--r--   0        0        0      171 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_request_truncate.py
--rw-r--r--   0        0        0     1137 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_response.py
--rw-r--r--   0        0        0     2560 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_response_classifications_item.py
--rw-r--r--   0        0        0      214 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_response_classifications_item_classification_type.py
--rw-r--r--   0        0        0      971 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/classify_response_classifications_item_labels_value.py
--rw-r--r--   0        0        0      220 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/compatible_endpoint.py
--rw-r--r--   0        0        0     3383 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/connector.py
--rw-r--r--   0        0        0      163 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/connector_auth_status.py
--rw-r--r--   0        0        0     1660 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/connector_o_auth.py
--rw-r--r--   0        0        0     1725 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/create_connector_o_auth.py
--rw-r--r--   0        0        0      960 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/create_connector_response.py
--rw-r--r--   0        0        0     1195 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/create_connector_service_auth.py
--rw-r--r--   0        0        0     1047 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/create_embed_job_response.py
--rw-r--r--   0        0        0     2209 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/dataset.py
--rw-r--r--   0        0        0     1788 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/dataset_part.py
--rw-r--r--   0        0        0      427 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/dataset_type.py
--rw-r--r--   0        0        0      222 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/dataset_validation_status.py
--rw-r--r--   0        0        0      135 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/delete_connector_response.py
--rw-r--r--   0        0        0     1068 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/detokenize_response.py
--rw-r--r--   0        0        0     1416 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_by_type_response.py
--rw-r--r--   0        0        0     2271 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_by_type_response_embeddings.py
--rw-r--r--   0        0        0     1364 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_floats_response.py
--rw-r--r--   0        0        0      211 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_input_type.py
--rw-r--r--   0        0        0     1864 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_job.py
--rw-r--r--   0        0        0      201 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_job_status.py
--rw-r--r--   0        0        0      156 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_job_truncate.py
--rw-r--r--   0        0        0      168 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_request_truncate.py
--rw-r--r--   0        0        0     1057 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embed_response.py
--rw-r--r--   0        0        0      184 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/embedding_type.py
--rw-r--r--   0        0        0     1735 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/finetune_dataset_metrics.py
--rw-r--r--   0        0        0      222 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/finish_reason.py
--rw-r--r--   0        0        0      185 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_request_return_likelihoods.py
--rw-r--r--   0        0        0      171 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_request_truncate.py
--rw-r--r--   0        0        0     1197 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_end.py
--rw-r--r--   0        0        0     1101 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_end_response.py
--rw-r--r--   0        0        0     1311 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_error.py
--rw-r--r--   0        0        0      897 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_event.py
--rw-r--r--   0        0        0      191 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_request_return_likelihoods.py
--rw-r--r--   0        0        0      177 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_request_truncate.py
--rw-r--r--   0        0        0     1312 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_stream_text.py
--rw-r--r--   0        0        0     1456 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generate_streamed_response.py
--rw-r--r--   0        0        0     1254 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/generation.py
--rw-r--r--   0        0        0      957 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/get_connector_response.py
--rw-r--r--   0        0        0     2150 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/get_model_response.py
--rw-r--r--   0        0        0     1256 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/label_metric.py
--rw-r--r--   0        0        0     1095 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/list_connectors_response.py
--rw-r--r--   0        0        0      993 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/list_embed_job_response.py
--rw-r--r--   0        0        0     1187 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/list_models_response.py
--rw-r--r--   0        0        0     1336 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/message.py
--rw-r--r--   0        0        0     1130 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/metrics.py
--rw-r--r--   0        0        0     1115 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/metrics_embed_data.py
--rw-r--r--   0        0        0     1154 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/metrics_embed_data_fields_item.py
--rw-r--r--   0        0        0     2940 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/non_streamed_chat_response.py
--rw-r--r--   0        0        0     1080 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/o_auth_authorize_response.py
--rw-r--r--   0        0        0      974 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/parse_info.py
--rw-r--r--   0        0        0      239 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/rerank_request_documents_item.py
--rw-r--r--   0        0        0     1001 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/rerank_request_documents_item_text.py
--rw-r--r--   0        0        0     1200 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/rerank_response.py
--rw-r--r--   0        0        0     1909 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/rerank_response_results_item.py
--rw-r--r--   0        0        0     1136 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/rerank_response_results_item_document.py
--rw-r--r--   0        0        0     1818 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/reranker_data_metrics.py
--rw-r--r--   0        0        0     1819 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/single_generation.py
--rw-r--r--   0        0        0     1248 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/single_generation_in_stream.py
--rw-r--r--   0        0        0      952 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/single_generation_token_likelihoods_item.py
--rw-r--r--   0        0        0     3157 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/streamed_chat_response.py
--rw-r--r--   0        0        0      179 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/summarize_request_extractiveness.py
--rw-r--r--   0        0        0      170 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/summarize_request_format.py
--rw-r--r--   0        0        0      173 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/summarize_request_length.py
--rw-r--r--   0        0        0     1201 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/summarize_response.py
--rw-r--r--   0        0        0     1127 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tokenize_response.py
--rw-r--r--   0        0        0      941 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/too_many_requests_error_body.py
--rw-r--r--   0        0        0     1928 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tool.py
--rw-r--r--   0        0        0     1221 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tool_call.py
--rw-r--r--   0        0        0     1057 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tool_message.py
--rw-r--r--   0        0        0     1331 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tool_parameter_definitions_value.py
--rw-r--r--   0        0        0      995 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/tool_result.py
--rw-r--r--   0        0        0      960 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/types/update_connector_response.py
--rw-r--r--   0        0        0    10055 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/utils.py
--rw-r--r--   0        0        0       74 2024-05-14 14:20:55.089003 cohere-5.5.0/src/cohere/version.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 cohere-5.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-22 14:34:21.058162 cohere-5.5.1/LICENSE
+-rw-r--r--   0        0        0     2359 2024-05-22 14:34:21.058162 cohere-5.5.1/README.md
+-rw-r--r--   0        0        0     1458 2024-05-22 14:34:21.066162 cohere-5.5.1/pyproject.toml
+-rw-r--r--   0        0        0     8381 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/__init__.py
+-rw-r--r--   0        0        0   211417 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/base_client.py
+-rw-r--r--   0        0        0     9142 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/bedrock_client.py
+-rw-r--r--   0        0        0    19723 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/client.py
+-rw-r--r--   0        0        0       22 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/config.py
+-rw-r--r--   0        0        0       65 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/connectors/__init__.py
+-rw-r--r--   0        0        0    53293 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/connectors/client.py
+-rw-r--r--   0        0        0     1126 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/__init__.py
+-rw-r--r--   0        0        0      426 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/api_error.py
+-rw-r--r--   0        0        0     2226 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/client_wrapper.py
+-rw-r--r--   0        0        0     1047 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/datetime_utils.py
+-rw-r--r--   0        0        0     1480 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/file.py
+-rw-r--r--   0        0        0     5059 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/http_client.py
+-rw-r--r--   0        0        0     3742 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/jsonable_encoder.py
+-rw-r--r--   0        0        0      748 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/pydantic_utilities.py
+-rw-r--r--   0        0        0     1266 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/query_encoder.py
+-rw-r--r--   0        0        0      330 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/remove_none_from_dict.py
+-rw-r--r--   0        0        0     1420 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/request_options.py
+-rw-r--r--   0        0        0     7165 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/core/unchecked_base_model.py
+-rw-r--r--   0        0        0      419 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/__init__.py
+-rw-r--r--   0        0        0    38300 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/client.py
+-rw-r--r--   0        0        0      578 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/__init__.py
+-rw-r--r--   0        0        0     1265 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_create_response.py
+-rw-r--r--   0        0        0     1665 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py
+-rw-r--r--   0        0        0     1222 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_get_response.py
+-rw-r--r--   0        0        0     1320 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_get_usage_response.py
+-rw-r--r--   0        0        0     1261 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/datasets/types/datasets_list_response.py
+-rw-r--r--   0        0        0      159 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/__init__.py
+-rw-r--r--   0        0        0    32495 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/client.py
+-rw-r--r--   0        0        0      187 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/types/__init__.py
+-rw-r--r--   0        0        0      169 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/embed_jobs/types/create_embed_job_request_truncate.py
+-rw-r--r--   0        0        0      160 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/environment.py
+-rw-r--r--   0        0        0      617 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/__init__.py
+-rw-r--r--   0        0        0      248 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/bad_request_error.py
+-rw-r--r--   0        0        0      247 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/forbidden_error.py
+-rw-r--r--   0        0        0      252 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/internal_server_error.py
+-rw-r--r--   0        0        0      246 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/not_found_error.py
+-rw-r--r--   0        0        0      290 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/service_unavailable_error.py
+-rw-r--r--   0        0        0      326 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/too_many_requests_error.py
+-rw-r--r--   0        0        0      284 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/errors/unauthorized_error.py
+-rw-r--r--   0        0        0      953 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/__init__.py
+-rw-r--r--   0        0        0    65157 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/client.py
+-rw-r--r--   0        0        0      905 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/__init__.py
+-rw-r--r--   0        0        0     1343 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/__init__.py
+-rw-r--r--   0        0        0     1738 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_model.py
+-rw-r--r--   0        0        0      305 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_type.py
+-rw-r--r--   0        0        0     1438 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py
+-rw-r--r--   0        0        0      140 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/delete_finetuned_model_response.py
+-rw-r--r--   0        0        0     1346 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/error.py
+-rw-r--r--   0        0        0     1663 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/event.py
+-rw-r--r--   0        0        0     2620 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/finetuned_model.py
+-rw-r--r--   0        0        0     1434 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py
+-rw-r--r--   0        0        0     2086 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/hyperparameters.py
+-rw-r--r--   0        0        0     1752 2024-05-22 14:34:21.066162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_events_response.py
+-rw-r--r--   0        0        0     1795 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py
+-rw-r--r--   0        0        0     1726 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py
+-rw-r--r--   0        0        0     1840 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/settings.py
+-rw-r--r--   0        0        0      402 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/status.py
+-rw-r--r--   0        0        0      193 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/strategy.py
+-rw-r--r--   0        0        0     1653 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py
+-rw-r--r--   0        0        0     1440 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py
+-rw-r--r--   0        0        0      811 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/manually_maintained/cache.py
+-rw-r--r--   0        0        0     3015 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/manually_maintained/tokenizers.py
+-rw-r--r--   0        0        0       65 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/models/__init__.py
+-rw-r--r--   0        0        0    14701 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/models/client.py
+-rw-r--r--   0        0        0      730 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/overrides.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/py.typed
+-rw-r--r--   0        0        0    10564 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/__init__.py
+-rw-r--r--   0        0        0     1523 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta.py
+-rw-r--r--   0        0        0     1274 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_api_version.py
+-rw-r--r--   0        0        0     1697 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_billed_units.py
+-rw-r--r--   0        0        0     1440 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/api_meta_tokens.py
+-rw-r--r--   0        0        0      168 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/auth_token_type.py
+-rw-r--r--   0        0        0     2192 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_citation.py
+-rw-r--r--   0        0        0     1390 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_citation_generation_event.py
+-rw-r--r--   0        0        0     2124 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_connector.py
+-rw-r--r--   0        0        0     1560 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_data_metrics.py
+-rw-r--r--   0        0        0      117 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_document.py
+-rw-r--r--   0        0        0     1804 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_message.py
+-rw-r--r--   0        0        0      170 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_citation_quality.py
+-rw-r--r--   0        0        0     1971 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_connectors_search_options.py
+-rw-r--r--   0        0        0      189 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1443 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_queries_generation_event.py
+-rw-r--r--   0        0        0     1510 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_query.py
+-rw-r--r--   0        0        0     1916 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_result.py
+-rw-r--r--   0        0        0     1318 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_result_connector.py
+-rw-r--r--   0        0        0     1680 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_search_results_event.py
+-rw-r--r--   0        0        0     2124 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_end_event.py
+-rw-r--r--   0        0        0      225 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_end_event_finish_reason.py
+-rw-r--r--   0        0        0     1156 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_event.py
+-rw-r--r--   0        0        0      176 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_citation_quality.py
+-rw-r--r--   0        0        0     1977 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_connectors_search_options.py
+-rw-r--r--   0        0        0      195 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_request_prompt_truncation.py
+-rw-r--r--   0        0        0     1365 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_stream_start_event.py
+-rw-r--r--   0        0        0     1331 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_text_generation_event.py
+-rw-r--r--   0        0        0     1303 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/chat_tool_calls_generation_event.py
+-rw-r--r--   0        0        0     1268 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/check_api_key_response.py
+-rw-r--r--   0        0        0     1267 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_data_metrics.py
+-rw-r--r--   0        0        0     1234 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_example.py
+-rw-r--r--   0        0        0      171 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_request_truncate.py
+-rw-r--r--   0        0        0     1400 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response.py
+-rw-r--r--   0        0        0     2823 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item.py
+-rw-r--r--   0        0        0      214 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item_classification_type.py
+-rw-r--r--   0        0        0     1234 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/classify_response_classifications_item_labels_value.py
+-rw-r--r--   0        0        0      220 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/compatible_endpoint.py
+-rw-r--r--   0        0        0     3646 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector.py
+-rw-r--r--   0        0        0      163 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector_auth_status.py
+-rw-r--r--   0        0        0     1923 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/connector_o_auth.py
+-rw-r--r--   0        0        0     1988 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_o_auth.py
+-rw-r--r--   0        0        0     1223 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_response.py
+-rw-r--r--   0        0        0     1458 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_connector_service_auth.py
+-rw-r--r--   0        0        0     1310 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/create_embed_job_response.py
+-rw-r--r--   0        0        0     2472 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset.py
+-rw-r--r--   0        0        0     2051 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_part.py
+-rw-r--r--   0        0        0      427 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_type.py
+-rw-r--r--   0        0        0      222 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/dataset_validation_status.py
+-rw-r--r--   0        0        0      135 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/delete_connector_response.py
+-rw-r--r--   0        0        0     1331 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/detokenize_response.py
+-rw-r--r--   0        0        0     1679 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_by_type_response.py
+-rw-r--r--   0        0        0     2534 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_by_type_response_embeddings.py
+-rw-r--r--   0        0        0     1627 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_floats_response.py
+-rw-r--r--   0        0        0      211 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_input_type.py
+-rw-r--r--   0        0        0     2127 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job.py
+-rw-r--r--   0        0        0      201 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job_status.py
+-rw-r--r--   0        0        0      156 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_job_truncate.py
+-rw-r--r--   0        0        0      168 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_request_truncate.py
+-rw-r--r--   0        0        0     2831 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embed_response.py
+-rw-r--r--   0        0        0      184 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/embedding_type.py
+-rw-r--r--   0        0        0     1998 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/finetune_dataset_metrics.py
+-rw-r--r--   0        0        0      222 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/finish_reason.py
+-rw-r--r--   0        0        0      185 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_request_return_likelihoods.py
+-rw-r--r--   0        0        0      171 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_request_truncate.py
+-rw-r--r--   0        0        0     1460 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_end.py
+-rw-r--r--   0        0        0     1364 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_end_response.py
+-rw-r--r--   0        0        0     1574 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_error.py
+-rw-r--r--   0        0        0     1160 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_event.py
+-rw-r--r--   0        0        0      191 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_request_return_likelihoods.py
+-rw-r--r--   0        0        0      177 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_request_truncate.py
+-rw-r--r--   0        0        0     1575 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_stream_text.py
+-rw-r--r--   0        0        0     4579 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generate_streamed_response.py
+-rw-r--r--   0        0        0     1517 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/generation.py
+-rw-r--r--   0        0        0     1220 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/get_connector_response.py
+-rw-r--r--   0        0        0     2413 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/get_model_response.py
+-rw-r--r--   0        0        0     1519 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/label_metric.py
+-rw-r--r--   0        0        0     1358 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_connectors_response.py
+-rw-r--r--   0        0        0     1256 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_embed_job_response.py
+-rw-r--r--   0        0        0     1450 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/list_models_response.py
+-rw-r--r--   0        0        0     4531 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/message.py
+-rw-r--r--   0        0        0     1393 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics.py
+-rw-r--r--   0        0        0     1378 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics_embed_data.py
+-rw-r--r--   0        0        0     1417 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/metrics_embed_data_fields_item.py
+-rw-r--r--   0        0        0     3203 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/non_streamed_chat_response.py
+-rw-r--r--   0        0        0     1343 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/o_auth_authorize_response.py
+-rw-r--r--   0        0        0     1237 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/parse_info.py
+-rw-r--r--   0        0        0      239 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_request_documents_item.py
+-rw-r--r--   0        0        0     1264 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_request_documents_item_text.py
+-rw-r--r--   0        0        0     1463 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response.py
+-rw-r--r--   0        0        0     2172 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response_results_item.py
+-rw-r--r--   0        0        0     1399 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/rerank_response_results_item_document.py
+-rw-r--r--   0        0        0     2081 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/reranker_data_metrics.py
+-rw-r--r--   0        0        0     2082 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation.py
+-rw-r--r--   0        0        0     1511 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation_in_stream.py
+-rw-r--r--   0        0        0     1215 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/single_generation_token_likelihoods_item.py
+-rw-r--r--   0        0        0     9119 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/streamed_chat_response.py
+-rw-r--r--   0        0        0      179 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_extractiveness.py
+-rw-r--r--   0        0        0      170 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_format.py
+-rw-r--r--   0        0        0      173 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_request_length.py
+-rw-r--r--   0        0        0     1464 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/summarize_response.py
+-rw-r--r--   0        0        0     1390 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tokenize_response.py
+-rw-r--r--   0        0        0     1204 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/too_many_requests_error_body.py
+-rw-r--r--   0        0        0     2191 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool.py
+-rw-r--r--   0        0        0     1484 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_call.py
+-rw-r--r--   0        0        0     1320 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_message.py
+-rw-r--r--   0        0        0     1594 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_parameter_definitions_value.py
+-rw-r--r--   0        0        0     1258 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/tool_result.py
+-rw-r--r--   0        0        0     1223 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/types/update_connector_response.py
+-rw-r--r--   0        0        0    10055 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/utils.py
+-rw-r--r--   0        0        0       74 2024-05-22 14:34:21.070162 cohere-5.5.1/src/cohere/version.py
+-rw-r--r--   0        0        0     3561 1970-01-01 00:00:00.000000 cohere-5.5.1/PKG-INFO
```

### Comparing `cohere-5.5.0/LICENSE` & `cohere-5.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/README.md` & `cohere-5.5.1/README.md`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/__init__.py` & `cohere-5.5.1/src/cohere/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/base_client.py` & `cohere-5.5.1/src/cohere/base_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import httpx
 
 from .connectors.client import AsyncConnectorsClient, ConnectorsClient
 from .core.api_error import ApiError
 from .core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from .core.jsonable_encoder import jsonable_encoder
+from .core.query_encoder import encode_query
 from .core.remove_none_from_dict import remove_none_from_dict
 from .core.request_options import RequestOptions
 from .core.unchecked_base_model import construct_type
 from .datasets.client import AsyncDatasetsClient, DatasetsClient
 from .embed_jobs.client import AsyncEmbedJobsClient, EmbedJobsClient
 from .environment import ClientEnvironment
 from .errors.bad_request_error import BadRequestError
@@ -62,31 +63,41 @@
 OMIT = typing.cast(typing.Any, ...)
 
 
 class BaseCohere:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: ClientEnvironment. The environment to use for requests from the client. from .environment import ClientEnvironment
+    environment : ClientEnvironment
+        The environment to use for requests from the client. from .environment import ClientEnvironment
 
-                                          Defaults to ClientEnvironment.PRODUCTION
 
-        - client_name: typing.Optional[str].
 
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
+        Defaults to ClientEnvironment.PRODUCTION
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.Client]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+    client_name : typing.Optional[str]
+    token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.Client]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from cohere.client import Client
 
     client = Client(
         client_name="YOUR_CLIENT_NAME",
         token="YOUR_TOKEN",
     )
     """
@@ -95,15 +106,15 @@
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
         client_name: typing.Optional[str] = None,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv("CO_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.Client] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 300 if httpx_client is None else None
         if token is None:
             raise ApiError(body="The client must be instantiated be either passing in token or setting CO_API_KEY")
         self._client_wrapper = SyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
@@ -144,169 +155,227 @@
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
         return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ToolResult]] = OMIT,
+        force_single_step: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.Iterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
-        Parameters:
-            - message: str. Text input for the model to respond to.
-                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        Parameters
+        ----------
+        message : str
+            Text input for the model to respond to.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        model : typing.Optional[str]
+            Defaults to `command-r-plus`.
+
+            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+            Compatible Deployments: Cohere Platform, Private Deployments
+
+
+        preamble : typing.Optional[str]
+            When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+
+            The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        chat_history : typing.Optional[typing.Sequence[Message]]
+            A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+
+            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+
+            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        conversation_id : typing.Optional[str]
+            An alternative to `chat_history`.
+
+            Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+            Compatible Deployments: Cohere Platform
+
+
+        prompt_truncation : typing.Optional[ChatStreamRequestPromptTruncation]
+            Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
+
+            Dictates how the prompt will be constructed.
+
+            With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+
+            With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
+
+            With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+            Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+
+
+        connectors : typing.Optional[typing.Sequence[ChatConnector]]
+            Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
+
+            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+            Compatible Deployments: Cohere Platform
+
+
+        search_queries_only : typing.Optional[bool]
+            Defaults to `false`.
+
+            When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
 
-            - model: typing.Optional[str]. Defaults to `command-r-plus`.
+        documents : typing.Optional[typing.Sequence[ChatDocument]]
+            A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
-                                           The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
-                                           Compatible Deployments: Cohere Platform, Private Deployments
+            Example:
+            `[
+              { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
+              { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
+            ]`
 
-            - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+            Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-                                              The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
-                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-            - chat_history: typing.Optional[typing.Sequence[Message]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+            An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
-                                                                       Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+            An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                       The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
-                                                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
-                                                     Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
-                                                     Compatible Deployments: Cohere Platform
+        citation_quality : typing.Optional[ChatStreamRequestCitationQuality]
+            Defaults to `"accurate"`.
 
-            - prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
+            Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                                     Dictates how the prompt will be constructed.
 
-                                                                                     With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+        temperature : typing.Optional[float]
+            Defaults to `0.3`.
 
-                                                                                     With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
-                                                                                     With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
-                                                                                     Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+            Randomness can be further maximized by increasing the  value of the `p` parameter.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
-                                                                           When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
-                                                                           Compatible Deployments: Cohere Platform
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
-                                                          When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
-                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        max_input_tokens : typing.Optional[int]
+            The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
-            - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
+            Input will be truncated according to the `prompt_truncation` parameter.
+            Compatible Deployments: Cohere Platform
 
-                                                                         Example:
-                                                                         `[
-                                                                           { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
-                                                                           { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
-                                                                         ]`
 
-                                                                         Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-                                                                         An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
-                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens
+            deterministically, such that repeated requests with the same
+            seed and parameters should return the same result. However,
+            determinism cannot be totally guaranteed.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
 
-                                                                                   Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
-                                                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - temperature: typing.Optional[float]. Defaults to `0.3`.
 
-                                                   A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
+        frequency_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                   Randomness can be further maximized by increasing the  value of the `p` parameter.
-                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
-                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                      Input will be truncated according to the `prompt_truncation` parameter.
-                                                      Compatible Deployments: Cohere Platform
+            Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
-                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
-                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without
+            any pre-processing.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
-                                            deterministically, such that repeated requests with the same
-                                            seed and parameters should return the same result. However,
-                                            determinism cannot be totally guaranteed.
-                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
-                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        return_prompt : typing.Optional[bool]
+            The prompt is returned in the `prompt` response field when this is enabled.
 
-            - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        tools : typing.Optional[typing.Sequence[Tool]]
+            A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
-                                                         Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
-                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                        Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
-                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        tool_results : typing.Optional[typing.Sequence[ToolResult]]
+            A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
+            Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
-                                                    any pre-processing.
-                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
+            ```
+            tool_results = [
+              {
+                "call": {
+                  "name": <tool name>,
+                  "parameters": {
+                    <param name>: <param value>
+                  }
+                },
+                "outputs": [{
+                  <key>: <value>
+                }]
+              },
+              ...
+            ]
+            ```
+            **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
-            - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
+        force_single_step : typing.Optional[bool]
+            Forces the chat to be single step. Defaults to `false`.
 
-                                                             When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
-                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - tool_results: typing.Optional[typing.Sequence[ToolResult]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
-                                                                          Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+        Yields
+        ------
+        typing.Iterator[StreamedChatResponse]
 
-                                                                          **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
-                                                                          ```
-                                                                          tool_results = [
-                                                                            {
-                                                                              "call": {
-                                                                                "name": <tool name>,
-                                                                                "parameters": {
-                                                                                  <param name>: <param value>
-                                                                                }
-                                                                              },
-                                                                              "outputs": [{
-                                                                                <key>: <value>
-                                                                              }]
-                                                                            },
-                                                                            ...
-                                                                          ]
-                                                                          ```
-                                                                          **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
-                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere import (
             ChatConnector,
             ChatStreamRequestConnectorsSearchOptions,
             Message_Chatbot,
             Tool,
             ToolCall,
             ToolParameterDefinitionsValue,
@@ -314,15 +383,15 @@
         )
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.chat_stream(
+        response = client.chat_stream(
             message="string",
             model="string",
             preamble="string",
             chat_history=[
                 Message_Chatbot(
                     message="string",
                     tool_calls=[
@@ -340,15 +409,15 @@
                     id="string",
                     user_access_token="string",
                     continue_on_failure=True,
                     options={"string": {"key": "value"}},
                 )
             ],
             search_queries_only=True,
-            documents=[{{"key": "value"}: {"key": "value"}}],
+            documents=[{"string": {"key": "value"}}],
             citation_quality="fast",
             temperature=1.1,
             max_tokens=1,
             max_input_tokens=1,
             k=1,
             p=1.1,
             seed=1.1,
@@ -382,18 +451,20 @@
                     call=ToolCall(
                         name="string",
                         parameters={"string": {"key": "value"}},
                     ),
                     outputs=[{"string": {"key": "value"}}],
                 )
             ],
-            enable_multi_step=True,
+            force_single_step=True,
         )
+        for chunk in response:
+            yield chunk
         """
-        _request: typing.Dict[str, typing.Any] = {"message": message, "stream": True}
+        _request: typing.Dict[str, typing.Any] = {"message": message}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
         if chat_history is not OMIT:
             _request["chat_history"] = chat_history
         if conversation_id is not OMIT:
@@ -430,19 +501,23 @@
             _request["raw_prompting"] = raw_prompting
         if return_prompt is not OMIT:
             _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
+        if force_single_step is not OMIT:
+            _request["force_single_step"] = force_single_step
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -499,182 +574,240 @@
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
         return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ToolResult]] = OMIT,
+        force_single_step: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
-        Parameters:
-            - message: str. Text input for the model to respond to.
-                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        Parameters
+        ----------
+        message : str
+            Text input for the model to respond to.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        model : typing.Optional[str]
+            Defaults to `command-r-plus`.
+
+            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+            Compatible Deployments: Cohere Platform, Private Deployments
+
+
+        preamble : typing.Optional[str]
+            When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+
+            The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        chat_history : typing.Optional[typing.Sequence[Message]]
+            A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+
+            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+
+            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        conversation_id : typing.Optional[str]
+            An alternative to `chat_history`.
+
+            Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+            Compatible Deployments: Cohere Platform
 
-            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
-                                           The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
-                                           Compatible Deployments: Cohere Platform, Private Deployments
+        prompt_truncation : typing.Optional[ChatRequestPromptTruncation]
+            Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
-            - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+            Dictates how the prompt will be constructed.
 
-                                              The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
-                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
-            - chat_history: typing.Optional[typing.Sequence[Message]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+            With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
-                                                                       Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+            With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+            Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
-                                                                       The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
-                                                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
+        connectors : typing.Optional[typing.Sequence[ChatConnector]]
+            Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
-                                                     Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
-                                                     Compatible Deployments: Cohere Platform
+            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+            Compatible Deployments: Cohere Platform
 
-            - prompt_truncation: typing.Optional[ChatRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
-                                                                               Dictates how the prompt will be constructed.
+        search_queries_only : typing.Optional[bool]
+            Defaults to `false`.
 
-                                                                               With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+            When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                               With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
-                                                                               With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
-                                                                               Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+        documents : typing.Optional[typing.Sequence[ChatDocument]]
+            A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
-            - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
+            Example:
+            `[
+              { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
+              { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
+            ]`
 
-                                                                           When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
-                                                                           Compatible Deployments: Cohere Platform
+            Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-            - search_queries_only: typing.Optional[bool]. Defaults to `false`.
+            Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-                                                          When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
-                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
-            - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
+            An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         Example:
-                                                                         `[
-                                                                           { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
-                                                                           { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
-                                                                         ]`
+            See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-                                                                         Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
+        citation_quality : typing.Optional[ChatRequestCitationQuality]
+            Defaults to `"accurate"`.
 
-                                                                         An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
+            Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
-                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        temperature : typing.Optional[float]
+            Defaults to `0.3`.
 
-            - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
-                                                                             Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
-                                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Randomness can be further maximized by increasing the  value of the `p` parameter.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - temperature: typing.Optional[float]. Defaults to `0.3`.
 
-                                                   A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                   Randomness can be further maximized by increasing the  value of the `p` parameter.
-                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
-                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        max_input_tokens : typing.Optional[int]
+            The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
-            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+            Input will be truncated according to the `prompt_truncation` parameter.
+            Compatible Deployments: Cohere Platform
 
-                                                      Input will be truncated according to the `prompt_truncation` parameter.
-                                                      Compatible Deployments: Cohere Platform
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
-                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
-                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
-                                            deterministically, such that repeated requests with the same
-                                            seed and parameters should return the same result. However,
-                                            determinism cannot be totally guaranteed.
-                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
-                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens
+            deterministically, such that repeated requests with the same
+            seed and parameters should return the same result. However,
+            determinism cannot be totally guaranteed.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                         Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
-                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                        Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
-                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
-                                                    any pre-processing.
-                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        frequency_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
-                                                             When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
-                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-            - tool_results: typing.Optional[typing.Sequence[ToolResult]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
-                                                                          Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+            Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                          **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
-                                                                          ```
-                                                                          tool_results = [
-                                                                            {
-                                                                              "call": {
-                                                                                "name": <tool name>,
-                                                                                "parameters": {
-                                                                                  <param name>: <param value>
-                                                                                }
-                                                                              },
-                                                                              "outputs": [{
-                                                                                <key>: <value>
-                                                                              }]
-                                                                            },
-                                                                            ...
-                                                                          ]
-                                                                          ```
-                                                                          **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
-                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without
+            any pre-processing.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        return_prompt : typing.Optional[bool]
+            The prompt is returned in the `prompt` response field when this is enabled.
+
+        tools : typing.Optional[typing.Sequence[Tool]]
+            A list of available tools (functions) that the model may suggest invoking before producing a text response.
+
+            When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        tool_results : typing.Optional[typing.Sequence[ToolResult]]
+            A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
+            Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+
+            **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
+            ```
+            tool_results = [
+              {
+                "call": {
+                  "name": <tool name>,
+                  "parameters": {
+                    <param name>: <param value>
+                  }
+                },
+                "outputs": [{
+                  <key>: <value>
+                }]
+              },
+              ...
+            ]
+            ```
+            **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        force_single_step : typing.Optional[bool]
+            Forces the chat to be single step. Defaults to `false`.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NonStreamedChatResponse
+
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.chat(
             message="Can you give me a global market overview of solar panels?",
             prompt_truncation="OFF",
             temperature=0.3,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"message": message, "stream": False}
+        _request: typing.Dict[str, typing.Any] = {"message": message}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
         if chat_history is not OMIT:
             _request["chat_history"] = chat_history
         if conversation_id is not OMIT:
@@ -711,19 +844,23 @@
             _request["raw_prompting"] = raw_prompting
         if return_prompt is not OMIT:
             _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
+        if force_single_step is not OMIT:
+            _request["force_single_step"] = force_single_step
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -777,77 +914,114 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates realistic text conditioned on a given input.
 
-        Parameters:
-            - prompt: str. The input text that serves as the starting point for generating the response.
-                           Note: The prompt will be pre-processed and modified before reaching the model.
+        Parameters
+        ----------
+        prompt : str
+            The input text that serves as the starting point for generating the response.
+            Note: The prompt will be pre-processed and modified before reaching the model.
 
-            - model: typing.Optional[str]. The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
-                                           Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
-            - num_generations: typing.Optional[int]. The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+        model : typing.Optional[str]
+            The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
+            Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
 
-                                                This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+        num_generations : typing.Optional[int]
+            The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-                                                Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - truncate: typing.Optional[GenerateStreamRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
-                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
 
-                                                                        If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - temperature: typing.Optional[float]. A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
-                                                   Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
+            Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-            - preset: typing.Optional[str]. Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.ai/playground/generate).
-                                            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
+        truncate : typing.Optional[GenerateStreamRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-            - end_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
+        temperature : typing.Optional[float]
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
+            Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - frequency_penalty: typing.Optional[float]. Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-                                                         Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        preset : typing.Optional[str]
+            Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.com/playground/generate).
+            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                        Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+        end_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-                                                        Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
 
-            - return_likelihoods: typing.Optional[GenerateStreamRequestReturnLikelihoods]. One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
 
-                                                                                           If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
 
-                                                                                           If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+
+        frequency_penalty : typing.Optional[float]
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+
+
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+
+            Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+
+
+        return_likelihoods : typing.Optional[GenerateStreamRequestReturnLikelihoods]
+            One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+
+            If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
+
+            If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
+
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without any pre-processing.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.Iterator[GenerateStreamedResponse]
+
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        client.generate_stream(
+        response = client.generate_stream(
             prompt="string",
             model="string",
             num_generations=1,
             max_tokens=1,
             truncate="NONE",
             temperature=1.1,
             seed=1.1,
@@ -857,16 +1031,18 @@
             k=1,
             p=1.1,
             frequency_penalty=1.1,
             presence_penalty=1.1,
             return_likelihoods="GENERATION",
             raw_prompting=True,
         )
+        for chunk in response:
+            yield chunk
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": True}
+        _request: typing.Dict[str, typing.Any] = {"prompt": prompt}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if truncate is not OMIT:
@@ -890,18 +1066,20 @@
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if return_likelihoods is not OMIT:
             _request["return_likelihoods"] = return_likelihoods
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
         with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -968,81 +1146,118 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates realistic text conditioned on a given input.
 
-        Parameters:
-            - prompt: str. The input text that serves as the starting point for generating the response.
-                           Note: The prompt will be pre-processed and modified before reaching the model.
+        Parameters
+        ----------
+        prompt : str
+            The input text that serves as the starting point for generating the response.
+            Note: The prompt will be pre-processed and modified before reaching the model.
+
+
+        model : typing.Optional[str]
+            The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
+            Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+
+        num_generations : typing.Optional[int]
+            The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
+
+
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+
+            This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+
+            Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
+
+
+        truncate : typing.Optional[GenerateRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
+
+        temperature : typing.Optional[float]
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
+            Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
 
-            - model: typing.Optional[str]. The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
-                                           Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
-            - num_generations: typing.Optional[int]. The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-                                                This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+        preset : typing.Optional[str]
+            Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.com/playground/generate).
+            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
 
-                                                Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - truncate: typing.Optional[GenerateRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+        end_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-                                                                  Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
 
-                                                                  If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - temperature: typing.Optional[float]. A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
-                                                   Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-            - preset: typing.Optional[str]. Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.ai/playground/generate).
-                                            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - end_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
+        frequency_penalty : typing.Optional[float]
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - frequency_penalty: typing.Optional[float]. Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                         Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+            Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
 
-                                                        Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
-                                                        Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        return_likelihoods : typing.Optional[GenerateRequestReturnLikelihoods]
+            One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
 
-            - return_likelihoods: typing.Optional[GenerateRequestReturnLikelihoods]. One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+            If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
 
-                                                                                     If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
+            If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
 
-                                                                                     If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without any pre-processing.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Generation
+
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.generate(
             prompt="Please explain to me how LLMs work",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": False}
+        _request: typing.Dict[str, typing.Any] = {"prompt": prompt}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if truncate is not OMIT:
@@ -1066,18 +1281,20 @@
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if return_likelihoods is not OMIT:
             _request["return_likelihoods"] = return_likelihoods
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1128,47 +1345,63 @@
         """
         This endpoint returns text embeddings. An embedding is a list of floating point numbers that captures semantic information about the text that it represents.
 
         Embeddings can be used to create text classifiers as well as empower semantic search. To learn more about embeddings, see the embedding page.
 
         If you want to learn more how to use the embedding model, have a look at the [Semantic Search Guide](/docs/semantic-search).
 
-        Parameters:
-            - texts: typing.Sequence[str]. An array of strings for the model to embed. Maximum number of texts per call is `96`. We recommend reducing the length of each text to be under `512` tokens for optimal quality.
+        Parameters
+        ----------
+        texts : typing.Sequence[str]
+            An array of strings for the model to embed. Maximum number of texts per call is `96`. We recommend reducing the length of each text to be under `512` tokens for optimal quality.
+
+        model : typing.Optional[str]
+            Defaults to embed-english-v2.0
+
+            The identifier of the model. Smaller "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+
+            Available models and corresponding embedding dimensions:
 
-            - model: typing.Optional[str]. Defaults to embed-english-v2.0
+            * `embed-english-v3.0`  1024
+            * `embed-multilingual-v3.0`  1024
+            * `embed-english-light-v3.0`  384
+            * `embed-multilingual-light-v3.0`  384
 
-                                           The identifier of the model. Smaller "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+            * `embed-english-v2.0`  4096
+            * `embed-english-light-v2.0`  1024
+            * `embed-multilingual-v2.0`  768
 
-                                           Available models and corresponding embedding dimensions:
+        input_type : typing.Optional[EmbedInputType]
 
-                                           * `embed-english-v3.0`  1024
-                                           * `embed-multilingual-v3.0`  1024
-                                           * `embed-english-light-v3.0`  384
-                                           * `embed-multilingual-light-v3.0`  384
+        embedding_types : typing.Optional[typing.Sequence[EmbeddingType]]
+            Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-                                           * `embed-english-v2.0`  4096
-                                           * `embed-english-light-v2.0`  1024
-                                           * `embed-multilingual-v2.0`  768
-            - input_type: typing.Optional[EmbedInputType].
+            * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+            * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+            * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+            * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+            * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
 
-            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
+        truncate : typing.Optional[EmbedRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
-                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
-                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
-                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
-                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
-            - truncate: typing.Optional[EmbedRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-                                                               Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
 
-                                                               If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        EmbedResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.embed(
@@ -1185,18 +1418,20 @@
         if input_type is not OMIT:
             _request["input_type"] = input_type
         if embedding_types is not OMIT:
             _request["embedding_types"] = embedding_types
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1233,47 +1468,65 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def rerank(
         self,
         *,
-        model: typing.Optional[str] = OMIT,
         query: str,
         documents: typing.Sequence[RerankRequestDocumentsItem],
+        model: typing.Optional[str] = OMIT,
         top_n: typing.Optional[int] = OMIT,
         rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         return_documents: typing.Optional[bool] = OMIT,
         max_chunks_per_doc: typing.Optional[int] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankResponse:
         """
         This endpoint takes in a query and a list of texts and produces an ordered array with each text assigned a relevance score.
 
-        Parameters:
-            - model: typing.Optional[str]. The identifier of the model to use, one of : `rerank-english-v3.0`, `rerank-multilingual-v3.0`, `rerank-english-v2.0`, `rerank-multilingual-v2.0`
+        Parameters
+        ----------
+        query : str
+            The search query
+
+        documents : typing.Sequence[RerankRequestDocumentsItem]
+            A list of document objects or strings to rerank.
+            If a document is provided the text fields is required and all other fields will be preserved in the response.
+
+            The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
 
-            - query: str. The search query
+            We recommend a maximum of 1,000 documents for optimal endpoint performance.
 
-            - documents: typing.Sequence[RerankRequestDocumentsItem]. A list of document objects or strings to rerank.
-                                                                      If a document is provided the text fields is required and all other fields will be preserved in the response.
+        model : typing.Optional[str]
+            The identifier of the model to use, one of : `rerank-english-v3.0`, `rerank-multilingual-v3.0`, `rerank-english-v2.0`, `rerank-multilingual-v2.0`
 
-                                                                      The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
+        top_n : typing.Optional[int]
+            The number of most relevant documents or indices to return, defaults to the length of the documents
 
-                                                                      We recommend a maximum of 1,000 documents for optimal endpoint performance.
-            - top_n: typing.Optional[int]. The number of most relevant documents or indices to return, defaults to the length of the documents
+        rank_fields : typing.Optional[typing.Sequence[str]]
+            If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
 
-            - rank_fields: typing.Optional[typing.Sequence[str]]. If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
+        return_documents : typing.Optional[bool]
+            - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
+            - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
 
-            - return_documents: typing.Optional[bool]. - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
-                                                       - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
-            - max_chunks_per_doc: typing.Optional[int]. The maximum number of chunks to produce internally from a document
+        max_chunks_per_doc : typing.Optional[int]
+            The maximum number of chunks to produce internally from a document
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RerankResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.rerank(
@@ -1295,18 +1548,20 @@
         if rank_fields is not OMIT:
             _request["rank_fields"] = rank_fields
         if return_documents is not OMIT:
             _request["return_documents"] = return_documents
         if max_chunks_per_doc is not OMIT:
             _request["max_chunks_per_doc"] = max_chunks_per_doc
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1346,29 +1601,46 @@
         truncate: typing.Optional[ClassifyRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ClassifyResponse:
         """
         This endpoint makes a prediction about which label fits the specified text inputs best. To make a prediction, Classify uses the provided `examples` of text + label pairs as a reference.
         Note: [Fine-tuned models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
 
-        Parameters:
-            - inputs: typing.Sequence[str]. A list of up to 96 texts to be classified. Each one must be a non-empty string.
-                                            There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
-                                            Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
-            - examples: typing.Optional[typing.Sequence[ClassifyExample]]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
-                                                                           Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
-            - model: typing.Optional[str]. The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
-
-            - preset: typing.Optional[str]. The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.ai/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
-
-            - truncate: typing.Optional[ClassifyRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
-                                                                  Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
-                                                                  If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        inputs : typing.Sequence[str]
+            A list of up to 96 texts to be classified. Each one must be a non-empty string.
+            There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
+            Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
+
+        examples : typing.Optional[typing.Sequence[ClassifyExample]]
+            An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
+            Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
+
+        model : typing.Optional[str]
+            The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
+
+        preset : typing.Optional[str]
+            The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.com/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
+
+        truncate : typing.Optional[ClassifyRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ClassifyResponse
+            OK
+
+        Examples
+        --------
         from cohere import ClassifyExample
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -1424,18 +1696,20 @@
         if model is not OMIT:
             _request["model"] = model
         if preset is not OMIT:
             _request["preset"] = preset
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "classify"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "classify"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1488,31 +1762,47 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates a summary in English for a given text.
 
-        Parameters:
-            - text: str. The text to generate a summary for. Can be up to 100,000 characters long. Currently the only supported language is English.
+        Parameters
+        ----------
+        text : str
+            The text to generate a summary for. Can be up to 100,000 characters long. Currently the only supported language is English.
+
+        length : typing.Optional[SummarizeRequestLength]
+            One of `short`, `medium`, `long`, or `auto` defaults to `auto`. Indicates the approximate length of the summary. If `auto` is selected, the best option will be picked based on the input text.
+
+        format : typing.Optional[SummarizeRequestFormat]
+            One of `paragraph`, `bullets`, or `auto`, defaults to `auto`. Indicates the style in which the summary will be delivered - in a free form paragraph or in bullet points. If `auto` is selected, the best option will be picked based on the input text.
 
-            - length: typing.Optional[SummarizeRequestLength]. One of `short`, `medium`, `long`, or `auto` defaults to `auto`. Indicates the approximate length of the summary. If `auto` is selected, the best option will be picked based on the input text.
+        model : typing.Optional[str]
+            The identifier of the model to generate the summary with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental). Smaller, "light" models are faster, while larger models will perform better.
 
-            - format: typing.Optional[SummarizeRequestFormat]. One of `paragraph`, `bullets`, or `auto`, defaults to `auto`. Indicates the style in which the summary will be delivered - in a free form paragraph or in bullet points. If `auto` is selected, the best option will be picked based on the input text.
+        extractiveness : typing.Optional[SummarizeRequestExtractiveness]
+            One of `low`, `medium`, `high`, or `auto`, defaults to `auto`. Controls how close to the original text the summary is. `high` extractiveness summaries will lean towards reusing sentences verbatim, while `low` extractiveness summaries will tend to paraphrase more. If `auto` is selected, the best option will be picked based on the input text.
 
-            - model: typing.Optional[str]. The identifier of the model to generate the summary with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental). Smaller, "light" models are faster, while larger models will perform better.
+        temperature : typing.Optional[float]
+            Ranges from 0 to 5. Controls the randomness of the output. Lower values tend to generate more “predictable” output, while higher values tend to generate more “creative” output. The sweet spot is typically between 0 and 1.
 
-            - extractiveness: typing.Optional[SummarizeRequestExtractiveness]. One of `low`, `medium`, `high`, or `auto`, defaults to `auto`. Controls how close to the original text the summary is. `high` extractiveness summaries will lean towards reusing sentences verbatim, while `low` extractiveness summaries will tend to paraphrase more. If `auto` is selected, the best option will be picked based on the input text.
+        additional_command : typing.Optional[str]
+            A free-form instruction for modifying how the summaries get generated. Should complete the sentence "Generate a summary _". Eg. "focusing on the next steps" or "written by Yoda"
 
-            - temperature: typing.Optional[float]. Ranges from 0 to 5. Controls the randomness of the output. Lower values tend to generate more “predictable” output, while higher values tend to generate more “creative” output. The sweet spot is typically between 0 and 1.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - additional_command: typing.Optional[str]. A free-form instruction for modifying how the summaries get generated. Should complete the sentence "Generate a summary _". Eg. "focusing on the next steps" or "written by Yoda"
+        Returns
+        -------
+        SummarizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.summarize(
@@ -1529,18 +1819,20 @@
         if extractiveness is not OMIT:
             _request["extractiveness"] = extractiveness
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if additional_command is not OMIT:
             _request["additional_command"] = additional_command
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "summarize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "summarize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1572,37 +1864,50 @@
 
     def tokenize(
         self, *, text: str, model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> TokenizeResponse:
         """
         This endpoint splits input text into smaller units called tokens using byte-pair encoding (BPE). To learn more about tokenization and byte pair encoding, see the tokens page.
 
-        Parameters:
-            - text: str. The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
-
-            - model: str. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+        Parameters
+        ----------
+        text : str
+            The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
+
+        model : str
+            An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        TokenizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.tokenize(
             text="tokenize me! :D",
             model="command",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"text": text, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"text": text, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1642,37 +1947,50 @@
 
     def detokenize(
         self, *, tokens: typing.Sequence[int], model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> DetokenizeResponse:
         """
         This endpoint takes tokens using byte-pair encoding and returns their text representation. To learn more about tokenization and byte pair encoding, see the tokens page.
 
-        Parameters:
-            - tokens: typing.Sequence[int]. The list of tokens to be detokenized.
-
-            - model: str. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+        Parameters
+        ----------
+        tokens : typing.Sequence[int]
+            The list of tokens to be detokenized.
+
+        model : str
+            An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DetokenizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.detokenize(
             tokens=[10104, 12221, 1315, 34, 1420, 69],
             model="command",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"tokens": tokens, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"tokens": tokens, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1702,30 +2020,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def check_api_key(self, *, request_options: typing.Optional[RequestOptions] = None) -> CheckApiKeyResponse:
         """
         Checks that the api key in the Authorization header is valid and active
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CheckApiKeyResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.check_api_key()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -1753,31 +2082,41 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
 
 class AsyncBaseCohere:
     """
     Use this class to access the different functions within the SDK. You can instantiate any number of clients with different configuration that will propogate to these functions.
 
-    Parameters:
-        - base_url: typing.Optional[str]. The base url to use for requests from the client.
+    Parameters
+    ----------
+    base_url : typing.Optional[str]
+        The base url to use for requests from the client.
 
-        - environment: ClientEnvironment. The environment to use for requests from the client. from .environment import ClientEnvironment
+    environment : ClientEnvironment
+        The environment to use for requests from the client. from .environment import ClientEnvironment
 
-                                          Defaults to ClientEnvironment.PRODUCTION
 
-        - client_name: typing.Optional[str].
 
-        - token: typing.Optional[typing.Union[str, typing.Callable[[], str]]].
+        Defaults to ClientEnvironment.PRODUCTION
 
-        - timeout: typing.Optional[float]. The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
 
-        - follow_redirects: typing.Optional[bool]. Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
 
-        - httpx_client: typing.Optional[httpx.AsyncClient]. The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
-    ---
+    client_name : typing.Optional[str]
+    token : typing.Optional[typing.Union[str, typing.Callable[[], str]]]
+    timeout : typing.Optional[float]
+        The timeout to be used, in seconds, for requests by default the timeout is 60 seconds, unless a custom httpx client is used, in which case a default is not set.
+
+    follow_redirects : typing.Optional[bool]
+        Whether the default httpx client follows redirects or not, this is irrelevant if a custom httpx client is passed in.
+
+    httpx_client : typing.Optional[httpx.AsyncClient]
+        The httpx client to use for making requests, a preconfigured client is used by default, however this is useful should you want to pass in any custom httpx configuration.
+
+    Examples
+    --------
     from cohere.client import AsyncClient
 
     client = AsyncClient(
         client_name="YOUR_CLIENT_NAME",
         token="YOUR_TOKEN",
     )
     """
@@ -1786,15 +2125,15 @@
         self,
         *,
         base_url: typing.Optional[str] = None,
         environment: ClientEnvironment = ClientEnvironment.PRODUCTION,
         client_name: typing.Optional[str] = None,
         token: typing.Optional[typing.Union[str, typing.Callable[[], str]]] = os.getenv("CO_API_KEY"),
         timeout: typing.Optional[float] = None,
-        follow_redirects: typing.Optional[bool] = None,
+        follow_redirects: typing.Optional[bool] = True,
         httpx_client: typing.Optional[httpx.AsyncClient] = None,
     ):
         _defaulted_timeout = timeout if timeout is not None else 300 if httpx_client is None else None
         if token is None:
             raise ApiError(body="The client must be instantiated be either passing in token or setting CO_API_KEY")
         self._client_wrapper = AsyncClientWrapper(
             base_url=_get_base_url(base_url=base_url, environment=environment),
@@ -1835,169 +2174,227 @@
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
         return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ToolResult]] = OMIT,
+        force_single_step: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> typing.AsyncIterator[StreamedChatResponse]:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
-        Parameters:
-            - message: str. Text input for the model to respond to.
-                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        Parameters
+        ----------
+        message : str
+            Text input for the model to respond to.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        model : typing.Optional[str]
+            Defaults to `command-r-plus`.
+
+            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+            Compatible Deployments: Cohere Platform, Private Deployments
+
+
+        preamble : typing.Optional[str]
+            When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+
+            The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        chat_history : typing.Optional[typing.Sequence[Message]]
+            A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+
+            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+
+            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        conversation_id : typing.Optional[str]
+            An alternative to `chat_history`.
+
+            Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+            Compatible Deployments: Cohere Platform
+
+
+        prompt_truncation : typing.Optional[ChatStreamRequestPromptTruncation]
+            Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
+
+            Dictates how the prompt will be constructed.
+
+            With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+
+            With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
+
+            With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+            Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+
+
+        connectors : typing.Optional[typing.Sequence[ChatConnector]]
+            Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
+
+            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+            Compatible Deployments: Cohere Platform
+
+
+        search_queries_only : typing.Optional[bool]
+            Defaults to `false`.
+
+            When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
 
-            - model: typing.Optional[str]. Defaults to `command-r-plus`.
+        documents : typing.Optional[typing.Sequence[ChatDocument]]
+            A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
-                                           The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
-                                           Compatible Deployments: Cohere Platform, Private Deployments
+            Example:
+            `[
+              { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
+              { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
+            ]`
 
-            - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+            Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-                                              The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
-                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-            - chat_history: typing.Optional[typing.Sequence[Message]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+            An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
-                                                                       Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+            An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                       The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
-                                                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
 
-                                                     Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
-                                                     Compatible Deployments: Cohere Platform
+        citation_quality : typing.Optional[ChatStreamRequestCitationQuality]
+            Defaults to `"accurate"`.
 
-            - prompt_truncation: typing.Optional[ChatStreamRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
+            Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                                     Dictates how the prompt will be constructed.
 
-                                                                                     With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+        temperature : typing.Optional[float]
+            Defaults to `0.3`.
 
-                                                                                     With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
-                                                                                     With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
-                                                                                     Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+            Randomness can be further maximized by increasing the  value of the `p` parameter.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
-                                                                           When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
-                                                                           Compatible Deployments: Cohere Platform
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - search_queries_only: typing.Optional[bool]. Defaults to `false`.
 
-                                                          When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
-                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        max_input_tokens : typing.Optional[int]
+            The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
-            - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
+            Input will be truncated according to the `prompt_truncation` parameter.
+            Compatible Deployments: Cohere Platform
 
-                                                                         Example:
-                                                                         `[
-                                                                           { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
-                                                                           { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
-                                                                         ]`
 
-                                                                         Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-                                                                         An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
-                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens
+            deterministically, such that repeated requests with the same
+            seed and parameters should return the same result. However,
+            determinism cannot be totally guaranteed.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - citation_quality: typing.Optional[ChatStreamRequestCitationQuality]. Defaults to `"accurate"`.
 
-                                                                                   Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
-                                                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - temperature: typing.Optional[float]. Defaults to `0.3`.
 
-                                                   A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
+        frequency_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                   Randomness can be further maximized by increasing the  value of the `p` parameter.
-                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
-                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                      Input will be truncated according to the `prompt_truncation` parameter.
-                                                      Compatible Deployments: Cohere Platform
+            Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
-                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
-                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without
+            any pre-processing.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
-                                            deterministically, such that repeated requests with the same
-                                            seed and parameters should return the same result. However,
-                                            determinism cannot be totally guaranteed.
-                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
-                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        return_prompt : typing.Optional[bool]
+            The prompt is returned in the `prompt` response field when this is enabled.
 
-            - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        tools : typing.Optional[typing.Sequence[Tool]]
+            A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
-                                                         Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
-                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                        Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
-                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        tool_results : typing.Optional[typing.Sequence[ToolResult]]
+            A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
+            Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
-                                                    any pre-processing.
-                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
+            ```
+            tool_results = [
+              {
+                "call": {
+                  "name": <tool name>,
+                  "parameters": {
+                    <param name>: <param value>
+                  }
+                },
+                "outputs": [{
+                  <key>: <value>
+                }]
+              },
+              ...
+            ]
+            ```
+            **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
 
-            - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
+        force_single_step : typing.Optional[bool]
+            Forces the chat to be single step. Defaults to `false`.
 
-                                                             When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
-                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - tool_results: typing.Optional[typing.Sequence[ToolResult]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
-                                                                          Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+        Yields
+        ------
+        typing.AsyncIterator[StreamedChatResponse]
 
-                                                                          **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
-                                                                          ```
-                                                                          tool_results = [
-                                                                            {
-                                                                              "call": {
-                                                                                "name": <tool name>,
-                                                                                "parameters": {
-                                                                                  <param name>: <param value>
-                                                                                }
-                                                                              },
-                                                                              "outputs": [{
-                                                                                <key>: <value>
-                                                                              }]
-                                                                            },
-                                                                            ...
-                                                                          ]
-                                                                          ```
-                                                                          **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
-                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere import (
             ChatConnector,
             ChatStreamRequestConnectorsSearchOptions,
             Message_Chatbot,
             Tool,
             ToolCall,
             ToolParameterDefinitionsValue,
@@ -2005,15 +2402,15 @@
         )
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.chat_stream(
+        response = await client.chat_stream(
             message="string",
             model="string",
             preamble="string",
             chat_history=[
                 Message_Chatbot(
                     message="string",
                     tool_calls=[
@@ -2031,15 +2428,15 @@
                     id="string",
                     user_access_token="string",
                     continue_on_failure=True,
                     options={"string": {"key": "value"}},
                 )
             ],
             search_queries_only=True,
-            documents=[{{"key": "value"}: {"key": "value"}}],
+            documents=[{"string": {"key": "value"}}],
             citation_quality="fast",
             temperature=1.1,
             max_tokens=1,
             max_input_tokens=1,
             k=1,
             p=1.1,
             seed=1.1,
@@ -2073,18 +2470,20 @@
                     call=ToolCall(
                         name="string",
                         parameters={"string": {"key": "value"}},
                     ),
                     outputs=[{"string": {"key": "value"}}],
                 )
             ],
-            enable_multi_step=True,
+            force_single_step=True,
         )
+        async for chunk in response:
+            yield chunk
         """
-        _request: typing.Dict[str, typing.Any] = {"message": message, "stream": True}
+        _request: typing.Dict[str, typing.Any] = {"message": message}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
         if chat_history is not OMIT:
             _request["chat_history"] = chat_history
         if conversation_id is not OMIT:
@@ -2121,19 +2520,23 @@
             _request["raw_prompting"] = raw_prompting
         if return_prompt is not OMIT:
             _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
+        if force_single_step is not OMIT:
+            _request["force_single_step"] = force_single_step
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -2190,182 +2593,240 @@
         stop_sequences: typing.Optional[typing.Sequence[str]] = OMIT,
         frequency_penalty: typing.Optional[float] = OMIT,
         presence_penalty: typing.Optional[float] = OMIT,
         raw_prompting: typing.Optional[bool] = OMIT,
         return_prompt: typing.Optional[bool] = OMIT,
         tools: typing.Optional[typing.Sequence[Tool]] = OMIT,
         tool_results: typing.Optional[typing.Sequence[ToolResult]] = OMIT,
+        force_single_step: typing.Optional[bool] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> NonStreamedChatResponse:
         """
         Generates a text response to a user message.
         To learn how to use Chat with Streaming and RAG follow [this guide](https://docs.cohere.com/docs/cochat-beta#various-ways-of-using-the-chat-endpoint).
 
-        Parameters:
-            - message: str. Text input for the model to respond to.
-                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        Parameters
+        ----------
+        message : str
+            Text input for the model to respond to.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        model : typing.Optional[str]
+            Defaults to `command-r-plus`.
+
+            The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
+            Compatible Deployments: Cohere Platform, Private Deployments
+
+
+        preamble : typing.Optional[str]
+            When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+
+            The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        chat_history : typing.Optional[typing.Sequence[Message]]
+            A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+
+            Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+
+            The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        conversation_id : typing.Optional[str]
+            An alternative to `chat_history`.
+
+            Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
+            Compatible Deployments: Cohere Platform
 
-            - model: typing.Optional[str]. Defaults to `command-r-plus`.
 
-                                           The name of a compatible [Cohere model](https://docs.cohere.com/docs/models) or the ID of a [fine-tuned](https://docs.cohere.com/docs/chat-fine-tuning) model.
-                                           Compatible Deployments: Cohere Platform, Private Deployments
+        prompt_truncation : typing.Optional[ChatRequestPromptTruncation]
+            Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
-            - preamble: typing.Optional[str]. When specified, the default Cohere preamble will be replaced with the provided one. Preambles are a part of the prompt used to adjust the model's overall behavior and conversation style, and use the `SYSTEM` role.
+            Dictates how the prompt will be constructed.
 
-                                              The `SYSTEM` role is also used for the contents of the optional `chat_history=` parameter. When used with the `chat_history=` parameter it adds content throughout a conversation. Conversely, when used with the `preamble=` parameter it adds content at the start of the conversation only.
-                                              Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
 
-            - chat_history: typing.Optional[typing.Sequence[Message]]. A list of previous messages between the user and the model, giving the model conversational context for responding to the user's `message`.
+            With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
-                                                                       Each item represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
+            With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
+            Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
 
-                                                                       The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
-                                                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - conversation_id: typing.Optional[str]. An alternative to `chat_history`.
+        connectors : typing.Optional[typing.Sequence[ChatConnector]]
+            Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
 
-                                                     Providing a `conversation_id` creates or resumes a persisted conversation with the specified ID. The ID can be any non empty string.
-                                                     Compatible Deployments: Cohere Platform
+            When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
+            Compatible Deployments: Cohere Platform
 
-            - prompt_truncation: typing.Optional[ChatRequestPromptTruncation]. Defaults to `AUTO` when `connectors` are specified and `OFF` in all other cases.
 
-                                                                               Dictates how the prompt will be constructed.
+        search_queries_only : typing.Optional[bool]
+            Defaults to `false`.
 
-                                                                               With `prompt_truncation` set to "AUTO", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be changed and ranked by relevance.
+            When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                               With `prompt_truncation` set to "AUTO_PRESERVE_ORDER", some elements from `chat_history` and `documents` will be dropped in an attempt to construct a prompt that fits within the model's context length limit. During this process the order of the documents and chat history will be preserved as they are inputted into the API.
 
-                                                                               With `prompt_truncation` set to "OFF", no elements will be dropped. If the sum of the inputs exceeds the model's context length limit, a `TooManyTokens` error will be returned.
-                                                                               Compatible Deployments: Cohere Platform Only AUTO_PRESERVE_ORDER: Azure, AWS Sagemaker, Private Deployments
+        documents : typing.Optional[typing.Sequence[ChatDocument]]
+            A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
 
-            - connectors: typing.Optional[typing.Sequence[ChatConnector]]. Accepts `{"id": "web-search"}`, and/or the `"id"` for a custom [connector](https://docs.cohere.com/docs/connectors), if you've [created](https://docs.cohere.com/docs/creating-and-deploying-a-connector) one.
+            Example:
+            `[
+              { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
+              { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
+            ]`
 
-                                                                           When specified, the model's reply will be enriched with information found by quering each of the connectors (RAG).
-                                                                           Compatible Deployments: Cohere Platform
+            Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-            - search_queries_only: typing.Optional[bool]. Defaults to `false`.
+            Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
 
-                                                          When `true`, the response will only contain a list of generated search queries, but no search will take place, and no reply from the model to the user's `message` will be generated.
-                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
 
-            - documents: typing.Optional[typing.Sequence[ChatDocument]]. A list of relevant documents that the model can cite to generate a more accurate reply. Each document is a string-string dictionary.
+            An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         Example:
-                                                                         `[
-                                                                           { "title": "Tall penguins", "text": "Emperor penguins are the tallest." },
-                                                                           { "title": "Penguin habitats", "text": "Emperor penguins only live in Antarctica." },
-                                                                         ]`
+            See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         Keys and values from each document will be serialized to a string and passed to the model. The resulting generation will include citations that reference some of these documents.
 
-                                                                         Some suggested keys are "text", "author", and "date". For better generation quality, it is recommended to keep the total word count of the strings in the dictionary to under 300 words.
+        citation_quality : typing.Optional[ChatRequestCitationQuality]
+            Defaults to `"accurate"`.
 
-                                                                         An `id` field (string) can be optionally supplied to identify the document in the citations. This field will not be passed to the model.
+            Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                         An `_excludes` field (array of strings) can be optionally supplied to omit some key-value pairs from being shown to the model. The omitted fields will still show up in the citation object. The "_excludes" field will not be passed to the model.
 
-                                                                         See ['Document Mode'](https://docs.cohere.com/docs/retrieval-augmented-generation-rag#document-mode) in the guide for more information.
-                                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        temperature : typing.Optional[float]
+            Defaults to `0.3`.
 
-            - citation_quality: typing.Optional[ChatRequestCitationQuality]. Defaults to `"accurate"`.
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
 
-                                                                             Dictates the approach taken to generating citations as part of the RAG flow by allowing the user to specify whether they want `"accurate"` results or `"fast"` results.
-                                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+            Randomness can be further maximized by increasing the  value of the `p` parameter.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - temperature: typing.Optional[float]. Defaults to `0.3`.
 
-                                                   A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations, and higher temperatures mean more random generations.
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                   Randomness can be further maximized by increasing the  value of the `p` parameter.
-                                                   Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
-                                                Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        max_input_tokens : typing.Optional[int]
+            The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
 
-            - max_input_tokens: typing.Optional[int]. The maximum number of input tokens to send to the model. If not specified, `max_input_tokens` is the model's context length limit minus a small buffer.
+            Input will be truncated according to the `prompt_truncation` parameter.
+            Compatible Deployments: Cohere Platform
 
-                                                      Input will be truncated according to the `prompt_truncation` parameter.
-                                                      Compatible Deployments: Cohere Platform
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
-                                       Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
-                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens
-                                            deterministically, such that repeated requests with the same
-                                            seed and parameters should return the same result. However,
-                                            determinism cannot be totally guaranteed.
-                                            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
-                                                                     Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - frequency_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens
+            deterministically, such that repeated requests with the same
+            seed and parameters should return the same result. However,
+            determinism cannot be totally guaranteed.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                         Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
-                                                         Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            A list of up to 5 strings that the model will use to stop generation. If the model generates a string that matches any of the strings in the list, it will stop generating tokens and return the generated text up to that point not including the stop sequence.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                        Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
-                                                        Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without
-                                                    any pre-processing.
-                                                    Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        frequency_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-            - return_prompt: typing.Optional[bool]. The prompt is returned in the `prompt` response field when this is enabled.
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - tools: typing.Optional[typing.Sequence[Tool]]. A list of available tools (functions) that the model may suggest invoking before producing a text response.
 
-                                                             When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
-                                                             Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-            - tool_results: typing.Optional[typing.Sequence[ToolResult]]. A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
-                                                                          Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+            Used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-                                                                          **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
-                                                                          ```
-                                                                          tool_results = [
-                                                                            {
-                                                                              "call": {
-                                                                                "name": <tool name>,
-                                                                                "parameters": {
-                                                                                  <param name>: <param value>
-                                                                                }
-                                                                              },
-                                                                              "outputs": [{
-                                                                                <key>: <value>
-                                                                              }]
-                                                                            },
-                                                                            ...
-                                                                          ]
-                                                                          ```
-                                                                          **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
-                                                                          Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without
+            any pre-processing.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        return_prompt : typing.Optional[bool]
+            The prompt is returned in the `prompt` response field when this is enabled.
+
+        tools : typing.Optional[typing.Sequence[Tool]]
+            A list of available tools (functions) that the model may suggest invoking before producing a text response.
+
+            When `tools` is passed (without `tool_results`), the `text` field in the response will be `""` and the `tool_calls` field in the response will be populated with a list of tool calls that need to be made. If no calls need to be made, the `tool_calls` array will be empty.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        tool_results : typing.Optional[typing.Sequence[ToolResult]]
+            A list of results from invoking tools recommended by the model in the previous chat turn. Results are used to produce a text response and will be referenced in citations. When using `tool_results`, `tools` must be passed as well.
+            Each tool_result contains information about how it was invoked, as well as a list of outputs in the form of dictionaries.
+
+            **Note**: `outputs` must be a list of objects. If your tool returns a single object (eg `{"status": 200}`), make sure to wrap it in a list.
+            ```
+            tool_results = [
+              {
+                "call": {
+                  "name": <tool name>,
+                  "parameters": {
+                    <param name>: <param value>
+                  }
+                },
+                "outputs": [{
+                  <key>: <value>
+                }]
+              },
+              ...
+            ]
+            ```
+            **Note**: Chat calls with `tool_results` should not be included in the Chat history to avoid duplication of the message text.
+            Compatible Deployments: Cohere Platform, Azure, AWS Sagemaker, Private Deployments
+
+
+        force_single_step : typing.Optional[bool]
+            Forces the chat to be single step. Defaults to `false`.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        NonStreamedChatResponse
+
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.chat(
             message="Can you give me a global market overview of solar panels?",
             prompt_truncation="OFF",
             temperature=0.3,
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"message": message, "stream": False}
+        _request: typing.Dict[str, typing.Any] = {"message": message}
         if model is not OMIT:
             _request["model"] = model
         if preamble is not OMIT:
             _request["preamble"] = preamble
         if chat_history is not OMIT:
             _request["chat_history"] = chat_history
         if conversation_id is not OMIT:
@@ -2402,19 +2863,23 @@
             _request["raw_prompting"] = raw_prompting
         if return_prompt is not OMIT:
             _request["return_prompt"] = return_prompt
         if tools is not OMIT:
             _request["tools"] = tools
         if tool_results is not OMIT:
             _request["tool_results"] = tool_results
+        if force_single_step is not OMIT:
+            _request["force_single_step"] = force_single_step
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "chat"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -2468,77 +2933,114 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates realistic text conditioned on a given input.
 
-        Parameters:
-            - prompt: str. The input text that serves as the starting point for generating the response.
-                           Note: The prompt will be pre-processed and modified before reaching the model.
+        Parameters
+        ----------
+        prompt : str
+            The input text that serves as the starting point for generating the response.
+            Note: The prompt will be pre-processed and modified before reaching the model.
 
-            - model: typing.Optional[str]. The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
-                                           Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
-            - num_generations: typing.Optional[int]. The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+        model : typing.Optional[str]
+            The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
+            Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
 
-                                                This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+        num_generations : typing.Optional[int]
+            The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-                                                Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - truncate: typing.Optional[GenerateStreamRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
 
-                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
 
-                                                                        If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - temperature: typing.Optional[float]. A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
-                                                   Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
+            Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-            - preset: typing.Optional[str]. Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.ai/playground/generate).
-                                            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
+        truncate : typing.Optional[GenerateStreamRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-            - end_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
+        temperature : typing.Optional[float]
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
+            Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - frequency_penalty: typing.Optional[float]. Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-                                                         Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        preset : typing.Optional[str]
+            Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.com/playground/generate).
+            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                        Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+        end_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-                                                        Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
 
-            - return_likelihoods: typing.Optional[GenerateStreamRequestReturnLikelihoods]. One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
 
-                                                                                           If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
 
-                                                                                           If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+
+        frequency_penalty : typing.Optional[float]
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+
+
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+
+            Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
+
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+
+
+        return_likelihoods : typing.Optional[GenerateStreamRequestReturnLikelihoods]
+            One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+
+            If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
+
+            If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
+
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without any pre-processing.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Yields
+        ------
+        typing.AsyncIterator[GenerateStreamedResponse]
+
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
-        await client.generate_stream(
+        response = await client.generate_stream(
             prompt="string",
             model="string",
             num_generations=1,
             max_tokens=1,
             truncate="NONE",
             temperature=1.1,
             seed=1.1,
@@ -2548,16 +3050,18 @@
             k=1,
             p=1.1,
             frequency_penalty=1.1,
             presence_penalty=1.1,
             return_likelihoods="GENERATION",
             raw_prompting=True,
         )
+        async for chunk in response:
+            yield chunk
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": True}
+        _request: typing.Dict[str, typing.Any] = {"prompt": prompt}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if truncate is not OMIT:
@@ -2581,18 +3085,20 @@
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if return_likelihoods is not OMIT:
             _request["return_likelihoods"] = return_likelihoods
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
         async with self._client_wrapper.httpx_client.stream(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -2659,81 +3165,118 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates realistic text conditioned on a given input.
 
-        Parameters:
-            - prompt: str. The input text that serves as the starting point for generating the response.
-                           Note: The prompt will be pre-processed and modified before reaching the model.
+        Parameters
+        ----------
+        prompt : str
+            The input text that serves as the starting point for generating the response.
+            Note: The prompt will be pre-processed and modified before reaching the model.
+
+
+        model : typing.Optional[str]
+            The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
+            Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+
+        num_generations : typing.Optional[int]
+            The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
+
+
+        max_tokens : typing.Optional[int]
+            The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+
+            This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+
+            Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
+
+
+        truncate : typing.Optional[GenerateRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
+
+        temperature : typing.Optional[float]
+            A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
+            Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
 
-            - model: typing.Optional[str]. The identifier of the model to generate with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental).
-                                           Smaller, "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
-            - num_generations: typing.Optional[int]. The maximum number of generations that will be returned. Defaults to `1`, min value of `1`, max value of `5`.
 
-            - max_tokens: typing.Optional[int]. The maximum number of tokens the model will generate as part of the response. Note: Setting a low value may result in incomplete generations.
+        seed : typing.Optional[float]
+            If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-                                                This parameter is off by default, and if it's not specified, the model will continue generating until it emits an EOS completion token. See [BPE Tokens](/bpe-tokens-wiki) for more details.
+        preset : typing.Optional[str]
+            Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.com/playground/generate).
+            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
 
-                                                Can only be set to `0` if `return_likelihoods` is set to `ALL` to get the likelihood of the prompt.
 
-            - truncate: typing.Optional[GenerateRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+        end_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-                                                                  Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+        stop_sequences : typing.Optional[typing.Sequence[str]]
+            The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
 
-                                                                  If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - temperature: typing.Optional[float]. A non-negative float that tunes the degree of randomness in generation. Lower temperatures mean less random generations. See [Temperature](/temperature-wiki) for more details.
-                                                   Defaults to `0.75`, min value of `0.0`, max value of `5.0`.
+        k : typing.Optional[int]
+            Ensures only the top `k` most likely tokens are considered for generation at each step.
+            Defaults to `0`, min value of `0`, max value of `500`.
 
-            - seed: typing.Optional[float]. If specified, the backend will make a best effort to sample tokens deterministically, such that repeated requests with the same seed and parameters should return the same result. However, determinsim cannot be totally guaranteed.
 
-            - preset: typing.Optional[str]. Identifier of a custom preset. A preset is a combination of parameters, such as prompt, temperature etc. You can create presets in the [playground](https://dashboard.cohere.ai/playground/generate).
-                                            When a preset is specified, the `prompt` parameter becomes optional, and any included parameters will override the preset's parameters.
+        p : typing.Optional[float]
+            Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
+            Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - end_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the beginning of the earliest occurrence of an end sequence. The sequence will be excluded from the text.
 
-            - stop_sequences: typing.Optional[typing.Sequence[str]]. The generated text will be cut at the end of the earliest occurrence of a stop sequence. The sequence will be included the text.
+        frequency_penalty : typing.Optional[float]
+            Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
 
-            - k: typing.Optional[int]. Ensures only the top `k` most likely tokens are considered for generation at each step.
-                                       Defaults to `0`, min value of `0`, max value of `500`.
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
 
-            - p: typing.Optional[float]. Ensures that only the most likely tokens, with total probability mass of `p`, are considered for generation at each step. If both `k` and `p` are enabled, `p` acts after `k`.
-                                         Defaults to `0.75`. min value of `0.01`, max value of `0.99`.
 
-            - frequency_penalty: typing.Optional[float]. Used to reduce repetitiveness of generated tokens. The higher the value, the stronger a penalty is applied to previously present tokens, proportional to how many times they have already appeared in the prompt or prior generation.
+        presence_penalty : typing.Optional[float]
+            Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
 
-                                                         Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+            Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
-            - presence_penalty: typing.Optional[float]. Defaults to `0.0`, min value of `0.0`, max value of `1.0`.
+            Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
 
-                                                        Can be used to reduce repetitiveness of generated tokens. Similar to `frequency_penalty`, except that this penalty is applied equally to all tokens that have already appeared, regardless of their exact frequencies.
 
-                                                        Using `frequency_penalty` in combination with `presence_penalty` is not supported on newer models.
+        return_likelihoods : typing.Optional[GenerateRequestReturnLikelihoods]
+            One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
 
-            - return_likelihoods: typing.Optional[GenerateRequestReturnLikelihoods]. One of `GENERATION|ALL|NONE` to specify how and if the token likelihoods are returned with the response. Defaults to `NONE`.
+            If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
 
-                                                                                     If `GENERATION` is selected, the token likelihoods will only be provided for generated text.
+            If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
 
-                                                                                     If `ALL` is selected, the token likelihoods will be provided both for the prompt and the generated text.
-            - raw_prompting: typing.Optional[bool]. When enabled, the user's prompt will be sent to the model without any pre-processing.
+        raw_prompting : typing.Optional[bool]
+            When enabled, the user's prompt will be sent to the model without any pre-processing.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        Generation
+
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.generate(
             prompt="Please explain to me how LLMs work",
         )
         """
-        _request: typing.Dict[str, typing.Any] = {"prompt": prompt, "stream": False}
+        _request: typing.Dict[str, typing.Any] = {"prompt": prompt}
         if model is not OMIT:
             _request["model"] = model
         if num_generations is not OMIT:
             _request["num_generations"] = num_generations
         if max_tokens is not OMIT:
             _request["max_tokens"] = max_tokens
         if truncate is not OMIT:
@@ -2757,18 +3300,20 @@
         if presence_penalty is not OMIT:
             _request["presence_penalty"] = presence_penalty
         if return_likelihoods is not OMIT:
             _request["return_likelihoods"] = return_likelihoods
         if raw_prompting is not OMIT:
             _request["raw_prompting"] = raw_prompting
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "generate"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -2819,47 +3364,63 @@
         """
         This endpoint returns text embeddings. An embedding is a list of floating point numbers that captures semantic information about the text that it represents.
 
         Embeddings can be used to create text classifiers as well as empower semantic search. To learn more about embeddings, see the embedding page.
 
         If you want to learn more how to use the embedding model, have a look at the [Semantic Search Guide](/docs/semantic-search).
 
-        Parameters:
-            - texts: typing.Sequence[str]. An array of strings for the model to embed. Maximum number of texts per call is `96`. We recommend reducing the length of each text to be under `512` tokens for optimal quality.
+        Parameters
+        ----------
+        texts : typing.Sequence[str]
+            An array of strings for the model to embed. Maximum number of texts per call is `96`. We recommend reducing the length of each text to be under `512` tokens for optimal quality.
+
+        model : typing.Optional[str]
+            Defaults to embed-english-v2.0
+
+            The identifier of the model. Smaller "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+
+            Available models and corresponding embedding dimensions:
 
-            - model: typing.Optional[str]. Defaults to embed-english-v2.0
+            * `embed-english-v3.0`  1024
+            * `embed-multilingual-v3.0`  1024
+            * `embed-english-light-v3.0`  384
+            * `embed-multilingual-light-v3.0`  384
 
-                                           The identifier of the model. Smaller "light" models are faster, while larger models will perform better. [Custom models](/docs/training-custom-models) can also be supplied with their full ID.
+            * `embed-english-v2.0`  4096
+            * `embed-english-light-v2.0`  1024
+            * `embed-multilingual-v2.0`  768
 
-                                           Available models and corresponding embedding dimensions:
+        input_type : typing.Optional[EmbedInputType]
 
-                                           * `embed-english-v3.0`  1024
-                                           * `embed-multilingual-v3.0`  1024
-                                           * `embed-english-light-v3.0`  384
-                                           * `embed-multilingual-light-v3.0`  384
+        embedding_types : typing.Optional[typing.Sequence[EmbeddingType]]
+            Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-                                           * `embed-english-v2.0`  4096
-                                           * `embed-english-light-v2.0`  1024
-                                           * `embed-multilingual-v2.0`  768
-            - input_type: typing.Optional[EmbedInputType].
+            * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+            * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+            * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+            * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+            * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
 
-            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
+        truncate : typing.Optional[EmbedRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
-                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
-                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
-                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
-                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
-            - truncate: typing.Optional[EmbedRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-                                                               Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
 
-                                                               If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        EmbedResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.embed(
@@ -2876,18 +3437,20 @@
         if input_type is not OMIT:
             _request["input_type"] = input_type
         if embedding_types is not OMIT:
             _request["embedding_types"] = embedding_types
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -2924,47 +3487,65 @@
         except JSONDecodeError:
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def rerank(
         self,
         *,
-        model: typing.Optional[str] = OMIT,
         query: str,
         documents: typing.Sequence[RerankRequestDocumentsItem],
+        model: typing.Optional[str] = OMIT,
         top_n: typing.Optional[int] = OMIT,
         rank_fields: typing.Optional[typing.Sequence[str]] = OMIT,
         return_documents: typing.Optional[bool] = OMIT,
         max_chunks_per_doc: typing.Optional[int] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> RerankResponse:
         """
         This endpoint takes in a query and a list of texts and produces an ordered array with each text assigned a relevance score.
 
-        Parameters:
-            - model: typing.Optional[str]. The identifier of the model to use, one of : `rerank-english-v3.0`, `rerank-multilingual-v3.0`, `rerank-english-v2.0`, `rerank-multilingual-v2.0`
+        Parameters
+        ----------
+        query : str
+            The search query
+
+        documents : typing.Sequence[RerankRequestDocumentsItem]
+            A list of document objects or strings to rerank.
+            If a document is provided the text fields is required and all other fields will be preserved in the response.
+
+            The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
 
-            - query: str. The search query
+            We recommend a maximum of 1,000 documents for optimal endpoint performance.
 
-            - documents: typing.Sequence[RerankRequestDocumentsItem]. A list of document objects or strings to rerank.
-                                                                      If a document is provided the text fields is required and all other fields will be preserved in the response.
+        model : typing.Optional[str]
+            The identifier of the model to use, one of : `rerank-english-v3.0`, `rerank-multilingual-v3.0`, `rerank-english-v2.0`, `rerank-multilingual-v2.0`
 
-                                                                      The total max chunks (length of documents * max_chunks_per_doc) must be less than 10000.
+        top_n : typing.Optional[int]
+            The number of most relevant documents or indices to return, defaults to the length of the documents
 
-                                                                      We recommend a maximum of 1,000 documents for optimal endpoint performance.
-            - top_n: typing.Optional[int]. The number of most relevant documents or indices to return, defaults to the length of the documents
+        rank_fields : typing.Optional[typing.Sequence[str]]
+            If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
 
-            - rank_fields: typing.Optional[typing.Sequence[str]]. If a JSON object is provided, you can specify which keys you would like to have considered for reranking. The model will rerank based on order of the fields passed in (i.e. rank_fields=['title','author','text'] will rerank using the values in title, author, text  sequentially. If the length of title, author, and text exceeds the context length of the model, the chunking will not re-consider earlier fields). If not provided, the model will use the default text field for ranking.
+        return_documents : typing.Optional[bool]
+            - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
+            - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
 
-            - return_documents: typing.Optional[bool]. - If false, returns results without the doc text - the api will return a list of {index, relevance score} where index is inferred from the list passed into the request.
-                                                       - If true, returns results with the doc text passed in - the api will return an ordered list of {index, text, relevance score} where index + text refers to the list passed into the request.
-            - max_chunks_per_doc: typing.Optional[int]. The maximum number of chunks to produce internally from a document
+        max_chunks_per_doc : typing.Optional[int]
+            The maximum number of chunks to produce internally from a document
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        RerankResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.rerank(
@@ -2986,18 +3567,20 @@
         if rank_fields is not OMIT:
             _request["rank_fields"] = rank_fields
         if return_documents is not OMIT:
             _request["return_documents"] = return_documents
         if max_chunks_per_doc is not OMIT:
             _request["max_chunks_per_doc"] = max_chunks_per_doc
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "rerank"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -3037,29 +3620,46 @@
         truncate: typing.Optional[ClassifyRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ClassifyResponse:
         """
         This endpoint makes a prediction about which label fits the specified text inputs best. To make a prediction, Classify uses the provided `examples` of text + label pairs as a reference.
         Note: [Fine-tuned models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
 
-        Parameters:
-            - inputs: typing.Sequence[str]. A list of up to 96 texts to be classified. Each one must be a non-empty string.
-                                            There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
-                                            Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
-            - examples: typing.Optional[typing.Sequence[ClassifyExample]]. An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
-                                                                           Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
-            - model: typing.Optional[str]. The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
-
-            - preset: typing.Optional[str]. The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.ai/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
-
-            - truncate: typing.Optional[ClassifyRequestTruncate]. One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
-                                                                  Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
-                                                                  If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        inputs : typing.Sequence[str]
+            A list of up to 96 texts to be classified. Each one must be a non-empty string.
+            There is, however, no consistent, universal limit to the length a particular input can be. We perform classification on the first `x` tokens of each input, and `x` varies depending on which underlying model is powering classification. The maximum token length for each model is listed in the "max tokens" column [here](https://docs.cohere.com/docs/models).
+            Note: by default the `truncate` parameter is set to `END`, so tokens exceeding the limit will be automatically dropped. This behavior can be disabled by setting `truncate` to `NONE`, which will result in validation errors for longer texts.
+
+        examples : typing.Optional[typing.Sequence[ClassifyExample]]
+            An array of examples to provide context to the model. Each example is a text string and its associated label/class. Each unique label requires at least 2 examples associated with it; the maximum number of examples is 2500, and each example has a maximum length of 512 tokens. The values should be structured as `{text: "...",label: "..."}`.
+            Note: [Fine-tuned Models](https://docs.cohere.com/docs/classify-fine-tuning) trained on classification examples don't require the `examples` parameter to be passed in explicitly.
+
+        model : typing.Optional[str]
+            The identifier of the model. Currently available models are `embed-multilingual-v2.0`, `embed-english-light-v2.0`, and `embed-english-v2.0` (default). Smaller "light" models are faster, while larger models will perform better. [Fine-tuned models](https://docs.cohere.com/docs/fine-tuning) can also be supplied with their full ID.
+
+        preset : typing.Optional[str]
+            The ID of a custom playground preset. You can create presets in the [playground](https://dashboard.cohere.com/playground/classify?model=large). If you use a preset, all other parameters become optional, and any included parameters will override the preset's parameters.
+
+        truncate : typing.Optional[ClassifyRequestTruncate]
+            One of `NONE|START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
+            If `NONE` is selected, when the input exceeds the maximum input token length an error will be returned.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ClassifyResponse
+            OK
+
+        Examples
+        --------
         from cohere import ClassifyExample
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -3115,18 +3715,20 @@
         if model is not OMIT:
             _request["model"] = model
         if preset is not OMIT:
             _request["preset"] = preset
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "classify"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "classify"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -3179,31 +3781,47 @@
         """
         > 🚧 Warning
         >
         > This API is marked as "Legacy" and is no longer maintained. Follow the [migration guide](/docs/migrating-from-cogenerate-to-cochat) to start using the Chat API.
 
         Generates a summary in English for a given text.
 
-        Parameters:
-            - text: str. The text to generate a summary for. Can be up to 100,000 characters long. Currently the only supported language is English.
+        Parameters
+        ----------
+        text : str
+            The text to generate a summary for. Can be up to 100,000 characters long. Currently the only supported language is English.
+
+        length : typing.Optional[SummarizeRequestLength]
+            One of `short`, `medium`, `long`, or `auto` defaults to `auto`. Indicates the approximate length of the summary. If `auto` is selected, the best option will be picked based on the input text.
+
+        format : typing.Optional[SummarizeRequestFormat]
+            One of `paragraph`, `bullets`, or `auto`, defaults to `auto`. Indicates the style in which the summary will be delivered - in a free form paragraph or in bullet points. If `auto` is selected, the best option will be picked based on the input text.
 
-            - length: typing.Optional[SummarizeRequestLength]. One of `short`, `medium`, `long`, or `auto` defaults to `auto`. Indicates the approximate length of the summary. If `auto` is selected, the best option will be picked based on the input text.
+        model : typing.Optional[str]
+            The identifier of the model to generate the summary with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental). Smaller, "light" models are faster, while larger models will perform better.
 
-            - format: typing.Optional[SummarizeRequestFormat]. One of `paragraph`, `bullets`, or `auto`, defaults to `auto`. Indicates the style in which the summary will be delivered - in a free form paragraph or in bullet points. If `auto` is selected, the best option will be picked based on the input text.
+        extractiveness : typing.Optional[SummarizeRequestExtractiveness]
+            One of `low`, `medium`, `high`, or `auto`, defaults to `auto`. Controls how close to the original text the summary is. `high` extractiveness summaries will lean towards reusing sentences verbatim, while `low` extractiveness summaries will tend to paraphrase more. If `auto` is selected, the best option will be picked based on the input text.
 
-            - model: typing.Optional[str]. The identifier of the model to generate the summary with. Currently available models are `command` (default), `command-nightly` (experimental), `command-light`, and `command-light-nightly` (experimental). Smaller, "light" models are faster, while larger models will perform better.
+        temperature : typing.Optional[float]
+            Ranges from 0 to 5. Controls the randomness of the output. Lower values tend to generate more “predictable” output, while higher values tend to generate more “creative” output. The sweet spot is typically between 0 and 1.
 
-            - extractiveness: typing.Optional[SummarizeRequestExtractiveness]. One of `low`, `medium`, `high`, or `auto`, defaults to `auto`. Controls how close to the original text the summary is. `high` extractiveness summaries will lean towards reusing sentences verbatim, while `low` extractiveness summaries will tend to paraphrase more. If `auto` is selected, the best option will be picked based on the input text.
+        additional_command : typing.Optional[str]
+            A free-form instruction for modifying how the summaries get generated. Should complete the sentence "Generate a summary _". Eg. "focusing on the next steps" or "written by Yoda"
 
-            - temperature: typing.Optional[float]. Ranges from 0 to 5. Controls the randomness of the output. Lower values tend to generate more “predictable” output, while higher values tend to generate more “creative” output. The sweet spot is typically between 0 and 1.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - additional_command: typing.Optional[str]. A free-form instruction for modifying how the summaries get generated. Should complete the sentence "Generate a summary _". Eg. "focusing on the next steps" or "written by Yoda"
+        Returns
+        -------
+        SummarizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.summarize(
@@ -3220,18 +3838,20 @@
         if extractiveness is not OMIT:
             _request["extractiveness"] = extractiveness
         if temperature is not OMIT:
             _request["temperature"] = temperature
         if additional_command is not OMIT:
             _request["additional_command"] = additional_command
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "summarize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "summarize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -3263,37 +3883,50 @@
 
     async def tokenize(
         self, *, text: str, model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> TokenizeResponse:
         """
         This endpoint splits input text into smaller units called tokens using byte-pair encoding (BPE). To learn more about tokenization and byte pair encoding, see the tokens page.
 
-        Parameters:
-            - text: str. The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
-
-            - model: str. An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+        Parameters
+        ----------
+        text : str
+            The string to be tokenized, the minimum text length is 1 character, and the maximum text length is 65536 characters.
+
+        model : str
+            An optional parameter to provide the model name. This will ensure that the tokenization uses the tokenizer used by that model.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        TokenizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.tokenize(
             text="tokenize me! :D",
             model="command",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "tokenize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"text": text, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"text": text, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -3333,37 +3966,50 @@
 
     async def detokenize(
         self, *, tokens: typing.Sequence[int], model: str, request_options: typing.Optional[RequestOptions] = None
     ) -> DetokenizeResponse:
         """
         This endpoint takes tokens using byte-pair encoding and returns their text representation. To learn more about tokenization and byte pair encoding, see the tokens page.
 
-        Parameters:
-            - tokens: typing.Sequence[int]. The list of tokens to be detokenized.
-
-            - model: str. An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+        Parameters
+        ----------
+        tokens : typing.Sequence[int]
+            The list of tokens to be detokenized.
+
+        model : str
+            An optional parameter to provide the model name. This will ensure that the detokenization is done by the tokenizer used by that model.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DetokenizeResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.detokenize(
             tokens=[10104, 12221, 1315, 34, 1420, 69],
             model="command",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "detokenize"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder({"tokens": tokens, "model": model})
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder({"tokens": tokens, "model": model}),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -3393,30 +4039,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def check_api_key(self, *, request_options: typing.Optional[RequestOptions] = None) -> CheckApiKeyResponse:
         """
         Checks that the api key in the Authorization header is valid and active
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CheckApiKeyResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.check_api_key()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "check-api-key"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `cohere-5.5.0/src/cohere/bedrock_client.py` & `cohere-5.5.1/src/cohere/bedrock_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/client.py` & `cohere-5.5.1/src/cohere/client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/connectors/client.py` & `cohere-5.5.1/src/cohere/connectors/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.not_found_error import NotFoundError
@@ -39,43 +40,56 @@
         limit: typing.Optional[float] = None,
         offset: typing.Optional[float] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListConnectorsResponse:
         """
         Returns a list of connectors ordered by descending creation date (newer first). See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
 
-        Parameters:
-            - limit: typing.Optional[float]. Maximum number of connectors to return [0, 100].
+        Parameters
+        ----------
+        limit : typing.Optional[float]
+            Maximum number of connectors to return [0, 100].
+
+        offset : typing.Optional[float]
+            Number of connectors to skip before returning results [0, inf].
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListConnectorsResponse
+            OK
 
-            - offset: typing.Optional[float]. Number of connectors to skip before returning results [0, inf].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "offset": offset,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "offset": offset,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -108,45 +122,62 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         name: str,
-        description: typing.Optional[str] = OMIT,
         url: str,
+        description: typing.Optional[str] = OMIT,
         excludes: typing.Optional[typing.Sequence[str]] = OMIT,
         oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
         active: typing.Optional[bool] = OMIT,
         continue_on_failure: typing.Optional[bool] = OMIT,
         service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateConnectorResponse:
         """
         Creates a new connector. The connector is tested during registration and will cancel registration when the test is unsuccessful. See ['Creating and Deploying a Connector'](https://docs.cohere.com/docs/creating-and-deploying-a-connector) for more information.
 
-        Parameters:
-            - name: str. A human-readable name for the connector.
+        Parameters
+        ----------
+        name : str
+            A human-readable name for the connector.
+
+        url : str
+            The URL of the connector that will be used to search for documents.
 
-            - description: typing.Optional[str]. A description of the connector.
+        description : typing.Optional[str]
+            A description of the connector.
 
-            - url: str. The URL of the connector that will be used to search for documents.
+        excludes : typing.Optional[typing.Sequence[str]]
+            A list of fields to exclude from the prompt (fields remain in the document).
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+        oauth : typing.Optional[CreateConnectorOAuth]
+            The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+        active : typing.Optional[bool]
+            Whether the connector is active or not.
 
-            - active: typing.Optional[bool]. Whether the connector is active or not.
+        continue_on_failure : typing.Optional[bool]
+            Whether a chat request should continue or not if the request to this connector fails.
 
-            - continue_on_failure: typing.Optional[bool]. Whether a chat request should continue or not if the request to this connector fails.
+        service_auth : typing.Optional[CreateConnectorServiceAuth]
+            The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        CreateConnectorResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.create(
@@ -164,18 +195,20 @@
         if active is not OMIT:
             _request["active"] = active
         if continue_on_failure is not OMIT:
             _request["continue_on_failure"] = continue_on_failure
         if service_auth is not OMIT:
             _request["service_auth"] = service_auth
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -217,34 +250,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetConnectorResponse:
         """
         Retrieve a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to retrieve.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetConnectorResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.get(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -280,34 +325,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DeleteConnectorResponse:
         """
         Delete a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to delete.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to delete.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteConnectorResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.delete(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -359,33 +416,48 @@
         continue_on_failure: typing.Optional[bool] = OMIT,
         service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpdateConnectorResponse:
         """
         Update a connector by ID. Omitted fields will not be updated. See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to update.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to update.
+
+        name : typing.Optional[str]
+            A human-readable name for the connector.
 
-            - name: typing.Optional[str]. A human-readable name for the connector.
+        url : typing.Optional[str]
+            The URL of the connector that will be used to search for documents.
 
-            - url: typing.Optional[str]. The URL of the connector that will be used to search for documents.
+        excludes : typing.Optional[typing.Sequence[str]]
+            A list of fields to exclude from the prompt (fields remain in the document).
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+        oauth : typing.Optional[CreateConnectorOAuth]
+            The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+        active : typing.Optional[bool]
 
-            - active: typing.Optional[bool].
+        continue_on_failure : typing.Optional[bool]
 
-            - continue_on_failure: typing.Optional[bool].
+        service_auth : typing.Optional[CreateConnectorServiceAuth]
+            The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        UpdateConnectorResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.update(
@@ -404,18 +476,20 @@
         if active is not OMIT:
             _request["active"] = active
         if continue_on_failure is not OMIT:
             _request["continue_on_failure"] = continue_on_failure
         if service_auth is not OMIT:
             _request["service_auth"] = service_auth
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -467,46 +541,59 @@
         *,
         after_token_redirect: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OAuthAuthorizeResponse:
         """
         Authorize the connector with the given ID for the connector oauth app. See ['Connector Authentication'](https://docs.cohere.com/docs/connector-authentication) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to authorize.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to authorize.
+
+        after_token_redirect : typing.Optional[str]
+            The URL to redirect to after the connector has been authorized.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        OAuthAuthorizeResponse
+            OK
 
-            - after_token_redirect: typing.Optional[str]. The URL to redirect to after the connector has been authorized.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.connectors.o_auth_authorize(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}/oauth/authorize"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "after_token_redirect": after_token_redirect,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "after_token_redirect": after_token_redirect,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
@@ -557,43 +644,56 @@
         limit: typing.Optional[float] = None,
         offset: typing.Optional[float] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListConnectorsResponse:
         """
         Returns a list of connectors ordered by descending creation date (newer first). See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
 
-        Parameters:
-            - limit: typing.Optional[float]. Maximum number of connectors to return [0, 100].
+        Parameters
+        ----------
+        limit : typing.Optional[float]
+            Maximum number of connectors to return [0, 100].
+
+        offset : typing.Optional[float]
+            Number of connectors to skip before returning results [0, inf].
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListConnectorsResponse
+            OK
 
-            - offset: typing.Optional[float]. Number of connectors to skip before returning results [0, inf].
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "limit": limit,
-                        "offset": offset,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "limit": limit,
+                            "offset": offset,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -626,45 +726,62 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         name: str,
-        description: typing.Optional[str] = OMIT,
         url: str,
+        description: typing.Optional[str] = OMIT,
         excludes: typing.Optional[typing.Sequence[str]] = OMIT,
         oauth: typing.Optional[CreateConnectorOAuth] = OMIT,
         active: typing.Optional[bool] = OMIT,
         continue_on_failure: typing.Optional[bool] = OMIT,
         service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateConnectorResponse:
         """
         Creates a new connector. The connector is tested during registration and will cancel registration when the test is unsuccessful. See ['Creating and Deploying a Connector'](https://docs.cohere.com/docs/creating-and-deploying-a-connector) for more information.
 
-        Parameters:
-            - name: str. A human-readable name for the connector.
+        Parameters
+        ----------
+        name : str
+            A human-readable name for the connector.
+
+        url : str
+            The URL of the connector that will be used to search for documents.
 
-            - description: typing.Optional[str]. A description of the connector.
+        description : typing.Optional[str]
+            A description of the connector.
 
-            - url: str. The URL of the connector that will be used to search for documents.
+        excludes : typing.Optional[typing.Sequence[str]]
+            A list of fields to exclude from the prompt (fields remain in the document).
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+        oauth : typing.Optional[CreateConnectorOAuth]
+            The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+        active : typing.Optional[bool]
+            Whether the connector is active or not.
 
-            - active: typing.Optional[bool]. Whether the connector is active or not.
+        continue_on_failure : typing.Optional[bool]
+            Whether a chat request should continue or not if the request to this connector fails.
 
-            - continue_on_failure: typing.Optional[bool]. Whether a chat request should continue or not if the request to this connector fails.
+        service_auth : typing.Optional[CreateConnectorServiceAuth]
+            The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        CreateConnectorResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.create(
@@ -682,18 +799,20 @@
         if active is not OMIT:
             _request["active"] = active
         if continue_on_failure is not OMIT:
             _request["continue_on_failure"] = continue_on_failure
         if service_auth is not OMIT:
             _request["service_auth"] = service_auth
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "connectors"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -735,34 +854,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetConnectorResponse:
         """
         Retrieve a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to retrieve.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetConnectorResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.get(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -800,34 +931,46 @@
 
     async def delete(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteConnectorResponse:
         """
         Delete a connector by ID. See ['Connectors'](https://docs.cohere.com/docs/connectors) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to delete.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to delete.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteConnectorResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.delete(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -879,33 +1022,48 @@
         continue_on_failure: typing.Optional[bool] = OMIT,
         service_auth: typing.Optional[CreateConnectorServiceAuth] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpdateConnectorResponse:
         """
         Update a connector by ID. Omitted fields will not be updated. See ['Managing your Connector'](https://docs.cohere.com/docs/managing-your-connector) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to update.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to update.
+
+        name : typing.Optional[str]
+            A human-readable name for the connector.
 
-            - name: typing.Optional[str]. A human-readable name for the connector.
+        url : typing.Optional[str]
+            The URL of the connector that will be used to search for documents.
 
-            - url: typing.Optional[str]. The URL of the connector that will be used to search for documents.
+        excludes : typing.Optional[typing.Sequence[str]]
+            A list of fields to exclude from the prompt (fields remain in the document).
 
-            - excludes: typing.Optional[typing.Sequence[str]]. A list of fields to exclude from the prompt (fields remain in the document).
+        oauth : typing.Optional[CreateConnectorOAuth]
+            The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
 
-            - oauth: typing.Optional[CreateConnectorOAuth]. The OAuth 2.0 configuration for the connector. Cannot be specified if service_auth is specified.
+        active : typing.Optional[bool]
 
-            - active: typing.Optional[bool].
+        continue_on_failure : typing.Optional[bool]
 
-            - continue_on_failure: typing.Optional[bool].
+        service_auth : typing.Optional[CreateConnectorServiceAuth]
+            The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
 
-            - service_auth: typing.Optional[CreateConnectorServiceAuth]. The service to service authentication configuration for the connector. Cannot be specified if oauth is specified.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        UpdateConnectorResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.update(
@@ -924,18 +1082,20 @@
         if active is not OMIT:
             _request["active"] = active
         if continue_on_failure is not OMIT:
             _request["continue_on_failure"] = continue_on_failure
         if service_auth is not OMIT:
             _request["service_auth"] = service_auth
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="PATCH",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -987,46 +1147,59 @@
         *,
         after_token_redirect: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> OAuthAuthorizeResponse:
         """
         Authorize the connector with the given ID for the connector oauth app. See ['Connector Authentication'](https://docs.cohere.com/docs/connector-authentication) for more information.
 
-        Parameters:
-            - id: str. The ID of the connector to authorize.
+        Parameters
+        ----------
+        id : str
+            The ID of the connector to authorize.
+
+        after_token_redirect : typing.Optional[str]
+            The URL to redirect to after the connector has been authorized.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        OAuthAuthorizeResponse
+            OK
 
-            - after_token_redirect: typing.Optional[str]. The URL to redirect to after the connector has been authorized.
-
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.connectors.o_auth_authorize(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"connectors/{jsonable_encoder(id)}/oauth/authorize"
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "after_token_redirect": after_token_redirect,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "after_token_redirect": after_token_redirect,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
```

### Comparing `cohere-5.5.0/src/cohere/core/__init__.py` & `cohere-5.5.1/src/cohere/core/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 
 from .api_error import ApiError
 from .client_wrapper import AsyncClientWrapper, BaseClientWrapper, SyncClientWrapper
 from .datetime_utils import serialize_datetime
 from .file import File, convert_file_dict_to_httpx_tuples
 from .http_client import AsyncHttpClient, HttpClient
 from .jsonable_encoder import jsonable_encoder
-from .pydantic_utilities import pydantic_v1
+from .pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .query_encoder import encode_query
 from .remove_none_from_dict import remove_none_from_dict
 from .request_options import RequestOptions
 from .unchecked_base_model import UncheckedBaseModel, UnionMetadata, construct_type
 
 __all__ = [
     "ApiError",
     "AsyncClientWrapper",
@@ -20,12 +21,14 @@
     "HttpClient",
     "RequestOptions",
     "SyncClientWrapper",
     "UncheckedBaseModel",
     "UnionMetadata",
     "construct_type",
     "convert_file_dict_to_httpx_tuples",
+    "deep_union_pydantic_dicts",
+    "encode_query",
     "jsonable_encoder",
     "pydantic_v1",
     "remove_none_from_dict",
     "serialize_datetime",
 ]
```

### Comparing `cohere-5.5.0/src/cohere/core/client_wrapper.py` & `cohere-5.5.1/src/cohere/core/client_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._base_url = base_url
         self._timeout = timeout
 
     def get_headers(self) -> typing.Dict[str, str]:
         headers: typing.Dict[str, str] = {
             "X-Fern-Language": "Python",
             "X-Fern-SDK-Name": "cohere",
-            "X-Fern-SDK-Version": "5.5.0",
+            "X-Fern-SDK-Version": "5.5.1",
         }
         if self._client_name is not None:
             headers["X-Client-Name"] = self._client_name
         headers["Authorization"] = f"Bearer {self._get_token()}"
         return headers
 
     def _get_token(self) -> str:
```

### Comparing `cohere-5.5.0/src/cohere/core/datetime_utils.py` & `cohere-5.5.1/src/cohere/core/datetime_utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/core/file.py` & `cohere-5.5.1/src/cohere/core/file.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/core/http_client.py` & `cohere-5.5.1/src/cohere/core/http_client.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/core/jsonable_encoder.py` & `cohere-5.5.1/src/cohere/core/jsonable_encoder.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/core/request_options.py` & `cohere-5.5.1/src/cohere/core/request_options.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/core/unchecked_base_model.py` & `cohere-5.5.1/src/cohere/core/unchecked_base_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -161,16 +161,18 @@
         inner_type = pydantic_v1.typing.get_args(type_)[0]
         return {construct_type(object_=entry, type_=inner_type) for entry in object_}
 
     if pydantic_v1.typing.is_union(base_type) or is_annotated_union:
         return _convert_union_type(type_, object_)
 
     # Cannot do an `issubclass` with a literal type, let's also just confirm we have a class before this call
-    if not pydantic_v1.typing.is_literal_type(type_) and (
-        inspect.isclass(base_type) and issubclass(base_type, pydantic_v1.BaseModel)
+    if (
+        object_ is not None
+        and not pydantic_v1.typing.is_literal_type(type_)
+        and (inspect.isclass(base_type) and issubclass(base_type, pydantic_v1.BaseModel))
     ):
         return type_.construct(**object_)
 
     if base_type == dt.datetime:
         try:
             return pydantic_v1.datetime_parse.parse_datetime(object_)
         except Exception:
```

### Comparing `cohere-5.5.0/src/cohere/datasets/client.py` & `cohere-5.5.1/src/cohere/datasets/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from json.decoder import JSONDecodeError
 
 from .. import core
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.datetime_utils import serialize_datetime
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.dataset_type import DatasetType
 from ..types.dataset_validation_status import DatasetValidationStatus
 from ..types.too_many_requests_error_body import TooManyRequestsErrorBody
@@ -40,55 +41,72 @@
         offset: typing.Optional[float] = None,
         validation_status: typing.Optional[DatasetValidationStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsListResponse:
         """
         List datasets that have been created.
 
-        Parameters:
-            - dataset_type: typing.Optional[str]. optional filter by dataset type
+        Parameters
+        ----------
+        dataset_type : typing.Optional[str]
+            optional filter by dataset type
 
-            - before: typing.Optional[dt.datetime]. optional filter before a date
+        before : typing.Optional[dt.datetime]
+            optional filter before a date
 
-            - after: typing.Optional[dt.datetime]. optional filter after a date
+        after : typing.Optional[dt.datetime]
+            optional filter after a date
 
-            - limit: typing.Optional[float]. optional limit to number of results
+        limit : typing.Optional[float]
+            optional limit to number of results
 
-            - offset: typing.Optional[float]. optional offset to start of results
+        offset : typing.Optional[float]
+            optional offset to start of results
 
-            - validation_status: typing.Optional[DatasetValidationStatus]. optional filter by validation status
+        validation_status : typing.Optional[DatasetValidationStatus]
+            optional filter by validation status
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsListResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.datasets.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "datasetType": dataset_type,
-                        "before": serialize_datetime(before) if before is not None else None,
-                        "after": serialize_datetime(after) if after is not None else None,
-                        "limit": limit,
-                        "offset": offset,
-                        "validationStatus": validation_status,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "datasetType": dataset_type,
+                            "before": serialize_datetime(before) if before is not None else None,
+                            "after": serialize_datetime(after) if after is not None else None,
+                            "limit": limit,
+                            "offset": offset,
+                            "validationStatus": validation_status,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -114,85 +132,107 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create(
         self,
         *,
         name: str,
         type: DatasetType,
+        data: core.File,
         keep_original_file: typing.Optional[bool] = None,
         skip_malformed_input: typing.Optional[bool] = None,
         keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         text_separator: typing.Optional[str] = None,
         csv_delimiter: typing.Optional[str] = None,
         dry_run: typing.Optional[bool] = None,
-        data: core.File,
         eval_data: typing.Optional[core.File] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
-        Parameters:
-            - name: str. The name of the uploaded dataset.
+        Parameters
+        ----------
+        name : str
+            The name of the uploaded dataset.
+
+        type : DatasetType
+            The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
-            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
+        data : core.File
+            See core.File for more documentation
 
-            - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
+        keep_original_file : typing.Optional[bool]
+            Indicates if the original file should be stored.
 
-            - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
+        skip_malformed_input : typing.Optional[bool]
+            Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
-            - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
+        keep_fields : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
 
-            - optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
+        optional_fields : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
 
-            - text_separator: typing.Optional[str]. Raw .txt uploads will be split into entries using the text_separator value.
+        text_separator : typing.Optional[str]
+            Raw .txt uploads will be split into entries using the text_separator value.
 
-            - csv_delimiter: typing.Optional[str]. The delimiter used for .csv uploads.
+        csv_delimiter : typing.Optional[str]
+            The delimiter used for .csv uploads.
 
-            - dry_run: typing.Optional[bool]. flag to enable dry_run mode
+        dry_run : typing.Optional[bool]
+            flag to enable dry_run mode
 
-            - data: core.File. See core.File for more documentation
+        eval_data : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - eval_data: typing.Optional[core.File]. See core.File for more documentation
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        DatasetsCreateResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.datasets.create(
             name="name",
             type="embed-input",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "name": name,
-                        "type": type,
-                        "keep_original_file": keep_original_file,
-                        "skip_malformed_input": skip_malformed_input,
-                        "keep_fields": keep_fields,
-                        "optional_fields": optional_fields,
-                        "text_separator": text_separator,
-                        "csv_delimiter": csv_delimiter,
-                        "dry_run": dry_run,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "name": name,
+                            "type": type,
+                            "keep_original_file": keep_original_file,
+                            "skip_malformed_input": skip_malformed_input,
+                            "keep_fields": keep_fields,
+                            "optional_fields": optional_fields,
+                            "text_separator": text_separator,
+                            "csv_delimiter": csv_delimiter,
+                            "dry_run": dry_run,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             data=jsonable_encoder(remove_none_from_dict({}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(remove_none_from_dict({})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
@@ -224,30 +264,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_usage(self, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetUsageResponse:
         """
         View the dataset storage usage for your Organization. Each Organization can have up to 10GB of storage across all their users.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsGetUsageResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.datasets.get_usage()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets/usage"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets/usage"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -271,34 +322,45 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetResponse:
         """
         Retrieve a dataset by ID. See ['Datasets'](https://docs.cohere.com/docs/datasets) for more information.
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsGetResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.datasets.get(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -324,34 +386,45 @@
 
     def delete(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Dict[str, typing.Any]:
         """
         Delete a dataset by ID. Datasets are automatically deleted after 30 days, but they can also be deleted manually.
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Dict[str, typing.Any]
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.datasets.delete(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -390,55 +463,72 @@
         offset: typing.Optional[float] = None,
         validation_status: typing.Optional[DatasetValidationStatus] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsListResponse:
         """
         List datasets that have been created.
 
-        Parameters:
-            - dataset_type: typing.Optional[str]. optional filter by dataset type
+        Parameters
+        ----------
+        dataset_type : typing.Optional[str]
+            optional filter by dataset type
 
-            - before: typing.Optional[dt.datetime]. optional filter before a date
+        before : typing.Optional[dt.datetime]
+            optional filter before a date
 
-            - after: typing.Optional[dt.datetime]. optional filter after a date
+        after : typing.Optional[dt.datetime]
+            optional filter after a date
 
-            - limit: typing.Optional[float]. optional limit to number of results
+        limit : typing.Optional[float]
+            optional limit to number of results
 
-            - offset: typing.Optional[float]. optional offset to start of results
+        offset : typing.Optional[float]
+            optional offset to start of results
 
-            - validation_status: typing.Optional[DatasetValidationStatus]. optional filter by validation status
+        validation_status : typing.Optional[DatasetValidationStatus]
+            optional filter by validation status
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsListResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.datasets.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "datasetType": dataset_type,
-                        "before": serialize_datetime(before) if before is not None else None,
-                        "after": serialize_datetime(after) if after is not None else None,
-                        "limit": limit,
-                        "offset": offset,
-                        "validationStatus": validation_status,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "datasetType": dataset_type,
+                            "before": serialize_datetime(before) if before is not None else None,
+                            "after": serialize_datetime(after) if after is not None else None,
+                            "limit": limit,
+                            "offset": offset,
+                            "validationStatus": validation_status,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -464,85 +554,107 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create(
         self,
         *,
         name: str,
         type: DatasetType,
+        data: core.File,
         keep_original_file: typing.Optional[bool] = None,
         skip_malformed_input: typing.Optional[bool] = None,
         keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]] = None,
         text_separator: typing.Optional[str] = None,
         csv_delimiter: typing.Optional[str] = None,
         dry_run: typing.Optional[bool] = None,
-        data: core.File,
         eval_data: typing.Optional[core.File] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> DatasetsCreateResponse:
         """
         Create a dataset by uploading a file. See ['Dataset Creation'](https://docs.cohere.com/docs/datasets#dataset-creation) for more information.
 
-        Parameters:
-            - name: str. The name of the uploaded dataset.
+        Parameters
+        ----------
+        name : str
+            The name of the uploaded dataset.
+
+        type : DatasetType
+            The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
 
-            - type: DatasetType. The dataset type, which is used to validate the data. Valid types are `embed-input`, `reranker-finetune-input`, `single-label-classification-finetune-input`, `chat-finetune-input`, and `multi-label-classification-finetune-input`.
+        data : core.File
+            See core.File for more documentation
 
-            - keep_original_file: typing.Optional[bool]. Indicates if the original file should be stored.
+        keep_original_file : typing.Optional[bool]
+            Indicates if the original file should be stored.
 
-            - skip_malformed_input: typing.Optional[bool]. Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
+        skip_malformed_input : typing.Optional[bool]
+            Indicates whether rows with malformed input should be dropped (instead of failing the validation check). Dropped rows will be returned in the warnings field.
 
-            - keep_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
+        keep_fields : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `keep_fields` are missing from the uploaded file, Dataset validation will fail.
 
-            - optional_fields: typing.Optional[typing.Union[str, typing.Sequence[str]]]. List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
+        optional_fields : typing.Optional[typing.Union[str, typing.Sequence[str]]]
+            List of names of fields that will be persisted in the Dataset. By default the Dataset will retain only the required fields indicated in the [schema for the corresponding Dataset type](https://docs.cohere.com/docs/datasets#dataset-types). For example, Datasets of type `embed-input` will drop all fields other than the required `text` field. If any of the fields in `optional_fields` are missing from the uploaded file, Dataset validation will pass.
 
-            - text_separator: typing.Optional[str]. Raw .txt uploads will be split into entries using the text_separator value.
+        text_separator : typing.Optional[str]
+            Raw .txt uploads will be split into entries using the text_separator value.
 
-            - csv_delimiter: typing.Optional[str]. The delimiter used for .csv uploads.
+        csv_delimiter : typing.Optional[str]
+            The delimiter used for .csv uploads.
 
-            - dry_run: typing.Optional[bool]. flag to enable dry_run mode
+        dry_run : typing.Optional[bool]
+            flag to enable dry_run mode
 
-            - data: core.File. See core.File for more documentation
+        eval_data : typing.Optional[core.File]
+            See core.File for more documentation
 
-            - eval_data: typing.Optional[core.File]. See core.File for more documentation
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        DatasetsCreateResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.datasets.create(
             name="name",
             type="embed-input",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "name": name,
-                        "type": type,
-                        "keep_original_file": keep_original_file,
-                        "skip_malformed_input": skip_malformed_input,
-                        "keep_fields": keep_fields,
-                        "optional_fields": optional_fields,
-                        "text_separator": text_separator,
-                        "csv_delimiter": csv_delimiter,
-                        "dry_run": dry_run,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "name": name,
+                            "type": type,
+                            "keep_original_file": keep_original_file,
+                            "skip_malformed_input": skip_malformed_input,
+                            "keep_fields": keep_fields,
+                            "optional_fields": optional_fields,
+                            "text_separator": text_separator,
+                            "csv_delimiter": csv_delimiter,
+                            "dry_run": dry_run,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             data=jsonable_encoder(remove_none_from_dict({}))
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(remove_none_from_dict({})),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
@@ -574,30 +686,41 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_usage(self, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetUsageResponse:
         """
         View the dataset storage usage for your Organization. Each Organization can have up to 10GB of storage across all their users.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsGetUsageResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.datasets.get_usage()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets/usage"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "datasets/usage"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -621,34 +744,45 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> DatasetsGetResponse:
         """
         Retrieve a dataset by ID. See ['Datasets'](https://docs.cohere.com/docs/datasets) for more information.
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DatasetsGetResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.datasets.get(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -674,34 +808,45 @@
 
     async def delete(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> typing.Dict[str, typing.Any]:
         """
         Delete a dataset by ID. Datasets are automatically deleted after 30 days, but they can also be deleted manually.
 
-        Parameters:
-            - id: str.
+        Parameters
+        ----------
+        id : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        typing.Dict[str, typing.Any]
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.datasets.delete(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="DELETE",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"datasets/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
```

### Comparing `cohere-5.5.0/src/cohere/datasets/types/__init__.py` & `cohere-5.5.1/src/cohere/datasets/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/datasets/types/datasets_create_response.py` & `cohere-5.5.1/src/cohere/types/classify_response_classifications_item_labels_value.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,29 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...core.unchecked_base_model import UncheckedBaseModel
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsCreateResponse(UncheckedBaseModel):
-    id: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The dataset ID
-    """
+class ClassifyResponseClassificationsItemLabelsValue(UncheckedBaseModel):
+    confidence: typing.Optional[float] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py` & `cohere-5.5.1/src/cohere/datasets/types/datasets_create_response_dataset_parts_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ...core.unchecked_base_model import UncheckedBaseModel
 
 
 class DatasetsCreateResponseDatasetPartsItem(UncheckedBaseModel):
     """
     the underlying files that make up the dataset
     """
@@ -30,15 +30,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/datasets/types/datasets_get_response.py` & `cohere-5.5.1/src/cohere/types/list_embed_job_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...core.unchecked_base_model import UncheckedBaseModel
-from ...types.dataset import Dataset
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .embed_job import EmbedJob
 
 
-class DatasetsGetResponse(UncheckedBaseModel):
-    dataset: Dataset
+class ListEmbedJobResponse(UncheckedBaseModel):
+    embed_jobs: typing.Optional[typing.List[EmbedJob]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/datasets/types/datasets_get_usage_response.py` & `cohere-5.5.1/src/cohere/types/check_api_key_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
-from ...core.unchecked_base_model import UncheckedBaseModel
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class DatasetsGetUsageResponse(UncheckedBaseModel):
-    organization_usage: typing.Optional[int] = pydantic_v1.Field(default=None)
-    """
-    The total number of bytes used by the organization.
-    """
+class CheckApiKeyResponse(UncheckedBaseModel):
+    valid: bool
+    organization_id: typing.Optional[str] = None
+    owner_id: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/datasets/types/datasets_list_response.py` & `cohere-5.5.1/src/cohere/datasets/types/datasets_list_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ...core.datetime_utils import serialize_datetime
-from ...core.pydantic_utilities import pydantic_v1
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ...core.unchecked_base_model import UncheckedBaseModel
 from ...types.dataset import Dataset
 
 
 class DatasetsListResponse(UncheckedBaseModel):
     datasets: typing.Optional[typing.List[Dataset]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/embed_jobs/client.py` & `cohere-5.5.1/src/cohere/embed_jobs/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.not_found_error import NotFoundError
 from ..errors.too_many_requests_error import TooManyRequestsError
@@ -30,30 +31,41 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListEmbedJobResponse:
         """
         The list embed job endpoint allows users to view all embed jobs history for that specific user.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListEmbedJobResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.embed_jobs.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -95,43 +107,60 @@
         embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
         truncate: typing.Optional[CreateEmbedJobRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateEmbedJobResponse:
         """
         This API launches an async Embed job for a [Dataset](https://docs.cohere.com/docs/datasets) of type `embed-input`. The result of a completed embed job is new Dataset of type `embed-output`, which contains the original text entries and the corresponding embeddings.
 
-        Parameters:
-            - model: str. ID of the embedding model.
+        Parameters
+        ----------
+        model : str
+            ID of the embedding model.
+
+            Available models and corresponding embedding dimensions:
+
+            - `embed-english-v3.0` : 1024
+            - `embed-multilingual-v3.0` : 1024
+            - `embed-english-light-v3.0` : 384
+            - `embed-multilingual-light-v3.0` : 384
+
 
-                          Available models and corresponding embedding dimensions:
+        dataset_id : str
+            ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
 
-                          - `embed-english-v3.0` : 1024
-                          - `embed-multilingual-v3.0` : 1024
-                          - `embed-english-light-v3.0` : 384
-                          - `embed-multilingual-light-v3.0` : 384
+        input_type : EmbedInputType
 
-            - dataset_id: str. ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
+        name : typing.Optional[str]
+            The name of the embed job.
 
-            - input_type: EmbedInputType.
+        embedding_types : typing.Optional[typing.Sequence[EmbeddingType]]
+            Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-            - name: typing.Optional[str]. The name of the embed job.
+            * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+            * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+            * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+            * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+            * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
 
-            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
+        truncate : typing.Optional[CreateEmbedJobRequestTruncate]
+            One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
-                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
-                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
-                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
-                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
-            - truncate: typing.Optional[CreateEmbedJobRequestTruncate]. One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CreateEmbedJobResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.embed_jobs.create(
@@ -144,18 +173,20 @@
         if name is not OMIT:
             _request["name"] = name
         if embedding_types is not OMIT:
             _request["embedding_types"] = embedding_types
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -193,34 +224,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> EmbedJob:
         """
         This API retrieves the details about an embed job started by the same user.
 
-        Parameters:
-            - id: str. The ID of the embed job to retrieve.
+        Parameters
+        ----------
+        id : str
+            The ID of the embed job to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        EmbedJob
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.embed_jobs.get(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -256,36 +299,47 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def cancel(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         This API allows users to cancel an active embed job. Once invoked, the embedding process will be terminated, and users will be charged for the embeddings processed up to the cancellation point. It's important to note that partial results will not be available to users after cancellation.
 
-        Parameters:
-            - id: str. The ID of the embed job to cancel.
+        Parameters
+        ----------
+        id : str
+            The ID of the embed job to cancel.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.embed_jobs.cancel(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}/cancel"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
@@ -329,30 +383,41 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def list(self, *, request_options: typing.Optional[RequestOptions] = None) -> ListEmbedJobResponse:
         """
         The list embed job endpoint allows users to view all embed jobs history for that specific user.
 
-        Parameters:
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Parameters
+        ----------
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListEmbedJobResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.embed_jobs.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -394,43 +459,60 @@
         embedding_types: typing.Optional[typing.Sequence[EmbeddingType]] = OMIT,
         truncate: typing.Optional[CreateEmbedJobRequestTruncate] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> CreateEmbedJobResponse:
         """
         This API launches an async Embed job for a [Dataset](https://docs.cohere.com/docs/datasets) of type `embed-input`. The result of a completed embed job is new Dataset of type `embed-output`, which contains the original text entries and the corresponding embeddings.
 
-        Parameters:
-            - model: str. ID of the embedding model.
+        Parameters
+        ----------
+        model : str
+            ID of the embedding model.
+
+            Available models and corresponding embedding dimensions:
+
+            - `embed-english-v3.0` : 1024
+            - `embed-multilingual-v3.0` : 1024
+            - `embed-english-light-v3.0` : 384
+            - `embed-multilingual-light-v3.0` : 384
+
 
-                          Available models and corresponding embedding dimensions:
+        dataset_id : str
+            ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
 
-                          - `embed-english-v3.0` : 1024
-                          - `embed-multilingual-v3.0` : 1024
-                          - `embed-english-light-v3.0` : 384
-                          - `embed-multilingual-light-v3.0` : 384
+        input_type : EmbedInputType
 
-            - dataset_id: str. ID of a [Dataset](https://docs.cohere.com/docs/datasets). The Dataset must be of type `embed-input` and must have a validation status `Validated`
+        name : typing.Optional[str]
+            The name of the embed job.
 
-            - input_type: EmbedInputType.
+        embedding_types : typing.Optional[typing.Sequence[EmbeddingType]]
+            Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
 
-            - name: typing.Optional[str]. The name of the embed job.
+            * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
+            * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
+            * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
+            * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
+            * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
 
-            - embedding_types: typing.Optional[typing.Sequence[EmbeddingType]]. Specifies the types of embeddings you want to get back. Not required and default is None, which returns the Embed Floats response type. Can be one or more of the following types.
+        truncate : typing.Optional[CreateEmbedJobRequestTruncate]
+            One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
 
-                                                                                * `"float"`: Use this when you want to get back the default float embeddings. Valid for all models.
-                                                                                * `"int8"`: Use this when you want to get back signed int8 embeddings. Valid for only v3 models.
-                                                                                * `"uint8"`: Use this when you want to get back unsigned int8 embeddings. Valid for only v3 models.
-                                                                                * `"binary"`: Use this when you want to get back signed binary embeddings. Valid for only v3 models.
-                                                                                * `"ubinary"`: Use this when you want to get back unsigned binary embeddings. Valid for only v3 models.
-            - truncate: typing.Optional[CreateEmbedJobRequestTruncate]. One of `START|END` to specify how the API will handle inputs longer than the maximum token length.
+            Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-                                                                        Passing `START` will discard the start of the input. `END` will discard the end of the input. In both cases, input is discarded until the remaining input is exactly the maximum input token length for the model.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CreateEmbedJobResponse
+            OK
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.embed_jobs.create(
@@ -443,18 +525,20 @@
         if name is not OMIT:
             _request["name"] = name
         if embedding_types is not OMIT:
             _request["embedding_types"] = embedding_types
         if truncate is not OMIT:
             _request["truncate"] = truncate
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "embed-jobs"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -492,34 +576,46 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> EmbedJob:
         """
         This API retrieves the details about an embed job started by the same user.
 
-        Parameters:
-            - id: str. The ID of the embed job to retrieve.
+        Parameters
+        ----------
+        id : str
+            The ID of the embed job to retrieve.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        EmbedJob
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.embed_jobs.get(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -555,36 +651,47 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def cancel(self, id: str, *, request_options: typing.Optional[RequestOptions] = None) -> None:
         """
         This API allows users to cancel an active embed job. Once invoked, the embedding process will be terminated, and users will be charged for the embeddings processed up to the cancellation point. It's important to note that partial results will not be available to users after cancellation.
 
-        Parameters:
-            - id: str. The ID of the embed job to cancel.
+        Parameters
+        ----------
+        id : str
+            The ID of the embed job to cancel.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        None
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.embed_jobs.cancel(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(
+            method="POST",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"embed-jobs/{jsonable_encoder(id)}/cancel"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))
             if request_options is not None
             else None,
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
```

### Comparing `cohere-5.5.0/src/cohere/errors/__init__.py` & `cohere-5.5.1/src/cohere/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/finetuning/__init__.py` & `cohere-5.5.1/src/cohere/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/finetuning/client.py` & `cohere-5.5.1/src/cohere/finetuning/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.forbidden_error import ForbiddenError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.not_found_error import NotFoundError
@@ -42,51 +43,66 @@
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         order_by: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListFinetunedModelsResponse:
         """
-        Parameters:
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
 
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
 
-            - order_by: typing.Optional[str]. Comma separated list of fields. For example: "created_at,name". The default
-                                              sorting order is ascending. To specify descending order for a field, append
-                                              " desc" to the field name. For example: "created_at desc,name".
+        order_by : typing.Optional[str]
+            Comma separated list of fields. For example: "created_at,name". The default
+            sorting order is ascending. To specify descending order for a field, append
+            " desc" to the field name. For example: "created_at desc,name".
 
-                                              Supported sorting fields:
+            Supported sorting fields:
 
-                                              - created_at (default)
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+            - created_at (default)
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListFinetunedModelsResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.finetuning.list_finetuned_models()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "order_by": order_by,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "order_by": order_by,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -131,19 +147,28 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def create_finetuned_model(
         self, *, request: FinetunedModel, request_options: typing.Optional[RequestOptions] = None
     ) -> CreateFinetunedModelResponse:
         """
-        Parameters:
-            - request: FinetunedModel.
+        Parameters
+        ----------
+        request : FinetunedModel
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CreateFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
         from cohere.finetuning import BaseModel, FinetunedModel, Settings
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -156,18 +181,20 @@
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -217,36 +244,48 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def get_finetuned_model(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. The fine-tuned model ID.
+        Parameters
+        ----------
+        id : str
+            The fine-tuned model ID.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.finetuning.get_finetuned_model(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -290,36 +329,48 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def delete_finetuned_model(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. The fine-tuned model ID.
+        Parameters
+        ----------
+        id : str
+            The fine-tuned model ID.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.finetuning.delete_finetuned_model(
             id="id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -364,48 +415,67 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     def update_finetuned_model(
         self,
         id: str,
         *,
         name: str,
+        settings: Settings,
         creator_id: typing.Optional[str] = OMIT,
         organization_id: typing.Optional[str] = OMIT,
-        settings: Settings,
         status: typing.Optional[Status] = OMIT,
         created_at: typing.Optional[dt.datetime] = OMIT,
         updated_at: typing.Optional[dt.datetime] = OMIT,
         completed_at: typing.Optional[dt.datetime] = OMIT,
         last_used: typing.Optional[dt.datetime] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpdateFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. FinetunedModel ID.
+        Parameters
+        ----------
+        id : str
+            FinetunedModel ID.
+
+        name : str
+            FinetunedModel name (e.g. `foobar`).
+
+        settings : Settings
+            FinetunedModel settings such as dataset, hyperparameters...
 
-            - name: str. FinetunedModel name (e.g. `foobar`).
+        creator_id : typing.Optional[str]
+            User ID of the creator.
 
-            - creator_id: typing.Optional[str]. User ID of the creator.
+        organization_id : typing.Optional[str]
+            Organization ID.
 
-            - organization_id: typing.Optional[str]. Organization ID.
+        status : typing.Optional[Status]
+            Current stage in the life-cycle of the fine-tuned model.
 
-            - settings: Settings. FinetunedModel settings such as dataset, hyperparameters...
+        created_at : typing.Optional[dt.datetime]
+            Creation timestamp.
 
-            - status: typing.Optional[Status]. Current stage in the life-cycle of the fine-tuned model.
+        updated_at : typing.Optional[dt.datetime]
+            Latest update timestamp.
 
-            - created_at: typing.Optional[dt.datetime]. Creation timestamp.
+        completed_at : typing.Optional[dt.datetime]
+            Timestamp for the completed fine-tuning.
 
-            - updated_at: typing.Optional[dt.datetime]. Latest update timestamp.
+        last_used : typing.Optional[dt.datetime]
+            Timestamp for the latest request to this fine-tuned model.
 
-            - completed_at: typing.Optional[dt.datetime]. Timestamp for the completed fine-tuning.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - last_used: typing.Optional[dt.datetime]. Timestamp for the latest request to this fine-tuned model.
+        Returns
+        -------
+        UpdateFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
         from cohere.finetuning import BaseModel, Settings
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -432,20 +502,22 @@
         if updated_at is not OMIT:
             _request["updated_at"] = updated_at
         if completed_at is not OMIT:
             _request["completed_at"] = completed_at
         if last_used is not OMIT:
             _request["last_used"] = last_used
         _response = self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -501,58 +573,74 @@
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         order_by: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListEventsResponse:
         """
-        Parameters:
-            - finetuned_model_id: str. The parent fine-tuned model ID.
+        Parameters
+        ----------
+        finetuned_model_id : str
+            The parent fine-tuned model ID.
+
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
+
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
 
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
+        order_by : typing.Optional[str]
+            Comma separated list of fields. For example: "created_at,name". The default
+            sorting order is ascending. To specify descending order for a field, append
+            " desc" to the field name. For example: "created_at desc,name".
 
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+            Supported sorting fields:
 
-            - order_by: typing.Optional[str]. Comma separated list of fields. For example: "created_at,name". The default
-                                              sorting order is ascending. To specify descending order for a field, append
-                                              " desc" to the field name. For example: "created_at desc,name".
+            - created_at (default)
 
-                                              Supported sorting fields:
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-                                              - created_at (default)
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        ListEventsResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.finetuning.list_events(
             finetuned_model_id="finetuned_model_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"finetuning/finetuned-models/{jsonable_encoder(finetuned_model_id)}/events",
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "order_by": order_by,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "order_by": order_by,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -602,50 +690,64 @@
         finetuned_model_id: str,
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListTrainingStepMetricsResponse:
         """
-        Parameters:
-            - finetuned_model_id: str. The parent fine-tuned model ID.
-
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
-
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+        Parameters
+        ----------
+        finetuned_model_id : str
+            The parent fine-tuned model ID.
+
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
+
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTrainingStepMetricsResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.finetuning.list_training_step_metrics(
             finetuned_model_id="finetuned_model_id",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"finetuning/finetuned-models/{jsonable_encoder(finetuned_model_id)}/training-step-metrics",
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -700,51 +802,66 @@
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         order_by: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListFinetunedModelsResponse:
         """
-        Parameters:
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
+        Parameters
+        ----------
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
 
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
 
-            - order_by: typing.Optional[str]. Comma separated list of fields. For example: "created_at,name". The default
-                                              sorting order is ascending. To specify descending order for a field, append
-                                              " desc" to the field name. For example: "created_at desc,name".
+        order_by : typing.Optional[str]
+            Comma separated list of fields. For example: "created_at,name". The default
+            sorting order is ascending. To specify descending order for a field, append
+            " desc" to the field name. For example: "created_at desc,name".
 
-                                              Supported sorting fields:
+            Supported sorting fields:
 
-                                              - created_at (default)
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+            - created_at (default)
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListFinetunedModelsResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.finetuning.list_finetuned_models()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "order_by": order_by,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "order_by": order_by,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -789,19 +906,28 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def create_finetuned_model(
         self, *, request: FinetunedModel, request_options: typing.Optional[RequestOptions] = None
     ) -> CreateFinetunedModelResponse:
         """
-        Parameters:
-            - request: FinetunedModel.
+        Parameters
+        ----------
+        request : FinetunedModel
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        CreateFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
         from cohere.finetuning import BaseModel, FinetunedModel, Settings
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -814,18 +940,20 @@
                     ),
                     dataset_id="my-dataset-id",
                 ),
             ),
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "POST",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="POST",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "finetuning/finetuned-models"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -875,36 +1003,48 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def get_finetuned_model(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> GetFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. The fine-tuned model ID.
+        Parameters
+        ----------
+        id : str
+            The fine-tuned model ID.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.finetuning.get_finetuned_model(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -948,36 +1088,48 @@
             raise ApiError(status_code=_response.status_code, body=_response.text)
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def delete_finetuned_model(
         self, id: str, *, request_options: typing.Optional[RequestOptions] = None
     ) -> DeleteFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. The fine-tuned model ID.
+        Parameters
+        ----------
+        id : str
+            The fine-tuned model ID.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        DeleteFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.finetuning.delete_finetuned_model(
             id="id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "DELETE",
-            urllib.parse.urljoin(
+            method="DELETE",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -1022,48 +1174,67 @@
         raise ApiError(status_code=_response.status_code, body=_response_json)
 
     async def update_finetuned_model(
         self,
         id: str,
         *,
         name: str,
+        settings: Settings,
         creator_id: typing.Optional[str] = OMIT,
         organization_id: typing.Optional[str] = OMIT,
-        settings: Settings,
         status: typing.Optional[Status] = OMIT,
         created_at: typing.Optional[dt.datetime] = OMIT,
         updated_at: typing.Optional[dt.datetime] = OMIT,
         completed_at: typing.Optional[dt.datetime] = OMIT,
         last_used: typing.Optional[dt.datetime] = OMIT,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> UpdateFinetunedModelResponse:
         """
-        Parameters:
-            - id: str. FinetunedModel ID.
+        Parameters
+        ----------
+        id : str
+            FinetunedModel ID.
+
+        name : str
+            FinetunedModel name (e.g. `foobar`).
+
+        settings : Settings
+            FinetunedModel settings such as dataset, hyperparameters...
 
-            - name: str. FinetunedModel name (e.g. `foobar`).
+        creator_id : typing.Optional[str]
+            User ID of the creator.
 
-            - creator_id: typing.Optional[str]. User ID of the creator.
+        organization_id : typing.Optional[str]
+            Organization ID.
 
-            - organization_id: typing.Optional[str]. Organization ID.
+        status : typing.Optional[Status]
+            Current stage in the life-cycle of the fine-tuned model.
 
-            - settings: Settings. FinetunedModel settings such as dataset, hyperparameters...
+        created_at : typing.Optional[dt.datetime]
+            Creation timestamp.
 
-            - status: typing.Optional[Status]. Current stage in the life-cycle of the fine-tuned model.
+        updated_at : typing.Optional[dt.datetime]
+            Latest update timestamp.
 
-            - created_at: typing.Optional[dt.datetime]. Creation timestamp.
+        completed_at : typing.Optional[dt.datetime]
+            Timestamp for the completed fine-tuning.
 
-            - updated_at: typing.Optional[dt.datetime]. Latest update timestamp.
+        last_used : typing.Optional[dt.datetime]
+            Timestamp for the latest request to this fine-tuned model.
 
-            - completed_at: typing.Optional[dt.datetime]. Timestamp for the completed fine-tuning.
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-            - last_used: typing.Optional[dt.datetime]. Timestamp for the latest request to this fine-tuned model.
+        Returns
+        -------
+        UpdateFinetunedModelResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
         from cohere.finetuning import BaseModel, Settings
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
@@ -1090,20 +1261,22 @@
         if updated_at is not OMIT:
             _request["updated_at"] = updated_at
         if completed_at is not OMIT:
             _request["completed_at"] = completed_at
         if last_used is not OMIT:
             _request["last_used"] = last_used
         _response = await self._client_wrapper.httpx_client.request(
-            "PATCH",
-            urllib.parse.urljoin(
+            method="PATCH",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/", f"finetuning/finetuned-models/{jsonable_encoder(id)}"
             ),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             json=jsonable_encoder(_request)
             if request_options is None or request_options.get("additional_body_parameters") is None
             else {
                 **jsonable_encoder(_request),
                 **(jsonable_encoder(remove_none_from_dict(request_options.get("additional_body_parameters", {})))),
             },
@@ -1159,58 +1332,74 @@
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         order_by: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListEventsResponse:
         """
-        Parameters:
-            - finetuned_model_id: str. The parent fine-tuned model ID.
+        Parameters
+        ----------
+        finetuned_model_id : str
+            The parent fine-tuned model ID.
+
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
+
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
 
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
+        order_by : typing.Optional[str]
+            Comma separated list of fields. For example: "created_at,name". The default
+            sorting order is ascending. To specify descending order for a field, append
+            " desc" to the field name. For example: "created_at desc,name".
 
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+            Supported sorting fields:
 
-            - order_by: typing.Optional[str]. Comma separated list of fields. For example: "created_at,name". The default
-                                              sorting order is ascending. To specify descending order for a field, append
-                                              " desc" to the field name. For example: "created_at desc,name".
+            - created_at (default)
 
-                                              Supported sorting fields:
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
 
-                                              - created_at (default)
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Returns
+        -------
+        ListEventsResponse
+            A successful response.
+
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.finetuning.list_events(
             finetuned_model_id="finetuned_model_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"finetuning/finetuned-models/{jsonable_encoder(finetuned_model_id)}/events",
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "order_by": order_by,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "order_by": order_by,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -1260,50 +1449,64 @@
         finetuned_model_id: str,
         *,
         page_size: typing.Optional[int] = None,
         page_token: typing.Optional[str] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListTrainingStepMetricsResponse:
         """
-        Parameters:
-            - finetuned_model_id: str. The parent fine-tuned model ID.
-
-            - page_size: typing.Optional[int]. Maximum number of results to be returned by the server. If 0, defaults to 50.
-
-            - page_token: typing.Optional[str]. Request a specific page of the list results.
+        Parameters
+        ----------
+        finetuned_model_id : str
+            The parent fine-tuned model ID.
+
+        page_size : typing.Optional[int]
+            Maximum number of results to be returned by the server. If 0, defaults to 50.
+
+        page_token : typing.Optional[str]
+            Request a specific page of the list results.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListTrainingStepMetricsResponse
+            A successful response.
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.finetuning.list_training_step_metrics(
             finetuned_model_id="finetuned_model_id",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(
+            method="GET",
+            url=urllib.parse.urljoin(
                 f"{self._client_wrapper.get_base_url()}/",
                 f"finetuning/finetuned-models/{jsonable_encoder(finetuned_model_id)}/training-step-metrics",
             ),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/__init__.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/__init__.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/base_model.py` & `cohere-5.5.1/src/cohere/types/chat_search_query.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from ....core.unchecked_base_model import UncheckedBaseModel
-from .base_type import BaseType
-from .strategy import Strategy
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class BaseModel(UncheckedBaseModel):
+class ChatSearchQuery(UncheckedBaseModel):
     """
-    The base model used for fine-tuning.
+    The generated search query. Contains the text of the query and a unique identifier for the query.
     """
 
-    name: typing.Optional[str] = pydantic_v1.Field(default=None)
+    text: str = pydantic_v1.Field()
     """
-    The name of the base model.
+    The text of the search query.
     """
 
-    version: typing.Optional[str] = pydantic_v1.Field(default=None)
+    generation_id: str = pydantic_v1.Field()
     """
-    read-only. The version of the base model.
-    """
-
-    base_type: BaseType = pydantic_v1.Field()
-    """
-    The type of the base model.
-    """
-
-    strategy: typing.Optional[Strategy] = pydantic_v1.Field(default=None)
-    """
-    The fine-tuning strategy.
+    Unique identifier for the generated search query. Useful for submitting feedback.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class CreateFinetunedModelResponse(UncheckedBaseModel):
+class ListFinetunedModelsResponse(UncheckedBaseModel):
     """
-    Response to request to create a fine-tuned model.
+    Response to a request to list fine-tuned models.
     """
 
-    finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
+    finetuned_models: typing.Optional[typing.List[FinetunedModel]] = pydantic_v1.Field(default=None)
     """
-    Information about the fine-tuned model.
+    List of fine-tuned models matching the request.
+    """
+
+    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Pagination token to retrieve the next page of results. If the value is "",
+    it means no further results for the request.
+    """
+
+    total_size: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Total count of results.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/error.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/error.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 
 
 class Error(UncheckedBaseModel):
     """
     Error is the response for any unsuccessful event.
     """
@@ -19,15 +19,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/event.py` & `cohere-5.5.1/src/cohere/types/api_meta_tokens.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from ....core.unchecked_base_model import UncheckedBaseModel
-from .status import Status
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class Event(UncheckedBaseModel):
+class ApiMetaTokens(UncheckedBaseModel):
+    input_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    A change in status of a fine-tuned model.
+    The number of tokens used as input to the model.
     """
 
-    user_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+    output_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    ID of the user who initiated the event. Empty if initiated by the system.
-    """
-
-    status: typing.Optional[Status] = pydantic_v1.Field(default=None)
-    """
-    Status of the fine-tuned model.
-    """
-
-    created_at: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
-    """
-    Timestamp when the event happened.
+    The number of tokens produced by the model.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/finetuned_model.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/finetuned_model.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 from .settings import Settings
 from .status import Status
 
 
 class FinetunedModel(UncheckedBaseModel):
     """
@@ -66,15 +66,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_events_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,49 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
-from .finetuned_model import FinetunedModel
+from .event import Event
 
 
-class GetFinetunedModelResponse(UncheckedBaseModel):
+class ListEventsResponse(UncheckedBaseModel):
     """
-    Response to a request to get a fine-tuned model.
+    Response to a request to list events of a fine-tuned model.
     """
 
-    finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
+    events: typing.Optional[typing.List[Event]] = pydantic_v1.Field(default=None)
     """
-    Information about the fine-tuned model.
+    List of events for the fine-tuned model.
+    """
+
+    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    Pagination token to retrieve the next page of results. If the value is "",
+    it means no further results for the request.
+    """
+
+    total_size: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Total count of results.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/hyperparameters.py` & `cohere-5.5.1/src/cohere/types/chat_connector.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from ....core.unchecked_base_model import UncheckedBaseModel
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class Hyperparameters(UncheckedBaseModel):
+class ChatConnector(UncheckedBaseModel):
     """
-    The fine-tuning hyperparameters.
+    The connector used for fetching documents.
     """
 
-    early_stopping_patience: typing.Optional[int] = pydantic_v1.Field(default=None)
+    id: str = pydantic_v1.Field()
     """
-    Stops training if the loss metric does not improve beyond the value of
-    `early_stopping_threshold` after this many times of evaluation.
+    The identifier of the connector.
     """
 
-    early_stopping_threshold: typing.Optional[float] = pydantic_v1.Field(default=None)
+    user_access_token: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    How much the loss must improve to prevent early stopping.
+    When specified, this user access token will be passed to the connector in the Authorization header instead of the Cohere generated one.
     """
 
-    train_batch_size: typing.Optional[int] = pydantic_v1.Field(default=None)
+    continue_on_failure: typing.Optional[bool] = pydantic_v1.Field(default=None)
     """
-    The batch size is the number of training examples included in a single
-    training pass.
+    Defaults to `false`.
+    
+    When `true`, the request will continue if this connector returned an error.
     """
 
-    train_epochs: typing.Optional[int] = pydantic_v1.Field(default=None)
+    options: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
     """
-    The number of epochs to train for.
-    """
-
-    learning_rate: typing.Optional[float] = pydantic_v1.Field(default=None)
-    """
-    The learning rate to be used during training.
+    Provides the connector with different settings at request time. The key/value pairs of this object are specific to each connector.
+    
+    For example, the connector `web-search` supports the `site` option, which limits search results to the specified domain.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_events_response.py` & `cohere-5.5.1/src/cohere/types/rerank_response_results_item.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from ....core.unchecked_base_model import UncheckedBaseModel
-from .event import Event
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .rerank_response_results_item_document import RerankResponseResultsItemDocument
 
 
-class ListEventsResponse(UncheckedBaseModel):
+class RerankResponseResultsItem(UncheckedBaseModel):
+    document: typing.Optional[RerankResponseResultsItemDocument] = pydantic_v1.Field(default=None)
     """
-    Response to a request to list events of a fine-tuned model.
+    If `return_documents` is set as `false` this will return none, if `true` it will return the documents passed in
     """
 
-    events: typing.Optional[typing.List[Event]] = pydantic_v1.Field(default=None)
+    index: int = pydantic_v1.Field()
     """
-    List of events for the fine-tuned model.
+    Corresponds to the index in the original list of documents to which the ranked document belongs. (i.e. if the first value in the `results` object has an `index` value of 3, it means in the list of documents passed in, the document at `index=3` had the highest relevance)
     """
 
-    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
+    relevance_score: float = pydantic_v1.Field()
     """
-    Pagination token to retrieve the next page of results. If the value is "",
-    it means no further results for the request.
-    """
-
-    total_size: typing.Optional[int] = pydantic_v1.Field(default=None)
-    """
-    Total count of results.
+    Relevance scores are normalized to be in the range `[0, 1]`. Scores close to `1` indicate a high relevance to the query, and scores closer to `0` indicate low relevance. It is not accurate to assume a score of 0.9 means the document is 2x more relevant than a document with a score of 0.45
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_finetuned_models_response.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,45 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class ListFinetunedModelsResponse(UncheckedBaseModel):
+class UpdateFinetunedModelResponse(UncheckedBaseModel):
     """
-    Response to a request to list fine-tuned models.
+    Response to a request to update a fine-tuned model.
     """
 
-    finetuned_models: typing.Optional[typing.List[FinetunedModel]] = pydantic_v1.Field(default=None)
+    finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
     """
-    List of fine-tuned models matching the request.
-    """
-
-    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    Pagination token to retrieve the next page of results. If the value is "",
-    it means no further results for the request.
-    """
-
-    total_size: typing.Optional[int] = pydantic_v1.Field(default=None)
-    """
-    Total count of results.
+    Information about the fine-tuned model.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py` & `cohere-5.5.1/src/cohere/types/o_auth_authorize_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,40 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
-from ....core.unchecked_base_model import UncheckedBaseModel
-from .training_step_metrics import TrainingStepMetrics
+from ..core.datetime_utils import serialize_datetime
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ListTrainingStepMetricsResponse(UncheckedBaseModel):
+class OAuthAuthorizeResponse(UncheckedBaseModel):
+    redirect_url: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Response to a request to list training-step metrics of a fine-tuned model.
-    """
-
-    step_metrics: typing.Optional[typing.List[TrainingStepMetrics]] = pydantic_v1.Field(default=None)
-    """
-    The metrics for each step the evaluation was run on.
-    """
-
-    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    Pagination token to retrieve the next page of results. If the value is "",
-    it means no further results for the request.
+    The OAuth 2.0 redirect url. Redirect the user to this url to authorize the connector.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/settings.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 from .base_model import BaseModel
 from .hyperparameters import Hyperparameters
 
 
 class Settings(UncheckedBaseModel):
     """
@@ -36,15 +36,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/training_step_metrics.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/base_model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,54 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
+from .base_type import BaseType
+from .strategy import Strategy
 
 
-class TrainingStepMetrics(UncheckedBaseModel):
+class BaseModel(UncheckedBaseModel):
     """
-    The evaluation metrics at a given step of the training of a fine-tuned model.
+    The base model used for fine-tuning.
     """
 
-    created_at: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
+    name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Creation timestamp.
+    The name of the base model.
     """
 
-    step_number: typing.Optional[int] = pydantic_v1.Field(default=None)
+    version: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Step number.
+    read-only. The version of the base model.
     """
 
-    metrics: typing.Optional[typing.Dict[str, float]] = pydantic_v1.Field(default=None)
+    base_type: BaseType = pydantic_v1.Field()
     """
-    Map of names and values for each evaluation metrics.
+    The type of the base model.
+    """
+
+    strategy: typing.Optional[Strategy] = pydantic_v1.Field(default=None)
+    """
+    The fine-tuning strategy.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/finetuning/finetuning/types/update_finetuned_model_response.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/get_finetuned_model_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ....core.datetime_utils import serialize_datetime
-from ....core.pydantic_utilities import pydantic_v1
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ....core.unchecked_base_model import UncheckedBaseModel
 from .finetuned_model import FinetunedModel
 
 
-class UpdateFinetunedModelResponse(UncheckedBaseModel):
+class GetFinetunedModelResponse(UncheckedBaseModel):
     """
-    Response to a request to update a fine-tuned model.
+    Response to a request to get a fine-tuned model.
     """
 
     finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
     """
     Information about the fine-tuned model.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/manually_maintained/cache.py` & `cohere-5.5.1/src/cohere/manually_maintained/cache.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/manually_maintained/tokenizers.py` & `cohere-5.5.1/src/cohere/manually_maintained/tokenizers.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/models/client.py` & `cohere-5.5.1/src/cohere/models/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import typing
 import urllib.parse
 from json.decoder import JSONDecodeError
 
 from ..core.api_error import ApiError
 from ..core.client_wrapper import AsyncClientWrapper, SyncClientWrapper
 from ..core.jsonable_encoder import jsonable_encoder
+from ..core.query_encoder import encode_query
 from ..core.remove_none_from_dict import remove_none_from_dict
 from ..core.request_options import RequestOptions
 from ..core.unchecked_base_model import construct_type
 from ..errors.bad_request_error import BadRequestError
 from ..errors.internal_server_error import InternalServerError
 from ..errors.too_many_requests_error import TooManyRequestsError
 from ..types.compatible_endpoint import CompatibleEndpoint
@@ -23,34 +24,45 @@
     def __init__(self, *, client_wrapper: SyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     def get(self, model: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetModelResponse:
         """
         Returns the details of a model, provided its name.
 
-        Parameters:
-            - model: str.
+        Parameters
+        ----------
+        model : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetModelResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.models.get(
             model="model",
         )
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"models/{jsonable_encoder(model)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"models/{jsonable_encoder(model)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -90,49 +102,65 @@
         endpoint: typing.Optional[CompatibleEndpoint] = None,
         default_only: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListModelsResponse:
         """
         Returns a list of models available for use. The list contains models from Cohere as well as your fine-tuned models.
 
-        Parameters:
-            - page_size: typing.Optional[float]. Maximum number of models to include in a page
-                                                 Defaults to `20`, min value of `1`, max value of `1000`.
-            - page_token: typing.Optional[str]. Page token provided in the `next_page_token` field of a previous response.
-
-            - endpoint: typing.Optional[CompatibleEndpoint]. When provided, filters the list of models to only those that are compatible with the specified endpoint.
-
-            - default_only: typing.Optional[bool]. When provided, filters the list of models to only the default model to the endpoint. This parameter is only valid when `endpoint` is provided.
+        Parameters
+        ----------
+        page_size : typing.Optional[float]
+            Maximum number of models to include in a page
+            Defaults to `20`, min value of `1`, max value of `1000`.
+
+        page_token : typing.Optional[str]
+            Page token provided in the `next_page_token` field of a previous response.
+
+        endpoint : typing.Optional[CompatibleEndpoint]
+            When provided, filters the list of models to only those that are compatible with the specified endpoint.
+
+        default_only : typing.Optional[bool]
+            When provided, filters the list of models to only the default model to the endpoint. This parameter is only valid when `endpoint` is provided.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListModelsResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import Client
 
         client = Client(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         client.models.list()
         """
         _response = self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "models"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "endpoint": endpoint,
-                        "default_only": default_only,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "models"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "endpoint": endpoint,
+                            "default_only": default_only,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
@@ -162,34 +190,45 @@
     def __init__(self, *, client_wrapper: AsyncClientWrapper):
         self._client_wrapper = client_wrapper
 
     async def get(self, model: str, *, request_options: typing.Optional[RequestOptions] = None) -> GetModelResponse:
         """
         Returns the details of a model, provided its name.
 
-        Parameters:
-            - model: str.
+        Parameters
+        ----------
+        model : str
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        GetModelResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.models.get(
             model="model",
         )
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"models/{jsonable_encoder(model)}"),
-            params=jsonable_encoder(
-                request_options.get("additional_query_parameters") if request_options is not None else None
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", f"models/{jsonable_encoder(model)}"),
+            params=encode_query(
+                jsonable_encoder(
+                    request_options.get("additional_query_parameters") if request_options is not None else None
+                )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
                     }
@@ -229,49 +268,65 @@
         endpoint: typing.Optional[CompatibleEndpoint] = None,
         default_only: typing.Optional[bool] = None,
         request_options: typing.Optional[RequestOptions] = None,
     ) -> ListModelsResponse:
         """
         Returns a list of models available for use. The list contains models from Cohere as well as your fine-tuned models.
 
-        Parameters:
-            - page_size: typing.Optional[float]. Maximum number of models to include in a page
-                                                 Defaults to `20`, min value of `1`, max value of `1000`.
-            - page_token: typing.Optional[str]. Page token provided in the `next_page_token` field of a previous response.
-
-            - endpoint: typing.Optional[CompatibleEndpoint]. When provided, filters the list of models to only those that are compatible with the specified endpoint.
-
-            - default_only: typing.Optional[bool]. When provided, filters the list of models to only the default model to the endpoint. This parameter is only valid when `endpoint` is provided.
+        Parameters
+        ----------
+        page_size : typing.Optional[float]
+            Maximum number of models to include in a page
+            Defaults to `20`, min value of `1`, max value of `1000`.
+
+        page_token : typing.Optional[str]
+            Page token provided in the `next_page_token` field of a previous response.
+
+        endpoint : typing.Optional[CompatibleEndpoint]
+            When provided, filters the list of models to only those that are compatible with the specified endpoint.
+
+        default_only : typing.Optional[bool]
+            When provided, filters the list of models to only the default model to the endpoint. This parameter is only valid when `endpoint` is provided.
+
+        request_options : typing.Optional[RequestOptions]
+            Request-specific configuration.
+
+        Returns
+        -------
+        ListModelsResponse
+            OK
 
-            - request_options: typing.Optional[RequestOptions]. Request-specific configuration.
-        ---
+        Examples
+        --------
         from cohere.client import AsyncClient
 
         client = AsyncClient(
             client_name="YOUR_CLIENT_NAME",
             token="YOUR_TOKEN",
         )
         await client.models.list()
         """
         _response = await self._client_wrapper.httpx_client.request(
-            "GET",
-            urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "models"),
-            params=jsonable_encoder(
-                remove_none_from_dict(
-                    {
-                        "page_size": page_size,
-                        "page_token": page_token,
-                        "endpoint": endpoint,
-                        "default_only": default_only,
-                        **(
-                            request_options.get("additional_query_parameters", {})
-                            if request_options is not None
-                            else {}
-                        ),
-                    }
+            method="GET",
+            url=urllib.parse.urljoin(f"{self._client_wrapper.get_base_url()}/", "models"),
+            params=encode_query(
+                jsonable_encoder(
+                    remove_none_from_dict(
+                        {
+                            "page_size": page_size,
+                            "page_token": page_token,
+                            "endpoint": endpoint,
+                            "default_only": default_only,
+                            **(
+                                request_options.get("additional_query_parameters", {})
+                                if request_options is not None
+                                else {}
+                            ),
+                        }
+                    )
                 )
             ),
             headers=jsonable_encoder(
                 remove_none_from_dict(
                     {
                         **self._client_wrapper.get_headers(),
                         **(request_options.get("additional_headers", {}) if request_options is not None else {}),
```

### Comparing `cohere-5.5.0/src/cohere/overrides.py` & `cohere-5.5.1/src/cohere/overrides.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/types/__init__.py` & `cohere-5.5.1/src/cohere/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/src/cohere/types/api_meta.py` & `cohere-5.5.1/src/cohere/types/api_meta.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta_api_version import ApiMetaApiVersion
 from .api_meta_billed_units import ApiMetaBilledUnits
 from .api_meta_tokens import ApiMetaTokens
 
 
 class ApiMeta(UncheckedBaseModel):
@@ -18,15 +18,19 @@
     warnings: typing.Optional[typing.List[str]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/api_meta_api_version.py` & `cohere-5.5.1/src/cohere/types/update_connector_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .connector import Connector
 
 
-class ApiMetaApiVersion(UncheckedBaseModel):
-    version: str
-    is_deprecated: typing.Optional[bool] = None
-    is_experimental: typing.Optional[bool] = None
+class UpdateConnectorResponse(UncheckedBaseModel):
+    connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/api_meta_billed_units.py` & `cohere-5.5.1/src/cohere/types/api_meta_billed_units.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class ApiMetaBilledUnits(UncheckedBaseModel):
     input_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
     The number of billed input tokens.
@@ -30,15 +30,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/api_meta_tokens.py` & `cohere-5.5.1/src/cohere/types/chat_data_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ApiMetaTokens(UncheckedBaseModel):
-    input_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
+class ChatDataMetrics(UncheckedBaseModel):
+    num_train_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    The number of tokens used as input to the model.
+    The sum of all turns of valid train examples.
     """
 
-    output_tokens: typing.Optional[float] = pydantic_v1.Field(default=None)
+    num_eval_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    The number of tokens produced by the model.
+    The sum of all turns of valid eval examples.
+    """
+
+    preamble: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The preamble of this dataset.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_citation.py` & `cohere-5.5.1/src/cohere/types/chat_citation.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class ChatCitation(UncheckedBaseModel):
     """
     A section of the generated reply which cites external knowledge.
     """
@@ -34,15 +34,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_citation_generation_event.py` & `cohere-5.5.1/src/cohere/types/chat_citation_generation_event.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_citation import ChatCitation
 from .chat_stream_event import ChatStreamEvent
 
 
 class ChatCitationGenerationEvent(ChatStreamEvent):
     citations: typing.List[ChatCitation] = pydantic_v1.Field()
     """
@@ -16,16 +16,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_connector.py` & `cohere-5.5.1/src/cohere/types/connector_o_auth.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatConnector(UncheckedBaseModel):
+class ConnectorOAuth(UncheckedBaseModel):
+    client_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The connector used for fetching documents.
+    The OAuth 2.0 client ID. This field is encrypted at rest.
     """
 
-    id: str = pydantic_v1.Field()
+    client_secret: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The identifier of the connector.
+    The OAuth 2.0 client Secret. This field is encrypted at rest and never returned in a response.
     """
 
-    user_access_token: typing.Optional[str] = pydantic_v1.Field(default=None)
+    authorize_url: str = pydantic_v1.Field()
     """
-    When specified, this user access token will be passed to the connector in the Authorization header instead of the Cohere generated one.
+    The OAuth 2.0 /authorize endpoint to use when users authorize the connector.
     """
 
-    continue_on_failure: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    token_url: str = pydantic_v1.Field()
     """
-    Defaults to `false`.
-    
-    When `true`, the request will continue if this connector returned an error.
+    The OAuth 2.0 /token endpoint to use when users authorize the connector.
     """
 
-    options: typing.Optional[typing.Dict[str, typing.Any]] = pydantic_v1.Field(default=None)
+    scope: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Provides the connector with different settings at request time. The key/value pairs of this object are specific to each connector.
-    
-    For example, the connector `web-search` supports the `site` option, which limits search results to the specified domain.
+    The OAuth scopes to request when users authorize the connector.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_data_metrics.py` & `cohere-5.5.1/src/cohere/types/tool_message.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .tool_result import ToolResult
 
 
-class ChatDataMetrics(UncheckedBaseModel):
-    num_train_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
+class ToolMessage(UncheckedBaseModel):
     """
-    The sum of all turns of valid train examples.
+    Represents tool result in the chat history.
     """
 
-    num_eval_turns: typing.Optional[int] = pydantic_v1.Field(default=None)
-    """
-    The sum of all turns of valid eval examples.
-    """
-
-    preamble: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The preamble of this dataset.
-    """
+    tool_results: typing.Optional[typing.List[ToolResult]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_message.py` & `cohere-5.5.1/src/cohere/types/chat_message.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,19 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .tool_call import ToolCall
 
 
 class ChatMessage(UncheckedBaseModel):
-
-    def __init__(self, **kwargs):
-        super().__init__(**kwargs)
-        self.__fields_set__.add("role")
-
     """
     Represents a single message in the chat history, excluding the current user turn. It has two properties: `role` and `message`. The `role` identifies the sender (`CHATBOT`, `SYSTEM`, or `USER`), while the `message` contains the text content.
 
     The chat_history parameter should not be used for `SYSTEM` messages in most cases. Instead, to add a `SYSTEM` role message at the beginning of a conversation, the `preamble` parameter should be used.
     """
 
     message: str = pydantic_v1.Field()
@@ -29,15 +24,19 @@
     tool_calls: typing.Optional[typing.List[ToolCall]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_request_connectors_search_options.py` & `cohere-5.5.1/src/cohere/types/chat_stream_request_connectors_search_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatRequestConnectorsSearchOptions(UncheckedBaseModel):
+class ChatStreamRequestConnectorsSearchOptions(UncheckedBaseModel):
     """
     (internal) Sets inference and model options for RAG search query and tool use generations. Defaults are used when options are not specified here, meaning that other parameters outside of connectors_search_options are ignored (such as model= or temperature=).
     """
 
     model: typing.Optional[typing.Any] = None
     temperature: typing.Optional[typing.Any] = None
     max_tokens: typing.Optional[typing.Any] = None
@@ -23,15 +23,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_search_queries_generation_event.py` & `cohere-5.5.1/src/cohere/types/chat_search_queries_generation_event.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_search_query import ChatSearchQuery
 from .chat_stream_event import ChatStreamEvent
 
 
 class ChatSearchQueriesGenerationEvent(ChatStreamEvent):
     search_queries: typing.List[ChatSearchQuery] = pydantic_v1.Field()
     """
@@ -16,16 +16,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_search_query.py` & `cohere-5.5.1/src/cohere/types/rerank_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
+from .rerank_response_results_item import RerankResponseResultsItem
 
 
-class ChatSearchQuery(UncheckedBaseModel):
+class RerankResponse(UncheckedBaseModel):
+    id: typing.Optional[str] = None
+    results: typing.List[RerankResponseResultsItem] = pydantic_v1.Field()
     """
-    The generated search query. Contains the text of the query and a unique identifier for the query.
+    An ordered list of ranked documents
     """
 
-    text: str = pydantic_v1.Field()
-    """
-    The text of the search query.
-    """
-
-    generation_id: str = pydantic_v1.Field()
-    """
-    Unique identifier for the generated search query. Useful for submitting feedback.
-    """
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_search_result.py` & `cohere-5.5.1/src/cohere/types/chat_search_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result_connector import ChatSearchResultConnector
 
 
 class ChatSearchResult(UncheckedBaseModel):
     search_query: typing.Optional[ChatSearchQuery] = None
@@ -33,15 +33,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_search_result_connector.py` & `cohere-5.5.1/src/cohere/types/chat_search_result_connector.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class ChatSearchResultConnector(UncheckedBaseModel):
     """
     The connector used for fetching documents.
     """
@@ -19,15 +19,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_search_results_event.py` & `cohere-5.5.1/src/cohere/types/chat_stream_start_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,37 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .chat_document import ChatDocument
-from .chat_search_result import ChatSearchResult
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_stream_event import ChatStreamEvent
 
 
-class ChatSearchResultsEvent(ChatStreamEvent):
-    search_results: typing.Optional[typing.List[ChatSearchResult]] = pydantic_v1.Field(default=None)
+class ChatStreamStartEvent(ChatStreamEvent):
+    generation_id: str = pydantic_v1.Field()
     """
-    Conducted searches and the ids of documents retrieved from each of them.
-    """
-
-    documents: typing.Optional[typing.List[ChatDocument]] = pydantic_v1.Field(default=None)
-    """
-    Documents fetched from searches or provided by the user.
+    Unique identifier for the generated reply. Useful for submitting feedback.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_stream_end_event.py` & `cohere-5.5.1/src/cohere/types/chat_stream_end_event.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_stream_end_event_finish_reason import ChatStreamEndEventFinishReason
 from .chat_stream_event import ChatStreamEvent
 from .non_streamed_chat_response import NonStreamedChatResponse
 
 
 class ChatStreamEndEvent(ChatStreamEvent):
     finish_reason: ChatStreamEndEventFinishReason = pydantic_v1.Field()
@@ -26,16 +26,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_stream_event.py` & `cohere-5.5.1/src/cohere/types/chat_stream_event.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class ChatStreamEvent(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_stream_request_connectors_search_options.py` & `cohere-5.5.1/src/cohere/types/chat_request_connectors_search_options.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatStreamRequestConnectorsSearchOptions(UncheckedBaseModel):
+class ChatRequestConnectorsSearchOptions(UncheckedBaseModel):
     """
     (internal) Sets inference and model options for RAG search query and tool use generations. Defaults are used when options are not specified here, meaning that other parameters outside of connectors_search_options are ignored (such as model= or temperature=).
     """
 
     model: typing.Optional[typing.Any] = None
     temperature: typing.Optional[typing.Any] = None
     max_tokens: typing.Optional[typing.Any] = None
@@ -23,15 +23,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_stream_start_event.py` & `cohere-5.5.1/src/cohere/types/rerank_request_documents_item_text.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .chat_stream_event import ChatStreamEvent
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ChatStreamStartEvent(ChatStreamEvent):
-    generation_id: str = pydantic_v1.Field()
+class RerankRequestDocumentsItemText(UncheckedBaseModel):
+    text: str = pydantic_v1.Field()
     """
-    Unique identifier for the generated reply. Useful for submitting feedback.
+    The text of the document to rerank.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_text_generation_event.py` & `cohere-5.5.1/src/cohere/types/chat_text_generation_event.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_stream_event import ChatStreamEvent
 
 
 class ChatTextGenerationEvent(ChatStreamEvent):
     text: str = pydantic_v1.Field()
     """
     The next batch of text generated by the model.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/chat_tool_calls_generation_event.py` & `cohere-5.5.1/src/cohere/types/chat_tool_calls_generation_event.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .chat_stream_event import ChatStreamEvent
 from .tool_call import ToolCall
 
 
 class ChatToolCallsGenerationEvent(ChatStreamEvent):
     tool_calls: typing.List[ToolCall]
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/check_api_key_response.py` & `cohere-5.5.1/src/cohere/types/classify_example.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class CheckApiKeyResponse(UncheckedBaseModel):
-    valid: bool
-    organization_id: typing.Optional[str] = None
-    owner_id: typing.Optional[str] = None
+class ClassifyExample(UncheckedBaseModel):
+    text: typing.Optional[str] = None
+    label: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/classify_data_metrics.py` & `cohere-5.5.1/src/cohere/datasets/types/datasets_get_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
-from .label_metric import LabelMetric
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
+from ...types.dataset import Dataset
 
 
-class ClassifyDataMetrics(UncheckedBaseModel):
-    label_metrics: typing.Optional[typing.List[LabelMetric]] = None
+class DatasetsGetResponse(UncheckedBaseModel):
+    dataset: Dataset
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/classify_example.py` & `cohere-5.5.1/src/cohere/types/tokenize_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
 
 
-class ClassifyExample(UncheckedBaseModel):
-    text: typing.Optional[str] = None
-    label: typing.Optional[str] = None
+class TokenizeResponse(UncheckedBaseModel):
+    tokens: typing.List[int] = pydantic_v1.Field()
+    """
+    An array of tokens, where each token is an integer.
+    """
+
+    token_strings: typing.List[str]
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/classify_response.py` & `cohere-5.5.1/src/cohere/types/classify_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 from .classify_response_classifications_item import ClassifyResponseClassificationsItem
 
 
 class ClassifyResponse(UncheckedBaseModel):
     id: str
@@ -16,15 +16,19 @@
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/classify_response_classifications_item.py` & `cohere-5.5.1/src/cohere/types/classify_response_classifications_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .classify_response_classifications_item_classification_type import (
     ClassifyResponseClassificationsItemClassificationType,
 )
 from .classify_response_classifications_item_labels_value import ClassifyResponseClassificationsItemLabelsValue
 
 
@@ -50,15 +50,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/classify_response_classifications_item_labels_value.py` & `cohere-5.5.1/src/cohere/types/generate_stream_end_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .single_generation_in_stream import SingleGenerationInStream
 
 
-class ClassifyResponseClassificationsItemLabelsValue(UncheckedBaseModel):
-    confidence: typing.Optional[float] = None
+class GenerateStreamEndResponse(UncheckedBaseModel):
+    id: str
+    prompt: typing.Optional[str] = None
+    generations: typing.Optional[typing.List[SingleGenerationInStream]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/connector.py` & `cohere-5.5.1/src/cohere/types/connector.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .connector_auth_status import ConnectorAuthStatus
 from .connector_o_auth import ConnectorOAuth
 
 
 class Connector(UncheckedBaseModel):
     """
@@ -84,15 +84,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/connector_o_auth.py` & `cohere-5.5.1/src/cohere/types/summarize_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
 
 
-class ConnectorOAuth(UncheckedBaseModel):
-    client_id: typing.Optional[str] = pydantic_v1.Field(default=None)
+class SummarizeResponse(UncheckedBaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The OAuth 2.0 client ID. This field is encrypted at rest.
+    Generated ID for the summary
     """
 
-    client_secret: typing.Optional[str] = pydantic_v1.Field(default=None)
+    summary: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The OAuth 2.0 client Secret. This field is encrypted at rest and never returned in a response.
+    Generated summary for the text
     """
 
-    authorize_url: str = pydantic_v1.Field()
-    """
-    The OAuth 2.0 /authorize endpoint to use when users authorize the connector.
-    """
-
-    token_url: str = pydantic_v1.Field()
-    """
-    The OAuth 2.0 /token endpoint to use when users authorize the connector.
-    """
-
-    scope: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    The OAuth scopes to request when users authorize the connector.
-    """
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/create_connector_o_auth.py` & `cohere-5.5.1/src/cohere/types/create_connector_o_auth.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class CreateConnectorOAuth(UncheckedBaseModel):
     client_id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
     The OAuth 2.0 client ID. This fields is encrypted at rest.
@@ -35,15 +35,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/create_connector_response.py` & `cohere-5.5.1/src/cohere/types/create_connector_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .connector import Connector
 
 
 class CreateConnectorResponse(UncheckedBaseModel):
     connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/create_connector_service_auth.py` & `cohere-5.5.1/src/cohere/types/create_connector_service_auth.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .auth_token_type import AuthTokenType
 
 
 class CreateConnectorServiceAuth(UncheckedBaseModel):
     type: AuthTokenType
     token: str = pydantic_v1.Field()
@@ -17,15 +17,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/create_embed_job_response.py` & `cohere-5.5.1/src/cohere/types/too_many_requests_error_body.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
 
 
-class CreateEmbedJobResponse(UncheckedBaseModel):
-    """
-    Response from creating an embed job.
-    """
-
-    job_id: str
-    meta: typing.Optional[ApiMeta] = None
+class TooManyRequestsErrorBody(UncheckedBaseModel):
+    data: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/dataset.py` & `cohere-5.5.1/src/cohere/types/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .dataset_part import DatasetPart
 from .dataset_type import DatasetType
 from .dataset_validation_status import DatasetValidationStatus
 
 
 class Dataset(UncheckedBaseModel):
@@ -57,16 +57,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/dataset_part.py` & `cohere-5.5.1/src/cohere/types/dataset_part.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class DatasetPart(UncheckedBaseModel):
     id: str = pydantic_v1.Field()
     """
     The dataset part ID
@@ -50,15 +50,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/detokenize_response.py` & `cohere-5.5.1/src/cohere/datasets/types/datasets_get_usage_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class DetokenizeResponse(UncheckedBaseModel):
-    text: str = pydantic_v1.Field()
+class DatasetsGetUsageResponse(UncheckedBaseModel):
+    organization_usage: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    A string representing the list of tokens.
+    The total number of bytes used by the organization.
     """
 
-    meta: typing.Optional[ApiMeta] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/embed_by_type_response.py` & `cohere-5.5.1/src/cohere/types/embed_by_type_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 from .embed_by_type_response_embeddings import EmbedByTypeResponseEmbeddings
 
 
 class EmbedByTypeResponse(UncheckedBaseModel):
     id: str
@@ -25,15 +25,19 @@
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/embed_by_type_response_embeddings.py` & `cohere-5.5.1/src/cohere/types/embed_by_type_response_embeddings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class EmbedByTypeResponseEmbeddings(UncheckedBaseModel):
     """
     An object with different embedding types. The length of each embedding type array will be the same as the length of the original `texts` array.
     """
@@ -39,16 +39,20 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/embed_floats_response.py` & `cohere-5.5.1/src/cohere/types/embed_floats_response.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 
 
 class EmbedFloatsResponse(UncheckedBaseModel):
     id: str
     embeddings: typing.List[typing.List[float]] = pydantic_v1.Field()
@@ -24,15 +24,19 @@
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/embed_job.py` & `cohere-5.5.1/src/cohere/types/embed_job.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 from .embed_job_status import EmbedJobStatus
 from .embed_job_truncate import EmbedJobTruncate
 
 
 class EmbedJob(UncheckedBaseModel):
@@ -55,15 +55,19 @@
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/finetune_dataset_metrics.py` & `cohere-5.5.1/src/cohere/types/finetune_dataset_metrics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class FinetuneDatasetMetrics(UncheckedBaseModel):
     trainable_token_count: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of tokens of valid examples that can be used for training.
@@ -40,15 +40,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/generate_stream_end.py` & `cohere-5.5.1/src/cohere/types/generate_stream_text.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,41 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .finish_reason import FinishReason
-from .generate_stream_end_response import GenerateStreamEndResponse
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from .generate_stream_event import GenerateStreamEvent
 
 
-class GenerateStreamEnd(GenerateStreamEvent):
+class GenerateStreamText(GenerateStreamEvent):
+    text: str = pydantic_v1.Field()
+    """
+    A segment of text of the generation.
+    """
+
+    index: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Refers to the nth generation. Only present when `num_generations` is greater than zero, and only when text responses are being streamed.
+    """
+
     is_finished: bool
-    finish_reason: typing.Optional[FinishReason] = None
-    response: GenerateStreamEndResponse
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/generate_stream_end_response.py` & `cohere-5.5.1/src/cohere/types/create_embed_job_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,36 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .single_generation_in_stream import SingleGenerationInStream
+from .api_meta import ApiMeta
 
 
-class GenerateStreamEndResponse(UncheckedBaseModel):
-    id: str
-    prompt: typing.Optional[str] = None
-    generations: typing.Optional[typing.List[SingleGenerationInStream]] = None
+class CreateEmbedJobResponse(UncheckedBaseModel):
+    """
+    Response from creating an embed job.
+    """
+
+    job_id: str
+    meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/generate_stream_error.py` & `cohere-5.5.1/src/cohere/types/list_models_response.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from .finish_reason import FinishReason
-from .generate_stream_event import GenerateStreamEvent
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ..core.unchecked_base_model import UncheckedBaseModel
+from .get_model_response import GetModelResponse
 
 
-class GenerateStreamError(GenerateStreamEvent):
-    index: typing.Optional[int] = pydantic_v1.Field(default=None)
+class ListModelsResponse(UncheckedBaseModel):
+    models: typing.List[GetModelResponse]
+    next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    Refers to the nth generation. Only present when `num_generations` is greater than zero.
-    """
-
-    is_finished: bool
-    finish_reason: FinishReason
-    err: str = pydantic_v1.Field()
-    """
-    Error message
+    A token to retrieve the next page of results. Provide in the page_token parameter of the next request.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
-        allow_population_by_field_name = True
-        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/generate_stream_event.py` & `cohere-5.5.1/src/cohere/types/tool_result.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .tool_call import ToolCall
 
 
-class GenerateStreamEvent(UncheckedBaseModel):
+class ToolResult(UncheckedBaseModel):
+    call: ToolCall
+    outputs: typing.List[typing.Dict[str, typing.Any]]
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/generate_stream_text.py` & `cohere-5.5.1/src/cohere/types/generate_stream_error.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .finish_reason import FinishReason
 from .generate_stream_event import GenerateStreamEvent
 
 
-class GenerateStreamText(GenerateStreamEvent):
-    text: str = pydantic_v1.Field()
-    """
-    A segment of text of the generation.
-    """
-
+class GenerateStreamError(GenerateStreamEvent):
     index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    Refers to the nth generation. Only present when `num_generations` is greater than zero, and only when text responses are being streamed.
+    Refers to the nth generation. Only present when `num_generations` is greater than zero.
     """
 
     is_finished: bool
+    finish_reason: FinishReason
+    err: str = pydantic_v1.Field()
+    """
+    Error message
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         allow_population_by_field_name = True
         populate_by_name = True
         extra = pydantic_v1.Extra.allow
```

### Comparing `cohere-5.5.0/src/cohere/types/generation.py` & `cohere-5.5.1/src/cohere/types/tool_call.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
-from .single_generation import SingleGeneration
 
 
-class Generation(UncheckedBaseModel):
-    id: str
-    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ToolCall(UncheckedBaseModel):
     """
-    Prompt used for generations.
+    Contains the tool calls generated by the model. Use it to invoke your tools.
     """
 
-    generations: typing.List[SingleGeneration] = pydantic_v1.Field()
+    name: str = pydantic_v1.Field()
     """
-    List of generated results
+    Name of the tool to call.
     """
 
-    meta: typing.Optional[ApiMeta] = None
+    parameters: typing.Dict[str, typing.Any] = pydantic_v1.Field()
+    """
+    The name and value of the parameters to use when invoking a tool.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/get_connector_response.py` & `cohere-5.5.1/src/cohere/types/metrics_embed_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,34 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .connector import Connector
+from .metrics_embed_data_fields_item import MetricsEmbedDataFieldsItem
 
 
-class GetConnectorResponse(UncheckedBaseModel):
-    connector: Connector
+class MetricsEmbedData(UncheckedBaseModel):
+    fields: typing.Optional[typing.List[MetricsEmbedDataFieldsItem]] = pydantic_v1.Field(default=None)
+    """
+    the fields in the dataset
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/get_model_response.py` & `cohere-5.5.1/src/cohere/types/get_model_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .compatible_endpoint import CompatibleEndpoint
 
 
 class GetModelResponse(UncheckedBaseModel):
     """
     Contains information about the model and which API endpoints it can be used with.
@@ -45,15 +45,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/label_metric.py` & `cohere-5.5.1/src/cohere/types/label_metric.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class LabelMetric(UncheckedBaseModel):
     total_examples: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     Total number of examples for this label
@@ -25,15 +25,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/list_connectors_response.py` & `cohere-5.5.1/src/cohere/types/api_meta_api_version.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .connector import Connector
 
 
-class ListConnectorsResponse(UncheckedBaseModel):
-    connectors: typing.List[Connector]
-    total_count: typing.Optional[float] = pydantic_v1.Field(default=None)
-    """
-    Total number of connectors.
-    """
+class ApiMetaApiVersion(UncheckedBaseModel):
+    version: str
+    is_deprecated: typing.Optional[bool] = None
+    is_experimental: typing.Optional[bool] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/list_embed_job_response.py` & `cohere-5.5.1/src/cohere/types/metrics.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,27 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .embed_job import EmbedJob
+from .finetune_dataset_metrics import FinetuneDatasetMetrics
+from .metrics_embed_data import MetricsEmbedData
 
 
-class ListEmbedJobResponse(UncheckedBaseModel):
-    embed_jobs: typing.Optional[typing.List[EmbedJob]] = None
+class Metrics(UncheckedBaseModel):
+    finetune_dataset_metrics: typing.Optional[FinetuneDatasetMetrics] = None
+    embed_data: typing.Optional[MetricsEmbedData] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/list_models_response.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/list_training_step_metrics_response.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,44 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
-from .get_model_response import GetModelResponse
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .training_step_metrics import TrainingStepMetrics
 
 
-class ListModelsResponse(UncheckedBaseModel):
-    models: typing.List[GetModelResponse]
+class ListTrainingStepMetricsResponse(UncheckedBaseModel):
+    """
+    Response to a request to list training-step metrics of a fine-tuned model.
+    """
+
+    step_metrics: typing.Optional[typing.List[TrainingStepMetrics]] = pydantic_v1.Field(default=None)
+    """
+    The metrics for each step the evaluation was run on.
+    """
+
     next_page_token: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    A token to retrieve the next page of results. Provide in the page_token parameter of the next request.
+    Pagination token to retrieve the next page of results. If the value is "",
+    it means no further results for the request.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/metrics.py` & `cohere-5.5.1/src/cohere/types/generate_stream_event.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .finetune_dataset_metrics import FinetuneDatasetMetrics
-from .metrics_embed_data import MetricsEmbedData
 
 
-class Metrics(UncheckedBaseModel):
-    finetune_dataset_metrics: typing.Optional[FinetuneDatasetMetrics] = None
-    embed_data: typing.Optional[MetricsEmbedData] = None
-
+class GenerateStreamEvent(UncheckedBaseModel):
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/metrics_embed_data.py` & `cohere-5.5.1/src/cohere/types/rerank_response_results_item_document.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,30 +1,37 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .metrics_embed_data_fields_item import MetricsEmbedDataFieldsItem
 
 
-class MetricsEmbedData(UncheckedBaseModel):
-    fields: typing.Optional[typing.List[MetricsEmbedDataFieldsItem]] = pydantic_v1.Field(default=None)
+class RerankResponseResultsItemDocument(UncheckedBaseModel):
     """
-    the fields in the dataset
+    If `return_documents` is set as `false` this will return none, if `true` it will return the documents passed in
+    """
+
+    text: str = pydantic_v1.Field()
+    """
+    The text of the document to rerank
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/metrics_embed_data_fields_item.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/training_step_metrics.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,47 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
 
 
-class MetricsEmbedDataFieldsItem(UncheckedBaseModel):
-    name: typing.Optional[str] = pydantic_v1.Field(default=None)
+class TrainingStepMetrics(UncheckedBaseModel):
     """
-    the name of the field
+    The evaluation metrics at a given step of the training of a fine-tuned model.
     """
 
-    count: typing.Optional[float] = pydantic_v1.Field(default=None)
+    created_at: typing.Optional[dt.datetime] = pydantic_v1.Field(default=None)
     """
-    the number of times the field appears in the dataset
+    Creation timestamp.
+    """
+
+    step_number: typing.Optional[int] = pydantic_v1.Field(default=None)
+    """
+    Step number.
+    """
+
+    metrics: typing.Optional[typing.Dict[str, float]] = pydantic_v1.Field(default=None)
+    """
+    Map of names and values for each evaluation metrics.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/non_streamed_chat_response.py` & `cohere-5.5.1/src/cohere/types/non_streamed_chat_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .api_meta import ApiMeta
 from .chat_citation import ChatCitation
 from .chat_document import ChatDocument
 from .chat_search_query import ChatSearchQuery
 from .chat_search_result import ChatSearchResult
 from .finish_reason import FinishReason
@@ -67,15 +67,19 @@
     meta: typing.Optional[ApiMeta] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/o_auth_authorize_response.py` & `cohere-5.5.1/src/cohere/types/metrics_embed_data_fields_item.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class OAuthAuthorizeResponse(UncheckedBaseModel):
-    redirect_url: typing.Optional[str] = pydantic_v1.Field(default=None)
+class MetricsEmbedDataFieldsItem(UncheckedBaseModel):
+    name: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The OAuth 2.0 redirect url. Redirect the user to this url to authorize the connector.
+    the name of the field
+    """
+
+    count: typing.Optional[float] = pydantic_v1.Field(default=None)
+    """
+    the number of times the field appears in the dataset
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/parse_info.py` & `cohere-5.5.1/src/cohere/types/get_connector_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,27 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .connector import Connector
 
 
-class ParseInfo(UncheckedBaseModel):
-    separator: typing.Optional[str] = None
-    delimiter: typing.Optional[str] = None
+class GetConnectorResponse(UncheckedBaseModel):
+    connector: Connector
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/rerank_request_documents_item_text.py` & `cohere-5.5.1/src/cohere/types/generation.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
+from .api_meta import ApiMeta
+from .single_generation import SingleGeneration
 
 
-class RerankRequestDocumentsItemText(UncheckedBaseModel):
-    text: str = pydantic_v1.Field()
+class Generation(UncheckedBaseModel):
+    id: str
+    prompt: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    The text of the document to rerank.
+    Prompt used for generations.
     """
 
+    generations: typing.List[SingleGeneration] = pydantic_v1.Field()
+    """
+    List of generated results
+    """
+
+    meta: typing.Optional[ApiMeta] = None
+
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/rerank_response.py` & `cohere-5.5.1/src/cohere/types/classify_data_metrics.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
-from .rerank_response_results_item import RerankResponseResultsItem
+from .label_metric import LabelMetric
 
 
-class RerankResponse(UncheckedBaseModel):
-    id: typing.Optional[str] = None
-    results: typing.List[RerankResponseResultsItem] = pydantic_v1.Field()
-    """
-    An ordered list of ranked documents
-    """
-
-    meta: typing.Optional[ApiMeta] = None
+class ClassifyDataMetrics(UncheckedBaseModel):
+    label_metrics: typing.Optional[typing.List[LabelMetric]] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/rerank_response_results_item.py` & `cohere-5.5.1/src/cohere/types/single_generation_in_stream.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .rerank_response_results_item_document import RerankResponseResultsItemDocument
+from .finish_reason import FinishReason
 
 
-class RerankResponseResultsItem(UncheckedBaseModel):
-    document: typing.Optional[RerankResponseResultsItemDocument] = pydantic_v1.Field(default=None)
+class SingleGenerationInStream(UncheckedBaseModel):
+    id: str
+    text: str = pydantic_v1.Field()
     """
-    If `return_documents` is set as `false` this will return none, if `true` it will return the documents passed in
+    Full text of the generation.
     """
 
-    index: int = pydantic_v1.Field()
+    index: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
-    Corresponds to the index in the original list of documents to which the ranked document belongs. (i.e. if the first value in the `results` object has an `index` value of 3, it means in the list of documents passed in, the document at `index=3` had the highest relevance)
+    Refers to the nth generation. Only present when `num_generations` is greater than zero.
     """
 
-    relevance_score: float = pydantic_v1.Field()
-    """
-    Relevance scores are normalized to be in the range `[0, 1]`. Scores close to `1` indicate a high relevance to the query, and scores closer to `0` indicate low relevance. It is not accurate to assume a score of 0.9 means the document is 2x more relevant than a document with a score of 0.45
-    """
+    finish_reason: FinishReason
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/rerank_response_results_item_document.py` & `cohere-5.5.1/src/cohere/types/single_generation_token_likelihoods_item.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class RerankResponseResultsItemDocument(UncheckedBaseModel):
-    """
-    If `return_documents` is set as `false` this will return none, if `true` it will return the documents passed in
-    """
-
-    text: str = pydantic_v1.Field()
-    """
-    The text of the document to rerank
-    """
+class SingleGenerationTokenLikelihoodsItem(UncheckedBaseModel):
+    token: str
+    likelihood: float
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/reranker_data_metrics.py` & `cohere-5.5.1/src/cohere/types/reranker_data_metrics.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
 class RerankerDataMetrics(UncheckedBaseModel):
     num_train_queries: typing.Optional[int] = pydantic_v1.Field(default=None)
     """
     The number of training queries.
@@ -40,15 +40,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/single_generation.py` & `cohere-5.5.1/src/cohere/types/single_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .single_generation_token_likelihoods_item import SingleGenerationTokenLikelihoodsItem
 
 
 class SingleGeneration(UncheckedBaseModel):
     id: str
     text: str
@@ -26,15 +26,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/summarize_response.py` & `cohere-5.5.1/src/cohere/types/list_connectors_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
+from .connector import Connector
 
 
-class SummarizeResponse(UncheckedBaseModel):
-    id: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ListConnectorsResponse(UncheckedBaseModel):
+    connectors: typing.List[Connector]
+    total_count: typing.Optional[float] = pydantic_v1.Field(default=None)
     """
-    Generated ID for the summary
+    Total number of connectors.
     """
 
-    summary: typing.Optional[str] = pydantic_v1.Field(default=None)
-    """
-    Generated summary for the text
-    """
-
-    meta: typing.Optional[ApiMeta] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/tokenize_response.py` & `cohere-5.5.1/src/cohere/datasets/types/datasets_create_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
-from .api_meta import ApiMeta
+from ...core.datetime_utils import serialize_datetime
+from ...core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ...core.unchecked_base_model import UncheckedBaseModel
 
 
-class TokenizeResponse(UncheckedBaseModel):
-    tokens: typing.List[int] = pydantic_v1.Field()
+class DatasetsCreateResponse(UncheckedBaseModel):
+    id: typing.Optional[str] = pydantic_v1.Field(default=None)
     """
-    An array of tokens, where each token is an integer.
+    The dataset ID
     """
 
-    token_strings: typing.List[str]
-    meta: typing.Optional[ApiMeta] = None
-
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/too_many_requests_error_body.py` & `cohere-5.5.1/src/cohere/types/tool_parameter_definitions_value.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,43 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class TooManyRequestsErrorBody(UncheckedBaseModel):
-    data: typing.Optional[str] = None
+class ToolParameterDefinitionsValue(UncheckedBaseModel):
+    description: typing.Optional[str] = pydantic_v1.Field(default=None)
+    """
+    The description of the parameter.
+    """
+
+    type: str = pydantic_v1.Field()
+    """
+    The type of the parameter. Must be a valid Python type.
+    """
+
+    required: typing.Optional[bool] = pydantic_v1.Field(default=None)
+    """
+    Denotes whether the parameter is always present (required) or not. Defaults to not required.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/tool.py` & `cohere-5.5.1/src/cohere/types/tool.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 from .tool_parameter_definitions_value import ToolParameterDefinitionsValue
 
 
 class Tool(UncheckedBaseModel):
     name: str = pydantic_v1.Field()
     """
@@ -38,15 +38,19 @@
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/tool_call.py` & `cohere-5.5.1/src/cohere/types/parse_info.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,31 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
 from ..core.unchecked_base_model import UncheckedBaseModel
 
 
-class ToolCall(UncheckedBaseModel):
-    """
-    Contains the tool calls generated by the model. Use it to invoke your tools.
-    """
-
-    name: str = pydantic_v1.Field()
-    """
-    Name of the tool to call.
-    """
-
-    parameters: typing.Dict[str, typing.Any] = pydantic_v1.Field()
-    """
-    The name and value of the parameters to use when invoking a tool.
-    """
+class ParseInfo(UncheckedBaseModel):
+    separator: typing.Optional[str] = None
+    delimiter: typing.Optional[str] = None
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/tool_parameter_definitions_value.py` & `cohere-5.5.1/src/cohere/types/chat_search_results_event.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,39 +1,42 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
 from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
+from ..core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from .chat_document import ChatDocument
+from .chat_search_result import ChatSearchResult
+from .chat_stream_event import ChatStreamEvent
 
 
-class ToolParameterDefinitionsValue(UncheckedBaseModel):
-    description: typing.Optional[str] = pydantic_v1.Field(default=None)
+class ChatSearchResultsEvent(ChatStreamEvent):
+    search_results: typing.Optional[typing.List[ChatSearchResult]] = pydantic_v1.Field(default=None)
     """
-    The description of the parameter.
+    Conducted searches and the ids of documents retrieved from each of them.
     """
 
-    type: str = pydantic_v1.Field()
+    documents: typing.Optional[typing.List[ChatDocument]] = pydantic_v1.Field(default=None)
     """
-    The type of the parameter. Must be a valid Python type.
-    """
-
-    required: typing.Optional[bool] = pydantic_v1.Field(default=None)
-    """
-    Denotes whether the parameter is always present (required) or not. Defaults to not required.
+    Documents fetched from searches or provided by the user.
     """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
+        allow_population_by_field_name = True
+        populate_by_name = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/types/tool_result.py` & `cohere-5.5.1/src/cohere/finetuning/finetuning/types/create_finetuned_model_response.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,38 @@
 # This file was auto-generated by Fern from our API Definition.
 
 import datetime as dt
 import typing
 
-from ..core.datetime_utils import serialize_datetime
-from ..core.pydantic_utilities import pydantic_v1
-from ..core.unchecked_base_model import UncheckedBaseModel
-from .tool_call import ToolCall
+from ....core.datetime_utils import serialize_datetime
+from ....core.pydantic_utilities import deep_union_pydantic_dicts, pydantic_v1
+from ....core.unchecked_base_model import UncheckedBaseModel
+from .finetuned_model import FinetunedModel
 
 
-class ToolResult(UncheckedBaseModel):
-    call: ToolCall
-    outputs: typing.List[typing.Dict[str, typing.Any]]
+class CreateFinetunedModelResponse(UncheckedBaseModel):
+    """
+    Response to request to create a fine-tuned model.
+    """
+
+    finetuned_model: typing.Optional[FinetunedModel] = pydantic_v1.Field(default=None)
+    """
+    Information about the fine-tuned model.
+    """
 
     def json(self, **kwargs: typing.Any) -> str:
         kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
         return super().json(**kwargs_with_defaults)
 
     def dict(self, **kwargs: typing.Any) -> typing.Dict[str, typing.Any]:
-        kwargs_with_defaults: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
-        return super().dict(**kwargs_with_defaults)
+        kwargs_with_defaults_exclude_unset: typing.Any = {"by_alias": True, "exclude_unset": True, **kwargs}
+        kwargs_with_defaults_exclude_none: typing.Any = {"by_alias": True, "exclude_none": True, **kwargs}
+
+        return deep_union_pydantic_dicts(
+            super().dict(**kwargs_with_defaults_exclude_unset), super().dict(**kwargs_with_defaults_exclude_none)
+        )
 
     class Config:
         frozen = True
         smart_union = True
         extra = pydantic_v1.Extra.allow
         json_encoders = {dt.datetime: serialize_datetime}
```

### Comparing `cohere-5.5.0/src/cohere/utils.py` & `cohere-5.5.1/src/cohere/utils.py`

 * *Files identical despite different names*

### Comparing `cohere-5.5.0/PKG-INFO` & `cohere-5.5.1/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 Metadata-Version: 2.1
 Name: cohere
-Version: 5.5.0
+Version: 5.5.1
 Summary: 
 Requires-Python: >=3.8,<4.0
+Classifier: Intended Audience :: Developers
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: OS Independent
+Classifier: Operating System :: POSIX
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Classifier: Typing :: Typed
 Requires-Dist: boto3 (>=1.34.0,<2.0.0)
 Requires-Dist: fastavro (>=1.9.4,<2.0.0)
 Requires-Dist: httpx (>=0.21.2)
 Requires-Dist: httpx-sse (>=0.4.0,<0.5.0)
 Requires-Dist: pydantic (>=1.9.2)
 Requires-Dist: requests (>=2.0.0,<3.0.0)
 Requires-Dist: tokenizers (>=0.19,<0.20)
```

