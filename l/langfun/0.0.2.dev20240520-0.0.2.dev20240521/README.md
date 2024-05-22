# Comparing `tmp/langfun-0.0.2.dev20240520.tar.gz` & `tmp/langfun-0.0.2.dev20240521.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langfun-0.0.2.dev20240520.tar", last modified: Mon May 20 08:04:14 2024, max compression
+gzip compressed data, was "langfun-0.0.2.dev20240521.tar", last modified: Tue May 21 08:04:06 2024, max compression
```

## Comparing `langfun-0.0.2.dev20240520.tar` & `langfun-0.0.2.dev20240521.tar`

### file list

```diff
@@ -1,130 +1,130 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.170641 langfun-0.0.2.dev20240520/langfun/
--rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.178641 langfun-0.0.2.dev20240520/langfun/core/
--rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.178641 langfun-0.0.2.dev20240520/langfun/core/coding/
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.178641 langfun-0.0.2.dev20240520/langfun/core/coding/python/
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/correction.py
--rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/correction_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/errors_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/execution.py
--rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/execution_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/coding/python/permissions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/component.py
--rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/component_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/concurrent.py
--rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/concurrent_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/console.py
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/console_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.182641 langfun-0.0.2.dev20240520/langfun/core/eval/
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/base_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/matching.py
--rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/matching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/patching.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/patching_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/eval/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/langfunc.py
--rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/langfunc_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/language_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/language_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.182641 langfun-0.0.2.dev20240520/langfun/core/llms/
--rw-r--r--   0 runner    (1001) docker     (127)     4175 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/anthropic.py
--rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/anthropic_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.186641 langfun-0.0.2.dev20240520/langfun/core/llms/cache/
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/cache/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/cache/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/cache/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/cache/in_memory_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/fake.py
--rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/fake_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/google_genai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/google_genai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/groq.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/groq_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/llama_cpp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/llama_cpp_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/openai.py
--rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/openai_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9317 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/vertexai.py
--rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/llms/vertexai_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.186641 langfun-0.0.2.dev20240520/langfun/core/memories/
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/memories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/memories/conversation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/memories/conversation_history_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/memory.py
--rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/message.py
--rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/message_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.186641 langfun-0.0.2.dev20240520/langfun/core/modalities/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/image.py
--rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/image_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/mime.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/mime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/video.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modalities/video_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modality.py
--rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/modality_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/natural_language.py
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/natural_language_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/sampling.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/sampling_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/langfun/core/structured/
--rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/description.py
--rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/function_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/function_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/mapping_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/parsing.py
--rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/parsing_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/prompting.py
--rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/prompting_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/schema_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/schema_generation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/structured/scoring_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/subscription_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/template.py
--rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/template_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/langfun/core/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/completion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/completion_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/conversation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/conversation_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/demonstration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/demonstration_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/selfplay.py
--rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/templates/selfplay_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/text_formatting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/langfun/core/text_formatting_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/langfun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-20 08:04:14.000000 langfun-0.0.2.dev20240520/langfun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-20 08:04:14.000000 langfun-0.0.2.dev20240520/langfun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 08:04:14.000000 langfun-0.0.2.dev20240520/langfun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-20 08:04:14.000000 langfun-0.0.2.dev20240520/langfun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-20 08:04:14.000000 langfun-0.0.2.dev20240520/langfun.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 08:04:14.190641 langfun-0.0.2.dev20240520/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-20 08:03:39.000000 langfun-0.0.2.dev20240520/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.670966 langfun-0.0.2.dev20240521/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 08:04:06.666966 langfun-0.0.2.dev20240521/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.646966 langfun-0.0.2.dev20240521/langfun/
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.650966 langfun-0.0.2.dev20240521/langfun/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     4248 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.654966 langfun-0.0.2.dev20240521/langfun/core/coding/
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.654966 langfun-0.0.2.dev20240521/langfun/core/coding/python/
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6589 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/correction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3507 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/correction_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3166 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/errors_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10096 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/execution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7197 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/execution_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7750 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7097 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7386 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2699 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/coding/python/permissions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9909 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8021 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/component_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24537 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/concurrent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15185 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/concurrent_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2317 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/console.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/console_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.658966 langfun-0.0.2.dev20240521/langfun/core/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74268 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26743 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9782 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/matching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5532 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/matching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3866 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/patching.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/patching_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/eval/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11060 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/langfunc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8501 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/langfunc_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20760 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/language_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20122 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/language_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.658966 langfun-0.0.2.dev20240521/langfun/core/llms/
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8505 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/anthropic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5540 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/anthropic_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.662966 langfun-0.0.2.dev20240521/langfun/core/llms/cache/
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/cache/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3338 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/cache/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4742 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/cache/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8747 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/cache/in_memory_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2927 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/fake.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7212 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/fake_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8808 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/google_genai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/google_genai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7844 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/groq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/groq_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2385 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/llama_cpp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1683 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/llama_cpp_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13657 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/openai.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14854 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/openai_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9563 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/vertexai.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7642 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/llms/vertexai_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.662966 langfun-0.0.2.dev20240521/langfun/core/memories/
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/memories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/memories/conversation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2052 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/memories/conversation_history_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15734 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9501 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/message_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.662966 langfun-0.0.2.dev20240521/langfun/core/modalities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2301 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/image_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/mime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/mime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/video.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modalities/video_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modality.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2396 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/modality_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/natural_language.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/natural_language_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5795 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/sampling_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.666966 langfun-0.0.2.dev20240521/langfun/core/structured/
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7299 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19273 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/description.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7362 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/function_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10065 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/function_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12253 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/mapping_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11492 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20895 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/parsing_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8815 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/prompting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21700 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/prompting_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25818 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/schema_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/schema_generation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23078 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2751 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/structured/scoring_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8717 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/subscription_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22284 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15464 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/template_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.666966 langfun-0.0.2.dev20240521/langfun/core/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1931 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/completion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/completion_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3911 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/conversation_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/demonstration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/demonstration_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2273 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/selfplay.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2156 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/templates/selfplay_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5158 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/text_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/langfun/core/text_formatting_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:04:06.666966 langfun-0.0.2.dev20240521/langfun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3443 2024-05-21 08:04:06.000000 langfun-0.0.2.dev20240521/langfun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-21 08:04:06.000000 langfun-0.0.2.dev20240521/langfun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:04:06.000000 langfun-0.0.2.dev20240521/langfun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-05-21 08:04:06.000000 langfun-0.0.2.dev20240521/langfun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-21 08:04:06.000000 langfun-0.0.2.dev20240521/langfun.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 08:04:06.670966 langfun-0.0.2.dev20240521/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 2024-05-21 08:03:34.000000 langfun-0.0.2.dev20240521/setup.py
```

### Comparing `langfun-0.0.2.dev20240520/LICENSE` & `langfun-0.0.2.dev20240521/LICENSE`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/PKG-INFO` & `langfun-0.0.2.dev20240521/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240520
+Version: 0.0.2.dev20240521
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240520/README.md` & `langfun-0.0.2.dev20240521/README.md`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/__init__.py` & `langfun-0.0.2.dev20240521/langfun/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/correction.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/correction.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/correction_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/correction_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/errors.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/errors.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/errors_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/errors_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/execution.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/execution.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/execution_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/execution_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/generation.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/generation_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/parsing.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/parsing_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/permissions.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/permissions.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/coding/python/permissions_test.py` & `langfun-0.0.2.dev20240521/langfun/core/coding/python/permissions_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/component.py` & `langfun-0.0.2.dev20240521/langfun/core/component.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/component_test.py` & `langfun-0.0.2.dev20240521/langfun/core/component_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/concurrent.py` & `langfun-0.0.2.dev20240521/langfun/core/concurrent.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/concurrent_test.py` & `langfun-0.0.2.dev20240521/langfun/core/concurrent_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/console.py` & `langfun-0.0.2.dev20240521/langfun/core/console.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/console_test.py` & `langfun-0.0.2.dev20240521/langfun/core/console_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/base.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/base_test.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/base_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/matching.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/matching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/matching_test.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/matching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/patching.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/patching.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/patching_test.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/patching_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/scoring.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/eval/scoring_test.py` & `langfun-0.0.2.dev20240521/langfun/core/eval/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/langfunc.py` & `langfun-0.0.2.dev20240521/langfun/core/langfunc.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/langfunc_test.py` & `langfun-0.0.2.dev20240521/langfun/core/langfunc_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/language_model.py` & `langfun-0.0.2.dev20240521/langfun/core/language_model.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/language_model_test.py` & `langfun-0.0.2.dev20240521/langfun/core/language_model_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -86,14 +86,15 @@
 from langfun.core.llms.groq import GroqLlama3_8B
 from langfun.core.llms.groq import GroqLlama2_70B
 from langfun.core.llms.groq import GroqMistral_8x7B
 from langfun.core.llms.groq import GroqGemma7B_IT
 
 from langfun.core.llms.vertexai import VertexAI
 from langfun.core.llms.vertexai import VertexAIGeminiPro1_5
+from langfun.core.llms.vertexai import VertexAIGeminiFlash1_5
 from langfun.core.llms.vertexai import VertexAIGeminiPro1
 from langfun.core.llms.vertexai import VertexAIGeminiPro1Vision
 from langfun.core.llms.vertexai import VertexAIPalm2
 from langfun.core.llms.vertexai import VertexAIPalm2_32K
 
 
 # LLaMA C++ models.
```

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/anthropic.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/anthropic.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/anthropic_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/anthropic_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/cache/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/cache/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/cache/base.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/cache/base.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/cache/in_memory.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/cache/in_memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/cache/in_memory_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/cache/in_memory_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/fake.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/fake.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/fake_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/fake_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/google_genai.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/google_genai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/google_genai_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/google_genai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/groq.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/groq.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/groq_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/groq_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/llama_cpp.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/llama_cpp.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/llama_cpp_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/llama_cpp_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/openai.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/openai.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/openai_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/openai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/vertexai.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/vertexai.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 import langfun.core as lf
 from langfun.core import modalities as lf_modalities
 import pyglove as pg
 
 
 SUPPORTED_MODELS_AND_SETTINGS = {
     'gemini-1.5-pro-preview-0409': pg.Dict(api='gemini', rpm=5),
+    'gemini-1.5-flash-preview-0514': pg.Dict(api='gemini', rpm=5),
     'gemini-1.0-pro': pg.Dict(api='gemini', rpm=300),
     'gemini-1.0-pro-vision': pg.Dict(api='gemini', rpm=100),
     # PaLM APIs.
     'text-bison': pg.Dict(api='palm', rpm=1600),
     'text-bison-32k': pg.Dict(api='palm', rpm=300),
     'text-unicorn': pg.Dict(api='palm', rpm=100),
 }
@@ -262,14 +263,21 @@
 class VertexAIGeminiPro1_5(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.5 Pro model."""
 
   model = 'gemini-1.5-pro-preview-0409'
   multimodal = True
 
 
+class VertexAIGeminiFlash1_5(VertexAI):  # pylint: disable=invalid-name
+  """Vertex AI Gemini 1.5 Flash model."""
+
+  model = 'gemini-1.5-flash-preview-0514'
+  multimodal = True
+
+
 class VertexAIGeminiPro1(VertexAI):  # pylint: disable=invalid-name
   """Vertex AI Gemini 1.0 Pro model."""
 
   model = 'gemini-1.0-pro'
 
 
 class VertexAIGeminiPro1Vision(VertexAI):  # pylint: disable=invalid-name
```

### Comparing `langfun-0.0.2.dev20240520/langfun/core/llms/vertexai_test.py` & `langfun-0.0.2.dev20240521/langfun/core/llms/vertexai_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/memories/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/memories/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/memories/conversation_history.py` & `langfun-0.0.2.dev20240521/langfun/core/memories/conversation_history.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/memories/conversation_history_test.py` & `langfun-0.0.2.dev20240521/langfun/core/memories/conversation_history_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/memory.py` & `langfun-0.0.2.dev20240521/langfun/core/memory.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/message.py` & `langfun-0.0.2.dev20240521/langfun/core/message.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/message_test.py` & `langfun-0.0.2.dev20240521/langfun/core/message_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/image.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/image.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/image_test.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/image_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/mime.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/mime.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/mime_test.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/mime_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/video.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/video.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modalities/video_test.py` & `langfun-0.0.2.dev20240521/langfun/core/modalities/video_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modality.py` & `langfun-0.0.2.dev20240521/langfun/core/modality.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/modality_test.py` & `langfun-0.0.2.dev20240521/langfun/core/modality_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/natural_language.py` & `langfun-0.0.2.dev20240521/langfun/core/natural_language.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/natural_language_test.py` & `langfun-0.0.2.dev20240521/langfun/core/natural_language_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/sampling.py` & `langfun-0.0.2.dev20240521/langfun/core/sampling.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/sampling_test.py` & `langfun-0.0.2.dev20240521/langfun/core/sampling_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/completion.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/completion_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/description.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/description.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/description_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/description_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/function_generation.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/function_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/function_generation_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/function_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/mapping.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/mapping.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/mapping_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/mapping_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/parsing.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/parsing.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/parsing_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/parsing_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/prompting.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/prompting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/prompting_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/prompting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/schema.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/schema.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/schema_generation.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/schema_generation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/schema_generation_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/schema_generation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/schema_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/schema_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/scoring.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/scoring.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/structured/scoring_test.py` & `langfun-0.0.2.dev20240521/langfun/core/structured/scoring_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/subscription.py` & `langfun-0.0.2.dev20240521/langfun/core/subscription.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/subscription_test.py` & `langfun-0.0.2.dev20240521/langfun/core/subscription_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/template.py` & `langfun-0.0.2.dev20240521/langfun/core/template.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/template_test.py` & `langfun-0.0.2.dev20240521/langfun/core/template_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/__init__.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/completion.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/completion.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/completion_test.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/completion_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/conversation.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/conversation.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/conversation_test.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/conversation_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/demonstration.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/demonstration.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/demonstration_test.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/demonstration_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/selfplay.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/selfplay.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/templates/selfplay_test.py` & `langfun-0.0.2.dev20240521/langfun/core/templates/selfplay_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/text_formatting.py` & `langfun-0.0.2.dev20240521/langfun/core/text_formatting.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun/core/text_formatting_test.py` & `langfun-0.0.2.dev20240521/langfun/core/text_formatting_test.py`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/langfun.egg-info/PKG-INFO` & `langfun-0.0.2.dev20240521/langfun.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langfun
-Version: 0.0.2.dev20240520
+Version: 0.0.2.dev20240521
 Summary: Langfun: Language as Functions.
 Home-page: https://github.com/google/langfun
 Author: Langfun Authors
 Author-email: langfun-authors@google.com
 License: Apache License 2.0
 Keywords: llm generative-ai machine-learning
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `langfun-0.0.2.dev20240520/langfun.egg-info/SOURCES.txt` & `langfun-0.0.2.dev20240521/langfun.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `langfun-0.0.2.dev20240520/setup.py` & `langfun-0.0.2.dev20240521/setup.py`

 * *Files identical despite different names*

