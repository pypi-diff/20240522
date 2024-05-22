# Comparing `tmp/tokencost-0.1.7.tar.gz` & `tmp/tokencost-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokencost-0.1.7.tar", last modified: Wed Mar 27 21:14:34 2024, max compression
+gzip compressed data, was "tokencost-0.1.8.tar", last modified: Wed May 22 01:06:46 2024, max compression
```

## Comparing `tokencost-0.1.7.tar` & `tokencost-0.1.8.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:34.478331 tokencost-0.1.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-03-27 21:14:29.000000 tokencost-0.1.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-27 21:14:29.000000 tokencost-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-27 21:14:34.478331 tokencost-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15446 2024-03-27 21:14:29.000000 tokencost-0.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-03-27 21:14:29.000000 tokencost-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 21:14:34.478331 tokencost-0.1.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:34.474331 tokencost-0.1.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-03-27 21:14:29.000000 tokencost-0.1.7/tests/test_costs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-03-27 21:14:29.000000 tokencost-0.1.7/tests/test_llama_index_callbacks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:34.474331 tokencost-0.1.7/tokencost/
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:34.474331 tokencost-0.1.7/tokencost/callbacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/callbacks/llama_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/costs.py
--rw-r--r--   0 runner    (1001) docker     (127)    93463 2024-03-27 21:14:29.000000 tokencost-0.1.7/tokencost/model_prices.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 21:14:34.474331 tokencost-0.1.7/tokencost.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16384 2024-03-27 21:14:34.000000 tokencost-0.1.7/tokencost.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-03-27 21:14:34.000000 tokencost-0.1.7/tokencost.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 21:14:34.000000 tokencost-0.1.7/tokencost.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-27 21:14:34.000000 tokencost-0.1.7/tokencost.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-03-27 21:14:34.000000 tokencost-0.1.7/tokencost.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:46.032980 tokencost-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 01:06:39.000000 tokencost-0.1.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 01:06:39.000000 tokencost-0.1.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    77193 2024-05-22 01:06:46.032980 tokencost-0.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    76255 2024-05-22 01:06:39.000000 tokencost-0.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 01:06:39.000000 tokencost-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:06:46.032980 tokencost-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:46.028980 tokencost-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2024-05-22 01:06:39.000000 tokencost-0.1.8/tests/test_costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-22 01:06:39.000000 tokencost-0.1.8/tests/test_llama_index_callbacks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:46.028980 tokencost-0.1.8/tokencost/
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:46.028980 tokencost-0.1.8/tokencost/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/callbacks/llama_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6656 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/costs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   114581 2024-05-22 01:06:39.000000 tokencost-0.1.8/tokencost/model_prices.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:06:46.032980 tokencost-0.1.8/tokencost.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    77193 2024-05-22 01:06:46.000000 tokencost-0.1.8/tokencost.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-22 01:06:46.000000 tokencost-0.1.8/tokencost.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:06:46.000000 tokencost-0.1.8/tokencost.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-22 01:06:46.000000 tokencost-0.1.8/tokencost.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 01:06:46.000000 tokencost-0.1.8/tokencost.egg-info/top_level.txt
```

### Comparing `tokencost-0.1.7/LICENSE` & `tokencost-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/pyproject.toml` & `tokencost-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 include-package-data = true
 
 [tool.setuptools.package-data]
 tokencost = ["model_prices.json"]
 
 [project]
 name = "tokencost"
-version = "0.1.7"
+version = "0.1.8"
 authors = [
   { name = "Trisha Pan", email = "trishaepan@gmail.com" },
   { name = "Alex Reibman", email = "areibman@gmail.com" },
 ]
 description = "To calculate token and translated USD cost of string and message calls to OpenAI, for example when used by AI agents"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-    "tiktoken>=0.5.2",
+    "tiktoken>=0.7.0",
     "aiohttp>=3.9.3"
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest>=7.4.4",
     "flake8>=3.1.0",
```

### Comparing `tokencost-0.1.7/tests/test_costs.py` & `tokencost-0.1.8/tests/test_costs.py`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/tests/test_llama_index_callbacks.py` & `tokencost-0.1.8/tests/test_llama_index_callbacks.py`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/tokencost/callbacks/llama_index.py` & `tokencost-0.1.8/tokencost/callbacks/llama_index.py`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/tokencost/constants.py` & `tokencost-0.1.8/tokencost/constants.py`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/tokencost/costs.py` & `tokencost-0.1.8/tokencost/costs.py`

 * *Files identical despite different names*

### Comparing `tokencost-0.1.7/tokencost/model_prices.json` & `tokencost-0.1.8/tokencost/model_prices.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7880351324068601%*

 * *Differences: {"'amazon.titan-embed-text-v2:0'": "OrderedDict([('max_tokens', 8192), ('max_input_tokens', 8192), "*

 * *                                   "('output_vector_size', 1024), ('input_cost_per_token', 2e-07), "*

 * *                                   "('output_cost_per_token', 0.0), ('litellm_provider', "*

 * *                                   "'bedrock'), ('mode', 'embedding')])",*

 * * "'anthropic.claude-3-haiku-20240307-v1:0'": "{'supports_function_calling': True, "*

 * *                                             "'supports_visio […]*

```diff
@@ -68,14 +68,23 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 8192,
         "max_tokens": 8192,
         "mode": "embedding",
         "output_cost_per_token": 0.0,
         "output_vector_size": 1536
     },
+    "amazon.titan-embed-text-v2:0": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1024
+    },
     "amazon.titan-text-express-v1": {
         "input_cost_per_token": 1.3e-06,
         "litellm_provider": "bedrock",
         "max_input_tokens": 42000,
         "max_output_tokens": 8000,
         "max_tokens": 8000,
         "mode": "chat",
@@ -93,24 +102,39 @@
     "anthropic.claude-3-haiku-20240307-v1:0": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "bedrock",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-06
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "anthropic.claude-3-opus-20240229-v1:0": {
+        "input_cost_per_token": 1.5e-05,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "anthropic.claude-3-sonnet-20240229-v1:0": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "bedrock",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-05
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "anthropic.claude-instant-v1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
@@ -213,14 +237,24 @@
         "input_cost_per_token": 1e-07,
         "litellm_provider": "azure",
         "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "azure/command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "azure",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true
+    },
     "azure/gpt-3.5-turbo-instruct-0914": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "text-completion-openai",
         "max_input_tokens": 4097,
         "max_tokens": 4097,
         "mode": "completion",
         "output_cost_per_token": 2e-06
@@ -351,22 +385,35 @@
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
+    "azure/gpt-4-turbo-2024-04-09": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "azure",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
     "azure/gpt-4-turbo-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "azure",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
     },
     "azure/hd/1024-x-1024/dall-e-3": {
         "input_cost_per_pixel": 7.629e-08,
         "litellm_provider": "azure",
         "mode": "image_generation",
         "output_cost_per_token": 0.0
     },
@@ -711,14 +758,41 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
+    "bedrock/eu-west-3/mistral.mistral-7b-instruct-v0:2": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.6e-07
+    },
+    "bedrock/eu-west-3/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 1.04e-05,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 3.12e-05
+    },
+    "bedrock/eu-west-3/mistral.mixtral-8x7b-instruct-v0:1": {
+        "input_cost_per_token": 5.9e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 9.1e-07
+    },
     "bedrock/us-east-1/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.011,
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
@@ -819,14 +893,41 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
+    "bedrock/us-east-1/mistral.mistral-7b-instruct-v0:2": {
+        "input_cost_per_token": 1.5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2e-07
+    },
+    "bedrock/us-east-1/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "bedrock/us-east-1/mistral.mixtral-8x7b-instruct-v0:1": {
+        "input_cost_per_token": 4.5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 7e-07
+    },
     "bedrock/us-west-2/1-month-commitment/anthropic.claude-instant-v1": {
         "input_cost_per_second": 0.011,
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
@@ -927,24 +1028,33 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2.4e-05
     },
-    "bedrock/us-west-2/mistral.mistral-7b-instruct": {
+    "bedrock/us-west-2/mistral.mistral-7b-instruct-v0:2": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "bedrock",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
-    "bedrock/us-west-2/mistral.mixtral-8x7b-instruct": {
+    "bedrock/us-west-2/mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "bedrock/us-west-2/mistral.mixtral-8x7b-instruct-v0:1": {
         "input_cost_per_token": 4.5e-07,
         "litellm_provider": "bedrock",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 7e-07
@@ -1019,33 +1129,42 @@
     "claude-3-haiku-20240307": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "anthropic",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.25e-06
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 264
     },
     "claude-3-opus-20240229": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "anthropic",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 7.5e-05
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 395
     },
     "claude-3-sonnet-20240229": {
         "input_cost_per_token": 3e-06,
         "litellm_provider": "anthropic",
         "max_input_tokens": 200000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 1.5e-05
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 159
     },
     "claude-instant-1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "anthropic",
         "max_input_tokens": 100000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
@@ -1182,14 +1301,32 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 6e-07
     },
+    "cohere.command-r-plus-v1:0": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05
+    },
+    "cohere.command-r-v1:0": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-06
+    },
     "cohere.command-text-v14": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "bedrock",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
@@ -1253,14 +1390,24 @@
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-06,
         "supports_function_calling": true
     },
+    "command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "cohere_chat",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true
+    },
     "command-xlarge-beta": {
         "input_cost_per_token": 1.5e-05,
         "litellm_provider": "cohere",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
@@ -1433,14 +1580,32 @@
         "litellm_provider": "deepinfra",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
+    "deepseek-chat": {
+        "input_cost_per_token": 1.4e-07,
+        "litellm_provider": "deepseek",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.8e-07
+    },
+    "deepseek-coder": {
+        "input_cost_per_token": 1.4e-07,
+        "litellm_provider": "deepseek",
+        "max_input_tokens": 16000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.8e-07
+    },
     "dolphin": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "nlp_cloud",
         "max_input_tokens": 16384,
         "max_output_tokens": 16384,
         "max_tokens": 16384,
         "mode": "completion",
@@ -1462,77 +1627,113 @@
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 5e-07,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
         "supports_function_calling": true
     },
+    "gemini-1.0-pro-001": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
+    },
+    "gemini-1.0-pro-002": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 32760,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true
+    },
     "gemini-1.0-pro-vision": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-vision-models",
         "max_images_per_prompt": 16,
         "max_input_tokens": 16384,
         "max_output_tokens": 2048,
         "max_tokens": 2048,
         "max_video_length": 2,
         "max_videos_per_prompt": 1,
         "mode": "chat",
         "output_cost_per_token": 5e-07,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gemini-1.0-pro-vision-001": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-vision-models",
         "max_images_per_prompt": 16,
         "max_input_tokens": 16384,
         "max_output_tokens": 2048,
         "max_tokens": 2048,
         "max_video_length": 2,
         "max_videos_per_prompt": 1,
         "mode": "chat",
         "output_cost_per_token": 5e-07,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gemini-1.5-pro": {
-        "input_cost_per_token": 0,
+        "input_cost_per_token": 6.25e-07,
         "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0,
+        "output_cost_per_token": 1.875e-06,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_tool_choice": true
     },
     "gemini-1.5-pro-preview-0215": {
-        "input_cost_per_token": 0,
+        "input_cost_per_token": 6.25e-07,
         "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 0,
+        "output_cost_per_token": 1.875e-06,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_tool_choice": true
+    },
+    "gemini-1.5-pro-preview-0409": {
+        "input_cost_per_token": 6.25e-07,
+        "litellm_provider": "vertex_ai-language-models",
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1.875e-06,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
+        "supports_function_calling": true,
+        "supports_tool_choice": true
     },
-    "gemini-1.5-pro-vision": {
+    "gemini-experimental": {
         "input_cost_per_token": 0,
-        "litellm_provider": "vertex_ai-vision-models",
-        "max_images_per_prompt": 16,
+        "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
-        "max_video_length": 2,
-        "max_videos_per_prompt": 1,
         "mode": "chat",
         "output_cost_per_token": 0,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": false,
+        "supports_tool_choice": true
     },
     "gemini-pro": {
         "input_cost_per_token": 2.5e-07,
         "litellm_provider": "vertex_ai-language-models",
         "max_input_tokens": 32760,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
@@ -1549,37 +1750,42 @@
         "max_output_tokens": 2048,
         "max_tokens": 2048,
         "max_video_length": 2,
         "max_videos_per_prompt": 1,
         "mode": "chat",
         "output_cost_per_token": 5e-07,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gemini/gemini-1.5-pro": {
         "input_cost_per_token": 0,
         "litellm_provider": "gemini",
         "max_input_tokens": 1000000,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 0,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_tool_choice": true,
+        "supports_vision": true
     },
-    "gemini/gemini-1.5-pro-vision": {
+    "gemini/gemini-1.5-pro-latest": {
         "input_cost_per_token": 0,
         "litellm_provider": "gemini",
-        "max_input_tokens": 1000000,
+        "max_input_tokens": 1048576,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 0,
-        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "source": "https://ai.google.dev/models/gemini",
+        "supports_function_calling": true,
+        "supports_tool_choice": true,
+        "supports_vision": true
     },
     "gemini/gemini-pro": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "gemini",
         "max_input_tokens": 32760,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
@@ -1593,15 +1799,16 @@
         "litellm_provider": "gemini",
         "max_input_tokens": 30720,
         "max_output_tokens": 2048,
         "max_tokens": 2048,
         "mode": "chat",
         "output_cost_per_token": 0.0,
         "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models",
-        "supports_function_calling": true
+        "supports_function_calling": true,
+        "supports_vision": true
     },
     "gpt-3.5-turbo": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "openai",
         "max_input_tokens": 16385,
         "max_output_tokens": 4096,
         "max_tokens": 4097,
@@ -1740,15 +1947,16 @@
     "gpt-4-1106-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
     },
     "gpt-4-32k": {
         "input_cost_per_token": 6e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
@@ -1769,60 +1977,132 @@
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.00012
     },
+    "gpt-4-turbo": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
+    "gpt-4-turbo-2024-04-09": {
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
     "gpt-4-turbo-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
-        "max_input_tokens": 8192,
+        "max_input_tokens": 128000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 3e-05,
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
     "gpt-4-vision-preview": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "openai",
         "max_input_tokens": 128000,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 3e-05
+        "output_cost_per_token": 3e-05,
+        "supports_vision": true
+    },
+    "gpt-4o": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
+    },
+    "gpt-4o-2024-05-13": {
+        "input_cost_per_token": 5e-06,
+        "litellm_provider": "openai",
+        "max_input_tokens": 128000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_parallel_function_calling": true,
+        "supports_vision": true
     },
     "groq/gemma-7b-it": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "groq",
         "max_input_tokens": 8192,
         "max_output_tokens": 8192,
         "max_tokens": 8192,
         "mode": "chat",
-        "output_cost_per_token": 1e-07
+        "output_cost_per_token": 1e-07,
+        "supports_function_calling": true
     },
     "groq/llama2-70b-4096": {
         "input_cost_per_token": 7e-07,
         "litellm_provider": "groq",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
-        "output_cost_per_token": 8e-07
+        "output_cost_per_token": 8e-07,
+        "supports_function_calling": true
+    },
+    "groq/llama3-70b-8192": {
+        "input_cost_per_token": 6.4e-07,
+        "litellm_provider": "groq",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 8e-07,
+        "supports_function_calling": true
+    },
+    "groq/llama3-8b-8192": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "groq",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 1e-07,
+        "supports_function_calling": true
     },
     "groq/mixtral-8x7b-32768": {
         "input_cost_per_token": 2.7e-07,
         "litellm_provider": "groq",
         "max_input_tokens": 32768,
         "max_output_tokens": 32768,
         "max_tokens": 32768,
         "mode": "chat",
-        "output_cost_per_token": 2.7e-07
+        "output_cost_per_token": 2.7e-07,
+        "supports_function_calling": true
     },
     "hd/1024-x-1024/dall-e-3": {
         "input_cost_per_pixel": 7.629e-08,
         "litellm_provider": "openai",
         "mode": "image_generation",
         "output_cost_per_pixel": 0.0
     },
@@ -1935,24 +2215,51 @@
         "litellm_provider": "bedrock",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2.56e-06
     },
+    "meta.llama3-70b-instruct-v1:0": {
+        "input_cost_per_token": 2.65e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 3.5e-06
+    },
+    "meta.llama3-8b-instruct-v1:0": {
+        "input_cost_per_token": 4e-07,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 8192,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 6e-07
+    },
     "mistral.mistral-7b-instruct-v0:2": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "bedrock",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
-    "mistral.mixtral-8x7b-instruct": {
+    "mistral.mistral-large-2402-v1:0": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "bedrock",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "mistral.mixtral-8x7b-instruct-v0:1": {
         "input_cost_per_token": 4.5e-07,
         "litellm_provider": "bedrock",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 7e-07
@@ -2014,34 +2321,46 @@
     "mistral/mistral-small": {
         "input_cost_per_token": 2e-06,
         "litellm_provider": "mistral",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
-        "output_cost_per_token": 6e-06
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
     },
     "mistral/mistral-small-latest": {
         "input_cost_per_token": 2e-06,
         "litellm_provider": "mistral",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
-        "output_cost_per_token": 6e-06
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
     },
     "mistral/mistral-tiny": {
         "input_cost_per_token": 1.5e-07,
         "litellm_provider": "mistral",
         "max_input_tokens": 32000,
         "max_output_tokens": 8191,
         "max_tokens": 8191,
         "mode": "chat",
         "output_cost_per_token": 4.6e-07
     },
+    "mistral/open-mixtral-8x7b": {
+        "input_cost_per_token": 2e-06,
+        "litellm_provider": "mistral",
+        "max_input_tokens": 32000,
+        "max_output_tokens": 8191,
+        "max_tokens": 8191,
+        "mode": "chat",
+        "output_cost_per_token": 6e-06,
+        "supports_function_calling": true
+    },
     "ollama/codellama": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "ollama",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
@@ -2114,33 +2433,115 @@
         "input_cost_per_token": 1.102e-05,
         "litellm_provider": "openrouter",
         "max_output_tokens": 8191,
         "max_tokens": 100000,
         "mode": "chat",
         "output_cost_per_token": 3.268e-05
     },
+    "openrouter/anthropic/claude-3-haiku": {
+        "input_cost_per_image": 0.0004,
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 200000,
+        "mode": "chat",
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/anthropic/claude-3-opus": {
+        "input_cost_per_token": 1.5e-05,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true,
+        "tool_use_system_prompt_tokens": 395
+    },
+    "openrouter/anthropic/claude-3-sonnet": {
+        "input_cost_per_image": 0.0048,
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 200000,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/anthropic/claude-instant-v1": {
         "input_cost_per_token": 1.63e-06,
         "litellm_provider": "openrouter",
         "max_output_tokens": 8191,
         "max_tokens": 100000,
         "mode": "chat",
         "output_cost_per_token": 5.51e-06
     },
+    "openrouter/cognitivecomputations/dolphin-mixtral-8x7b": {
+        "input_cost_per_token": 5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32769,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "openrouter/cohere/command-r-plus": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 128000,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05
+    },
+    "openrouter/databricks/dbrx-instruct": {
+        "input_cost_per_token": 6e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32768,
+        "mode": "chat",
+        "output_cost_per_token": 6e-07
+    },
+    "openrouter/fireworks/firellava-13b": {
+        "input_cost_per_token": 2e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2e-07
+    },
+    "openrouter/google/gemini-pro-1.5": {
+        "input_cost_per_image": 0.00265,
+        "input_cost_per_token": 2.5e-06,
+        "litellm_provider": "openrouter",
+        "max_input_tokens": 1000000,
+        "max_output_tokens": 8192,
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "openrouter/google/gemini-pro-vision": {
+        "input_cost_per_image": 0.0025,
+        "input_cost_per_token": 1.25e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 45875,
+        "mode": "chat",
+        "output_cost_per_token": 3.75e-07,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/google/palm-2-chat-bison": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "openrouter",
-        "max_tokens": 8000,
+        "max_tokens": 25804,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "openrouter/google/palm-2-codechat-bison": {
         "input_cost_per_token": 5e-07,
         "litellm_provider": "openrouter",
-        "max_tokens": 8000,
+        "max_tokens": 20070,
         "mode": "chat",
         "output_cost_per_token": 5e-07
     },
     "openrouter/gryphe/mythomax-l2-13b": {
         "input_cost_per_token": 1.875e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
@@ -2178,28 +2579,77 @@
     "openrouter/meta-llama/llama-2-70b-chat": {
         "input_cost_per_token": 1.5e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.5e-06
     },
+    "openrouter/meta-llama/llama-3-70b-instruct": {
+        "input_cost_per_token": 5.9e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 7.9e-07
+    },
+    "openrouter/meta-llama/llama-3-70b-instruct:nitro": {
+        "input_cost_per_token": 9e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 9e-07
+    },
+    "openrouter/meta-llama/llama-3-8b-instruct:extended": {
+        "input_cost_per_token": 2.25e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 16384,
+        "mode": "chat",
+        "output_cost_per_token": 2.25e-06
+    },
+    "openrouter/meta-llama/llama-3-8b-instruct:free": {
+        "input_cost_per_token": 0.0,
+        "litellm_provider": "openrouter",
+        "max_tokens": 8192,
+        "mode": "chat",
+        "output_cost_per_token": 0.0
+    },
+    "openrouter/microsoft/wizardlm-2-8x22b:nitro": {
+        "input_cost_per_token": 1e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06
+    },
     "openrouter/mistralai/mistral-7b-instruct": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 1.3e-07
     },
     "openrouter/mistralai/mistral-7b-instruct:free": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
+    "openrouter/mistralai/mistral-large": {
+        "input_cost_per_token": 8e-06,
+        "litellm_provider": "openrouter",
+        "max_tokens": 32000,
+        "mode": "chat",
+        "output_cost_per_token": 2.4e-05
+    },
+    "openrouter/mistralai/mixtral-8x22b-instruct": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "openrouter",
+        "max_tokens": 65536,
+        "mode": "chat",
+        "output_cost_per_token": 6.5e-07
+    },
     "openrouter/nousresearch/nous-hermes-llama2-13b": {
         "input_cost_per_token": 2e-07,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 2e-07
     },
@@ -2220,14 +2670,24 @@
     "openrouter/openai/gpt-4": {
         "input_cost_per_token": 3e-05,
         "litellm_provider": "openrouter",
         "max_tokens": 8192,
         "mode": "chat",
         "output_cost_per_token": 6e-05
     },
+    "openrouter/openai/gpt-4-vision-preview": {
+        "input_cost_per_image": 0.01445,
+        "input_cost_per_token": 1e-05,
+        "litellm_provider": "openrouter",
+        "max_tokens": 130000,
+        "mode": "chat",
+        "output_cost_per_token": 3e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "openrouter/pygmalionai/mythalion-13b": {
         "input_cost_per_token": 1.875e-06,
         "litellm_provider": "openrouter",
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 1.875e-06
     },
@@ -2424,14 +2884,131 @@
         "litellm_provider": "replicate",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "chat",
         "output_cost_per_token": 0.0
     },
+    "replicate/meta/llama-2-13b": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "replicate/meta/llama-2-13b-chat": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 5e-07
+    },
+    "replicate/meta/llama-2-70b": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-2-70b-chat": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-2-7b": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-2-7b-chat": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-3-70b": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-3-70b-instruct": {
+        "input_cost_per_token": 6.5e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.75e-06
+    },
+    "replicate/meta/llama-3-8b": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/meta/llama-3-8b-instruct": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mistral-7b-instruct-v0.2": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mistral-7b-v0.1": {
+        "input_cost_per_token": 5e-08,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 2.5e-07
+    },
+    "replicate/mistralai/mixtral-8x7b-instruct-v0.1": {
+        "input_cost_per_token": 3e-07,
+        "litellm_provider": "replicate",
+        "max_input_tokens": 4096,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1e-06
+    },
     "sagemaker/meta-textgeneration-llama-2-13b": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "sagemaker",
         "max_input_tokens": 4096,
         "max_output_tokens": 4096,
         "max_tokens": 4096,
         "mode": "completion",
@@ -2522,40 +3099,54 @@
     },
     "text-embedding-3-large": {
         "input_cost_per_token": 1.3e-07,
         "litellm_provider": "openai",
         "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 3072
     },
     "text-embedding-3-small": {
         "input_cost_per_token": 2e-08,
         "litellm_provider": "openai",
         "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1536
     },
     "text-embedding-ada-002": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "openai",
         "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
-        "output_cost_per_token": 0.0
+        "output_cost_per_token": 0.0,
+        "output_vector_size": 1536
     },
     "text-embedding-ada-002-v2": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "openai",
         "max_input_tokens": 8191,
         "max_tokens": 8191,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "text-embedding-preview-0409": {
+        "input_cost_per_token": 6.25e-09,
+        "input_cost_per_token_batch_requests": 5e-09,
+        "litellm_provider": "vertex_ai-embedding-models",
+        "max_input_tokens": 3072,
+        "max_tokens": 3072,
+        "mode": "embedding",
+        "output_cost_per_token": 0,
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/pricing"
+    },
     "text-moderation-007": {
         "input_cost_per_token": 0.0,
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 0,
         "max_tokens": 32768,
         "mode": "moderations",
@@ -2575,14 +3166,24 @@
         "litellm_provider": "openai",
         "max_input_tokens": 32768,
         "max_output_tokens": 0,
         "max_tokens": 32768,
         "mode": "moderations",
         "output_cost_per_token": 0.0
     },
+    "text-multilingual-embedding-preview-0409": {
+        "input_cost_per_token": 6.25e-09,
+        "litellm_provider": "vertex_ai-embedding-models",
+        "max_input_tokens": 3072,
+        "max_tokens": 3072,
+        "mode": "embedding",
+        "output_cost_per_token": 0,
+        "output_vector_size": 768,
+        "source": "https://cloud.google.com/vertex-ai/generative-ai/docs/learn/models#foundation_models"
+    },
     "text-unicorn": {
         "input_cost_per_token": 1e-05,
         "litellm_provider": "vertex_ai-text-models",
         "max_input_tokens": 8192,
         "max_output_tokens": 1024,
         "max_tokens": 1024,
         "mode": "completion",
@@ -2688,30 +3289,103 @@
         "supports_parallel_function_calling": true
     },
     "together_ai/togethercomputer/CodeLlama-34b-Instruct": {
         "litellm_provider": "together_ai",
         "supports_function_calling": true,
         "supports_parallel_function_calling": true
     },
+    "vertex_ai/claude-3-haiku@20240307": {
+        "input_cost_per_token": 2.5e-07,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.25e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "vertex_ai/claude-3-opus@20240229": {
+        "input_cost_per_token": 1.5e-06,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 7.5e-06,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
+    "vertex_ai/claude-3-sonnet@20240229": {
+        "input_cost_per_token": 3e-06,
+        "litellm_provider": "vertex_ai-anthropic_models",
+        "max_input_tokens": 200000,
+        "max_output_tokens": 4096,
+        "max_tokens": 4096,
+        "mode": "chat",
+        "output_cost_per_token": 1.5e-05,
+        "supports_function_calling": true,
+        "supports_vision": true
+    },
     "voyage/voyage-01": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "voyage",
         "max_input_tokens": 4096,
         "max_tokens": 4096,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "voyage/voyage-2": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 4000,
+        "max_tokens": 4000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-code-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-large-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
+    "voyage/voyage-law-2": {
+        "input_cost_per_token": 1.2e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 16000,
+        "max_tokens": 16000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
     "voyage/voyage-lite-01": {
         "input_cost_per_token": 1e-07,
         "litellm_provider": "voyage",
         "max_input_tokens": 4096,
         "max_tokens": 4096,
         "mode": "embedding",
         "output_cost_per_token": 0.0
     },
+    "voyage/voyage-lite-02-instruct": {
+        "input_cost_per_token": 1e-07,
+        "litellm_provider": "voyage",
+        "max_input_tokens": 4000,
+        "max_tokens": 4000,
+        "mode": "embedding",
+        "output_cost_per_token": 0.0
+    },
     "whisper-1": {
         "input_cost_per_second": 0,
         "litellm_provider": "openai",
         "mode": "audio_transcription",
         "output_cost_per_second": 0.0001
     }
 }
```

