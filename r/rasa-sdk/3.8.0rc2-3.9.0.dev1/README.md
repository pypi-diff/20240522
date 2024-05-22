# Comparing `tmp/rasa_sdk-3.8.0rc2.tar.gz` & `tmp/rasa_sdk-3.9.0.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rasa_sdk-3.8.0rc2.tar", max compression
+gzip compressed data, was "rasa_sdk-3.9.0.dev1.tar", max compression
```

## Comparing `rasa_sdk-3.8.0rc2.tar` & `rasa_sdk-3.9.0.dev1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rw-r--r--   0        0        0    11553 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/LICENSE.txt
--rw-r--r--   0        0        0     5282 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/README.md
--rw-r--r--   0        0        0     3266 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/pyproject.toml
--rw-r--r--   0        0        0      420 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/rasa_sdk/__init__.py
--rw-r--r--   0        0        0     1075 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/rasa_sdk/__main__.py
--rw-r--r--   0        0        0        0 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/rasa_sdk/cli/__init__.py
--rw-r--r--   0        0        0     1714 2024-03-15 13:12:45.682959 rasa_sdk-3.8.0rc2/rasa_sdk/cli/arguments.py
--rw-r--r--   0        0        0      487 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/constants.py
--rw-r--r--   0        0        0     7106 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/endpoint.py
--rw-r--r--   0        0        0     6459 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/events.py
--rw-r--r--   0        0        0     1905 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/exceptions.py
--rw-r--r--   0        0        0    15183 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/executor.py
--rw-r--r--   0        0        0    11265 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/forms.py
--rw-r--r--   0        0        0    13092 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/interfaces.py
--rw-r--r--   0        0        0        0 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/__init__.py
--rw-r--r--   0        0        0    10413 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/actions.py
--rw-r--r--   0        0        0     8091 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/storage.py
--rw-r--r--   0        0        0     7266 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/utils.py
--rw-r--r--   0        0        0     1035 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/plugin.py
--rw-r--r--   0        0        0     7066 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/slots.py
--rw-r--r--   0        0        0     6743 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/config.py
--rw-r--r--   0        0        0     1805 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/endpoints.py
--rw-r--r--   0        0        0     2929 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/instrumentation/attribute_extractors.py
--rw-r--r--   0        0        0    11015 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/instrumentation/instrumentation.py
--rw-r--r--   0        0        0      628 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/tracer_register.py
--rw-r--r--   0        0        0     1881 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/tracing/utils.py
--rw-r--r--   0        0        0     1749 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/types.py
--rw-r--r--   0        0        0    11774 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/utils.py
--rw-r--r--   0        0        0      119 2024-03-15 13:12:45.686960 rasa_sdk-3.8.0rc2/rasa_sdk/version.py
--rw-r--r--   0        0        0     7027 1970-01-01 00:00:00.000000 rasa_sdk-3.8.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11553 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/LICENSE.txt
+-rw-r--r--   0        0        0     5282 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/README.md
+-rw-r--r--   0        0        0     3268 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/pyproject.toml
+-rw-r--r--   0        0        0      420 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/__init__.py
+-rw-r--r--   0        0        0     1075 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/cli/__init__.py
+-rw-r--r--   0        0        0     1714 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/cli/arguments.py
+-rw-r--r--   0        0        0      487 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/constants.py
+-rw-r--r--   0        0        0     7106 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/endpoint.py
+-rw-r--r--   0        0        0     6459 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/events.py
+-rw-r--r--   0        0        0     1905 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/exceptions.py
+-rw-r--r--   0        0        0    15183 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/executor.py
+-rw-r--r--   0        0        0    11265 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/forms.py
+-rw-r--r--   0        0        0    13092 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/interfaces.py
+-rw-r--r--   0        0        0        0 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/__init__.py
+-rw-r--r--   0        0        0    10413 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/actions.py
+-rw-r--r--   0        0        0     8091 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/storage.py
+-rw-r--r--   0        0        0     7266 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/utils.py
+-rw-r--r--   0        0        0     1035 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/plugin.py
+-rw-r--r--   0        0        0     7066 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/slots.py
+-rw-r--r--   0        0        0     6743 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/config.py
+-rw-r--r--   0        0        0     1805 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/endpoints.py
+-rw-r--r--   0        0        0     2929 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/instrumentation/attribute_extractors.py
+-rw-r--r--   0        0        0    11015 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/instrumentation/instrumentation.py
+-rw-r--r--   0        0        0      628 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/tracer_register.py
+-rw-r--r--   0        0        0     1881 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/utils.py
+-rw-r--r--   0        0        0     1749 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/types.py
+-rw-r--r--   0        0        0    11774 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/utils.py
+-rw-r--r--   0        0        0      121 2024-05-22 15:37:10.586297 rasa_sdk-3.9.0.dev1/rasa_sdk/version.py
+-rw-r--r--   0        0        0     7029 1970-01-01 00:00:00.000000 rasa_sdk-3.9.0.dev1/PKG-INFO
```

### Comparing `rasa_sdk-3.8.0rc2/LICENSE.txt` & `rasa_sdk-3.9.0.dev1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/README.md` & `rasa_sdk-3.9.0.dev1/README.md`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/pyproject.toml` & `rasa_sdk-3.9.0.dev1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 [tool.black]
 line-length = 88
 target-version = [ "py37", "py38", "py39", "py310",]
 exclude = "((.eggs | .git | .mypy_cache | .pytest_cache | build | dist))"
 
 [tool.poetry]
 name = "rasa-sdk"
-version = "3.8.0rc2"
+version = "3.9.0.dev1"
 description = "Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants"
 authors = [ "Rasa Technologies GmbH <hi@rasa.com>",]
 maintainers = [ "Tom Bocklisch <tom@rasa.com>",]
 homepage = "https://rasa.com"
 repository = "https://github.com/rasahq/rasa-sdk"
 documentation = "https://rasa.com/docs"
 classifiers = [ "Development Status :: 5 - Production/Stable", "Intended Audience :: Developers", "License :: OSI Approved :: Apache Software License", "Topic :: Software Development :: Libraries",]
```

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/__main__.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/cli/arguments.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/cli/arguments.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/endpoint.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/endpoint.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/events.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/events.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/exceptions.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/executor.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/executor.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/forms.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/forms.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/interfaces.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/interfaces.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/actions.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/actions.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/storage.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/storage.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/knowledge_base/utils.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/knowledge_base/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/plugin.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/plugin.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/slots.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/slots.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/config.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/config.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/endpoints.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/endpoints.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/instrumentation/attribute_extractors.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/instrumentation/attribute_extractors.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/instrumentation/instrumentation.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/instrumentation/instrumentation.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/tracer_register.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/tracer_register.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/tracing/utils.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/tracing/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/types.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/types.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/rasa_sdk/utils.py` & `rasa_sdk-3.9.0.dev1/rasa_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `rasa_sdk-3.8.0rc2/PKG-INFO` & `rasa_sdk-3.9.0.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rasa-sdk
-Version: 3.8.0rc2
+Version: 3.9.0.dev1
 Summary: Open source machine learning framework to automate text- and voice-based conversations: NLU, dialogue management, connect to Slack, Facebook, and more - Create chatbots and voice assistants
 Home-page: https://rasa.com
 License: Apache-2.0
 Keywords: nlp,machine-learning,machine-learning-library,bot,bots,botkit,rasa conversational-agents,conversational-ai,chatbot,chatbot-framework,bot-framework
 Author: Rasa Technologies GmbH
 Author-email: hi@rasa.com
 Maintainer: Tom Bocklisch
```

