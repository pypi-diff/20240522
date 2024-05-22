# Comparing `tmp/semantic_kernel-1.0.0rc1.tar.gz` & `tmp/semantic_kernel-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-1.0.0rc1.tar", max compression
+gzip compressed data, was "semantic_kernel-1.0.1.tar", max compression
```

## Comparing `semantic_kernel-1.0.0rc1.tar` & `semantic_kernel-1.0.1.tar`

### file list

```diff
@@ -1,233 +1,239 @@
--rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/pip/README.md
--rw-r--r--   0        0        0     5411 2024-05-17 22:45:44.178248 semantic_kernel-1.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/__init__.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/__init__.py
--rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     3250 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0      437 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0     7538 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py
--rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py
--rw-r--r--   0        0        0     1795 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
--rw-r--r--   0        0        0    10535 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
--rw-r--r--   0        0        0     4676 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
--rw-r--r--   0        0        0     3118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
--rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
--rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     1169 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
--rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
--rw-r--r--   0        0        0     6683 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2119 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py
--rw-r--r--   0        0        0      822 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
--rw-r--r--   0        0        0     8451 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
--rw-r--r--   0        0        0     3983 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
--rw-r--r--   0        0        0     1805 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
--rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/utils.py
--rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/const.py
--rw-r--r--   0        0        0     2636 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
--rw-r--r--   0        0        0     3817 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
--rw-r--r--   0        0        0     4147 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
--rw-r--r--   0        0        0    11081 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     5356 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
--rw-r--r--   0        0        0     6087 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     6075 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     3614 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0    23919 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
--rw-r--r--   0        0        0     3737 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
--rw-r--r--   0        0        0     4046 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
--rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
--rw-r--r--   0        0        0     3823 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     6363 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
--rw-r--r--   0        0        0     3663 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1907 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
--rw-r--r--   0        0        0     2908 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py
--rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
--rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
--rw-r--r--   0        0        0     3908 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py
--rw-r--r--   0        0        0     1741 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/__init__.py
--rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/__init__.py
--rw-r--r--   0        0        0     6718 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py
--rw-r--r--   0        0        0    13347 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
--rw-r--r--   0        0        0      735 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
--rw-r--r--   0        0        0     1607 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py
--rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0     1160 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
--rw-r--r--   0        0        0    16963 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     7882 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
--rw-r--r--   0        0        0    11118 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
--rw-r--r--   0        0        0     2230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
--rw-r--r--   0        0        0      538 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
--rw-r--r--   0        0        0     1592 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
--rw-r--r--   0        0        0    13020 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    14277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4603 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      560 2024-05-16 18:28:06.371055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/memory_settings_base.py
--rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16598 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
--rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
--rw-r--r--   0        0        0    13131 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
--rw-r--r--   0        0        0      518 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
--rw-r--r--   0        0        0     2302 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
--rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    15618 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0      460 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
--rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    21145 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0      494 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
--rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/__init__.py
--rw-r--r--   0        0        0    11703 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
--rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md
--rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/__init__.py
--rw-r--r--   0        0        0    15880 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
--rw-r--r--   0        0        0      486 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_settings.py
--rw-r--r--   0        0        0     3677 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py
--rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/__init__.py
--rw-r--r--   0        0        0    23257 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
--rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/__init__.py
--rw-r--r--   0        0        0    12496 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      908 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
--rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py
--rw-r--r--   0        0        0      799 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
--rw-r--r--   0        0        0      506 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
--rw-r--r--   0        0        0     1011 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py
--rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/__init__.py
--rw-r--r--   0        0        0     1268 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
--rw-r--r--   0        0        0    28989 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
--rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     3425 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
--rw-r--r--   0        0        0      323 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0     2978 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py
--rw-r--r--   0        0        0     1111 2024-03-20 18:24:28.763758 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py
--rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/__init__.py
--rw-r--r--   0        0        0      895 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py
--rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/const.py
--rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py
--rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/author_role.py
--rw-r--r--   0        0        0    14167 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py
--rw-r--r--   0        0        0    12590 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py
--rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/const.py
--rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/contents/finish_reason.py
--rw-r--r--   0        0        0     4032 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py
--rw-r--r--   0        0        0     4556 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py
--rw-r--r--   0        0        0      772 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py
--rw-r--r--   0        0        0    10964 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py
--rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py
--rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py
--rw-r--r--   0        0        0     2011 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py
--rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py
--rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py
--rw-r--r--   0        0        0     3452 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py
--rw-r--r--   0        0        0     4069 2024-05-06 13:16:31.755032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py
--rw-r--r--   0        0        0     2474 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py
--rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md
--rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
--rw-r--r--   0        0        0     9954 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
--rw-r--r--   0        0        0     1919 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
--rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
--rw-r--r--   0        0        0     3783 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py
--rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py
--rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py
--rw-r--r--   0        0        0     1163 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/wait_plugin.py
--rw-r--r--   0        0        0     1789 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py
--rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py
--rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py
--rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py
--rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py
--rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/memory_connector_exceptions.py
--rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py
--rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py
--rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py
--rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
--rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_context_base.py
--rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_types.py
--rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/functions/function_invocation_context.py
--rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/filters/prompts/prompt_render_context.py
--rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py
--rw-r--r--   0        0        0     2455 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py
--rw-r--r--   0        0        0     1750 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py
--rw-r--r--   0        0        0    10657 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py
--rw-r--r--   0        0        0     6170 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py
--rw-r--r--   0        0        0     7843 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py
--rw-r--r--   0        0        0    16893 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py
--rw-r--r--   0        0        0     1991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py
--rw-r--r--   0        0        0      559 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_parameter_metadata.py
--rw-r--r--   0        0        0    24196 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py
--rw-r--r--   0        0        0      974 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/functions/prompt_rendering_result.py
--rw-r--r--   0        0        0      260 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/functions/types.py
--rw-r--r--   0        0        0    37221 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     6346 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_extensions/kernel_filters_extension.py
--rw-r--r--   0        0        0      618 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/kernel_pydantic.py
--rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     4267 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     7146 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1592 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6521 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     3619 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12065 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py
--rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
--rw-r--r--   0        0        0    12815 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
--rw-r--r--   0        0        0     1675 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
--rw-r--r--   0        0        0      928 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
--rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
--rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
--rw-r--r--   0        0        0    14404 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py
--rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py
--rw-r--r--   0        0        0      592 2024-05-09 23:07:37.265180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py
--rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
--rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
--rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/__init__.py
--rw-r--r--   0        0        0     5978 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py
--rw-r--r--   0        0        0     1135 2024-03-13 15:37:17.055380 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
--rw-r--r--   0        0        0     4720 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
--rw-r--r--   0        0        0     4987 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
--rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py
--rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py
--rw-r--r--   0        0        0     4760 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py
--rw-r--r--   0        0        0      893 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py
--rw-r--r--   0        0        0     4945 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py
--rw-r--r--   0        0        0     6744 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py
--rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py
--rw-r--r--   0        0        0     5586 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py
--rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/__init__.py
--rw-r--r--   0        0        0     4592 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
--rw-r--r--   0        0        0     2483 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
--rw-r--r--   0        0        0     2069 2024-05-17 22:45:44.198248 semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py
--rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.0rc1/semantic_kernel/py.typed
--rw-r--r--   0        0        0      972 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      652 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.0rc1/semantic_kernel/services/__init__.py
--rw-r--r--   0        0        0     1979 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py
--rw-r--r--   0        0        0     2648 2024-05-09 23:07:37.275180 semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py
--rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     7474 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2432 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0     3917 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py
--rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1688 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2389 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2927 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6593 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     6295 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      678 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8475 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      504 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/chat.py
--rw-r--r--   0        0        0      838 2024-05-16 18:28:06.381055 semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py
--rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/logging.py
--rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py
--rw-r--r--   0        0        0     1177 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2583 2024-03-13 15:37:17.065380 semantic_kernel-1.0.0rc1/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     5105 1970-01-01 00:00:00.000000 semantic_kernel-1.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1186 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/pip/README.md
+-rw-r--r--   0        0        0     4591 2024-05-22 16:18:31.525428 semantic_kernel-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      113 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/semantic_kernel/connectors/__init__.py
+-rw-r--r--   0        0        0      180 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     3242 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0      527 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0     7530 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/function_call_behavior.py
+-rw-r--r--   0        0        0      768 2024-03-13 15:37:17.045380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py
+-rw-r--r--   0        0        0    10522 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py
+-rw-r--r--   0        0        0     4670 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py
+-rw-r--r--   0        0        0     3208 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py
+-rw-r--r--   0        0        0     1866 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py
+-rw-r--r--   0        0        0      533 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     1163 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py
+-rw-r--r--   0        0        0        0 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/__init__.py
+-rw-r--r--   0        0        0     6673 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2193 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      600 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/__init__.py
+-rw-r--r--   0        0        0      779 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/ollama_prompt_execution_settings.py
+-rw-r--r--   0        0        0     8459 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py
+-rw-r--r--   0        0        0     3991 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py
+-rw-r--r--   0        0        0     1882 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py
+-rw-r--r--   0        0        0      387 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/utils.py
+-rw-r--r--   0        0        0     2036 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0      246 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/const.py
+-rw-r--r--   0        0        0     2630 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py
+-rw-r--r--   0        0        0     3676 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py
+-rw-r--r--   0        0        0     3766 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/open_ai_prompt_execution_settings.py
+-rw-r--r--   0        0        0    11076 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     5309 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py
+-rw-r--r--   0        0        0     6096 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     6180 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     3604 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0    24070 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py
+-rw-r--r--   0        0        0     3712 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py
+-rw-r--r--   0        0        0     4011 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py
+-rw-r--r--   0        0        0      230 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_model_types.py
+-rw-r--r--   0        0        0     3807 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     6359 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py
+-rw-r--r--   0        0        0     3743 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1984 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py
+-rw-r--r--   0        0        0     2871 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/utils.py
+-rw-r--r--   0        0        0     4169 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py
+-rw-r--r--   0        0        0     2060 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py
+-rw-r--r--   0        0        0     3879 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/prompt_execution_settings.py
+-rw-r--r--   0        0        0     1733 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0       48 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/__init__.py
+-rw-r--r--   0        0        0      292 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/__init__.py
+-rw-r--r--   0        0        0     6750 2024-05-22 16:18:31.535428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astra_client.py
+-rw-r--r--   0        0        0    13396 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py
+-rw-r--r--   0        0        0      831 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_settings.py
+-rw-r--r--   0        0        0     1601 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/utils.py
+-rw-r--r--   0        0        0      383 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0     1256 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py
+-rw-r--r--   0        0        0    17012 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     7836 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      345 2024-05-16 18:28:06.371055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/__init__.py
+-rw-r--r--   0        0        0    11153 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py
+-rw-r--r--   0        0        0     2295 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py
+-rw-r--r--   0        0        0      634 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py
+-rw-r--r--   0        0        0     1740 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py
+-rw-r--r--   0        0        0    13097 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py
+-rw-r--r--   0        0        0      236 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/__init__.py
+-rw-r--r--   0        0        0     7720 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb_no_sql/azure_cosmosdb_no_sql_memory_store.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    14357 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4597 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      657 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/memory_settings_base.py
+-rw-r--r--   0        0        0      133 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16748 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0     1422 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/README.md
+-rw-r--r--   0        0        0      336 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/__init__.py
+-rw-r--r--   0        0        0    13206 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py
+-rw-r--r--   0        0        0      614 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py
+-rw-r--r--   0        0        0     2267 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py
+-rw-r--r--   0        0        0      309 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    15682 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0      556 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_settings.py
+-rw-r--r--   0        0        0     1154 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      300 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    21197 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      590 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_settings.py
+-rw-r--r--   0        0        0      182 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11743 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0     1362 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/README.md
+-rw-r--r--   0        0        0      276 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/__init__.py
+-rw-r--r--   0        0        0    15945 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_memory_store.py
+-rw-r--r--   0        0        0      582 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_settings.py
+-rw-r--r--   0        0        0     3664 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/utils.py
+-rw-r--r--   0        0        0      186 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/__init__.py
+-rw-r--r--   0        0        0    23249 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py
+-rw-r--r--   0        0        0      298 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/__init__.py
+-rw-r--r--   0        0        0    12561 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0     1004 2024-05-21 00:02:54.747516 semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py
+-rw-r--r--   0        0        0      549 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/__init__.py
+-rw-r--r--   0        0        0      764 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_function_execution_parameters.py
+-rw-r--r--   0        0        0      976 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_utils.py
+-rw-r--r--   0        0        0      235 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/__init__.py
+-rw-r--r--   0        0        0     1350 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py
+-rw-r--r--   0        0        0    29335 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py
+-rw-r--r--   0        0        0      265 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     3401 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0     1165 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector_settings.py
+-rw-r--r--   0        0        0      299 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     2954 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0     1105 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/telemetry.py
+-rw-r--r--   0        0        0      155 2024-04-01 16:45:47.997053 semantic_kernel-1.0.1/semantic_kernel/connectors/utils/__init__.py
+-rw-r--r--   0        0        0      906 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/connectors/utils/document_loader.py
+-rw-r--r--   0        0        0      123 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/const.py
+-rw-r--r--   0        0        0      865 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/__init__.py
+-rw-r--r--   0        0        0      215 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/author_role.py
+-rw-r--r--   0        0        0    14163 2024-05-22 16:18:31.545428 semantic_kernel-1.0.1/semantic_kernel/contents/chat_history.py
+-rw-r--r--   0        0        0    12555 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/chat_message_content.py
+-rw-r--r--   0        0        0      364 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/const.py
+-rw-r--r--   0        0        0      277 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/contents/finish_reason.py
+-rw-r--r--   0        0        0     3997 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/function_call_content.py
+-rw-r--r--   0        0        0     4521 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/function_result_content.py
+-rw-r--r--   0        0        0      737 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/kernel_content.py
+-rw-r--r--   0        0        0    10933 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_chat_message_content.py
+-rw-r--r--   0        0        0      565 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_content_mixin.py
+-rw-r--r--   0        0        0     2637 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/streaming_text_content.py
+-rw-r--r--   0        0        0     1976 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/contents/text_content.py
+-rw-r--r--   0        0        0      740 2024-05-06 13:16:31.755032 semantic_kernel-1.0.1/semantic_kernel/contents/types.py
+-rw-r--r--   0        0        0      886 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/__init__.py
+-rw-r--r--   0        0        0     3336 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/conversation_summary_plugin.py
+-rw-r--r--   0        0        0     3932 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/http_plugin.py
+-rw-r--r--   0        0        0     2378 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/math_plugin.py
+-rw-r--r--   0        0        0     5812 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/README.md
+-rw-r--r--   0        0        0      341 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/__init__.py
+-rw-r--r--   0        0        0     9946 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py
+-rw-r--r--   0        0        0     1884 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py
+-rw-r--r--   0        0        0      724 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py
+-rw-r--r--   0        0        0     3662 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_memory_plugin.py
+-rw-r--r--   0        0        0     2658 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_plugin.py
+-rw-r--r--   0        0        0     8030 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/core_plugins/time_plugin.py
+-rw-r--r--   0        0        0     1020 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/wait_plugin.py
+-rw-r--r--   0        0        0     1652 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/core_plugins/web_search_engine_plugin.py
+-rw-r--r--   0        0        0      626 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/exceptions/__init__.py
+-rw-r--r--   0        0        0      727 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/exceptions/content_exceptions.py
+-rw-r--r--   0        0        0     1270 2024-05-17 22:45:44.188248 semantic_kernel-1.0.1/semantic_kernel/exceptions/function_exceptions.py
+-rw-r--r--   0        0        0     1417 2024-05-17 22:45:44.188248 semantic_kernel-1.0.1/semantic_kernel/exceptions/kernel_exceptions.py
+-rw-r--r--   0        0        0      467 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/exceptions/memory_connector_exceptions.py
+-rw-r--r--   0        0        0      690 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/exceptions/planner_exceptions.py
+-rw-r--r--   0        0        0     1144 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/exceptions/service_exceptions.py
+-rw-r--r--   0        0        0     2875 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/exceptions/template_engine_exceptions.py
+-rw-r--r--   0        0        0      655 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py
+-rw-r--r--   0        0        0      631 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/filter_context_base.py
+-rw-r--r--   0        0        0      386 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/filter_types.py
+-rw-r--r--   0        0        0      396 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/functions/function_invocation_context.py
+-rw-r--r--   0        0        0     6398 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/filters/kernel_filters_extension.py
+-rw-r--r--   0        0        0      437 2024-05-17 22:45:44.198248 semantic_kernel-1.0.1/semantic_kernel/filters/prompts/prompt_render_context.py
+-rw-r--r--   0        0        0     1009 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/functions/__init__.py
+-rw-r--r--   0        0        0     2420 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/function_result.py
+-rw-r--r--   0        0        0     1711 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_arguments.py
+-rw-r--r--   0        0        0    10643 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function.py
+-rw-r--r--   0        0        0     5499 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_decorator.py
+-rw-r--r--   0        0        0    18367 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_extension.py
+-rw-r--r--   0        0        0     8163 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_method.py
+-rw-r--r--   0        0        0    16879 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_prompt.py
+-rw-r--r--   0        0        0     1925 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_metadata.py
+-rw-r--r--   0        0        0     2157 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_parameter_metadata.py
+-rw-r--r--   0        0        0    24109 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/kernel_plugin.py
+-rw-r--r--   0        0        0      939 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/prompt_rendering_result.py
+-rw-r--r--   0        0        0      252 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/functions/types.py
+-rw-r--r--   0        0        0    13830 2024-05-22 16:18:31.555428 semantic_kernel-1.0.1/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0      462 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/kernel_pydantic.py
+-rw-r--r--   0        0        0      257 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2582 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     4285 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7211 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1639 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6571 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3675 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12124 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0      903 2024-05-09 23:07:37.265180 semantic_kernel-1.0.1/semantic_kernel/planners/__init__.py
+-rw-r--r--   0        0        0      605 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py
+-rw-r--r--   0        0        0    12968 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py
+-rw-r--r--   0        0        0     1667 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py
+-rw-r--r--   0        0        0      797 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_result.py
+-rw-r--r--   0        0        0     1377 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml
+-rw-r--r--   0        0        0      184 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/step_prompt.txt
+-rw-r--r--   0        0        0    14329 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/plan.py
+-rw-r--r--   0        0        0     2770 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/planners/planner_extensions.py
+-rw-r--r--   0        0        0      568 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/planner_options.py
+-rw-r--r--   0        0        0      718 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3179 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2024-03-13 15:37:17.055380 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1125 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     4678 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     4973 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      634 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/prompt_template/__init__.py
+-rw-r--r--   0        0        0      756 2024-05-06 13:16:31.765032 semantic_kernel-1.0.1/semantic_kernel/prompt_template/const.py
+-rw-r--r--   0        0        0     4787 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/handlebars_prompt_template.py
+-rw-r--r--   0        0        0      871 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/input_variable.py
+-rw-r--r--   0        0        0     4972 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/jinja2_prompt_template.py
+-rw-r--r--   0        0        0     6735 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/kernel_prompt_template.py
+-rw-r--r--   0        0        0     2991 2024-05-16 18:28:06.381055 semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_base.py
+-rw-r--r--   0        0        0     5535 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_config.py
+-rw-r--r--   0        0        0      477 2024-03-15 14:30:59.091994 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/__init__.py
+-rw-r--r--   0        0        0     4615 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py
+-rw-r--r--   0        0        0     2450 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py
+-rw-r--r--   0        0        0     2116 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/template_function_helpers.py
+-rw-r--r--   0        0        0        0 2024-04-01 16:45:47.997053 semantic_kernel-1.0.1/semantic_kernel/py.typed
+-rw-r--r--   0        0        0      545 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/kernel_reliability_extension.py
+-rw-r--r--   0        0        0      999 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      679 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     1559 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/schema/kernel_json_schema.py
+-rw-r--r--   0        0        0     2587 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/schema/kernel_json_schema_builder.py
+-rw-r--r--   0        0        0      157 2024-04-16 13:30:52.656626 semantic_kernel-1.0.1/semantic_kernel/services/__init__.py
+-rw-r--r--   0        0        0     1851 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/ai_service_client_base.py
+-rw-r--r--   0        0        0     2624 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/ai_service_selector.py
+-rw-r--r--   0        0        0     6202 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/services/kernel_services_extension.py
+-rw-r--r--   0        0        0     1115 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      251 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     7447 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2413 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0     3908 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/named_arg_block.py
+-rw-r--r--   0        0        0      346 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1672 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2376 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2924 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6569 2024-05-22 16:18:31.565428 semantic_kernel-1.0.1/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0      630 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0      673 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     6271 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      461 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      654 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8531 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      498 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/chat.py
+-rw-r--r--   0        0        0      841 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/experimental_decorator.py
+-rw-r--r--   0        0        0      276 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/utils/logging.py
+-rw-r--r--   0        0        0      560 2024-03-13 15:37:17.065380 semantic_kernel-1.0.1/semantic_kernel/utils/naming.py
+-rw-r--r--   0        0        0      269 2024-05-22 16:18:31.575428 semantic_kernel-1.0.1/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     4516 1970-01-01 00:00:00.000000 semantic_kernel-1.0.1/PKG-INFO
```

### Comparing `semantic_kernel-1.0.0rc1/pip/README.md` & `semantic_kernel-1.0.1/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/pyproject.toml` & `semantic_kernel-1.0.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,72 +1,61 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "1.0.0rc1"
+version = "1.0.1"
 description = "Semantic Kernel Python SDK"
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.10,<3.13"
 aiohttp = "^3.8"
 numpy = [
-    { version = "^1.24", python = "3.8" },
-    { version = ">=1.25", python = ">=3.9,<3.12" },
+    { version = ">=1.25", python = "<3.12" },
     { version = ">=1.26", python = ">=3.12" },
 ]
 scipy = [
     { version = ">=1.5.0", python = "<3.12" },
     { version = ">=1.12.0", python = ">=3.12" }
 ]
 grpcio = [
-    { version = ">=1.40.0", python = "3.8" },
-    { version = ">=1.50.0", python = ">=3.9" },
+    { version = ">=1.50.0", python = "<3.12" },
     { version = ">=1.60.0", python = ">=3.12" }
 ]
 openai = ">=1.0"
 regex = "^2023.6.3"
 openapi_core = ">=0.18,<0.20"
 prance = "^23.6.21.0"
 pydantic = "^2"
 pydantic-settings = "^2.2.1"
 motor = "^3.3.2"
 defusedxml = "^0.7.1"
 pybars4 = "^0.9.13"
 jinja2 = "^3.1.3"
 nest-asyncio = "^1.6.0"
-eval_type_backport = { version = "^0.1.3", markers = "python_version < '3.10'" }
 
 # Optional dependencies
 ipykernel = { version = "^6.21.1", optional = true}
 google-generativeai = { version = ">=0.1", markers = "python_version >= '3.9'", optional = true}
 grpcio-status = { version = "^1.53.0", markers = "python_version >= '3.9'", optional = true}
 transformers = { version = "^4.28.1", optional = true}
 sentence-transformers = { version = "^2.2.2", optional = true}
 torch = { version = "^2.2.0", optional = true}
-qdrant-client = [
-    { version = '^1.6', python = '3.8', optional = true },
-    { version = '>=1.7', python = '>3.9', optional = true }
-]
+qdrant-client = { version = '^1.9', optional = true}
 chromadb = { version = "^0.4.13", optional = true}
-pymilvus = [
-    { version = "^2.2,<2.3", markers = 'python_version == "3.8"', optional = true},
-    { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8"', optional = true}
-]
-milvus = [
-    { version = "^2.2,<2.3", markers = 'python_version == "3.8" and sys_platform != "win32"', optional = true},
-    { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8" and sys_platform != "win32"', optional = true}
-]
+pymilvus = { version = ">=2.3,<2.3.8", optional = true}
+milvus = { version = ">=2.3,<2.3.8", markers = 'sys_platform != "win32"', optional = true}
 weaviate-client = { version = ">=3.18,<5.0", optional = true}
 pinecone-client = { version = ">=3.0.0", optional = true}
 psycopg = { version="^3.1.9", extras=["binary","pool"], optional = true}
 redis = { version = "^4.6.0", optional = true}
-azure-search-documents = {version = "11.6.0b1", allow-prereleases = true, optional = true}
+azure-search-documents = {version = "11.6.0b4", allow-prereleases = true, optional = true}
 azure-core = { version = "^1.28.0", optional = true}
 azure-identity = { version = "^1.13.0", optional = true}
+azure-cosmos = { version = "^4.7.0", optional = true}
 usearch = { version = "^2.9", optional = true}
 pyarrow = { version = ">=12.0.1,<16.0.0", optional = true}
 
 # Groups are for development only (installed through Poetry)
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.5"
 black = "^24.2.0"
@@ -79,47 +68,43 @@
 mypy = ">=1.9.0"
 types-PyYAML = "^6.0.12.20240311"
 
 [tool.poetry.group.unit-tests]
 optional = true
 
 [tool.poetry.group.unit-tests.dependencies]
-google-generativeai = { version = ">=0.1,<0.4", markers = "python_version >= '3.9'"}
-azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
+google-generativeai = { version = ">=0.1,<0.4" }
+azure-search-documents = {version = "11.6.0b4", allow-prereleases = true}
 azure-core = "^1.28.0"
+azure-cosmos = "^4.7.0"
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "^2.2.0"
 
 [tool.poetry.group.tests]
 optional = true
 
 [tool.poetry.group.tests.dependencies]
-google-generativeai = { version = ">=0.1,<0.4", markers = "python_version >= '3.9'"}
-grpcio-status = { version = "^1.53.0", markers = "python_version >= '3.9'"}
+google-generativeai = { version = ">=0.1,<0.4" }
+grpcio-status = "^1.53.0"
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "^2.2.0"
-qdrant-client = {version = "^1.3.2", python = ">=3.8,<3.12"}
+qdrant-client = '^1.9'
 chromadb = "^0.4.13"
-pymilvus = [
-    { version = "^2.2,<2.3", markers = 'python_version == "3.8"'},
-    { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8"'}
-]
-milvus = [
-    { version = "^2.2,<2.3", markers = 'python_version == "3.8" and sys_platform != "win32"'},
-    { version = ">=2.3,<2.3.8", markers = 'python_version > "3.8" and sys_platform != "win32"'}
-]
+pymilvus = ">=2.3,<2.3.8"
+milvus = { version = ">=2.3,<2.3.8", markers = 'sys_platform != "win32"'}
 weaviate-client = ">=3.18,<5.0"
 pinecone-client = ">=3.0.0"
 psycopg = { version="^3.1.9", extras=["binary","pool"]}
 redis = "^4.6.0"
-azure-search-documents = {version = "11.6.0b1", allow-prereleases = true}
+azure-search-documents = {version = "11.6.0b4", allow-prereleases = true}
 azure-core = "^1.28.0"
 azure-identity = "^1.13.0"
+azure-cosmos = "^4.7.0"
 usearch = "^2.9"
 pyarrow = ">=12.0.1,<16.0.0"
 msgraph-sdk = "^1.2.0"
 
 # Extras are exposed to pip, this allows a user to easily add the right dependencies to their environment
 [tool.poetry.extras]
 google = ["google-generativeai", "grpcio-status"]
@@ -127,18 +112,18 @@
 qdrant = ["qdrant-client"]
 chromadb = ["chromadb"]
 milvus = ["pymilvus", "milvus"]
 weaviate = ["weaviate-client"]
 pinecone = ["pinecone-client"]
 postgres = ["psycopg"]
 redis = ["redis"]
-azure = ["azure-search-documents", "azure-core", "azure-identity", "msgraph-sdk"]
+azure = ["azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "msgraph-sdk"]
 usearch = ["usearch", "pyarrow"]
 notebooks = ["ipykernel"]
-all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "usearch", "pyarrow", "ipykernel"]
+all = ["google-generativeai", "grpcio-status", "transformers", "sentence-transformers", "torch", "qdrant-client", "chromadb", "pymilvus", "milvus", "weaviate-client", "pinecone-client", "psycopg", "redis", "azure-search-documents", "azure-core", "azure-identity", "azure-cosmos", "usearch", "pyarrow", "ipykernel"]
 
 [tool.ruff]
 lint.select = ["E", "F", "I"]
 line-length = 120
 
 [tool.black]
 line-length = 120
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, AsyncGenerator
+from collections.abc import AsyncGenerator
+from typing import TYPE_CHECKING, Any
 
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
     from semantic_kernel.contents.chat_history import ChatHistory
     from semantic_kernel.contents.chat_message_content import ChatMessageContent
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/function_call_behavior.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/function_call_behavior.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
-from typing import TYPE_CHECKING, Callable, Literal
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Literal
 
 from pydantic.dataclasses import dataclass
 
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 if TYPE_CHECKING:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/gp_prompt_execution_settings.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,45 +1,46 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Any, Dict, Iterable, List, Optional, Union
+from collections.abc import Iterable
+from typing import Any, Union
 
 from pydantic import Field, model_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.exceptions import ServiceInvalidExecutionSettingsError
 
 # TODO: replace back with google types once pydantic issue is fixed.
-MessagesOptions = List[Dict[str, Any]]
+MessagesOptions = list[dict[str, Any]]
 
-MessagePromptOption = Union[str, Dict[str, Any]]
-MessagePromptOptions = Union[MessagePromptOption, List[MessagePromptOption]]
+MessagePromptOption = Union[str, dict[str, Any]]
+MessagePromptOptions = Union[MessagePromptOption, list[MessagePromptOption]]
 
-ExampleOptions = Union[Dict[str, Any], List[Dict[str, Any]]]
+ExampleOptions = Union[dict[str, Any], list[dict[str, Any]]]
 
 
 class GooglePalmPromptExecutionSettings(PromptExecutionSettings):
-    ai_model_id: Optional[str] = Field(None, serialization_alias="model")
+    ai_model_id: str | None = Field(None, serialization_alias="model")
     temperature: float = Field(0.0, ge=0.0, le=1.0)
     top_p: float = 1.0
     top_k: int = 1
     candidate_count: int = Field(1, ge=1, le=8)
-    safety_settings: Optional[Dict[str, Any]] = None
-    prompt: Optional[MessagePromptOptions] = None
+    safety_settings: dict[str, Any] | None = None
+    prompt: MessagePromptOptions | None = None
 
 
 class GooglePalmTextPromptExecutionSettings(GooglePalmPromptExecutionSettings):
     max_output_tokens: int = Field(256, gt=0)
-    stop_sequences: Optional[Union[str, Iterable[str]]] = None
+    stop_sequences: str | Iterable[str] | None = None
 
 
 class GooglePalmChatPromptExecutionSettings(GooglePalmPromptExecutionSettings):
-    messages: Optional[MessagesOptions] = None
-    examples: Optional[ExampleOptions] = None
-    context: Optional[str] = None
-    token_selection_biases: Optional[Dict[int, int]] = None
+    messages: MessagesOptions | None = None
+    examples: ExampleOptions | None = None
+    context: str | None = None
+    token_selection_biases: dict[int, int] | None = None
 
     @model_validator(mode="after")
     def validate_input(self):
         if self.prompt is not None:
             if self.messages or self.context or self.examples:
                 raise ServiceInvalidExecutionSettingsError(
                     "Prompt cannot be used without messages, context or examples"
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Annotated, Any, List, Tuple
+from typing import Annotated, Any
 
 import google.generativeai as palm
 from google.generativeai.types import ChatResponse, MessageDict
 from pydantic import PrivateAttr, StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import (
@@ -72,15 +72,15 @@
         self._message_history = message_history
 
     async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
-    ) -> List[ChatMessageContent]:
+    ) -> list[ChatMessageContent]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
         Arguments:
             chat_history {List[ChatMessage]} -- A list of chat messages, that can be rendered into a
                 set of messages, from system, user, assistant and function.
             settings {GooglePalmPromptExecutionSettings} -- Settings for the request.
@@ -120,25 +120,25 @@
             metadata=metadata,
             role=int_to_role[int(candidate.get("author"))],  # TODO: why is author coming back as '1'?
             content=candidate.get("content"),
         )
 
     async def get_streaming_chat_message_contents(
         self,
-        messages: List[Tuple[str, str]],
+        messages: list[tuple[str, str]],
         settings: GooglePalmPromptExecutionSettings,
         **kwargs: Any,
     ):
         raise NotImplementedError("Google Palm API does not currently support streaming")
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: GooglePalmPromptExecutionSettings,
-    ) -> List[TextContent]:
+    ) -> list[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {GooglePalmPromptExecutionSettings} -- Settings for the request.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Annotated, List
+from typing import Annotated
 
 import google.generativeai as palm
 from google.generativeai.types import Completion
 from google.generativeai.types.text_types import TextCompletion
 from pydantic import StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.google_palm.gp_prompt_execution_settings import GooglePalmTextPromptExecutionSettings
@@ -47,15 +47,15 @@
             google_palm_settings.text_model_id if google_palm_settings and google_palm_settings.text_model_id else None
         )
 
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
     async def get_text_contents(
         self, prompt: str, settings: GooglePalmTextPromptExecutionSettings
-    ) -> List[TextContent]:
+    ) -> list[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {GooglePalmTextPromptExecutionSettings} -- Settings for the request.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/services/gp_text_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Annotated, Any, List
+from typing import Annotated, Any
 
 import google.generativeai as palm
 from numpy import array, ndarray
 from pydantic import StringConstraints, ValidationError
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.google_palm.settings.google_palm_settings import GooglePalmSettings
 from semantic_kernel.exceptions import ServiceInvalidAuthError, ServiceResponseException
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class GooglePalmTextEmbedding(EmbeddingGeneratorBase):
     api_key: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
 
     def __init__(self, ai_model_id: str, api_key: str | None = None, env_file_path: str | None = None) -> None:
         """
         Initializes a new instance of the GooglePalmTextEmbedding class.
 
@@ -42,15 +44,15 @@
         ai_model_id = ai_model_id or (
             google_palm_settings.embedding_model_id
             if google_palm_settings and google_palm_settings.embedding_model_id
             else None
         )
         super().__init__(ai_model_id=ai_model_id, api_key=api_key)
 
-    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
+    async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/google_palm/settings/google_palm_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/hf_prompt_execution_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Dict
+from typing import Any
 
 from transformers import GenerationConfig
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 
 
 class HuggingFacePromptExecutionSettings(PromptExecutionSettings):
@@ -21,15 +21,15 @@
                 include={"max_new_tokens", "pad_token_id", "eos_token_id", "temperature", "top_p"},
                 exclude_unset=False,
                 exclude_none=True,
                 by_alias=True,
             )
         )
 
-    def prepare_settings_dict(self, **kwargs) -> Dict[str, Any]:
+    def prepare_settings_dict(self, **kwargs) -> dict[str, Any]:
         gen_config = self.get_generation_config()
         settings = {
             "generation_config": gen_config,
             "num_return_sequences": self.num_return_sequences,
             "do_sample": self.do_sample,
         }
         settings.update(kwargs)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
+from collections.abc import AsyncGenerator
 from threading import Thread
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Literal, Optional
+from typing import TYPE_CHECKING, Any, Literal
 
 import torch
 from transformers import AutoTokenizer, TextIteratorStreamer, pipeline
 
 from semantic_kernel.connectors.ai.hugging_face.hf_prompt_execution_settings import HuggingFacePromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.streaming_text_content import StreamingTextContent
@@ -23,19 +24,19 @@
     task: Literal["summarization", "text-generation", "text2text-generation"]
     device: str
     generator: Any
 
     def __init__(
         self,
         ai_model_id: str,
-        task: Optional[str] = "text2text-generation",
-        device: Optional[int] = -1,
-        service_id: Optional[str] = None,
-        model_kwargs: Optional[Dict[str, Any]] = None,
-        pipeline_kwargs: Optional[Dict[str, Any]] = None,
+        task: str | None = "text2text-generation",
+        device: int | None = -1,
+        service_id: str | None = None,
+        model_kwargs: dict[str, Any] | None = None,
+        pipeline_kwargs: dict[str, Any] | None = None,
     ) -> None:
         """
         Initializes a new instance of the HuggingFaceTextCompletion class.
 
         Arguments:
             ai_model_id {str} -- Hugging Face model card string, see
                 https://huggingface.co/models
@@ -73,15 +74,15 @@
             generator=generator,
         )
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
-    ) -> List[TextContent]:
+    ) -> list[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {HuggingFacePromptExecutionSettings} -- Settings for the request.
 
@@ -92,26 +93,26 @@
             results = self.generator(prompt, **settings.prepare_settings_dict())
         except Exception as e:
             raise ServiceResponseException("Hugging Face completion failed", e) from e
         if isinstance(results, list):
             return [self._create_text_content(results, result) for result in results]
         return [self._create_text_content(results, results)]
 
-    def _create_text_content(self, response: Any, candidate: Dict[str, str]) -> TextContent:
+    def _create_text_content(self, response: Any, candidate: dict[str, str]) -> TextContent:
         return TextContent(
             inner_content=response,
             ai_model_id=self.ai_model_id,
             text=candidate["summary_text" if self.task == "summarization" else "generated_text"],
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: HuggingFacePromptExecutionSettings,
-    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
+    ) -> AsyncGenerator[list[StreamingTextContent], Any]:
         """
         Streams a text completion using a Hugging Face model.
         Note that this method does not support multiple responses.
 
         Arguments:
             prompt {str} -- Prompt to complete.
             settings {HuggingFacePromptExecutionSettings} -- Request settings.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,33 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Any, List, Optional
+from typing import Any
 
 import sentence_transformers
 import torch
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.exceptions import ServiceResponseException
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class HuggingFaceTextEmbedding(EmbeddingGeneratorBase):
     device: str
     generator: Any
 
     def __init__(
         self,
         ai_model_id: str,
-        device: Optional[int] = -1,
-        service_id: Optional[str] = None,
+        device: int | None = -1,
+        service_id: str | None = None,
     ) -> None:
         """
         Initializes a new instance of the HuggingFaceTextEmbedding class.
 
         Arguments:
             ai_model_id {str} -- Hugging Face model card string, see
                 https://huggingface.co/sentence-transformers
@@ -38,15 +40,15 @@
         super().__init__(
             ai_model_id=ai_model_id,
             service_id=service_id,
             device=resolved_device,
             generator=sentence_transformers.SentenceTransformer(model_name_or_path=ai_model_id, device=resolved_device),
         )
 
-    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
+    async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_chat_completion.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import Any, AsyncGenerator, List, Optional
+from collections.abc import AsyncGenerator
+from typing import Any
 
 import aiohttp
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.ollama.ollama_prompt_execution_settings import OllamaChatPromptExecutionSettings
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
@@ -29,22 +30,22 @@
     Arguments:
         ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/chat
         session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/chat"
-    session: Optional[aiohttp.ClientSession] = None
+    session: aiohttp.ClientSession | None = None
 
     async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> List[ChatMessageContent]:
+    ) -> list[ChatMessageContent]:
         """
         This is the method that is called from the kernel to get a response from a chat-optimized LLM.
 
         Arguments:
             chat_history {ChatHistory} -- A chat history that contains a list of chat messages,
                 that can be rendered into a set of messages, from system, user, assistant and function.
             settings {PromptExecutionSettings} -- Settings for the request.
@@ -71,15 +72,15 @@
                 ]
 
     async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OllamaChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> AsyncGenerator[List[StreamingChatMessageContent], Any]:
+    ) -> AsyncGenerator[list[StreamingChatMessageContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses.
 
         Arguments:
             chat_history {ChatHistory} -- A chat history that contains a list of chat messages,
                 that can be rendered into a set of messages, from system, user, assistant and function.
@@ -112,15 +113,15 @@
                     if body.get("done"):
                         break
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
-    ) -> List[TextContent]:
+    ) -> list[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             chat_history {ChatHistory} -- A chat history that contains the prompt to complete.
             settings {OllamaChatPromptExecutionSettings} -- Settings for the request.
 
@@ -143,15 +144,15 @@
                     )
                 ]
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaChatPromptExecutionSettings,
-    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
+    ) -> AsyncGenerator[list[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses.
 
         Arguments:
             prompt {str} -- A chat history that contains the prompt to complete.
             settings {OllamaChatPromptExecutionSettings} -- Request settings.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import Any, AsyncGenerator, List, Optional
+from collections.abc import AsyncGenerator
+from typing import Any
 
 import aiohttp
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.ollama.ollama_prompt_execution_settings import OllamaTextPromptExecutionSettings
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
@@ -24,21 +25,21 @@
 
     Arguments:
         ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/generate
     """
 
     url: HttpUrl = "http://localhost:11434/api/generate"
-    session: Optional[aiohttp.ClientSession] = None
+    session: aiohttp.ClientSession | None = None
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
-    ) -> List[TextContent]:
+    ) -> list[TextContent]:
         """
         This is the method that is called from the kernel to get a response from a text-optimized LLM.
 
         Arguments:
             prompt {str} -- The prompt to send to the LLM.
             settings {OllamaTextPromptExecutionSettings} -- Settings for the request.
 
@@ -56,15 +57,15 @@
                 text = inner_content["response"]
                 return [TextContent(inner_content=inner_content, ai_model_id=self.ai_model_id, text=text)]
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: OllamaTextPromptExecutionSettings,
-    ) -> AsyncGenerator[List[StreamingTextContent], Any]:
+    ) -> AsyncGenerator[list[StreamingTextContent], Any]:
         """
         Streams a text completion using a Ollama model.
         Note that this method does not support multiple responses,
         but the result will be a list anyway.
 
         Arguments:
             prompt {str} -- Prompt to complete.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/ollama/services/ollama_text_embedding.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Any, List, Optional
+from typing import Any
 
 import aiohttp
 from numpy import array, ndarray
 from pydantic import HttpUrl
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.ollama.utils import AsyncSession
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class OllamaTextEmbedding(EmbeddingGeneratorBase):
     """Ollama embeddings client.
 
     Make sure to have the ollama service running either locally or remotely.
 
     Arguments:
         ai_model_id {str} -- Ollama model name, see https://ollama.ai/library
         url {Optional[Union[str, HttpUrl]]} -- URL of the Ollama server, defaults to http://localhost:11434/api/embeddings
         session {Optional[aiohttp.ClientSession]} -- Optional client session to use for requests.
     """
 
     url: HttpUrl = "http://localhost:11434/api/embeddings"
-    session: Optional[aiohttp.ClientSession] = None
+    session: aiohttp.ClientSession | None = None
 
-    async def generate_embeddings(self, texts: List[str], **kwargs: Any) -> ndarray:
+    async def generate_embeddings(self, texts: list[str], **kwargs: Any) -> ndarray:
         """
         Generates embeddings for a list of texts.
 
         Arguments:
             texts {List[str]} -- Texts to generate embeddings for.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/exceptions/content_filter_ai_exception.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from dataclasses import dataclass
 from enum import Enum
-from typing import Any, Dict
+from typing import Any
 
 from openai import BadRequestError
 
 from semantic_kernel.exceptions import ServiceContentFilterException
 
 
 class ContentFilterResultSeverity(Enum):
@@ -18,15 +18,15 @@
 @dataclass
 class ContentFilterResult:
     filtered: bool = False
     detected: bool = False
     severity: ContentFilterResultSeverity = ContentFilterResultSeverity.SAFE
 
     @classmethod
-    def from_inner_error_result(cls, inner_error_results: Dict[str, Any]) -> "ContentFilterResult":
+    def from_inner_error_result(cls, inner_error_results: dict[str, Any]) -> "ContentFilterResult":
         """Creates a ContentFilterResult from the inner error results.
 
         Arguments:
             key {str} -- The key to get the inner error result from.
             inner_error_results {Dict[str, Any]} -- The inner error results.
 
         Returns:
@@ -52,15 +52,15 @@
     # The parameter that caused the error.
     param: str
 
     # The error code specific to the content filter.
     content_filter_code: ContentFilterCodes
 
     # The results of the different content filter checks.
-    content_filter_result: Dict[str, ContentFilterResult]
+    content_filter_result: dict[str, ContentFilterResult]
 
     def __init__(
         self,
         message: str,
         inner_exception: BadRequestError,
     ) -> None:
         """Initializes a new instance of the ContentFilterAIException class.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/prompt_execution_settings/azure_chat_prompt_execution_settings.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import logging
-from typing import Any, Dict, List, Literal, Optional, Union
+from typing import Annotated, Any, Literal, Union
 
 from pydantic import AliasGenerator, ConfigDict, Field
 from pydantic.alias_generators import to_camel, to_snake
 from pydantic.functional_validators import AfterValidator
-from typing_extensions import Annotated
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 logger = logging.getLogger(__name__)
@@ -20,84 +19,84 @@
         use_enum_values=True,
         extra="allow",
     )
 
 
 class ConnectionStringAuthentication(AzureChatRequestBase):
     type: Annotated[Literal["ConnectionString", "connection_string"], AfterValidator(to_snake)] = "connection_string"
-    connection_string: Optional[str] = None
+    connection_string: str | None = None
 
 
 class ApiKeyAuthentication(AzureChatRequestBase):
     type: Annotated[Literal["APIKey", "api_key"], AfterValidator(to_snake)] = "api_key"
-    key: Optional[str] = None
+    key: str | None = None
 
 
 class AzureEmbeddingDependency(AzureChatRequestBase):
     type: Annotated[Literal["DeploymentName", "deployment_name"], AfterValidator(to_snake)] = "deployment_name"
-    deployment_name: Optional[str] = None
+    deployment_name: str | None = None
 
 
 class DataSourceFieldsMapping(AzureChatRequestBase):
-    title_field: Optional[str] = None
-    url_field: Optional[str] = None
-    filepath_field: Optional[str] = None
-    content_fields: Optional[List[str]] = None
-    vector_fields: Optional[List[str]] = None
-    content_fields_separator: Optional[str] = "\n"
+    title_field: str | None = None
+    url_field: str | None = None
+    filepath_field: str | None = None
+    content_fields: list[str] | None = None
+    vector_fields: list[str] | None = None
+    content_fields_separator: str | None = "\n"
 
 
 class AzureDataSourceParameters(AzureChatRequestBase):
     index_name: str
-    index_language: Optional[str] = None
-    fields_mapping: Optional[DataSourceFieldsMapping] = None
-    in_scope: Optional[bool] = True
-    top_n_documents: Optional[int] = 5
-    semantic_configuration: Optional[str] = None
-    role_information: Optional[str] = None
-    filter: Optional[str] = None
+    index_language: str | None = None
+    fields_mapping: DataSourceFieldsMapping | None = None
+    in_scope: bool | None = True
+    top_n_documents: int | None = 5
+    semantic_configuration: str | None = None
+    role_information: str | None = None
+    filter: str | None = None
     strictness: int = 3
-    embedding_dependency: Optional[AzureEmbeddingDependency] = None
+    embedding_dependency: AzureEmbeddingDependency | None = None
 
 
 class AzureCosmosDBDataSourceParameters(AzureDataSourceParameters):
-    authentication: Optional[ConnectionStringAuthentication] = None
-    database_name: Optional[str] = None
-    container_name: Optional[str] = None
-    embedding_dependency_type: Optional[AzureEmbeddingDependency] = None
+    authentication: ConnectionStringAuthentication | None = None
+    database_name: str | None = None
+    container_name: str | None = None
+    embedding_dependency_type: AzureEmbeddingDependency | None = None
 
 
 class AzureCosmosDBDataSource(AzureChatRequestBase):
     type: Literal["azure_cosmos_db"] = "azure_cosmos_db"
     parameters: AzureCosmosDBDataSourceParameters
 
 
 class AzureAISearchDataSourceParameters(AzureDataSourceParameters):
-    endpoint: Optional[str] = None
+    endpoint: str | None = None
     query_type: Annotated[
         Literal["simple", "semantic", "vector", "vectorSimpleHybrid", "vectorSemanticHybrid"], AfterValidator(to_snake)
     ] = "simple"
-    authentication: Optional[ApiKeyAuthentication] = None
+    authentication: ApiKeyAuthentication | None = None
 
 
 class AzureAISearchDataSource(AzureChatRequestBase):
     type: Literal["azure_search"] = "azure_search"
     parameters: Annotated[dict, AzureAISearchDataSourceParameters]
 
 
 DataSource = Annotated[Union[AzureAISearchDataSource, AzureCosmosDBDataSource], Field(discriminator="type")]
 
 
 class ExtraBody(KernelBaseModel):
-    data_sources: Optional[List[DataSource]] = None
-    input_language: Optional[str] = Field(None, serialization_alias="inputLanguage")
-    output_language: Optional[str] = Field(None, serialization_alias="outputLanguage")
+    data_sources: list[DataSource] | None = None
+    input_language: str | None = Field(None, serialization_alias="inputLanguage")
+    output_language: str | None = Field(None, serialization_alias="outputLanguage")
 
     def __getitem__(self, item):
         return getattr(self, item)
 
 
 class AzureChatPromptExecutionSettings(OpenAIChatPromptExecutionSettings):
     """Specific settings for the Azure OpenAI Chat Completion endpoint."""
 
-    response_format: Optional[str] = None
-    extra_body: Optional[Union[Dict[str, Any], ExtraBody]] = None
+    response_format: str | None = None
+    extra_body: dict[str, Any] | ExtraBody | None = None
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 import json
 import logging
+from collections.abc import Mapping
 from copy import deepcopy
-from typing import Any, Dict, Mapping, Optional, Union
+from typing import Any
 from uuid import uuid4
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
@@ -116,15 +117,15 @@
             ad_token_provider=ad_token_provider,
             default_headers=default_headers,
             ai_model_type=OpenAIModelTypes.CHAT,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: Dict[str, str]) -> "AzureChatCompletion":
+    def from_dict(cls, settings: dict[str, str]) -> "AzureChatCompletion":
         """
         Initialize an Azure OpenAI service from a dictionary of settings.
 
         Arguments:
             settings: A dictionary of settings for the service.
                 should contains keys: service_id, and optionally:
                     ad_auth, ad_token_provider, default_headers
@@ -144,25 +145,25 @@
         )
 
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Create a request settings object."""
         return AzureChatPromptExecutionSettings
 
     def _create_chat_message_content(
-        self, response: ChatCompletion, choice: Choice, response_metadata: Dict[str, Any]
+        self, response: ChatCompletion, choice: Choice, response_metadata: dict[str, Any]
     ) -> ChatMessageContent:
         """Create a Azure chat message content object from a choice."""
         content = super()._create_chat_message_content(response, choice, response_metadata)
         return self._add_tool_message_to_chat_message_content(content, choice)
 
     def _create_streaming_chat_message_content(
         self,
         chunk: ChatCompletionChunk,
         choice: ChunkChoice,
-        chunk_metadata: Dict[str, Any],
+        chunk_metadata: dict[str, Any],
     ) -> "StreamingChatMessageContent":
         """Create a Azure streaming chat message content object from a choice."""
         content = super()._create_streaming_chat_message_content(chunk, choice, chunk_metadata)
         return self._add_tool_message_to_chat_message_content(content, choice)
 
     def _add_tool_message_to_chat_message_content(
         self, content: ChatMessageContent | StreamingChatMessageContent, choice: Choice
@@ -182,15 +183,15 @@
             result = FunctionResultContent.from_function_call_content_and_result(
                 result=tool_message_dict["citations"], function_call_content=function_call
             )
             content.items.insert(0, function_call)
             content.items.insert(1, result)
         return content
 
-    def _get_tool_message_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Optional[str]:
+    def _get_tool_message_from_chat_choice(self, choice: Choice | ChunkChoice) -> str | None:
         """Get the tool message from a choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.model_extra is not None and "context" in content.model_extra:
             return json.dumps(content.model_extra["context"])
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_config_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Awaitable, Callable, Dict, Mapping, Optional, Union
+from collections.abc import Awaitable, Callable, Mapping
 
 from openai import AsyncAzureOpenAI
 from pydantic import ConfigDict, validate_call
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION, USER_AGENT
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler, OpenAIModelTypes
 from semantic_kernel.connectors.telemetry import APP_INFO, prepend_semantic_kernel_to_user_agent
@@ -19,23 +19,23 @@
     """Internal class for configuring a connection to an Azure OpenAI service."""
 
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def __init__(
         self,
         deployment_name: str,
         ai_model_type: OpenAIModelTypes,
-        endpoint: Optional[HttpsUrl] = None,
-        base_url: Optional[HttpsUrl] = None,
+        endpoint: HttpsUrl | None = None,
+        base_url: HttpsUrl | None = None,
         api_version: str = DEFAULT_AZURE_API_VERSION,
-        service_id: Optional[str] = None,
-        api_key: Optional[str] = None,
-        ad_token: Optional[str] = None,
-        ad_token_provider: Optional[Callable[[], Union[str, Awaitable[str]]]] = None,
-        default_headers: Union[Mapping[str, str], None] = None,
-        async_client: Optional[AsyncAzureOpenAI] = None,
+        service_id: str | None = None,
+        api_key: str | None = None,
+        ad_token: str | None = None,
+        ad_token_provider: Callable[[], str | Awaitable[str]] | None = None,
+        default_headers: Mapping[str, str] | None = None,
+        async_client: AsyncAzureOpenAI | None = None,
     ) -> None:
         """Internal class for configuring a connection to an Azure OpenAI service.
 
         Arguments:
             deployment_name {str} -- Name of the deployment.
             ai_model_type {OpenAIModelTypes} -- The type of OpenAI model to deploy.
             endpoint {Optional[HttpsUrl]} -- The specific endpoint URL for the deployment. (Optional)
@@ -86,15 +86,15 @@
             "client": async_client,
             "ai_model_type": ai_model_type,
         }
         if service_id:
             args["service_id"] = service_id
         super().__init__(**args)
 
-    def to_dict(self) -> Dict[str, str]:
+    def to_dict(self) -> dict[str, str]:
         client_settings = {
             "base_url": str(self.client.base_url),
             "api_version": self.client._custom_query["api-version"],
             "api_key": self.client.api_key,
             "ad_token": self.client._azure_ad_token,
             "ad_token_provider": self.client._azure_ad_token_provider,
             "default_headers": {k: v for k, v in self.client.default_headers.items() if k != USER_AGENT},
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Mapping
+from collections.abc import Mapping
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
 from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import (
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 import logging
-from typing import Mapping
+from collections.abc import Mapping
 
 from openai import AsyncAzureOpenAI
 from openai.lib.azure import AsyncAzureADTokenProvider
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.const import DEFAULT_AZURE_API_VERSION
 from semantic_kernel.connectors.ai.open_ai.services.azure_config_base import (
@@ -17,18 +17,20 @@
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
 from semantic_kernel.connectors.ai.open_ai.settings.azure_open_ai_settings import AzureOpenAISettings
 from semantic_kernel.exceptions.service_exceptions import ServiceInitializationError
 from semantic_kernel.kernel_pydantic import HttpsUrl
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class AzureTextEmbedding(AzureOpenAIConfigBase, OpenAITextEmbeddingBase):
     """Azure Text Embedding class."""
 
     def __init__(
         self,
         service_id: str | None = None,
         api_key: str | None = None,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import (
-    Dict,
-    Mapping,
-)
+from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_chat_completion_base import OpenAIChatCompletionBase
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import OpenAIConfigBase
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
@@ -73,15 +70,15 @@
             service_id=service_id,
             ai_model_type=OpenAIModelTypes.CHAT,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: Dict[str, str]) -> "OpenAIChatCompletion":
+    def from_dict(cls, settings: dict[str, str]) -> "OpenAIChatCompletion":
         """
         Initialize an Open AI service from a dictionary of settings.
 
         Arguments:
             settings: A dictionary of settings for the service.
         """
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
+from collections.abc import AsyncGenerator
 from copy import copy
 from functools import reduce
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Optional, Union
+from typing import TYPE_CHECKING, Any
 
 from openai import AsyncStream
 from openai.types.chat.chat_completion import ChatCompletion, Choice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 from openai.types.chat.chat_completion_chunk import Choice as ChunkChoice
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
@@ -37,16 +38,16 @@
     ServiceInvalidExecutionSettingsError,
     ServiceInvalidResponseError,
 )
 from semantic_kernel.filters.auto_function_invocation.auto_function_invocation_context import (
     AutoFunctionInvocationContext,
 )
 from semantic_kernel.filters.filter_types import FilterTypes
+from semantic_kernel.filters.kernel_filters_extension import _rebuild_auto_function_invocation_context
 from semantic_kernel.functions.function_result import FunctionResult
-from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_auto_function_invocation_context
 
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.kernel import Kernel
 
 logger: logging.Logger = logging.getLogger(__name__)
 
@@ -69,15 +70,15 @@
         return OpenAIChatPromptExecutionSettings
 
     async def get_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> List["ChatMessageContent"]:
+    ) -> list["ChatMessageContent"]:
         """Executes a chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
@@ -89,15 +90,15 @@
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
             if kernel is None or arguments is None:
                 raise ServiceInvalidExecutionSettingsError(
                     "The kernel and kernel arguments are required for auto invoking OpenAI tool calls."
                 )
-            if settings.number_of_responses > 1:
+            if settings.number_of_responses is not None and settings.number_of_responses > 1:
                 raise ServiceInvalidExecutionSettingsError(
                     "Auto-invocation of tool calls may only be used with a "
                     "OpenAIChatPromptExecutions.number_of_responses of 1."
                 )
 
         # behavior for non-function calling or for enable, but not auto-invoke.
         self._prepare_settings(settings, chat_history, stream_request=False, kernel=kernel)
@@ -146,15 +147,15 @@
             return await self._send_chat_request(settings)
 
     async def get_streaming_chat_message_contents(
         self,
         chat_history: ChatHistory,
         settings: OpenAIChatPromptExecutionSettings,
         **kwargs: Any,
-    ) -> AsyncGenerator[List[StreamingChatMessageContent | None], Any]:
+    ) -> AsyncGenerator[list[StreamingChatMessageContent | None], Any]:
         """Executes a streaming chat completion request and returns the result.
 
         Arguments:
             chat_history {ChatHistory} -- The chat history to use for the chat completion.
             settings {OpenAIChatPromptExecutionSettings | AzureChatPromptExecutionSettings} -- The settings to use
                 for the chat completion request.
             kwargs {Dict[str, Any]} -- The optional arguments.
@@ -166,15 +167,15 @@
         kernel = kwargs.get("kernel", None)
         arguments = kwargs.get("arguments", None)
         if settings.function_call_behavior is not None and settings.function_call_behavior.auto_invoke_kernel_functions:
             if kernel is None or arguments is None:
                 raise ServiceInvalidExecutionSettingsError(
                     "The kernel argument and arguments are required for OpenAI tool calling."
                 )
-            if settings.number_of_responses > 1:
+            if settings.number_of_responses is not None and settings.number_of_responses > 1:
                 raise ServiceInvalidExecutionSettingsError(
                     "Auto-invocation of tool calls may only be used with a "
                     "OpenAIChatPromptExecutions.number_of_responses of 1."
                 )
 
         # Prepare settings for streaming requests
         self._prepare_settings(settings, chat_history, stream_request=True, kernel=kernel)
@@ -204,20 +205,20 @@
                 # no need to process function calls
                 # note that we don't check the FinishReason and instead check whether there are any tool calls,
                 # as the service may return a FinishReason of "stop" even if there are tool calls to be made,
                 # in particular if a required tool is specified.
                 return
 
             # there is one response stream in the messages, combining now to create the full completion
+            # depending on the prompt, the message may contain both function call content and others
             full_completion: StreamingChatMessageContent = reduce(lambda x, y: x + y, all_messages)
+            function_calls = [item for item in full_completion.items if isinstance(item, FunctionCallContent)]
             chat_history.add_message(message=full_completion)
 
-            function_calls = [item for item in chat_history.messages[-1].items if isinstance(item, FunctionCallContent)]
             fc_count = len(function_calls)
-
             logger.info(f"processing {fc_count} tool calls in parallel.")
 
             # this function either updates the chat history with the function call results
             # or returns the context, with terminate set to True
             # in which case the loop will break and the function calls are returned.
             # Exceptions are not caught, that is up to the developer, can be done with a filter
             results = await asyncio.gather(
@@ -235,15 +236,15 @@
                 ],
             )
             if any(result.terminate for result in results if result is not None):
                 return
 
             self._update_settings(settings, chat_history, kernel=kernel)
 
-    def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> Dict[str, Optional[str]]:
+    def _chat_message_content_to_dict(self, message: "ChatMessageContent") -> dict[str, str | None]:
         msg = super()._chat_message_content_to_dict(message)
         if message.role == "assistant":
             if tool_calls := getattr(message, "tool_calls", None):
                 msg["tool_calls"] = [tool_call.model_dump() for tool_call in tool_calls]
             if function_call := getattr(message, "function_call", None):
                 msg["function_call"] = function_call.model_dump_json()
         if message.role == "tool":
@@ -252,15 +253,15 @@
             if message.metadata and "function" in message.metadata:
                 msg["name"] = message.metadata["function_name"]
         return msg
 
     # endregion
     # region internal handlers
 
-    async def _send_chat_request(self, settings: OpenAIChatPromptExecutionSettings) -> List["ChatMessageContent"]:
+    async def _send_chat_request(self, settings: OpenAIChatPromptExecutionSettings) -> list["ChatMessageContent"]:
         """Send the chat request"""
         response = await self._send_request(request_settings=settings)
         response_metadata = self._get_metadata_from_chat_response(response)
         completions = [
             self._create_chat_message_content(response, choice, response_metadata) for choice in response.choices
         ]
         return completions
@@ -280,15 +281,15 @@
                 self._create_streaming_chat_message_content(chunk, choice, chunk_metadata) for choice in chunk.choices
             ]
 
     # endregion
     # region content creation
 
     def _create_chat_message_content(
-        self, response: ChatCompletion, choice: Choice, response_metadata: Dict[str, Any]
+        self, response: ChatCompletion, choice: Choice, response_metadata: dict[str, Any]
     ) -> "ChatMessageContent":
         """Create a chat message content object from a choice."""
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(response_metadata)
 
         items: list[Any] = self._get_tool_calls_from_chat_choice(choice)
         items.extend(self._get_function_call_from_chat_choice(choice))
@@ -304,15 +305,15 @@
             finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason else None,
         )
 
     def _create_streaming_chat_message_content(
         self,
         chunk: ChatCompletionChunk,
         choice: ChunkChoice,
-        chunk_metadata: Dict[str, Any],
+        chunk_metadata: dict[str, Any],
     ) -> StreamingChatMessageContent | None:
         """Create a streaming chat message content object from a choice."""
         metadata = self._get_metadata_from_chat_choice(choice)
         metadata.update(chunk_metadata)
 
         items: list[Any] = self._get_tool_calls_from_chat_choice(choice)
         items.extend(self._get_function_call_from_chat_choice(choice))
@@ -324,38 +325,38 @@
             ai_model_id=self.ai_model_id,
             metadata=metadata,
             role=AuthorRole(choice.delta.role) if choice.delta.role else AuthorRole.ASSISTANT,
             finish_reason=FinishReason(choice.finish_reason) if choice.finish_reason else None,
             items=items,
         )
 
-    def _get_metadata_from_chat_response(self, response: ChatCompletion) -> Dict[str, Any]:
+    def _get_metadata_from_chat_response(self, response: ChatCompletion) -> dict[str, Any]:
         """Get metadata from a chat response."""
         return {
             "id": response.id,
             "created": response.created,
             "system_fingerprint": response.system_fingerprint,
             "usage": getattr(response, "usage", None),
         }
 
-    def _get_metadata_from_streaming_chat_response(self, response: ChatCompletionChunk) -> Dict[str, Any]:
+    def _get_metadata_from_streaming_chat_response(self, response: ChatCompletionChunk) -> dict[str, Any]:
         """Get metadata from a streaming chat response."""
         return {
             "id": response.id,
             "created": response.created,
             "system_fingerprint": response.system_fingerprint,
         }
 
-    def _get_metadata_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> Dict[str, Any]:
+    def _get_metadata_from_chat_choice(self, choice: Choice | ChunkChoice) -> dict[str, Any]:
         """Get metadata from a chat choice."""
         return {
             "logprobs": getattr(choice, "logprobs", None),
         }
 
-    def _get_tool_calls_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> List[FunctionCallContent]:
+    def _get_tool_calls_from_chat_choice(self, choice: Choice | ChunkChoice) -> list[FunctionCallContent]:
         """Get tool calls from a chat choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.tool_calls is None:
             return []
@@ -365,15 +366,15 @@
                 index=getattr(tool, "index", None),
                 name=tool.function.name,
                 arguments=tool.function.arguments,
             )
             for tool in content.tool_calls
         ]
 
-    def _get_function_call_from_chat_choice(self, choice: Union[Choice, ChunkChoice]) -> List[FunctionCallContent]:
+    def _get_function_call_from_chat_choice(self, choice: Choice | ChunkChoice) -> list[FunctionCallContent]:
         """Get a function call from a chat choice."""
         if isinstance(choice, Choice):
             content = choice.message
         else:
             content = choice.delta
         if content.function_call is None:
             return []
@@ -411,15 +412,15 @@
             settings.function_call_behavior.configure(
                 kernel=kernel,
                 update_settings_callback=update_settings_from_function_call_configuration,
                 settings=settings,
             )
 
     # endregion
-    # region tool calling
+    # region function calling
 
     async def _process_function_call(
         self,
         function_call: FunctionCallContent,
         chat_history: ChatHistory,
         kernel: "Kernel",
         arguments: "KernelArguments",
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_config_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Dict, Mapping, Optional
+from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ConfigDict, Field, validate_call
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_model_types import OpenAIModelTypes
@@ -16,20 +16,20 @@
 
 
 class OpenAIConfigBase(OpenAIHandler):
     @validate_call(config=ConfigDict(arbitrary_types_allowed=True))
     def __init__(
         self,
         ai_model_id: str = Field(min_length=1),
-        api_key: Optional[str] = Field(min_length=1),
-        ai_model_type: Optional[OpenAIModelTypes] = OpenAIModelTypes.CHAT,
-        org_id: Optional[str] = None,
-        service_id: Optional[str] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-        async_client: Optional[AsyncOpenAI] = None,
+        api_key: str | None = Field(min_length=1),
+        ai_model_type: OpenAIModelTypes | None = OpenAIModelTypes.CHAT,
+        org_id: str | None = None,
+        service_id: str | None = None,
+        default_headers: Mapping[str, str] | None = None,
+        async_client: AsyncOpenAI | None = None,
     ) -> None:
         """Initialize a client for OpenAI services.
 
         This constructor sets up a client to interact with OpenAI's API, allowing for
         different types of AI model interactions, like chat or text completion.
 
         Arguments:
@@ -64,15 +64,15 @@
             "client": async_client,
             "ai_model_type": ai_model_type,
         }
         if service_id:
             args["service_id"] = service_id
         super().__init__(**args)
 
-    def to_dict(self) -> Dict[str, str]:
+    def to_dict(self) -> dict[str, str]:
         """
         Create a dict of the service settings.
         """
         client_settings = {
             "api_key": self.client.api_key,
             "default_headers": {k: v for k, v in self.client.default_headers.items() if k != USER_AGENT},
         }
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_handler.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from abc import ABC
-from typing import List, Union
 
 from numpy import array, ndarray
 from openai import AsyncOpenAI, AsyncStream, BadRequestError
 from openai.types import Completion
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
 
 from semantic_kernel.connectors.ai.open_ai.exceptions.content_filter_ai_exception import (
@@ -33,15 +32,15 @@
     prompt_tokens: int = 0
     completion_tokens: int = 0
     total_tokens: int = 0
 
     async def _send_request(
         self,
         request_settings: OpenAIPromptExecutionSettings,
-    ) -> Union[ChatCompletion, Completion, AsyncStream[ChatCompletionChunk], AsyncStream[Completion]]:
+    ) -> ChatCompletion | Completion | AsyncStream[ChatCompletionChunk] | AsyncStream[Completion]:
         """
         Completes the given prompt. Returns a single string completion.
         Cannot return multiple completions. Cannot return logprobs.
 
         Arguments:
             prompt {str} -- The prompt to complete.
             messages {List[Tuple[str, str]]} -- A list of tuples, where each tuple is a role and content set.
@@ -71,15 +70,15 @@
             ) from ex
         except Exception as ex:
             raise ServiceResponseException(
                 f"{type(self)} service failed to complete the prompt",
                 ex,
             ) from ex
 
-    async def _send_embedding_request(self, settings: OpenAIEmbeddingPromptExecutionSettings) -> List[ndarray]:
+    async def _send_embedding_request(self, settings: OpenAIEmbeddingPromptExecutionSettings) -> list[ndarray]:
         try:
             response = await self.client.embeddings.create(**settings.prepare_settings_dict())
             self.store_usage(response)
             # make numpy arrays from the response
             # TODO: the openai response is cast to a list[float], could be used instead of ndarray
             return [array(x.embedding) for x in response.data]
         except Exception as ex:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
-from typing import Dict, Mapping, Optional
+from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
     OpenAIConfigBase,
 )
@@ -25,17 +25,17 @@
     """OpenAI Text Completion class."""
 
     def __init__(
         self,
         ai_model_id: str | None = None,
         api_key: str | None = None,
         org_id: str | None = None,
-        service_id: Optional[str] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-        async_client: Optional[AsyncOpenAI] = None,
+        service_id: str | None = None,
+        default_headers: Mapping[str, str] | None = None,
+        async_client: AsyncOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
         """
         Initialize an OpenAITextCompletion service.
 
         Arguments:
             ai_model_id {str | None} -- OpenAI model name, see
@@ -71,15 +71,15 @@
             service_id=service_id,
             ai_model_type=OpenAIModelTypes.TEXT,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: Dict[str, str]) -> "OpenAITextCompletion":
+    def from_dict(cls, settings: dict[str, str]) -> "OpenAITextCompletion":
         """
         Initialize an Open AI service from a dictionary of settings.
 
         Arguments:
             settings: A dictionary of settings for the service.
         """
         if "default_headers" in settings and isinstance(settings["default_headers"], str):
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, AsyncGenerator, Dict, List, Union
+from collections.abc import AsyncGenerator
+from typing import TYPE_CHECKING, Any
 
 from openai import AsyncStream
 from openai.types import Completion, CompletionChoice
 from openai.types.chat.chat_completion import Choice as ChatCompletionChoice
 from openai.types.chat.chat_completion_chunk import ChatCompletionChunk
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
@@ -31,15 +32,15 @@
         """Create a request settings object."""
         return OpenAITextPromptExecutionSettings
 
     async def get_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
-    ) -> List["TextContent"]:
+    ) -> list["TextContent"]:
         """Executes a completion request and returns the result.
 
         Arguments:
             prompt {str} -- The prompt to use for the completion request.
             settings {OpenAITextPromptExecutionSettings} -- The settings to use for the completion request.
 
         Returns:
@@ -54,16 +55,16 @@
         response = await self._send_request(request_settings=settings)
         metadata = self._get_metadata_from_text_response(response)
         return [self._create_text_content(response, choice, metadata) for choice in response.choices]
 
     def _create_text_content(
         self,
         response: Completion,
-        choice: Union[CompletionChoice, ChatCompletionChoice],
-        response_metadata: Dict[str, Any],
+        choice: CompletionChoice | ChatCompletionChoice,
+        response_metadata: dict[str, Any],
     ) -> "TextContent":
         """Create a text content object from a choice."""
         choice_metadata = self._get_metadata_from_text_choice(choice)
         choice_metadata.update(response_metadata)
         text = choice.text if isinstance(choice, CompletionChoice) else choice.message.content
         return TextContent(
             inner_content=response,
@@ -72,15 +73,15 @@
             metadata=choice_metadata,
         )
 
     async def get_streaming_text_contents(
         self,
         prompt: str,
         settings: "OpenAIPromptExecutionSettings",
-    ) -> AsyncGenerator[List["StreamingTextContent"], Any]:
+    ) -> AsyncGenerator[list["StreamingTextContent"], Any]:
         """
         Executes a completion request and streams the result.
         Supports both chat completion and text completion.
 
         Arguments:
             prompt {str} -- The prompt to use for the completion request.
             settings {OpenAITextPromptExecutionSettings} -- The settings to use for the completion request.
@@ -104,43 +105,43 @@
         async for chunk in response:
             if len(chunk.choices) == 0:
                 continue
             chunk_metadata = self._get_metadata_from_text_response(chunk)
             yield [self._create_streaming_text_content(chunk, choice, chunk_metadata) for choice in chunk.choices]
 
     def _create_streaming_text_content(
-        self, chunk: Completion, choice: Union[CompletionChoice, ChatCompletionChunk], response_metadata: Dict[str, Any]
+        self, chunk: Completion, choice: CompletionChoice | ChatCompletionChunk, response_metadata: dict[str, Any]
     ) -> "StreamingTextContent":
         """Create a streaming text content object from a choice."""
         choice_metadata = self._get_metadata_from_text_choice(choice)
         choice_metadata.update(response_metadata)
         text = choice.text if isinstance(choice, CompletionChoice) else choice.delta.content
         return StreamingTextContent(
             choice_index=choice.index,
             inner_content=chunk,
             ai_model_id=self.ai_model_id,
             metadata=choice_metadata,
             text=text,
         )
 
-    def _get_metadata_from_text_response(self, response: Completion) -> Dict[str, Any]:
+    def _get_metadata_from_text_response(self, response: Completion) -> dict[str, Any]:
         """Get metadata from a completion response."""
         return {
             "id": response.id,
             "created": response.created,
             "system_fingerprint": response.system_fingerprint,
             "usage": response.usage,
         }
 
-    def _get_metadata_from_streaming_text_response(self, response: Completion) -> Dict[str, Any]:
+    def _get_metadata_from_streaming_text_response(self, response: Completion) -> dict[str, Any]:
         """Get metadata from a streaming completion response."""
         return {
             "id": response.id,
             "created": response.created,
             "system_fingerprint": response.system_fingerprint,
         }
 
-    def _get_metadata_from_text_choice(self, choice: CompletionChoice) -> Dict[str, Any]:
+    def _get_metadata_from_text_choice(self, choice: CompletionChoice) -> dict[str, Any]:
         """Get metadata from a completion choice."""
         return {
             "logprobs": getattr(choice, "logprobs", None),
         }
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Dict, Mapping, Optional
+from collections.abc import Mapping
 
 from openai import AsyncOpenAI
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_config_base import (
     OpenAIConfigBase,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import (
     OpenAIModelTypes,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_text_embedding_base import (
     OpenAITextEmbeddingBase,
 )
 from semantic_kernel.connectors.ai.open_ai.settings.open_ai_settings import OpenAISettings
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class OpenAITextEmbedding(OpenAIConfigBase, OpenAITextEmbeddingBase):
     """OpenAI Text Embedding class."""
 
     def __init__(
         self,
         ai_model_id: str,
         api_key: str | None = None,
         org_id: str | None = None,
-        service_id: Optional[str] = None,
-        default_headers: Optional[Mapping[str, str]] = None,
-        async_client: Optional[AsyncOpenAI] = None,
+        service_id: str | None = None,
+        default_headers: Mapping[str, str] | None = None,
+        async_client: AsyncOpenAI | None = None,
         env_file_path: str | None = None,
     ) -> None:
         """
         Initializes a new instance of the OpenAITextCompletion class.
 
         Arguments:
             ai_model_id {str} -- OpenAI model name, see
@@ -70,15 +72,15 @@
             org_id=org_id,
             service_id=service_id,
             default_headers=default_headers,
             async_client=async_client,
         )
 
     @classmethod
-    def from_dict(cls, settings: Dict[str, str]) -> "OpenAITextEmbedding":
+    def from_dict(cls, settings: dict[str, str]) -> "OpenAITextEmbedding":
         """
         Initialize an Open AI service from a dictionary of settings.
 
         Arguments:
             settings: A dictionary of settings for the service.
         """
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Any, List, Optional
+from typing import Any
 
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIEmbeddingPromptExecutionSettings,
 )
 from semantic_kernel.connectors.ai.open_ai.services.open_ai_handler import OpenAIHandler
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class OpenAITextEmbeddingBase(OpenAIHandler, EmbeddingGeneratorBase):
-    async def generate_embeddings(self, texts: List[str], batch_size: Optional[int] = None, **kwargs: Any) -> ndarray:
+    async def generate_embeddings(self, texts: list[str], batch_size: int | None = None, **kwargs: Any) -> ndarray:
         """Generates embeddings for the given texts.
 
         Arguments:
             texts {List[str]} -- The texts to generate embeddings for.
             batch_size {Optional[int]} -- The batch size to use for the request.
             kwargs {Dict[str, Any]} -- Additional arguments to pass to the request,
                 see OpenAIEmbeddingPromptExecutionSettings for the details.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/services/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/services/utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,24 +9,14 @@
     from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
         OpenAIChatPromptExecutionSettings,
     )
 
 logger = logging.getLogger(__name__)
 
 
-TYPE_MAPPER = {
-    "str": "string",
-    "int": "number",
-    "float": "number",
-    "bool": "boolean",
-    "list": "array",
-    "dict": "object",
-}
-
-
 def update_settings_from_function_call_configuration(
     function_call_configuration: "FunctionCallConfiguration", settings: "OpenAIChatPromptExecutionSettings"
 ) -> None:
     """Update the settings from a FunctionCallConfiguration."""
     if function_call_configuration.required_functions:
         if len(function_call_configuration.required_functions) > 1:
             logger.warning("Multiple required functions are not supported. Using the first required function.")
@@ -40,35 +30,35 @@
         settings.tools = [
             kernel_function_metadata_to_openai_tool_format(f) for f in function_call_configuration.available_functions
         ]
 
 
 def kernel_function_metadata_to_openai_tool_format(metadata: KernelFunctionMetadata) -> dict[str, Any]:
     """Convert the kernel function metadata to OpenAI format."""
+
+    def parse_schema(schema_data):
+        """Recursively parse the schema data to include nested properties."""
+        if schema_data.get("type") == "object":
+            return {
+                "type": "object",
+                "properties": {key: parse_schema(value) for key, value in schema_data.get("properties", {}).items()},
+                "description": schema_data.get("description", ""),
+            }
+        else:
+            return {
+                "type": schema_data.get("type", "string"),
+                "description": schema_data.get("description", ""),
+                **({"enum": schema_data.get("enum")} if "enum" in schema_data else {}),
+            }
+
     return {
         "type": "function",
         "function": {
             "name": metadata.fully_qualified_name,
             "description": metadata.description or "",
             "parameters": {
                 "type": "object",
-                "properties": {
-                    param.name: {
-                        "description": param.description or "",
-                        "type": parse_parameter_type(param.type_),
-                        **({"enum": param.enum} if hasattr(param, "enum") else {}),  # Added support for enum
-                    }
-                    for param in metadata.parameters
-                },
+                "properties": {param.name: parse_schema(param.schema_data) for param in metadata.parameters},
                 "required": [p.name for p in metadata.parameters if p.is_required],
             },
         },
     }
-
-
-def parse_parameter_type(param_type: str | None) -> str:
-    """Parse the parameter type."""
-    if not param_type:
-        return "string"
-    if "," in param_type:
-        param_type = param_type.split(",", maxsplit=1)[0]
-    return TYPE_MAPPER.get(param_type, "string")
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/azure_open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/open_ai/settings/open_ai_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/prompt_execution_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/prompt_execution_settings.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
@@ -52,24 +51,24 @@
                 "service_id",
                 "extension_data",
             },
             exclude_none=True,
             by_alias=True,
         )
 
-    def update_from_prompt_execution_settings(self, config: PromptExecutionSettings) -> None:
+    def update_from_prompt_execution_settings(self, config: "PromptExecutionSettings") -> None:
         """Update the prompt execution settings from a completion config."""
         if config.service_id is not None:
             self.service_id = config.service_id
         config.pack_extension_data()
         self.extension_data.update(config.extension_data)
         self.unpack_extension_data()
 
     @classmethod
-    def from_prompt_execution_settings(cls, config: PromptExecutionSettings) -> PromptExecutionSettings:
+    def from_prompt_execution_settings(cls, config: "PromptExecutionSettings") -> "PromptExecutionSettings":
         """Create a prompt execution settings from a completion config."""
         config.pack_extension_data()
         return cls(
             service_id=config.service_id,
             extension_data=config.extension_data,
         )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from typing import TYPE_CHECKING, Any, AsyncGenerator
+from collections.abc import AsyncGenerator
+from typing import TYPE_CHECKING, Any
 
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
     from semantic_kernel.contents import StreamingTextContent, TextContent
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astra_client.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astra_client.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 import json
-from typing import Dict, List, Optional
 
 import aiohttp
 
 from semantic_kernel.connectors.memory.astradb.utils import AsyncSession
 from semantic_kernel.connectors.telemetry import APP_INFO
 from semantic_kernel.exceptions import ServiceResponseException
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 ASTRA_CALLER_IDENTITY: str
 SEMANTIC_KERNEL_VERSION = APP_INFO.get("Semantic-Kernel-Version")
 if SEMANTIC_KERNEL_VERSION:
     ASTRA_CALLER_IDENTITY = f"semantic-kernel/{SEMANTIC_KERNEL_VERSION}"
 else:
     ASTRA_CALLER_IDENTITY = "semantic-kernel"
 
 
+@experimental_class
 class AstraClient:
     def __init__(
         self,
         astra_id: str,
         astra_region: str,
         astra_application_token: str,
         keyspace_name: str,
         embedding_dim: int,
         similarity_function: str,
-        session: Optional[aiohttp.ClientSession] = None,
+        session: aiohttp.ClientSession | None = None,
     ):
         self.astra_id = astra_id
         self.astra_application_token = astra_application_token
         self.astra_region = astra_region
         self.keyspace_name = keyspace_name
         self.embedding_dim = embedding_dim
         self.similarity_function = similarity_function
@@ -39,15 +40,15 @@
         self.request_header = {
             "x-cassandra-token": self.astra_application_token,
             "Content-Type": "application/json",
             "User-Agent": ASTRA_CALLER_IDENTITY,
         }
         self._session = session
 
-    async def _run_query(self, request_url: str, query: Dict):
+    async def _run_query(self, request_url: str, query: dict):
         async with AsyncSession(self._session) as session:
             async with session.post(request_url, data=json.dumps(query), headers=self.request_header) as response:
                 if response.status == 200:
                     response_dict = await response.json()
                     if "errors" in response_dict:
                         raise ServiceResponseException(f"Astra DB request error - {response_dict['errors']}")
                     else:
@@ -68,16 +69,16 @@
                 found = True
                 break
         return found
 
     async def create_collection(
         self,
         collection_name: str,
-        embedding_dim: Optional[int] = None,
-        similarity_function: Optional[str] = None,
+        embedding_dim: int | None = None,
+        similarity_function: str | None = None,
     ):
         query = {
             "createCollection": {
                 "name": collection_name,
                 "options": {
                     "vector": {
                         "dimension": embedding_dim if embedding_dim is not None else self.embedding_dim,
@@ -96,20 +97,20 @@
 
     def _build_request_collection_url(self, collection_name: str):
         return f"{self.request_base_url}/{collection_name}"
 
     async def find_documents(
         self,
         collection_name: str,
-        filter: Optional[Dict] = None,
-        vector: Optional[List[float]] = None,
-        limit: Optional[int] = None,
-        include_vector: Optional[bool] = None,
-        include_similarity: Optional[bool] = None,
-    ) -> List[Dict]:
+        filter: dict | None = None,
+        vector: list[float] | None = None,
+        limit: int | None = None,
+        include_vector: bool | None = None,
+        include_similarity: bool | None = None,
+    ) -> list[dict]:
         find_query = {}
 
         if filter is not None:
             find_query["filter"] = filter
 
         if vector is not None:
             find_query["sort"] = {"$vector": vector}
@@ -126,42 +127,42 @@
             else:
                 find_query["options"] = {"includeSimilarity": int(include_similarity)}
 
         query = {"find": find_query}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["data"]["documents"]
 
-    async def insert_document(self, collection_name: str, document: Dict) -> str:
+    async def insert_document(self, collection_name: str, document: dict) -> str:
         query = {"insertOne": {"document": document}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["insertedIds"][0]
 
-    async def insert_documents(self, collection_name: str, documents: List[Dict]) -> List[str]:
+    async def insert_documents(self, collection_name: str, documents: list[dict]) -> list[str]:
         query = {"insertMany": {"documents": documents}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["insertedIds"]
 
-    async def update_document(self, collection_name: str, filter: Dict, update: Dict, upsert: bool = True) -> Dict:
+    async def update_document(self, collection_name: str, filter: dict, update: dict, upsert: bool = True) -> dict:
         query = {
             "findOneAndUpdate": {
                 "filter": filter,
                 "update": update,
                 "options": {"returnDocument": "after", "upsert": upsert},
             }
         }
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]
 
-    async def update_documents(self, collection_name: str, filter: Dict, update: Dict):
+    async def update_documents(self, collection_name: str, filter: dict, update: dict):
         query = {
             "updateMany": {
                 "filter": filter,
                 "update": update,
             }
         }
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]
 
-    async def delete_documents(self, collection_name: str, filter: Dict) -> int:
+    async def delete_documents(self, collection_name: str, filter: dict) -> int:
         query = {"deleteMany": {"filter": filter}}
         result = await self._run_query(self._build_request_collection_url(collection_name), query)
         return result["status"]["deletedCount"]
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_memory_store.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
-from typing import List, Optional, Tuple
 
 import aiohttp
 from numpy import ndarray
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.astradb.astra_client import AstraClient
 from semantic_kernel.connectors.memory.astradb.astradb_settings import AstraDBSettings
 from semantic_kernel.connectors.memory.astradb.utils import (
     build_payload,
     parse_payload,
 )
 from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class AstraDBMemoryStore(MemoryStoreBase):
     """A memory store that uses Astra database as the backend."""
 
     def __init__(
         self,
         astra_application_token: str,
         astra_id: str,
@@ -93,27 +94,27 @@
             astra_application_token=astra_application_token,
             keyspace_name=keyspace_name,
             embedding_dim=embedding_dim,
             similarity_function=similarity,
             session=self._session,
         )
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         return await self._client.find_collections(False)
 
     async def create_collection(
         self,
         collection_name: str,
-        dimension_num: Optional[int] = None,
-        distance_type: Optional[str] = "cosine",
+        dimension_num: int | None = None,
+        distance_type: str | None = "cosine",
     ) -> None:
         """Creates a new collection in Astra if it does not exist.
 
         Arguments:
             collection_name {str} -- The name of the collection to create.
             dimension_num {int} -- The dimension of the vectors to be stored in this collection.
             distance_type {str} -- Specifies the similarity metric to be used when querying or comparing vectors within
@@ -173,15 +174,15 @@
         """
         filter = {"_id": record._id}
         update = {"$set": build_payload(record)}
         status = await self._client.update_document(collection_name, filter, update, True)
 
         return status["upsertedId"] if "upsertedId" in status else record._id
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of memory records into the data store. Does not guarantee that the collection exists.
             If the record already exists, it will be updated.
             If the record does not exist, it will be created.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             records {List[MemoryRecord]} -- The memory records to upsert.
@@ -211,16 +212,16 @@
 
         if len(documents) == 0:
             raise KeyError(f"Record with key '{key}' does not exist")
 
         return parse_payload(documents[0])
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """Gets a batch of records. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -245,15 +246,15 @@
 
         Returns:
             None
         """
         filter = {"_id": key}
         await self._client.delete_documents(collection_name, filter)
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique ids associated with the memory records to remove.
 
         Returns:
@@ -264,15 +265,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -291,15 +292,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/astradb_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/astradb_settings.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class AstraDBSettings(BaseModelSettings):
     """AstraDB model settings
 
     Optional:
     - app_token: SecretStr | None - AstraDB token
         (Env var ASTRADB_APP_TOKEN)
     - db_id: str | None - AstraDB database ID
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/astradb/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/astradb/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
-from typing import Any, Dict
+from typing import Any
 
 import aiohttp
 import numpy
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 
@@ -14,30 +14,30 @@
     async def __aenter__(self):
         return await self._session.__aenter__()
 
     async def __aexit__(self, *args, **kwargs):
         await self._session.close()
 
 
-def build_payload(record: MemoryRecord) -> Dict[str, Any]:
+def build_payload(record: MemoryRecord) -> dict[str, Any]:
     """
     Builds a metadata payload to be sent to AstraDb from a MemoryRecord.
     """
-    payload: Dict[str, Any] = {}
+    payload: dict[str, Any] = {}
     payload["$vector"] = record.embedding.tolist()
     if record._text:
         payload["text"] = record._text
     if record._description:
         payload["description"] = record._description
     if record._additional_metadata:
         payload["additional_metadata"] = record._additional_metadata
     return payload
 
 
-def parse_payload(document: Dict[str, Any]) -> MemoryRecord:
+def parse_payload(document: dict[str, Any]) -> MemoryRecord:
     """
     Parses a record from AstraDb into a MemoryRecord.
     """
     text = document.get("text", None)
     description = document["description"] if "description" in document else None
     additional_metadata = document["additional_metadata"] if "additional_metadata" in document else None
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_ai_search_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class AzureAISearchSettings(BaseModelSettings):
     """Azure AI Search model settings currently used by the AzureCognitiveSearchMemoryStore connector
 
     Optional:
     - api_key: SecretStr - Azure AI Search API key (Env var AZURE_AI_SEARCH_API_KEY)
     - endpoint: HttpsUrl - Azure AI Search endpoint (Env var AZURE_AI_SEARCH_ENDPOINT)
     - index_name: str - Azure AI Search index name (Env var AZURE_AI_SEARCH_INDEX_NAME)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import uuid
 from inspect import isawaitable
-from typing import List, Optional, Tuple
 
 from azure.core.credentials import AzureKeyCredential, TokenCredential
 from azure.core.exceptions import ResourceNotFoundError
 from azure.search.documents.indexes.aio import SearchIndexClient
 from azure.search.documents.indexes.models import (
     HnswAlgorithmConfiguration,
     HnswParameters,
@@ -29,18 +28,20 @@
     get_index_schema,
     get_search_index_async_client,
     memory_record_to_search_record,
 )
 from semantic_kernel.exceptions import MemoryConnectorInitializationError, MemoryConnectorResourceNotFound
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class AzureCognitiveSearchMemoryStore(MemoryStoreBase):
     _search_index_client: SearchIndexClient = None
     _vector_size: int = None
 
     def __init__(
         self,
         vector_size: int,
@@ -95,16 +96,16 @@
         """Async close connection, invoked by MemoryStoreBase.__aexit__()"""
         if self._search_index_client is not None:
             await self._search_index_client.close()
 
     async def create_collection(
         self,
         collection_name: str,
-        vector_config: Optional[HnswAlgorithmConfiguration] = None,
-        search_resource_encryption_key: Optional[SearchResourceEncryptionKey] = None,
+        vector_config: HnswAlgorithmConfiguration | None = None,
+        search_resource_encryption_key: SearchResourceEncryptionKey | None = None,
     ) -> None:
         """Creates a new collection if it does not exist.
 
         Arguments:
             collection_name {str}                              -- The name of the collection to create.
             vector_config {HnswVectorSearchAlgorithmConfiguration} -- Optional search algorithm configuration
                                                                       (default: {None}).
@@ -160,15 +161,15 @@
                 fields=get_index_schema(self._vector_size, vector_search_profile_name),
                 vector_search=vector_search,
                 encryption_key=search_resource_encryption_key,
             )
 
             await self._search_index_client.create_index(index)
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
 
         results_list = []
@@ -224,15 +225,15 @@
         """
 
         result = await self.upsert_batch(collection_name, [record])
         if result:
             return result[0]
         return None
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upsert a batch of records.
 
         Arguments:
             collection_name {str}        -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
@@ -290,16 +291,16 @@
 
         await search_client.close()
 
         # Create Memory record from document
         return dict_to_memory_record(search_result, with_embedding)
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str}  -- The name of the collection to get the records from.
             keys {List[str]}       -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -315,15 +316,15 @@
                 key=key,
                 with_embedding=with_embeddings,
             )
             search_results.append(search_result)
 
         return search_results
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]}      -- The unique database keys of the records to remove.
 
         Returns:
@@ -353,15 +354,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using vector configuration parameters.
 
         Arguments:
             collection_name {str}       -- The name of the collection to get the nearest match from.
             embedding {ndarray}         -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool}       -- Whether to include the embedding in the result. (default: {False})
@@ -386,15 +387,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using vector configuration.
 
         Parameters:
             collection_name (str)       -- The name of the collection to get the nearest matches from.
             embedding (ndarray)         -- The embedding to find the nearest matches to.
             limit {int}                 -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import base64
 import os
-from typing import List, Optional
 
 from azure.core.credentials import AzureKeyCredential, TokenCredential
 from azure.search.documents.indexes.aio import SearchIndexClient
 from azure.search.documents.indexes.models import SearchableField, SearchField, SearchFieldDataType, SimpleField
 from dotenv import load_dotenv
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
@@ -19,18 +18,18 @@
 SEARCH_FIELD_SRC = "ExternalSourceName"
 SEARCH_FIELD_DESC = "Description"
 SEARCH_FIELD_METADATA = "AdditionalMetadata"
 SEARCH_FIELD_IS_REF = "IsReference"
 
 
 def get_search_index_async_client(
-    search_endpoint: Optional[str] = None,
-    admin_key: Optional[str] = None,
-    azure_credential: Optional[AzureKeyCredential] = None,
-    token_credential: Optional[TokenCredential] = None,
+    search_endpoint: str | None = None,
+    admin_key: str | None = None,
+    azure_credential: AzureKeyCredential | None = None,
+    token_credential: TokenCredential | None = None,
 ):
     """Return a client for Azure Cognitive Search.
 
     Arguments:
         search_endpoint {str}                 -- Optional endpoint (default: {None}).
         admin_key {str}                       -- Optional API key (default: {None}).
         azure_credential {AzureKeyCredential} -- Optional Azure credentials (default: {None}).
@@ -143,15 +142,15 @@
             retrievable=True,
         ),
     ]
 
     return search_fields
 
 
-def get_field_selection(with_embeddings: bool) -> List[str]:
+def get_field_selection(with_embeddings: bool) -> list[str]:
     """Get the list of fields to search and load.
 
     Arguments:
         with_embedding {bool} -- Whether to include the embedding vector field.
 
     Returns:
         List[str] -- List of fields.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_memory_store.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, Tuple
 
 from numpy import ndarray
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import AzureCosmosDBStoreApi
 from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmosdb_settings import AzureCosmosDBSettings
 from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
@@ -13,18 +12,20 @@
     CosmosDBVectorSearchType,
     get_mongodb_search_client,
 )
 from semantic_kernel.connectors.memory.azure_cosmosdb.mongo_vcore_store_api import MongoStoreApi
 from semantic_kernel.exceptions import MemoryConnectorInitializationError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class AzureCosmosDBMemoryStore(MemoryStoreBase):
     """A memory store that uses AzureCosmosDB for MongoDB vCore, to perform vector similarity search on a fully
     managed MongoDB compatible database service.
     https://learn.microsoft.com/en-us/azure/cosmos-db/mongodb/vcore/vector-search"""
 
     # Right now this only supports Mongo, but set up to support more later.
     apiStore: AzureCosmosDBStoreApi = None
@@ -144,15 +145,15 @@
             collection_name {str} -- The name associated with a collection of embeddings.
 
         Returns:
             None
         """
         return await self.cosmosStore.create_collection(collection_name)
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         return await self.cosmosStore.get_collections()
 
@@ -161,135 +162,135 @@
 
         Arguments:
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
-        return await self.cosmosStore.delete_collection(str())
+        return await self.cosmosStore.delete_collection("")
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
         Returns:
             bool -- True if the collection exists; otherwise, False.
         """
-        return await self.cosmosStore.does_collection_exist(str())
+        return await self.cosmosStore.does_collection_exist("")
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         """Upsert a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the record into.
             record {MemoryRecord} -- The record to upsert.
 
         Returns:
             str -- The unique record id of the record.
         """
-        return await self.cosmosStore.upsert(str(), record)
+        return await self.cosmosStore.upsert("", record)
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upsert a batch of records.
 
         Arguments:
             collection_name {str}        -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
             List[str] -- The unique database keys of the records.
         """
-        return await self.cosmosStore.upsert_batch(str(), records)
+        return await self.cosmosStore.upsert_batch("", records)
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         """Gets a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the record from.
             key {str}             -- The unique database key of the record.
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             MemoryRecord -- The record.
         """
-        return await self.cosmosStore.get(str(), key, with_embedding)
+        return await self.cosmosStore.get("", key, with_embedding)
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str}  -- The name of the collection to get the records from.
             keys {List[str]}       -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[MemoryRecord] -- The records.
         """
-        return await self.cosmosStore.get_batch(str(), keys, with_embeddings)
+        return await self.cosmosStore.get_batch("", keys, with_embeddings)
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Removes a record.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the record from.
             key {str}             -- The unique database key of the record to remove.
 
         Returns:
             None
         """
-        return await self.cosmosStore.remove(str(), key)
+        return await self.cosmosStore.remove("", key)
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]}      -- The unique database keys of the records to remove.
 
         Returns:
             None
         """
-        return await self.cosmosStore.remove_batch(str(), keys)
+        return await self.cosmosStore.remove_batch("", keys)
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using vector configuration.
 
         Parameters:
             collection_name (str)       -- The name of the collection to get the nearest matches from.
             embedding (ndarray)         -- The embedding to find the nearest matches to.
             limit {int}                 -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
             with_embeddings {bool}      -- Whether to include the embeddings in the results. (default: {False})
 
         Returns:
             List[Tuple[MemoryRecord, float]] -- The records and their relevance scores.
         """
-        return await self.cosmosStore.get_nearest_matches(str(), embedding, limit, min_relevance_score, with_embeddings)
+        return await self.cosmosStore.get_nearest_matches("", embedding, limit, min_relevance_score, with_embeddings)
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using vector configuration parameters.
 
         Arguments:
             collection_name {str}       -- The name of the collection to get the nearest match from.
             embedding {ndarray}         -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool}       -- Whether to include the embedding in the result. (default: {False})
 
         Returns:
             Tuple[MemoryRecord, float] -- The record and the relevance score.
         """
-        return await self.cosmosStore.get_nearest_match(str(), embedding, min_relevance_score, with_embedding)
+        return await self.cosmosStore.get_nearest_match("", embedding, min_relevance_score, with_embedding)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmos_db_store_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 
 from abc import ABC, abstractmethod
-from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
 # Abstract class similar to the original data store that allows API level abstraction
+@experimental_class
 class AzureCosmosDBStoreApi(ABC):
     @abstractmethod
     async def create_collection(self, collection_name: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         raise NotImplementedError
 
     @abstractmethod
     async def delete_collection(self, collection_name: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
@@ -28,46 +29,46 @@
         raise NotImplementedError
 
     @abstractmethod
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         raise NotImplementedError
 
     @abstractmethod
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         raise NotImplementedError
 
     @abstractmethod
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         raise NotImplementedError
 
     @abstractmethod
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         raise NotImplementedError
 
     @abstractmethod
     async def remove(self, collection_name: str, key: str) -> None:
         raise NotImplementedError
 
     @abstractmethod
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         raise NotImplementedError
 
     @abstractmethod
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         raise NotImplementedError
 
     @abstractmethod
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         raise NotImplementedError
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-class AzureCosmosDBSettings(BaseModelSettings):
-    """Azure CosmosDB model settings
+@experimental_class
+class RedisSettings(BaseModelSettings):
+    """Redis model settings
 
     Optional:
-    - connection_string: str - Azure CosmosDB connection string
-        (Env var COSMOSDB_CONNECTION_STRING)
+    - connection_string: str | None - Redis connection string
+        (Env var REDIS_CONNECTION_STRING)
     """
 
-    api: str | None = None
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
-        env_prefix = "COSMOSDB_"
+        env_prefix = "REDIS_"
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/cosmosdb_utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,36 +3,40 @@
 from enum import Enum
 
 from dotenv import load_dotenv
 from pymongo import MongoClient
 
 from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 from semantic_kernel.exceptions import ServiceInitializationError
+from semantic_kernel.utils.experimental_decorator import experimental_function
 
 
+@experimental_function
 class CosmosDBSimilarityType(str, Enum):
     """Cosmos DB Similarity Type as enumerator."""
 
     COS = "COS"
     """CosineSimilarity"""
     IP = "IP"
     """inner - product"""
     L2 = "L2"
     """Euclidean distance"""
 
 
+@experimental_function
 class CosmosDBVectorSearchType(str, Enum):
     """Cosmos DB Vector Search Type as enumerator."""
 
     VECTOR_IVF = "vector-ivf"
     """IVF vector index"""
     VECTOR_HNSW = "vector-hnsw"
     """HNSW vector index"""
 
 
+@experimental_function
 def get_mongodb_search_client(connection_string: str, application_name: str):
     """
     Returns a client for Azure Cosmos Mongo vCore Vector DB
 
     Arguments:
         connection_string {str}
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/mongo_vcore_store_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
-from typing import Any, Dict, List, Tuple
+from typing import Any
 
 import numpy as np
 
 from semantic_kernel.connectors.memory.azure_cosmosdb.azure_cosmos_db_store_api import (
     AzureCosmosDBStoreApi,
 )
 from semantic_kernel.connectors.memory.azure_cosmosdb.cosmosdb_utils import (
     CosmosDBSimilarityType,
     CosmosDBVectorSearchType,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class MongoStoreApi(AzureCosmosDBStoreApi):
     database = None
     collection_name: str
     index_name = None
     vector_dimensions = None
     num_lists = None
     similarity = None
@@ -111,15 +113,15 @@
                     )
                 # invoke the command from the database object
                 self.database.command(create_index_commands)
         self.collection = self.database[collection_name]
 
     def _get_vector_index_ivf(
         self, collection_name: str, kind: str, num_lists: int, similarity: str, dimensions: int
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         command = {
             "createIndexes": collection_name,
             "indexes": [
                 {
                     "name": self.index_name,
                     "key": {"embedding": "cosmosSearch"},
                     "cosmosSearchOptions": {
@@ -131,15 +133,15 @@
                 }
             ],
         }
         return command
 
     def _get_vector_index_hnsw(
         self, collection_name: str, kind: str, m: int, ef_construction: int, similarity: str, dimensions: int
-    ) -> Dict[str, Any]:
+    ) -> dict[str, Any]:
         command = {
             "createIndexes": collection_name,
             "indexes": [
                 {
                     "name": self.index_name,
                     "key": {"embedding": "cosmosSearch"},
                     "cosmosSearchOptions": {
@@ -150,30 +152,30 @@
                         "dimensions": dimensions,
                     },
                 }
             ],
         }
         return command
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         return self.database.list_collection_names()
 
     async def delete_collection(self, collection_name: str) -> None:
         return self.collection.drop()
 
     async def does_collection_exist(self, collection_name: str) -> bool:
         return collection_name in self.database.list_collection_names()
 
     async def upsert(self, collection_name: str, record: MemoryRecord) -> str:
         result = await self.upsert_batch(collection_name, [record])
         return result[0]
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
-        doc_ids: List[str] = []
-        cosmosRecords: List[dict] = []
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
+        doc_ids: list[str] = []
+        cosmosRecords: list[dict] = []
         for record in records:
             cosmosRecord: dict = {
                 "_id": record.id,
                 "embedding": record.embedding.tolist(),
                 "text": record.text,
                 "description": record.description,
                 "metadata": self.__serialize_metadata(record),
@@ -196,15 +198,15 @@
             embedding=np.array(result["embedding"]) if with_embedding else np.array([]),
             text=result["text"],
             description=result["description"],
             additional_metadata=result["metadata"],
             timestamp=result.get("timestamp", None),
         )
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         if not with_embeddings:
             results = self.collection.find({"_id": {"$in": keys}}, {"embedding": 0})
         else:
             results = self.collection.find({"_id": {"$in": keys}})
 
         return [
             MemoryRecord.local_record(
@@ -217,26 +219,26 @@
             )
             for result in results
         ]
 
     async def remove(self, collection_name: str, key: str) -> None:
         self.collection.delete_one({"_id": key})
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         self.collection.delete_many({"_id": {"$in": keys}})
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: np.ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
-    ) -> List[Tuple[MemoryRecord, float]]:
-        pipeline: List[dict[str, Any]] = []
+    ) -> list[tuple[MemoryRecord, float]]:
+        pipeline: list[dict[str, Any]] = []
         if self.kind == CosmosDBVectorSearchType.VECTOR_IVF:
             pipeline = self._get_pipeline_vector_ivf(embedding.tolist(), limit)
         elif self.kind == CosmosDBVectorSearchType.VECTOR_HNSW:
             pipeline = self._get_pipeline_vector_hnsw(embedding.tolist(), limit, self.ef_search)
 
         cursor = self.collection.aggregate(pipeline)
 
@@ -253,16 +255,16 @@
                 description=aggResult["document"]["description"],
                 additional_metadata=aggResult["document"]["metadata"],
                 timestamp=aggResult["document"].get("timestamp", None),
             )
             nearest_results.append((result, aggResult["similarityScore"]))
         return nearest_results
 
-    def _get_pipeline_vector_ivf(self, embeddings: List[float], k: int = 4) -> List[dict[str, Any]]:
-        pipeline: List[dict[str, Any]] = [
+    def _get_pipeline_vector_ivf(self, embeddings: list[float], k: int = 4) -> list[dict[str, Any]]:
+        pipeline: list[dict[str, Any]] = [
             {
                 "$search": {
                     "cosmosSearch": {
                         "vector": embeddings,
                         "path": "embedding",
                         "k": k,
                     },
@@ -275,17 +277,17 @@
                     "document": "$$ROOT",
                 }
             },
         ]
         return pipeline
 
     def _get_pipeline_vector_hnsw(
-        self, embeddings: List[float], k: int = 4, ef_search: int = 40
-    ) -> List[dict[str, Any]]:
-        pipeline: List[dict[str, Any]] = [
+        self, embeddings: list[float], k: int = 4, ef_search: int = 40
+    ) -> list[dict[str, Any]]:
+        pipeline: list[dict[str, Any]] = [
             {
                 "$search": {
                     "cosmosSearch": {
                         "vector": embeddings,
                         "path": "embedding",
                         "k": k,
                         "efSearch": ef_search,
@@ -303,15 +305,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: np.ndarray,
         min_relevance_score: float,
         with_embedding: bool,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         nearest_results = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
             limit=1,
         )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, List, Optional, Tuple
+from typing import TYPE_CHECKING, Optional
 
 from numpy import array, ndarray
 
 from semantic_kernel.connectors.memory.chroma.utils import chroma_compute_similarity_scores, query_results_to_records
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 if TYPE_CHECKING:
     import chromadb
     import chromadb.config
     from chromadb.api.models.Collection import Collection
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class ChromaMemoryStore(MemoryStoreBase):
     _client: "chromadb.Client"
 
     def __init__(
         self,
-        persist_directory: Optional[str] = None,
+        persist_directory: str | None = None,
         client_settings: Optional["chromadb.config.Settings"] = None,
         **kwargs,
     ) -> None:
         """
         ChromaMemoryStore provides an interface to store and retrieve data using ChromaDB.
         Collection names with uppercase characters are not supported by ChromaDB, they will be automatically converted.
 
@@ -87,15 +89,15 @@
     async def get_collection(self, collection_name: str) -> Optional["Collection"]:
         try:
             # Current version of ChromeDB rejects camel case collection names.
             return self._client.get_collection(name=collection_name)
         except ValueError:
             return None
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         return [collection.name for collection in self._client.list_collections()]
 
@@ -153,15 +155,15 @@
             # by providing embeddings, we can skip the chroma's embedding function call
             embeddings=record.embedding.tolist(),
             documents=record._text,
             ids=record._key,
         )
         return record._key
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
@@ -185,15 +187,15 @@
         try:
             return records[0]
         except IndexError as exc:
             raise ServiceResourceNotFoundError(
                 f"Record with key '{key}' does not exist in collection '{collection_name}'"
             ) from exc
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -218,15 +220,15 @@
             key {str} -- The unique database key of the record to remove.
 
         Returns:
             None
         """
         await self.remove_batch(collection_name, [key])
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
@@ -239,15 +241,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = True,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
@@ -306,15 +308,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = True,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest match from.
             embedding {ndarray} -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING
 
 from numpy import array, linalg, ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 if TYPE_CHECKING:
     from chromadb.api.types import QueryResult
@@ -21,15 +21,15 @@
                 snake_str += "_"
             if i != len(camel_str) - 1 and camel_str[i + 1].islower():
                 snake_str += "_"
         snake_str += char.lower()
     return snake_str
 
 
-def query_results_to_records(results: "QueryResult", with_embedding: bool) -> List[MemoryRecord]:
+def query_results_to_records(results: "QueryResult", with_embedding: bool) -> list[MemoryRecord]:
     # if results has only one record, it will be a list instead of a nested list
     # this is to make sure that results is always a nested list
     # {'ids': ['test_id1'], 'embeddings': [[...]], 'documents': ['sample text1'], 'metadatas': [{...}]}
     # => {'ids': [['test_id1']], 'embeddings': [[[...]]], 'documents': [['sample text1']], 'metadatas': [[{...}]]}
     try:
         if isinstance(results["ids"][0], str):
             for k, v in results.items():
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from datetime import datetime
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Any
 
 from numpy import array, expand_dims, ndarray
 from pymilvus import Collection, CollectionSchema, DataType, FieldSchema, connections, utility
 
 from semantic_kernel.exceptions import ServiceResourceNotFoundError, ServiceResponseException
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class, experimental_function
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 # Index parameters
 _INDEX_TYPE = "IVF_FLAT"
 _NLIST = 1024
 
@@ -43,15 +44,16 @@
     SEARCH_FIELD_DESC,
     SEARCH_FIELD_METADATA,
     SEARCH_FIELD_IS_REF,
     SEARCH_FIELD_TIMESTAMP,
 ]
 
 
-def memoryrecord_to_milvus_dict(mem: MemoryRecord) -> Dict[str, Any]:
+@experimental_function
+def memoryrecord_to_milvus_dict(mem: MemoryRecord) -> dict[str, Any]:
     """Convert a memoryrecord into a dict.
     Args:
         mem (MemoryRecord): MemoryRecord to convert.
 
     Returns:
         dict: Dict result.
     """
@@ -62,15 +64,16 @@
             # Remove underscore
             if isinstance(val, datetime):
                 val = val.isoformat()
             ret_dict[key[1:]] = val
     return ret_dict
 
 
-def milvus_dict_to_memoryrecord(milvus_dict: Dict[str, Any]) -> MemoryRecord:
+@experimental_function
+def milvus_dict_to_memoryrecord(milvus_dict: dict[str, Any]) -> MemoryRecord:
     """Convert Milvus search result dict into MemoryRecord.
 
     Args:
         milvus_dict (dict): Search hit
 
     Returns:
         MemoryRecord
@@ -88,15 +91,16 @@
         additional_metadata=milvus_dict.get(SEARCH_FIELD_METADATA, None),
         embedding=embedding,
         key=milvus_dict.get("key", None),
         timestamp=milvus_dict.get(SEARCH_FIELD_TIMESTAMP, None),
     )
 
 
-def create_fields(dimensions: int) -> List[FieldSchema]:
+@experimental_function
+def create_fields(dimensions: int) -> list[FieldSchema]:
     return [
         FieldSchema(
             name=SEARCH_FIELD_ID,
             dtype=DataType.VARCHAR,
             is_primary=True,
             auto_id=False,
             max_length=100,
@@ -134,19 +138,20 @@
             name=SEARCH_FIELD_TIMESTAMP,
             dtype=DataType.VARCHAR,
             max_length=100,
         ),
     ]
 
 
+@experimental_class
 class MilvusMemoryStore(MemoryStoreBase):
     def __init__(
         self,
         uri: str = "http://localhost:19530",
-        token: Optional[str] = None,
+        token: str | None = None,
         **kwargs,
     ) -> None:
         """MilvusMemoryStore allows for searching for records using Milvus/Zilliz Cloud.
 
         For more details on how to get the service started, take a look here:
             Milvus: https://milvus.io/docs/get_started.md
             Zilliz Cloud: https://docs.zilliz.com/docs/quick-start
@@ -155,21 +160,21 @@
         Args:
             uri (str, optional): The uri of the cluster. Defaults to
                 "http://localhost:19530".
             token (Optional[str], optional): The token to connect to the cluster if
                 authentication is required. Defaults to None.
         """
         connections.connect("default", uri=uri, token=token)
-        self.collections: Dict[str, Collection] = {}
+        self.collections: dict[str, Collection] = {}
 
     async def create_collection(
         self,
         collection_name: str,
         dimension_num: int = 1536,
-        distance_type: Optional[str] = "IP",
+        distance_type: str | None = "IP",
         overwrite: bool = False,
         consistency: str = "Session",
     ) -> None:
         """Create a Milvus collection.
 
         Args:
             collection_name (str): The name of the collection.
@@ -194,23 +199,23 @@
             schema=schema,
             consistency_level=consistency,
         )
         self.collections[collection_name].create_index(SEARCH_FIELD_EMBEDDING, index_param)
 
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> list[str]:
         """Return a list of present collections.
 
         Returns:
             List[str]: List of collection names.
         """
         return utility.list_collections()
 
-    async def delete_collection(self, collection_name: Optional[str] = None, all: bool = False) -> None:
+    async def delete_collection(self, collection_name: str | None = None, all: bool = False) -> None:
         """Delete the specified collection.
 
         If all is True, all collections in the cluster will be removed.
 
         Args:
             collection_name (str, optional): The name of the collection to delete. Defaults to "".
             all (bool, optional): Whether to delete all collections. Defaults to False.
@@ -249,15 +254,15 @@
         res = await self.upsert_batch(
             collection_name=collection_name,
             records=[record],
             batch_size=0,
         )
         return res[0]
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord], batch_size=100) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord], batch_size=100) -> list[str]:
         """_summary_
 
         Args:
             collection_name (str): The collection name.
             records (List[MemoryRecord]): A list of memory records.
             batch_size (int, optional): Batch size of the insert, 0 is a batch
                 size of total size. Defaults to 100.
@@ -293,15 +298,15 @@
 
         Returns:
             MemoryRecord: The MemoryRecord for the key.
         """
         res = await self.get_batch(collection_name=collection_name, keys=[key], with_embeddings=with_embedding)
         return res[0]
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Get the MemoryRecords corresponding to the keys
 
         Args:
             collection_name (str): _description_
             keys (List[str]): _description_
             with_embeddings (bool): _description_
 
@@ -333,15 +338,15 @@
 
         Args:
             collection_name (str): Collection to remove from.
             key (str): The key to remove.
         """
         await self.remove_batch(collection_name=collection_name, keys=[key])
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Remove multiple records based on keys.
 
         Args:
             collection_name (str): Collection to remove from
             keys (List[str]): The list of keys.
 
         Raises:
@@ -369,15 +374,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Find the nearest `limit` matches for an embedding.
 
         Args:
             collection_name (str): The collection to search.
             embedding (ndarray): The embedding to search.
             limit (int): The total results to display.
             min_relevance_score (float, optional): Minimum distance to include. Defaults to None.
@@ -420,15 +425,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Find the nearest match for an embedding.
 
         Args:
             collection_name (str): The collection to search.
             embedding (ndarray): The embedding to search for.
             min_relevance_score (float, optional): T. Defaults to 0.0.
             with_embedding (bool, optional): Whether to include embedding in result. Defaults to False.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/README.md` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
+from collections.abc import Mapping
 from importlib import metadata
-from typing import Any, List, Mapping, Tuple
+from typing import Any
 
 from motor import core, motor_asyncio
 from numpy import ndarray
 from pydantic import ValidationError
 from pymongo import DeleteOne, ReadPreference, UpdateOne, results
 from pymongo.driver_info import DriverInfo
 
@@ -19,18 +19,20 @@
     NUM_CANDIDATES_SCALAR,
     document_to_memory_record,
     memory_record_to_mongo_document,
 )
 from semantic_kernel.exceptions import ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class MongoDBAtlasMemoryStore(MemoryStoreBase):
     """Memory Store for MongoDB Atlas Vector Search Connections"""
 
     __slots__ = ("_mongo_client", "__database_name")
 
     _mongo_client: motor_asyncio.AsyncIOMotorClient
     __database_name: str
@@ -98,15 +100,15 @@
             None
         """
         if not await self.does_collection_exist(collection_name):
             await self.database.create_collection(collection_name)
 
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> list[str]:
         """Gets all collection names in the data store.
 
         Returns:
             List[str] -- A group of collection names.
         """
         return await self.database.list_collection_names()
 
@@ -150,28 +152,28 @@
         update_result: results.UpdateResult = await self.database[collection_name].update_one(
             document, {"$set": document}, upsert=True
         )
 
         assert update_result.acknowledged
         return record._id
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
             If the record already exists, it will be updated.
             If the record does not exist, it will be created.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             records {MemoryRecord} -- The memory records to upsert.
 
         Returns:
             List[str] -- The unique identifiers for the memory records.
         """
 
-        upserts: List[UpdateOne] = []
+        upserts: list[UpdateOne] = []
         for record in records:
             document = memory_record_to_mongo_document(record)
             upserts.append(UpdateOne(document, {"$set": document}, upsert=True))
         bulk_update_result: results.BulkWriteResult = await self.database[collection_name].bulk_write(
             upserts, ordered=False
         )
 
@@ -195,15 +197,15 @@
         Returns:
             MemoryRecord -- The memory record if found
         """
         document = await self.database[collection_name].find_one({MONGODB_FIELD_ID: key})
 
         return document_to_memory_record(document, with_embedding) if document else None
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             keys {List[str]} -- The unique ids associated with the memory records to get.
             with_embeddings {bool} -- If true, the embedding will be returned in the memory records.
 
@@ -226,52 +228,52 @@
         Returns:
             None
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"collection {collection_name} not found")
         await self.database[collection_name].delete_one({MONGODB_FIELD_ID: key})
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             keys {List[str]} -- The unique ids associated with the memory records to remove.
 
         Returns:
             None
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"collection {collection_name} not found")
-        deletes: List[DeleteOne] = [DeleteOne({MONGODB_FIELD_ID: key}) for key in keys]
+        deletes: list[DeleteOne] = [DeleteOne({MONGODB_FIELD_ID: key}) for key in keys]
         bulk_write_result = await self.database[collection_name].bulk_write(deletes, ordered=False)
         logger.debug("%s entries deleted", bulk_write_result.deleted_count)
 
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         with_embeddings: bool,
         min_relevance_score: float | None = None,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding of type float. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             embedding {ndarray} -- The embedding to compare the collection's embeddings with.
             limit {int} -- The maximum number of similarity results to return, defaults to 1.
             min_relevance_score {float} -- The minimum relevance threshold for returned results.
             with_embeddings {bool} -- If true, the embeddings will be returned in the memory records.
         Returns:
             List[Tuple[MemoryRecord, float]] -- A list of tuples where item1 is a MemoryRecord and item2
                 is its similarity score as a float.
         """
         pipeline: list[dict[str, Any]] = []
-        vector_search_query: List[Mapping[str, Any]] = {
+        vector_search_query: list[Mapping[str, Any]] = {
             "$vectorSearch": {
                 "queryVector": embedding.tolist(),
                 "limit": limit,
                 "numCandidates": limit * NUM_CANDIDATES_SCALAR,
                 "path": MONGODB_FIELD_EMBEDDING,
                 "index": self.index_name,
             }
@@ -296,27 +298,27 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         with_embedding: bool,
         min_relevance_score: float | None = None,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding of type float. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             embedding {ndarray} -- The embedding to compare the collection's embeddings with.
             min_relevance_score {float} -- The minimum relevance threshold for returned result.
             with_embedding {bool} -- If true, the embeddings will be returned in the memory record.
 
         Returns:
             Tuple[MemoryRecord, float] -- A tuple consisting of the MemoryRecord and the similarity score as a float.
         """
-        matches: List[Tuple[MemoryRecord, float]] = await self.get_nearest_matches(
+        matches: list[tuple[MemoryRecord, float]] = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/mongodb_atlas_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/azure_cosmosdb/azure_cosmosdb_settings.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
-class MongoDBAtlasSettings(BaseModelSettings):
-    """MongoDB Atlas model settings
+@experimental_class
+class AzureCosmosDBSettings(BaseModelSettings):
+    """Azure CosmosDB model settings
 
     Optional:
-    - connection_string: str - MongoDB Atlas connection string
-        (Env var MONGODB_ATLAS_CONNECTION_STRING)
+    - connection_string: str - Azure CosmosDB connection string
+        (Env var COSMOSDB_CONNECTION_STRING)
     """
 
+    api: str | None = None
     connection_string: SecretStr | None = None
 
     class Config(BaseModelSettings.Config):
-        env_prefix = "MONGODB_ATLAS_"
+        env_prefix = "COSMOSDB_"
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/mongodb_atlas/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from numpy import array
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
 DEFAULT_DB_NAME = "default"
 DEFAULT_SEARCH_INDEX_NAME = "default"
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, NamedTuple, Optional, Tuple
+from typing import NamedTuple
 
 from numpy import ndarray
 from pinecone import FetchResponse, IndexDescription, IndexList, Pinecone, ServerlessSpec
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.pinecone.pinecone_settings import PineconeSettings
 from semantic_kernel.connectors.memory.pinecone.utils import (
@@ -16,26 +16,28 @@
     ServiceInitializationError,
     ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 # Limitations set by Pinecone at https://docs.pinecone.io/reference/known-limitations
 MAX_DIMENSIONALITY = 20000
 MAX_UPSERT_BATCH_SIZE = 100
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class PineconeMemoryStore(MemoryStoreBase):
     """A memory store that uses Pinecone as the backend."""
 
     _pinecone_api_key: str
     _default_dimensionality: int
 
     DEFAULT_INDEX_SPEC: ServerlessSpec = ServerlessSpec(
@@ -79,16 +81,16 @@
 
         self.pinecone = Pinecone(api_key=self._pinecone_api_key)
         self.collection_names_cache = set()
 
     async def create_collection(
         self,
         collection_name: str,
-        dimension_num: Optional[int] = None,
-        distance_type: Optional[str] = "cosine",
+        dimension_num: int | None = None,
+        distance_type: str | None = "cosine",
         index_spec: NamedTuple = DEFAULT_INDEX_SPEC,
     ) -> None:
         """Creates a new collection in Pinecone if it does not exist.
             This function creates an index, by default the following index
             settings are used: metric = cosine, cloud = aws, region = us-east-1.
 
         Arguments:
@@ -108,15 +110,15 @@
 
         if not await self.does_collection_exist(collection_name):
             self.pinecone.create_index(
                 name=collection_name, dimension=dimension_num, metric=distance_type, spec=index_spec
             )
             self.collection_names_cache.add(collection_name)
 
-    async def describe_collection(self, collection_name: str) -> Optional[IndexDescription]:
+    async def describe_collection(self, collection_name: str) -> IndexDescription | None:
         """Gets the description of the index.
         Arguments:
             collection_name {str} -- The name of the index to get.
         Returns:
             Optional[dict] -- The index.
         """
         if await self.does_collection_exist(collection_name):
@@ -184,15 +186,15 @@
         )
 
         if upsert_response.upserted_count is None:
             raise ServiceResponseException(f"Error upserting record: {upsert_response.message}")
 
         return record._id
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
@@ -238,16 +240,16 @@
 
         if len(fetch_response.vectors) == 0:
             raise ServiceResourceNotFoundError(f"Record with key '{key}' does not exist")
 
         return parse_payload(fetch_response.vectors[key], with_embedding)
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -272,15 +274,15 @@
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         collection = self.pinecone.Index(collection_name)
         collection.delete([key])
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
@@ -296,15 +298,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest match from.
             embedding {ndarray} -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
@@ -324,15 +326,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
@@ -382,15 +384,15 @@
                 for match in matches
             ]
             if len(matches) > 0
             else []
         )
 
     async def __get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
     ) -> "FetchResponse":
         index = self.pinecone.Index(collection_name)
         if len(keys) > MAX_FETCH_BATCH_SIZE:
             fetch_response = index.fetch(keys[0:MAX_FETCH_BATCH_SIZE])
             for i in range(MAX_FETCH_BATCH_SIZE, len(keys), MAX_FETCH_BATCH_SIZE):
                 fetch_response.vectors.update(index.fetch(keys[i : i + MAX_FETCH_BATCH_SIZE]).vectors)
         else:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import atexit
 import json
 import logging
-from typing import List, Optional, Tuple
 
 import numpy as np
 from numpy import ndarray
 from psycopg import Cursor
 from psycopg.sql import SQL, Identifier
 from psycopg_pool import ConnectionPool
 from pydantic import ValidationError
@@ -16,22 +15,24 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 # Limitation based on pgvector documentation https://github.com/pgvector/pgvector#what-if-i-want-to-index-vectors-with-more-than-2000-dimensions
 MAX_DIMENSIONALITY = 2000
 DEFAULT_SCHEMA = "public"
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class PostgresMemoryStore(MemoryStoreBase):
     """A memory store that uses Postgres with pgvector as the backend."""
 
     _connection_string: str
     _connection_pool: ConnectionPool
     _default_dimensionality: int
     _schema: str
@@ -77,15 +78,15 @@
         self._connection_pool = ConnectionPool(self._connection_string, min_size=min_pool, max_size=max_pool)
         self._schema = schema
         atexit.register(self._connection_pool.close)
 
     async def create_collection(
         self,
         collection_name: str,
-        dimension_num: Optional[int] = None,
+        dimension_num: int | None = None,
     ) -> None:
         """Creates a new collection.
 
         Arguments:
             collection_name {str} -- The name of the collection to create.\n
             dimension_num {Optional[int]} -- The dimensionality of the embeddings. (default: {None})
             Uses the default dimensionality when not provided
@@ -113,15 +114,15 @@
                         scm=Identifier(self._schema),
                         tbl=Identifier(collection_name),
                         dim=dimension_num,
                     ),
                     (),
                 )
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         with self._connection_pool.connection() as conn:
             with conn.cursor() as cur:
@@ -194,15 +195,15 @@
                     ),
                 )
                 result = cur.fetchone()
                 if result is None:
                     raise ServiceResponseException("Upsert failed")
                 return result[0]
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
@@ -287,16 +288,16 @@
                     text=result[2]["text"],
                     description=result[2]["description"],
                     additional_metadata=result[2]["additional_metadata"],
                     timestamp=result[3],
                 )
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -357,15 +358,15 @@
                         DELETE FROM {scm}.{tbl}
                         WHERE key = %s
                         """
                     ).format(scm=Identifier(self._schema), tbl=Identifier(collection_name)),
                     (key,),
                 )
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
@@ -388,15 +389,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
@@ -457,15 +458,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest match from.
             embedding {ndarray} -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
@@ -485,15 +486,15 @@
             raise ServiceResourceNotFoundError("No match found")
         return results[0]
 
     async def __does_collection_exist(self, cur: Cursor, collection_name: str) -> bool:
         results = await self.__get_collections(cur)
         return collection_name in results
 
-    async def __get_collections(self, cur: Cursor) -> List[str]:
+    async def __get_collections(self, cur: Cursor) -> list[str]:
         cur.execute(
             """
             SELECT table_name
             FROM information_schema.tables
             WHERE table_schema = %s
             """,
             (self._schema,),
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,36 +4,37 @@
 QdrantMemoryStore provides functionality to add Qdrant vector database to support Semantic Kernel memory.
 The QdrantMemoryStore inherits from MemoryStoreBase for persisting/retrieving data from a Qdrant Vector Database.
 """
 
 import asyncio
 import logging
 import uuid
-from typing import List, Optional, Tuple
 
 from numpy import ndarray
 from qdrant_client import QdrantClient
 from qdrant_client import models as qdrant_models
 
 from semantic_kernel.exceptions import ServiceResponseException
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class QdrantMemoryStore(MemoryStoreBase):
     _qdrantclient: QdrantClient
 
     def __init__(
         self,
         vector_size: int,
-        url: Optional[str] = None,
-        port: Optional[int] = 6333,
-        local: Optional[bool] = False,
+        url: str | None = None,
+        port: int | None = 6333,
+        local: bool | None = False,
         **kwargs,
     ) -> None:
         """Initializes a new instance of the QdrantMemoryStore class."""
         if kwargs.get("logger"):
             logger.warning("The `logger` parameter is deprecated. Please use the `logging` module instead.")
         if local:
             if url:
@@ -60,15 +61,15 @@
             vectors_config=qdrant_models.VectorParams(
                 size=self._default_vector_size, distance=qdrant_models.Distance.COSINE
             ),
         )
 
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         collection_info = self._qdrantclient.get_collections()
         return [collection.name for collection in collection_info.collections]
@@ -130,15 +131,15 @@
         )
 
         if result.status == qdrant_models.UpdateStatus.COMPLETED:
             return data_to_upsert.id
         else:
             raise ServiceResponseException("Upsert failed")
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         tasks = []
         for record in records:
             tasks.append(
                 self._convert_from_memory_record(
                     collection_name=collection_name,
                     record=record,
                 )
@@ -152,15 +153,15 @@
         )
 
         if result.status == qdrant_models.UpdateStatus.COMPLETED:
             return [data.id for data in data_to_upsert]
         else:
             raise ServiceResponseException("Batch upsert failed")
 
-    async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> Optional[MemoryRecord]:
+    async def get(self, collection_name: str, key: str, with_embedding: bool = False) -> MemoryRecord | None:
         result = await self._get_existing_record_by_payload_id(
             collection_name=collection_name,
             payload_id=key,
             with_embedding=with_embedding,
         )
 
         if result:
@@ -175,16 +176,16 @@
                 key=result.id,
                 timestamp=result.payload["_timestamp"],
             )
         else:
             return None
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         tasks = []
         for key in keys:
             tasks.append(
                 self.get(
                     collection_name=collection_name,
                     key=key,
                     with_embedding=with_embeddings,
@@ -201,15 +202,15 @@
 
         if existing_record:
             pointId = existing_record.id
             result = self._qdrantclient.delete(collection_name=collection_name, points_selector=[pointId])
             if result.status != qdrant_models.UpdateStatus.COMPLETED:
                 raise ServiceResponseException("Delete failed")
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         tasks = []
         for key in keys:
             tasks.append(
                 self._get_existing_record_by_payload_id(
                     collection_name=collection_name,
                     payload_id=key,
                     with_embedding=False,
@@ -229,15 +230,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         match_results = self._qdrantclient.search(
             collection_name=collection_name,
             query_vector=embedding,
             limit=limit,
             score_threshold=min_relevance_score,
             with_vectors=with_embeddings,
         )
@@ -262,30 +263,30 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         result = await self.get_nearest_matches(
             collection_name=collection_name,
             embedding=embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
         return result[0] if result else None
 
     async def _get_existing_record_by_payload_id(
         self,
         collection_name: str,
         payload_id: str,
         with_embedding: bool = False,
-    ) -> Optional[qdrant_models.ScoredPoint]:
+    ) -> qdrant_models.ScoredPoint | None:
         """Gets an existing record based upon payload id.
 
         Arguments:
             collection_name {str} -- The name of the collection.
             payload_id {str} -- The payload id to search for.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/README.md` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/redis_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/redis_memory_store.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, Tuple
 
 import numpy as np
 import redis
 from numpy import ndarray
 from pydantic import ValidationError
 from redis.commands.search.field import TextField, VectorField
 from redis.commands.search.indexDefinition import IndexDefinition, IndexType
@@ -22,18 +21,20 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceResourceNotFoundError,
     ServiceResponseException,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class RedisMemoryStore(MemoryStoreBase):
     """A memory store implementation using Redis"""
 
     _database: "redis.Redis"
     _ft: "redis.Redis.ft"
     # Without RedisAI, it is currently not possible to retrieve index-specific vector attributes to have
     # fully independent collections.
@@ -131,15 +132,15 @@
             )
 
             try:
                 self._ft(collection_name).create_index(definition=index_def, fields=schema)
             except Exception as e:
                 raise ServiceResponseException(f"Failed to create collection {collection_name}") from e
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """
         Returns a list of names of all collection names present in the data store.
 
         Returns:
             List[str] -- list of collection names
         """
         # Note: FT._LIST is a temporary command that may be deprecated in the future according to Redis
@@ -204,15 +205,15 @@
                 record._key,
                 mapping=serialize_record_to_redis(record, self._vector_type),
             )
             return record._key
         except Exception as e:
             raise ServiceResponseException("Could not upsert messages.") from e
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """
         Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
             * If the record already exists, it will be updated.
             * If the record does not exist, it will be created.
 
         Note: if the records do not have the same dimensionality configured for the collection,
         they will not be detected to belong to the collection in Redis.
@@ -257,16 +258,16 @@
 
         record = deserialize_redis_to_record(fields, self._vector_type, with_embedding)
         record._key = internal_key
 
         return record
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """
         Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- Name for a collection of embeddings
             keys {List[str]} -- IDs associated with the memory records to get
             with_embedding {bool} -- Include embeddings with the memory records, default to False
@@ -293,15 +294,15 @@
             key {str} -- ID associated with the memory to remove
         """
         if not await self.does_collection_exist(collection_name):
             raise ServiceResourceNotFoundError(f'Collection "{collection_name}" does not exist')
 
         self._database.delete(get_redis_key(collection_name, key))
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """
         Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- Name for a collection of embeddings
             keys {List[str]} -- IDs associated with the memory records to remove
         """
@@ -313,15 +314,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """
         Get the nearest matches to an embedding using the configured similarity algorithm.
 
         Arguments:
             collection_name {str} -- Name for a collection of embeddings
             embedding {ndarray} -- Embedding to find the nearest matches to
             limit {int} -- Maximum number of matches to return
@@ -366,15 +367,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """
         Get the nearest match to an embedding using the configured similarity algorithm.
 
         Arguments:
             collection_name {str} -- Name for a collection of embeddings
             embedding {ndarray} -- Embedding to find the nearest match to
             min_relevance_score {float} -- Minimum relevance score of the match, default to 0.0
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/redis/utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/redis/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 from datetime import datetime
-from typing import Any, Dict, Tuple
+from typing import Any
 
 import numpy as np
 from redis import Redis
 from redis.commands.search.document import Document
 
 from semantic_kernel.memory.memory_record import MemoryRecord
 
@@ -21,29 +21,29 @@
 
     Returns:
         str -- Redis key in the format collection_name:id
     """
     return f"{collection_name}:{record_id}"
 
 
-def split_redis_key(redis_key: str) -> Tuple[str, str]:
+def split_redis_key(redis_key: str) -> tuple[str, str]:
     """
     Split a Redis key into its collection name and record ID
 
     Arguments:
         collection_name {str} -- Redis key
 
     Returns:
         Tuple[str, str] -- Tuple of the collection name and ID
     """
     collection, record_id = redis_key.split(":")
     return collection, record_id
 
 
-def serialize_record_to_redis(record: MemoryRecord, vector_type: np.dtype) -> Dict[str, Any]:
+def serialize_record_to_redis(record: MemoryRecord, vector_type: np.dtype) -> dict[str, Any]:
     all_metadata = {
         "is_reference": record._is_reference,
         "external_source_name": record._external_source_name or "",
         "id": record._id or "",
         "description": record._description or "",
         "text": record._text or "",
         "additional_metadata": record._additional_metadata or "",
@@ -54,15 +54,15 @@
         "timestamp": record._timestamp.isoformat() if record._timestamp else "",
         "metadata": json.dumps(all_metadata),
         "embedding": (record._embedding.astype(vector_type).tobytes() if record._embedding is not None else ""),
     }
     return redis_mapping
 
 
-def deserialize_redis_to_record(fields: Dict[str, Any], vector_type: np.dtype, with_embedding: bool) -> MemoryRecord:
+def deserialize_redis_to_record(fields: dict[str, Any], vector_type: np.dtype, with_embedding: bool) -> MemoryRecord:
     metadata = json.loads(fields[b"metadata"])
     record = MemoryRecord(
         id=metadata["id"],
         is_reference=True if metadata["is_reference"] is True else False,
         description=metadata["description"],
         external_source_name=metadata["external_source_name"],
         text=metadata["text"],
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/usearch/usearch_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 
 import itertools
 import logging
 import os
 from dataclasses import dataclass
 from enum import Enum
 from pathlib import Path
-from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
 import pyarrow.parquet as pq
 from numpy import ndarray
 from usearch.index import BatchMatches, CompiledMetric, Index, Matches, MetricKind, ScalarKind
@@ -18,14 +17,15 @@
 from semantic_kernel.exceptions import (
     ServiceInitializationError,
     ServiceInvalidRequestError,
     ServiceResourceNotFoundError,
 )
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 @dataclass
 class _USearchCollection:
     """Represents a collection for USearch with embeddings and related data.
@@ -34,15 +34,15 @@
         embeddings_index (Index): The index of embeddings.
         embeddings_data_table (pa.Table): The PyArrow table holding embeddings data.
         embeddings_id_to_label (Dict[str, int]): Mapping of embeddings ID to label.
     """
 
     embeddings_index: Index
     embeddings_data_table: pa.Table
-    embeddings_id_to_label: Dict[str, int]
+    embeddings_id_to_label: dict[str, int]
 
     @staticmethod
     def create_default(embeddings_index: Index) -> "_USearchCollection":
         """Create a default `_USearchCollection` using a given embeddings index.
 
         Args:
             embeddings_index (Index): The index of embeddings to be used for the default collection.
@@ -79,29 +79,29 @@
     """Enumeration of file types used for storing collections."""
 
     USEARCH = 0
     PARQUET = 1
 
 
 # Mapping of collection file types to their file extensions.
-_collection_file_extensions: Dict[_CollectionFileType, str] = {
+_collection_file_extensions: dict[_CollectionFileType, str] = {
     _CollectionFileType.USEARCH: ".usearch",
     _CollectionFileType.PARQUET: ".parquet",
 }
 
 
-def memoryrecords_to_pyarrow_table(records: List[MemoryRecord]) -> pa.Table:
+def memoryrecords_to_pyarrow_table(records: list[MemoryRecord]) -> pa.Table:
     """Convert a list of `MemoryRecord` to a PyArrow Table"""
     records_pylist = [
         {attr: getattr(record, "_" + attr) for attr in _embeddings_data_schema.names} for record in records
     ]
     return pa.Table.from_pylist(records_pylist, schema=_embeddings_data_schema)
 
 
-def pyarrow_table_to_memoryrecords(table: pa.Table, vectors: Optional[ndarray] = None) -> List[MemoryRecord]:
+def pyarrow_table_to_memoryrecords(table: pa.Table, vectors: ndarray | None = None) -> list[MemoryRecord]:
     """Convert a PyArrow Table to a list of MemoryRecords.
 
     Args:
         table (pa.Table): The PyArrow Table to convert.
         vectors (Optional[ndarray], optional): An array of vectors to include as embeddings in the MemoryRecords.
             The length and order of the vectors should match the rows in the table. Defaults to None.
 
@@ -112,18 +112,19 @@
         MemoryRecord(**row.to_dict(), embedding=vectors[index] if vectors is not None else None)
         for index, row in table.to_pandas().iterrows()
     ]
 
     return result_memory_records
 
 
+@experimental_class
 class USearchMemoryStore(MemoryStoreBase):
     def __init__(
         self,
-        persist_directory: Optional[os.PathLike] = None,
+        persist_directory: os.PathLike | None = None,
     ) -> None:
         """
         Create a USearchMemoryStore instance.
 
         This store helps searching embeddings with USearch, keeping collections in memory.
         To save collections to disk, provide the `persist_directory` param.
         Collections are saved when `close` is called.
@@ -134,15 +135,15 @@
 
         Args:
             persist_directory (Optional[os.PathLike], default=None): Directory for loading and saving collections.
             If None, collections are not loaded nor saved.
         """
         self._persist_directory = Path(persist_directory) if persist_directory is not None else None
 
-        self._collections: Dict[str, _USearchCollection] = {}
+        self._collections: dict[str, _USearchCollection] = {}
         if self._persist_directory:
             self._collections = self._read_collections_from_dir()
 
     def _get_collection_path(self, collection_name: str, *, file_type: _CollectionFileType) -> Path:
         """
         Get the path for the given collection name and file type.
 
@@ -162,19 +163,19 @@
 
         return self._persist_directory / (collection_name + _collection_file_extensions[file_type])
 
     async def create_collection(
         self,
         collection_name: str,
         ndim: int = 0,
-        metric: Union[str, MetricKind, CompiledMetric] = MetricKind.IP,
-        dtype: Optional[Union[str, ScalarKind]] = None,
-        connectivity: Optional[int] = None,
-        expansion_add: Optional[int] = None,
-        expansion_search: Optional[int] = None,
+        metric: str | MetricKind | CompiledMetric = MetricKind.IP,
+        dtype: str | ScalarKind | None = None,
+        connectivity: int | None = None,
+        expansion_add: int | None = None,
+        expansion_search: int | None = None,
         view: bool = False,
     ) -> None:
         """Create a new collection.
 
         Args:
             collection_name (str): Name of the collection. Case-insensitive.
                 Must have name that is valid file name for the current OS environment.
@@ -213,45 +214,45 @@
             view=view,
         )
 
         self._collections[collection_name] = _USearchCollection.create_default(embeddings_index)
 
         return None
 
-    def _read_embeddings_table(self, path: os.PathLike) -> Tuple[pa.Table, Dict[str, int]]:
+    def _read_embeddings_table(self, path: os.PathLike) -> tuple[pa.Table, dict[str, int]]:
         """Read embeddings from the provided path and generate an ID to label mapping.
 
         Args:
             path (os.PathLike): Path to the embeddings.
 
         Returns:
             Tuple of embeddings table and a dictionary mapping from record ID to its label.
         """
         embeddings_table = pq.read_table(path, schema=_embeddings_data_schema)
-        embeddings_id_to_label: Dict[str, int] = {
+        embeddings_id_to_label: dict[str, int] = {
             record_id: idx for idx, record_id in enumerate(embeddings_table.column("id").to_pylist())
         }
         return embeddings_table, embeddings_id_to_label
 
     def _read_embeddings_index(self, path: Path) -> Index:
         """Read embeddings index."""
         # str cast is temporarily fix for https://github.com/unum-cloud/usearch/issues/196
         return Index.restore(str(path), view=False)
 
-    def _read_collections_from_dir(self) -> Dict[str, _USearchCollection]:
+    def _read_collections_from_dir(self) -> dict[str, _USearchCollection]:
         """Read all collections from directory to memory.
 
         Raises:
             ValueError: If files for a collection do not match expected amount.
 
         Returns:
             Dict[str, _USearchCollection]: Dictionary with collection names as keys and
               their _USearchCollection as values.
         """
-        collections: Dict[str, _USearchCollection] = {}
+        collections: dict[str, _USearchCollection] = {}
 
         for collection_name, collection_files in self._get_all_storage_files().items():
             expected_storage_files = len(_CollectionFileType)
             if len(collection_files) != expected_storage_files:
                 raise ServiceInitializationError(
                     f"Expected {expected_storage_files} files for collection {collection_name}"
                 )
@@ -266,15 +267,15 @@
                 embeddings_index,
                 embeddings_table,
                 embeddings_id_to_label,
             )
 
         return collections
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Get list of existing collections.
 
         Returns:
             List[str]: List of collection names.
         """
         return list(self._collections.keys())
 
@@ -294,22 +295,22 @@
         collection_name = collection_name.lower()
         res = await self.upsert_batch(collection_name=collection_name, records=[record])
         return res[0]
 
     async def upsert_batch(
         self,
         collection_name: str,
-        records: List[MemoryRecord],
+        records: list[MemoryRecord],
         *,
         compact: bool = False,
         copy: bool = True,
         threads: int = 0,
-        log: Union[str, bool] = False,
+        log: str | bool = False,
         batch_size: int = 0,
-    ) -> List[str]:
+    ) -> list[str]:
         """Upsert a batch of MemoryRecords and return their IDs.
 
         Args:
             collection_name (str): Name of the collection to search within.
             records (List[MemoryRecord]): Records to upsert.
             compact (bool, optional): Removes links to removed nodes (expensive). Defaults to False.
             copy (bool, optional): Should the index store a copy of vectors. Defaults to True.
@@ -378,18 +379,18 @@
         if not result:
             raise ServiceResourceNotFoundError(f"Key '{key}' not found in collection '{collection_name}'")
         return result[0]
 
     async def get_batch(
         self,
         collection_name: str,
-        keys: List[str],
+        keys: list[str],
         with_embeddings: bool,
         dtype: ScalarKind = ScalarKind.F32,
-    ) -> List[MemoryRecord]:
+    ) -> list[MemoryRecord]:
         """Retrieve a batch of MemoryRecords using their keys."""
         collection_name = collection_name.lower()
         if collection_name not in self._collections:
             raise ServiceResourceNotFoundError(f"Collection {collection_name} does not exist")
 
         ucollection = self._collections[collection_name]
         labels = [ucollection.embeddings_id_to_label[key] for key in keys if key in ucollection.embeddings_id_to_label]
@@ -401,15 +402,15 @@
 
     async def remove(self, collection_name: str, key: str) -> None:
         """Remove a single MemoryRecord using its key."""
         collection_name = collection_name.lower()
         await self.remove_batch(collection_name=collection_name, keys=[key])
         return None
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Remove a batch of MemoryRecords using their keys."""
         collection_name = collection_name.lower()
         if collection_name not in self._collections:
             raise ServiceResourceNotFoundError(f"Collection {collection_name} does not exist, cannot insert.")
 
         ucollection = self._collections[collection_name]
 
@@ -423,15 +424,15 @@
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = True,
         exact: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Retrieve the nearest matching MemoryRecord for the provided embedding.
 
         By default it is approximately search, see `exact` param description.
 
         Measure of similarity between vectors is relevance score. It is from 0 to 1.
         USearch returns distances for vectors. Distance is converted to relevance score by inverse function.
 
@@ -463,17 +464,17 @@
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = True,
         *,
         threads: int = 0,
         exact: bool = False,
-        log: Union[str, bool] = False,
+        log: str | bool = False,
         batch_size: int = 0,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Get the nearest matches to a given embedding.
 
         By default it is approximately search, see `exact` param description.
 
         Measure of similarity between vectors is relevance score. It is from 0 to 1.
         USearch returns distances for vectors. Distance is converted to relevance score by inverse function.
 
@@ -494,42 +495,42 @@
 
         Returns:
             List[Tuple[MemoryRecord, float]]: The nearest matching records and their relevance score.
         """
         collection_name = collection_name.lower()
         ucollection = self._collections[collection_name]
 
-        result: Union[Matches, BatchMatches] = ucollection.embeddings_index.search(
+        result: Matches | BatchMatches = ucollection.embeddings_index.search(
             vectors=embedding,
             count=limit,
             threads=threads,
             exact=exact,
             log=log,
         )
 
         assert isinstance(result, Matches)
 
         relevance_score = 1 / (result.distances + 1)
         filtered_labels = result.keys[np.where(relevance_score >= min_relevance_score)[0]]
 
-        filtered_vectors: Optional[np.ndarray] = None
+        filtered_vectors: np.ndarray | None = None
         if with_embeddings:
             filtered_vectors = ucollection.embeddings_index.get(filtered_labels)
 
         return [
             (mem_rec, relevance_score[index].item())
             for index, mem_rec in enumerate(
                 pyarrow_table_to_memoryrecords(
                     ucollection.embeddings_data_table.take(pa.array(filtered_labels)),
                     filtered_vectors,
                 )
             )
         ]
 
-    def _get_all_storage_files(self) -> Dict[str, List[Path]]:
+    def _get_all_storage_files(self) -> dict[str, list[Path]]:
         """Return storage files for each collection in `self._persist_directory`.
 
         Collection name is derived from file name and converted to lowercase. Files with extensions that
         do not match storage extensions are discarded.
 
         Raises:
             ValueError: If persist directory is not set.
@@ -537,15 +538,15 @@
         Returns:
             Dict[str, List[Path]]: Dictionary of collection names mapped to their respective files.
         """
         if self._persist_directory is None:
             raise ServiceInitializationError("Persist directory is not set")
 
         storage_exts = _collection_file_extensions.values()
-        collection_storage_files: Dict[str, List[Path]] = {}
+        collection_storage_files: dict[str, list[Path]] = {}
         for path in self._persist_directory.iterdir():
             if path.is_file() and (path.suffix in storage_exts):
                 collection_name = path.stem.lower()
                 if collection_name in collection_storage_files:
                     collection_storage_files[collection_name].append(path)
                 else:
                     collection_storage_files[collection_name] = [path]
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
 from dataclasses import dataclass
-from typing import List, Tuple
 
 import numpy as np
 import weaviate
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.memory.weaviate.weaviate_settings import WeaviateSettings
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 SCHEMA = {
     "class": "MemoryRecord",
     "description": "A document from semantic kernel.",
     "properties": [
@@ -68,14 +68,15 @@
 @dataclass
 class WeaviateConfig:
     use_embed: bool = False
     url: str = None
     api_key: str = None
 
 
+@experimental_class
 class WeaviateMemoryStore(MemoryStoreBase):
     class FieldMapper:
         """
         This inner class is responsible for mapping attribute names between
         the SK's memory record and weaviate's schema. It provides methods
         for converting between the two naming conventions.
         """
@@ -170,15 +171,15 @@
         return weaviate.Client(url=self.settings.url)
 
     async def create_collection(self, collection_name: str) -> None:
         schema = SCHEMA.copy()
         schema["class"] = collection_name
         await asyncio.get_running_loop().run_in_executor(None, self.client.schema.create_class, schema)
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         schemas = await asyncio.get_running_loop().run_in_executor(None, self.client.schema.get)
         return [schema["class"] for schema in schemas["classes"]]
 
     async def delete_collection(self, collection_name: str) -> bool:
         await asyncio.get_running_loop().run_in_executor(None, self.client.schema.delete_class, collection_name)
 
     async def does_collection_exist(self, collection_name: str) -> bool:
@@ -196,15 +197,15 @@
             self.client.data_object.create,
             weaviate_record,
             collection_name,
             weaviate_id,
             vector,
         )
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         def _upsert_batch_inner():
             results = []
             with self.client.batch as batch:
                 for record in records:
                     weaviate_record = self.FieldMapper.sk_to_weaviate(vars(record))
                     vector = weaviate_record.pop("vector", None)
                     weaviate_id = weaviate.util.generate_uuid5(weaviate_record, collection_name)
@@ -221,28 +222,28 @@
         return await asyncio.get_running_loop().run_in_executor(None, _upsert_batch_inner)
 
     async def get(self, collection_name: str, key: str, with_embedding: bool) -> MemoryRecord:
         # Call the batched version with a single key
         results = await self.get_batch(collection_name, [key], with_embedding)
         return results[0] if results else None
 
-    async def get_batch(self, collection_name: str, keys: List[str], with_embedding: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embedding: bool) -> list[MemoryRecord]:
         queries = self._build_multi_get_query(collection_name, keys, with_embedding)
 
         results = await asyncio.get_running_loop().run_in_executor(None, self.client.query.multi_get(queries).do)
 
         get_dict = results.get("data", {}).get("Get", {})
 
         memory_records = [
             self._convert_weaviate_doc_to_memory_record(doc) for docs in get_dict.values() for doc in docs
         ]
 
         return memory_records
 
-    def _build_multi_get_query(self, collection_name: str, keys: List[str], with_embedding: bool):
+    def _build_multi_get_query(self, collection_name: str, keys: list[str], with_embedding: bool):
         queries = []
         for i, key in enumerate(keys):
             query = self.client.query.get(collection_name, ALL_PROPERTIES).with_where(
                 {
                     "path": ["key"],
                     "operator": "Equal",
                     "valueString": key,
@@ -264,15 +265,15 @@
         sk_doc = self.FieldMapper.weaviate_to_sk(weaviate_doc_copy)
         mem_vals = self.FieldMapper.remove_underscore_prefix(sk_doc)
         return MemoryRecord(**mem_vals)
 
     async def remove(self, collection_name: str, key: str) -> None:
         await self.remove_batch(collection_name, [key])
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         # TODO: Use In operator when it's available
         #       (https://github.com/weaviate/weaviate/issues/2387)
         #       and handle max delete objects
         #       (https://weaviate.io/developers/weaviate/api/rest/batch#maximum-number-of-deletes-per-query)
         for key in keys:
             where = {
                 "path": ["key"],
@@ -287,15 +288,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: np.ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         nearVector = {
             "vector": embedding,
             "certainty": min_relevance_score,
         }
 
         additional = ["certainty"]
         if with_embeddings:
@@ -326,15 +327,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: np.ndarray,
         min_relevance_score: float,
         with_embedding: bool,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         results = await self.get_nearest_matches(
             collection_name,
             embedding,
             limit=1,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embedding,
         )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/memory/weaviate/weaviate_settings.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from pydantic import SecretStr
 
 from semantic_kernel.connectors.memory.memory_settings_base import BaseModelSettings
 from semantic_kernel.kernel_pydantic import HttpsUrl
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class WeaviateSettings(BaseModelSettings):
     """Weaviate model settings
 
     Optional:
     - url: HttpsUrl | None - Weaviate URL (Env var WEAVIATE_URL)
     - api_key: SecretStr | None - Weaviate token (Env var WEAVIATE_API_KEY)
     - use_embed: bool - Whether to use the client embedding options
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_authentication_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
 from enum import Enum
 
 from pydantic import HttpUrl
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openai_plugin/openai_utils.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/openai_plugin/openai_utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
 import logging
 from typing import Any
 
 from semantic_kernel.exceptions.function_exceptions import PluginInitializationError
 
 logger: logging.Logger = logging.getLogger(__name__)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_function_execution_parameters.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,33 +1,35 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
-from typing import Any, Awaitable, Callable, List
+from collections.abc import Awaitable, Callable
+from typing import Any
 from urllib.parse import urlparse
 
 import httpx
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 AuthCallbackType = Callable[..., Awaitable[Any]]
 
 
+@experimental_class
 class OpenAPIFunctionExecutionParameters(KernelBaseModel):
     """OpenAPI function execution parameters."""
 
     http_client: httpx.AsyncClient | None = None
     auth_callback: AuthCallbackType | None = None
     server_url_override: str | None = None
     ignore_non_compliant_errors: bool = False
     user_agent: str | None = None
     enable_dynamic_payload: bool = True
     enable_payload_namespacing: bool = False
-    operations_to_exclude: List[str] = Field(default_factory=list)
+    operations_to_exclude: list[str] = Field(default_factory=list)
 
     def model_post_init(self, __context: Any) -> None:
         from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 
         if self.server_url_override:
             parsed_url = urlparse(self.server_url_override)
             if not parsed_url.scheme or not parsed_url.netloc:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/openapi_plugin/openapi_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,94 +1,98 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
-
 import json
 import logging
 import re
+from collections.abc import Callable, Mapping
 from enum import Enum
-from typing import TYPE_CHECKING, Any, Callable, Dict, Mapping, Tuple
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urlencode, urljoin, urlparse, urlunparse
 
 import httpx
 from openapi_core import Spec
 from prance import ResolvingParser
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.exceptions.function_exceptions import FunctionExecutionException, PluginInitializationError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
+from semantic_kernel.utils.experimental_decorator import experimental_class, experimental_function
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
         OpenAIFunctionExecutionParameters,
     )
     from semantic_kernel.connectors.openapi_plugin.openapi_function_execution_parameters import (
         OpenAPIFunctionExecutionParameters,
     )
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class RestApiOperationParameterStyle(Enum):
     SIMPLE = "simple"
 
 
+@experimental_class
 class RestApiOperationPayloadProperty:
     def __init__(
         self,
         name: str,
         type: str,
-        properties: RestApiOperationPayloadProperty,
+        properties: "RestApiOperationPayloadProperty",
         description: str | None = None,
         is_required: bool = False,
         default_value: Any | None = None,
         schema: str | None = None,
     ):
         self.name = name
         self.type = type
         self.properties = properties
         self.description = description
         self.is_required = is_required
         self.default_value = default_value
         self.schema = schema
 
 
+@experimental_class
 class RestApiOperationPayload:
     def __init__(
         self,
         media_type: str,
-        properties: list[RestApiOperationPayloadProperty],
+        properties: list["RestApiOperationPayloadProperty"],
         description: str | None = None,
         schema: str | None = None,
     ):
         self.media_type = media_type
         self.properties = properties
         self.description = description
         self.schema = schema
 
 
+@experimental_class
 class RestApiOperation:
     MEDIA_TYPE_TEXT_PLAIN = "text/plain"
     PAYLOAD_ARGUMENT_NAME = "payload"
     CONTENT_TYPE_ARGUMENT_NAME = "content-type"
     INVALID_SYMBOLS_REGEX = re.compile(r"[^0-9A-Za-z_]+")
 
     def __init__(
         self,
         id: str,
         method: str,
         server_url: str,
         path: str,
         summary: str | None = None,
         description: str | None = None,
-        params: list[RestApiOperationParameter] | None = None,
-        request_body: RestApiOperationPayload | None = None,
+        params: list["RestApiOperationParameter"] | None = None,
+        request_body: "RestApiOperationPayload | None" = None,
     ):
         self.id = id
         self.method = method.upper()
         self.server_url = server_url
         self.path = path
         self.summary = summary
         self.description = description
@@ -101,15 +105,15 @@
         if not parsed_base.path.endswith("/"):
             base_path = parsed_base.path + "/"
         else:
             base_path = parsed_base.path
         full_path = urljoin(base_path, path.lstrip("/"))
         return urlunparse(parsed_base._replace(path=full_path))
 
-    def build_headers(self, arguments: Dict[str, Any]) -> Dict[str, str]:
+    def build_headers(self, arguments: dict[str, Any]) -> dict[str, str]:
         headers = {}
 
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.HEADER]
 
         for parameter in parameters:
             argument = arguments.get(parameter.name)
 
@@ -142,29 +146,29 @@
 
         # make sure the base URL ends with a trailing slash
         if not server_url_string.endswith("/"):
             server_url_string += "/"
 
         return urlparse(server_url_string)
 
-    def build_path(self, path_template: str, arguments: Dict[str, Any]) -> str:
+    def build_path(self, path_template: str, arguments: dict[str, Any]) -> str:
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.PATH]
         for parameter in parameters:
             argument = arguments.get(parameter.name)
             if argument is None:
                 if parameter.is_required:
                     raise FunctionExecutionException(
                         f"No argument is provided for the `{parameter.name}` "
                         f"required parameter of the operation - `{self.id}`."
                     )
                 continue
             path_template = path_template.replace(f"{{{parameter.name}}}", str(argument))
         return path_template
 
-    def build_query_string(self, arguments: Dict[str, Any]) -> str:
+    def build_query_string(self, arguments: dict[str, Any]) -> str:
         segments = []
         parameters = [p for p in self.parameters if p.location == RestApiOperationParameterLocation.QUERY]
         for parameter in parameters:
             argument = arguments.get(parameter.name)
             if argument is None:
                 if parameter.is_required:
                     raise FunctionExecutionException(
@@ -176,18 +180,18 @@
         return urlencode(segments)
 
     def replace_invalid_symbols(self, parameter_name):
         return RestApiOperation.INVALID_SYMBOLS_REGEX.sub("_", parameter_name)
 
     def get_parameters(
         self,
-        operation: RestApiOperation,
+        operation: "RestApiOperation",
         add_payload_params_from_metadata: bool = True,
         enable_payload_spacing: bool = False,
-    ) -> list[RestApiOperationParameter]:
+    ) -> list["RestApiOperationParameter"]:
         params = list(operation.parameters)
         if operation.request_body is not None:
             params.extend(
                 self.get_payload_parameters(
                     operation=operation,
                     use_parameters_from_metadata=add_payload_params_from_metadata,
                     enable_namespacing=enable_payload_spacing,
@@ -195,15 +199,15 @@
             )
 
         for parameter in params:
             parameter.alternative_name = self.replace_invalid_symbols(parameter.name)
 
         return params
 
-    def create_payload_artificial_parameter(self, operation: RestApiOperation) -> RestApiOperationParameter:
+    def create_payload_artificial_parameter(self, operation: "RestApiOperation") -> "RestApiOperationParameter":
         return RestApiOperationParameter(
             name=self.PAYLOAD_ARGUMENT_NAME,
             type=(
                 "string"
                 if operation.request_body
                 and operation.request_body.media_type == RestApiOperation.MEDIA_TYPE_TEXT_PLAIN
                 else "object"
@@ -211,15 +215,15 @@
             is_required=True,
             location=RestApiOperationParameterLocation.BODY,
             style=RestApiOperationParameterStyle.SIMPLE,
             description=operation.request_body.description if operation.request_body else "REST API request body.",
             schema=operation.request_body.schema if operation.request_body else None,
         )
 
-    def create_content_type_artificial_parameter(self) -> RestApiOperationParameter:
+    def create_content_type_artificial_parameter(self) -> "RestApiOperationParameter":
         return RestApiOperationParameter(
             name=self.CONTENT_TYPE_ARGUMENT_NAME,
             type="string",
             is_required=False,
             location=RestApiOperationParameterLocation.BODY,
             style=RestApiOperationParameterStyle.SIMPLE,
             description="Content type of REST API request body.",
@@ -230,18 +234,18 @@
     ):
         if enable_namespacing and root_property_name:
             return f"{root_property_name}.{property.name}"
         return property.name
 
     def _get_parameters_from_payload_metadata(
         self,
-        properties: list[RestApiOperationPayloadProperty],
+        properties: list["RestApiOperationPayloadProperty"],
         enable_namespacing: bool = False,
         root_property_name: bool = None,
-    ) -> list[RestApiOperationParameter]:
+    ) -> list["RestApiOperationParameter"]:
         parameters: list[RestApiOperationParameter] = []
         for property in properties:
             parameter_name = self._get_property_name(property, root_property_name, enable_namespacing)
             if not property.properties:
                 parameters.append(
                     RestApiOperationParameter(
                         name=parameter_name,
@@ -255,15 +259,15 @@
                 )
             parameters.extend(
                 self._get_parameters_from_payload_metadata(property.properties, enable_namespacing, parameter_name)
             )
         return parameters
 
     def get_payload_parameters(
-        self, operation: RestApiOperation, use_parameters_from_metadata: bool, enable_namespacing: bool
+        self, operation: "RestApiOperation", use_parameters_from_metadata: bool, enable_namespacing: bool
     ):
         if use_parameters_from_metadata:
             if operation.request_body is None:
                 raise Exception(
                     f"Payload parameters cannot be retrieved from the `{operation.Id}` "
                     f"operation payload metadata because it is missing."
                 )
@@ -274,49 +278,51 @@
 
         return [
             self.create_payload_artificial_parameter(operation),
             self.create_content_type_artificial_parameter(operation),
         ]
 
 
+@experimental_class
 class RestApiOperationParameterLocation(Enum):
     """The location of the REST API operation parameter."""
 
     PATH = "path"
     QUERY = "query"
     HEADER = "header"
     COOKIE = "cookie"
     BODY = "body"
 
 
+@experimental_class
 class RestApiOperationParameter:
     def __init__(
         self,
         name: str,
         type: str,
         location: RestApiOperationParameterLocation,
         style: RestApiOperationParameterStyle | None = None,
         alternative_name: str | None = None,
         description: str | None = None,
         is_required: bool = False,
         default_value: Any | None = None,
         schema: str | None = None,
     ):
-
         self.name = name
         self.type = type
         self.location = location
         self.style = style
         self.alternative_name = alternative_name
         self.description = description
         self.is_required = is_required
         self.default_value = default_value
         self.schema = schema
 
 
+@experimental_class
 class OpenApiParser:
     """
     NOTE: SK Python only supports the OpenAPI Spec >=3.0
 
     Import an OpenAPI file.
 
     Args:
@@ -412,15 +418,15 @@
             schema="str",  # TODO - add support for JSON schema?
         )
 
     def create_rest_api_operations(
         self,
         parsed_document: Any,
         execution_settings: "OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None" = None,
-    ) -> Dict[str, RestApiOperation]:
+    ) -> dict[str, RestApiOperation]:
         """Create the REST API Operations from the parsed OpenAPI document.
 
         Args:
             parsed_document: The parsed OpenAPI document
             execution_settings: The execution settings
 
         Returns:
@@ -459,43 +465,46 @@
                     description=description,
                 )
 
                 request_objects[operationId] = rest_api_operation
         return request_objects
 
 
+@experimental_class
 class Uri:
     """The Uri class that represents the URI."""
 
     def __init__(self, uri):
         self.uri = uri
 
     def get_left_part(self):
         parsed_uri = urlparse(self.uri)
         return f"{parsed_uri.scheme}://{parsed_uri.netloc}"
 
 
+@experimental_class
 class RestApiOperationRunOptions:
     """The options for running the REST API operation."""
 
     def __init__(self, server_url_override=None, api_host_url=None):
         self.server_url_override: str = server_url_override
         self.api_host_url: str = api_host_url
 
 
+@experimental_class
 class OpenApiRunner:
     """The OpenApiRunner that runs the operations defined in the OpenAPI manifest"""
 
     payload_argument_name = "payload"
     media_type_application_json = "application/json"
 
     def __init__(
         self,
         parsed_openapi_document: Mapping[str, str],
-        auth_callback: Callable[[Dict[str, str]], Dict[str, str]] | None = None,
+        auth_callback: Callable[[dict[str, str]], dict[str, str]] | None = None,
         http_client: httpx.AsyncClient | None = None,
         enable_dynamic_payload: bool = True,
         enable_payload_namespacing: bool = False,
     ):
         self.spec = Spec.from_dict(parsed_openapi_document)
         self.auth_callback = auth_callback
         self.http_client = http_client
@@ -512,16 +521,16 @@
         self, operation: RestApiOperation, arguments: KernelArguments, server_url_override=None, api_host_url=None
     ):
         """Build the operation URL."""
         url = operation.build_operation_url(arguments, server_url_override, api_host_url)
         return self.build_full_url(url, operation.build_query_string(arguments))
 
     def build_json_payload(
-        self, payload_metadata: RestApiOperationPayload, arguments: Dict[str, Any]
-    ) -> Tuple[str, str]:
+        self, payload_metadata: RestApiOperationPayload, arguments: dict[str, Any]
+    ) -> tuple[str, str]:
         """Build the JSON payload."""
         if self.enable_dynamic_payload:
             if payload_metadata is None:
                 raise FunctionExecutionException(
                     "Payload can't be built dynamically due to the missing payload metadata."
                 )
 
@@ -551,15 +560,15 @@
                 continue
             if property_metadata.is_required:
                 raise FunctionExecutionException(
                     f"No argument is found for the '{property_metadata.name}' payload property."
                 )
         return result
 
-    def build_operation_payload(self, operation: RestApiOperation, arguments: KernelArguments) -> Tuple[str, str]:
+    def build_operation_payload(self, operation: RestApiOperation, arguments: KernelArguments) -> tuple[str, str]:
         if operation.request_body is None and self.payload_argument_name not in arguments:
             return None, None
         return self.build_json_payload(operation.request_body, arguments)
 
     def get_argument_name_for_payload(self, property_name, property_namespace=None):
         if not self.enable_payload_namespacing:
             return property_name
@@ -613,14 +622,15 @@
             else:
                 async with httpx.AsyncClient() as client:
                     return await make_request(client)
 
         return await fetch()
 
 
+@experimental_function
 def create_functions_from_openapi(
     plugin_name: str,
     openapi_document_path: str,
     execution_settings: "OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None" = None,
 ) -> list[KernelFunctionFromMethod]:
     """Creates the functions from OpenAPI document.
 
@@ -649,14 +659,15 @@
 
     return [
         _create_function_from_operation(openapi_runner, operation, plugin_name, execution_parameters=execution_settings)
         for operation in operations.values()
     ]
 
 
+@experimental_function
 def _create_function_from_operation(
     runner: OpenApiRunner,
     operation: RestApiOperation,
     plugin_name: str | None = None,
     execution_parameters: "OpenAIFunctionExecutionParameters | OpenAPIFunctionExecutionParameters | None" = None,
     document_uri: str | None = None,
 ) -> KernelFunctionFromMethod:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import urllib
-from typing import List
 
 import aiohttp
 from pydantic import ValidationError
 
 from semantic_kernel.connectors.search_engine.bing_connector_settings import BingSettings
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 from semantic_kernel.exceptions import ServiceInvalidRequestError
@@ -37,15 +36,15 @@
             logger.warning(f"Failed to load the Bing pydantic settings: {e}.")
 
         self._api_key = api_key or (
             bing_settings.api_key.get_secret_value() if bing_settings and bing_settings.api_key else None
         )
         assert self._api_key, "API key cannot be 'None' or empty."
 
-    async def search(self, query: str, num_results: int = 1, offset: int = 0) -> List[str]:
+    async def search(self, query: str, num_results: int = 1, offset: int = 0) -> list[str]:
         """
         Returns the search results of the query provided by pinging the Bing web search API.
         Returns `num_results` results and ignores the first `offset`.
 
         :param query: search query
         :param num_results: the number of search results to return
         :param offset: the number of search results to ignore
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/bing_connector_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/bing_connector_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/search_engine/google_connector.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/search_engine/google_connector.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import urllib
-from typing import List
 
 import aiohttp
 
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 from semantic_kernel.exceptions import ServiceInitializationError, ServiceInvalidRequestError
 
 logger: logging.Logger = logging.getLogger(__name__)
@@ -26,15 +25,15 @@
 
         if not self._api_key:
             raise ServiceInitializationError("Google Custom Search API key cannot be null.")
 
         if not self._search_engine_id:
             raise ServiceInitializationError("Google search engine ID cannot be null.")
 
-    async def search(self, query: str, num_results: int = 1, offset: int = 0) -> List[str]:
+    async def search(self, query: str, num_results: int = 1, offset: int = 0) -> list[str]:
         """
         Returns the search results of the query provided by pinging the Google Custom search API.
         Returns `num_results` results and ignores the first `offset`.
 
         :param query: search query
         :param num_results: the number of search results to return
         :param offset: the number of search results to ignore
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/telemetry.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/telemetry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import os
 from importlib.metadata import PackageNotFoundError, version
-from typing import Any, Dict
+from typing import Any
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 
 TELEMETRY_DISABLED_ENV_VAR = "AZURE_TELEMETRY_DISABLED"
 
 IS_TELEMETRY_ENABLED = os.environ.get(TELEMETRY_DISABLED_ENV_VAR, "false").lower() not in ["true", "1"]
 
@@ -22,15 +22,15 @@
         "Semantic-Kernel-Version": f"python-{version_info}",
     }
     if IS_TELEMETRY_ENABLED
     else None
 )
 
 
-def prepend_semantic_kernel_to_user_agent(headers: Dict[str, Any]):
+def prepend_semantic_kernel_to_user_agent(headers: dict[str, Any]):
     """
     Prepend "Semantic-Kernel" to the User-Agent in the headers.
 
     Args:
         headers: The existing headers dictionary.
 
     Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/connectors/utils/document_loader.py` & `semantic_kernel-1.0.1/semantic_kernel/connectors/utils/document_loader.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Any, Callable, Optional
+from collections.abc import Callable
+from typing import Any
 
 import httpx
 
 from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class DocumentLoader:
 
     @staticmethod
     async def from_uri(
         url: str,
         http_client: httpx.AsyncClient,
-        auth_callback: Optional[Callable[[Any], None]],
-        user_agent: Optional[str] = HTTP_USER_AGENT,
+        auth_callback: Callable[[Any], None] | None,
+        user_agent: str | None = HTTP_USER_AGENT,
     ):
         """Load the manifest from the given URL"""
         headers = {"User-Agent": user_agent}
         async with http_client as client:
             if auth_callback:
                 await auth_callback(client, url)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_history.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/chat_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
+from collections.abc import Generator
 from functools import singledispatchmethod
 from html import unescape
-from typing import Any, Generator
+from typing import Any
 from xml.etree.ElementTree import Element, tostring
 
 from defusedxml.ElementTree import XML, ParseError
 from pydantic import field_validator
 
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
@@ -284,15 +284,15 @@
         """
         try:
             return self.model_dump_json(indent=2, exclude_none=True)
         except Exception as e:  # pragma: no cover
             raise ContentSerializationError(f"Unable to serialize ChatHistory to JSON: {e}") from e
 
     @classmethod
-    def restore_chat_history(cls, chat_history_json: str) -> ChatHistory:
+    def restore_chat_history(cls, chat_history_json: str) -> "ChatHistory":
         """
         Restores a ChatHistory instance from a JSON string.
 
         Args:
             chat_history_json (str): The JSON string to deserialize
                 into a ChatHistory instance.
 
@@ -316,15 +316,15 @@
             file_path (str): The path to the file where the serialized data will be stored.
         """
         json_str = self.serialize()
         with open(file_path, "w") as file:
             file.write(json_str)
 
     @classmethod
-    def load_chat_history_from_file(cls, file_path: str) -> ChatHistory:
+    def load_chat_history_from_file(cls, file_path: str) -> "ChatHistory":
         """
         Loads the ChatHistory from a file.
 
         Args:
             file_path (str): The path to the file from which to load the ChatHistory.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/chat_message_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/chat_message_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
 from enum import Enum
 from html import unescape
 from typing import Any, Union, overload
 from xml.etree.ElementTree import Element
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_call_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/function_call_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import json
 import logging
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from xml.etree.ElementTree import Element
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/function_result_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/function_result_content.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from functools import cached_property
 from typing import TYPE_CHECKING, Any
 from xml.etree.ElementTree import Element
 
 from pydantic import field_validator
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/kernel_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/kernel_content.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from abc import ABC, abstractmethod
 from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_chat_message_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_chat_message_content.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from enum import Enum
 from typing import Any, Union, overload
 from xml.etree.ElementTree import Element
 
 from semantic_kernel.contents.author_role import AuthorRole
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
@@ -159,15 +158,15 @@
             **kwargs,
         )
 
     def __bytes__(self) -> bytes:
         """Return the content of the response encoded in the encoding."""
         return self.content.encode(self.encoding if self.encoding else "utf-8") if self.content else b""
 
-    def __add__(self, other: StreamingChatMessageContent) -> StreamingChatMessageContent:
+    def __add__(self, other: "StreamingChatMessageContent") -> "StreamingChatMessageContent":
         """When combining two StreamingChatMessageContent instances, the content fields are combined.
 
         The inner_content of the first one is used, ai_model_id and encoding should be the same,
         if role is set, they should be the same.
         """
         if not isinstance(other, StreamingChatMessageContent):
             raise ContentAdditionException(
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_content_mixin.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_content_mixin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/streaming_text_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/streaming_text_content.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/text_content.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/text_content.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from html import unescape
 from xml.etree.ElementTree import Element
 
 from semantic_kernel.contents.const import TEXT_CONTENT_TAG
 from semantic_kernel.contents.kernel_content import KernelContent
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/contents/types.py` & `semantic_kernel-1.0.1/semantic_kernel/contents/types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/conversation_summary_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/conversation_summary_plugin.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
-import sys
-from typing import TYPE_CHECKING
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
-
+from typing import TYPE_CHECKING, Annotated
 
 if TYPE_CHECKING:
     from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.kernel import Kernel
     from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/http_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/http_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
-import sys
-from typing import Any, Dict, Optional
+from typing import Annotated, Any
 
 import aiohttp
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
-
 from semantic_kernel.exceptions import FunctionExecutionException
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class HttpPlugin(KernelBaseModel):
     """
@@ -48,15 +42,15 @@
             async with session.get(url, raise_for_status=True) as response:
                 return await response.text()
 
     @kernel_function(description="Makes a POST request to a uri", name="postAsync")
     async def post(
         self,
         url: Annotated[str, "The URI to send the request to."],
-        body: Annotated[Optional[Dict[str, Any]], "The body of the request"] = {},
+        body: Annotated[dict[str, Any] | None, "The body of the request"] = {},
     ) -> str:
         """
         Sends an HTTP POST request to the specified URI and returns
         the response body as a string.
         params:
             url: The URI to send the request to.
             body: Contains the body of the request
@@ -72,15 +66,15 @@
             async with session.post(url, headers=headers, data=data, raise_for_status=True) as response:
                 return await response.text()
 
     @kernel_function(description="Makes a PUT request to a uri", name="putAsync")
     async def put(
         self,
         url: Annotated[str, "The URI to send the request to."],
-        body: Annotated[Optional[Dict[str, Any]], "The body of the request"] = {},
+        body: Annotated[dict[str, Any] | None, "The body of the request"] = {},
     ) -> str:
         """
         Sends an HTTP PUT request to the specified URI and returns
         the response body as a string.
         params:
             url: The URI to send the request to.
         returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/math_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/math_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
-import sys
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
+from typing import Annotated
 
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 
 
 class MathPlugin:
     """
     Description: MathPlugin provides a set of functions to make Math calculations.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/README.md` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_plugin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
 import logging
 import os
 import re
+from collections.abc import Awaitable, Callable
 from io import BufferedReader, BytesIO
-from typing import Annotated, Any, Awaitable, Callable
+from typing import Annotated, Any
 
 import httpx
 from pydantic import ValidationError, field_validator
 
 from semantic_kernel.connectors.ai.open_ai.const import USER_AGENT
 from semantic_kernel.connectors.telemetry import HTTP_USER_AGENT, version_info
 from semantic_kernel.core_plugins.sessions_python_tool.sessions_python_settings import (
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_python_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
 import uuid
 from enum import Enum
 
 from pydantic import Field
 from pydantic_settings import BaseSettings
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/sessions_python_tool/sessions_remote_file_metadata.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_memory_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_memory_plugin.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 import json
 import logging
-import sys
-from typing import Any, Dict, Final
+from typing import Annotated, Any, Final
 
 from pydantic import Field
 
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
-
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 DEFAULT_COLLECTION: Final[str] = "generic"
@@ -22,17 +16,17 @@
 DEFAULT_RELEVANCE: Final[float] = 0.75
 RELEVANCE_PARAM: Final[str] = "relevance"
 DEFAULT_LIMIT: Final[int] = 1
 
 
 class TextMemoryPlugin(KernelBaseModel):
     memory: SemanticTextMemoryBase
-    embeddings_kwargs: Dict[str, Any] = Field(default_factory=dict)
+    embeddings_kwargs: dict[str, Any] = Field(default_factory=dict)
 
-    def __init__(self, memory: SemanticTextMemoryBase, embeddings_kwargs: Dict[str, Any] = {}) -> None:
+    def __init__(self, memory: SemanticTextMemoryBase, embeddings_kwargs: dict[str, Any] = {}) -> None:
         """
         Initialize a new instance of the TextMemoryPlugin
 
         Args:
             memory (SemanticTextMemoryBase) - the underlying Semantic Text Memory to use
             embeddings_kwargs (Optional[Dict[str, Any]]) - the keyword arguments to pass to the embedding generator
         """
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/text_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/text_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/time_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/time_plugin.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/core_plugins/web_search_engine_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/core_plugins/web_search_engine_plugin.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,8 @@
-import sys
-from typing import TYPE_CHECKING, List, Optional
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
+from typing import TYPE_CHECKING, Annotated
 
 from semantic_kernel.functions.kernel_function_decorator import kernel_function
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.search_engine.connector import ConnectorBase
 
 
@@ -31,17 +25,17 @@
     def __init__(self, connector: "ConnectorBase") -> None:
         self._connector = connector
 
     @kernel_function(description="Performs a web search for a given query")
     async def search(
         self,
         query: Annotated[str, "The search query"],
-        num_results: Annotated[Optional[int], "The number of search results to return"] = 1,
-        offset: Annotated[Optional[int], "The number of search results to skip"] = 0,
-    ) -> List[str]:
+        num_results: Annotated[int | None, "The number of search results to return"] = 1,
+        offset: Annotated[int | None, "The number of search results to skip"] = 0,
+    ) -> list[str]:
         """
         Returns the search results of the query provided.
         Returns `num_results` results and ignores the first `offset`.
 
         :param query: search query
         :param num_results: number of search results to return, default is 1
         :param offset: number of search results to skip, default is 0
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/content_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/content_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/function_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/function_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/kernel_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/kernel_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/planner_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/planner_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/service_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/service_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/exceptions/template_engine_exceptions.py` & `semantic_kernel-1.0.1/semantic_kernel/exceptions/template_engine_exceptions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py` & `semantic_kernel-1.0.1/semantic_kernel/filters/auto_function_invocation/auto_function_invocation_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/filters/filter_context_base.py` & `semantic_kernel-1.0.1/semantic_kernel/filters/filter_context_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/function_result.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/function_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
 from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.contents.kernel_content import KernelContent
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_arguments.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_arguments.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any
 
 if TYPE_CHECKING:
     from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 
 
 class KernelArguments(dict):
     def __init__(
         self,
         settings: (
-            "PromptExecutionSettings" | list["PromptExecutionSettings"] | dict[str, "PromptExecutionSettings"] | None
+            "PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None"
         ) = None,
         **kwargs: Any,
     ):
         """Initializes a new instance of the KernelArguments class,
         this is a dict-like class with the additional field for the execution_settings.
 
         This class is derived from a dict, hence behaves the same way,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
 from abc import abstractmethod
-from collections.abc import AsyncGenerator
+from collections.abc import AsyncGenerator, Callable
 from copy import copy, deepcopy
 from inspect import isasyncgen, isgenerator
-from typing import TYPE_CHECKING, Any, Callable
+from typing import TYPE_CHECKING, Any
 
 from semantic_kernel.filters.filter_types import FilterTypes
 from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
+from semantic_kernel.filters.kernel_filters_extension import _rebuild_function_invocation_context
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
-from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_function_invocation_context
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import (
     HANDLEBARS_TEMPLATE_FORMAT_NAME,
     JINJA2_TEMPLATE_FORMAT_NAME,
     KERNEL_TEMPLATE_FORMAT_NAME,
     TEMPLATE_FORMAT_TYPES,
 )
@@ -73,20 +72,20 @@
     def from_prompt(
         cls,
         function_name: str,
         plugin_name: str,
         description: str | None = None,
         prompt: str | None = None,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
-        prompt_template: PromptTemplateBase | None = None,
-        prompt_template_config: PromptTemplateConfig | None = None,
+        prompt_template: "PromptTemplateBase | None " = None,
+        prompt_template_config: "PromptTemplateConfig | None" = None,
         prompt_execution_settings: (
-            PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None
+            "PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings] | None"
         ) = None,
-    ) -> KernelFunctionFromPrompt:
+    ) -> "KernelFunctionFromPrompt":
         """
         Create a new instance of the KernelFunctionFromPrompt class.
         """
         from semantic_kernel.functions.kernel_function_from_prompt import KernelFunctionFromPrompt
 
         return KernelFunctionFromPrompt(
             function_name=function_name,
@@ -101,15 +100,15 @@
 
     @classmethod
     def from_method(
         cls,
         method: Callable[..., Any],
         plugin_name: str | None = None,
         stream_method: Callable[..., Any] | None = None,
-    ) -> KernelFunctionFromMethod:
+    ) -> "KernelFunctionFromMethod":
         """
         Create a new instance of the KernelFunctionFromMethod class.
         """
         from semantic_kernel.functions.kernel_function_from_method import KernelFunctionFromMethod
 
         return KernelFunctionFromMethod(
             plugin_name=plugin_name,
@@ -134,25 +133,25 @@
         return self.metadata.description
 
     @property
     def is_prompt(self) -> bool:
         return self.metadata.is_prompt
 
     @property
-    def parameters(self) -> list[KernelParameterMetadata]:
+    def parameters(self) -> list["KernelParameterMetadata"]:
         return self.metadata.parameters
 
     @property
-    def return_parameter(self) -> KernelParameterMetadata | None:
+    def return_parameter(self) -> "KernelParameterMetadata | None":
         return self.metadata.return_parameter
 
     async def __call__(
         self,
-        kernel: Kernel,
-        arguments: KernelArguments | None = None,
+        kernel: "Kernel",
+        arguments: "KernelArguments | None" = None,
         metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> FunctionResult | None:
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
@@ -176,16 +175,16 @@
             context (FunctionInvocationContext): The invocation context.
 
         """
         pass
 
     async def invoke(
         self,
-        kernel: Kernel,
-        arguments: KernelArguments | None = None,
+        kernel: "Kernel",
+        arguments: "KernelArguments | None" = None,
         metadata: dict[str, Any] = {},
         **kwargs: Any,
     ) -> "FunctionResult | None":
         """Invoke the function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
@@ -216,19 +215,19 @@
         The abstract method is defined without async because otherwise the typing fails.
         A implementation of this function should be async.
         """
         ...
 
     async def invoke_stream(
         self,
-        kernel: Kernel,
-        arguments: KernelArguments | None = None,
+        kernel: "Kernel",
+        arguments: "KernelArguments | None" = None,
         metadata: dict[str, Any] = {},
         **kwargs: Any,
-    ) -> AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]:
+    ) -> "AsyncGenerator[FunctionResult | list[StreamingContentMixin | Any], Any]":
         """
         Invoke a stream async function with the given arguments.
 
         Args:
             kernel (Kernel): The kernel
             arguments (KernelArguments): The Kernel arguments
             kwargs (Any): Additional keyword arguments that will be
@@ -256,15 +255,15 @@
                     yield partial
             elif isgenerator(function_context.result.value):
                 for partial in function_context.result.value:
                     yield partial
             else:
                 yield function_context.result
 
-    def function_copy(self, plugin_name: str | None = None) -> KernelFunction:
+    def function_copy(self, plugin_name: str | None = None) -> "KernelFunction":
         """Copy the function, can also override the plugin_name.
 
         Args:
             plugin_name (str): The new plugin name.
 
         Returns:
             KernelFunction: The copied function.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_decorator.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
-from inspect import get_annotations, isasyncgenfunction, isclass, isgeneratorfunction, signature
-from typing import Any, Callable, ForwardRef
+from collections.abc import Callable
+from inspect import Parameter, isasyncgenfunction, isclass, isgeneratorfunction, signature
+from typing import Any, ForwardRef
 
 NoneType = type(None)
 logger = logging.getLogger(__name__)
 
 
 def kernel_function(
     func: Callable[..., object] | None = None,
@@ -45,86 +45,74 @@
 
     def decorator(func: Callable[..., object]) -> Callable[..., object]:
         setattr(func, "__kernel_function__", True)
         setattr(func, "__kernel_function_description__", description or func.__doc__)
         setattr(func, "__kernel_function_name__", name or getattr(func, "__name__", "unknown"))
         setattr(func, "__kernel_function_streaming__", isasyncgenfunction(func) or isgeneratorfunction(func))
         logger.debug(f"Parsing decorator for function: {getattr(func, '__kernel_function_name__')}")
-        func_sig = signature(func)
-        annotations = {name: None for name, _ in func_sig.parameters.items() if name != "self"}
-        try:
-            annotations.update(get_annotations(func, eval_str=True))
-        except Exception as ex:
-            logger.error(f"Failed to get annotations for function {func.__name__}: {ex}")
+        func_sig = signature(func, eval_str=True)
+        annotations = []
+        for arg in func_sig.parameters.values():
+            if arg.name == "self":
+                continue
+            if arg.default == arg.empty:
+                annotations.append(_parse_parameter(arg.name, arg.annotation, None))
+            else:
+                annotations.append(_parse_parameter(arg.name, arg.annotation, arg.default))
         logger.debug(f"{annotations=}")
-        setattr(
-            func,
-            "__kernel_function_parameters__",
-            [_parse_parameter(name, param) for name, param in annotations.items() if name != "return"],
+        setattr(func, "__kernel_function_parameters__", annotations)
+
+        return_annotation = (
+            _parse_parameter("return", func_sig.return_annotation, None) if func_sig.return_annotation else {}
         )
-        defaults = getattr(func, "__defaults__", None)
-        logger.debug(f"{defaults=}")
-        assert hasattr(func, "__kernel_function_parameters__")
-        if defaults:
-            for index, default in enumerate(defaults):
-                if default is None:
-                    continue
-                if func.__kernel_function_parameters__[index]:
-                    func.__kernel_function_parameters__[index]["default_value"] = default
-                    func.__kernel_function_parameters__[index]["is_required"] = False
-        return_param_dict = {}
-        if "return" in annotations:
-            return_param_dict = _parse_parameter("return", annotations["return"])
-        setattr(func, "__kernel_function_return_type__", return_param_dict.get("type_", "None"))
-        setattr(func, "__kernel_function_return_description__", return_param_dict.get("description", ""))
-        setattr(func, "__kernel_function_return_required__", return_param_dict.get("is_required", False))
+        setattr(func, "__kernel_function_return_type__", return_annotation.get("type_", "None"))
+        setattr(func, "__kernel_function_return_description__", return_annotation.get("description", ""))
+        setattr(func, "__kernel_function_return_required__", return_annotation.get("is_required", False))
         return func
 
     if func:
         return decorator(func)
     return decorator
 
 
-def _parse_parameter(name: str, param: Any) -> dict[str, Any]:
+def _parse_parameter(name: str, param: Any, default: Any) -> dict[str, Any]:
     logger.debug(f"Parsing param: {name}")
     logger.debug(f"Parsing annotation: {param}")
     ret: dict[str, Any] = {"name": name}
-    if not param:
-        ret["type_"] = "Any"
+    if default:
+        ret["default_value"] = default
+        ret["is_required"] = False
+    else:
         ret["is_required"] = True
+    if not param or param == Parameter.empty:
+        ret["type_"] = "Any"
         return ret
     if not isinstance(param, str):
-        if hasattr(param, "default"):
-            ret["default_value"] = param.default
-            ret["is_required"] = False
-        else:
-            ret["is_required"] = True
         if hasattr(param, "__metadata__"):
             ret["description"] = param.__metadata__[0]
         if hasattr(param, "__origin__"):
-            ret.update(_parse_parameter(name, param.__origin__))
+            ret.update(_parse_parameter(name, param.__origin__, default))
         if hasattr(param, "__args__"):
             args = []
             for arg in param.__args__:
                 if arg == NoneType:
                     ret["is_required"] = False
-                    ret["default_value"] = None
+                    if "default_value" not in ret:
+                        ret["default_value"] = None
                     continue
                 if isinstance(arg, ForwardRef):
                     arg = arg.__forward_arg__
-                args.append(_parse_parameter(name, arg))
+                args.append(_parse_parameter(name, arg, default))
             if ret.get("type_") in ["list", "dict"]:
                 ret["type_"] = f"{ret['type_']}[{', '.join([arg['type_'] for arg in args])}]"
             elif len(args) > 1:
                 ret["type_"] = ", ".join([arg["type_"] for arg in args])
             else:
                 ret["type_"] = args[0]["type_"]
                 ret["type_object"] = args[0].get("type_object", None)
-                if def_value := args[0].get("default_value", None):
-                    ret["default_value"] = def_value
         elif isclass(param):
             ret["type_"] = param.__name__
             ret["type_object"] = param
         else:
             ret["type_"] = str(param).replace(" |", ",")
     else:
         if "|" in param:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_method.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
+from collections.abc import Callable
 from inspect import isasyncgen, isasyncgenfunction, isawaitable, iscoroutinefunction, isgenerator, isgeneratorfunction
-from typing import Any, Callable
+from typing import Any
 
 from pydantic import ValidationError
 
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_function import KernelFunction
@@ -58,15 +58,15 @@
         if parameters is None:
             parameters = [KernelParameterMetadata(**param) for param in method.__kernel_function_parameters__]  # type: ignore
         if return_parameter is None:
             return_param = KernelParameterMetadata(
                 name="return",
                 description=method.__kernel_function_return_description__,  # type: ignore
                 default_value=None,
-                type=method.__kernel_function_return_type__,  # type: ignore
+                type_=method.__kernel_function_return_type__,  # type: ignore
                 is_required=method.__kernel_function_return_required__,  # type: ignore
             )
 
         try:
             metadata = KernelFunctionMetadata(
                 name=function_name,
                 description=description,
@@ -120,14 +120,16 @@
         function_arguments = self.gather_function_parameters(context)
         context.result = FunctionResult(function=self.metadata, value=self.stream_method(**function_arguments))
 
     def gather_function_parameters(self, context: FunctionInvocationContext) -> dict[str, Any]:
         """Gathers the function parameters from the arguments."""
         function_arguments: dict[str, Any] = {}
         for param in self.parameters:
+            if param.name is None:
+                raise FunctionExecutionException("Parameter name cannot be None")
             if param.name == "kernel":
                 function_arguments[param.name] = context.kernel
                 continue
             if param.name == "service":
                 function_arguments[param.name] = context.kernel.select_ai_service(self, context.arguments)[0]
                 continue
             if param.name == "execution_settings":
@@ -144,18 +146,21 @@
                             value = param.type_object.model_validate(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
                                 f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
                             ) from exc
                     else:
                         try:
-                            value = param.type_object(value)
+                            if isinstance(value, dict) and hasattr(param.type_object, "__init__"):
+                                value = param.type_object(**value)
+                            else:
+                                value = param.type_object(value)
                         except Exception as exc:
                             raise FunctionExecutionException(
-                                f"Parameter {param.name} is expected to be parsed to {param.type_} but is not."
+                                f"Parameter {param.name} is expected to be parsed to {param.type_object} but is not."
                             ) from exc
                 function_arguments[param.name] = value
                 continue
             if param.is_required:
                 raise FunctionExecutionException(
                     f"Parameter {param.name} is required but not provided in the arguments."
                 )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_from_prompt.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_from_prompt.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import logging
 import os
+from collections.abc import AsyncGenerator
 from html import unescape
-from typing import Any, AsyncGenerator
+from typing import Any
 
 import yaml
 from pydantic import Field, ValidationError, model_validator
 
 from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
 from semantic_kernel.contents.chat_history import ChatHistory
 from semantic_kernel.contents.chat_message_content import ChatMessageContent
 from semantic_kernel.contents.text_content import TextContent
 from semantic_kernel.exceptions import FunctionExecutionException, FunctionInitializationError
 from semantic_kernel.exceptions.function_exceptions import PromptRenderingException
 from semantic_kernel.filters.filter_types import FilterTypes
 from semantic_kernel.filters.functions.function_invocation_context import FunctionInvocationContext
+from semantic_kernel.filters.kernel_filters_extension import _rebuild_prompt_render_context
 from semantic_kernel.filters.prompts.prompt_render_context import PromptRenderContext
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import TEMPLATE_FORMAT_MAP, KernelFunction
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.functions.prompt_rendering_result import PromptRenderingResult
-from semantic_kernel.kernel_extensions.kernel_filters_extension import _rebuild_prompt_render_context
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
 from semantic_kernel.prompt_template.prompt_template_base import PromptTemplateBase
 from semantic_kernel.prompt_template.prompt_template_config import PromptTemplateConfig
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 PROMPT_FILE_NAME = "skprompt.txt"
@@ -270,15 +270,15 @@
     def update_arguments_with_defaults(self, arguments: KernelArguments) -> None:
         """Update any missing values with their defaults."""
         for parameter in self.prompt_template.prompt_template_config.input_variables:
             if parameter.name not in arguments and parameter.default not in {None, "", False, 0}:
                 arguments[parameter.name] = parameter.default
 
     @classmethod
-    def from_yaml(cls, yaml_str: str, plugin_name: str | None = None) -> KernelFunctionFromPrompt:
+    def from_yaml(cls, yaml_str: str, plugin_name: str | None = None) -> "KernelFunctionFromPrompt":
         """Creates a new instance of the KernelFunctionFromPrompt class from a YAML string."""
         try:
             data = yaml.safe_load(yaml_str)
         except yaml.YAMLError as exc:  # pragma: no cover
             raise FunctionInitializationError(f"Invalid YAML content: {yaml_str}, error: {exc}") from exc
 
         if not isinstance(data, dict):
@@ -295,15 +295,15 @@
             plugin_name=plugin_name,
             description=prompt_template_config.description,
             prompt_template_config=prompt_template_config,
             template_format=prompt_template_config.template_format,
         )
 
     @classmethod
-    def from_directory(cls, path: str, plugin_name: str | None = None) -> KernelFunctionFromPrompt:
+    def from_directory(cls, path: str, plugin_name: str | None = None) -> "KernelFunctionFromPrompt":
         """Creates a new instance of the KernelFunctionFromPrompt class from a directory.
 
         The directory needs to contain:
         - A prompt file named `skprompt.txt`
         - A config file named `config.json`
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_function_metadata.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_function_metadata.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,28 +1,27 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
-from typing import Any, List, Optional
+from typing import Any
 
 from pydantic import Field
 
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.utils.validation import FUNCTION_NAME_REGEX, PLUGIN_NAME_REGEX
 
 
 class KernelFunctionMetadata(KernelBaseModel):
     name: str = Field(pattern=FUNCTION_NAME_REGEX)
-    plugin_name: Optional[str] = Field(None, pattern=PLUGIN_NAME_REGEX)
-    description: Optional[str] = Field(default=None)
-    parameters: List[KernelParameterMetadata] = Field(default_factory=list)
+    plugin_name: str | None = Field(None, pattern=PLUGIN_NAME_REGEX)
+    description: str | None = Field(default=None)
+    parameters: list[KernelParameterMetadata] = Field(default_factory=list)
     is_prompt: bool
-    is_asynchronous: Optional[bool] = Field(default=True)
-    return_parameter: Optional[KernelParameterMetadata] = None
-    additional_properties: Optional[dict[str, Any]] = Field(default=None)
+    is_asynchronous: bool | None = Field(default=True)
+    return_parameter: KernelParameterMetadata | None = None
+    additional_properties: dict[str, Any] | None = Field(default=None)
 
     @property
     def fully_qualified_name(self) -> str:
         """
         Get the fully qualified name of the function.
 
         Returns:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/kernel_plugin.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/kernel_plugin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,19 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 import importlib
 import inspect
 import json
 import logging
 import os
-import sys
-from collections.abc import Generator
+from collections.abc import Generator, ItemsView
 from functools import singledispatchmethod
 from glob import glob
 from types import MethodType
-from typing import TYPE_CHECKING, Any, ItemsView
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated  # pragma: no cover
-else:
-    from typing_extensions import Annotated  # pragma: no cover
+from typing import TYPE_CHECKING, Annotated, Any
 
 import httpx
 from pydantic import Field, StringConstraints
 
 from semantic_kernel.connectors.openai_plugin.openai_authentication_config import OpenAIAuthenticationConfig
 from semantic_kernel.connectors.openai_plugin.openai_function_execution_parameters import (
     OpenAIFunctionExecutionParameters,
@@ -59,15 +52,16 @@
         name (str): The name of the plugin. The name can be upper/lower
             case letters and underscores.
         description (str): The description of the plugin.
         functions (Dict[str, KernelFunction]): The functions in the plugin,
             indexed by their name.
 
     Methods:
-        set, __setitem__ (key: str, value: KernelFunction): Set a function in the plugin.
+        set (key: str, value: KernelFunction): Set a function in the plugin.
+        __setitem__ (key: str, value: KernelFunction): Set a function in the plugin.
         get (key: str, default: KernelFunction | None = None): Get a function from the plugin.
         __getitem__ (key: str): Get a function from the plugin.
         __contains__ (key: str): Check if a function is in the plugin.
         __iter__ (): Iterate over the functions in the plugin.
         update(*args: Any, **kwargs: Any): Update the plugin with the functions from another.
         setdefault(key: str, value: KernelFunction | None): Set a default value for a key.
         get_functions_metadata(): Get the metadata for the functions in the plugin.
@@ -100,16 +94,16 @@
 
     def __init__(
         self,
         name: str,
         description: str | None = None,
         functions: (
             KERNEL_FUNCTION_TYPE
-            | KernelPlugin
-            | list[KERNEL_FUNCTION_TYPE | KernelPlugin]
+            | "KernelPlugin"
+            | list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]
             | dict[str, KERNEL_FUNCTION_TYPE]
             | None
         ) = None,
     ):
         """Create a KernelPlugin
 
         Attributes:
@@ -134,15 +128,15 @@
             description=description,
             functions=self._validate_functions(functions=functions, plugin_name=name),
         )
 
     # region Dict-like methods
 
     def __setitem__(self, key: str, value: KERNEL_FUNCTION_TYPE) -> None:
-        """Set a function in the plugin.
+        """Sets a function in the plugin.
 
         This function uses plugin[function_name] = function syntax.
 
         Args:
             key (str): The name of the function.
             value (KernelFunction): The function to set.
 
@@ -195,15 +189,15 @@
         self.add(kwargs)
 
     @singledispatchmethod
     def add(self, functions: Any) -> None:
         raise TypeError(f"Unknown type being added, type was {type(functions)}")
 
     @add.register(list)
-    def add_list(self, functions: list[KERNEL_FUNCTION_TYPE | KernelPlugin]) -> None:
+    def add_list(self, functions: list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]) -> None:
         """Add a list of functions to the plugin."""
         for function in functions:
             if isinstance(function, KernelPlugin):
                 self.add(function.functions)
                 continue
             function = KernelPlugin._parse_or_copy(function, self.name)
             self[function.name] = function
@@ -227,30 +221,30 @@
 
     def __contains__(self, key: str) -> bool:
         return key in self.functions
 
     # endregion
     # region Properties
 
-    def get_functions_metadata(self) -> list[KernelFunctionMetadata]:
+    def get_functions_metadata(self) -> list["KernelFunctionMetadata"]:
         """
         Get the metadata for the functions in the plugin.
 
         Returns:
             A list of KernelFunctionMetadata instances.
         """
         return [func.metadata for func in self]
 
     # endregion
     # region Class Methods
 
     @classmethod
     def from_object(
         cls, plugin_name: str, plugin_instance: Any | dict[str, Any], description: str | None = None
-    ) -> KernelPlugin:
+    ) -> "KernelPlugin":
         """
         Creates a plugin that wraps the specified target object and imports it into the kernel's plugin collection
 
         Args:
             plugin_instance (Any | dict[str, Any]): The plugin instance. This can be a custom class or a
                 dictionary of classes that contains methods with the kernel_function decorator for one or
                 several methods. See `TextMemoryPlugin` as an example.
@@ -277,15 +271,15 @@
     @classmethod
     def from_directory(
         cls,
         plugin_name: str,
         parent_directory: str,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
-    ) -> KernelPlugin:
+    ) -> "KernelPlugin":
         """Create a plugin from a specified directory.
 
         This method does not recurse into subdirectories beyond one level deep from the specified plugin directory.
         For YAML files, function names are extracted from the content of the YAML files themselves (the name property).
         For directories, the function name is assumed to be the name of the directory. Each KernelFunction object is
         initialized with data parsed from the associated files and added to a list of functions that are then assigned
         to the created KernelPlugin object.
@@ -366,17 +360,17 @@
         return cls(name=plugin_name, description=description, functions=functions)  # type: ignore
 
     @classmethod
     def from_openapi(
         cls,
         plugin_name: str,
         openapi_document_path: str,
-        execution_settings: OpenAPIFunctionExecutionParameters | None = None,
+        execution_settings: "OpenAPIFunctionExecutionParameters | None" = None,
         description: str | None = None,
-    ) -> KernelPlugin:
+    ) -> "KernelPlugin":
         """Create a plugin from an OpenAPI document.
 
         Args:
             plugin_name (str): The name of the plugin
             plugin_url (str | None): The URL of the plugin
             plugin_str (str | None): The JSON string of the plugin
             execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
@@ -404,17 +398,17 @@
 
     @classmethod
     async def from_openai(
         cls,
         plugin_name: str,
         plugin_url: str | None = None,
         plugin_str: str | None = None,
-        execution_parameters: OpenAIFunctionExecutionParameters | None = None,
+        execution_parameters: "OpenAIFunctionExecutionParameters | None" = None,
         description: str | None = None,
-    ) -> KernelPlugin:
+    ) -> "KernelPlugin":
         """Create a plugin from the Open AI manifest.
 
         Args:
             plugin_name (str): The name of the plugin
             plugin_url (str | None): The URL of the plugin
             plugin_str (str | None): The JSON string of the plugin
             execution_parameters (OpenAIFunctionExecutionParameters | None): The execution parameters
@@ -470,15 +464,15 @@
     @classmethod
     def from_python_file(
         cls,
         plugin_name: str,
         py_file: str,
         description: str | None = None,
         class_init_arguments: dict[str, dict[str, Any]] | None = None,
-    ) -> KernelPlugin:
+    ) -> "KernelPlugin":
         module_name = os.path.basename(py_file).replace(".py", "")
         spec = importlib.util.spec_from_file_location(module_name, py_file)
         if not spec:
             raise PluginInitializationError(f"Could not load spec from file {py_file}")
         module = importlib.util.module_from_spec(spec)
         if not module or not spec.loader:
             raise PluginInitializationError(f"No module found in file {py_file}")
@@ -494,21 +488,21 @@
     # endregion
     # region Internal Static Methods
 
     @staticmethod
     def _validate_functions(
         functions: (
             KERNEL_FUNCTION_TYPE
-            | list[KERNEL_FUNCTION_TYPE | KernelPlugin]
+            | list[KERNEL_FUNCTION_TYPE | "KernelPlugin"]
             | dict[str, KERNEL_FUNCTION_TYPE]
-            | KernelPlugin
+            | "KernelPlugin"
             | None
         ),
         plugin_name: str,
-    ) -> dict[str, KernelFunction]:
+    ) -> dict[str, "KernelFunction"]:
         """Validates the functions and returns a dictionary of functions."""
         if not functions or not plugin_name:
             # if the plugin_name is not present, the validation will fail, so no point in parsing.
             return {}
         if isinstance(functions, dict):
             return {
                 name: KernelPlugin._parse_or_copy(function=function, plugin_name=plugin_name)
@@ -538,15 +532,15 @@
                     )
                 else:
                     raise ValueError(f"Invalid type for functions in list: {function} (type: {type(function)})")
             return functions_dict
         raise ValueError(f"Invalid type for supplied functions: {functions} (type: {type(functions)})")
 
     @staticmethod
-    def _parse_or_copy(function: KERNEL_FUNCTION_TYPE, plugin_name: str) -> KernelFunction:
+    def _parse_or_copy(function: KERNEL_FUNCTION_TYPE, plugin_name: str) -> "KernelFunction":
         """Handle the function and return a KernelFunction instance."""
         if isinstance(function, KernelFunction):
             return function.function_copy(plugin_name=plugin_name)
         if callable(function):
             return KernelFunctionFromMethod(method=function, plugin_name=plugin_name)
         raise ValueError(f"Invalid type for function: {function} (type: {type(function)})")
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/functions/prompt_rendering_result.py` & `semantic_kernel-1.0.1/semantic_kernel/functions/prompt_rendering_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.functions.function_result import FunctionResult
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.services.ai_service_client_base import AIServiceClientBase
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/kernel_extensions/kernel_filters_extension.py` & `semantic_kernel-1.0.1/semantic_kernel/filters/kernel_filters_extension.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+from abc import ABC
+from collections.abc import Callable, Coroutine
 from functools import partial
-from typing import Any, Callable, Coroutine, Literal, TypeVar
+from typing import Any, Literal, TypeVar
 
 from pydantic import Field
 
 from semantic_kernel.filters.filter_context_base import FilterContextBase
 from semantic_kernel.filters.filter_types import FilterTypes
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.utils.experimental_decorator import experimental_function
@@ -19,15 +21,15 @@
 FILTER_MAPPING = {
     FilterTypes.FUNCTION_INVOCATION: "function_invocation_filters",
     FilterTypes.PROMPT_RENDERING: "prompt_rendering_filters",
     FilterTypes.AUTO_FUNCTION_INVOCATION: "auto_function_invocation_filters",
 }
 
 
-class KernelFilterExtension(KernelBaseModel):
+class KernelFilterExtension(KernelBaseModel, ABC):
     """KernelFilterExtension."""
 
     function_invocation_filters: list[tuple[int, CALLABLE_FILTER_TYPE]] = Field(default_factory=list)
     prompt_rendering_filters: list[tuple[int, CALLABLE_FILTER_TYPE]] = Field(default_factory=list)
     auto_function_invocation_filters: list[tuple[int, CALLABLE_FILTER_TYPE]] = Field(default_factory=list)
 
     @experimental_function
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/memory_query_result.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Optional
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class MemoryQueryResult:
     is_reference: bool
-    external_source_name: Optional[str]
+    external_source_name: str | None
     id: str
-    description: Optional[str]
-    text: Optional[str]
-    additional_metadata: Optional[str]
+    description: str | None
+    text: str | None
+    additional_metadata: str | None
     relevance: float
-    embedding: Optional[ndarray]
+    embedding: ndarray | None
 
     def __init__(
         self,
         is_reference: bool,
-        external_source_name: Optional[str],
+        external_source_name: str | None,
         id: str,
-        description: Optional[str],
-        text: Optional[str],
-        additional_metadata: Optional[str],
-        embedding: Optional[ndarray],
+        description: str | None,
+        text: str | None,
+        additional_metadata: str | None,
+        embedding: ndarray | None,
         relevance: float,
     ) -> None:
         """Initialize a new instance of MemoryQueryResult.
 
         Arguments:
             is_reference {bool} -- Whether the record is a reference record.
             external_source_name {Optional[str]} -- The name of the external source.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_record.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/memory_record.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from datetime import datetime
-from typing import Optional
 
 from numpy import ndarray
 
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
+
+@experimental_class
 class MemoryRecord:
     _key: str
-    _timestamp: Optional[datetime]
+    _timestamp: datetime | None
     _is_reference: bool
-    _external_source_name: Optional[str]
+    _external_source_name: str | None
     _id: str
-    _description: Optional[str]
-    _text: Optional[str]
-    _additional_metadata: Optional[str]
+    _description: str | None
+    _text: str | None
+    _additional_metadata: str | None
     _embedding: ndarray
 
     def __init__(
         self,
         is_reference: bool,
-        external_source_name: Optional[str],
+        external_source_name: str | None,
         id: str,
-        description: Optional[str],
-        text: Optional[str],
-        additional_metadata: Optional[str],
-        embedding: Optional[ndarray],
-        key: Optional[str] = None,
-        timestamp: Optional[datetime] = None,
+        description: str | None,
+        text: str | None,
+        additional_metadata: str | None,
+        embedding: ndarray | None,
+        key: str | None = None,
+        timestamp: datetime | None = None,
     ) -> None:
         """Initialize a new instance of MemoryRecord.
 
         Arguments:
             is_reference {bool} -- Whether the record is a reference record.
             external_source_name {Optional[str]} -- The name of the external source.
             id {str} -- A unique for the record.
@@ -53,16 +55,16 @@
         self._additional_metadata = additional_metadata
         self._embedding = embedding
 
     @staticmethod
     def reference_record(
         external_id: str,
         source_name: str,
-        description: Optional[str],
-        additional_metadata: Optional[str],
+        description: str | None,
+        additional_metadata: str | None,
         embedding: ndarray,
     ) -> "MemoryRecord":
         """Create a reference record.
 
         Arguments:
             external_id {str} -- The external id of the record.
             source_name {str} -- The name of the external source.
@@ -83,18 +85,18 @@
             embedding=embedding,
         )
 
     @staticmethod
     def local_record(
         id: str,
         text: str,
-        description: Optional[str],
-        additional_metadata: Optional[str],
+        description: str | None,
+        additional_metadata: str | None,
         embedding: ndarray,
-        timestamp: Optional[datetime] = None,
+        timestamp: datetime | None = None,
     ) -> "MemoryRecord":
         """Create a local record.
 
         Arguments:
             id {str} -- A unique for the record.
             text {str} -- The text of the record.
             description {Optional[str]} -- The description of the record.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/memory_store_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import ABC, abstractmethod
-from typing import List, Tuple
 
 from numpy import ndarray
 
 from semantic_kernel.memory.memory_record import MemoryRecord
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class MemoryStoreBase(ABC):
     async def __aenter__(self):
         return self
 
     async def __aexit__(self, *args):
         await self.close()
 
@@ -30,15 +31,15 @@
             None
         """
         pass
 
     @abstractmethod
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> list[str]:
         """Gets all collection names in the data store.
 
         Returns:
             List[str] -- A group of collection names.
         """
         pass
 
@@ -79,15 +80,15 @@
 
         Returns:
             str -- The unique identifier for the memory record.
         """
         pass
 
     @abstractmethod
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a group of memory records into the data store. Does not guarantee that the collection exists.
             If the record already exists, it will be updated.
             If the record does not exist, it will be created.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             records {MemoryRecord} -- The memory records to upsert.
@@ -108,15 +109,15 @@
 
         Returns:
             MemoryRecord -- The memory record if found
         """
         pass
 
     @abstractmethod
-    async def get_batch(self, collection_name: str, keys: List[str], with_embeddings: bool) -> List[MemoryRecord]:
+    async def get_batch(self, collection_name: str, keys: list[str], with_embeddings: bool) -> list[MemoryRecord]:
         """Gets a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             keys {List[str]} -- The unique ids associated with the memory records to get.
             with_embeddings {bool} -- If true, the embedding will be returned in the memory records.
 
@@ -135,15 +136,15 @@
 
         Returns:
             None
         """
         pass
 
     @abstractmethod
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of memory records from the data store. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             keys {List[str]} -- The unique ids associated with the memory records to remove.
 
         Returns:
@@ -155,15 +156,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float,
         with_embeddings: bool,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding of type float. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             embedding {ndarray} -- The embedding to compare the collection's embeddings with.
             limit {int} -- The maximum number of similarity results to return.
             min_relevance_score {float} -- The minimum relevance threshold for returned results.
@@ -178,15 +179,15 @@
     @abstractmethod
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float,
         with_embedding: bool,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding of type float. Does not guarantee that the collection exists.
 
         Arguments:
             collection_name {str} -- The name associated with a collection of embeddings.
             embedding {ndarray} -- The embedding to compare the collection's embeddings with.
             min_relevance_score {float} -- The minimum relevance threshold for returned result.
             with_embedding {bool} -- If true, the embeddings will be returned in the memory record.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/null_memory.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/null_memory.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,52 +1,53 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import List, Optional
 
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class NullMemory(SemanticTextMemoryBase):
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
+        description: str | None = None,
+        additional_metadata: str | None = None,
     ) -> None:
         """Nullifies behavior of SemanticTextMemoryBase.save_information()"""
         return None
 
     async def save_reference(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
+        description: str | None = None,
+        additional_metadata: str | None = None,
     ) -> None:
         """Nullifies behavior of SemanticTextMemoryBase.save_reference()"""
         return None
 
-    async def get(self, collection: str, query: str) -> Optional[MemoryQueryResult]:
+    async def get(self, collection: str, query: str) -> MemoryQueryResult | None:
         """Nullifies behavior of SemanticTextMemoryBase.get()"""
         return None
 
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.7,
-    ) -> List[MemoryQueryResult]:
+    ) -> list[MemoryQueryResult]:
         """Nullifies behavior of SemanticTextMemoryBase.search()"""
         return []
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Nullifies behavior of SemanticTextMemoryBase.get_collections()"""
         return []
 
 
 NullMemory.instance = NullMemory()  # type: ignore
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Any, Dict, List, Optional
+from typing import Any
 
 from pydantic import PrivateAttr
 
 from semantic_kernel.connectors.ai.embeddings.embedding_generator_base import EmbeddingGeneratorBase
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
 from semantic_kernel.memory.semantic_text_memory_base import SemanticTextMemoryBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 
+@experimental_class
 class SemanticTextMemory(SemanticTextMemoryBase):
     _storage: MemoryStoreBase = PrivateAttr()
     # TODO: replace with kernel and service_selector pattern
     _embeddings_generator: EmbeddingGeneratorBase = PrivateAttr()
 
     def __init__(self, storage: MemoryStoreBase, embeddings_generator: EmbeddingGeneratorBase) -> None:
         """Initialize a new instance of SemanticTextMemory.
@@ -32,17 +34,17 @@
         self._embeddings_generator = embeddings_generator
 
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
-        embeddings_kwargs: Optional[Dict[str, Any]] = {},
+        description: str | None = None,
+        additional_metadata: str | None = None,
+        embeddings_kwargs: dict[str, Any] | None = {},
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the information to.
             text {str} -- The text to save.
             id {str} -- The id of the information.
@@ -68,17 +70,17 @@
 
     async def save_reference(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
-        embeddings_kwargs: Optional[Dict[str, Any]] = {},
+        description: str | None = None,
+        additional_metadata: str | None = None,
+        embeddings_kwargs: dict[str, Any] | None = {},
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the reference to.
             text {str} -- The text to save.
             external_id {str} -- The external id of the reference.
@@ -103,15 +105,15 @@
 
         await self._storage.upsert(collection_name=collection, record=data)
 
     async def get(
         self,
         collection: str,
         key: str,
-    ) -> Optional[MemoryQueryResult]:
+    ) -> MemoryQueryResult | None:
         """Get information from the memory (calls the memory store's get method).
 
         Arguments:
             collection {str} -- The collection to get the information from.
             key {str} -- The key of the information.
 
         Returns:
@@ -123,16 +125,16 @@
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-        embeddings_kwargs: Optional[Dict[str, Any]] = {},
-    ) -> List[MemoryQueryResult]:
+        embeddings_kwargs: dict[str, Any] | None = {},
+    ) -> list[MemoryQueryResult]:
         """Search the memory (calls the memory store's get_nearest_matches method).
 
         Arguments:
             collection {str} -- The collection to search in.
             query {str} -- The query to search for.
             limit {int} -- The maximum number of results to return. (default: {1})
             min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
@@ -148,14 +150,14 @@
             limit=limit,
             min_relevance_score=min_relevance_score,
             with_embeddings=with_embeddings,
         )
 
         return [MemoryQueryResult.from_memory_record(r[0], r[1]) for r in results]
 
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Get the list of collections in the memory (calls the memory store's get_collections method).
 
         Returns:
             List[str] -- The list of all the memory collection names.
         """
         return await self._storage.get_collections()
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from abc import abstractmethod
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import Any, TypeVar
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 SemanticTextMemoryT = TypeVar("SemanticTextMemoryT", bound="SemanticTextMemoryBase")
 
 
+@experimental_class
 class SemanticTextMemoryBase(KernelBaseModel):
     @abstractmethod
     async def save_information(
         self,
         collection: str,
         text: str,
         id: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
-        embeddings_kwargs: Optional[Dict[str, Any]] = None,
+        description: str | None = None,
+        additional_metadata: str | None = None,
+        embeddings_kwargs: dict[str, Any] | None = None,
         # TODO: ctoken?
     ) -> None:
         """Save information to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the information to.
             text {str} -- The text to save.
@@ -37,16 +39,16 @@
     @abstractmethod
     async def save_reference(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
-        description: Optional[str] = None,
-        additional_metadata: Optional[str] = None,
+        description: str | None = None,
+        additional_metadata: str | None = None,
     ) -> None:
         """Save a reference to the memory (calls the memory store's upsert method).
 
         Arguments:
             collection {str} -- The collection to save the reference to.
             text {str} -- The text to save.
             external_id {str} -- The external id of the reference.
@@ -60,15 +62,15 @@
 
     @abstractmethod
     async def get(
         self,
         collection: str,
         key: str,
         # TODO: with_embedding: bool,
-    ) -> Optional[MemoryQueryResult]:
+    ) -> MemoryQueryResult | None:
         """Get information from the memory (calls the memory store's get method).
 
         Arguments:
             collection {str} -- The collection to get the information from.
             key {str} -- The key of the information.
 
         Returns:
@@ -80,15 +82,15 @@
     async def search(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.7,
         # TODO: ctoken?
-    ) -> List[MemoryQueryResult]:
+    ) -> list[MemoryQueryResult]:
         """Search the memory (calls the memory store's get_nearest_matches method).
 
         Arguments:
             collection {str} -- The collection to search in.
             query {str} -- The query to search for.
             limit {int} -- The maximum number of results to return. (default: {1})
             min_relevance_score {float} -- The minimum relevance score to return. (default: {0.0})
@@ -96,14 +98,14 @@
 
         Returns:
             List[MemoryQueryResult] -- The list of MemoryQueryResult found.
         """
         pass
 
     @abstractmethod
-    async def get_collections(self) -> List[str]:
+    async def get_collections(self) -> list[str]:
         """Get the list of collections in the memory (calls the memory store's get_collections method).
 
         Returns:
             List[str] -- The list of all the memory collection names.
         """
         pass
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-1.0.1/semantic_kernel/memory/volatile_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from copy import deepcopy
-from typing import Dict, List, Tuple
 
 from numpy import array, linalg, ndarray
 
 from semantic_kernel.exceptions import ServiceResourceNotFoundError
 from semantic_kernel.memory.memory_record import MemoryRecord
 from semantic_kernel.memory.memory_store_base import MemoryStoreBase
+from semantic_kernel.utils.experimental_decorator import experimental_class
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
+@experimental_class
 class VolatileMemoryStore(MemoryStoreBase):
-    _store: Dict[str, Dict[str, MemoryRecord]]
+    _store: dict[str, dict[str, MemoryRecord]]
 
     def __init__(self) -> None:
         """Initializes a new instance of the VolatileMemoryStore class."""
         self._store = {}
 
     async def create_collection(self, collection_name: str) -> None:
         """Creates a new collection if it does not exist.
@@ -32,15 +33,15 @@
         if collection_name in self._store:
             pass
         else:
             self._store[collection_name] = {}
 
     async def get_collections(
         self,
-    ) -> List[str]:
+    ) -> list[str]:
         """Gets the list of collections.
 
         Returns:
             List[str] -- The list of collections.
         """
         return list(self._store.keys())
 
@@ -80,15 +81,15 @@
         if collection_name not in self._store:
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         record._key = record._id
         self._store[collection_name][record._key] = record
         return record._key
 
-    async def upsert_batch(self, collection_name: str, records: List[MemoryRecord]) -> List[str]:
+    async def upsert_batch(self, collection_name: str, records: list[MemoryRecord]) -> list[str]:
         """Upserts a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to upsert the records into.
             records {List[MemoryRecord]} -- The records to upsert.
 
         Returns:
@@ -124,16 +125,16 @@
         if not with_embedding:
             # create copy of results without embeddings
             result = deepcopy(result)
             result._embedding = None
         return result
 
     async def get_batch(
-        self, collection_name: str, keys: List[str], with_embeddings: bool = False
-    ) -> List[MemoryRecord]:
+        self, collection_name: str, keys: list[str], with_embeddings: bool = False
+    ) -> list[MemoryRecord]:
         """Gets a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the records from.
             keys {List[str]} -- The unique database keys of the records.
             with_embeddings {bool} -- Whether to include the embeddings in the results. (default: {False})
 
@@ -166,15 +167,15 @@
             raise ServiceResourceNotFoundError(f"Collection '{collection_name}' does not exist")
 
         if key not in self._store[collection_name]:
             raise ServiceResourceNotFoundError(f"Key '{key}' not found in collection '{collection_name}'")
 
         del self._store[collection_name][key]
 
-    async def remove_batch(self, collection_name: str, keys: List[str]) -> None:
+    async def remove_batch(self, collection_name: str, keys: list[str]) -> None:
         """Removes a batch of records.
 
         Arguments:
             collection_name {str} -- The name of the collection to remove the records from.
             keys {List[str]} -- The unique database keys of the records to remove.
 
         Returns:
@@ -189,15 +190,15 @@
 
     async def get_nearest_match(
         self,
         collection_name: str,
         embedding: ndarray,
         min_relevance_score: float = 0.0,
         with_embedding: bool = False,
-    ) -> Tuple[MemoryRecord, float]:
+    ) -> tuple[MemoryRecord, float]:
         """Gets the nearest match to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest match from.
             embedding {ndarray} -- The embedding to find the nearest match to.
             min_relevance_score {float} -- The minimum relevance score of the match. (default: {0.0})
             with_embedding {bool} -- Whether to include the embedding in the result. (default: {False})
@@ -216,15 +217,15 @@
     async def get_nearest_matches(
         self,
         collection_name: str,
         embedding: ndarray,
         limit: int,
         min_relevance_score: float = 0.0,
         with_embeddings: bool = False,
-    ) -> List[Tuple[MemoryRecord, float]]:
+    ) -> list[tuple[MemoryRecord, float]]:
         """Gets the nearest matches to an embedding using cosine similarity.
 
         Arguments:
             collection_name {str} -- The name of the collection to get the nearest matches from.
             embedding {ndarray} -- The embedding to find the nearest matches to.
             limit {int} -- The maximum number of matches to return.
             min_relevance_score {float} -- The minimum relevance score of the matches. (default: {0.0})
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from __future__ import annotations
 
 import asyncio
 import logging
 import os
 from copy import copy
-from typing import Any, Optional
+from typing import Any
 
 import yaml
 
 from semantic_kernel.connectors.ai.function_call_behavior import FunctionCallBehavior
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIChatPromptExecutionSettings,
 )
@@ -55,15 +54,15 @@
 
 class FunctionCallingStepwisePlanner(KernelBaseModel):
     service_id: str
     options: FunctionCallingStepwisePlannerOptions
     generate_plan_yaml: str
     step_prompt: str
 
-    def __init__(self, service_id: str, options: Optional[FunctionCallingStepwisePlannerOptions] = None):
+    def __init__(self, service_id: str, options: FunctionCallingStepwisePlannerOptions | None = None):
         """Initialize a new instance of the FunctionCallingStepwisePlanner
 
         The FunctionCallingStepwisePlanner is a planner based on top of an OpenAI Chat Completion service
         (whether it be AzureOpenAI or OpenAI), so that we can use tools.
 
         If the options are configured to use callbacks to get the initial plan and the step prompt,
         the planner will use those provided callbacks to get that information. Otherwise it will
@@ -180,35 +179,37 @@
                 args = function_call_content.parse_arguments()
                 return FunctionCallingStepwisePlannerResult(
                     final_answer=args.get("answer", ""),
                     chat_history=chat_history_for_steps,
                     iterations=i + 1,
                 )
 
-            for content in chat_result.items:
-                if not isinstance(content, FunctionCallContent):
+            for item in chat_result.items:
+                if not isinstance(item, FunctionCallContent):
                     continue
                 try:
                     context = await chat_completion._process_function_call(
-                        function_call=content,
-                        result=chat_result,
+                        function_call=item,
                         kernel=cloned_kernel,
                         chat_history=chat_history_for_steps,
                         arguments=arguments,
                         function_call_count=1,
                         request_index=0,
                         function_call_behavior=prompt_execution_settings.function_call_behavior,
                     )
-                    frc = FunctionResultContent.from_function_call_content_and_result(
-                        function_call_content=content, result=context.function_result
-                    )
-                    chat_history_for_steps.add_message(message=frc.to_chat_message_content())
+                    if context is not None:
+                        # Only add the function result content to the chat history if the context is present
+                        # which means it wasn't added in the _process_function_call method
+                        frc = FunctionResultContent.from_function_call_content_and_result(
+                            function_call_content=item, result=context.function_result
+                        )
+                        chat_history_for_steps.add_message(message=frc.to_chat_message_content())
                 except Exception as exc:
                     frc = FunctionResultContent.from_function_call_content_and_result(
-                        function_call_content=content,
+                        function_call_content=item,
                         result=TextContent(text=f"An error occurred during planner invocation: {exc}"),
                     )
                     chat_history_for_steps.add_message(message=frc.to_chat_message_content())
                     continue
 
         # We're done, but the model hasn't returned a final answer.
         return FunctionCallingStepwisePlannerResult(
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/function_calling_stepwise_planner_options.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
-from typing import Any, Callable
+from collections.abc import Callable
+from typing import Any
 
 from pydantic import model_validator
 
 from semantic_kernel.connectors.ai.open_ai.prompt_execution_settings.open_ai_prompt_execution_settings import (
     OpenAIPromptExecutionSettings,
 )
 from semantic_kernel.planners.planner_options import PlannerOptions
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml` & `semantic_kernel-1.0.1/semantic_kernel/planners/function_calling_stepwise_planner/generate_plan.yaml`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/plan.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/plan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import re
 import threading
+from collections.abc import Callable
 from copy import copy
-from typing import Any, Callable, ClassVar, List, Optional, Union
+from typing import Any, ClassVar, Optional
 
 from pydantic import PrivateAttr
 
 from semantic_kernel import Kernel
 from semantic_kernel.connectors.ai import PromptExecutionSettings
 from semantic_kernel.exceptions import KernelInvokeException
 from semantic_kernel.functions.function_result import FunctionResult
@@ -18,18 +19,18 @@
 from semantic_kernel.utils.naming import generate_random_ascii_name
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class Plan:
     _state: KernelArguments = PrivateAttr()
-    _steps: List["Plan"] = PrivateAttr()
+    _steps: list["Plan"] = PrivateAttr()
     _function: KernelFunction = PrivateAttr()
     _parameters: KernelArguments = PrivateAttr()
-    _outputs: List[str] = PrivateAttr()
+    _outputs: list[str] = PrivateAttr()
     _has_next_step: bool = PrivateAttr()
     _next_step_index: int = PrivateAttr()
     _name: str = PrivateAttr()
     _plugin_name: str = PrivateAttr()
     _description: str = PrivateAttr()
     _is_prompt: bool = PrivateAttr()
     _prompt_execution_settings: PromptExecutionSettings = PrivateAttr()
@@ -40,15 +41,15 @@
         return self._name
 
     @property
     def state(self) -> KernelArguments:
         return self._state
 
     @property
-    def steps(self) -> List["Plan"]:
+    def steps(self) -> list["Plan"]:
         return self._steps
 
     @property
     def plugin_name(self) -> str:
         return self._plugin_name
 
     @property
@@ -84,23 +85,23 @@
 
     @property
     def next_step_index(self) -> int:
         return self._next_step_index
 
     def __init__(
         self,
-        name: Optional[str] = None,
-        plugin_name: Optional[str] = None,
-        description: Optional[str] = None,
-        next_step_index: Optional[int] = None,
-        state: Optional[KernelArguments] = None,
-        parameters: Optional[KernelArguments] = None,
-        outputs: Optional[List[str]] = None,
-        steps: Optional[List["Plan"]] = None,
-        function: Optional[KernelFunction] = None,
+        name: str | None = None,
+        plugin_name: str | None = None,
+        description: str | None = None,
+        next_step_index: int | None = None,
+        state: KernelArguments | None = None,
+        parameters: KernelArguments | None = None,
+        outputs: list[str] | None = None,
+        steps: list["Plan"] | None = None,
+        function: KernelFunction | None = None,
     ) -> None:
         self._name = f"plan_{generate_random_ascii_name()}" if name is None else name
         self._plugin_name = f"p_{generate_random_ascii_name()}" if plugin_name is None else plugin_name
         self._description = "" if description is None else description
         self._next_step_index = 0 if next_step_index is None else next_step_index
         self._state = KernelArguments() if state is None else state
         self._parameters = KernelArguments() if parameters is None else parameters
@@ -123,15 +124,15 @@
         plan = cls()
         plan.set_function(function)
         return plan
 
     async def invoke(
         self,
         kernel: Kernel,
-        arguments: Optional[KernelArguments] = None,
+        arguments: KernelArguments | None = None,
         # TODO: cancellation_token: CancellationToken,
     ) -> FunctionResult:
         """
         Invoke the plan asynchronously.
 
         Args:
             input (str, optional): The input to the plan. Defaults to None.
@@ -145,17 +146,15 @@
         """
         if not arguments:
             arguments = copy(self._state)
         if self._function is not None:
             try:
                 result = await self._function.invoke(kernel=kernel, arguments=arguments)
             except Exception as exc:
-                logger.error(
-                    "Something went wrong in plan step {0}.{1}:'{2}'".format(self._plugin_name, self._name, exc)
-                )
+                logger.error(f"Something went wrong in plan step {self._plugin_name}.{self._name}:'{exc}'")
                 raise KernelInvokeException(
                     "Error occurred while running plan step: " + str(exc),
                     exc,
                 ) from exc
             return result
         else:
             # loop through steps until completion
@@ -207,15 +206,15 @@
                 pass
         else:
             for step in plan.steps:
                 step = self.set_available_functions(step, kernel, arguments)
 
         return plan
 
-    def add_steps(self, steps: Union[List["Plan"], List[KernelFunction]]) -> None:
+    def add_steps(self, steps: list["Plan"] | list[KernelFunction]) -> None:
         for step in steps:
             if type(step) is Plan:
                 self._steps.append(step)
             else:
                 new_step = Plan(
                     name=step.name,
                     plugin_name=step.plugin_name,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_extensions.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/planner_extensions.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/planner_options.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/planner_options.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
-from __future__ import annotations
 
-from typing import Callable
+from collections.abc import Callable
 
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class PlannerOptions(KernelBaseModel):
     """The default planner options that planners inherit from"""
 
     excluded_plugins: set[str] = set()
     excluded_functions: set[str] = set()
-    get_available_functions: Callable[[PlannerOptions, str | None], list[KernelFunctionMetadata]] | None = None
+    get_available_functions: Callable[["PlannerOptions", str | None], list[KernelFunctionMetadata]] | None = None
     # TODO semantic_memory_config
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/config.json`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/Plugins/SequentialPlanning/skprompt.txt`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 CUR_DIR = os.path.dirname(os.path.realpath(__file__))
 PROMPT_CONFIG_FILE_PATH = os.path.join(CUR_DIR, "Plugins/SequentialPlanning/config.json")
 PROMPT_TEMPLATE_FILE_PATH = os.path.join(CUR_DIR, "Plugins/SequentialPlanning/skprompt.txt")
 
 
 def read_file(file_path: str) -> str:
-    with open(file_path, "r") as file:
+    with open(file_path) as file:
         return file.read()
 
 
 class SequentialPlanner:
     RESTRICTED_PLUGIN_NAME = "SequentialPlanner_Excluded"
 
     config: SequentialPlannerConfig
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_config.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Callable, List, Optional
+from collections.abc import Callable
 
 
 class SequentialPlannerConfig:
     def __init__(
         self,
-        relevancy_threshold: Optional[float] = None,
+        relevancy_threshold: float | None = None,
         max_relevant_functions: int = 100,
-        excluded_plugins: List[str] = None,
-        excluded_functions: List[str] = None,
-        included_functions: List[str] = None,
+        excluded_plugins: list[str] = None,
+        excluded_functions: list[str] = None,
+        included_functions: list[str] = None,
         max_tokens: int = 1024,
         allow_missing_functions: bool = False,
         get_available_functions: Callable = None,
         get_plugin_function: Callable = None,
     ):
         self.relevancy_threshold: float = relevancy_threshold
         self.max_relevant_functions: int = max_relevant_functions
-        self.excluded_plugins: List[str] = excluded_plugins or []
-        self.excluded_functions: List[str] = excluded_functions or []
-        self.included_functions: List[str] = included_functions or []
+        self.excluded_plugins: list[str] = excluded_plugins or []
+        self.excluded_functions: list[str] = excluded_functions or []
+        self.included_functions: list[str] = included_functions or []
         self.max_tokens: int = max_tokens
         self.allow_missing_functions: bool = allow_missing_functions
         self.get_available_functions = get_available_functions
         self.get_plugin_function = get_plugin_function
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_extensions.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List, Optional
 
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.kernel import Kernel
 from semantic_kernel.memory.memory_query_result import MemoryQueryResult
 from semantic_kernel.planners.sequential_planner.sequential_planner_config import SequentialPlannerConfig
 
@@ -52,15 +51,15 @@
         return "\n\n".join([SequentialPlannerFunctionExtension.to_manual_string(func) for func in functions])
 
     @staticmethod
     async def get_available_functions(
         kernel: Kernel,
         arguments: KernelArguments,
         config: SequentialPlannerConfig,
-        semantic_query: Optional[str] = None,
+        semantic_query: str | None = None,
     ):
         excluded_plugins = config.excluded_plugins or []
         excluded_functions = config.excluded_functions or []
         included_functions = config.included_functions or []
 
         available_functions = [
             func
@@ -87,29 +86,29 @@
         relevant_functions += [func for func in available_functions if func.name in missing_functions]
 
         return sorted(relevant_functions, key=lambda x: (x.plugin_name, x.name))
 
     @staticmethod
     async def get_relevant_functions(
         kernel: Kernel,
-        available_functions: List[KernelFunctionMetadata],
-        memories: Optional[List[MemoryQueryResult]] = None,
-    ) -> List[KernelFunctionMetadata]:
+        available_functions: list[KernelFunctionMetadata],
+        memories: list[MemoryQueryResult] | None = None,
+    ) -> list[KernelFunctionMetadata]:
         relevant_functions = []
         # TODO: cancellation
         if memories is None:
             return relevant_functions
         for memory_entry in memories:
             function = next(
                 (func for func in available_functions if func.fully_qualified_name == memory_entry.id),
                 None,
             )
             if function is not None:
                 logger.debug(
-                    "Found relevant function. Relevance Score: {0}, Function: {1}".format(
+                    "Found relevant function. Relevance Score: {}, Function: {}".format(
                         memory_entry.relevance,
                         function.fully_qualified_name,
                     )
                 )
                 relevant_functions.append(function)
 
         return relevant_functions
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py` & `semantic_kernel-1.0.1/semantic_kernel/planners/sequential_planner/sequential_planner_parser.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import re
-from typing import Callable, Optional, Tuple
+from collections.abc import Callable
 
 from defusedxml import ElementTree as ET
 
 from semantic_kernel.exceptions import PlannerInvalidPlanError
 from semantic_kernel.exceptions.kernel_exceptions import KernelFunctionNotFoundError, KernelPluginNotFoundError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
@@ -22,15 +22,15 @@
 
 class SequentialPlanParser:
     @staticmethod
     def to_plan_from_xml(
         xml_string: str,
         goal: str,
         kernel: Kernel,
-        get_plugin_function: Optional[Callable[[str, str], Optional[KernelFunction]]] = None,
+        get_plugin_function: Callable[[str, str], KernelFunction | None] | None = None,
         allow_missing_functions: bool = False,
     ):
         xml_string = "<xml>" + xml_string + "</xml>"
         try:
             xml_doc = ET.fromstring(xml_string)
         except ET.ParseError:
             # Attempt to parse <plan> out of it
@@ -107,12 +107,12 @@
                     plan._outputs.append(result)
 
                 plan.add_steps([plan_step])
 
         return plan
 
     @staticmethod
-    def get_plugin_function_names(plugin_function_name: str) -> Tuple[str, str]:
+    def get_plugin_function_names(plugin_function_name: str) -> tuple[str, str]:
         plugin_function_name_parts = plugin_function_name.split("-")
         plugin_name = plugin_function_name_parts[0] if len(plugin_function_name_parts) > 0 else ""
         function_name = plugin_function_name_parts[1] if len(plugin_function_name_parts) > 1 else plugin_function_name
         return plugin_name, function_name
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/__init__.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/const.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/const.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/handlebars_prompt_template.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/handlebars_prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Optional
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any, Optional
 
 from pybars import Compiler, PybarsError
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import HandlebarsTemplateRenderException, HandlebarsTemplateSyntaxError
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import HANDLEBARS_TEMPLATE_FORMAT_NAME
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/input_variable.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/input_variable.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import Any, Optional
+from typing import Any
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
 class InputVariable(KernelBaseModel):
     """Input variable for a prompt template.
 
@@ -15,12 +15,12 @@
         is_required: Whether the input variable is required.
         json_schema: The JSON schema for the input variable.
         allow_dangerously_set_content (default: false): Allow content without encoding, this controls
             if this variable is encoded before use.
     """
 
     name: str
-    description: Optional[str] = ""
-    default: Optional[Any] = ""
-    is_required: Optional[bool] = True
-    json_schema: Optional[str] = ""
+    description: str | None = ""
+    default: Any | None = ""
+    is_required: bool | None = True
+    json_schema: str | None = ""
     allow_dangerously_set_content: bool = False
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/jinja2_prompt_template.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/jinja2_prompt_template.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Optional
+from collections.abc import Callable
+from typing import TYPE_CHECKING, Any, Optional
 
 from jinja2 import BaseLoader, TemplateError
 from jinja2.sandbox import ImmutableSandboxedEnvironment
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import Jinja2TemplateRenderException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/kernel_prompt_template.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/kernel_prompt_template.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from html import escape
-from typing import TYPE_CHECKING, Any, List, Optional
+from typing import TYPE_CHECKING, Any, Optional
 
 from pydantic import PrivateAttr, field_validator
 
 from semantic_kernel.exceptions import TemplateRenderException
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME
 from semantic_kernel.prompt_template.input_variable import InputVariable
@@ -33,15 +33,15 @@
             This reverts the behavior to unencoded input.
 
     Raises:
         ValueError: If the template format is not 'semantic-kernel'
         TemplateSyntaxError: If the template has a syntax error
     """
 
-    _blocks: List[Block] = PrivateAttr(default_factory=list)
+    _blocks: list[Block] = PrivateAttr(default_factory=list)
 
     @field_validator("prompt_template_config")
     @classmethod
     def validate_template_format(cls, v: "PromptTemplateConfig") -> "PromptTemplateConfig":
         if v.template_format != KERNEL_TEMPLATE_FORMAT_NAME:
             raise ValueError(f"Invalid prompt template format: {v.template_format}. Expected: semantic-kernel")
         return v
@@ -67,21 +67,21 @@
                     if sub_block.type == BlockTypes.NAMED_ARG and sub_block.variable:
                         # Add all variables from named arguments, e.g. "{{p.bar b = $b}}".
                         # represents a named argument for a function call.
                         # For example, in the template {{ MyPlugin.MyFunction var1=$boo }}, var1=$boo
                         # is a named arg block.
                         self._add_if_missing(sub_block.variable.name, seen)
 
-    def _add_if_missing(self, variable_name: str, seen: Optional[set] = None):
+    def _add_if_missing(self, variable_name: str, seen: set | None = None):
         # Convert variable_name to lower case to handle case-insensitivity
         if variable_name and variable_name.lower() not in seen:
             seen.add(variable_name.lower())
             self.prompt_template_config.input_variables.append(InputVariable(name=variable_name))
 
-    def extract_blocks(self) -> List[Block]:
+    def extract_blocks(self) -> list[Block]:
         """
         Given a prompt template string, extract all the blocks
         (text, variables, function calls).
 
         Args:
             template_text: Prompt template
 
@@ -107,27 +107,27 @@
         Returns:
             The prompt template ready to be used for an AI request
         """
         if arguments is None:
             arguments = KernelArguments()
         return await self.render_blocks(self._blocks, kernel, arguments)
 
-    async def render_blocks(self, blocks: List[Block], kernel: "Kernel", arguments: "KernelArguments") -> str:
+    async def render_blocks(self, blocks: list[Block], kernel: "Kernel", arguments: "KernelArguments") -> str:
         """
         Given a list of blocks render each block and compose the final result.
 
         :param blocks: Template blocks generated by ExtractBlocks
         :param context: Access into the current kernel execution context
         :return: The prompt template ready to be used for an AI request
         """
         from semantic_kernel.template_engine.protocols.code_renderer import CodeRenderer
         from semantic_kernel.template_engine.protocols.text_renderer import TextRenderer
 
         logger.debug(f"Rendering list of {len(blocks)} blocks")
-        rendered_blocks: List[str] = []
+        rendered_blocks: list[str] = []
 
         arguments = self._get_trusted_arguments(arguments)
         allow_unsafe_function_output = self._get_allow_unsafe_function_output()
         for block in blocks:
             if isinstance(block, TextRenderer):
                 rendered_blocks.append(block.render(kernel, arguments))
                 continue
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_base.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/prompt_template_config.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/prompt_template_config.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 import logging
-from typing import Dict, List, Optional, TypeVar, Union
+from typing import TypeVar
 
 from pydantic import Field, field_validator, model_validator
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.functions.kernel_parameter_metadata import KernelParameterMetadata
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.prompt_template.const import KERNEL_TEMPLATE_FORMAT_NAME, TEMPLATE_FORMAT_TYPES
@@ -27,37 +27,35 @@
         allow_dangerously_set_content (default: false): Allow content without encoding, this controls
             if the output of functions called in the template is encoded before use.
         execution_settings: The execution settings for the prompt.
 
     """
 
     name: str = ""
-    description: Optional[str] = ""
-    template: Optional[str] = None
+    description: str | None = ""
+    template: str | None = None
     template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME
-    input_variables: List[InputVariable] = Field(default_factory=list)
+    input_variables: list[InputVariable] = Field(default_factory=list)
     allow_dangerously_set_content: bool = False
-    execution_settings: Dict[str, PromptExecutionSettings] = Field(default_factory=dict)
+    execution_settings: dict[str, PromptExecutionSettings] = Field(default_factory=dict)
 
     @model_validator(mode="after")
     def check_input_variables(self):
         """Verify that input variable default values are string only"""
         for variable in self.input_variables:
             if variable.default and not isinstance(variable.default, str):
-                raise ValueError(f"Default value for input variable {variable.name} must be a string.")
+                raise TypeError(f"Default value for input variable {variable.name} must be a string.")
         return self
 
     @field_validator("execution_settings", mode="before")
     @classmethod
     def rewrite_execution_settings(
         cls,
-        settings: Optional[
-            Union[PromptExecutionSettings, List[PromptExecutionSettings], Dict[str, PromptExecutionSettings]]
-        ],
-    ) -> Dict[str, PromptExecutionSettings]:
+        settings: None | (PromptExecutionSettings | list[PromptExecutionSettings] | dict[str, PromptExecutionSettings]),
+    ) -> dict[str, PromptExecutionSettings]:
         """Rewrite execution settings to a dictionary."""
         if not settings:
             return {}
         if isinstance(settings, PromptExecutionSettings):
             return {settings.service_id or "default": settings}
         if isinstance(settings, list):
             return {s.service_id or "default": s for s in settings}
@@ -66,15 +64,15 @@
     def add_execution_settings(self, settings: PromptExecutionSettings, overwrite: bool = True) -> None:
         """Add execution settings to the prompt template."""
         if settings.service_id in self.execution_settings and not overwrite:
             return
         self.execution_settings[settings.service_id or "default"] = settings
         logger.warning("Execution settings already exist and overwrite is set to False")
 
-    def get_kernel_parameter_metadata(self) -> List[KernelParameterMetadata]:
+    def get_kernel_parameter_metadata(self) -> list[KernelParameterMetadata]:
         """Get the kernel parameter metadata for the input variables."""
         return [
             KernelParameterMetadata(
                 name=variable.name,
                 description=variable.description,
                 default_value=variable.default,
                 type_=variable.json_schema,  # TODO: update to handle complex JSON schemas
@@ -86,29 +84,29 @@
     @classmethod
     def from_json(cls, json_str: str) -> "PromptTemplateConfig":
         """Create a PromptTemplateConfig instance from a JSON string."""
         if not json_str:
             raise ValueError("json_str is empty")
         try:
             return cls.model_validate_json(json_str)
-        except Exception as e:
+        except Exception as exc:
             raise ValueError(
                 "Unable to deserialize PromptTemplateConfig from the "
-                f"specified JSON string: {json_str} with exception: {e}"
-            )
+                f"specified JSON string: {json_str} with exception: {exc}"
+            ) from exc
 
     @classmethod
     def restore(
         cls,
         name: str,
         description: str,
         template: str,
         template_format: TEMPLATE_FORMAT_TYPES = KERNEL_TEMPLATE_FORMAT_NAME,
-        input_variables: List[InputVariable] = [],
-        execution_settings: Dict[str, PromptExecutionSettings] = {},
+        input_variables: list[InputVariable] = [],
+        execution_settings: dict[str, PromptExecutionSettings] = {},
         allow_dangerously_set_content: bool = False,
     ) -> "PromptTemplateConfig":
         """Restore a PromptTemplateConfig instance from the specified parameters.
 
         Args:
             name: The name of the prompt template.
             description: The description of the prompt template.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/handlebars_system_helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import json
 import logging
 import re
+from collections.abc import Callable
 from enum import Enum
-from typing import Callable, Dict
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _messages(this, options, *args, **kwargs):
     from semantic_kernel.contents.chat_history import ChatHistory
 
@@ -36,15 +36,15 @@
             value = value.value
         if value is not None:
             start += f' {key}="{value}"'
     start += ">"
     end = f"</{CHAT_MESSAGE_CONTENT_TAG}>"
     try:
         content = options["fn"](this)
-    except Exception:
+    except Exception:  # pragma: no cover
         content = ""
     return f"{start}{content}{end}"
 
 
 def _set(this, *args, **kwargs):
     if "name" in kwargs and "value" in kwargs:
         this.context[kwargs["name"]] = kwargs["value"]
@@ -138,15 +138,15 @@
     arg = args[0]
     arg = re.sub(r"([A-Z]+)([A-Z][a-z])", r"\1_\2", arg)
     arg = re.sub(r"([a-z\d])([A-Z])", r"\1_\2", arg)
     arg = arg.replace("-", "_")
     return arg.lower()
 
 
-HANDLEBAR_SYSTEM_HELPERS: Dict[str, Callable] = {
+HANDLEBAR_SYSTEM_HELPERS: dict[str, Callable] = {
     "set": _set,
     "get": _get,
     "array": _array,
     "range": _range,
     "concat": _concat,
     "or": _or,
     "add": _add,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/jinja2_system_helpers.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 import re
+from collections.abc import Callable
 from enum import Enum
-from typing import Callable, Dict
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 def _messages(chat_history):
     from semantic_kernel.contents.chat_history import ChatHistory
 
@@ -57,15 +57,14 @@
 
 def _double_close():
     """Returns the string representing double close braces."""
     return "}}"
 
 
 def _array(*args, **kwargs):
-    print(f"Received args: {args}")
     return list(args)
 
 
 def _camel_case(*args, **kwargs):
     return "".join([word.capitalize() for word in args[0].split("_")])
 
 
@@ -73,15 +72,15 @@
     arg = args[0]
     arg = re.sub(r"([A-Z]+)([A-Z][a-z])", r"\1_\2", arg)
     arg = re.sub(r"([a-z\d])([A-Z])", r"\1_\2", arg)
     arg = arg.replace("-", "_")
     return arg.lower()
 
 
-JINJA2_SYSTEM_HELPERS: Dict[str, Callable] = {
+JINJA2_SYSTEM_HELPERS: dict[str, Callable] = {
     "get": _safe_get_wrapper,
     "double_open": _double_open,
     "doubleOpen": _double_open,
     "double_close": _double_close,
     "doubleClose": _double_close,
     "message": _message,
     "message_to_prompt": _message_to_prompt,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/prompt_template/utils/template_function_helpers.py` & `semantic_kernel-1.0.1/semantic_kernel/prompt_template/utils/template_function_helpers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import logging
+from collections.abc import Callable
 from html import escape
-from typing import TYPE_CHECKING, Any, Callable, Literal
+from typing import TYPE_CHECKING, Any, Literal
 
 import nest_asyncio
 
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.prompt_template.const import HANDLEBARS_TEMPLATE_FORMAT_NAME
 
 if TYPE_CHECKING:
@@ -28,15 +29,15 @@
     """Create a helper function for both the Handlebars and Jinja2 templating engines from a kernel function."""
     if not getattr(asyncio, "_nest_patched", False):
         nest_asyncio.apply()
 
     def func(*args, **kwargs):
         arguments = KernelArguments()
         if base_arguments and base_arguments.execution_settings:
-            arguments.execution_settings = base_arguments.execution_settings
+            arguments.execution_settings = base_arguments.execution_settings  # pragma: no cover
         arguments.update(base_arguments)
         arguments.update(kwargs)
 
         if len(args) > 0 and template_format == HANDLEBARS_TEMPLATE_FORMAT_NAME:
             this = args[0]
             actual_args = args[1:]
         else:
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-1.0.1/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import Awaitable, Callable, TypeVar
+from collections.abc import Awaitable, Callable
+from typing import TypeVar
 
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
 
 T = TypeVar("T")
 
 logger: logging.Logger = logging.getLogger(__name__)
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-1.0.1/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from abc import ABC, abstractmethod
-from typing import Awaitable, Callable, TypeVar
+from collections.abc import Awaitable, Callable
+from typing import TypeVar
 
 T = TypeVar("T")
 
 logger: logging.Logger = logging.getLogger(__name__)
 
 
 class RetryMechanismBase(ABC):
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_client_base.py` & `semantic_kernel-1.0.1/semantic_kernel/services/ai_service_client_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-import sys
 from abc import ABC
-from typing import Optional
-
-if sys.version_info >= (3, 9):
-    from typing import Annotated
-else:
-    from typing_extensions import Annotated
+from typing import Annotated
 
 from pydantic import Field, StringConstraints
 
 from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.kernel_pydantic import KernelBaseModel
 
 
@@ -25,15 +19,15 @@
 
     The service_id is used in Semantic Kernel to identify the service, if empty the ai_model_id is used.
     """
 
     ai_model_id: Annotated[str, StringConstraints(strip_whitespace=True, min_length=1)]
     service_id: str = Field("")
 
-    def model_post_init(self, __context: Optional[object] = None):
+    def model_post_init(self, __context: object | None = None):
         """Update the service_id if it is not set."""
         if not self.service_id:
             self.service_id = self.ai_model_id
 
     def get_prompt_execution_settings_class(self) -> "PromptExecutionSettings":
         """Get the request settings class."""
         return PromptExecutionSettings  # pragma: no cover
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/services/ai_service_selector.py` & `semantic_kernel-1.0.1/semantic_kernel/services/ai_service_selector.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,51 +1,56 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import TYPE_CHECKING, Tuple, Union
+from typing import TYPE_CHECKING
 
-from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
 from semantic_kernel.exceptions import KernelServiceNotFoundError
-from semantic_kernel.functions.kernel_arguments import KernelArguments
 
 if TYPE_CHECKING:
-    from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
-    from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+    from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+    from semantic_kernel.functions.kernel_arguments import KernelArguments
     from semantic_kernel.functions.kernel_function import KernelFunction
-    from semantic_kernel.kernel import Kernel
-
-    ALL_COMPLETION_SERVICE_TYPES = Union[TextCompletionClientBase, ChatCompletionClientBase]
+    from semantic_kernel.kernel import AI_SERVICE_CLIENT_TYPE, Kernel
 
 
 class AIServiceSelector:
     """Default service selector, can be subclassed and overridden.
 
     To use a custom service selector, subclass this class and override the select_ai_service method.
     Make sure that the function signature stays the same.
     """
 
     def select_ai_service(
-        self, kernel: "Kernel", function: "KernelFunction", arguments: KernelArguments
-    ) -> Tuple["ALL_COMPLETION_SERVICE_TYPES", PromptExecutionSettings]:
+        self,
+        kernel: "Kernel",
+        function: "KernelFunction",
+        arguments: "KernelArguments",
+        type_: type["AI_SERVICE_CLIENT_TYPE"] | None = None,
+    ) -> tuple["AI_SERVICE_CLIENT_TYPE", "PromptExecutionSettings"]:
         """Select a AI Service on a first come, first served basis,
         starting with execution settings in the arguments,
         followed by the execution settings from the function.
         If the same service_id is in both, the one in the arguments will be used.
         """
-        from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
-        from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+        if type_ is None:
+            from semantic_kernel.connectors.ai.chat_completion_client_base import ChatCompletionClientBase
+            from semantic_kernel.connectors.ai.text_completion_client_base import TextCompletionClientBase
+
+            type_ = (TextCompletionClientBase, ChatCompletionClientBase)
 
         execution_settings_dict = arguments.execution_settings or {}
         if func_exec_settings := getattr(function, "prompt_execution_settings", None):
             for id, settings in func_exec_settings.items():
                 if id not in execution_settings_dict:
                     execution_settings_dict[id] = settings
         if not execution_settings_dict:
+            from semantic_kernel.connectors.ai.prompt_execution_settings import PromptExecutionSettings
+
             execution_settings_dict = {"default": PromptExecutionSettings()}
         for service_id, settings in execution_settings_dict.items():
             try:
-                service = kernel.get_service(service_id, type=(TextCompletionClientBase, ChatCompletionClientBase))
+                service = kernel.get_service(service_id, type=type_)
             except KernelServiceNotFoundError:
                 continue
             if service:
                 service_settings = service.get_prompt_execution_settings_from_settings(settings)
                 return service, service_settings
         raise KernelServiceNotFoundError("No service found.")
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/README.md` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from copy import copy
-from typing import TYPE_CHECKING, Any, ClassVar, List
+from typing import TYPE_CHECKING, Any, ClassVar
 
 from pydantic import Field, field_validator, model_validator
 
-from semantic_kernel.const import METADATA_EXCEPTION_KEY
 from semantic_kernel.exceptions import CodeBlockRenderException, CodeBlockTokenError
 from semantic_kernel.exceptions.kernel_exceptions import KernelFunctionNotFoundError, KernelPluginNotFoundError
 from semantic_kernel.functions.kernel_function_metadata import KernelFunctionMetadata
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.code_tokenizer import CodeTokenizer
 
@@ -44,15 +43,15 @@
         CodeBlockRenderError: If the plugin collection is not set in the kernel.
         CodeBlockRenderError: If the function is not found in the plugin collection.
         CodeBlockRenderError: If the function does not take any arguments but it is being
             called in the template with arguments.
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.CODE
-    tokens: List[Block] = Field(default_factory=list)
+    tokens: list[Block] = Field(default_factory=list)
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: Any) -> Any:
         """Parse the content of the code block and tokenize it.
 
         If tokens are already present, skip the tokenizing.
@@ -60,15 +59,15 @@
         if isinstance(fields, Block) or "tokens" in fields:
             return fields
         content = fields.get("content", "").strip()
         fields["tokens"] = CodeTokenizer.tokenize(content)
         return fields
 
     @field_validator("tokens", mode="after")
-    def check_tokens(cls, tokens: List[Block]) -> List[Block]:
+    def check_tokens(cls, tokens: list[Block]) -> list[Block]:
         """Check the tokens in the list.
 
         If the first token is a value or variable, the rest of the tokens will be ignored.
         If the first token is a function_id, then the next token can be a value,
             variable or named_arg, the rest have to be named_args.
 
         Raises:
@@ -121,19 +120,20 @@
             error_msg = f"Function `{function_block.content}` not found"
             logger.error(error_msg)
             raise CodeBlockRenderException(error_msg) from exc
 
         arguments_clone = copy(arguments)
         if len(self.tokens) > 1:
             arguments_clone = self._enrich_function_arguments(kernel, arguments_clone, function.metadata)
-
-        result = await function.invoke(kernel, arguments_clone)
-        if exc := result.metadata.get(METADATA_EXCEPTION_KEY, None):
-            raise CodeBlockRenderException(f"Error rendering function: {function.metadata} with error: {exc}") from exc
-
+        try:
+            result = await function.invoke(kernel, arguments_clone)
+        except Exception as exc:
+            error_msg = f"Error invoking function `{function_block.content}`"
+            logger.error(error_msg)
+            raise CodeBlockRenderException(error_msg) from exc
         return str(result) if result else ""
 
     def _enrich_function_arguments(
         self,
         kernel: "Kernel",
         arguments: "KernelArguments",
         function_metadata: KernelFunctionMetadata,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from re import compile
-from typing import TYPE_CHECKING, Any, ClassVar, Dict, Optional, Tuple
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
 from pydantic import model_validator
 
 from semantic_kernel.exceptions import FunctionIdBlockSyntaxError
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 
@@ -35,20 +35,20 @@
         plugin_name (Optional[str], optional): The plugin name.
 
     Raises:
         ValueError: If the content does not have valid syntax.
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.FUNCTION_ID
-    function_name: Optional[str] = ""
-    plugin_name: Optional[str] = None
+    function_name: str | None = ""
+    plugin_name: str | None = None
 
     @model_validator(mode="before")
     @classmethod
-    def parse_content(cls, fields: Dict[str, Any]) -> Dict[str, Any]:
+    def parse_content(cls, fields: dict[str, Any]) -> dict[str, Any]:
         """Parse the content of the function id block and extract the plugin and function name.
 
         If both are present in the fields, return the fields as is.
         Otherwise use the regex to extract the plugin and function name.
         """
         if "plugin_name" in fields and "function_name" in fields:
             return fields
@@ -57,9 +57,9 @@
         if not matches:
             raise FunctionIdBlockSyntaxError(content=content)
         if plugin := matches.groupdict().get("plugin"):
             fields["plugin_name"] = plugin
         fields["function_name"] = matches.group("function")
         return fields
 
-    def render(self, *_: Tuple["Kernel", Optional["KernelArguments"]]) -> str:
+    def render(self, *_: tuple["Kernel", Optional["KernelArguments"]]) -> str:
         return self.content
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/named_arg_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/named_arg_block.py`

 * *Files 7% similar despite different names*

```diff
@@ -51,17 +51,17 @@
 
     Raises:
         NamedArgBlockSyntaxError: If the content does not match the named argument syntax.
 
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.NAMED_ARG
-    name: Optional[str] = None
-    value: Optional[ValBlock] = None
-    variable: Optional[VarBlock] = None
+    name: str | None = None
+    value: ValBlock | None = None
+    variable: VarBlock | None = None
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: Any) -> Any:
         """Parse the content of the named argument block and extract the name and value.
 
         If the name and either value or variable is present the parsing is skipped.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import TYPE_CHECKING, ClassVar, Optional, Tuple
+from typing import TYPE_CHECKING, ClassVar, Optional
 
 from pydantic import field_validator
 
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 
 if TYPE_CHECKING:
@@ -23,17 +23,17 @@
     def content_strip(cls, content: str):
         # overload strip method text blocks are not stripped.
         return content
 
     @classmethod
     def from_text(
         cls,
-        text: Optional[str] = None,
-        start_index: Optional[int] = None,
-        stop_index: Optional[int] = None,
+        text: str | None = None,
+        start_index: int | None = None,
+        stop_index: int | None = None,
     ):
         if text is None:
             return cls(content="")
         if start_index is not None and stop_index is not None:
             if start_index > stop_index:
                 raise ValueError(f"start_index ({start_index}) must be less than " f"stop_index ({stop_index})")
 
@@ -44,9 +44,9 @@
         elif start_index is not None:
             text = text[start_index:]
         elif stop_index is not None:
             text = text[:stop_index]
 
         return cls(content=text)
 
-    def render(self, *_: Tuple[Optional["Kernel"], Optional["KernelArguments"]]) -> str:
+    def render(self, *_: tuple[Optional["Kernel"], Optional["KernelArguments"]]) -> str:
         return self.content
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
 from re import S, compile
-from typing import TYPE_CHECKING, Any, ClassVar, Optional, Tuple
+from typing import TYPE_CHECKING, Any, ClassVar, Optional
 
 from pydantic import model_validator
 
 from semantic_kernel.exceptions import ValBlockSyntaxError
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 
@@ -42,16 +42,16 @@
 
     Raises:
         ValBlockSyntaxError: If the content does not match the value block syntax.
 
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.VALUE
-    value: Optional[str] = ""
-    quote: Optional[str] = "'"
+    value: str | None = ""
+    quote: str | None = "'"
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: Any) -> Any:
         """Parse the content and extract the value and quote.
 
         The parsing is based on a regex that returns the value and quote.
@@ -65,9 +65,9 @@
             raise ValBlockSyntaxError(content=content)
         if value := matches.groupdict().get("value"):
             fields["value"] = value
         if quote := matches.groupdict().get("quote"):
             fields["quote"] = quote
         return fields
 
-    def render(self, *_: Tuple["Kernel", Optional["KernelArguments"]]) -> str:
+    def render(self, *_: tuple["Kernel", Optional["KernelArguments"]]) -> str:
         return self.value
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
     Raises:
         VarBlockSyntaxError: If the content does not match the variable syntax.
 
     """
 
     type: ClassVar[BlockTypes] = BlockTypes.VARIABLE
-    name: Optional[str] = ""
+    name: str | None = ""
 
     @model_validator(mode="before")
     @classmethod
     def parse_content(cls, fields: Any) -> Any:
         """Parse the content and extract the name.
 
         The parsing is based on a regex that returns the name.
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List
 
 from semantic_kernel.exceptions import CodeBlockSyntaxError
 from semantic_kernel.template_engine.blocks.block import Block
 from semantic_kernel.template_engine.blocks.block_types import BlockTypes
 from semantic_kernel.template_engine.blocks.function_id_block import FunctionIdBlock
 from semantic_kernel.template_engine.blocks.named_arg_block import NamedArgBlock
 from semantic_kernel.template_engine.blocks.symbols import Symbols
@@ -21,36 +20,36 @@
 #                         | [function-call] " " [template]
 # [variable]       ::= "$" [valid-name]
 # [value]          ::= "'" [text] "'" | '"' [text] '"'
 # [function-call]  ::= [function-id] | [function-id] [parameter]
 # [parameter]      ::= [variable] | [value]
 class CodeTokenizer:
     @staticmethod
-    def tokenize(text: str) -> List[Block]:
+    def tokenize(text: str) -> list[Block]:
         # Remove spaces, which are ignored anyway
         text = text.strip() if text else ""
         # Render None/empty to []
         if not text:
             return []
         # 1 char only edge case, var and val blocks are invalid with one char, so it must be a function id block
         if len(text) == 1:
             return [FunctionIdBlock(content=text)]
 
         # Track what type of token we're reading
         current_token_type = None
 
         # Track the content of the current token
-        current_token_content: List[str] = []
+        current_token_content: list[str] = []
 
         # Other state we need to track
         text_value_delimiter = None
         space_separator_found = False
         skip_next_char = False
         next_char = ""
-        blocks: List[Block] = []
+        blocks: list[Block] = []
 
         for index, current_char in enumerate(text[:-1]):
             next_char = text[index + 1]
 
             if skip_next_char:
                 skip_next_char = False
                 continue
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-1.0.1/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import logging
-from typing import List
 
 from semantic_kernel.exceptions import (
     BlockSyntaxError,
     CodeBlockTokenError,
     TemplateSyntaxError,
 )
 from semantic_kernel.template_engine.blocks.block import Block
@@ -24,15 +23,15 @@
 # [sk-block]       ::= "{{" [variable] "}}"
 #                      | "{{" [value] "}}"
 #                      | "{{" [function-call] "}}"
 # [text-block]     ::= [any-char] | [any-char] [text-block]
 # [any-char]       ::= any char
 class TemplateTokenizer:
     @staticmethod
-    def tokenize(text: str) -> List[Block]:
+    def tokenize(text: str) -> list[Block]:
         code_tokenizer = CodeTokenizer()
         # An empty block consists of 4 chars: "{{}}"
         EMPTY_CODE_BLOCK_LENGTH = 4
         # A block shorter than 5 chars is either empty or
         # invalid, e.g. "{{ }}" and "{{$}}"
         MIN_CODE_BLOCK_LENGTH = EMPTY_CODE_BLOCK_LENGTH + 1
 
@@ -42,15 +41,15 @@
         if not text:
             return [TextBlock.from_text("")]
 
         # If the template is "empty" return it as a text block
         if len(text) < MIN_CODE_BLOCK_LENGTH:
             return [TextBlock.from_text(text)]
 
-        blocks: List[Block] = []
+        blocks: list[Block] = []
         end_of_last_block = 0
         block_start_pos = 0
         block_start_found = False
         inside_text_value = False
         text_value_delimiter = None
         skip_next_char = False
 
@@ -107,26 +106,26 @@
             blocks.append(TextBlock.from_text(text, end_of_last_block, len(text)))
 
         return blocks
 
     @staticmethod
     def _extract_blocks(
         text: str, code_tokenizer: CodeTokenizer, block_start_pos: int, end_of_last_block: int, next_char_pos: int
-    ) -> List[Block]:
+    ) -> list[Block]:
         """Extract the blocks from the found code.
 
         If there is text before the current block, create a TextBlock from that.
 
         If the block is empty, return a TextBlock with the delimiters.
 
         If the block is not empty, tokenize it and return the result.
         If there is only a variable or value in the code block,
         return just that, instead of the CodeBlock.
         """
-        new_blocks: List[Block] = []
+        new_blocks: list[Block] = []
         if block_start_pos > end_of_last_block:
             new_blocks.append(
                 TextBlock.from_text(
                     text,
                     end_of_last_block,
                     block_start_pos,
                 )
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/text/function_extension.py` & `semantic_kernel-1.0.1/semantic_kernel/text/function_extension.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from typing import List
 
 from semantic_kernel.functions.kernel_arguments import KernelArguments
 from semantic_kernel.functions.kernel_function import KernelFunction
 from semantic_kernel.kernel import Kernel
 
 
 async def aggregate_chunked_results(
-    func: KernelFunction, chunked_results: List[str], kernel: Kernel, arguments: KernelArguments
+    func: KernelFunction, chunked_results: list[str], kernel: Kernel, arguments: KernelArguments
 ) -> str:
     """
     Aggregate the results from the chunked results.
     """
     results = []
     for chunk in chunked_results:
         arguments["input"] = chunk
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/text/text_chunker.py` & `semantic_kernel-1.0.1/semantic_kernel/text/text_chunker.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 Split text in chunks, attempting to leave meaning intact.
 For plain text, split looking at new lines first, then periods, and so on.
 For markdown, split looking at punctuation first, and so on.
 """
 
 import os
 import re
-from typing import Callable, List, Tuple
+from collections.abc import Callable
 
 NEWLINE = os.linesep
 
 TEXT_SPLIT_OPTIONS = [
     ["\n", "\r"],
     ["."],
     ["?", "!"],
@@ -45,41 +45,41 @@
     TODO: chunking methods should be configurable to allow for different
           tokenization strategies depending on the model to be called.
           For now, we use an extremely rough estimate.
     """
     return len(text) // 4
 
 
-def split_plaintext_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> List[str]:
+def split_plaintext_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> list[str]:
     """
     Split plain text into lines.
     it will split on new lines first, and then on punctuation.
     """
     return _split_text_lines(
         text=text,
         max_token_per_line=max_token_per_line,
         trim=True,
         token_counter=token_counter,
     )
 
 
-def split_markdown_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> List[str]:
+def split_markdown_lines(text: str, max_token_per_line: int, token_counter: Callable = _token_counter) -> list[str]:
     """
     Split markdown into lines.
     It will split on punctuation first, and then on space and new lines.
     """
     return _split_markdown_lines(
         text=text,
         max_token_per_line=max_token_per_line,
         trim=True,
         token_counter=token_counter,
     )
 
 
-def split_plaintext_paragraph(text: List[str], max_tokens: int, token_counter: Callable = _token_counter) -> List[str]:
+def split_plaintext_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
     """
     Split plain text into paragraphs.
     """
 
     split_lines = []
     for line in text:
         split_lines.extend(
@@ -90,15 +90,15 @@
                 token_counter=token_counter,
             )
         )
 
     return _split_text_paragraph(text=split_lines, max_tokens=max_tokens, token_counter=token_counter)
 
 
-def split_markdown_paragraph(text: List[str], max_tokens: int, token_counter: Callable = _token_counter) -> List[str]:
+def split_markdown_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
     """
     Split markdown into paragraphs.
     """
     split_lines = []
     for line in text:
         split_lines.extend(
             _split_markdown_lines(
@@ -108,15 +108,15 @@
                 token_counter=token_counter,
             )
         )
 
     return _split_text_paragraph(text=split_lines, max_tokens=max_tokens, token_counter=token_counter)
 
 
-def _split_text_paragraph(text: List[str], max_tokens: int, token_counter: Callable = _token_counter) -> List[str]:
+def _split_text_paragraph(text: list[str], max_tokens: int, token_counter: Callable = _token_counter) -> list[str]:
     """
     Split text into paragraphs.
     """
     if not text:
         return []
 
     paragraphs = []
@@ -160,15 +160,15 @@
 
 
 def _split_markdown_lines(
     text: str,
     max_token_per_line: int,
     trim: bool,
     token_counter: Callable = _token_counter,
-) -> List[str]:
+) -> list[str]:
     """
     Split markdown into lines.
     """
 
     return _split_str_lines(
         text=text,
         max_tokens=max_token_per_line,
@@ -179,15 +179,15 @@
 
 
 def _split_text_lines(
     text: str,
     max_token_per_line: int,
     trim: bool,
     token_counter: Callable = _token_counter,
-) -> List[str]:
+) -> list[str]:
     """
     Split text into lines.
     """
 
     return _split_str_lines(
         text=text,
         max_tokens=max_token_per_line,
@@ -196,18 +196,18 @@
         token_counter=token_counter,
     )
 
 
 def _split_str_lines(
     text: str,
     max_tokens: int,
-    separators: List[List[str]],
+    separators: list[list[str]],
     trim: bool,
     token_counter: Callable = _token_counter,
-) -> List[str]:
+) -> list[str]:
     if not text:
         return []
 
     text = text.replace("\r\n", "\n")
     lines = []
     was_split = False
     for split_option in separators:
@@ -224,32 +224,32 @@
                 text=lines,
                 max_tokens=max_tokens,
                 separators=split_option,
                 trim=trim,
                 token_counter=token_counter,
             )
         if was_split:
-            break
+            break  # pragma: no cover
 
     return lines
 
 
 def _split_str(
     text: str,
     max_tokens: int,
-    separators: List[str],
+    separators: list[str],
     trim: bool,
     token_counter: Callable = _token_counter,
-) -> Tuple[List[str], bool]:
+) -> tuple[list[str], bool]:
     """
     Split text into lines.
     """
     input_was_split = False
     if not text:
-        return [], input_was_split
+        return [], input_was_split  # pragma: no cover
 
     if trim:
         text = text.strip()
 
     text_as_is = [text]
 
     if token_counter(text) <= max_tokens:
@@ -291,25 +291,25 @@
     else:
         return text_as_is, input_was_split
 
     return lines, input_was_split
 
 
 def _split_list(
-    text: List[str],
+    text: list[str],
     max_tokens: int,
-    separators: List[str],
+    separators: list[str],
     trim: bool,
     token_counter: Callable = _token_counter,
-) -> Tuple[List[str], bool]:
+) -> tuple[list[str], bool]:
     """
     Split list of string into lines.
     """
     if not text:
-        return [], False
+        return [], False  # pragma: no cover
 
     lines = []
     input_was_split = False
     for line in text:
         split_str, was_split = _split_str(
             text=line,
             max_tokens=max_tokens,
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/utils/experimental_decorator.py` & `semantic_kernel-1.0.1/semantic_kernel/utils/experimental_decorator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import types
-from typing import Callable, Type
+from collections.abc import Callable
 
 
 def experimental_function(func: Callable) -> Callable:
     if isinstance(func, types.FunctionType):
         if func.__doc__:
             func.__doc__ += "\n\nNote: This function is experimental and may change in the future."
         else:
             func.__doc__ = "Note: This function is experimental and may change in the future."
 
         func.is_experimental = True
 
     return func
 
 
-def experimental_class(cls: Type) -> Type:
+def experimental_class(cls: type) -> type:
     if isinstance(cls, type):
         if cls.__doc__:
             cls.__doc__ += "\n\nNote: This class is experimental and may change in the future."
         else:
             cls.__doc__ = "Note: This class is experimental and may change in the future."
 
         cls.is_experimental = True
```

### Comparing `semantic_kernel-1.0.0rc1/semantic_kernel/utils/naming.py` & `semantic_kernel-1.0.1/semantic_kernel/utils/naming.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-1.0.0rc1/PKG-INFO` & `semantic_kernel-1.0.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 1.0.0rc1
+Version: 1.0.1
 Summary: Semantic Kernel Python SDK
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.10,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -20,46 +20,41 @@
 Provides-Extra: postgres
 Provides-Extra: qdrant
 Provides-Extra: redis
 Provides-Extra: usearch
 Provides-Extra: weaviate
 Requires-Dist: aiohttp (>=3.8,<4.0)
 Requires-Dist: azure-core (>=1.28.0,<2.0.0) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-cosmos (>=4.7.0,<5.0.0) ; extra == "azure" or extra == "all"
 Requires-Dist: azure-identity (>=1.13.0,<2.0.0) ; extra == "azure" or extra == "all"
-Requires-Dist: azure-search-documents (==11.6.0b1) ; extra == "azure" or extra == "all"
+Requires-Dist: azure-search-documents (==11.6.0b4) ; extra == "azure" or extra == "all"
 Requires-Dist: chromadb (>=0.4.13,<0.5.0) ; extra == "chromadb" or extra == "all"
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
-Requires-Dist: eval_type_backport (>=0.1.3,<0.2.0) ; python_version < "3.10"
 Requires-Dist: google-generativeai (>=0.1) ; (python_version >= "3.9") and (extra == "google" or extra == "all")
-Requires-Dist: grpcio (>=1.40.0) ; python_version == "3.8"
-Requires-Dist: grpcio (>=1.50.0) ; python_version >= "3.9"
+Requires-Dist: grpcio (>=1.50.0) ; python_version < "3.12"
 Requires-Dist: grpcio (>=1.60.0) ; python_version >= "3.12"
 Requires-Dist: grpcio-status (>=1.53.0,<2.0.0) ; (python_version >= "3.9") and (extra == "google" or extra == "all")
 Requires-Dist: ipykernel (>=6.21.1,<7.0.0) ; extra == "notebooks" or extra == "all"
 Requires-Dist: jinja2 (>=3.1.3,<4.0.0)
-Requires-Dist: milvus (>=2.2,<2.3) ; (python_version == "3.8" and sys_platform != "win32") and (extra == "milvus" or extra == "all")
-Requires-Dist: milvus (>=2.3,<2.3.8) ; (python_version > "3.8" and sys_platform != "win32") and (extra == "milvus" or extra == "all")
+Requires-Dist: milvus (>=2.3,<2.3.8) ; (sys_platform != "win32") and (extra == "milvus" or extra == "all")
 Requires-Dist: motor (>=3.3.2,<4.0.0)
 Requires-Dist: nest-asyncio (>=1.6.0,<2.0.0)
-Requires-Dist: numpy (>=1.24,<2.0) ; python_version == "3.8"
-Requires-Dist: numpy (>=1.25) ; python_version >= "3.9" and python_version < "3.12"
+Requires-Dist: numpy (>=1.25) ; python_version < "3.12"
 Requires-Dist: numpy (>=1.26) ; python_version >= "3.12"
 Requires-Dist: openai (>=1.0)
 Requires-Dist: openapi_core (>=0.18,<0.20)
 Requires-Dist: pinecone-client (>=3.0.0) ; extra == "pinecone" or extra == "all"
 Requires-Dist: prance (>=23.6.21.0,<24.0.0.0)
 Requires-Dist: psycopg[binary,pool] (>=3.1.9,<4.0.0) ; extra == "postgres" or extra == "all"
 Requires-Dist: pyarrow (>=12.0.1,<16.0.0) ; extra == "usearch" or extra == "all"
 Requires-Dist: pybars4 (>=0.9.13,<0.10.0)
 Requires-Dist: pydantic (>=2,<3)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
-Requires-Dist: pymilvus (>=2.2,<2.3) ; (python_version == "3.8") and (extra == "milvus" or extra == "all")
-Requires-Dist: pymilvus (>=2.3,<2.3.8) ; (python_version > "3.8") and (extra == "milvus" or extra == "all")
-Requires-Dist: qdrant-client (>=1.6,<2.0) ; (python_version == "3.8") and (extra == "qdrant" or extra == "all")
-Requires-Dist: qdrant-client (>=1.7) ; (python_full_version > "3.9.0") and (extra == "qdrant" or extra == "all")
+Requires-Dist: pymilvus (>=2.3,<2.3.8) ; extra == "milvus" or extra == "all"
+Requires-Dist: qdrant-client (>=1.9,<2.0) ; extra == "qdrant" or extra == "all"
 Requires-Dist: redis (>=4.6.0,<5.0.0) ; extra == "redis" or extra == "all"
 Requires-Dist: regex (>=2023.6.3,<2024.0.0)
 Requires-Dist: scipy (>=1.12.0) ; python_version >= "3.12"
 Requires-Dist: scipy (>=1.5.0) ; python_version < "3.12"
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "hugging-face" or extra == "all"
 Requires-Dist: torch (>=2.2.0,<3.0.0) ; extra == "hugging-face" or extra == "all"
 Requires-Dist: transformers (>=4.28.1,<5.0.0) ; extra == "hugging-face" or extra == "all"
```

