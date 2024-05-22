# Comparing `tmp/bolna-0.7.8.tar.gz` & `tmp/bolna-0.7.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bolna-0.7.8.tar", last modified: Mon May 20 14:36:33 2024, max compression
+gzip compressed data, was "bolna-0.7.9.tar", last modified: Wed May 22 05:14:08 2024, max compression
```

## Comparing `bolna-0.7.8.tar` & `bolna-0.7.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.279157 bolna-0.7.8/
--rw-r--r--   0 xan        (501) staff       (20)    34522 2024-05-16 15:44:48.000000 bolna-0.7.8/LICENSE
--rw-r--r--   0 xan        (501) staff       (20)    50955 2024-05-20 14:36:33.278889 bolna-0.7.8/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)    10028 2024-05-19 09:18:41.000000 bolna-0.7.8/README.md
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.262924 bolna-0.7.8/bolna/
--rw-r--r--   0 xan        (501) staff       (20)      330 2024-05-20 14:35:00.000000 bolna-0.7.8/bolna/__init__.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.265050 bolna-0.7.8/bolna/agent_manager/
--rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.8/bolna/agent_manager/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3138 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/agent_manager/assistant_manager.py
--rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/agent_manager/base_manager.py
--rw-r--r--   0 xan        (501) staff       (20)    89754 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/agent_manager/task_manager.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.268221 bolna-0.7.8/bolna/agent_types/
--rw-r--r--   0 xan        (501) staff       (20)      302 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/agent_types/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/agent_types/base_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1353 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/contextual_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      590 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/extraction_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     6673 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/graph_based_conversational_agent.py
--rw-r--r--   0 xan        (501) staff       (20)      843 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/agent_types/summarization_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1485 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/agent_types/webhook_agent.py
--rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.8/bolna/assistant.py
--rw-r--r--   0 xan        (501) staff       (20)     1256 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/constants.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.269893 bolna-0.7.8/bolna/helpers/
--rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.8/bolna/helpers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     9978 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/helpers/analytics_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.8/bolna/helpers/cache_helpers.py
--rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.8/bolna/helpers/logger_config.py
--rw-r--r--   0 xan        (501) staff       (20)    18791 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/helpers/utils.py
--rw-r--r--   0 xan        (501) staff       (20)     3929 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/helpers/vad.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.270461 bolna-0.7.8/bolna/input_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      159 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/input_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     3748 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     4617 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.270894 bolna-0.7.8/bolna/input_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)      664 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)      662 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/input_handlers/telephony_providers/twilio.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.271918 bolna-0.7.8/bolna/llms/
--rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.8/bolna/llms/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     4041 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/litellm.py
--rw-r--r--   0 xan        (501) staff       (20)      380 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/llm.py
--rw-r--r--   0 xan        (501) staff       (20)     3584 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/llms/openai_llm.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.259442 bolna-0.7.8/bolna/memory/
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.272832 bolna-0.7.8/bolna/memory/cache/
--rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.8/bolna/memory/cache/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)      161 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/base_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     1014 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/inmemory_scalar_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     1254 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/memory/cache/vector_cache.py
--rw-r--r--   0 xan        (501) staff       (20)     5673 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/models.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.273692 bolna-0.7.8/bolna/output_handlers/
--rw-r--r--   0 xan        (501) staff       (20)      162 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/output_handlers/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1492 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/default.py
--rw-r--r--   0 xan        (501) staff       (20)     2439 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/telephony.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.274111 bolna-0.7.8/bolna/output_handlers/telephony_providers/
--rw-r--r--   0 xan        (501) staff       (20)     1360 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/output_handlers/telephony_providers/exotel.py
--rw-r--r--   0 xan        (501) staff       (20)     2291 2024-05-17 09:22:34.000000 bolna-0.7.8/bolna/output_handlers/telephony_providers/twilio.py
--rw-r--r--   0 xan        (501) staff       (20)     2781 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/prompts.py
--rw-r--r--   0 xan        (501) staff       (20)     1714 2024-05-17 07:22:52.000000 bolna-0.7.8/bolna/providers.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.276330 bolna-0.7.8/bolna/synthesizer/
--rw-r--r--   0 xan        (501) staff       (20)      306 2024-05-17 07:22:52.000000 bolna-0.7.8/bolna/synthesizer/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     1208 2024-05-18 15:13:13.000000 bolna-0.7.8/bolna/synthesizer/base_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     2786 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/deepgram_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)    11230 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/synthesizer/elevenlabs_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.8/bolna/synthesizer/fourie_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     4287 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/openai_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     5577 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/synthesizer/polly_synthesizer.py
--rw-r--r--   0 xan        (501) staff       (20)     7100 2024-05-16 15:44:48.000000 bolna-0.7.8/bolna/synthesizer/xtts_synthesizer.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.278026 bolna-0.7.8/bolna/transcriber/
--rw-r--r--   0 xan        (501) staff       (20)      152 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/transcriber/__init__.py
--rw-r--r--   0 xan        (501) staff       (20)     2242 2024-05-15 20:50:00.000000 bolna-0.7.8/bolna/transcriber/base_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    16323 2024-05-20 13:21:39.000000 bolna-0.7.8/bolna/transcriber/deepgram_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    18909 2024-04-26 13:37:59.000000 bolna-0.7.8/bolna/transcriber/hume_transcriber.py
--rw-r--r--   0 xan        (501) staff       (20)    14620 2024-05-16 17:24:11.000000 bolna-0.7.8/bolna/transcriber/whisper_transcriber.py
-drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-20 14:36:33.278275 bolna-0.7.8/bolna.egg-info/
--rw-r--r--   0 xan        (501) staff       (20)    50955 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/PKG-INFO
--rw-r--r--   0 xan        (501) staff       (20)     2034 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/SOURCES.txt
--rw-r--r--   0 xan        (501) staff       (20)        1 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/dependency_links.txt
--rw-r--r--   0 xan        (501) staff       (20)      387 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/requires.txt
--rw-r--r--   0 xan        (501) staff       (20)        6 2024-05-20 14:36:33.000000 bolna-0.7.8/bolna.egg-info/top_level.txt
--rw-r--r--   0 xan        (501) staff       (20)     1164 2024-05-20 14:35:00.000000 bolna-0.7.8/pyproject.toml
--rw-r--r--   0 xan        (501) staff       (20)      370 2024-05-16 15:44:48.000000 bolna-0.7.8/requirements.txt
--rw-r--r--   0 xan        (501) staff       (20)       38 2024-05-20 14:36:33.279210 bolna-0.7.8/setup.cfg
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.047939 bolna-0.7.9/
+-rw-r--r--   0 xan        (501) staff       (20)     1048 2024-05-22 05:05:13.000000 bolna-0.7.9/LICENSE
+-rw-r--r--   0 xan        (501) staff       (20)    12328 2024-05-22 05:14:08.047669 bolna-0.7.9/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)    10028 2024-05-22 05:05:08.000000 bolna-0.7.9/README.md
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.033991 bolna-0.7.9/bolna/
+-rw-r--r--   0 xan        (501) staff       (20)      330 2024-05-22 05:09:53.000000 bolna-0.7.9/bolna/__init__.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.035655 bolna-0.7.9/bolna/agent_manager/
+-rw-r--r--   0 xan        (501) staff       (20)      124 2024-01-07 06:26:49.000000 bolna-0.7.9/bolna/agent_manager/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3138 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/agent_manager/assistant_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)      174 2024-01-07 16:40:54.000000 bolna-0.7.9/bolna/agent_manager/base_manager.py
+-rw-r--r--   0 xan        (501) staff       (20)    89754 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/agent_manager/task_manager.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.038056 bolna-0.7.9/bolna/agent_types/
+-rw-r--r--   0 xan        (501) staff       (20)      302 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/agent_types/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      176 2024-01-07 16:40:54.000000 bolna-0.7.9/bolna/agent_types/base_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1353 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/agent_types/contextual_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      590 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/agent_types/extraction_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     6673 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/agent_types/graph_based_conversational_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)      843 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/agent_types/summarization_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1485 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/agent_types/webhook_agent.py
+-rw-r--r--   0 xan        (501) staff       (20)     1807 2024-01-19 12:02:21.000000 bolna-0.7.9/bolna/assistant.py
+-rw-r--r--   0 xan        (501) staff       (20)     1256 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/constants.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.039027 bolna-0.7.9/bolna/helpers/
+-rw-r--r--   0 xan        (501) staff       (20)        0 2023-12-23 18:13:48.000000 bolna-0.7.9/bolna/helpers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     9978 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/helpers/analytics_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)        0 2024-01-12 18:42:30.000000 bolna-0.7.9/bolna/helpers/cache_helpers.py
+-rw-r--r--   0 xan        (501) staff       (20)      548 2024-01-07 16:40:54.000000 bolna-0.7.9/bolna/helpers/logger_config.py
+-rw-r--r--   0 xan        (501) staff       (20)    18791 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/helpers/utils.py
+-rw-r--r--   0 xan        (501) staff       (20)     3929 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/helpers/vad.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.039491 bolna-0.7.9/bolna/input_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      159 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/input_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     3748 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/input_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     4617 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/input_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.039984 bolna-0.7.9/bolna/input_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)      664 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/input_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)      662 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/input_handlers/telephony_providers/twilio.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.040719 bolna-0.7.9/bolna/llms/
+-rw-r--r--   0 xan        (501) staff       (20)       63 2023-12-23 22:38:43.000000 bolna-0.7.9/bolna/llms/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     4041 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/llms/litellm.py
+-rw-r--r--   0 xan        (501) staff       (20)      380 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/llms/llm.py
+-rw-r--r--   0 xan        (501) staff       (20)     3584 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/llms/openai_llm.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.031459 bolna-0.7.9/bolna/memory/
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.041426 bolna-0.7.9/bolna/memory/cache/
+-rw-r--r--   0 xan        (501) staff       (20)       54 2024-01-12 18:42:30.000000 bolna-0.7.9/bolna/memory/cache/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)      161 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/memory/cache/base_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1014 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/memory/cache/inmemory_scalar_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     1254 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/memory/cache/vector_cache.py
+-rw-r--r--   0 xan        (501) staff       (20)     5673 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/models.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.041896 bolna-0.7.9/bolna/output_handlers/
+-rw-r--r--   0 xan        (501) staff       (20)      162 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/output_handlers/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1492 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/output_handlers/default.py
+-rw-r--r--   0 xan        (501) staff       (20)     2439 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/output_handlers/telephony.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.042210 bolna-0.7.9/bolna/output_handlers/telephony_providers/
+-rw-r--r--   0 xan        (501) staff       (20)     1360 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/output_handlers/telephony_providers/exotel.py
+-rw-r--r--   0 xan        (501) staff       (20)     2291 2024-05-17 09:22:34.000000 bolna-0.7.9/bolna/output_handlers/telephony_providers/twilio.py
+-rw-r--r--   0 xan        (501) staff       (20)     2781 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/prompts.py
+-rw-r--r--   0 xan        (501) staff       (20)     1714 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/providers.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.045782 bolna-0.7.9/bolna/synthesizer/
+-rw-r--r--   0 xan        (501) staff       (20)      306 2024-05-17 07:22:52.000000 bolna-0.7.9/bolna/synthesizer/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     1208 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/synthesizer/base_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     2786 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/synthesizer/deepgram_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)    11230 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/synthesizer/elevenlabs_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     3483 2024-02-04 09:51:18.000000 bolna-0.7.9/bolna/synthesizer/fourie_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     4287 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/synthesizer/openai_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     5577 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/synthesizer/polly_synthesizer.py
+-rw-r--r--   0 xan        (501) staff       (20)     7100 2024-05-16 15:44:48.000000 bolna-0.7.9/bolna/synthesizer/xtts_synthesizer.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.047015 bolna-0.7.9/bolna/transcriber/
+-rw-r--r--   0 xan        (501) staff       (20)      152 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/transcriber/__init__.py
+-rw-r--r--   0 xan        (501) staff       (20)     2242 2024-05-15 20:50:00.000000 bolna-0.7.9/bolna/transcriber/base_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    16323 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/transcriber/deepgram_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    18909 2024-04-26 13:37:59.000000 bolna-0.7.9/bolna/transcriber/hume_transcriber.py
+-rw-r--r--   0 xan        (501) staff       (20)    14620 2024-05-22 05:05:08.000000 bolna-0.7.9/bolna/transcriber/whisper_transcriber.py
+drwxr-xr-x   0 xan        (501) staff       (20)        0 2024-05-22 05:14:08.047227 bolna-0.7.9/bolna.egg-info/
+-rw-r--r--   0 xan        (501) staff       (20)    12328 2024-05-22 05:14:08.000000 bolna-0.7.9/bolna.egg-info/PKG-INFO
+-rw-r--r--   0 xan        (501) staff       (20)     2034 2024-05-22 05:14:08.000000 bolna-0.7.9/bolna.egg-info/SOURCES.txt
+-rw-r--r--   0 xan        (501) staff       (20)        1 2024-05-22 05:14:08.000000 bolna-0.7.9/bolna.egg-info/dependency_links.txt
+-rw-r--r--   0 xan        (501) staff       (20)      387 2024-05-22 05:14:08.000000 bolna-0.7.9/bolna.egg-info/requires.txt
+-rw-r--r--   0 xan        (501) staff       (20)        6 2024-05-22 05:14:08.000000 bolna-0.7.9/bolna.egg-info/top_level.txt
+-rw-r--r--   0 xan        (501) staff       (20)     1139 2024-05-22 05:09:53.000000 bolna-0.7.9/pyproject.toml
+-rw-r--r--   0 xan        (501) staff       (20)      370 2024-05-16 15:44:48.000000 bolna-0.7.9/requirements.txt
+-rw-r--r--   0 xan        (501) staff       (20)       38 2024-05-22 05:14:08.047978 bolna-0.7.9/setup.cfg
```

### Comparing `bolna-0.7.8/README.md` & `bolna-0.7.9/README.md`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_manager/assistant_manager.py` & `bolna-0.7.9/bolna/agent_manager/assistant_manager.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_manager/task_manager.py` & `bolna-0.7.9/bolna/agent_manager/task_manager.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_types/contextual_conversational_agent.py` & `bolna-0.7.9/bolna/agent_types/contextual_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_types/extraction_agent.py` & `bolna-0.7.9/bolna/agent_types/extraction_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_types/graph_based_conversational_agent.py` & `bolna-0.7.9/bolna/agent_types/graph_based_conversational_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_types/summarization_agent.py` & `bolna-0.7.9/bolna/agent_types/summarization_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/agent_types/webhook_agent.py` & `bolna-0.7.9/bolna/agent_types/webhook_agent.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/assistant.py` & `bolna-0.7.9/bolna/assistant.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/constants.py` & `bolna-0.7.9/bolna/constants.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/helpers/analytics_helpers.py` & `bolna-0.7.9/bolna/helpers/analytics_helpers.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/helpers/logger_config.py` & `bolna-0.7.9/bolna/helpers/logger_config.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/helpers/utils.py` & `bolna-0.7.9/bolna/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/helpers/vad.py` & `bolna-0.7.9/bolna/helpers/vad.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/input_handlers/default.py` & `bolna-0.7.9/bolna/input_handlers/default.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/input_handlers/telephony.py` & `bolna-0.7.9/bolna/input_handlers/telephony.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/input_handlers/telephony_providers/exotel.py` & `bolna-0.7.9/bolna/input_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/input_handlers/telephony_providers/twilio.py` & `bolna-0.7.9/bolna/input_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/llms/litellm.py` & `bolna-0.7.9/bolna/llms/litellm.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/llms/openai_llm.py` & `bolna-0.7.9/bolna/llms/openai_llm.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/memory/cache/inmemory_scalar_cache.py` & `bolna-0.7.9/bolna/memory/cache/inmemory_scalar_cache.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/memory/cache/vector_cache.py` & `bolna-0.7.9/bolna/memory/cache/vector_cache.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/models.py` & `bolna-0.7.9/bolna/models.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/output_handlers/default.py` & `bolna-0.7.9/bolna/output_handlers/default.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/output_handlers/telephony.py` & `bolna-0.7.9/bolna/output_handlers/telephony.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/output_handlers/telephony_providers/exotel.py` & `bolna-0.7.9/bolna/output_handlers/telephony_providers/exotel.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/output_handlers/telephony_providers/twilio.py` & `bolna-0.7.9/bolna/output_handlers/telephony_providers/twilio.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/prompts.py` & `bolna-0.7.9/bolna/prompts.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/providers.py` & `bolna-0.7.9/bolna/providers.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/base_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/base_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/deepgram_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/deepgram_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/elevenlabs_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/elevenlabs_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/fourie_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/fourie_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/openai_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/openai_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/polly_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/polly_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/synthesizer/xtts_synthesizer.py` & `bolna-0.7.9/bolna/synthesizer/xtts_synthesizer.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/transcriber/base_transcriber.py` & `bolna-0.7.9/bolna/transcriber/base_transcriber.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/transcriber/deepgram_transcriber.py` & `bolna-0.7.9/bolna/transcriber/deepgram_transcriber.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/transcriber/hume_transcriber.py` & `bolna-0.7.9/bolna/transcriber/hume_transcriber.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna/transcriber/whisper_transcriber.py` & `bolna-0.7.9/bolna/transcriber/whisper_transcriber.py`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/bolna.egg-info/SOURCES.txt` & `bolna-0.7.9/bolna.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bolna-0.7.8/pyproject.toml` & `bolna-0.7.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "bolna"
-version = "0.7.8"
+version = "0.7.9"
 readme = "README.md"
 authors = [
     { name = "Prateek Sachan", email = "ps@prateeksachan.com" }
 ]
 license = { file = "LICENSE" }
 classifiers = [
-    "License :: OSI Approved :: GNU Affero General Public License v3",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
 dynamic = ["dependencies"]
 requires-python = ">=3.8"
 
 [project.optional-dependencies]
@@ -26,15 +26,15 @@
 [tool.setuptools]
 package-dir = {"bolna" = "bolna"}
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [tool.bumpver]
-current_version = "0.7.8"
+current_version = "0.7.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump bolna version {old_version} -> {new_version}"
 tag_message = "bolna-{new_version}"
 tag_scope = "default"
 pre_commit_hook = ""
 post_commit_hook = ""
 commit = true
```

