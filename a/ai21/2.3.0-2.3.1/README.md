# Comparing `tmp/ai21-2.3.0.tar.gz` & `tmp/ai21-2.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai21-2.3.0.tar", max compression
+gzip compressed data, was "ai21-2.3.1.tar", max compression
```

## Comparing `ai21-2.3.0.tar` & `ai21-2.3.1.tar`

### file list

```diff
@@ -1,105 +1,105 @@
--rw-r--r--   0        0        0    11357 2024-05-20 11:35:42.419077 ai21-2.3.0/LICENSE
--rw-r--r--   0        0        0    12340 2024-05-20 11:35:42.419077 ai21-2.3.0/README.md
--rw-r--r--   0        0        0     1575 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/__init__.py
--rw-r--r--   0        0        0     1014 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/ai21_env_config.py
--rw-r--r--   0        0        0     2703 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/ai21_http_client.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/__init__.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/__init__.py
--rw-r--r--   0        0        0      844 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/ai21_bedrock_client.py
--rw-r--r--   0        0        0       92 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/bedrock_model_id.py
--rw-r--r--   0        0        0     2414 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/bedrock_session.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_completion.py
--rw-r--r--   0        0        0      522 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_resource.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/__init__.py
--rw-r--r--   0        0        0      857 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/answer_base.py
--rw-r--r--   0        0        0     3594 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/chat_base.py
--rw-r--r--   0        0        0     4081 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/completion_base.py
--rw-r--r--   0        0        0     1496 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/custom_model_base.py
--rw-r--r--   0        0        0     1723 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/dataset_base.py
--rw-r--r--   0        0        0      770 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/embed_base.py
--rw-r--r--   0        0        0      577 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/gec_base.py
--rw-r--r--   0        0        0      639 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/improvements_base.py
--rw-r--r--   0        0        0     1478 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/paraphrase_base.py
--rw-r--r--   0        0        0      674 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/segmentation_base.py
--rw-r--r--   0        0        0     1217 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/summarize_base.py
--rw-r--r--   0        0        0      999 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/common/summarize_by_segment_base.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/__init__.py
--rw-r--r--   0        0        0     1545 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/ai21_sagemaker_client.py
--rw-r--r--   0        0        0      154 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/constants.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/__init__.py
--rw-r--r--   0        0        0      498 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_answer.py
--rw-r--r--   0        0        0     3194 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_completion.py
--rw-r--r--   0        0        0      399 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_gec.py
--rw-r--r--   0        0        0      789 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
--rw-r--r--   0        0        0      484 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_resource.py
--rw-r--r--   0        0        0      810 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py
--rw-r--r--   0        0        0     2522 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/sagemaker/sagemaker_session.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/__init__.py
--rw-r--r--   0        0        0     3496 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/ai21_client.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/__init__.py
--rw-r--r--   0        0        0      101 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/chat/__init__.py
--rw-r--r--   0        0        0     3647 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/chat/chat_completions.py
--rw-r--r--   0        0        0      550 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_answer.py
--rw-r--r--   0        0        0     2036 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_chat.py
--rw-r--r--   0        0        0     2006 2024-05-20 11:35:42.419077 ai21-2.3.0/ai21/clients/studio/resources/studio_completion.py
--rw-r--r--   0        0        0     1301 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_custom_model.py
--rw-r--r--   0        0        0     1455 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_dataset.py
--rw-r--r--   0        0        0      560 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_embed.py
--rw-r--r--   0        0        0      446 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_gec.py
--rw-r--r--   0        0        0      722 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_improvements.py
--rw-r--r--   0        0        0     4100 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_library.py
--rw-r--r--   0        0        0      854 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_paraphrase.py
--rw-r--r--   0        0        0     2808 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_resource.py
--rw-r--r--   0        0        0      587 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_segmentation.py
--rw-r--r--   0        0        0      871 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_summarize.py
--rw-r--r--   0        0        0      772 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/clients/studio/resources/studio_summarize_by_segment.py
--rw-r--r--   0        0        0       64 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/constants.py
--rw-r--r--   0        0        0     2821 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/errors.py
--rw-r--r--   0        0        0     5373 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/http_client.py
--rw-r--r--   0        0        0      484 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/logger.py
--rw-r--r--   0        0        0     2633 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/__init__.py
--rw-r--r--   0        0        0      262 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/ai21_base_model_mixin.py
--rw-r--r--   0        0        0      510 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/__init__.py
--rw-r--r--   0        0        0      651 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_completion_chunk.py
--rw-r--r--   0        0        0      592 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_completion_response.py
--rw-r--r--   0        0        0      219 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/chat_message.py
--rw-r--r--   0        0        0       97 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat/role_type.py
--rw-r--r--   0        0        0      233 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/chat_message.py
--rw-r--r--   0        0        0       89 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/document_type.py
--rw-r--r--   0        0        0       96 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/embed_type.py
--rw-r--r--   0        0        0      286 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/improvement_type.py
--rw-r--r--   0        0        0      410 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/logprobs.py
--rw-r--r--   0        0        0      168 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/paraphrase_style_type.py
--rw-r--r--   0        0        0      503 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/penalty.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/__init__.py
--rw-r--r--   0        0        0      273 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/answer_response.py
--rw-r--r--   0        0        0      518 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/chat_response.py
--rw-r--r--   0        0        0      786 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/completion_response.py
--rw-r--r--   0        0        0      713 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/custom_model_response.py
--rw-r--r--   0        0        0      376 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/dataset_response.py
--rw-r--r--   0        0        0      300 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/embed_response.py
--rw-r--r--   0        0        0      550 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/file_response.py
--rw-r--r--   0        0        0      635 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/gec_response.py
--rw-r--r--   0        0        0      401 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/improvement_response.py
--rw-r--r--   0        0        0      469 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/library_answer_response.py
--rw-r--r--   0        0        0      450 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/library_search_response.py
--rw-r--r--   0        0        0      294 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/paraphrase_response.py
--rw-r--r--   0        0        0      317 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/segmentation_response.py
--rw-r--r--   0        0        0      564 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/summarize_by_segment_response.py
--rw-r--r--   0        0        0      187 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/responses/summarize_response.py
--rw-r--r--   0        0        0      139 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/summary_method.py
--rw-r--r--   0        0        0      222 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/models/usage_info.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/py.typed
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/services/__init__.py
--rw-r--r--   0        0        0     2310 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/services/sagemaker.py
--rw-r--r--   0        0        0     2105 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/stream.py
--rw-r--r--   0        0        0      123 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/__init__.py
--rw-r--r--   0        0        0      608 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/ai21_tokenizer.py
--rw-r--r--   0        0        0      628 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/tokenizers/factory.py
--rw-r--r--   0        0        0     1074 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/types.py
--rw-r--r--   0        0        0        0 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/utils/__init__.py
--rw-r--r--   0        0        0      989 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/utils/typing.py
--rw-r--r--   0        0        0       18 2024-05-20 11:35:42.423077 ai21-2.3.0/ai21/version.py
--rw-r--r--   0        0        0     2286 2024-05-20 11:35:42.427077 ai21-2.3.0/pyproject.toml
--rw-r--r--   0        0        0    13091 1970-01-01 00:00:00.000000 ai21-2.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:06:40.054503 ai21-2.3.1/LICENSE
+-rw-r--r--   0        0        0    13215 2024-05-22 18:06:40.058503 ai21-2.3.1/README.md
+-rw-r--r--   0        0        0     1575 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/__init__.py
+-rw-r--r--   0        0        0     2516 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/ai21_env_config.py
+-rw-r--r--   0        0        0     2703 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/ai21_http_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/__init__.py
+-rw-r--r--   0        0        0      844 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/ai21_bedrock_client.py
+-rw-r--r--   0        0        0       92 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/bedrock_model_id.py
+-rw-r--r--   0        0        0     2414 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/bedrock_session.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/__init__.py
+-rw-r--r--   0        0        0     1996 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_completion.py
+-rw-r--r--   0        0        0      522 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_resource.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/__init__.py
+-rw-r--r--   0        0        0      857 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/answer_base.py
+-rw-r--r--   0        0        0     3594 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/chat_base.py
+-rw-r--r--   0        0        0     4081 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/completion_base.py
+-rw-r--r--   0        0        0     1496 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/custom_model_base.py
+-rw-r--r--   0        0        0     1723 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/dataset_base.py
+-rw-r--r--   0        0        0      770 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/embed_base.py
+-rw-r--r--   0        0        0      577 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/gec_base.py
+-rw-r--r--   0        0        0      639 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/improvements_base.py
+-rw-r--r--   0        0        0     1478 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/paraphrase_base.py
+-rw-r--r--   0        0        0      674 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/segmentation_base.py
+-rw-r--r--   0        0        0     1217 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/summarize_base.py
+-rw-r--r--   0        0        0      999 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/common/summarize_by_segment_base.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/__init__.py
+-rw-r--r--   0        0        0     1545 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/ai21_sagemaker_client.py
+-rw-r--r--   0        0        0      154 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/constants.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_answer.py
+-rw-r--r--   0        0        0     3194 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_completion.py
+-rw-r--r--   0        0        0      399 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_gec.py
+-rw-r--r--   0        0        0      789 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py
+-rw-r--r--   0        0        0      484 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_resource.py
+-rw-r--r--   0        0        0      810 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_summarize.py
+-rw-r--r--   0        0        0     2522 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/sagemaker/sagemaker_session.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/__init__.py
+-rw-r--r--   0        0        0     3496 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/ai21_client.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/__init__.py
+-rw-r--r--   0        0        0      101 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/chat/__init__.py
+-rw-r--r--   0        0        0     3647 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/chat/chat_completions.py
+-rw-r--r--   0        0        0      550 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_answer.py
+-rw-r--r--   0        0        0     2036 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_chat.py
+-rw-r--r--   0        0        0     2006 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_completion.py
+-rw-r--r--   0        0        0     1301 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_custom_model.py
+-rw-r--r--   0        0        0     1455 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_dataset.py
+-rw-r--r--   0        0        0      560 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_embed.py
+-rw-r--r--   0        0        0      446 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_gec.py
+-rw-r--r--   0        0        0      722 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_improvements.py
+-rw-r--r--   0        0        0     4100 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_library.py
+-rw-r--r--   0        0        0      854 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_paraphrase.py
+-rw-r--r--   0        0        0     2808 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_resource.py
+-rw-r--r--   0        0        0      587 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_segmentation.py
+-rw-r--r--   0        0        0      871 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_summarize.py
+-rw-r--r--   0        0        0      772 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/clients/studio/resources/studio_summarize_by_segment.py
+-rw-r--r--   0        0        0       64 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/constants.py
+-rw-r--r--   0        0        0     2821 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/errors.py
+-rw-r--r--   0        0        0     5373 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/http_client.py
+-rw-r--r--   0        0        0      484 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/logger.py
+-rw-r--r--   0        0        0     2633 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/__init__.py
+-rw-r--r--   0        0        0      262 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/ai21_base_model_mixin.py
+-rw-r--r--   0        0        0      510 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/__init__.py
+-rw-r--r--   0        0        0      651 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_completion_chunk.py
+-rw-r--r--   0        0        0      592 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_completion_response.py
+-rw-r--r--   0        0        0      219 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/chat_message.py
+-rw-r--r--   0        0        0       97 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat/role_type.py
+-rw-r--r--   0        0        0      233 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/chat_message.py
+-rw-r--r--   0        0        0       89 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/document_type.py
+-rw-r--r--   0        0        0       96 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/embed_type.py
+-rw-r--r--   0        0        0      286 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/improvement_type.py
+-rw-r--r--   0        0        0      410 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/logprobs.py
+-rw-r--r--   0        0        0      168 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/paraphrase_style_type.py
+-rw-r--r--   0        0        0      503 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/penalty.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/__init__.py
+-rw-r--r--   0        0        0      273 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/answer_response.py
+-rw-r--r--   0        0        0      518 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/chat_response.py
+-rw-r--r--   0        0        0      786 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/completion_response.py
+-rw-r--r--   0        0        0      713 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/custom_model_response.py
+-rw-r--r--   0        0        0      376 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/dataset_response.py
+-rw-r--r--   0        0        0      300 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/embed_response.py
+-rw-r--r--   0        0        0      550 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/file_response.py
+-rw-r--r--   0        0        0      635 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/gec_response.py
+-rw-r--r--   0        0        0      401 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/improvement_response.py
+-rw-r--r--   0        0        0      469 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/library_answer_response.py
+-rw-r--r--   0        0        0      450 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/library_search_response.py
+-rw-r--r--   0        0        0      294 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/paraphrase_response.py
+-rw-r--r--   0        0        0      317 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/segmentation_response.py
+-rw-r--r--   0        0        0      564 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/summarize_by_segment_response.py
+-rw-r--r--   0        0        0      187 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/responses/summarize_response.py
+-rw-r--r--   0        0        0      139 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/summary_method.py
+-rw-r--r--   0        0        0      222 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/models/usage_info.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/py.typed
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/services/__init__.py
+-rw-r--r--   0        0        0     2310 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/services/sagemaker.py
+-rw-r--r--   0        0        0     2105 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/stream.py
+-rw-r--r--   0        0        0      123 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/__init__.py
+-rw-r--r--   0        0        0      608 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/ai21_tokenizer.py
+-rw-r--r--   0        0        0      628 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/tokenizers/factory.py
+-rw-r--r--   0        0        0     1074 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/types.py
+-rw-r--r--   0        0        0        0 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/utils/__init__.py
+-rw-r--r--   0        0        0      989 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/utils/typing.py
+-rw-r--r--   0        0        0       18 2024-05-22 18:06:40.058503 ai21-2.3.1/ai21/version.py
+-rw-r--r--   0        0        0     2286 2024-05-22 18:06:40.062503 ai21-2.3.1/pyproject.toml
+-rw-r--r--   0        0        0    13966 1970-01-01 00:00:00.000000 ai21-2.3.1/PKG-INFO
```

### Comparing `ai21-2.3.0/LICENSE` & `ai21-2.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/README.md` & `ai21-2.3.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -14,14 +14,41 @@
 <a href="https://pypi.org/project/ai21" target="_blank"><img src="https://img.shields.io/pypi/pyversions/ai21?color=%2334D058" alt="Supported Python versions"></a>
 <a href="https://github.com/semantic-release/semantic-release" target="_blank"><img src="https://img.shields.io/badge/semantic--release-python-e10079?logo=semantic-release" alt="Semantic Release Support"></a>
 <a href="https://opensource.org/licenses/Apache-2.0" target="_blank"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License"></a>
 </p>
 
 ---
 
+## Table of Contents
+
+- [Examples](#examples-tldr) 🗂️
+- [Migration from v1.3.4 and below](#migration-from-v134-and-below)
+- [AI21 Official Documentation](#Documentation)
+- [Installation](#Installation) 💿
+- [Usage - Chat Completions](#Usage)
+- [Older Models Support Usage](#Older-Models-Support-Usage)
+- [More Models](#More-Models)
+  - [Streaming](#Streaming)
+  - [TSMs](#TSMs)
+- [Token Counting](#Token-Counting)
+- [Environment Variables](#Environment-Variables)
+- [Error Handling](#Error-Handling)
+- [Cloud Providers](#Cloud-Providers) ☁️
+  - [AWS](#AWS)
+    - [SageMaker](#SageMaker)
+    - [Bedrock](#Bedrock)
+
+## Examples (tl;dr)
+
+If you want to quickly get a glance how to use the AI21 Python SDK and jump straight to business, you can check out the examples. Take a look at our models and see them in action! Several examples and demonstrations have been put together to show our models' functionality and capabilities.
+
+### [Check out the Examples](examples/)
+
+Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
+
 ## Migration from v1.3.4 and below
 
 In `v2.0.0` we introduced a new SDK that is not backwards compatible with the previous version.
 This version allows for non-static instances of the client, defined parameters to each resource, modelized responses and
 more.
 
 <details>
@@ -129,15 +156,14 @@
 
 ## Usage
 
 ---
 
 ```python
 from ai21 import AI21Client
-from ai21.models import RoleType
 from ai21.models.chat import ChatMessage
 
 client = AI21Client(
     # defaults to os.enviorn.get('AI21_API_KEY')
     api_key='my_api_key',
 )
 
@@ -232,14 +258,16 @@
 for chunk in response:
     print(chunk.choices[0].delta.content, end="")
 
 ```
 
 ---
 
+## More Models
+
 ## TSMs
 
 AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
 The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
 
 ### Contextual Answers
 
@@ -253,15 +281,36 @@
     context="This is a text is for testing purposes",
     question="Question about context",
 )
 ```
 
 A detailed explanation on Contextual Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
 
-### Token Counting
+### File Upload
+
+---
+
+```python
+from ai21 import AI21Client
+
+client = AI21Client()
+
+file_id = client.library.files.create(
+    file_path="path/to/file",
+    path="path/to/file/in/library",
+    labels=["label1", "label2"],
+    public_url="www.example.com",
+)
+
+uploaded_file = client.library.files.get(file_id)
+```
+
+For more information on more Task Specific Models, see the [documentation](https://docs.ai21.com/reference/paraphrase-api-ref).
+
+## Token Counting
 
 ---
 
 By using the `count_tokens` method, you can estimate the billing for a given request.
 
 ```python
 from ai21.tokenizers import get_tokenizer
@@ -274,33 +323,14 @@
 Available tokenizers are:
 
 - `jamba-instruct-tokenizer`
 - `j2-tokenizer`
 
 For more information on AI21 Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-tokenizer).
 
-### File Upload
-
----
-
-```python
-from ai21 import AI21Client
-
-client = AI21Client()
-
-file_id = client.library.files.create(
-    file_path="path/to/file",
-    path="path/to/file/in/library",
-    labels=["label1", "label2"],
-    public_url="www.example.com",
-)
-
-uploaded_file = client.library.files.get(file_id)
-```
-
 ## Environment Variables
 
 ---
 
 You can set several environment variables to configure the client.
 
 ### Logging
@@ -351,18 +381,20 @@
 except ai21_errors.TooManyRequestsError as e:
     print("A 429 status code was returned. Slow down on the requests")
 except AI21APIError as e:
     print("A non 200 status code error. For more error types see ai21.errors")
 
 ```
 
-## AWS Clients
+## Cloud Providers
 
 ---
 
+### AWS
+
 AI21 Library provides convenient ways to interact with two AWS clients for use with AWS SageMaker and AWS Bedrock.
 
 ### Installation
 
 ---
 
 ```bash
@@ -431,16 +463,8 @@
 response = client.completion.create(
     prompt="Your prompt here",
     model_id=BedrockModelID.J2_MID_V1,
     max_tokens=10,
 )
 ```
 
-## Examples
-
-Explore our examples to see our models in action! We've put together a variety of use cases and demonstrations to showcase the capabilities and functionality of our models.
-
-### [Check out the Examples](examples/)
-
-Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
-
 Happy prompting! 🚀
```

#### html2text {}

```diff
@@ -1,107 +1,123 @@
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                       _[_S_e_m_a_n_t_i_c_ _R_e_l_e_a_s_e_ _S_u_p_p_o_r_t_]_[_L_i_c_e_n_s_e_]
---- ## Migration from v1.3.4 and below In `v2.0.0` we introduced a new SDK that
-is not backwards compatible with the previous version. This version allows for
-non-static instances of the client, defined parameters to each resource,
-modelized responses and more. Migration Examples ### Instance creation (not
-available in v1.3.4 and below) ```python from ai21 import AI21Client client =
-AI21Client(api_key='my_api_key') # or set api_key in environment variable -
-AI21_API_KEY and then client = AI21Client() ``` We No longer support static
-methods for each resource, instead we have a client instance that has a method
-for each allowing for more flexibility and better control. ### Completion
-before/after ```diff prompt = "some prompt" - import ai21 - response =
-ai21.Completion.execute(model="j2-light", prompt=prompt, maxTokens=2) + from
-ai21 import AI21Client + client = ai21.AI21Client() + response =
-client.completion.create(model="j2-light", prompt=prompt, max_tokens=2) ```
-This applies to all resources. You would now need to create a client instance
-and use it to call the resource method. ### Tokenization and Token counting
-before/after ```diff - response = ai21.Tokenization.execute(text=prompt) -
-print(len(response)) # number of tokens + from ai21 import AI21Client + client
-= AI21Client() + token_count = client.count_tokens(text=prompt) ``` ### Key
-Access in Response Objects before/after It is no longer possible to access the
-response object as a dictionary. Instead, you can access the response object as
-an object with attributes. ```diff - import ai21 - response =
-ai21.Summarize.execute(source="some text", sourceType="TEXT") - response
-["summary"] + from ai21 import AI21Client + from ai21.models import
-DocumentType + client = AI21Client() + response = client.summarize.create
-(source="some text", source_type=DocumentType.TEXT) + response.summary ``` --
-- ### AWS Client Creations ### Bedrock Client creation before/after ```diff -
-import ai21 - destination = ai21.BedrockDestination
+--- ## Table of Contents - [Examples](#examples-tldr) ðï¸ - [Migration from
+v1.3.4 and below](#migration-from-v134-and-below) - [AI21 Official
+Documentation](#Documentation) - [Installation](#Installation) ð¿ - [Usage -
+Chat Completions](#Usage) - [Older Models Support Usage](#Older-Models-Support-
+Usage) - [More Models](#More-Models) - [Streaming](#Streaming) - [TSMs](#TSMs)
+- [Token Counting](#Token-Counting) - [Environment Variables](#Environment-
+Variables) - [Error Handling](#Error-Handling) - [Cloud Providers](#Cloud-
+Providers) âï¸ - [AWS](#AWS) - [SageMaker](#SageMaker) - [Bedrock](#Bedrock)
+## Examples (tl;dr) If you want to quickly get a glance how to use the AI21
+Python SDK and jump straight to business, you can check out the examples. Take
+a look at our models and see them in action! Several examples and
+demonstrations have been put together to show our models' functionality and
+capabilities. ### [Check out the Examples](examples/) Feel free to dive in,
+experiment, and adapt these examples to suit your needs. We believe they'll
+help you get up and running quickly. ## Migration from v1.3.4 and below In
+`v2.0.0` we introduced a new SDK that is not backwards compatible with the
+previous version. This version allows for non-static instances of the client,
+defined parameters to each resource, modelized responses and more. Migration
+Examples ### Instance creation (not available in v1.3.4 and below) ```python
+from ai21 import AI21Client client = AI21Client(api_key='my_api_key') # or set
+api_key in environment variable - AI21_API_KEY and then client = AI21Client()
+``` We No longer support static methods for each resource, instead we have a
+client instance that has a method for each allowing for more flexibility and
+better control. ### Completion before/after ```diff prompt = "some prompt" -
+import ai21 - response = ai21.Completion.execute(model="j2-light",
+prompt=prompt, maxTokens=2) + from ai21 import AI21Client + client =
+ai21.AI21Client() + response = client.completion.create(model="j2-light",
+prompt=prompt, max_tokens=2) ``` This applies to all resources. You would now
+need to create a client instance and use it to call the resource method. ###
+Tokenization and Token counting before/after ```diff - response =
+ai21.Tokenization.execute(text=prompt) - print(len(response)) # number of
+tokens + from ai21 import AI21Client + client = AI21Client() + token_count =
+client.count_tokens(text=prompt) ``` ### Key Access in Response Objects before/
+after It is no longer possible to access the response object as a dictionary.
+Instead, you can access the response object as an object with attributes.
+```diff - import ai21 - response = ai21.Summarize.execute(source="some text",
+sourceType="TEXT") - response["summary"] + from ai21 import AI21Client + from
+ai21.models import DocumentType + client = AI21Client() + response =
+client.summarize.create(source="some text", source_type=DocumentType.TEXT) +
+response.summary ``` --- ### AWS Client Creations ### Bedrock Client creation
+before/after ```diff - import ai21 - destination = ai21.BedrockDestination
 (model_id=ai21.BedrockModelID.J2_MID_V1) - response = ai21.Completion.execute
 (prompt=prompt, maxTokens=1000, destination=destination) + from ai21 import
 AI21BedrockClient, BedrockModelID + client = AI21BedrockClient() + response =
 client.completion.create(prompt=prompt, max_tokens=1000,
 model_id=BedrockModelID.J2_MID_V1) ``` ### SageMaker Client creation before/
 after ```diff - import ai21 - destination = ai21.SageMakerDestination("j2-mid-
 test-endpoint") - response = ai21.Completion.execute(prompt=prompt,
 maxTokens=1000, destination=destination) + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint") + response
 = client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Documentation
 --- The full documentation for the REST API can be found on [docs.ai21.com]
 (https://docs.ai21.com/). ## Installation --- ```bash pip install ai21 ``` ##
-Usage --- ```python from ai21 import AI21Client from ai21.models import
-RoleType from ai21.models.chat import ChatMessage client = AI21Client( #
-defaults to os.enviorn.get('AI21_API_KEY') api_key='my_api_key', ) messages =
-[ # Could be a dict or a ChatMessage object ChatMessage(content="Hello, this is
-a readme", role="user"), ChatMessage(content="You are correct, how can I help
-you?", role="assistant"), ] chat_completions = client.chat.completions.create
-( messages=messages, model="jamba-instruct-preview", ) ``` A more detailed
-example can be found [here](examples/studio/chat/chat_completions.py). ## Older
-Models Support Usage Examples ### Supported Models: - j2-light - j2-mid - j2-
-ultra you can read more about the models [here](https://docs.ai21.com/
-reference/j2-complete-api-ref#jurassic-2-models). ### Chat ```python from ai21
-import AI21Client from ai21.models import RoleType from ai21.models import
-ChatMessage system = "You're a support engineer in a SaaS company" messages =
-[ ChatMessage(text="Hello, I need help with a signup process.",
-role=RoleType.USER), ChatMessage(text="Hi Alice, I can help you with that. What
-seems to be the problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am
-having trouble signing up for your product with my Google account.",
-role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
-( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
-example, see the chat [examples](examples/studio/chat.py). ### Completion
-```python from ai21 import AI21Client client = AI21Client() completion_response
-= client.completion.create( prompt="This is a test prompt", model="j2-mid", )
-``` For a more detailed example, see the completion [examples](examples/studio/
+Usage --- ```python from ai21 import AI21Client from ai21.models.chat import
+ChatMessage client = AI21Client( # defaults to os.enviorn.get('AI21_API_KEY')
+api_key='my_api_key', ) messages = [ # Could be a dict or a ChatMessage object
+ChatMessage(content="Hello, this is a readme", role="user"), ChatMessage
+(content="You are correct, how can I help you?", role="assistant"), ]
+chat_completions = client.chat.completions.create( messages=messages,
+model="jamba-instruct-preview", ) ``` A more detailed example can be found
+[here](examples/studio/chat/chat_completions.py). ## Older Models Support Usage
+Examples ### Supported Models: - j2-light - j2-mid - j2-ultra you can read more
+about the models [here](https://docs.ai21.com/reference/j2-complete-api-
+ref#jurassic-2-models). ### Chat ```python from ai21 import AI21Client from
+ai21.models import RoleType from ai21.models import ChatMessage system =
+"You're a support engineer in a SaaS company" messages = [ ChatMessage
+(text="Hello, I need help with a signup process.", role=RoleType.USER),
+ChatMessage(text="Hi Alice, I can help you with that. What seems to be the
+problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am having trouble
+signing up for your product with my Google account.", role=RoleType.USER), ]
+client = AI21Client() chat_response = client.chat.create( system=system,
+messages=messages, model="j2-ultra", ) ``` For a more detailed example, see the
+chat [examples](examples/studio/chat.py). ### Completion ```python from ai21
+import AI21Client client = AI21Client() completion_response =
+client.completion.create( prompt="This is a test prompt", model="j2-mid", ) ```
+For a more detailed example, see the completion [examples](examples/studio/
 completion.py). --- ## Streaming We currently support streaming for the Chat
 Completions API in Jamba. ```python from ai21 import AI21Client from
 ai21.models.chat import ChatMessage messages = [ChatMessage(content="What is
 the meaning of life?", role="user")] client = AI21Client() response =
 client.chat.completions.create( messages=messages, model="jamba-instruct-
 preview", stream=True, ) for chunk in response: print(chunk.choices
-[0].delta.content, end="") ``` --- ## TSMs AI21 Studio's Task-Specific Models
-offer a range of powerful tools. These models have been specifically designed
-for their respective tasks and provide high-quality results while optimizing
-efficiency. The full documentation and guides can be found [here](https://
-docs.ai21.com/docs/task-specific). ### Contextual Answers The `answer` API
-allows you to access our high-quality question answering model. ```python from
-ai21 import AI21Client client = AI21Client() response = client.answer.create
-( context="This is a text is for testing purposes", question="Question about
-context", ) ``` A detailed explanation on Contextual Answers, can be found
-[here](https://docs.ai21.com/docs/contextual-answers-api) ### Token Counting --
-- By using the `count_tokens` method, you can estimate the billing for a given
-request. ```python from ai21.tokenizers import get_tokenizer tokenizer =
-get_tokenizer(name="jamba-instruct-tokenizer") total_tokens =
-tokenizer.count_tokens(text="some text") # returns int print(total_tokens) ```
-Available tokenizers are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For
-more information on AI21 Tokenizers, see the [documentation](https://
-github.com/AI21Labs/ai21-tokenizer). ### File Upload --- ```python from ai21
-import AI21Client client = AI21Client() file_id = client.library.files.create
-( file_path="path/to/file", path="path/to/file/in/library", labels=["label1",
-"label2"], public_url="www.example.com", ) uploaded_file =
-client.library.files.get(file_id) ``` ## Environment Variables --- You can set
-several environment variables to configure the client. ### Logging We use the
-standard library [`logging`](https://docs.python.org/3/library/logging.html)
-module. To enable logging, set the `AI21_LOG_LEVEL` environment variable.
-```bash $ export AI21_LOG_LEVEL=debug ``` ### Other Important Environment
-Variables - `AI21_API_KEY` - Your API key. If not set, you must pass it to the
-client constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+[0].delta.content, end="") ``` --- ## More Models ## TSMs AI21 Studio's Task-
+Specific Models offer a range of powerful tools. These models have been
+specifically designed for their respective tasks and provide high-quality
+results while optimizing efficiency. The full documentation and guides can be
+found [here](https://docs.ai21.com/docs/task-specific). ### Contextual Answers
+The `answer` API allows you to access our high-quality question answering
+model. ```python from ai21 import AI21Client client = AI21Client() response =
+client.answer.create( context="This is a text is for testing purposes",
+question="Question about context", ) ``` A detailed explanation on Contextual
+Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
+### File Upload --- ```python from ai21 import AI21Client client = AI21Client()
+file_id = client.library.files.create( file_path="path/to/file", path="path/to/
+file/in/library", labels=["label1", "label2"], public_url="www.example.com", )
+uploaded_file = client.library.files.get(file_id) ``` For more information on
+more Task Specific Models, see the [documentation](https://docs.ai21.com/
+reference/paraphrase-api-ref). ## Token Counting --- By using the
+`count_tokens` method, you can estimate the billing for a given request.
+```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
+(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
+(text="some text") # returns int print(total_tokens) ``` Available tokenizers
+are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
+Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
+tokenizer). ## Environment Variables --- You can set several environment
+variables to configure the client. ### Logging We use the standard library
+[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
+logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
+AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
+`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
+constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
 `AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
 `AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
 maximum number of retries for API requests. Defaults to `3` retries. -
 `AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
 east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
 from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
 client = AI21Client() system = "You're a support engineer in a SaaS company"
@@ -109,32 +125,28 @@
 the raised error ChatMessage(text="Hello, I need help with a signup process.",
 role="Non-Existent-Role"), ] try: chat_completion = client.chat.create
 ( messages=messages, model="j2-ultra", system=system ) except
 ai21_errors.AI21ServerError as e: print("Server error and could not be
 reached") print(e.details) except ai21_errors.TooManyRequestsError as e: print
 ("A 429 status code was returned. Slow down on the requests") except
 AI21APIError as e: print("A non 200 status code error. For more error types see
-ai21.errors") ``` ## AWS Clients --- AI21 Library provides convenient ways to
-interact with two AWS clients for use with AWS SageMaker and AWS Bedrock. ###
-Installation --- ```bash pip install "ai21[AWS]" ``` This will make sure you
-have the required dependencies installed, including `boto3 >= 1.28.82`. ###
-Usage --- #### SageMaker ```python from ai21 import AI21SageMakerClient client
-= AI21SageMakerClient(endpoint_name="j2-endpoint-name") response =
-client.summarize.create( source="Text to summarize", source_type="TEXT", )
-print(response.summary) ``` #### With Boto3 Session ```python from ai21 import
-AI21SageMakerClient import boto3 boto_session = boto3.Session(region_name="us-
-east-1") client = AI21SageMakerClient( session=boto_session, endpoint_name="j2-
-endpoint-name", ) ``` #### Bedrock --- ```python from ai21 import
-AI21BedrockClient, BedrockModelID client = AI21BedrockClient(region='us-east-
-1') # region is optional, as you can use the env variable instead response =
-client.completion.create( prompt="Your prompt here",
-model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print(response.completions
-[0].data.text) ``` #### With Boto3 Session ```python from ai21 import
-AI21BedrockClient, BedrockModelID import boto3 boto_session = boto3.Session
-(region_name="us-east-1") client = AI21BedrockClient( session=boto_session, )
-response = client.completion.create( prompt="Your prompt here",
-model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` ## Examples Explore our
-examples to see our models in action! We've put together a variety of use cases
-and demonstrations to showcase the capabilities and functionality of our
-models. ### [Check out the Examples](examples/) Feel free to dive in,
-experiment, and adapt these examples to suit your needs. We believe they'll
-help you get up and running quickly. Happy prompting! ð
+ai21.errors") ``` ## Cloud Providers --- ### AWS AI21 Library provides
+convenient ways to interact with two AWS clients for use with AWS SageMaker and
+AWS Bedrock. ### Installation --- ```bash pip install "ai21[AWS]" ``` This will
+make sure you have the required dependencies installed, including `boto3 >=
+1.28.82`. ### Usage --- #### SageMaker ```python from ai21 import
+AI21SageMakerClient client = AI21SageMakerClient(endpoint_name="j2-endpoint-
+name") response = client.summarize.create( source="Text to summarize",
+source_type="TEXT", ) print(response.summary) ``` #### With Boto3 Session
+```python from ai21 import AI21SageMakerClient import boto3 boto_session =
+boto3.Session(region_name="us-east-1") client = AI21SageMakerClient
+( session=boto_session, endpoint_name="j2-endpoint-name", ) ``` #### Bedrock --
+- ```python from ai21 import AI21BedrockClient, BedrockModelID client =
+AI21BedrockClient(region='us-east-1') # region is optional, as you can use the
+env variable instead response = client.completion.create( prompt="Your prompt
+here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print
+(response.completions[0].data.text) ``` #### With Boto3 Session ```python from
+ai21 import AI21BedrockClient, BedrockModelID import boto3 boto_session =
+boto3.Session(region_name="us-east-1") client = AI21BedrockClient
+( session=boto_session, ) response = client.completion.create( prompt="Your
+prompt here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` Happy
+prompting! ð
```

### Comparing `ai21-2.3.0/ai21/__init__.py` & `ai21-2.3.1/ai21/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/ai21_http_client.py` & `ai21-2.3.1/ai21/ai21_http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/bedrock/ai21_bedrock_client.py` & `ai21-2.3.1/ai21/clients/bedrock/ai21_bedrock_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/bedrock/bedrock_session.py` & `ai21-2.3.1/ai21/clients/bedrock/bedrock_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_completion.py` & `ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/bedrock/resources/bedrock_resource.py` & `ai21-2.3.1/ai21/clients/bedrock/resources/bedrock_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/answer_base.py` & `ai21-2.3.1/ai21/clients/common/answer_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/chat_base.py` & `ai21-2.3.1/ai21/clients/common/chat_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/completion_base.py` & `ai21-2.3.1/ai21/clients/common/completion_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/custom_model_base.py` & `ai21-2.3.1/ai21/clients/common/custom_model_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/dataset_base.py` & `ai21-2.3.1/ai21/clients/common/dataset_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/embed_base.py` & `ai21-2.3.1/ai21/clients/common/embed_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/gec_base.py` & `ai21-2.3.1/ai21/clients/common/gec_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/improvements_base.py` & `ai21-2.3.1/ai21/clients/common/improvements_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/paraphrase_base.py` & `ai21-2.3.1/ai21/clients/common/paraphrase_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/segmentation_base.py` & `ai21-2.3.1/ai21/clients/common/segmentation_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/summarize_base.py` & `ai21-2.3.1/ai21/clients/common/summarize_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/common/summarize_by_segment_base.py` & `ai21-2.3.1/ai21/clients/common/summarize_by_segment_base.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/sagemaker/ai21_sagemaker_client.py` & `ai21-2.3.1/ai21/clients/sagemaker/ai21_sagemaker_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_completion.py` & `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py` & `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/sagemaker/resources/sagemaker_summarize.py` & `ai21-2.3.1/ai21/clients/sagemaker/resources/sagemaker_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/sagemaker/sagemaker_session.py` & `ai21-2.3.1/ai21/clients/sagemaker/sagemaker_session.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/ai21_client.py` & `ai21-2.3.1/ai21/clients/studio/ai21_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/chat/chat_completions.py` & `ai21-2.3.1/ai21/clients/studio/resources/chat/chat_completions.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_answer.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_answer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_chat.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_chat.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_completion.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_completion.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_custom_model.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_custom_model.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_dataset.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_dataset.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_embed.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_embed.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_improvements.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_improvements.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_library.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_library.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_paraphrase.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_paraphrase.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_resource.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_resource.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_segmentation.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_segmentation.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_summarize.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_summarize.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/clients/studio/resources/studio_summarize_by_segment.py` & `ai21-2.3.1/ai21/clients/studio/resources/studio_summarize_by_segment.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/errors.py` & `ai21-2.3.1/ai21/errors.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/http_client.py` & `ai21-2.3.1/ai21/http_client.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/__init__.py` & `ai21-2.3.1/ai21/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/chat/chat_completion_chunk.py` & `ai21-2.3.1/ai21/models/chat/chat_completion_chunk.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/chat/chat_completion_response.py` & `ai21-2.3.1/ai21/models/chat/chat_completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/chat_response.py` & `ai21-2.3.1/ai21/models/responses/chat_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/completion_response.py` & `ai21-2.3.1/ai21/models/responses/completion_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/custom_model_response.py` & `ai21-2.3.1/ai21/models/responses/custom_model_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/file_response.py` & `ai21-2.3.1/ai21/models/responses/file_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/gec_response.py` & `ai21-2.3.1/ai21/models/responses/gec_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/models/responses/summarize_by_segment_response.py` & `ai21-2.3.1/ai21/models/responses/summarize_by_segment_response.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/services/sagemaker.py` & `ai21-2.3.1/ai21/services/sagemaker.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/stream.py` & `ai21-2.3.1/ai21/stream.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/tokenizers/ai21_tokenizer.py` & `ai21-2.3.1/ai21/tokenizers/ai21_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/tokenizers/factory.py` & `ai21-2.3.1/ai21/tokenizers/factory.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/types.py` & `ai21-2.3.1/ai21/types.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/ai21/utils/typing.py` & `ai21-2.3.1/ai21/utils/typing.py`

 * *Files identical despite different names*

### Comparing `ai21-2.3.0/pyproject.toml` & `ai21-2.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   "if __name__ == .__main__.:",
   "if TYPE_CHECKING:",
   "if typing.TYPE_CHECKING:"
 ]
 
 [tool.poetry]
 name = "ai21"
-version = "2.3.0"
+version = "2.3.1"
 description = ""
 authors = ["AI21 Labs"]
 readme = "README.md"
 packages = [
     { include = "ai21" }
 ]
```

### Comparing `ai21-2.3.0/PKG-INFO` & `ai21-2.3.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai21
-Version: 2.3.0
+Version: 2.3.1
 Summary: 
 Author: AI21 Labs
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -35,14 +35,41 @@
 <a href="https://pypi.org/project/ai21" target="_blank"><img src="https://img.shields.io/pypi/pyversions/ai21?color=%2334D058" alt="Supported Python versions"></a>
 <a href="https://github.com/semantic-release/semantic-release" target="_blank"><img src="https://img.shields.io/badge/semantic--release-python-e10079?logo=semantic-release" alt="Semantic Release Support"></a>
 <a href="https://opensource.org/licenses/Apache-2.0" target="_blank"><img src="https://img.shields.io/badge/License-Apache_2.0-blue.svg" alt="License"></a>
 </p>
 
 ---
 
+## Table of Contents
+
+- [Examples](#examples-tldr) 🗂️
+- [Migration from v1.3.4 and below](#migration-from-v134-and-below)
+- [AI21 Official Documentation](#Documentation)
+- [Installation](#Installation) 💿
+- [Usage - Chat Completions](#Usage)
+- [Older Models Support Usage](#Older-Models-Support-Usage)
+- [More Models](#More-Models)
+  - [Streaming](#Streaming)
+  - [TSMs](#TSMs)
+- [Token Counting](#Token-Counting)
+- [Environment Variables](#Environment-Variables)
+- [Error Handling](#Error-Handling)
+- [Cloud Providers](#Cloud-Providers) ☁️
+  - [AWS](#AWS)
+    - [SageMaker](#SageMaker)
+    - [Bedrock](#Bedrock)
+
+## Examples (tl;dr)
+
+If you want to quickly get a glance how to use the AI21 Python SDK and jump straight to business, you can check out the examples. Take a look at our models and see them in action! Several examples and demonstrations have been put together to show our models' functionality and capabilities.
+
+### [Check out the Examples](examples/)
+
+Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
+
 ## Migration from v1.3.4 and below
 
 In `v2.0.0` we introduced a new SDK that is not backwards compatible with the previous version.
 This version allows for non-static instances of the client, defined parameters to each resource, modelized responses and
 more.
 
 <details>
@@ -150,15 +177,14 @@
 
 ## Usage
 
 ---
 
 ```python
 from ai21 import AI21Client
-from ai21.models import RoleType
 from ai21.models.chat import ChatMessage
 
 client = AI21Client(
     # defaults to os.enviorn.get('AI21_API_KEY')
     api_key='my_api_key',
 )
 
@@ -253,14 +279,16 @@
 for chunk in response:
     print(chunk.choices[0].delta.content, end="")
 
 ```
 
 ---
 
+## More Models
+
 ## TSMs
 
 AI21 Studio's Task-Specific Models offer a range of powerful tools. These models have been specifically designed for their respective tasks and provide high-quality results while optimizing efficiency.
 The full documentation and guides can be found [here](https://docs.ai21.com/docs/task-specific).
 
 ### Contextual Answers
 
@@ -274,15 +302,36 @@
     context="This is a text is for testing purposes",
     question="Question about context",
 )
 ```
 
 A detailed explanation on Contextual Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
 
-### Token Counting
+### File Upload
+
+---
+
+```python
+from ai21 import AI21Client
+
+client = AI21Client()
+
+file_id = client.library.files.create(
+    file_path="path/to/file",
+    path="path/to/file/in/library",
+    labels=["label1", "label2"],
+    public_url="www.example.com",
+)
+
+uploaded_file = client.library.files.get(file_id)
+```
+
+For more information on more Task Specific Models, see the [documentation](https://docs.ai21.com/reference/paraphrase-api-ref).
+
+## Token Counting
 
 ---
 
 By using the `count_tokens` method, you can estimate the billing for a given request.
 
 ```python
 from ai21.tokenizers import get_tokenizer
@@ -295,33 +344,14 @@
 Available tokenizers are:
 
 - `jamba-instruct-tokenizer`
 - `j2-tokenizer`
 
 For more information on AI21 Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-tokenizer).
 
-### File Upload
-
----
-
-```python
-from ai21 import AI21Client
-
-client = AI21Client()
-
-file_id = client.library.files.create(
-    file_path="path/to/file",
-    path="path/to/file/in/library",
-    labels=["label1", "label2"],
-    public_url="www.example.com",
-)
-
-uploaded_file = client.library.files.get(file_id)
-```
-
 ## Environment Variables
 
 ---
 
 You can set several environment variables to configure the client.
 
 ### Logging
@@ -372,18 +402,20 @@
 except ai21_errors.TooManyRequestsError as e:
     print("A 429 status code was returned. Slow down on the requests")
 except AI21APIError as e:
     print("A non 200 status code error. For more error types see ai21.errors")
 
 ```
 
-## AWS Clients
+## Cloud Providers
 
 ---
 
+### AWS
+
 AI21 Library provides convenient ways to interact with two AWS clients for use with AWS SageMaker and AWS Bedrock.
 
 ### Installation
 
 ---
 
 ```bash
@@ -452,17 +484,9 @@
 response = client.completion.create(
     prompt="Your prompt here",
     model_id=BedrockModelID.J2_MID_V1,
     max_tokens=10,
 )
 ```
 
-## Examples
-
-Explore our examples to see our models in action! We've put together a variety of use cases and demonstrations to showcase the capabilities and functionality of our models.
-
-### [Check out the Examples](examples/)
-
-Feel free to dive in, experiment, and adapt these examples to suit your needs. We believe they'll help you get up and running quickly.
-
 Happy prompting! 🚀
```

#### html2text {}

```diff
@@ -1,117 +1,133 @@
-Metadata-Version: 2.1 Name: ai21 Version: 2.3.0 Summary: Author: AI21 Labs
+Metadata-Version: 2.1 Name: ai21 Version: 2.3.1 Summary: Author: AI21 Labs
 Requires-Python: >=3.8,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Provides-Extra: aws Requires-Dist: ai21-tokenizer
 (>=0.9.1,<1.0.0) Requires-Dist: boto3 (>=1.28.82,<2.0.0) ; extra == "aws"
 Requires-Dist: dataclasses-json (>=0.6.3,<0.7.0) Requires-Dist: httpx
 (>=0.27.0,<0.28.0) Requires-Dist: tenacity (>=8.3.0,<9.0.0) Requires-Dist:
 typing-extensions (>=4.9.0,<5.0.0) Description-Content-Type: text/markdown
                       ************ _AA_II_22_11_ _LL_aa_bb_ss_ _PP_yy_tt_hh_oo_nn_ _SS_DD_KK ************
 [//]: # "Add when public" [//]: # '_[_T_e_s_t_]' [//]: # '_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
 _v_e_r_s_i_o_n_s_]'
  _[_T_e_s_t_]_[_I_n_t_e_g_r_a_t_i_o_n_ _T_e_s_t_s_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_P_o_e_t_r_y_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n_ _v_e_r_s_i_o_n_s_]
                       _[_S_e_m_a_n_t_i_c_ _R_e_l_e_a_s_e_ _S_u_p_p_o_r_t_]_[_L_i_c_e_n_s_e_]
---- ## Migration from v1.3.4 and below In `v2.0.0` we introduced a new SDK that
-is not backwards compatible with the previous version. This version allows for
-non-static instances of the client, defined parameters to each resource,
-modelized responses and more. Migration Examples ### Instance creation (not
-available in v1.3.4 and below) ```python from ai21 import AI21Client client =
-AI21Client(api_key='my_api_key') # or set api_key in environment variable -
-AI21_API_KEY and then client = AI21Client() ``` We No longer support static
-methods for each resource, instead we have a client instance that has a method
-for each allowing for more flexibility and better control. ### Completion
-before/after ```diff prompt = "some prompt" - import ai21 - response =
-ai21.Completion.execute(model="j2-light", prompt=prompt, maxTokens=2) + from
-ai21 import AI21Client + client = ai21.AI21Client() + response =
-client.completion.create(model="j2-light", prompt=prompt, max_tokens=2) ```
-This applies to all resources. You would now need to create a client instance
-and use it to call the resource method. ### Tokenization and Token counting
-before/after ```diff - response = ai21.Tokenization.execute(text=prompt) -
-print(len(response)) # number of tokens + from ai21 import AI21Client + client
-= AI21Client() + token_count = client.count_tokens(text=prompt) ``` ### Key
-Access in Response Objects before/after It is no longer possible to access the
-response object as a dictionary. Instead, you can access the response object as
-an object with attributes. ```diff - import ai21 - response =
-ai21.Summarize.execute(source="some text", sourceType="TEXT") - response
-["summary"] + from ai21 import AI21Client + from ai21.models import
-DocumentType + client = AI21Client() + response = client.summarize.create
-(source="some text", source_type=DocumentType.TEXT) + response.summary ``` --
-- ### AWS Client Creations ### Bedrock Client creation before/after ```diff -
-import ai21 - destination = ai21.BedrockDestination
+--- ## Table of Contents - [Examples](#examples-tldr) ðï¸ - [Migration from
+v1.3.4 and below](#migration-from-v134-and-below) - [AI21 Official
+Documentation](#Documentation) - [Installation](#Installation) ð¿ - [Usage -
+Chat Completions](#Usage) - [Older Models Support Usage](#Older-Models-Support-
+Usage) - [More Models](#More-Models) - [Streaming](#Streaming) - [TSMs](#TSMs)
+- [Token Counting](#Token-Counting) - [Environment Variables](#Environment-
+Variables) - [Error Handling](#Error-Handling) - [Cloud Providers](#Cloud-
+Providers) âï¸ - [AWS](#AWS) - [SageMaker](#SageMaker) - [Bedrock](#Bedrock)
+## Examples (tl;dr) If you want to quickly get a glance how to use the AI21
+Python SDK and jump straight to business, you can check out the examples. Take
+a look at our models and see them in action! Several examples and
+demonstrations have been put together to show our models' functionality and
+capabilities. ### [Check out the Examples](examples/) Feel free to dive in,
+experiment, and adapt these examples to suit your needs. We believe they'll
+help you get up and running quickly. ## Migration from v1.3.4 and below In
+`v2.0.0` we introduced a new SDK that is not backwards compatible with the
+previous version. This version allows for non-static instances of the client,
+defined parameters to each resource, modelized responses and more. Migration
+Examples ### Instance creation (not available in v1.3.4 and below) ```python
+from ai21 import AI21Client client = AI21Client(api_key='my_api_key') # or set
+api_key in environment variable - AI21_API_KEY and then client = AI21Client()
+``` We No longer support static methods for each resource, instead we have a
+client instance that has a method for each allowing for more flexibility and
+better control. ### Completion before/after ```diff prompt = "some prompt" -
+import ai21 - response = ai21.Completion.execute(model="j2-light",
+prompt=prompt, maxTokens=2) + from ai21 import AI21Client + client =
+ai21.AI21Client() + response = client.completion.create(model="j2-light",
+prompt=prompt, max_tokens=2) ``` This applies to all resources. You would now
+need to create a client instance and use it to call the resource method. ###
+Tokenization and Token counting before/after ```diff - response =
+ai21.Tokenization.execute(text=prompt) - print(len(response)) # number of
+tokens + from ai21 import AI21Client + client = AI21Client() + token_count =
+client.count_tokens(text=prompt) ``` ### Key Access in Response Objects before/
+after It is no longer possible to access the response object as a dictionary.
+Instead, you can access the response object as an object with attributes.
+```diff - import ai21 - response = ai21.Summarize.execute(source="some text",
+sourceType="TEXT") - response["summary"] + from ai21 import AI21Client + from
+ai21.models import DocumentType + client = AI21Client() + response =
+client.summarize.create(source="some text", source_type=DocumentType.TEXT) +
+response.summary ``` --- ### AWS Client Creations ### Bedrock Client creation
+before/after ```diff - import ai21 - destination = ai21.BedrockDestination
 (model_id=ai21.BedrockModelID.J2_MID_V1) - response = ai21.Completion.execute
 (prompt=prompt, maxTokens=1000, destination=destination) + from ai21 import
 AI21BedrockClient, BedrockModelID + client = AI21BedrockClient() + response =
 client.completion.create(prompt=prompt, max_tokens=1000,
 model_id=BedrockModelID.J2_MID_V1) ``` ### SageMaker Client creation before/
 after ```diff - import ai21 - destination = ai21.SageMakerDestination("j2-mid-
 test-endpoint") - response = ai21.Completion.execute(prompt=prompt,
 maxTokens=1000, destination=destination) + from ai21 import AI21SageMakerClient
 + client = AI21SageMakerClient(endpoint_name="j2-mid-test-endpoint") + response
 = client.completion.create(prompt=prompt, max_tokens=1000) ``` ## Documentation
 --- The full documentation for the REST API can be found on [docs.ai21.com]
 (https://docs.ai21.com/). ## Installation --- ```bash pip install ai21 ``` ##
-Usage --- ```python from ai21 import AI21Client from ai21.models import
-RoleType from ai21.models.chat import ChatMessage client = AI21Client( #
-defaults to os.enviorn.get('AI21_API_KEY') api_key='my_api_key', ) messages =
-[ # Could be a dict or a ChatMessage object ChatMessage(content="Hello, this is
-a readme", role="user"), ChatMessage(content="You are correct, how can I help
-you?", role="assistant"), ] chat_completions = client.chat.completions.create
-( messages=messages, model="jamba-instruct-preview", ) ``` A more detailed
-example can be found [here](examples/studio/chat/chat_completions.py). ## Older
-Models Support Usage Examples ### Supported Models: - j2-light - j2-mid - j2-
-ultra you can read more about the models [here](https://docs.ai21.com/
-reference/j2-complete-api-ref#jurassic-2-models). ### Chat ```python from ai21
-import AI21Client from ai21.models import RoleType from ai21.models import
-ChatMessage system = "You're a support engineer in a SaaS company" messages =
-[ ChatMessage(text="Hello, I need help with a signup process.",
-role=RoleType.USER), ChatMessage(text="Hi Alice, I can help you with that. What
-seems to be the problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am
-having trouble signing up for your product with my Google account.",
-role=RoleType.USER), ] client = AI21Client() chat_response = client.chat.create
-( system=system, messages=messages, model="j2-ultra", ) ``` For a more detailed
-example, see the chat [examples](examples/studio/chat.py). ### Completion
-```python from ai21 import AI21Client client = AI21Client() completion_response
-= client.completion.create( prompt="This is a test prompt", model="j2-mid", )
-``` For a more detailed example, see the completion [examples](examples/studio/
+Usage --- ```python from ai21 import AI21Client from ai21.models.chat import
+ChatMessage client = AI21Client( # defaults to os.enviorn.get('AI21_API_KEY')
+api_key='my_api_key', ) messages = [ # Could be a dict or a ChatMessage object
+ChatMessage(content="Hello, this is a readme", role="user"), ChatMessage
+(content="You are correct, how can I help you?", role="assistant"), ]
+chat_completions = client.chat.completions.create( messages=messages,
+model="jamba-instruct-preview", ) ``` A more detailed example can be found
+[here](examples/studio/chat/chat_completions.py). ## Older Models Support Usage
+Examples ### Supported Models: - j2-light - j2-mid - j2-ultra you can read more
+about the models [here](https://docs.ai21.com/reference/j2-complete-api-
+ref#jurassic-2-models). ### Chat ```python from ai21 import AI21Client from
+ai21.models import RoleType from ai21.models import ChatMessage system =
+"You're a support engineer in a SaaS company" messages = [ ChatMessage
+(text="Hello, I need help with a signup process.", role=RoleType.USER),
+ChatMessage(text="Hi Alice, I can help you with that. What seems to be the
+problem?", role=RoleType.ASSISTANT), ChatMessage(text="I am having trouble
+signing up for your product with my Google account.", role=RoleType.USER), ]
+client = AI21Client() chat_response = client.chat.create( system=system,
+messages=messages, model="j2-ultra", ) ``` For a more detailed example, see the
+chat [examples](examples/studio/chat.py). ### Completion ```python from ai21
+import AI21Client client = AI21Client() completion_response =
+client.completion.create( prompt="This is a test prompt", model="j2-mid", ) ```
+For a more detailed example, see the completion [examples](examples/studio/
 completion.py). --- ## Streaming We currently support streaming for the Chat
 Completions API in Jamba. ```python from ai21 import AI21Client from
 ai21.models.chat import ChatMessage messages = [ChatMessage(content="What is
 the meaning of life?", role="user")] client = AI21Client() response =
 client.chat.completions.create( messages=messages, model="jamba-instruct-
 preview", stream=True, ) for chunk in response: print(chunk.choices
-[0].delta.content, end="") ``` --- ## TSMs AI21 Studio's Task-Specific Models
-offer a range of powerful tools. These models have been specifically designed
-for their respective tasks and provide high-quality results while optimizing
-efficiency. The full documentation and guides can be found [here](https://
-docs.ai21.com/docs/task-specific). ### Contextual Answers The `answer` API
-allows you to access our high-quality question answering model. ```python from
-ai21 import AI21Client client = AI21Client() response = client.answer.create
-( context="This is a text is for testing purposes", question="Question about
-context", ) ``` A detailed explanation on Contextual Answers, can be found
-[here](https://docs.ai21.com/docs/contextual-answers-api) ### Token Counting --
-- By using the `count_tokens` method, you can estimate the billing for a given
-request. ```python from ai21.tokenizers import get_tokenizer tokenizer =
-get_tokenizer(name="jamba-instruct-tokenizer") total_tokens =
-tokenizer.count_tokens(text="some text") # returns int print(total_tokens) ```
-Available tokenizers are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For
-more information on AI21 Tokenizers, see the [documentation](https://
-github.com/AI21Labs/ai21-tokenizer). ### File Upload --- ```python from ai21
-import AI21Client client = AI21Client() file_id = client.library.files.create
-( file_path="path/to/file", path="path/to/file/in/library", labels=["label1",
-"label2"], public_url="www.example.com", ) uploaded_file =
-client.library.files.get(file_id) ``` ## Environment Variables --- You can set
-several environment variables to configure the client. ### Logging We use the
-standard library [`logging`](https://docs.python.org/3/library/logging.html)
-module. To enable logging, set the `AI21_LOG_LEVEL` environment variable.
-```bash $ export AI21_LOG_LEVEL=debug ``` ### Other Important Environment
-Variables - `AI21_API_KEY` - Your API key. If not set, you must pass it to the
-client constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
+[0].delta.content, end="") ``` --- ## More Models ## TSMs AI21 Studio's Task-
+Specific Models offer a range of powerful tools. These models have been
+specifically designed for their respective tasks and provide high-quality
+results while optimizing efficiency. The full documentation and guides can be
+found [here](https://docs.ai21.com/docs/task-specific). ### Contextual Answers
+The `answer` API allows you to access our high-quality question answering
+model. ```python from ai21 import AI21Client client = AI21Client() response =
+client.answer.create( context="This is a text is for testing purposes",
+question="Question about context", ) ``` A detailed explanation on Contextual
+Answers, can be found [here](https://docs.ai21.com/docs/contextual-answers-api)
+### File Upload --- ```python from ai21 import AI21Client client = AI21Client()
+file_id = client.library.files.create( file_path="path/to/file", path="path/to/
+file/in/library", labels=["label1", "label2"], public_url="www.example.com", )
+uploaded_file = client.library.files.get(file_id) ``` For more information on
+more Task Specific Models, see the [documentation](https://docs.ai21.com/
+reference/paraphrase-api-ref). ## Token Counting --- By using the
+`count_tokens` method, you can estimate the billing for a given request.
+```python from ai21.tokenizers import get_tokenizer tokenizer = get_tokenizer
+(name="jamba-instruct-tokenizer") total_tokens = tokenizer.count_tokens
+(text="some text") # returns int print(total_tokens) ``` Available tokenizers
+are: - `jamba-instruct-tokenizer` - `j2-tokenizer` For more information on AI21
+Tokenizers, see the [documentation](https://github.com/AI21Labs/ai21-
+tokenizer). ## Environment Variables --- You can set several environment
+variables to configure the client. ### Logging We use the standard library
+[`logging`](https://docs.python.org/3/library/logging.html) module. To enable
+logging, set the `AI21_LOG_LEVEL` environment variable. ```bash $ export
+AI21_LOG_LEVEL=debug ``` ### Other Important Environment Variables -
+`AI21_API_KEY` - Your API key. If not set, you must pass it to the client
+constructor. - `AI21_API_VERSION` - The API version. Defaults to `v1`. -
 `AI21_API_HOST` - The API host. Defaults to `https://api.ai21.com/v1/`. -
 `AI21_TIMEOUT_SEC` - The timeout for API requests. - `AI21_NUM_RETRIES` - The
 maximum number of retries for API requests. Defaults to `3` retries. -
 `AI21_AWS_REGION` - The AWS region to use for AWS clients. Defaults to `us-
 east-1`. ## Error Handling --- ```python from ai21 import errors as ai21_errors
 from ai21 import AI21Client, AI21APIError from ai21.models import ChatMessage
 client = AI21Client() system = "You're a support engineer in a SaaS company"
@@ -119,32 +135,28 @@
 the raised error ChatMessage(text="Hello, I need help with a signup process.",
 role="Non-Existent-Role"), ] try: chat_completion = client.chat.create
 ( messages=messages, model="j2-ultra", system=system ) except
 ai21_errors.AI21ServerError as e: print("Server error and could not be
 reached") print(e.details) except ai21_errors.TooManyRequestsError as e: print
 ("A 429 status code was returned. Slow down on the requests") except
 AI21APIError as e: print("A non 200 status code error. For more error types see
-ai21.errors") ``` ## AWS Clients --- AI21 Library provides convenient ways to
-interact with two AWS clients for use with AWS SageMaker and AWS Bedrock. ###
-Installation --- ```bash pip install "ai21[AWS]" ``` This will make sure you
-have the required dependencies installed, including `boto3 >= 1.28.82`. ###
-Usage --- #### SageMaker ```python from ai21 import AI21SageMakerClient client
-= AI21SageMakerClient(endpoint_name="j2-endpoint-name") response =
-client.summarize.create( source="Text to summarize", source_type="TEXT", )
-print(response.summary) ``` #### With Boto3 Session ```python from ai21 import
-AI21SageMakerClient import boto3 boto_session = boto3.Session(region_name="us-
-east-1") client = AI21SageMakerClient( session=boto_session, endpoint_name="j2-
-endpoint-name", ) ``` #### Bedrock --- ```python from ai21 import
-AI21BedrockClient, BedrockModelID client = AI21BedrockClient(region='us-east-
-1') # region is optional, as you can use the env variable instead response =
-client.completion.create( prompt="Your prompt here",
-model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print(response.completions
-[0].data.text) ``` #### With Boto3 Session ```python from ai21 import
-AI21BedrockClient, BedrockModelID import boto3 boto_session = boto3.Session
-(region_name="us-east-1") client = AI21BedrockClient( session=boto_session, )
-response = client.completion.create( prompt="Your prompt here",
-model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` ## Examples Explore our
-examples to see our models in action! We've put together a variety of use cases
-and demonstrations to showcase the capabilities and functionality of our
-models. ### [Check out the Examples](examples/) Feel free to dive in,
-experiment, and adapt these examples to suit your needs. We believe they'll
-help you get up and running quickly. Happy prompting! ð
+ai21.errors") ``` ## Cloud Providers --- ### AWS AI21 Library provides
+convenient ways to interact with two AWS clients for use with AWS SageMaker and
+AWS Bedrock. ### Installation --- ```bash pip install "ai21[AWS]" ``` This will
+make sure you have the required dependencies installed, including `boto3 >=
+1.28.82`. ### Usage --- #### SageMaker ```python from ai21 import
+AI21SageMakerClient client = AI21SageMakerClient(endpoint_name="j2-endpoint-
+name") response = client.summarize.create( source="Text to summarize",
+source_type="TEXT", ) print(response.summary) ``` #### With Boto3 Session
+```python from ai21 import AI21SageMakerClient import boto3 boto_session =
+boto3.Session(region_name="us-east-1") client = AI21SageMakerClient
+( session=boto_session, endpoint_name="j2-endpoint-name", ) ``` #### Bedrock --
+- ```python from ai21 import AI21BedrockClient, BedrockModelID client =
+AI21BedrockClient(region='us-east-1') # region is optional, as you can use the
+env variable instead response = client.completion.create( prompt="Your prompt
+here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) print
+(response.completions[0].data.text) ``` #### With Boto3 Session ```python from
+ai21 import AI21BedrockClient, BedrockModelID import boto3 boto_session =
+boto3.Session(region_name="us-east-1") client = AI21BedrockClient
+( session=boto_session, ) response = client.completion.create( prompt="Your
+prompt here", model_id=BedrockModelID.J2_MID_V1, max_tokens=10, ) ``` Happy
+prompting! ð
```

