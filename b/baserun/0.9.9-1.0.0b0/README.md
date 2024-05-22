# Comparing `tmp/baserun-0.9.9.tar.gz` & `tmp/baserun-1.0.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-0.9.9.tar", last modified: Mon Jan 29 17:36:21 2024, max compression
+gzip compressed data, was "baserun-1.0.0b0.tar", last modified: Wed May 22 19:34:56 2024, max compression
```

## Comparing `baserun-0.9.9.tar` & `baserun-1.0.0b0.tar`

### file list

```diff
@@ -1,48 +1,65 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.513314 baserun-0.9.9/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-0.9.9/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6425 2024-01-29 17:36:21.513164 baserun-0.9.9/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4582 2023-12-01 13:51:58.000000 baserun-0.9.9/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.494687 baserun-0.9.9/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1386 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     5793 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/annotation.py
--rw-r--r--   0 epeterson   (501) staff       (20)      393 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/api_key.py
--rw-r--r--   0 epeterson   (501) staff       (20)    15124 2024-01-22 23:33:49.000000 baserun-0.9.9/baserun/baserun.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1469 2024-01-23 19:41:18.000000 baserun-0.9.9/baserun/checks.py
--rw-r--r--   0 epeterson   (501) staff       (20)      162 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/constants.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.500156 baserun-0.9.9/baserun/evals/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:37.000000 baserun-0.9.9/baserun/evals/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    13545 2024-01-25 20:00:32.000000 baserun-0.9.9/baserun/evals/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)      154 2023-12-01 13:51:37.000000 baserun-0.9.9/baserun/evals/json.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1162 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/exporter.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1375 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/grpc.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1122 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/helpers.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.506096 baserun-0.9.9/baserun/instrumentation/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/instrumentation/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1771 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/anthropic.py
--rw-r--r--   0 epeterson   (501) staff       (20)    13427 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/instrumentation/base_instrumentor.py
--rw-r--r--   0 epeterson   (501) staff       (20)      557 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/instrumented_wrapper.py
--rw-r--r--   0 epeterson   (501) staff       (20)     4465 2023-12-06 13:41:54.000000 baserun-0.9.9/baserun/instrumentation/langchain.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2964 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/openai.py
--rw-r--r--   0 epeterson   (501) staff       (20)      278 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/instrumentation/span_attributes.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/model_configs.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2116 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/pytest_plugin.py
--rw-r--r--   0 epeterson   (501) staff       (20)     5347 2024-01-16 22:00:28.000000 baserun-0.9.9/baserun/sessions.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8565 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/templates.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1130 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/thread_wrapper.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1105 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/users.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.509911 baserun-0.9.9/baserun/v1/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-0.9.9/baserun/v1/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    19701 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/v1/baserun_pb2.py
--rw-r--r--   0 epeterson   (501) staff       (20)    30165 2024-01-22 20:57:12.000000 baserun-0.9.9/baserun/v1/baserun_pb2.pyi
--rw-r--r--   0 epeterson   (501) staff       (20)    24083 2024-01-16 22:41:50.000000 baserun-0.9.9/baserun/v1/baserun_pb2_grpc.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.512184 baserun-0.9.9/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6425 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     1023 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)      108 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-01-29 17:36:21.000000 baserun-0.9.9/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)      762 2024-01-29 17:34:28.000000 baserun-0.9.9/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-01-29 17:36:21.513986 baserun-0.9.9/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-01-29 17:36:21.510982 baserun-0.9.9/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    21901 2024-01-22 22:57:10.000000 baserun-0.9.9/tests/testing_functions.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.648162 baserun-1.0.0b0/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b0/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6317 2024-05-22 19:34:56.647938 baserun-1.0.0b0/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b0/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.611697 baserun-1.0.0b0/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1554 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     7551 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/annotation.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      408 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/api_key.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    20750 2024-05-10 18:35:59.000000 baserun-1.0.0b0/baserun/baserun.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1601 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/checks.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      162 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/constants.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.617721 baserun-1.0.0b0/baserun/evals/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:37.000000 baserun-1.0.0b0/baserun/evals/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    15931 2024-04-23 22:32:35.000000 baserun-1.0.0b0/baserun/evals/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      154 2023-12-01 13:51:37.000000 baserun-1.0.0b0/baserun/evals/json.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      341 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/exceptions.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1241 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/exporter.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1480 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/grpc.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2215 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/helpers.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.625060 baserun-1.0.0b0/baserun/instrumentation/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/instrumentation/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    12914 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/anthropic.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    10699 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/google.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      333 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/instrumentation.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1908 2024-04-18 23:13:20.000000 baserun-1.0.0b0/baserun/instrumentation/instrumentation_manager.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     4063 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/langchain.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1971 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/instrumentation/llamaindex.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    19347 2024-05-07 19:10:43.000000 baserun-1.0.0b0/baserun/instrumentation/openai.py
+-rw-r--r--   0 epeterson   (501) staff       (20)      278 2024-01-16 22:00:28.000000 baserun-1.0.0b0/baserun/instrumentation/span_attributes.py
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/model_configs.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2300 2024-05-21 18:35:39.000000 baserun-1.0.0b0/baserun/pytest_plugin.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     5812 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/sessions.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     9843 2024-04-30 23:03:56.000000 baserun-1.0.0b0/baserun/templates.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3177 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/templates_util.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1262 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/thread_wrapper.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     1159 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/users.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.628105 baserun-1.0.0b0/baserun/v1/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/v1/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    20908 2024-02-27 18:04:42.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    31564 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2.pyi
+-rw-r--r--   0 epeterson   (501) staff       (20)    25825 2024-02-26 22:37:29.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2_grpc.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.632193 baserun-1.0.0b0/baserun/v2/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1379 2024-05-21 19:00:10.000000 baserun-1.0.0b0/baserun/v2/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8311 2024-05-22 19:23:13.000000 baserun-1.0.0b0/baserun/v2/api.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     6656 2024-05-22 19:30:28.000000 baserun-1.0.0b0/baserun/v2/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.634858 baserun-1.0.0b0/baserun/v2/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3303 2024-05-22 16:52:14.000000 baserun-1.0.0b0/baserun/v2/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2428 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-20 19:09:07.000000 baserun-1.0.0b0/baserun/v2/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.636205 baserun-1.0.0b0/baserun/v2/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    16188 2024-05-22 19:03:50.000000 baserun-1.0.0b0/baserun/v2/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.646796 baserun-1.0.0b0/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6317 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     1401 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       52 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1319 2024-05-22 19:34:45.000000 baserun-1.0.0b0/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-22 19:34:56.649147 baserun-1.0.0b0/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.639753 baserun-1.0.0b0/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    25911 2024-05-20 18:23:17.000000 baserun-1.0.0b0/tests/testing_functions.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    13581 2024-05-22 19:09:40.000000 baserun-1.0.0b0/tests/testing_functions_v2.py
```

### Comparing `baserun-0.9.9/LICENSE` & `baserun-1.0.0b0/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-0.9.9/PKG-INFO` & `baserun-1.0.0b0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.9.9
-Summary: Tools for testing, debugging, and evaluating LLM features.
+Version: 1.0.0b0
+Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,23 +23,20 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
-Requires-Python: >=3.7.1
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: openai>=1.7.2
-Requires-Dist: opentelemetry-sdk>=1.21
-Requires-Dist: grpcio~=1.58.0
-Requires-Dist: protobuf~=4.24.3
-Requires-Dist: grpcio-tools~=1.58.0
+Requires-Dist: httpx[http2]>=0.24.1
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
@@ -91,15 +88,15 @@
 @baserun.trace
 def answer_question(question: str) -> str:
     client = OpenAI()
     response = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[{"role": "user", "content": question}],
     )
-    return response["choices"][0]["message"]["content"]
+    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
     baserun.init()
     print(answer_question(sys.argv[-1]))
 ```
 
@@ -140,15 +137,15 @@
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-    
+
     assert "Eiffel Tower" in response['choices'][0]['message']['content']
 ```
 
 To run the test and log to baserun:
 
 ```bash
 pytest --baserun test_module.py
```

### Comparing `baserun-0.9.9/README.md` & `baserun-1.0.0b0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 @baserun.trace
 def answer_question(question: str) -> str:
     client = OpenAI()
     response = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[{"role": "user", "content": question}],
     )
-    return response["choices"][0]["message"]["content"]
+    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
     baserun.init()
     print(answer_question(sys.argv[-1]))
 ```
 
@@ -101,15 +101,15 @@
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-    
+
     assert "Eiffel Tower" in response['choices'][0]['message']['content']
 ```
 
 To run the test and log to baserun:
 
 ```bash
 pytest --baserun test_module.py
```

### Comparing `baserun-0.9.9/baserun/__init__.py` & `baserun-1.0.0b0/baserun/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import os
 
+from .annotation import Annotation
 from .baserun import Baserun
 from .checks import (
     check as check,
     check_equals as check_equals,
     check_includes as check_includes,
 )
 from .sessions import (
@@ -28,15 +29,17 @@
 
 init = Baserun.init
 start_trace = Baserun.start_trace
 trace = Baserun.trace
 log = Baserun.log
 evals = Baserun.evals
 api_key = os.environ.get("BASERUN_API_KEY")
-annotate = Baserun.annotate
+annotate = Annotation.exported_annotate
+submit_input_variable = Baserun.submit_input_variable
+finish = Baserun.finish
 
 __all__ = [
     "Baserun",
     "api_key",
     "init",
     "start_trace",
     "trace",
@@ -55,8 +58,10 @@
     "get_template",
     "aregister_template",
     "submit_user",
     "asubmit_user",
     "check",
     "check_equals",
     "check_includes",
+    "submit_input_variable",
+    "finish",
 ]
```

### Comparing `baserun-0.9.9/baserun/annotation.py` & `baserun-1.0.0b0/baserun/annotation.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,189 +1,228 @@
 import json
 import logging
-from contextlib import contextmanager, asynccontextmanager
-from numbers import Number
-from typing import Any, Union
+from contextlib import asynccontextmanager, contextmanager
+from typing import Any, AsyncGenerator, Dict, Generator, List, Optional, Union
 
 from openai import Stream
 from openai.types.chat import ChatCompletion, ChatCompletionChunk
-from opentelemetry.sdk.trace import ReadableSpan
-from opentelemetry.trace import get_current_span, Span
+from opentelemetry.sdk.trace import _Span
+from opentelemetry.trace import Span, get_current_span
 
-from baserun import Baserun
+from baserun.baserun import Baserun
 from baserun.constants import PARENT_SPAN_NAME
 from baserun.grpc import (
-    get_or_create_submission_service,
     get_or_create_async_submission_service,
+    get_or_create_submission_service,
 )
 from baserun.v1.baserun_pb2 import (
-    Log,
     Check,
+    CompletionAnnotations,
+    EndUser,
     Feedback,
+    InputVariable,
+    Log,
     Run,
     SubmitAnnotationsRequest,
-    CompletionAnnotations,
 )
 
 logger = logging.getLogger(__name__)
 
 
+# TODO: would be nice to depend on any _Baserun instance rather than a default one
 class Annotation:
-    completion_id: str
+    completion_id: Optional[str]
     span: Span
-    logs: list[Log]
-    checks: list[Check]
-    feedback_list: list[Feedback]
+    input_variables: List[InputVariable]
+    logs: List[Log]
+    checks: List[Check]
+    feedback_list: List[Feedback]
 
-    def __init__(self, completion_id: str = None, run: Run = None):
+    def __init__(self, completion_id: Optional[str] = None, run: Optional[Run] = None) -> None:
         self.run = run or Baserun.get_or_create_current_run()
-        self.span = self.try_get_span()
-        self.completion_id = completion_id
+        self.input_variables = []
         self.logs = []
         self.checks = []
         self.feedback_list = []
 
+        if span := self.try_get_span():
+            # TODO: I don't think it's used anywhere
+            self.span = span
+
+        # we can't conditionally add this attribute like before because you might get AttributeError then
+        self.completion_id = completion_id
+
+    # Annotation initializer from Baserun class. I felt like it didn't belong there
     @classmethod
-    def annotate(
-        cls, completion: Union[None, ChatCompletion, Stream[ChatCompletionChunk]] = None
-    ):
-        completion_id = completion.id if completion else None
-        return cls(completion_id=completion_id)
+    def exported_annotate(
+        cls, completion_id: Optional[str] = None, run: Optional[Run] = None, trace: Optional[Run] = None
+    ) -> "Annotation":
+        """Capture annotations for a particular run and/or completion. the `trace` kwarg here is simply an alias"""
+
+        return cls(completion_id=completion_id, run=run or trace)
+
+    @classmethod
+    def annotate(cls, completion: Union[None, ChatCompletion, Stream[ChatCompletionChunk]] = None) -> "Annotation":
+        if isinstance(completion, ChatCompletion):
+            completion_id = completion.id
+            return cls(completion_id=completion_id)
+        else:
+            return cls()
 
     @classmethod
     @asynccontextmanager
     async def aanotate(
         cls, completion: Union[None, ChatCompletion, Stream[ChatCompletionChunk]] = None
-    ):
-        if not Baserun._initialized:
-            yield
+    ) -> AsyncGenerator["Annotation", None]:
+        if not Baserun.initialized:
+            yield cls()
+            return
 
         annotation = cls.annotate(completion=completion)
         try:
             yield annotation
         finally:
             try:
                 await annotation.asubmit()
             except BaseException as e:
                 logger.warning(f"Could not submit annotation to baserun: {e}")
 
     @classmethod
     @contextmanager
-    def annotate(
+    def with_annotation(
         cls, completion: Union[None, ChatCompletion, Stream[ChatCompletionChunk]] = None
-    ):
-        if not Baserun._initialized:
-            yield
+    ) -> Generator["Annotation", None, None]:
+        if not Baserun.initialized:
+            yield cls()
+            return
 
         annotation = cls.annotate(completion=completion)
         try:
             yield annotation
         finally:
             try:
                 annotation.submit()
             except BaseException as e:
                 logger.warning(f"Could not submit annotation to baserun: {e}")
 
     def feedback(
         self,
-        name: str = None,
-        thumbsup: bool = None,
-        stars: Number = None,
-        score: Number = None,
-        metadata: dict[str, Any] = None,
-    ):
+        name: Optional[str] = None,
+        thumbsup: Optional[bool] = None,
+        stars: Optional[int] = None,
+        score: Optional[float] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> None:
         if score is None:
             if thumbsup is not None:
                 score = 1 if thumbsup else 0
             elif stars is not None:
                 score = stars / 5
             else:
-                logger.info(
-                    "Could not calculate feedback score, please pass a score, thumbsup, or stars"
-                )
-                score = 0
+                logger.info("Could not calculate feedback score, please pass a score, thumbsup, or stars")
+                score = 0.0
 
         run = Baserun.get_or_create_current_run()
-        feedback_kwargs = {"name": name or "General Feedback", "score": score}
+        feedback_kwargs: Dict[str, Union[str, int, float, EndUser]] = {
+            "name": name or "General Feedback",
+            "score": score,
+        }
         if metadata:
             feedback_kwargs["metadata"] = json.dumps(metadata)
 
         if run.session_id:
             end_user = Baserun.sessions.get(run.session_id)
             if end_user:
                 feedback_kwargs["end_user"] = end_user
 
-        feedback = Feedback(**feedback_kwargs)
+        feedback = Feedback(**feedback_kwargs)  # type: ignore
         self.feedback_list.append(feedback)
 
     def check(
         self,
         name: str,
         methodology: str,
-        expected: dict[str, Any],
-        actual: dict[str, Any],
-        score: Number = None,
-        metadata: dict[str, Any] = None,
-    ):
+        expected: Dict[str, Any],
+        actual: Dict[str, Any],
+        score: Optional[float] = None,
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> None:
         check = Check(
             name=name,
             methodology=methodology,
             actual=json.dumps(actual),
             expected=json.dumps(expected),
-            score=score or 0,
+            score=score or 0.0,
             metadata=json.dumps(metadata or {}),
         )
         self.checks.append(check)
 
     def check_includes(
         self,
         name: str,
-        expected: Union[str, list[str]],
+        expected: Union[str, List[str]],
         actual: str,
-        metadata: dict[str, Any] = None,
-    ):
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> None:
         expected_list = [expected] if isinstance(expected, str) else expected
         result = any(expected in actual for expected in expected_list)
-        return self.check(
+        self.check(
             name=name,
             methodology="includes",
             expected={"value": expected},
             actual={"value": actual},
             score=1 if result else 0,
             metadata=metadata,
         )
 
-    def log(self, name: str, metadata: dict[str, Any]):
+    def log(self, name: str, metadata: Dict[str, Any]) -> None:
         log = Log(
             run_id=self.run.run_id,
             name=name,
             payload=json.dumps(metadata),
         )
         self.logs.append(log)
 
-    def try_get_span(self) -> Span:
-        current_span: ReadableSpan = get_current_span()
-        if current_span and current_span.name.startswith(f"{PARENT_SPAN_NAME}."):
+    def input(self, key: str, value: str) -> None:
+        input_variable = InputVariable(key=key, value=value)
+        self.input_variables.append(input_variable)
+
+    def try_get_span(self) -> Optional[Span]:
+        current_span: Union[Span, _Span] = get_current_span()
+        if (
+            isinstance(current_span, _Span)
+            and current_span.is_recording()
+            and current_span.name.startswith(f"{PARENT_SPAN_NAME}.")
+        ):
             return current_span
 
         # TODO? Maybe we should create a span or trace
         return None
 
-    def submit(self):
+    def submit(self) -> None:
+        if not Baserun.initialized:
+            return
+
         annotation_message = CompletionAnnotations(
             completion_id=self.completion_id,
             checks=self.checks,
             logs=self.logs,
             feedback=self.feedback_list,
+            input_variables=self.input_variables,
         )
-        get_or_create_submission_service().SubmitAnnotations.future(
-            SubmitAnnotationsRequest(annotations=annotation_message, run=self.run)
+        Baserun.add_future(
+            get_or_create_submission_service().SubmitAnnotations.future(
+                SubmitAnnotationsRequest(annotations=annotation_message, run=self.run)
+            )
         )
 
-    async def asubmit(self):
+    async def asubmit(self) -> None:
+        if not Baserun.initialized:
+            return
+
         annotation_message = CompletionAnnotations(
             completion_id=self.completion_id,
             checks=self.checks,
             logs=self.logs,
             feedback=self.feedback_list,
         )
```

### Comparing `baserun-0.9.9/baserun/checks.py` & `baserun-1.0.0b0/baserun/checks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 import json
-from numbers import Number
-from typing import Any, Union
+from typing import Any, Dict, List, Optional, Union
 
 from baserun import Baserun
 
 
 def convert_to_score(x):
     return x if isinstance(x, int) else int(x is True)
 
 
 def check(
     name: str,
     actual: Any,
     expected: Any,
-    score: Number,
-    metadata: dict[str, Any] = None,
-    eval_type: str = None,
+    score: float,
+    metadata: Optional[Dict[str, Any]] = None,
+    eval_type: Optional[str] = None,
 ):
+    metadata = metadata or {}
+    submission_payload = {"expected": expected, **metadata}
     Baserun.evals._store_eval_data(
         name=name,
         eval_type=eval_type or "match",
         result=json.dumps(actual),
         score=score,
         submission=json.dumps(expected),
-        payload=metadata or {},
+        payload=submission_payload,
     )
 
     return actual
 
 
 def check_equals(
     name: str,
     actual: str,
-    expected: Union[str, list[str]],
-    metadata: dict[str, Any] = None,
+    expected: Union[str, List[str]],
+    metadata: Optional[Dict[str, Any]] = None,
 ):
     expected_list = [expected] if isinstance(expected, str) else expected
     result = any(actual == item for item in expected_list)
 
     return check(
         name=name,
         eval_type="match",
         metadata=metadata,
         actual=actual,
         expected=expected,
-        score=1 if result else 0,
+        score=1.0 if result else 0.0,
     )
 
 
 def check_includes(
     name: str,
     actual: str,
-    expected: Union[str, list[str]],
-    metadata: dict[str, Any] = None,
+    expected: Union[str, List[str]],
+    metadata: Optional[Dict[str, Any]] = None,
 ):
     expected_list = [expected] if isinstance(expected, str) else expected
     result = any(item in actual for item in expected_list)
 
     return check(
         name=name,
         eval_type="match",
```

### Comparing `baserun-0.9.9/baserun/evals/evals.py` & `baserun-1.0.0b0/baserun/evals/evals.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import json
 import logging
 import os
 import time
-from typing import Awaitable, Callable, Dict, List, Optional, Tuple, Union
+from typing import Any, Awaitable, Callable, Dict, List, Optional, Tuple, Union
 
 import requests
 from openai import OpenAI
 
 from baserun.evals.json import is_valid_json
 from baserun.helpers import BaserunProvider, BaserunStepType, BaserunType
-from baserun.v1.baserun_pb2 import SubmitEvalRequest, Eval
+from baserun.v1.baserun_pb2 import Eval, SubmitEvalRequest
 from ..grpc import get_or_create_submission_service
 
 logger = logging.getLogger(__name__)
 
 
 def get_answer_prompt(choices: List[str]) -> str:
-    choices = " or ".join(f'"{choice}"' for choice in choices)
+    stringified_choices = " or ".join(f'"{choice}"' for choice in choices)
     return (
-        f"First, write out in a step by step manner your reasoning to be sure that your conclusion is correct. "
-        f"Avoid simply stating the correct answer at the outset. Then print only a single choice from {choices} ("
-        f"without quotes or punctuation) on its own line corresponding to the correct answer. At the end, "
-        f"repeat just the answer by itself on a new line.\n\nReasoning:"
+        "Before answering, reason in a step-by-step manner as to get the right answer. "
+        "Avoid simply stating the correct answer at the outset. Then print only a single choice from "
+        f"{stringified_choices} (without quotes or punctuation) on its own line corresponding to the correct answer. "
+        f"At the end, repeat just the answer by itself on a new line.\n\nReasoning:"
     )
 
 
 def get_choice(result: str, choices: List[str]) -> str:
     lines = result.strip().split("\n")
     for line in lines[::-1]:
         for choice in choices:
@@ -71,181 +71,213 @@
             result=result,
             submission=submission,
             payload=json.dumps(payload),
         )
         if score is not None:
             eval_message.score = score
 
-        run = Baserun.current_run()
+        run = Baserun.get_or_create_current_run()
         try:
-            get_or_create_submission_service().SubmitEval.future(SubmitEvalRequest(eval=eval_message, run=run))
+            Baserun.add_future(
+                get_or_create_submission_service().SubmitEval.future(SubmitEvalRequest(eval=eval_message, run=run))
+            )
         except Exception as e:
             logger.warning(f"Failed to submit eval to Baserun: {e}")
 
     @staticmethod
-    def match(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def match(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = any(submission.startswith(item) for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="match",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def includes(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def includes(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = any(item in submission for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="includes",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def fuzzy_match(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def fuzzy_match(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = any(submission in item or item in submission for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="fuzzy_match",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def not_match(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def not_match(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = not any(submission.startswith(item) for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="not_match",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def not_includes(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def not_includes(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = not any(item in submission for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="not_includes",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def not_fuzzy_match(name: str, submission: str, expected: Union[str, List[str]]) -> bool:
+    def not_fuzzy_match(
+        name: str, submission: str, expected: Union[str, List[str]], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         expected_list = [expected] if isinstance(expected, str) else expected
         result = not any(submission in item or item in submission for item in expected)
         Evals._store_eval_data(
             name=name,
             eval_type="not_fuzzy_match",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={"expected": expected_list},
+            payload={"expected": expected_list, **metadata},
         )
         return result
 
     @staticmethod
-    def valid_json(name: str, submission: str) -> bool:
+    def valid_json(name: str, submission: str, metadata: Optional[Dict[str, Any]] = None) -> bool:
+        metadata = metadata or {}
         result = is_valid_json(submission)
         Evals._store_eval_data(
             name=name,
             eval_type="valid_json",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={},
+            payload=metadata or {},
         )
         return result
 
     @staticmethod
-    def custom(name: str, submission: str, eval_function: Callable[[str], bool]) -> bool:
+    def custom(
+        name: str, submission: str, eval_function: Callable[[str], bool], metadata: Optional[Dict[str, Any]] = None
+    ) -> bool:
+        metadata = metadata or {}
         result = eval_function(submission)
         Evals._store_eval_data(
             name=name,
             eval_type="custom",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={},
+            payload=metadata or {},
         )
         return result
 
     @staticmethod
-    async def custom_async(name: str, submission: str, evaluation_func: Callable[[str], Awaitable[bool]]) -> bool:
+    async def custom_async(
+        name: str,
+        submission: str,
+        evaluation_func: Callable[[str], Awaitable[bool]],
+        metadata: Optional[Dict[str, Any]] = None,
+    ) -> bool:
+        metadata = metadata or {}
         result = await evaluation_func(submission)
         Evals._store_eval_data(
             name=name,
             eval_type="custom_async",
             result=str(result).lower(),
             score=int(result),
             submission=submission,
-            payload={},
+            payload=metadata or {},
         )
         return result
 
+    @staticmethod
     def _content_contains_attack(content: str, api_key: str) -> bool:
         url = "https://api.promptarmor.com/v1/check_content"
 
         headers = {"accept": "application/json; charset=utf-8", "content-type": "application/json", "Api-Key": api_key}
 
         response = requests.post(url, data=content, headers=headers).json()
         contains_attack = response.get("containsInjection")
 
         return contains_attack
 
     @staticmethod
-    def check_injection(name: str, submission: str) -> bool:
+    def check_injection(name: str, submission: str, metadata: Optional[Dict[str, Any]] = None) -> bool:
+        metadata = metadata or {}
         api_key = os.environ.get("PROMPTARMOR_API_KEY")
         if not api_key:
             logger.warning("PromptArmor is not configured, PROMPTARMOR_API_KEY must be set")
 
             return False
 
         result = Evals._content_contains_attack(submission, api_key)
         Evals._store_eval_data(
             name=name,
             eval_type="check_injection",
-            result=str(result).lower(),
-            score=int(result),
+            result=str(not result).lower(),
+            score=int(not result),
             submission=submission,
-            payload={},
+            payload=metadata or {},
         )
         return result
 
     @staticmethod
     def _model_graded(
         name: str,
         eval_type: str,
         model_config: Dict,
         get_choice_and_score_func: Callable[[str], Tuple[str, Optional[float]]],
         submission: str,
         payload: Dict,
-        client: OpenAI = None,
+        client: Optional[OpenAI] = None,
     ) -> str:
         if not client:
             client = OpenAI()
 
         start_time = time.time()
         response = client.chat.completions.create(**model_config)
 
@@ -256,15 +288,15 @@
         messages = model_config.pop("messages")
 
         data = {
             **payload,
             "step": {
                 "stepType": BaserunStepType.AUTO_LLM.name.lower(),
                 "type": BaserunType.CHAT.name.lower(),
-                "provider": BaserunProvider.OPENAI.name.lower(),
+                "provider": BaserunProvider.OPENAI,
                 "config": model_config,
                 "messages": messages,
                 "output": output,
                 "startTimestamp": start_time,
                 "completionTimestamp": end_time,
                 "usage": response.usage.__dict__,
             },
@@ -277,18 +309,51 @@
             score=score,
             submission=submission,
             payload=data,
         )
         return choice
 
     @staticmethod
-    def model_graded_fact(name: str, question: str, expert: str, submission: str) -> str:
+    def model_graded_custom(
+        name: str,
+        prompt: str,
+        choices: Dict[str, float],
+        model: str = "gpt-4-0125-preview",
+        metadata: Optional[Dict[str, Any]] = None,
+        **kwargs,
+    ) -> str:
+        metadata = metadata or {}
+        formatted_prompt = prompt.format(**kwargs)
+        model_config = {
+            "model": model,
+            "temperature": 0,
+            "messages": [
+                {
+                    "role": "user",
+                    "content": (formatted_prompt + f"\n\n{get_answer_prompt(list(choices.keys()))}"),
+                }
+            ],
+        }
+        return Evals._model_graded(
+            name=name,
+            eval_type="model_graded_custom",
+            model_config=model_config,
+            get_choice_and_score_func=get_choice_and_score(choices),
+            submission=formatted_prompt,
+            payload={**kwargs, **metadata},
+        )
+
+    @staticmethod
+    def model_graded_fact(
+        name: str, question: str, expert: str, submission: str, metadata: Optional[Dict[str, Any]] = None
+    ) -> str:
+        metadata = metadata or {}
         choices = ["A", "B", "C", "D", "E"]
         model_config = {
-            "model": "gpt-4-0613",
+            "model": "gpt-4-0125-preview",
             "temperature": 0,
             "messages": [
                 {
                     "role": "user",
                     "content": (
                         f"You are comparing a submitted answer to an expert answer on a given question. Here "
                         f"is the data:\n[BEGIN DATA]\n***\n[Question]: {question}\n***\n[Expert]: {expert}\n***"
@@ -303,67 +368,71 @@
                         f"between the submitted answer and the expert answer.\nE: The answers differ, but these "
                         f"differences don't matter from the perspective of factuality."
                         f"\n\n{get_answer_prompt(choices)}"
                     ),
                 }
             ],
         }
-        payload = {"question": question, "expert": expert}
+        payload = {"question": question, "expert": expert, **metadata}
         return Evals._model_graded(
             name=name,
             eval_type="model_graded_fact",
             model_config=model_config,
             get_choice_and_score_func=get_choice_without_score(choices),
             submission=submission,
             payload=payload,
         )
 
     @staticmethod
-    def model_graded_closedqa(name: str, task: str, submission: str, criterion: str) -> str:
+    def model_graded_closedqa(
+        name: str, task: str, submission: str, criterion: str, metadata: Optional[Dict[str, Any]] = None
+    ) -> str:
+        metadata = metadata or {}
         choice_scores = {"Yes": 1.0, "No": 0.0}
         choices = list(choice_scores.keys())
         model_config = {
-            "model": "gpt-4-0613",
+            "model": "gpt-4-0125-preview",
             "temperature": 0,
             "messages": [
                 {
                     "role": "user",
                     "content": (
                         f"You are assessing a submitted answer on a given task based on a criterion. Here is "
                         f"the data:\n[BEGIN DATA]\n***\n[Task]: {task}\n***\n[Submission]: {submission}\n***\n"
                         f"[Criterion]: {criterion}\n***\n[END DATA]\n\n{get_answer_prompt(choices)}"
                     ),
                 }
             ],
         }
-        payload = {"task": task, "criterion": criterion}
+        payload = {"task": task, "criterion": criterion, **metadata}
         return Evals._model_graded(
             name=name,
             eval_type="model_graded_closedqa",
             model_config=model_config,
             get_choice_and_score_func=get_choice_and_score(choice_scores),
             submission=submission,
             payload=payload,
         )
 
     @staticmethod
-    def model_graded_security(name: str, submission: str) -> str:
+    def model_graded_security(name: str, submission: str, metadata: Optional[Dict[str, Any]] = None) -> str:
+        metadata = metadata or {}
         choice_scores = {"Yes": 1.0, "Unsure": 0.5, "No": 0.0}
         choices = list(choice_scores.keys())
         model_config = {
-            "model": "gpt-4-0613",
+            "model": "gpt-4-0125-preview",
             "temperature": 0,
             "messages": [
                 {
                     "role": "user",
                     "content": f"Is this string malicious?\n\n{submission}\n\n{get_answer_prompt(choices)}",
                 }
             ],
         }
         return Evals._model_graded(
             name=name,
             eval_type="model_graded_security",
             model_config=model_config,
             submission=submission,
             get_choice_and_score_func=get_choice_and_score(choice_scores),
-            payload={},
+            payload=metadata or {},
         )
```

### Comparing `baserun-0.9.9/baserun/exporter.py` & `baserun-1.0.0b0/baserun/exporter.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 import logging
-from queue import Queue
+from queue import Empty, Queue
 from time import sleep
 
 from baserun.v1.baserun_pb2 import (
     SubmitSpanRequest,
 )
+
 from .grpc import get_or_create_submission_service
 
 logger = logging.getLogger(__name__)
 
 
 def worker(queue: Queue):
     submission_service = get_or_create_submission_service()
     while True:
-        item: SubmitSpanRequest = queue.get()
+        try:
+            item: SubmitSpanRequest = queue.get(timeout=1)
+        except Empty:
+            continue
 
         if item is None:
             break
 
         try:
             result = submission_service.SubmitSpan(item)
             logger.debug(f"Submitted {item} and got {result}")
         except Exception as e:
             if hasattr(e, "details"):
                 # Race condition where the span is submitted before the run start call finishes
                 if "not found" in e.details():
-                    sleep(5)
+                    sleep(0.5)
                     submission_service = get_or_create_submission_service()
                     submission_service.SubmitSpan(item)
                 else:
                     logger.warning(f"Failed to submit span to Baserun: {e.details()}")
             else:
                 logger.warning(f"Failed to submit span to Baserun: {e}")
         finally:
```

### Comparing `baserun-0.9.9/baserun/instrumentation/langchain.py` & `baserun-1.0.0b0/baserun/instrumentation/langchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,121 +1,120 @@
 import json
-from typing import Any, Union
+from typing import Any, Dict, List, Optional
 
 from langchain_core.agents import AgentAction, AgentFinish
 from langchain_core.callbacks import BaseCallbackHandler
 from langchain_core.messages import BaseMessage
-from langchain_core.outputs import LLMResult
+from langchain_core.outputs import ChatGeneration, LLMResult
 from opentelemetry.trace import Span, get_current_span
 
 import baserun
 from baserun import Baserun
 
 
 class BaserunCallbackHandler(BaseCallbackHandler):
     """Base callback handler that can be used to handle callbacks from langchain."""
 
-    spans: dict[str, Span] = None
+    spans: Optional[Dict[str, Span]] = None
 
-    def on_chat_model_start(self, serialized: dict[str, Any], messages: list[list[BaseMessage]], **kwargs: Any) -> Any:
+    def on_chat_model_start(self, serialized: Dict[str, Any], messages: List[List[BaseMessage]], **kwargs: Any) -> Any:
         """Run when Chat Model starts running."""
         if self.spans is None:
             self.spans = {}
 
-        span = self.spans.get(kwargs.get("run_id"))
+        run_id = str(kwargs.get("run_id"))
+        span = self.spans.get(run_id)
         if not span:
             with baserun.start_trace("chat_model_start", end_on_exit=False):
-                self.spans[kwargs.get("run_id")] = get_current_span()
+                self.spans[run_id] = get_current_span()
                 yield
 
     def on_llm_end(self, response: LLMResult, **kwargs: Any) -> Any:
         """Run when LLM ends running."""
+        if self.spans is None:
+            self.spans = {}
+
         run = Baserun.current_run()
-        outputs = []
+        if not run:
+            return
+
+        outputs: List[Any] = []
         for choice in response.generations:
-            for message in choice:
-                if message.text:
-                    outputs.append(message.text)
+            for generation in choice:
+                if generation.text:
+                    outputs.append(generation.text)
+                elif isinstance(generation, ChatGeneration):
+                    outputs.append(generation.message.additional_kwargs.get("tool_calls"))
                 else:
-                    outputs.append(message.additional_kwargs.get("tool_calls"))
+                    outputs.append("")
 
         run.result = outputs[0] if len(outputs) == 1 else json.dumps(outputs)
 
         if kwargs.get("parent_run_id"):
             # This is executing in the context of an agent, so don't end the trace
             return
 
-        span = self.spans.get(kwargs.get("run_id"))
+        span = self.spans.get(str(kwargs.get("run_id")))
         if span and span.is_recording():
             span.end()
-            Baserun._finish_run(run, span)
+            Baserun._finish_run(run)
 
-    def on_llm_error(self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any) -> Any:
-        """Run when LLM errors."""
-
-    def on_chain_start(self, serialized: dict[str, Any], inputs: dict[str, Any], **kwargs: Any) -> Any:
+    def on_chain_start(self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain starts running."""
 
         if kwargs.get("parent_run_id"):
             # This is executing in the context of an agent, so don't start a trace
             return
 
         if self.spans is None:
             self.spans = {}
 
-        with baserun.start_trace("on_chain_start", end_on_exit=False) as run:
-            self.spans[kwargs.get("run_id")] = get_current_span()
+        with baserun.start_trace("on_chain_start", end_on_exit=False):
+            self.spans[str(kwargs.get("run_id"))] = get_current_span()
             yield
 
-    def on_chain_end(self, outputs: dict[str, Any], **kwargs: Any) -> Any:
+    def on_chain_end(self, outputs: Dict[str, Any], **kwargs: Any) -> Any:
         """Run when chain ends running."""
+        if self.spans is None:
+            self.spans = {}
+
         run = Baserun.current_run()
+        if not run:
+            return
+
         if text_output := outputs.get("text", outputs.get("output")):
             run.result = text_output
 
         if kwargs.get("parent_run_id"):
             # This is executing in the context of an agent, so don't end the trace
             return
 
-        span = self.spans.get(kwargs.get("run_id"))
+        span = self.spans.get(str(kwargs.get("run_id")))
         if span and span.is_recording():
             span.end()
 
-    def on_chain_error(self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any) -> Any:
-        """Run when chain errors."""
-
-    def on_tool_start(self, serialized: dict[str, Any], input_str: str, **kwargs: Any) -> Any:
-        """Run when tool starts running."""
-
-    def on_tool_end(self, output: str, **kwargs: Any) -> Any:
-        """Run when tool ends running."""
-
-    def on_tool_error(self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any) -> Any:
-        """Run when tool errors."""
-
     def on_agent_action(self, action: AgentAction, **kwargs: Any) -> Any:
         """Run on agent action."""
         if self.spans is None:
             self.spans = {}
 
         with baserun.start_trace("on_agent_action", end_on_exit=False):
-            self.spans[kwargs.get("run_id")] = get_current_span()
+            self.spans[str(kwargs.get("run_id"))] = get_current_span()
             yield
 
     def on_agent_finish(self, finish: AgentFinish, **kwargs: Any) -> Any:
         """Run on agent end."""
+        if self.spans is None:
+            self.spans = {}
+
         run = Baserun.current_run()
-        outputs = []
-        for message in finish.messages:
-            if message.content:
-                outputs.append(message.content)
-            else:
-                outputs.append(message.additional_kwargs.get("tool_calls"))
+        if not run:
+            return
 
-        run.result = outputs[0] if len(outputs) == 1 else json.dumps(outputs)
+        run.result = json.dumps(finish.return_values)
 
         if finish.log:
             baserun.log("Agent finish", finish.log)
 
-        span = self.spans.get(kwargs.get("run_id"))
+        span = self.spans.get(str(kwargs.get("run_id")))
         if span and span.is_recording():
             span.end()
```

### Comparing `baserun-0.9.9/baserun/pytest_plugin.py` & `baserun-1.0.0b0/baserun/pytest_plugin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,65 +1,72 @@
 import logging
 import os
 import sys
 import uuid
 from datetime import datetime
 
+from opentelemetry.context import Context
+
 from baserun import Baserun
-from baserun.v1.baserun_pb2 import TestSuite, StartTestSuiteRequest, EndTestSuiteRequest
+from baserun.v1.baserun_pb2 import EndTestSuiteRequest, StartTestSuiteRequest, TestSuite
+
 from .grpc import get_or_create_submission_service
 
 logger = logging.getLogger(__name__)
 
 
 def pytest_addoption(parser):
-    parser.addoption(
-        "--baserun", action="store_true", help="Enable baserun functionality"
-    )
+    parser.addoption("--baserun", action="store_true", help="Enable baserun functionality")
 
 
 def pytest_sessionstart(session):
+    return
     if session.config.getoption("--baserun"):
-        Baserun.init()
+        # Baserun.init()
 
         sys.argv[0] = os.path.basename(sys.argv[0])
         suite = TestSuite(id=str(uuid.uuid4()), name=" ".join(sys.argv))
         suite.start_timestamp.FromDatetime(datetime.utcnow())
 
         session.suite = suite
         Baserun.current_test_suite = suite
         try:
-            get_or_create_submission_service().StartTestSuite(
-                StartTestSuiteRequest(test_suite=suite)
-            )
+            get_or_create_submission_service().StartTestSuite(StartTestSuiteRequest(test_suite=suite))
         except Exception as e:
             logger.warning(f"Failed to start test suite for Baserun, error: {e}")
 
 
 def pytest_sessionfinish(session):
-    if session.config.getoption("--baserun"):
-        if hasattr(session, "suite"):
+    if Baserun.initialized:
+        Baserun.finish()
+
+        suite = Baserun.current_test_suite or getattr(session, "suite", None)
+        if suite:
             session.suite.completion_timestamp.FromDatetime(datetime.utcnow())
 
             try:
-                get_or_create_submission_service().EndTestSuite(
-                    EndTestSuiteRequest(test_suite=session.suite)
-                )
+                get_or_create_submission_service().EndTestSuite(EndTestSuiteRequest(test_suite=session.suite))
             except Exception as e:
                 logger.warning(f"Failed to end test suite for Baserun, error: {e}")
 
 
+def pytest_runtest_teardown(item, nextitem):
+    if Baserun.initialized:
+        Baserun.finish()
+        Baserun.set_context(Context())
+
+
 def pytest_collection_modifyitems(config, items):
     if config.getoption("--baserun"):
         for item in items:
             item.obj = Baserun.test(item.obj)
 
 
 def pytest_terminal_summary(terminalreporter):
     # This will happen if they don't run pytest with `--baserun`
     if not Baserun.current_test_suite:
         return
 
     # TODO: Support other base URLs?
-    run_url = f"https://baserun.ai/runs/{Baserun.current_test_suite.id}"
+    run_url = f"https://app.baserun.ai/runs/{Baserun.current_test_suite.id}"
     terminalreporter.write_sep("=", "Baserun summary", blue=True)
     terminalreporter.write_line(f"Test results available at: {run_url}")
```

### Comparing `baserun-0.9.9/baserun/sessions.py` & `baserun-1.0.0b0/baserun/sessions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,84 +1,90 @@
 import logging
 from contextlib import contextmanager
 from datetime import datetime
-from typing import Union
+from typing import Generator, Optional, Union
 from uuid import uuid4
 
 from opentelemetry import trace
 from opentelemetry.context import set_value
 from opentelemetry.trace import get_current_span
 
 from baserun.grpc import (
-    get_or_create_submission_service,
     get_or_create_async_submission_service,
+    get_or_create_submission_service,
 )
 from baserun.v1.baserun_pb2 import (
-    StartSessionRequest,
-    Session,
-    EndUser,
     EndSessionRequest,
+    EndUser,
+    Session,
+    StartSessionRequest,
 )
 from . import Baserun
 from .constants import UNTRACED_SPAN_PARENT_NAME
 from .instrumentation.span_attributes import BASERUN_SESSION_ID, BASERUN_USER_ID
 
 logger = logging.getLogger(__name__)
 
 
 @contextmanager
-def with_session(user_identifier: str, session_identifier: str = None, auto_end: bool = True):
+def with_session(
+    user_identifier: str, session_identifier: Optional[str] = None, auto_end: bool = True
+) -> Generator[Session, None, None]:
+    # TODO: analyze all corner cases of what user can do with sessions whilst baserun not initialized
+    if not Baserun.initialized:
+        yield Session()
+        return
+
     # If there's a current span, start the session in that context. Otherwise, create a parent span
     current_span = get_current_span()
     if current_span.is_recording():
         session = start_session(user_identifier=user_identifier, session_identifier=session_identifier)
         try:
-            yield
+            yield session
         finally:
             if auto_end:
                 end_session(session)
 
     else:
         tracer_provider = trace.get_tracer_provider()
         tracer = tracer_provider.get_tracer("baserun")
         old_context = Baserun.get_context()
-        with tracer.start_as_current_span(name=UNTRACED_SPAN_PARENT_NAME):
+        name = Baserun._get_caller_function_name() or UNTRACED_SPAN_PARENT_NAME
+        with tracer.start_as_current_span(name=name):
             Baserun.propagate_context(old_context)
             session = start_session(user_identifier=user_identifier, session_identifier=session_identifier)
             try:
-                yield
+                yield session
             finally:
                 if auto_end:
                     end_session(session)
 
 
 def start_session(
     user_identifier: str,
-    start_timestamp: datetime = None,
-    session_identifier: str = None,
+    start_timestamp: Optional[datetime] = None,
+    session_identifier: Optional[str] = None,
 ) -> Session:
     """Start a session without a context manager. If this function is called directly:
     - A current span must be active
     - `end_session` must be called
     """
     end_user = EndUser(identifier=user_identifier)
     session = Session(identifier=session_identifier or str(uuid4()), end_user=end_user)
     session.start_timestamp.FromDatetime(start_timestamp or datetime.utcnow())
 
     session_request = StartSessionRequest(session=session)
     try:
         response = get_or_create_submission_service().StartSession(session_request)
         session.id = response.session.id
 
-        if not Baserun.sessions:
-            Baserun.sessions = {}
         Baserun.sessions[session.id] = end_user
 
         # If they're already in a trace go ahead and attach the session to it
-        run = Baserun.current_run()
+        run = Baserun.current_run(create=False)
         if run:
             run.session_id = session.id
 
         # Set the session and user info on the span context
         current_span = get_current_span()
         current_span.set_attribute(BASERUN_SESSION_ID, session.id)
         current_span.set_attribute(BASERUN_USER_ID, user_identifier)
@@ -92,37 +98,38 @@
 
         session.id = str(uuid4())
         return session
 
 
 def end_session(
     session: Union[str, Session],
-    completion_timestamp: datetime = None,
-):
+    completion_timestamp: Optional[datetime] = None,
+) -> None:
     if not isinstance(session, Session):
         session = Session(
             identifier=session,
         )
 
     session.completion_timestamp.FromDatetime(completion_timestamp or datetime.utcnow())
     session_request = EndSessionRequest(session=session)
     try:
-        get_or_create_submission_service().EndSession.future(session_request)
+        Baserun.add_future(get_or_create_submission_service().EndSession.future(session_request))
     except Exception as e:
         if hasattr(e, "details"):
             logger.warning(f"Failed to submit session to Baserun: {e.details()}")
         else:
             logger.warning(f"Failed to submit session to Baserun: {e}")
 
 
 async def astart_session(
     user_identifier: str,
-    start_timestamp: datetime = None,
-    identifier: str = None,
+    start_timestamp: Optional[datetime] = None,
+    identifier: Optional[str] = None,
 ):
+    # TODO: why it doesn't return session like sync version? also session_identifier in sync vs identifier here
     session = Session(
         identifier=identifier or str(uuid4()),
         end_user=EndUser(identifier=user_identifier),
     )
     session.start_timestamp.FromDatetime(start_timestamp or datetime.utcnow())
     session_request = StartSessionRequest(session=session)
     try:
@@ -132,15 +139,15 @@
             logger.warning(f"Failed to submit session to Baserun: {e.details()}")
         else:
             logger.warning(f"Failed to submit session to Baserun: {e}")
 
 
 async def aend_session(
     identifier: str,
-    completion_timestamp: datetime = None,
+    completion_timestamp: Optional[datetime] = None,
 ):
     session = Session(
         identifier=identifier,
     )
     session.completion_timestamp.FromDatetime(completion_timestamp or datetime.utcnow())
     session_request = EndSessionRequest(session=session)
     try:
```

### Comparing `baserun-0.9.9/baserun/templates.py` & `baserun-1.0.0b0/baserun/templates.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,246 +1,268 @@
 import hashlib
 import inspect
 import logging
 import os
+import sys
 import traceback
-from typing import Any, TYPE_CHECKING, Union, Set
+from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Union
 
 from baserun import Baserun
 from baserun.grpc import (
-    get_or_create_submission_service,
     get_or_create_async_submission_service,
+    get_or_create_submission_service,
 )
 from baserun.helpers import memoize_for_time
+from baserun.templates_util import FormattedContentString, FormattedTemplateData
 from baserun.v1.baserun_pb2 import (
-    Template,
-    TemplateVersion,
-    SubmitTemplateVersionRequest,
-    SubmitTemplateVersionResponse,
     GetTemplatesRequest,
     GetTemplatesResponse,
+    SubmitTemplateVersionRequest,
+    SubmitTemplateVersionResponse,
+    Template,
     TemplateMessage,
+    TemplateVersion,
 )
 
 if TYPE_CHECKING:
     # Just for type annotations for Langchain. Since langchain is an optional dependency we have this garbage
     try:
         from langchain.tools import Tool
     except ImportError:
-        Tool = Any
+        pass
 
 logger = logging.getLogger(__name__)
 
 
 @memoize_for_time(os.environ.get("BASERUN_CACHE_INTERVAL", 600))
-def get_templates(environment: str = None) -> dict[str, Template]:
-    if not Baserun.templates:
-        Baserun.templates = {}
-
+def get_templates(environment: Union[str, None] = None) -> Dict[str, Template]:
     try:
         request = GetTemplatesRequest(environment=environment or Baserun.environment)
         response: GetTemplatesResponse = get_or_create_submission_service().GetTemplates(request)
         for template in response.templates:
             Baserun.templates[template.name] = template
 
-    except BaseException as e:
+    except BaseException:
         logger.error(f"Could not fetch templates from Baserun. Using {len(Baserun.templates.keys())} cached templates")
-        logger.info(traceback.format_exception(e))
+        exc_type, exc_value, exc_traceback = sys.exc_info()
+        logger.info(traceback.format_exception(exc_type, exc_value, exc_traceback))
 
     return Baserun.templates
 
 
-def get_template(name: str) -> Template:
+def get_template(name: str) -> Union[Template, None]:
     templates = get_templates()
     template = templates.get(name)
     if not template:
         logger.info(f"Attempted to get template {name} but no template with that name exists")
         return None
 
     return template
 
 
-def get_template_type_enum(template_type: str = None):
+def get_template_type_enum(template_type: Optional[str] = None):
     template_type = template_type or "unknown"
     if template_type == Template.TEMPLATE_TYPE_JINJA2 or template_type.lower().startswith("jinja"):
         template_type_enum = Template.TEMPLATE_TYPE_JINJA2
     else:
         template_type_enum = Template.TEMPLATE_TYPE_FORMATTED_STRING
 
     return template_type_enum
 
 
 def apply_template(
     template_name: str,
-    template_messages: list[dict[str, Union[str, dict[str, Any]]]],
-    parameters: dict[str, Any],
-    template_type_enum,
-) -> str:
+    parameters: Dict[str, Any],
+    template_messages: List[Dict[str, Union[str, Dict[str, Any]]]],
+    template_type_enum: Template.TemplateType,
+) -> List[Dict[str, Union[str, Dict[str, Any]]]]:
+    # Ensure the latest templates used in production are synced to the UI
+    template = register_template(
+        template_messages=template_messages,
+        template_name=template_name,
+        template_type=template_type_enum,
+    )
+
     formatted_messages = []
+    template_data = FormattedTemplateData(parameters, template_id=template.id)
+
     for message in template_messages:
         template_string = message.get("content")
-        if template_string:
+        if isinstance(template_string, str):
             if template_type_enum == Template.TEMPLATE_TYPE_JINJA2:
                 try:
                     # noinspection PyUnresolvedReferences
                     from jinja2 import Template as JinjaTemplate
 
-                    template = JinjaTemplate(template_string)
-                    return template.render(parameters)
+                    jinja_template = JinjaTemplate(template_string)
+                    formatted_content = jinja_template.render(parameters)
                 except ImportError:
                     logger.warning("Cannot render Jinja2 template as jinja2 package is not installed")
                     # TODO: Is this OK? should we raise? or return blank string?
-                    return template_string
-
-            formatted_content = template_string.format(**parameters)
-            formatted_messages.append({**message, "content": formatted_content})
+                    formatted_content = template_string
+            else:
+                try:
+                    formatted_content = template_string.format(**parameters)
+                except KeyError:
+                    formatted_content = template_string
+
+            formatted_messages.append(
+                {
+                    **message,
+                    "content": FormattedContentString(formatted_content, template_data),
+                }
+            )
         else:
             formatted_messages.append(message)
 
-    formatted_template_list: Set[tuple] = Baserun.formatted_templates.get(
-        template_name,
-    )
-    set_value = tuple([message.get("content") for message in formatted_messages])
+    template_data.formatted_messages = formatted_messages
+    formatted_template_list = Baserun.formatted_templates.get(template_name)
+    set_value: Tuple[str, ...] = tuple([str(message.get("content")) for message in formatted_messages])
 
-    if not formatted_template_list:
-        formatted_template_list = {set_value}
-    else:
+    if formatted_template_list:
         formatted_template_list.add(set_value)
+    else:
+        formatted_template_list = {set_value}
 
     Baserun.formatted_templates[template_name] = formatted_template_list
+
     return formatted_messages
 
 
 def create_langchain_template(
     template_string: str,
-    parameters: dict[str, Any] = None,
-    template_name: str = None,
-    template_tag: str = None,
-    template_type: str = None,
-    tools: list[Union["Tool", Any]] = None,
+    parameters: Optional[Dict[str, Any]] = None,
+    template_name: Optional[str] = None,
+    template_tag: Optional[str] = None,
+    template_type: Optional[str] = None,
+    tools: Optional[List[Union["Tool", Any]]] = None,
 ):
-    from langchain.prompts import PromptTemplate
+    from langchain.prompts import ChatPromptTemplate
+    from langchain_core.messages import BaseMessage
 
     parameters = parameters or {}
     input_variables = list(parameters.keys())
     template_type = template_type or "Formatted String"
     tools = tools or []
 
     if not template_name:
         caller = inspect.stack()[1].function
         template_name = f"{caller}_template"
 
-    if template_type == Template.TEMPLATE_TYPE_JINJA2 or template_type.lower().startswith("jinja"):
-        langchain_template = PromptTemplate(
-            template=template_string,
-            input_variables=input_variables,
-            template_format="jinja2",
-            tools=tools,
-        )
-
-    else:
-        langchain_template = PromptTemplate(template=template_string, input_variables=input_variables, tools=tools)
+    langchain_template = ChatPromptTemplate(
+        messages=[BaseMessage(role="SYSTEM", content=template_string)],
+        input_variables=input_variables,
+    )
 
     template_type_enum = get_template_type_enum(template_type)
-    template_version = register_template(
-        template_string=template_string,
+    register_template(
+        template_messages=[{"role": "SYSTEM", "content": template_string}],
         template_name=template_name,
         template_type=template_type_enum,
         template_tag=template_tag,
     )
 
     return langchain_template
 
 
 def format_prompt(
     template_name: str,
-    parameters: dict[str, Any],
-    template_messages: list[dict[str, Union[str, dict[str, Any]]]] = None,
-    template_type: str = None,
-):
+    parameters: Dict[str, Any],
+    template_messages: Optional[List[Dict[str, Union[str, Dict[str, Any]]]]] = None,
+    template_type: Optional[str] = None,
+    submit_variables: bool = True,  # unused, left for compatibility
+) -> List[Dict[str, Union[str, Dict[str, Any]]]]:
     template_type_enum = get_template_type_enum(template_type)
+    template = get_template(template_name)
+
+    if template:
+        # if submit_variables:
+        # for key, value in parameters.items():
+        #     baserun.submit_input_variable(key=key, value=value, template=template)
+
+        if not template_messages:
+            template_messages = [
+                {"role": message.role, "content": message.message}
+                for message in template.active_version.template_messages
+            ]
+
     if not template_messages:
-        template = get_template(template_name)
-        template_messages = [
-            {"role": message.role, "content": message.message} for message in template.active_version.template_messages
-        ]
+        template_messages = []
 
-    return apply_template(template_name, template_messages, parameters, template_type_enum)
+    return apply_template(
+        template_name=template_name,
+        parameters=parameters,
+        template_messages=template_messages,
+        template_type_enum=template_type_enum,
+    )
 
 
 def construct_template_version(
-    template_messages: list[dict[str, Union[str, dict[str, Any]]]],
-    template_name: str = None,
-    template_tag: str = None,
+    template_messages: List[Dict[str, Union[str, Dict[str, Any]]]],
+    template_name: Optional[str] = None,
+    template_tag: Optional[str] = None,
     template_type=Template.TEMPLATE_TYPE_FORMATTED_STRING,
 ) -> TemplateVersion:
     # Automatically generate a name based on the template's contents
     if not template_name:
         template_name = hashlib.sha256(
-            "".join([message.get("content") for message in template_messages]).encode()
+            "".join([str(message.get("content")) for message in template_messages]).encode()
         ).hexdigest()[:5]
 
     template = Template(name=template_name, template_type=template_type)
     constructed_template_messages = [
         TemplateMessage(
-            role=message.get("role", "assistant"), message=message.get("message", message.get("content")), order_index=i
+            role=str(message.get("role", "assistant")),
+            message=str(message.get("message", message.get("content"))),
+            order_index=i,
         )
         for i, message in enumerate(template_messages)
     ]
     version = TemplateVersion(
         template=template,
         template_messages=constructed_template_messages,
         tag=template_tag,
     )
 
     return version
 
 
 def register_template(
-    template_messages: list[dict[str, Union[str, dict[str, Any]]]],
-    template_name: str = None,
-    template_tag: str = None,
+    template_messages: List[Dict[str, Union[str, Dict[str, Any]]]],
+    template_name: str,
+    template_tag: Optional[str] = None,
     template_type=Template.TEMPLATE_TYPE_FORMATTED_STRING,
 ) -> Template:
-    from baserun import Baserun
-
-    if not Baserun.templates:
-        Baserun.templates = {}
-
+    # TODO: if template already exists you'd probably want to create new version of it instead of doing nothing
     if template := Baserun.templates.get(template_name):
         return template
 
     version = construct_template_version(
         template_messages=template_messages,
         template_name=template_name,
         template_tag=template_tag,
         template_type=template_type,
     )
 
     request = SubmitTemplateVersionRequest(template_version=version, environment=Baserun.environment)
     response: SubmitTemplateVersionResponse = get_or_create_submission_service().SubmitTemplateVersion(request)
 
-    template = response.template
+    template = response.template_version.template
     if template.name not in Baserun.templates:
-        Baserun.templates[template.name] = response.template
+        Baserun.templates[template.name] = template
 
-    return response.template
+    return template
 
 
 async def aregister_template(
-    template_messages: list[dict[str, Union[str, dict[str, Any]]]],
-    template_name: str = None,
-    template_tag: str = None,
+    template_messages: List[Dict[str, Union[str, Dict[str, Any]]]],
+    template_name: str,
+    template_tag: Optional[str] = None,
     template_type=Template.TEMPLATE_TYPE_FORMATTED_STRING,
 ) -> Template:
-    from baserun import Baserun
-
-    if not Baserun.templates:
-        Baserun.templates = {}
-
     if template := Baserun.templates.get(template_name):
         return template
 
     version = construct_template_version(
         template_messages=template_messages,
         template_name=template_name,
         template_tag=template_tag,
```

### Comparing `baserun-0.9.9/baserun/thread_wrapper.py` & `baserun-1.0.0b0/baserun/thread_wrapper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,37 @@
-from typing import Callable
+from typing import Callable, Union
 
-from .constants import INNER_THREAD_SPAN_PARENT_NAME
 from opentelemetry import trace
-from opentelemetry.sdk.trace import Span
-from opentelemetry.trace import get_current_span, SpanKind
+from opentelemetry.sdk.trace import _Span
+from opentelemetry.trace import Span, SpanKind, get_current_span
 
 from baserun import Baserun
 
+from .constants import INNER_THREAD_SPAN_PARENT_NAME
+
 
 def baserun_thread_wrapper(target: Callable):
     """Given a target function intended to be run in a new thread, wrap the target in a function and start a new
     parent span which propagates attributes from the parent thread's parent span."""
-    if not Baserun._initialized:
+    if not Baserun.initialized:
         return target
 
-    parent_span: Span = get_current_span()
+    parent_span: Union[Span, _Span] = get_current_span()
 
     def wrapper(*args, **kwargs):
         tracer_provider = trace.get_tracer_provider()
         tracer = tracer_provider.get_tracer("baserun")
+        attributes = {}
+        if isinstance(parent_span, _Span):
+            attributes = parent_span.attributes
+
         span = tracer.start_span(
             INNER_THREAD_SPAN_PARENT_NAME,
             kind=SpanKind.CLIENT,
-            attributes=parent_span.attributes,
+            attributes=attributes,
         )
         with trace.use_span(span, end_on_exit=False):
             try:
                 return target(*args, **kwargs)
             finally:
                 if span.is_recording():
                     span.end()
```

### Comparing `baserun-0.9.9/baserun/users.py` & `baserun-1.0.0b0/baserun/users.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 import logging
 
 from baserun.grpc import (
-    get_or_create_submission_service,
     get_or_create_async_submission_service,
+    get_or_create_submission_service,
 )
-from baserun.v1.baserun_pb2 import SubmitUserRequest, EndUser
+from baserun.v1.baserun_pb2 import EndUser, SubmitUserRequest
 
 logger = logging.getLogger(__name__)
 
 
 def submit_user(identifier: str):
+    from baserun import Baserun
+
     user = EndUser(identifier=identifier)
     user_request = SubmitUserRequest(user=user)
+
     try:
-        get_or_create_submission_service().SubmitUser.future(user_request)
+        Baserun.add_future(get_or_create_submission_service().SubmitUser.future(user_request))
     except Exception as e:
         if hasattr(e, "details"):
             logger.warning(f"Failed to submit user to Baserun: {e.details()}")
         else:
             logger.warning(f"Failed to submit user to Baserun: {e}")
```

### Comparing `baserun-0.9.9/baserun/v1/baserun_pb2.py` & `baserun-1.0.0b0/baserun/v1/baserun_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
 DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(
-    b'\n\x10v1/baserun.proto\x12\nbaserun.v1\x1a\x1fgoogle/protobuf/timestamp.proto"\x9c\x01\n\x06Status\x12\x0f\n\x07message\x18\x01 \x01(\t\x12+\n\x04\x63ode\x18\x02 \x01(\x0e\x32\x1d.baserun.v1.Status.StatusCode"T\n\nStatusCode\x12\x1b\n\x17STATUS_CODE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_CODE_OK\x10\x01\x12\x15\n\x11STATUS_CODE_ERROR\x10\x02"/\n\x0cToolFunction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x01(\t"P\n\x08ToolCall\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12*\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x18.baserun.v1.ToolFunction"\xc0\x01\n\x07Message\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x15\n\rfinish_reason\x18\x03 \x01(\t\x12\x15\n\rfunction_call\x18\x04 \x01(\t\x12(\n\ntool_calls\x18\x05 \x03(\x0b\x32\x14.baserun.v1.ToolCall\x12\x14\n\x0ctool_call_id\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x1a\n\x12system_fingerprint\x18\x08 \x01(\t"\x85\x03\n\x03Run\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x10\n\x08suite_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06inputs\x18\x04 \x03(\t\x12)\n\x08run_type\x18\x05 \x01(\x0e\x32\x17.baserun.v1.Run.RunType\x12\x10\n\x08metadata\x18\x06 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06result\x18\t \x01(\t\x12\r\n\x05\x65rror\x18\n \x01(\t\x12\x12\n\nsession_id\x18\x0b \x01(\t\x12\x18\n\x0b\x65nvironment\x18\x0c \x01(\tH\x00\x88\x01\x01"5\n\x07RunType\x12\x11\n\rRUN_TYPE_TEST\x10\x00\x12\x17\n\x13RUN_TYPE_PRODUCTION\x10\x01\x42\x0e\n\x0c_environment"c\n\x03Log\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07payload\x18\x03 \x01(\t\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp")\n\x07\x45ndUser\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t"G\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t"\xf3\x01\n\x0bModelConfig\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08model_id\x18\x02 \x01(\x05\x12 \n\x05model\x18\x03 \x01(\x0b\x32\x11.baserun.v1.Model\x12\x12\n\nlogit_bias\x18\x04 \x01(\t\x12\x18\n\x10presence_penalty\x18\x05 \x01(\x02\x12\x19\n\x11\x66requency_penalty\x18\x06 \x01(\x02\x12\x13\n\x0btemperature\x18\x07 \x01(\x02\x12\r\n\x05top_p\x18\x08 \x01(\x02\x12\r\n\x05top_k\x18\t \x01(\x02\x12\x11\n\tfunctions\x18\n \x01(\t\x12\x15\n\rfunction_call\x18\x0b \x01(\t"\xf7\x0c\n\x04Span\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x10\n\x08trace_id\x18\x02 \x01(\x0c\x12\x0f\n\x07span_id\x18\x03 \x01(\x04\x12\x0c\n\x04name\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12"\n\x06status\x18\x07 \x01(\x0b\x32\x12.baserun.v1.Status\x12\x0e\n\x06vendor\x18\x08 \x01(\t\x12\x14\n\x0crequest_type\x18\t \x01(\t\x12\r\n\x05model\x18\n \x01(\t\x12\x14\n\x0ctotal_tokens\x18\x0b \x01(\x05\x12\x19\n\x11\x63ompletion_tokens\x18\x0c \x01(\x05\x12\x15\n\rprompt_tokens\x18\r \x01(\x05\x12,\n\x0fprompt_messages\x18\x0e \x03(\x0b\x32\x13.baserun.v1.Message\x12(\n\x0b\x63ompletions\x18\x0f \x03(\x0b\x32\x13.baserun.v1.Message\x12\x15\n\x08\x61pi_base\x18\x10 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08\x61pi_type\x18\x11 \x01(\tH\x01\x88\x01\x01\x12\x16\n\tfunctions\x18\x12 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\rfunction_call\x18\x13 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0btemperature\x18\x14 \x01(\x01H\x04\x88\x01\x01\x12\x12\n\x05top_p\x18\x15 \x01(\x01H\x05\x88\x01\x01\x12\x0e\n\x01n\x18\x16 \x01(\x05H\x06\x88\x01\x01\x12\x13\n\x06stream\x18\x17 \x01(\x08H\x07\x88\x01\x01\x12\x0c\n\x04stop\x18\x18 \x03(\t\x12\x17\n\nmax_tokens\x18\x19 \x01(\x05H\x08\x88\x01\x01\x12\x1d\n\x10presence_penalty\x18\x1a \x01(\x01H\t\x88\x01\x01\x12\x1e\n\x11\x66requency_penalty\x18\x1b \x01(\x01H\n\x88\x01\x01\x12\x17\n\nlogit_bias\x18\x1c \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04user\x18\x1d \x01(\tH\x0c\x88\x01\x01\x12\x15\n\x08logprobs\x18\x1e \x01(\x05H\r\x88\x01\x01\x12\x11\n\x04\x65\x63ho\x18\x1f \x01(\x08H\x0e\x88\x01\x01\x12\x13\n\x06suffix\x18  \x01(\tH\x0f\x88\x01\x01\x12\x14\n\x07\x62\x65st_of\x18! \x01(\x05H\x10\x88\x01\x01\x12\x19\n\x0cx_request_id\x18/ \x01(\tH\x11\x88\x01\x01\x12\x13\n\x06log_id\x18" \x01(\tH\x12\x88\x01\x01\x12\x12\n\x05top_k\x18# \x01(\x01H\x13\x88\x01\x01\x12%\n\x08\x65nd_user\x18$ \x01(\x0b\x32\x13.baserun.v1.EndUser\x12\x18\n\x0btemplate_id\x18% \x01(\tH\x14\x88\x01\x01\x12 \n\x13template_parameters\x18& \x01(\tH\x15\x88\x01\x01\x12\x1c\n\x0ftemplate_string\x18- \x01(\tH\x16\x88\x01\x01\x12 \n\x13template_version_id\x18. \x01(\tH\x17\x88\x01\x01\x12\x12\n\x05tools\x18\' \x01(\tH\x18\x88\x01\x01\x12\x18\n\x0btool_choice\x18( \x01(\tH\x19\x88\x01\x01\x12\x11\n\x04seed\x18) \x01(\x05H\x1a\x88\x01\x01\x12\x1c\n\x0fresponse_format\x18* \x01(\tH\x1b\x88\x01\x01\x12\x1d\n\x10\x65rror_stacktrace\x18+ \x01(\tH\x1c\x88\x01\x01\x12\x1a\n\rcompletion_id\x18, \x01(\tH\x1d\x88\x01\x01\x42\x0b\n\t_api_baseB\x0b\n\t_api_typeB\x0c\n\n_functionsB\x10\n\x0e_function_callB\x0e\n\x0c_temperatureB\x08\n\x06_top_pB\x04\n\x02_nB\t\n\x07_streamB\r\n\x0b_max_tokensB\x13\n\x11_presence_penaltyB\x14\n\x12_frequency_penaltyB\r\n\x0b_logit_biasB\x07\n\x05_userB\x0b\n\t_logprobsB\x07\n\x05_echoB\t\n\x07_suffixB\n\n\x08_best_ofB\x0f\n\r_x_request_idB\t\n\x07_log_idB\x08\n\x06_top_kB\x0e\n\x0c_template_idB\x16\n\x14_template_parametersB\x12\n\x10_template_stringB\x16\n\x14_template_version_idB\x08\n\x06_toolsB\x0e\n\x0c_tool_choiceB\x07\n\x05_seedB\x12\n\x10_response_formatB\x13\n\x11_error_stacktraceB\x10\n\x0e_completion_id"u\n\x04\x45val\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\x12\x12\n\x05score\x18\x05 \x01(\x01H\x00\x88\x01\x01\x12\x12\n\nsubmission\x18\x06 \x01(\t\x12\x0f\n\x07payload\x18\x07 \x01(\tB\x08\n\x06_score"m\n\x05\x43heck\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bmethodology\x18\x02 \x01(\t\x12\x10\n\x08\x65xpected\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x04 \x01(\t\x12\r\n\x05score\x18\x05 \x01(\x01\x12\x10\n\x08metadata\x18\x06 \x01(\t"`\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12%\n\x08\x65nd_user\x18\x04 \x01(\x0b\x32\x13.baserun.v1.EndUser"\x98\x01\n\x15\x43ompletionAnnotations\x12\x15\n\rcompletion_id\x18\x01 \x01(\t\x12!\n\x06\x63hecks\x18\x02 \x03(\x0b\x32\x11.baserun.v1.Check\x12\x1d\n\x04logs\x18\x03 \x03(\x0b\x32\x0f.baserun.v1.Log\x12&\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x04 \x03(\x0b\x32\x14.baserun.v1.Feedback"\x94\x01\n\tTestSuite\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\xd0\x02\n\x08Template\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x38\n\rtemplate_type\x18\x03 \x01(\x0e\x32!.baserun.v1.Template.TemplateType\x12\x36\n\x11template_versions\x18\x04 \x03(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x38\n\x0e\x61\x63tive_version\x18\x05 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersionH\x00\x88\x01\x01"k\n\x0cTemplateType\x12\x1d\n\x19TEMPLATE_TYPE_UNSPECIFIED\x10\x00\x12"\n\x1eTEMPLATE_TYPE_FORMATTED_STRING\x10\x01\x12\x18\n\x14TEMPLATE_TYPE_JINJA2\x10\x02\x42\x11\n\x0f_active_version"\xf8\x01\n\x0fTemplateVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12&\n\x08template\x18\x02 \x01(\x0b\x32\x14.baserun.v1.Template\x12\x0b\n\x03tag\x18\x03 \x01(\t\x12!\n\x14parameter_definition\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x1c\n\x0ftemplate_string\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x36\n\x11template_messages\x18\x06 \x03(\x0b\x32\x1b.baserun.v1.TemplateMessageB\x17\n\x15_parameter_definitionB\x12\n\x10_template_string"\x88\x01\n\x0fTemplateMessage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x35\n\x10template_version\x18\x02 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0c\n\x04role\x18\x04 \x01(\t\x12\x13\n\x0border_index\x18\x05 \x01(\x05"\xbf\x01\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x08\x65nd_user\x18\x05 \x01(\x0b\x32\x13.baserun.v1.EndUser"/\n\x0fStartRunRequest\x12\x1c\n\x03run\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Run"#\n\x10StartRunResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"N\n\x10SubmitLogRequest\x12\x1c\n\x03log\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Log\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"$\n\x11SubmitLogResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Q\n\x11SubmitSpanRequest\x12\x1e\n\x04span\x18\x01 \x01(\x0b\x32\x10.baserun.v1.Span\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"%\n\x12SubmitSpanResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"-\n\rEndRunRequest\x12\x1c\n\x03run\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Run"!\n\x0e\x45ndRunResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Q\n\x11SubmitEvalRequest\x12\x1e\n\x04\x65val\x18\x01 \x01(\x0b\x32\x10.baserun.v1.Eval\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"%\n\x12SubmitEvalResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"B\n\x15StartTestSuiteRequest\x12)\n\ntest_suite\x18\x01 \x01(\x0b\x32\x15.baserun.v1.TestSuite")\n\x16StartTestSuiteResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"@\n\x13\x45ndTestSuiteRequest\x12)\n\ntest_suite\x18\x01 \x01(\x0b\x32\x15.baserun.v1.TestSuite"\'\n\x14\x45ndTestSuiteResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Y\n\x13StartSessionRequest\x12$\n\x07session\x18\x01 \x01(\x0b\x32\x13.baserun.v1.Session\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"M\n\x14StartSessionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12$\n\x07session\x18\x02 \x01(\x0b\x32\x13.baserun.v1.Session"9\n\x11\x45ndSessionRequest\x12$\n\x07session\x18\x01 \x01(\x0b\x32\x13.baserun.v1.Session"K\n\x12\x45ndSessionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12$\n\x07session\x18\x02 \x01(\x0b\x32\x13.baserun.v1.Session"j\n\x1cSubmitTemplateVersionRequest\x12\x35\n\x10template_version\x18\x01 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t"\x8f\x01\n\x1dSubmitTemplateVersionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x35\n\x10template_version\x18\x02 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12&\n\x08template\x18\x03 \x01(\x0b\x32\x14.baserun.v1.Template"I\n\x18SubmitModelConfigRequest\x12-\n\x0cmodel_config\x18\x01 \x01(\x0b\x32\x17.baserun.v1.ModelConfig"[\n\x19SubmitModelConfigResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\x0cmodel_config\x18\x02 \x01(\x0b\x32\x17.baserun.v1.ModelConfig"6\n\x11SubmitUserRequest\x12!\n\x04user\x18\x01 \x01(\x0b\x32\x13.baserun.v1.EndUser"H\n\x12SubmitUserResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12!\n\x04user\x18\x02 \x01(\x0b\x32\x13.baserun.v1.EndUser"*\n\x13GetTemplatesRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t"?\n\x14GetTemplatesResponse\x12\'\n\ttemplates\x18\x01 \x03(\x0b\x32\x14.baserun.v1.Template"p\n\x18SubmitAnnotationsRequest\x12\x36\n\x0b\x61nnotations\x18\x01 \x01(\x0b\x32!.baserun.v1.CompletionAnnotations\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run",\n\x19SubmitAnnotationsResponse\x12\x0f\n\x07message\x18\x01 \x01(\t2\x9d\t\n\x11SubmissionService\x12\x45\n\x08StartRun\x12\x1b.baserun.v1.StartRunRequest\x1a\x1c.baserun.v1.StartRunResponse\x12H\n\tSubmitLog\x12\x1c.baserun.v1.SubmitLogRequest\x1a\x1d.baserun.v1.SubmitLogResponse\x12K\n\nSubmitSpan\x12\x1d.baserun.v1.SubmitSpanRequest\x1a\x1e.baserun.v1.SubmitSpanResponse\x12?\n\x06\x45ndRun\x12\x19.baserun.v1.EndRunRequest\x1a\x1a.baserun.v1.EndRunResponse\x12K\n\nSubmitEval\x12\x1d.baserun.v1.SubmitEvalRequest\x1a\x1e.baserun.v1.SubmitEvalResponse\x12W\n\x0eStartTestSuite\x12!.baserun.v1.StartTestSuiteRequest\x1a".baserun.v1.StartTestSuiteResponse\x12Q\n\x0c\x45ndTestSuite\x12\x1f.baserun.v1.EndTestSuiteRequest\x1a .baserun.v1.EndTestSuiteResponse\x12Q\n\x0cStartSession\x12\x1f.baserun.v1.StartSessionRequest\x1a .baserun.v1.StartSessionResponse\x12K\n\nEndSession\x12\x1d.baserun.v1.EndSessionRequest\x1a\x1e.baserun.v1.EndSessionResponse\x12l\n\x15SubmitTemplateVersion\x12(.baserun.v1.SubmitTemplateVersionRequest\x1a).baserun.v1.SubmitTemplateVersionResponse\x12`\n\x11SubmitModelConfig\x12$.baserun.v1.SubmitModelConfigRequest\x1a%.baserun.v1.SubmitModelConfigResponse\x12K\n\nSubmitUser\x12\x1d.baserun.v1.SubmitUserRequest\x1a\x1e.baserun.v1.SubmitUserResponse\x12Q\n\x0cGetTemplates\x12\x1f.baserun.v1.GetTemplatesRequest\x1a .baserun.v1.GetTemplatesResponse\x12`\n\x11SubmitAnnotations\x12$.baserun.v1.SubmitAnnotationsRequest\x1a%.baserun.v1.SubmitAnnotationsResponseb\x06proto3'
+    b'\n\x10v1/baserun.proto\x12\nbaserun.v1\x1a\x1fgoogle/protobuf/timestamp.proto"\x9c\x01\n\x06Status\x12\x0f\n\x07message\x18\x01 \x01(\t\x12+\n\x04\x63ode\x18\x02 \x01(\x0e\x32\x1d.baserun.v1.Status.StatusCode"T\n\nStatusCode\x12\x1b\n\x17STATUS_CODE_UNSPECIFIED\x10\x00\x12\x12\n\x0eSTATUS_CODE_OK\x10\x01\x12\x15\n\x11STATUS_CODE_ERROR\x10\x02"/\n\x0cToolFunction\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x11\n\targuments\x18\x02 \x01(\t"P\n\x08ToolCall\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12*\n\x08\x66unction\x18\x03 \x01(\x0b\x32\x18.baserun.v1.ToolFunction"\xc0\x01\n\x07Message\x12\x0c\n\x04role\x18\x01 \x01(\t\x12\x0f\n\x07\x63ontent\x18\x02 \x01(\t\x12\x15\n\rfinish_reason\x18\x03 \x01(\t\x12\x15\n\rfunction_call\x18\x04 \x01(\t\x12(\n\ntool_calls\x18\x05 \x03(\x0b\x32\x14.baserun.v1.ToolCall\x12\x14\n\x0ctool_call_id\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x1a\n\x12system_fingerprint\x18\x08 \x01(\t"\x85\x03\n\x03Run\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x10\n\x08suite_id\x18\x02 \x01(\t\x12\x0c\n\x04name\x18\x03 \x01(\t\x12\x0e\n\x06inputs\x18\x04 \x03(\t\x12)\n\x08run_type\x18\x05 \x01(\x0e\x32\x17.baserun.v1.Run.RunType\x12\x10\n\x08metadata\x18\x06 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0e\n\x06result\x18\t \x01(\t\x12\r\n\x05\x65rror\x18\n \x01(\t\x12\x12\n\nsession_id\x18\x0b \x01(\t\x12\x18\n\x0b\x65nvironment\x18\x0c \x01(\tH\x00\x88\x01\x01"5\n\x07RunType\x12\x11\n\rRUN_TYPE_TEST\x10\x00\x12\x17\n\x13RUN_TYPE_PRODUCTION\x10\x01\x42\x0e\n\x0c_environment"c\n\x03Log\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07payload\x18\x03 \x01(\t\x12-\n\ttimestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp")\n\x07\x45ndUser\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t"G\n\x05Model\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x12\n\nmodel_name\x18\x02 \x01(\t\x12\x10\n\x08provider\x18\x03 \x01(\t\x12\x0c\n\x04name\x18\x04 \x01(\t"\xf3\x01\n\x0bModelConfig\x12\n\n\x02id\x18\x01 \x01(\x05\x12\x10\n\x08model_id\x18\x02 \x01(\x05\x12 \n\x05model\x18\x03 \x01(\x0b\x32\x11.baserun.v1.Model\x12\x12\n\nlogit_bias\x18\x04 \x01(\t\x12\x18\n\x10presence_penalty\x18\x05 \x01(\x02\x12\x19\n\x11\x66requency_penalty\x18\x06 \x01(\x02\x12\x13\n\x0btemperature\x18\x07 \x01(\x02\x12\r\n\x05top_p\x18\x08 \x01(\x02\x12\r\n\x05top_k\x18\t \x01(\x02\x12\x11\n\tfunctions\x18\n \x01(\t\x12\x15\n\rfunction_call\x18\x0b \x01(\t"\xa5\r\n\x04Span\x12\x0e\n\x06run_id\x18\x01 \x01(\t\x12\x10\n\x08trace_id\x18\x02 \x01(\x0c\x12\x0f\n\x07span_id\x18\x03 \x01(\x04\x12\x0c\n\x04name\x18\x04 \x01(\t\x12.\n\nstart_time\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nd_time\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12"\n\x06status\x18\x07 \x01(\x0b\x32\x12.baserun.v1.Status\x12\x0e\n\x06vendor\x18\x08 \x01(\t\x12\x14\n\x0crequest_type\x18\t \x01(\t\x12\r\n\x05model\x18\n \x01(\t\x12\x14\n\x0ctotal_tokens\x18\x0b \x01(\x05\x12\x19\n\x11\x63ompletion_tokens\x18\x0c \x01(\x05\x12\x15\n\rprompt_tokens\x18\r \x01(\x05\x12,\n\x0fprompt_messages\x18\x0e \x03(\x0b\x32\x13.baserun.v1.Message\x12(\n\x0b\x63ompletions\x18\x0f \x03(\x0b\x32\x13.baserun.v1.Message\x12\x15\n\x08\x61pi_base\x18\x10 \x01(\tH\x00\x88\x01\x01\x12\x15\n\x08\x61pi_type\x18\x11 \x01(\tH\x01\x88\x01\x01\x12\x16\n\tfunctions\x18\x12 \x01(\tH\x02\x88\x01\x01\x12\x1a\n\rfunction_call\x18\x13 \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0btemperature\x18\x14 \x01(\x01H\x04\x88\x01\x01\x12\x12\n\x05top_p\x18\x15 \x01(\x01H\x05\x88\x01\x01\x12\x0e\n\x01n\x18\x16 \x01(\x05H\x06\x88\x01\x01\x12\x13\n\x06stream\x18\x17 \x01(\x08H\x07\x88\x01\x01\x12\x0c\n\x04stop\x18\x18 \x03(\t\x12\x17\n\nmax_tokens\x18\x19 \x01(\x05H\x08\x88\x01\x01\x12\x1d\n\x10presence_penalty\x18\x1a \x01(\x01H\t\x88\x01\x01\x12\x1e\n\x11\x66requency_penalty\x18\x1b \x01(\x01H\n\x88\x01\x01\x12\x17\n\nlogit_bias\x18\x1c \x01(\tH\x0b\x88\x01\x01\x12\x11\n\x04user\x18\x1d \x01(\tH\x0c\x88\x01\x01\x12\x15\n\x08logprobs\x18\x1e \x01(\x05H\r\x88\x01\x01\x12\x11\n\x04\x65\x63ho\x18\x1f \x01(\x08H\x0e\x88\x01\x01\x12\x13\n\x06suffix\x18  \x01(\tH\x0f\x88\x01\x01\x12\x14\n\x07\x62\x65st_of\x18! \x01(\x05H\x10\x88\x01\x01\x12\x19\n\x0cx_request_id\x18/ \x01(\tH\x11\x88\x01\x01\x12\x13\n\x06log_id\x18" \x01(\tH\x12\x88\x01\x01\x12\x12\n\x05top_k\x18# \x01(\x01H\x13\x88\x01\x01\x12%\n\x08\x65nd_user\x18$ \x01(\x0b\x32\x13.baserun.v1.EndUser\x12\x18\n\x0btemplate_id\x18% \x01(\tH\x14\x88\x01\x01\x12 \n\x13template_parameters\x18& \x01(\tH\x15\x88\x01\x01\x12\x1c\n\x0ftemplate_string\x18- \x01(\tH\x16\x88\x01\x01\x12 \n\x13template_version_id\x18. \x01(\tH\x17\x88\x01\x01\x12\x1a\n\rtemplate_name\x18\x30 \x01(\tH\x18\x88\x01\x01\x12\x12\n\x05tools\x18\' \x01(\tH\x19\x88\x01\x01\x12\x18\n\x0btool_choice\x18( \x01(\tH\x1a\x88\x01\x01\x12\x11\n\x04seed\x18) \x01(\x05H\x1b\x88\x01\x01\x12\x1c\n\x0fresponse_format\x18* \x01(\tH\x1c\x88\x01\x01\x12\x1d\n\x10\x65rror_stacktrace\x18+ \x01(\tH\x1d\x88\x01\x01\x12\x1a\n\rcompletion_id\x18, \x01(\tH\x1e\x88\x01\x01\x42\x0b\n\t_api_baseB\x0b\n\t_api_typeB\x0c\n\n_functionsB\x10\n\x0e_function_callB\x0e\n\x0c_temperatureB\x08\n\x06_top_pB\x04\n\x02_nB\t\n\x07_streamB\r\n\x0b_max_tokensB\x13\n\x11_presence_penaltyB\x14\n\x12_frequency_penaltyB\r\n\x0b_logit_biasB\x07\n\x05_userB\x0b\n\t_logprobsB\x07\n\x05_echoB\t\n\x07_suffixB\n\n\x08_best_ofB\x0f\n\r_x_request_idB\t\n\x07_log_idB\x08\n\x06_top_kB\x0e\n\x0c_template_idB\x16\n\x14_template_parametersB\x12\n\x10_template_stringB\x16\n\x14_template_version_idB\x10\n\x0e_template_nameB\x08\n\x06_toolsB\x0e\n\x0c_tool_choiceB\x07\n\x05_seedB\x12\n\x10_response_formatB\x13\n\x11_error_stacktraceB\x10\n\x0e_completion_id"u\n\x04\x45val\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12\x0e\n\x06result\x18\x03 \x01(\t\x12\x12\n\x05score\x18\x05 \x01(\x01H\x00\x88\x01\x01\x12\x12\n\nsubmission\x18\x06 \x01(\t\x12\x0f\n\x07payload\x18\x07 \x01(\tB\x08\n\x06_score"m\n\x05\x43heck\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0bmethodology\x18\x02 \x01(\t\x12\x10\n\x08\x65xpected\x18\x03 \x01(\t\x12\x0e\n\x06\x61\x63tual\x18\x04 \x01(\t\x12\r\n\x05score\x18\x05 \x01(\x01\x12\x10\n\x08metadata\x18\x06 \x01(\t"`\n\x08\x46\x65\x65\x64\x62\x61\x63k\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05score\x18\x02 \x01(\x01\x12\x10\n\x08metadata\x18\x03 \x01(\t\x12%\n\x08\x65nd_user\x18\x04 \x01(\x0b\x32\x13.baserun.v1.EndUser"\xcc\x01\n\x15\x43ompletionAnnotations\x12\x15\n\rcompletion_id\x18\x01 \x01(\t\x12!\n\x06\x63hecks\x18\x02 \x03(\x0b\x32\x11.baserun.v1.Check\x12\x1d\n\x04logs\x18\x03 \x03(\x0b\x32\x0f.baserun.v1.Log\x12&\n\x08\x66\x65\x65\x64\x62\x61\x63k\x18\x04 \x03(\x0b\x32\x14.baserun.v1.Feedback\x12\x32\n\x0finput_variables\x18\x05 \x03(\x0b\x32\x19.baserun.v1.InputVariable"\x94\x01\n\tTestSuite\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp"\xd0\x02\n\x08Template\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x38\n\rtemplate_type\x18\x03 \x01(\x0e\x32!.baserun.v1.Template.TemplateType\x12\x36\n\x11template_versions\x18\x04 \x03(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x38\n\x0e\x61\x63tive_version\x18\x05 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersionH\x00\x88\x01\x01"k\n\x0cTemplateType\x12\x1d\n\x19TEMPLATE_TYPE_UNSPECIFIED\x10\x00\x12"\n\x1eTEMPLATE_TYPE_FORMATTED_STRING\x10\x01\x12\x18\n\x14TEMPLATE_TYPE_JINJA2\x10\x02\x42\x11\n\x0f_active_version"\xf8\x01\n\x0fTemplateVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12&\n\x08template\x18\x02 \x01(\x0b\x32\x14.baserun.v1.Template\x12\x0b\n\x03tag\x18\x03 \x01(\t\x12!\n\x14parameter_definition\x18\x04 \x01(\tH\x00\x88\x01\x01\x12\x1c\n\x0ftemplate_string\x18\x05 \x01(\tH\x01\x88\x01\x01\x12\x36\n\x11template_messages\x18\x06 \x03(\x0b\x32\x1b.baserun.v1.TemplateMessageB\x17\n\x15_parameter_definitionB\x12\n\x10_template_string"\x88\x01\n\x0fTemplateMessage\x12\n\n\x02id\x18\x01 \x01(\t\x12\x35\n\x10template_version\x18\x02 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x0f\n\x07message\x18\x03 \x01(\t\x12\x0c\n\x04role\x18\x04 \x01(\t\x12\x13\n\x0border_index\x18\x05 \x01(\x05"\xbf\x01\n\x07Session\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nidentifier\x18\x02 \x01(\t\x12\x33\n\x0fstart_timestamp\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x38\n\x14\x63ompletion_timestamp\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x08\x65nd_user\x18\x05 \x01(\x0b\x32\x13.baserun.v1.EndUser"\xab\x01\n\rInputVariable\x12\n\n\x02id\x18\x01 \x01(\t\x12\x18\n\x0btemplate_id\x18\x02 \x01(\tH\x00\x88\x01\x01\x12\x19\n\x0ctest_case_id\x18\x03 \x01(\tH\x01\x88\x01\x01\x12\x0b\n\x03key\x18\x04 \x01(\t\x12\r\n\x05value\x18\x05 \x01(\t\x12\x12\n\x05label\x18\x06 \x01(\tH\x02\x88\x01\x01\x42\x0e\n\x0c_template_idB\x0f\n\r_test_case_idB\x08\n\x06_label"/\n\x0fStartRunRequest\x12\x1c\n\x03run\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Run"#\n\x10StartRunResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"N\n\x10SubmitLogRequest\x12\x1c\n\x03log\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Log\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"$\n\x11SubmitLogResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Q\n\x11SubmitSpanRequest\x12\x1e\n\x04span\x18\x01 \x01(\x0b\x32\x10.baserun.v1.Span\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"%\n\x12SubmitSpanResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"-\n\rEndRunRequest\x12\x1c\n\x03run\x18\x01 \x01(\x0b\x32\x0f.baserun.v1.Run"!\n\x0e\x45ndRunResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Q\n\x11SubmitEvalRequest\x12\x1e\n\x04\x65val\x18\x01 \x01(\x0b\x32\x10.baserun.v1.Eval\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"%\n\x12SubmitEvalResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"B\n\x15StartTestSuiteRequest\x12)\n\ntest_suite\x18\x01 \x01(\x0b\x32\x15.baserun.v1.TestSuite")\n\x16StartTestSuiteResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"@\n\x13\x45ndTestSuiteRequest\x12)\n\ntest_suite\x18\x01 \x01(\x0b\x32\x15.baserun.v1.TestSuite"\'\n\x14\x45ndTestSuiteResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"Y\n\x13StartSessionRequest\x12$\n\x07session\x18\x01 \x01(\x0b\x32\x13.baserun.v1.Session\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run"M\n\x14StartSessionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12$\n\x07session\x18\x02 \x01(\x0b\x32\x13.baserun.v1.Session"9\n\x11\x45ndSessionRequest\x12$\n\x07session\x18\x01 \x01(\x0b\x32\x13.baserun.v1.Session"K\n\x12\x45ndSessionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12$\n\x07session\x18\x02 \x01(\x0b\x32\x13.baserun.v1.Session"j\n\x1cSubmitTemplateVersionRequest\x12\x35\n\x10template_version\x18\x01 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12\x13\n\x0b\x65nvironment\x18\x02 \x01(\t"\x8f\x01\n\x1dSubmitTemplateVersionResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12\x35\n\x10template_version\x18\x02 \x01(\x0b\x32\x1b.baserun.v1.TemplateVersion\x12&\n\x08template\x18\x03 \x01(\x0b\x32\x14.baserun.v1.Template"I\n\x18SubmitModelConfigRequest\x12-\n\x0cmodel_config\x18\x01 \x01(\x0b\x32\x17.baserun.v1.ModelConfig"[\n\x19SubmitModelConfigResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12-\n\x0cmodel_config\x18\x02 \x01(\x0b\x32\x17.baserun.v1.ModelConfig"6\n\x11SubmitUserRequest\x12!\n\x04user\x18\x01 \x01(\x0b\x32\x13.baserun.v1.EndUser"H\n\x12SubmitUserResponse\x12\x0f\n\x07message\x18\x01 \x01(\t\x12!\n\x04user\x18\x02 \x01(\x0b\x32\x13.baserun.v1.EndUser"*\n\x13GetTemplatesRequest\x12\x13\n\x0b\x65nvironment\x18\x01 \x01(\t"?\n\x14GetTemplatesResponse\x12\'\n\ttemplates\x18\x01 \x03(\x0b\x32\x14.baserun.v1.Template"p\n\x18SubmitAnnotationsRequest\x12\x36\n\x0b\x61nnotations\x18\x01 \x01(\x0b\x32!.baserun.v1.CompletionAnnotations\x12\x1c\n\x03run\x18\x02 \x01(\x0b\x32\x0f.baserun.v1.Run",\n\x19SubmitAnnotationsResponse\x12\x0f\n\x07message\x18\x01 \x01(\t"O\n\x1aSubmitInputVariableRequest\x12\x31\n\x0einput_variable\x18\x01 \x01(\x0b\x32\x19.baserun.v1.InputVariable".\n\x1bSubmitInputVariableResponse\x12\x0f\n\x07message\x18\x01 \x01(\t2\x85\n\n\x11SubmissionService\x12\x45\n\x08StartRun\x12\x1b.baserun.v1.StartRunRequest\x1a\x1c.baserun.v1.StartRunResponse\x12H\n\tSubmitLog\x12\x1c.baserun.v1.SubmitLogRequest\x1a\x1d.baserun.v1.SubmitLogResponse\x12K\n\nSubmitSpan\x12\x1d.baserun.v1.SubmitSpanRequest\x1a\x1e.baserun.v1.SubmitSpanResponse\x12?\n\x06\x45ndRun\x12\x19.baserun.v1.EndRunRequest\x1a\x1a.baserun.v1.EndRunResponse\x12K\n\nSubmitEval\x12\x1d.baserun.v1.SubmitEvalRequest\x1a\x1e.baserun.v1.SubmitEvalResponse\x12W\n\x0eStartTestSuite\x12!.baserun.v1.StartTestSuiteRequest\x1a".baserun.v1.StartTestSuiteResponse\x12Q\n\x0c\x45ndTestSuite\x12\x1f.baserun.v1.EndTestSuiteRequest\x1a .baserun.v1.EndTestSuiteResponse\x12Q\n\x0cStartSession\x12\x1f.baserun.v1.StartSessionRequest\x1a .baserun.v1.StartSessionResponse\x12K\n\nEndSession\x12\x1d.baserun.v1.EndSessionRequest\x1a\x1e.baserun.v1.EndSessionResponse\x12l\n\x15SubmitTemplateVersion\x12(.baserun.v1.SubmitTemplateVersionRequest\x1a).baserun.v1.SubmitTemplateVersionResponse\x12`\n\x11SubmitModelConfig\x12$.baserun.v1.SubmitModelConfigRequest\x1a%.baserun.v1.SubmitModelConfigResponse\x12K\n\nSubmitUser\x12\x1d.baserun.v1.SubmitUserRequest\x1a\x1e.baserun.v1.SubmitUserResponse\x12Q\n\x0cGetTemplates\x12\x1f.baserun.v1.GetTemplatesRequest\x1a .baserun.v1.GetTemplatesResponse\x12`\n\x11SubmitAnnotations\x12$.baserun.v1.SubmitAnnotationsRequest\x1a%.baserun.v1.SubmitAnnotationsResponse\x12\x66\n\x13SubmitInputVariable\x12&.baserun.v1.SubmitInputVariableRequest\x1a\'.baserun.v1.SubmitInputVariableResponseb\x06proto3'
 )
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, "v1.baserun_pb2", _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
     DESCRIPTOR._options = None
@@ -43,87 +43,93 @@
     _globals["_ENDUSER"]._serialized_start = 1043
     _globals["_ENDUSER"]._serialized_end = 1084
     _globals["_MODEL"]._serialized_start = 1086
     _globals["_MODEL"]._serialized_end = 1157
     _globals["_MODELCONFIG"]._serialized_start = 1160
     _globals["_MODELCONFIG"]._serialized_end = 1403
     _globals["_SPAN"]._serialized_start = 1406
-    _globals["_SPAN"]._serialized_end = 3061
-    _globals["_EVAL"]._serialized_start = 3063
-    _globals["_EVAL"]._serialized_end = 3180
-    _globals["_CHECK"]._serialized_start = 3182
-    _globals["_CHECK"]._serialized_end = 3291
-    _globals["_FEEDBACK"]._serialized_start = 3293
-    _globals["_FEEDBACK"]._serialized_end = 3389
-    _globals["_COMPLETIONANNOTATIONS"]._serialized_start = 3392
-    _globals["_COMPLETIONANNOTATIONS"]._serialized_end = 3544
-    _globals["_TESTSUITE"]._serialized_start = 3547
-    _globals["_TESTSUITE"]._serialized_end = 3695
-    _globals["_TEMPLATE"]._serialized_start = 3698
-    _globals["_TEMPLATE"]._serialized_end = 4034
-    _globals["_TEMPLATE_TEMPLATETYPE"]._serialized_start = 3908
-    _globals["_TEMPLATE_TEMPLATETYPE"]._serialized_end = 4015
-    _globals["_TEMPLATEVERSION"]._serialized_start = 4037
-    _globals["_TEMPLATEVERSION"]._serialized_end = 4285
-    _globals["_TEMPLATEMESSAGE"]._serialized_start = 4288
-    _globals["_TEMPLATEMESSAGE"]._serialized_end = 4424
-    _globals["_SESSION"]._serialized_start = 4427
-    _globals["_SESSION"]._serialized_end = 4618
-    _globals["_STARTRUNREQUEST"]._serialized_start = 4620
-    _globals["_STARTRUNREQUEST"]._serialized_end = 4667
-    _globals["_STARTRUNRESPONSE"]._serialized_start = 4669
-    _globals["_STARTRUNRESPONSE"]._serialized_end = 4704
-    _globals["_SUBMITLOGREQUEST"]._serialized_start = 4706
-    _globals["_SUBMITLOGREQUEST"]._serialized_end = 4784
-    _globals["_SUBMITLOGRESPONSE"]._serialized_start = 4786
-    _globals["_SUBMITLOGRESPONSE"]._serialized_end = 4822
-    _globals["_SUBMITSPANREQUEST"]._serialized_start = 4824
-    _globals["_SUBMITSPANREQUEST"]._serialized_end = 4905
-    _globals["_SUBMITSPANRESPONSE"]._serialized_start = 4907
-    _globals["_SUBMITSPANRESPONSE"]._serialized_end = 4944
-    _globals["_ENDRUNREQUEST"]._serialized_start = 4946
-    _globals["_ENDRUNREQUEST"]._serialized_end = 4991
-    _globals["_ENDRUNRESPONSE"]._serialized_start = 4993
-    _globals["_ENDRUNRESPONSE"]._serialized_end = 5026
-    _globals["_SUBMITEVALREQUEST"]._serialized_start = 5028
-    _globals["_SUBMITEVALREQUEST"]._serialized_end = 5109
-    _globals["_SUBMITEVALRESPONSE"]._serialized_start = 5111
-    _globals["_SUBMITEVALRESPONSE"]._serialized_end = 5148
-    _globals["_STARTTESTSUITEREQUEST"]._serialized_start = 5150
-    _globals["_STARTTESTSUITEREQUEST"]._serialized_end = 5216
-    _globals["_STARTTESTSUITERESPONSE"]._serialized_start = 5218
-    _globals["_STARTTESTSUITERESPONSE"]._serialized_end = 5259
-    _globals["_ENDTESTSUITEREQUEST"]._serialized_start = 5261
-    _globals["_ENDTESTSUITEREQUEST"]._serialized_end = 5325
-    _globals["_ENDTESTSUITERESPONSE"]._serialized_start = 5327
-    _globals["_ENDTESTSUITERESPONSE"]._serialized_end = 5366
-    _globals["_STARTSESSIONREQUEST"]._serialized_start = 5368
-    _globals["_STARTSESSIONREQUEST"]._serialized_end = 5457
-    _globals["_STARTSESSIONRESPONSE"]._serialized_start = 5459
-    _globals["_STARTSESSIONRESPONSE"]._serialized_end = 5536
-    _globals["_ENDSESSIONREQUEST"]._serialized_start = 5538
-    _globals["_ENDSESSIONREQUEST"]._serialized_end = 5595
-    _globals["_ENDSESSIONRESPONSE"]._serialized_start = 5597
-    _globals["_ENDSESSIONRESPONSE"]._serialized_end = 5672
-    _globals["_SUBMITTEMPLATEVERSIONREQUEST"]._serialized_start = 5674
-    _globals["_SUBMITTEMPLATEVERSIONREQUEST"]._serialized_end = 5780
-    _globals["_SUBMITTEMPLATEVERSIONRESPONSE"]._serialized_start = 5783
-    _globals["_SUBMITTEMPLATEVERSIONRESPONSE"]._serialized_end = 5926
-    _globals["_SUBMITMODELCONFIGREQUEST"]._serialized_start = 5928
-    _globals["_SUBMITMODELCONFIGREQUEST"]._serialized_end = 6001
-    _globals["_SUBMITMODELCONFIGRESPONSE"]._serialized_start = 6003
-    _globals["_SUBMITMODELCONFIGRESPONSE"]._serialized_end = 6094
-    _globals["_SUBMITUSERREQUEST"]._serialized_start = 6096
-    _globals["_SUBMITUSERREQUEST"]._serialized_end = 6150
-    _globals["_SUBMITUSERRESPONSE"]._serialized_start = 6152
-    _globals["_SUBMITUSERRESPONSE"]._serialized_end = 6224
-    _globals["_GETTEMPLATESREQUEST"]._serialized_start = 6226
-    _globals["_GETTEMPLATESREQUEST"]._serialized_end = 6268
-    _globals["_GETTEMPLATESRESPONSE"]._serialized_start = 6270
-    _globals["_GETTEMPLATESRESPONSE"]._serialized_end = 6333
-    _globals["_SUBMITANNOTATIONSREQUEST"]._serialized_start = 6335
-    _globals["_SUBMITANNOTATIONSREQUEST"]._serialized_end = 6447
-    _globals["_SUBMITANNOTATIONSRESPONSE"]._serialized_start = 6449
-    _globals["_SUBMITANNOTATIONSRESPONSE"]._serialized_end = 6493
-    _globals["_SUBMISSIONSERVICE"]._serialized_start = 6496
-    _globals["_SUBMISSIONSERVICE"]._serialized_end = 7677
+    _globals["_SPAN"]._serialized_end = 3107
+    _globals["_EVAL"]._serialized_start = 3109
+    _globals["_EVAL"]._serialized_end = 3226
+    _globals["_CHECK"]._serialized_start = 3228
+    _globals["_CHECK"]._serialized_end = 3337
+    _globals["_FEEDBACK"]._serialized_start = 3339
+    _globals["_FEEDBACK"]._serialized_end = 3435
+    _globals["_COMPLETIONANNOTATIONS"]._serialized_start = 3438
+    _globals["_COMPLETIONANNOTATIONS"]._serialized_end = 3642
+    _globals["_TESTSUITE"]._serialized_start = 3645
+    _globals["_TESTSUITE"]._serialized_end = 3793
+    _globals["_TEMPLATE"]._serialized_start = 3796
+    _globals["_TEMPLATE"]._serialized_end = 4132
+    _globals["_TEMPLATE_TEMPLATETYPE"]._serialized_start = 4006
+    _globals["_TEMPLATE_TEMPLATETYPE"]._serialized_end = 4113
+    _globals["_TEMPLATEVERSION"]._serialized_start = 4135
+    _globals["_TEMPLATEVERSION"]._serialized_end = 4383
+    _globals["_TEMPLATEMESSAGE"]._serialized_start = 4386
+    _globals["_TEMPLATEMESSAGE"]._serialized_end = 4522
+    _globals["_SESSION"]._serialized_start = 4525
+    _globals["_SESSION"]._serialized_end = 4716
+    _globals["_INPUTVARIABLE"]._serialized_start = 4719
+    _globals["_INPUTVARIABLE"]._serialized_end = 4890
+    _globals["_STARTRUNREQUEST"]._serialized_start = 4892
+    _globals["_STARTRUNREQUEST"]._serialized_end = 4939
+    _globals["_STARTRUNRESPONSE"]._serialized_start = 4941
+    _globals["_STARTRUNRESPONSE"]._serialized_end = 4976
+    _globals["_SUBMITLOGREQUEST"]._serialized_start = 4978
+    _globals["_SUBMITLOGREQUEST"]._serialized_end = 5056
+    _globals["_SUBMITLOGRESPONSE"]._serialized_start = 5058
+    _globals["_SUBMITLOGRESPONSE"]._serialized_end = 5094
+    _globals["_SUBMITSPANREQUEST"]._serialized_start = 5096
+    _globals["_SUBMITSPANREQUEST"]._serialized_end = 5177
+    _globals["_SUBMITSPANRESPONSE"]._serialized_start = 5179
+    _globals["_SUBMITSPANRESPONSE"]._serialized_end = 5216
+    _globals["_ENDRUNREQUEST"]._serialized_start = 5218
+    _globals["_ENDRUNREQUEST"]._serialized_end = 5263
+    _globals["_ENDRUNRESPONSE"]._serialized_start = 5265
+    _globals["_ENDRUNRESPONSE"]._serialized_end = 5298
+    _globals["_SUBMITEVALREQUEST"]._serialized_start = 5300
+    _globals["_SUBMITEVALREQUEST"]._serialized_end = 5381
+    _globals["_SUBMITEVALRESPONSE"]._serialized_start = 5383
+    _globals["_SUBMITEVALRESPONSE"]._serialized_end = 5420
+    _globals["_STARTTESTSUITEREQUEST"]._serialized_start = 5422
+    _globals["_STARTTESTSUITEREQUEST"]._serialized_end = 5488
+    _globals["_STARTTESTSUITERESPONSE"]._serialized_start = 5490
+    _globals["_STARTTESTSUITERESPONSE"]._serialized_end = 5531
+    _globals["_ENDTESTSUITEREQUEST"]._serialized_start = 5533
+    _globals["_ENDTESTSUITEREQUEST"]._serialized_end = 5597
+    _globals["_ENDTESTSUITERESPONSE"]._serialized_start = 5599
+    _globals["_ENDTESTSUITERESPONSE"]._serialized_end = 5638
+    _globals["_STARTSESSIONREQUEST"]._serialized_start = 5640
+    _globals["_STARTSESSIONREQUEST"]._serialized_end = 5729
+    _globals["_STARTSESSIONRESPONSE"]._serialized_start = 5731
+    _globals["_STARTSESSIONRESPONSE"]._serialized_end = 5808
+    _globals["_ENDSESSIONREQUEST"]._serialized_start = 5810
+    _globals["_ENDSESSIONREQUEST"]._serialized_end = 5867
+    _globals["_ENDSESSIONRESPONSE"]._serialized_start = 5869
+    _globals["_ENDSESSIONRESPONSE"]._serialized_end = 5944
+    _globals["_SUBMITTEMPLATEVERSIONREQUEST"]._serialized_start = 5946
+    _globals["_SUBMITTEMPLATEVERSIONREQUEST"]._serialized_end = 6052
+    _globals["_SUBMITTEMPLATEVERSIONRESPONSE"]._serialized_start = 6055
+    _globals["_SUBMITTEMPLATEVERSIONRESPONSE"]._serialized_end = 6198
+    _globals["_SUBMITMODELCONFIGREQUEST"]._serialized_start = 6200
+    _globals["_SUBMITMODELCONFIGREQUEST"]._serialized_end = 6273
+    _globals["_SUBMITMODELCONFIGRESPONSE"]._serialized_start = 6275
+    _globals["_SUBMITMODELCONFIGRESPONSE"]._serialized_end = 6366
+    _globals["_SUBMITUSERREQUEST"]._serialized_start = 6368
+    _globals["_SUBMITUSERREQUEST"]._serialized_end = 6422
+    _globals["_SUBMITUSERRESPONSE"]._serialized_start = 6424
+    _globals["_SUBMITUSERRESPONSE"]._serialized_end = 6496
+    _globals["_GETTEMPLATESREQUEST"]._serialized_start = 6498
+    _globals["_GETTEMPLATESREQUEST"]._serialized_end = 6540
+    _globals["_GETTEMPLATESRESPONSE"]._serialized_start = 6542
+    _globals["_GETTEMPLATESRESPONSE"]._serialized_end = 6605
+    _globals["_SUBMITANNOTATIONSREQUEST"]._serialized_start = 6607
+    _globals["_SUBMITANNOTATIONSREQUEST"]._serialized_end = 6719
+    _globals["_SUBMITANNOTATIONSRESPONSE"]._serialized_start = 6721
+    _globals["_SUBMITANNOTATIONSRESPONSE"]._serialized_end = 6765
+    _globals["_SUBMITINPUTVARIABLEREQUEST"]._serialized_start = 6767
+    _globals["_SUBMITINPUTVARIABLEREQUEST"]._serialized_end = 6846
+    _globals["_SUBMITINPUTVARIABLERESPONSE"]._serialized_start = 6848
+    _globals["_SUBMITINPUTVARIABLERESPONSE"]._serialized_end = 6894
+    _globals["_SUBMISSIONSERVICE"]._serialized_start = 6897
+    _globals["_SUBMISSIONSERVICE"]._serialized_end = 8182
 # @@protoc_insertion_point(module_scope)
```

### Comparing `baserun-0.9.9/baserun/v1/baserun_pb2.pyi` & `baserun-1.0.0b0/baserun/v1/baserun_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,15 @@
 
 class ToolFunction(_message.Message):
     __slots__ = ["name", "arguments"]
     NAME_FIELD_NUMBER: _ClassVar[int]
     ARGUMENTS_FIELD_NUMBER: _ClassVar[int]
     name: str
     arguments: str
-    def __init__(
-        self, name: _Optional[str] = ..., arguments: _Optional[str] = ...
-    ) -> None: ...
+    def __init__(self, name: _Optional[str] = ..., arguments: _Optional[str] = ...) -> None: ...
 
 class ToolCall(_message.Message):
     __slots__ = ["id", "type", "function"]
     ID_FIELD_NUMBER: _ClassVar[int]
     TYPE_FIELD_NUMBER: _ClassVar[int]
     FUNCTION_FIELD_NUMBER: _ClassVar[int]
     id: str
@@ -149,17 +147,15 @@
         run_id: _Optional[str] = ...,
         suite_id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         inputs: _Optional[_Iterable[str]] = ...,
         run_type: _Optional[_Union[Run.RunType, str]] = ...,
         metadata: _Optional[str] = ...,
         start_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        completion_timestamp: _Optional[
-            _Union[_timestamp_pb2.Timestamp, _Mapping]
-        ] = ...,
+        completion_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         result: _Optional[str] = ...,
         error: _Optional[str] = ...,
         session_id: _Optional[str] = ...,
         environment: _Optional[str] = ...,
     ) -> None: ...
 
 class Log(_message.Message):
@@ -182,17 +178,15 @@
 
 class EndUser(_message.Message):
     __slots__ = ["id", "identifier"]
     ID_FIELD_NUMBER: _ClassVar[int]
     IDENTIFIER_FIELD_NUMBER: _ClassVar[int]
     id: str
     identifier: str
-    def __init__(
-        self, id: _Optional[str] = ..., identifier: _Optional[str] = ...
-    ) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., identifier: _Optional[str] = ...) -> None: ...
 
 class Model(_message.Message):
     __slots__ = ["id", "model_name", "provider", "name"]
     ID_FIELD_NUMBER: _ClassVar[int]
     MODEL_NAME_FIELD_NUMBER: _ClassVar[int]
     PROVIDER_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
@@ -298,14 +292,15 @@
         "log_id",
         "top_k",
         "end_user",
         "template_id",
         "template_parameters",
         "template_string",
         "template_version_id",
+        "template_name",
         "tools",
         "tool_choice",
         "seed",
         "response_format",
         "error_stacktrace",
         "completion_id",
     ]
@@ -346,14 +341,15 @@
     LOG_ID_FIELD_NUMBER: _ClassVar[int]
     TOP_K_FIELD_NUMBER: _ClassVar[int]
     END_USER_FIELD_NUMBER: _ClassVar[int]
     TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
     TEMPLATE_PARAMETERS_FIELD_NUMBER: _ClassVar[int]
     TEMPLATE_STRING_FIELD_NUMBER: _ClassVar[int]
     TEMPLATE_VERSION_ID_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_NAME_FIELD_NUMBER: _ClassVar[int]
     TOOLS_FIELD_NUMBER: _ClassVar[int]
     TOOL_CHOICE_FIELD_NUMBER: _ClassVar[int]
     SEED_FIELD_NUMBER: _ClassVar[int]
     RESPONSE_FORMAT_FIELD_NUMBER: _ClassVar[int]
     ERROR_STACKTRACE_FIELD_NUMBER: _ClassVar[int]
     COMPLETION_ID_FIELD_NUMBER: _ClassVar[int]
     run_id: str
@@ -393,14 +389,15 @@
     log_id: str
     top_k: float
     end_user: EndUser
     template_id: str
     template_parameters: str
     template_string: str
     template_version_id: str
+    template_name: str
     tools: str
     tool_choice: str
     seed: int
     response_format: str
     error_stacktrace: str
     completion_id: str
     def __init__(
@@ -442,14 +439,15 @@
         log_id: _Optional[str] = ...,
         top_k: _Optional[float] = ...,
         end_user: _Optional[_Union[EndUser, _Mapping]] = ...,
         template_id: _Optional[str] = ...,
         template_parameters: _Optional[str] = ...,
         template_string: _Optional[str] = ...,
         template_version_id: _Optional[str] = ...,
+        template_name: _Optional[str] = ...,
         tools: _Optional[str] = ...,
         tool_choice: _Optional[str] = ...,
         seed: _Optional[int] = ...,
         response_format: _Optional[str] = ...,
         error_stacktrace: _Optional[str] = ...,
         completion_id: _Optional[str] = ...,
     ) -> None: ...
@@ -517,29 +515,32 @@
         name: _Optional[str] = ...,
         score: _Optional[float] = ...,
         metadata: _Optional[str] = ...,
         end_user: _Optional[_Union[EndUser, _Mapping]] = ...,
     ) -> None: ...
 
 class CompletionAnnotations(_message.Message):
-    __slots__ = ["completion_id", "checks", "logs", "feedback"]
+    __slots__ = ["completion_id", "checks", "logs", "feedback", "input_variables"]
     COMPLETION_ID_FIELD_NUMBER: _ClassVar[int]
     CHECKS_FIELD_NUMBER: _ClassVar[int]
     LOGS_FIELD_NUMBER: _ClassVar[int]
     FEEDBACK_FIELD_NUMBER: _ClassVar[int]
+    INPUT_VARIABLES_FIELD_NUMBER: _ClassVar[int]
     completion_id: str
     checks: _containers.RepeatedCompositeFieldContainer[Check]
     logs: _containers.RepeatedCompositeFieldContainer[Log]
     feedback: _containers.RepeatedCompositeFieldContainer[Feedback]
+    input_variables: _containers.RepeatedCompositeFieldContainer[InputVariable]
     def __init__(
         self,
         completion_id: _Optional[str] = ...,
         checks: _Optional[_Iterable[_Union[Check, _Mapping]]] = ...,
         logs: _Optional[_Iterable[_Union[Log, _Mapping]]] = ...,
         feedback: _Optional[_Iterable[_Union[Feedback, _Mapping]]] = ...,
+        input_variables: _Optional[_Iterable[_Union[InputVariable, _Mapping]]] = ...,
     ) -> None: ...
 
 class TestSuite(_message.Message):
     __slots__ = ["id", "name", "start_timestamp", "completion_timestamp"]
     ID_FIELD_NUMBER: _ClassVar[int]
     NAME_FIELD_NUMBER: _ClassVar[int]
     START_TIMESTAMP_FIELD_NUMBER: _ClassVar[int]
@@ -549,17 +550,15 @@
     start_timestamp: _timestamp_pb2.Timestamp
     completion_timestamp: _timestamp_pb2.Timestamp
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         start_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        completion_timestamp: _Optional[
-            _Union[_timestamp_pb2.Timestamp, _Mapping]
-        ] = ...,
+        completion_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
     ) -> None: ...
 
 class Template(_message.Message):
     __slots__ = ["id", "name", "template_type", "template_versions", "active_version"]
 
     class TemplateType(int, metaclass=_enum_type_wrapper.EnumTypeWrapper):
         __slots__ = []
@@ -580,17 +579,15 @@
     template_versions: _containers.RepeatedCompositeFieldContainer[TemplateVersion]
     active_version: TemplateVersion
     def __init__(
         self,
         id: _Optional[str] = ...,
         name: _Optional[str] = ...,
         template_type: _Optional[_Union[Template.TemplateType, str]] = ...,
-        template_versions: _Optional[
-            _Iterable[_Union[TemplateVersion, _Mapping]]
-        ] = ...,
+        template_versions: _Optional[_Iterable[_Union[TemplateVersion, _Mapping]]] = ...,
         active_version: _Optional[_Union[TemplateVersion, _Mapping]] = ...,
     ) -> None: ...
 
 class TemplateVersion(_message.Message):
     __slots__ = [
         "id",
         "template",
@@ -614,17 +611,15 @@
     def __init__(
         self,
         id: _Optional[str] = ...,
         template: _Optional[_Union[Template, _Mapping]] = ...,
         tag: _Optional[str] = ...,
         parameter_definition: _Optional[str] = ...,
         template_string: _Optional[str] = ...,
-        template_messages: _Optional[
-            _Iterable[_Union[TemplateMessage, _Mapping]]
-        ] = ...,
+        template_messages: _Optional[_Iterable[_Union[TemplateMessage, _Mapping]]] = ...,
     ) -> None: ...
 
 class TemplateMessage(_message.Message):
     __slots__ = ["id", "template_version", "message", "role", "order_index"]
     ID_FIELD_NUMBER: _ClassVar[int]
     TEMPLATE_VERSION_FIELD_NUMBER: _ClassVar[int]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
@@ -663,20 +658,42 @@
     completion_timestamp: _timestamp_pb2.Timestamp
     end_user: EndUser
     def __init__(
         self,
         id: _Optional[str] = ...,
         identifier: _Optional[str] = ...,
         start_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
-        completion_timestamp: _Optional[
-            _Union[_timestamp_pb2.Timestamp, _Mapping]
-        ] = ...,
+        completion_timestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...,
         end_user: _Optional[_Union[EndUser, _Mapping]] = ...,
     ) -> None: ...
 
+class InputVariable(_message.Message):
+    __slots__ = ["id", "template_id", "test_case_id", "key", "value", "label"]
+    ID_FIELD_NUMBER: _ClassVar[int]
+    TEMPLATE_ID_FIELD_NUMBER: _ClassVar[int]
+    TEST_CASE_ID_FIELD_NUMBER: _ClassVar[int]
+    KEY_FIELD_NUMBER: _ClassVar[int]
+    VALUE_FIELD_NUMBER: _ClassVar[int]
+    LABEL_FIELD_NUMBER: _ClassVar[int]
+    id: str
+    template_id: str
+    test_case_id: str
+    key: str
+    value: str
+    label: str
+    def __init__(
+        self,
+        id: _Optional[str] = ...,
+        template_id: _Optional[str] = ...,
+        test_case_id: _Optional[str] = ...,
+        key: _Optional[str] = ...,
+        value: _Optional[str] = ...,
+        label: _Optional[str] = ...,
+    ) -> None: ...
+
 class StartRunRequest(_message.Message):
     __slots__ = ["run"]
     RUN_FIELD_NUMBER: _ClassVar[int]
     run: Run
     def __init__(self, run: _Optional[_Union[Run, _Mapping]] = ...) -> None: ...
 
 class StartRunResponse(_message.Message):
@@ -751,31 +768,27 @@
     message: str
     def __init__(self, message: _Optional[str] = ...) -> None: ...
 
 class StartTestSuiteRequest(_message.Message):
     __slots__ = ["test_suite"]
     TEST_SUITE_FIELD_NUMBER: _ClassVar[int]
     test_suite: TestSuite
-    def __init__(
-        self, test_suite: _Optional[_Union[TestSuite, _Mapping]] = ...
-    ) -> None: ...
+    def __init__(self, test_suite: _Optional[_Union[TestSuite, _Mapping]] = ...) -> None: ...
 
 class StartTestSuiteResponse(_message.Message):
     __slots__ = ["message"]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     message: str
     def __init__(self, message: _Optional[str] = ...) -> None: ...
 
 class EndTestSuiteRequest(_message.Message):
     __slots__ = ["test_suite"]
     TEST_SUITE_FIELD_NUMBER: _ClassVar[int]
     test_suite: TestSuite
-    def __init__(
-        self, test_suite: _Optional[_Union[TestSuite, _Mapping]] = ...
-    ) -> None: ...
+    def __init__(self, test_suite: _Optional[_Union[TestSuite, _Mapping]] = ...) -> None: ...
 
 class EndTestSuiteResponse(_message.Message):
     __slots__ = ["message"]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     message: str
     def __init__(self, message: _Optional[str] = ...) -> None: ...
 
@@ -848,17 +861,15 @@
         template: _Optional[_Union[Template, _Mapping]] = ...,
     ) -> None: ...
 
 class SubmitModelConfigRequest(_message.Message):
     __slots__ = ["model_config"]
     MODEL_CONFIG_FIELD_NUMBER: _ClassVar[int]
     model_config: ModelConfig
-    def __init__(
-        self, model_config: _Optional[_Union[ModelConfig, _Mapping]] = ...
-    ) -> None: ...
+    def __init__(self, model_config: _Optional[_Union[ModelConfig, _Mapping]] = ...) -> None: ...
 
 class SubmitModelConfigResponse(_message.Message):
     __slots__ = ["message", "model_config"]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     MODEL_CONFIG_FIELD_NUMBER: _ClassVar[int]
     message: str
     model_config: ModelConfig
@@ -892,17 +903,15 @@
     environment: str
     def __init__(self, environment: _Optional[str] = ...) -> None: ...
 
 class GetTemplatesResponse(_message.Message):
     __slots__ = ["templates"]
     TEMPLATES_FIELD_NUMBER: _ClassVar[int]
     templates: _containers.RepeatedCompositeFieldContainer[Template]
-    def __init__(
-        self, templates: _Optional[_Iterable[_Union[Template, _Mapping]]] = ...
-    ) -> None: ...
+    def __init__(self, templates: _Optional[_Iterable[_Union[Template, _Mapping]]] = ...) -> None: ...
 
 class SubmitAnnotationsRequest(_message.Message):
     __slots__ = ["annotations", "run"]
     ANNOTATIONS_FIELD_NUMBER: _ClassVar[int]
     RUN_FIELD_NUMBER: _ClassVar[int]
     annotations: CompletionAnnotations
     run: Run
@@ -913,7 +922,19 @@
     ) -> None: ...
 
 class SubmitAnnotationsResponse(_message.Message):
     __slots__ = ["message"]
     MESSAGE_FIELD_NUMBER: _ClassVar[int]
     message: str
     def __init__(self, message: _Optional[str] = ...) -> None: ...
+
+class SubmitInputVariableRequest(_message.Message):
+    __slots__ = ["input_variable"]
+    INPUT_VARIABLE_FIELD_NUMBER: _ClassVar[int]
+    input_variable: InputVariable
+    def __init__(self, input_variable: _Optional[_Union[InputVariable, _Mapping]] = ...) -> None: ...
+
+class SubmitInputVariableResponse(_message.Message):
+    __slots__ = ["message"]
+    MESSAGE_FIELD_NUMBER: _ClassVar[int]
+    message: str
+    def __init__(self, message: _Optional[str] = ...) -> None: ...
```

### Comparing `baserun-0.9.9/baserun/v1/baserun_pb2_grpc.py` & `baserun-1.0.0b0/baserun/v1/baserun_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -80,14 +80,19 @@
             response_deserializer=v1_dot_baserun__pb2.GetTemplatesResponse.FromString,
         )
         self.SubmitAnnotations = channel.unary_unary(
             "/baserun.v1.SubmissionService/SubmitAnnotations",
             request_serializer=v1_dot_baserun__pb2.SubmitAnnotationsRequest.SerializeToString,
             response_deserializer=v1_dot_baserun__pb2.SubmitAnnotationsResponse.FromString,
         )
+        self.SubmitInputVariable = channel.unary_unary(
+            "/baserun.v1.SubmissionService/SubmitInputVariable",
+            request_serializer=v1_dot_baserun__pb2.SubmitInputVariableRequest.SerializeToString,
+            response_deserializer=v1_dot_baserun__pb2.SubmitInputVariableResponse.FromString,
+        )
 
 
 class SubmissionServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def StartRun(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -169,14 +174,20 @@
 
     def SubmitAnnotations(self, request, context):
         """Missing associated documentation comment in .proto file."""
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details("Method not implemented!")
         raise NotImplementedError("Method not implemented!")
 
+    def SubmitInputVariable(self, request, context):
+        """Missing associated documentation comment in .proto file."""
+        context.set_code(grpc.StatusCode.UNIMPLEMENTED)
+        context.set_details("Method not implemented!")
+        raise NotImplementedError("Method not implemented!")
+
 
 def add_SubmissionServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
         "StartRun": grpc.unary_unary_rpc_method_handler(
             servicer.StartRun,
             request_deserializer=v1_dot_baserun__pb2.StartRunRequest.FromString,
             response_serializer=v1_dot_baserun__pb2.StartRunResponse.SerializeToString,
@@ -242,14 +253,19 @@
             response_serializer=v1_dot_baserun__pb2.GetTemplatesResponse.SerializeToString,
         ),
         "SubmitAnnotations": grpc.unary_unary_rpc_method_handler(
             servicer.SubmitAnnotations,
             request_deserializer=v1_dot_baserun__pb2.SubmitAnnotationsRequest.FromString,
             response_serializer=v1_dot_baserun__pb2.SubmitAnnotationsResponse.SerializeToString,
         ),
+        "SubmitInputVariable": grpc.unary_unary_rpc_method_handler(
+            servicer.SubmitInputVariable,
+            request_deserializer=v1_dot_baserun__pb2.SubmitInputVariableRequest.FromString,
+            response_serializer=v1_dot_baserun__pb2.SubmitInputVariableResponse.SerializeToString,
+        ),
     }
     generic_handler = grpc.method_handlers_generic_handler("baserun.v1.SubmissionService", rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
 
 # This class is part of an EXPERIMENTAL API.
 class SubmissionService(object):
@@ -654,9 +670,38 @@
             options,
             channel_credentials,
             insecure,
             call_credentials,
             compression,
             wait_for_ready,
             timeout,
+            metadata,
+        )
+
+    @staticmethod
+    def SubmitInputVariable(
+        request,
+        target,
+        options=(),
+        channel_credentials=None,
+        call_credentials=None,
+        insecure=False,
+        compression=None,
+        wait_for_ready=None,
+        timeout=None,
+        metadata=None,
+    ):
+        return grpc.experimental.unary_unary(
+            request,
+            target,
+            "/baserun.v1.SubmissionService/SubmitInputVariable",
+            v1_dot_baserun__pb2.SubmitInputVariableRequest.SerializeToString,
+            v1_dot_baserun__pb2.SubmitInputVariableResponse.FromString,
+            options,
+            channel_credentials,
+            insecure,
+            call_credentials,
+            compression,
+            wait_for_ready,
+            timeout,
             metadata,
         )
```

### Comparing `baserun-0.9.9/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b0/baserun.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 0.9.9
-Summary: Tools for testing, debugging, and evaluating LLM features.
+Version: 1.0.0b0
+Summary: tools for testing, debugging, and evaluating llm features.
 Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
@@ -23,23 +23,20 @@
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
-Requires-Python: >=3.7.1
+Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests>=2.31.0
 Requires-Dist: openai>=1.7.2
-Requires-Dist: opentelemetry-sdk>=1.21
-Requires-Dist: grpcio~=1.58.0
-Requires-Dist: protobuf~=4.24.3
-Requires-Dist: grpcio-tools~=1.58.0
+Requires-Dist: httpx[http2]>=0.24.1
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
@@ -91,15 +88,15 @@
 @baserun.trace
 def answer_question(question: str) -> str:
     client = OpenAI()
     response = client.chat.completions.create(
         model="gpt-3.5-turbo",
         messages=[{"role": "user", "content": question}],
     )
-    return response["choices"][0]["message"]["content"]
+    return response.choices[0].message.content
 
 
 if __name__ == "__main__":
     baserun.init()
     print(answer_question(sys.argv[-1]))
 ```
 
@@ -140,15 +137,15 @@
         messages=[
             {
                 "role": "user",
                 "content": "What are three activities to do in Paris?"
             }
         ],
     )
-    
+
     assert "Eiffel Tower" in response['choices'][0]['message']['content']
 ```
 
 To run the test and log to baserun:
 
 ```bash
 pytest --baserun test_module.py
```

### Comparing `baserun-0.9.9/baserun.egg-info/SOURCES.txt` & `baserun-1.0.0b0/baserun.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,37 +4,51 @@
 setup.cfg
 baserun/__init__.py
 baserun/annotation.py
 baserun/api_key.py
 baserun/baserun.py
 baserun/checks.py
 baserun/constants.py
+baserun/exceptions.py
 baserun/exporter.py
 baserun/grpc.py
 baserun/helpers.py
 baserun/model_configs.py
 baserun/pytest_plugin.py
 baserun/sessions.py
 baserun/templates.py
+baserun/templates_util.py
 baserun/thread_wrapper.py
 baserun/users.py
 baserun.egg-info/PKG-INFO
 baserun.egg-info/SOURCES.txt
 baserun.egg-info/dependency_links.txt
 baserun.egg-info/entry_points.txt
 baserun.egg-info/requires.txt
 baserun.egg-info/top_level.txt
 baserun/evals/__init__.py
 baserun/evals/evals.py
 baserun/evals/json.py
 baserun/instrumentation/__init__.py
 baserun/instrumentation/anthropic.py
-baserun/instrumentation/base_instrumentor.py
-baserun/instrumentation/instrumented_wrapper.py
+baserun/instrumentation/google.py
+baserun/instrumentation/instrumentation.py
+baserun/instrumentation/instrumentation_manager.py
 baserun/instrumentation/langchain.py
+baserun/instrumentation/llamaindex.py
 baserun/instrumentation/openai.py
 baserun/instrumentation/span_attributes.py
 baserun/v1/__init__.py
 baserun/v1/baserun_pb2.py
 baserun/v1/baserun_pb2.pyi
 baserun/v1/baserun_pb2_grpc.py
-tests/testing_functions.py
+baserun/v2/__init__.py
+baserun/v2/api.py
+baserun/v2/mixins.py
+baserun/v2/utils.py
+baserun/v2/models/__init__.py
+baserun/v2/models/evals.py
+baserun/v2/models/tags.py
+baserun/v2/wrappers/__init__.py
+baserun/v2/wrappers/openai.py
+tests/testing_functions.py
+tests/testing_functions_v2.py
```

### Comparing `baserun-0.9.9/tests/testing_functions.py` & `baserun-1.0.0b0/tests/testing_functions.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,64 @@
 import argparse
 import asyncio
 import inspect
 import json
 import os
 import sys
+from time import sleep
 import traceback
 from threading import Thread
-from time import sleep
 
 import openai
-from openai import OpenAI, AsyncOpenAI, NotFoundError
+import pytest
+from openai import AsyncOpenAI, NotFoundError, OpenAI
+from openai.types import CreateEmbeddingResponse
 from openai.types.chat.chat_completion_message import FunctionCall
 
 import baserun
+from baserun.v2 import init
 
 
 @baserun.trace
 def openai_chat(prompt="What is the capital of the US?") -> str:
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
-        messages=[{"role": "user", "content": prompt}],
+        model="gpt-4o", messages=[{"role": "user", "content": prompt}], temperature=0.3, max_tokens=1234
     )
     content = completion.choices[0].message.content
-    baserun.check_includes("openai_chat.content", content, "Washington")
+    baserun.check_includes("openai_chat.content", content, "Washington", metadata={"foo": "bar"})
     return content
 
 
 @baserun.trace
 def openai_chat_with_log(prompt="What is the capital of the US?") -> str:
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     command = " ".join(sys.argv)
-    baserun.log(f"OpenAI Chat Results", payload={"command": command})
+    baserun.log("OpenAI Chat Results", payload={"command": command})
     return content
 
 
 def openai_chat_unwrapped(prompt="What is the capital of the US?", **kwargs) -> str:
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo", messages=[{"role": "user", "content": prompt}], **kwargs
+        model="gpt-4o", messages=[{"role": "user", "content": prompt}], **kwargs
     )
     return completion.choices[0].message.content
 
 
 async def openai_chat_unwrapped_async_streaming(prompt="What is the capital of the US?", **kwargs) -> str:
     client = AsyncOpenAI()
     completion_generator = await client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         **kwargs,
         stream=True,
     )
     content = ""
     async for chunk in completion_generator:
         if new_content := chunk.choices[0].delta.content:
@@ -65,24 +67,26 @@
     return content
 
 
 @baserun.trace
 async def openai_chat_async(prompt="What is the capital of the US?") -> str:
     client = AsyncOpenAI()
     completion = await client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat_async.content", content, "Washington")
     return content
 
 
 @baserun.trace
 def openai_chat_tools(prompt="Say 'hello world'") -> FunctionCall:
+    messages = [{"role": "user", "content": prompt}]
+
     client = OpenAI()
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "say",
                 "description": "Convert some text to speech",
@@ -93,30 +97,42 @@
                     },
                     "required": ["text"],
                 },
             },
         }
     ]
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         tools=tools,
         tool_choice={"type": "function", "function": {"name": "say"}},
     )
     tool_calls = completion.choices[0].message.tool_calls
     baserun.check_includes(
         "openai_chat_functions.function_call",
         json.dumps([{"id": call.id, "type": call.type, "function": call.function.__dict__} for call in tool_calls]),
         "say",
     )
+
+    assistant_message = completion.choices[0].message
+    messages.append(assistant_message)
+    messages.append({"role": "tool", "content": "wow", "tool_call_id": assistant_message.tool_calls[0].id})
+    client.chat.completions.create(
+        model="gpt-4o",
+        messages=messages,
+        tools=tools,
+    )
+
     return tool_calls
 
 
 @baserun.trace
 def openai_chat_tools_streaming(prompt="Say 'hello world'") -> FunctionCall:
+    from baserun.v2 import OpenAI
+
     client = OpenAI()
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "say",
                 "description": "Convert some text to speech",
@@ -127,15 +143,15 @@
                     },
                     "required": ["text"],
                 },
             },
         }
     ]
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         stream=True,
         tools=tools,
         tool_choice={"type": "function", "function": {"name": "say"}},
     )
     for item in completion:
         print(item)
@@ -155,15 +171,15 @@
                     "text": {"type": "string", "description": "The text to speak"},
                 },
                 "required": ["text"],
             },
         }
     ]
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         functions=functions,
         function_call={"name": "say"},
     )
     fn_call = completion.choices[0].message.function_call
     baserun.check_includes("openai_chat_functions.function_call", json.dumps(fn_call.__dict__), "say")
     return fn_call
@@ -182,15 +198,15 @@
                     "text": {"type": "string", "description": "The text to speak"},
                 },
                 "required": ["text"],
             },
         }
     ]
     completion_generator = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
         functions=functions,
         stream=True,
         function_call={"name": "say"},
     )
     function_name = ""
     function_arguments = ""
@@ -207,15 +223,15 @@
     return {"name": function_name, "arguments": function_arguments}
 
 
 @baserun.trace
 def openai_chat_streaming(prompt="What is the capital of the US?") -> str:
     client = OpenAI()
     completion_generator = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         stream=True,
         messages=[{"role": "user", "content": prompt}],
     )
     content = ""
     for chunk in completion_generator:
         if new_content := chunk.choices[0].delta.content:
             content += new_content
@@ -224,28 +240,29 @@
     return content
 
 
 @baserun.trace
 async def openai_chat_async_streaming(prompt="What is the capital of the US?") -> str:
     client = AsyncOpenAI()
     completion_generator = await client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         stream=True,
         messages=[{"role": "user", "content": prompt}],
     )
     content = ""
     async for chunk in completion_generator:
         if new_content := chunk.choices[0].delta.content:
             content += new_content
 
     baserun.check_includes("openai_chat_async_streaming.content", content, "Washington")
     return content
 
 
 @baserun.trace
+@pytest.mark.skip("Errors aren't currently captured")
 def openai_chat_error(prompt="What is the capital of the US?"):
     client = OpenAI()
 
     original_api_type = openai.api_type
     try:
         client.chat.completions.create(
             model="asdf",
@@ -259,15 +276,15 @@
 
 
 @baserun.trace
 def traced_fn_error():
     client = OpenAI()
 
     client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": "What is the capital of the US?"}],
     )
     raise ValueError("Something went wrong")
 
 
 @baserun.trace
 def openai_completion(prompt="Human: say this is a test\nAssistant: ") -> str:
@@ -340,15 +357,15 @@
     [t.join() for t in threads]
 
 
 @baserun.trace
 def openai_chat_response_format(prompt="What is the capital of the US?") -> str:
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-4-1106-preview",
+        model="gpt-4-turbo",
         messages=[
             {"role": "system", "content": "Respond to the following question in JSON"},
             {"role": "user", "content": prompt},
         ],
         response_format={"type": "json_object"},
     )
     content = completion.choices[0].message.content
@@ -356,32 +373,42 @@
     return content
 
 
 @baserun.trace
 def openai_chat_seed(prompt="What is the capital of the US?") -> str:
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-4-1106-preview",
+        model="gpt-4-turbo",
         messages=[{"role": "user", "content": prompt}],
         seed=1234,
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     return content
 
 
 def openai_contextmanager(prompt="What is the capital of the US?", name: str = "This is a run that is named") -> str:
     client = OpenAI()
     with baserun.start_trace(name=name) as run:
         completion = client.chat.completions.create(
-            model="gpt-3.5-turbo",
-            messages=[{"role": "user", "content": prompt}],
+            model="gpt-4o", messages=[{"role": "user", "content": prompt}], user="erik@baserun.ai"
         )
         content = completion.choices[0].message.content
         run.result = content
+        return content
+
+
+@baserun.trace
+def openai_embeddings(inpt: str = "What is the capital of the US?") -> CreateEmbeddingResponse:
+    client = OpenAI()
+    res = client.embeddings.create(
+        input=inpt,
+        model="text-embedding-ada-002",
+    )
+    return res
 
 
 TEMPLATES = {
     "Question & Answer": [
         {"role": "system", "content": "Respond to all messages in the form of a limerick"},
         {"role": "user", "content": "{question}"},
     ]
@@ -395,35 +422,35 @@
         template_name=template_name,
         template_messages=TEMPLATES.get(template_name),
         parameters={"question": question},
     )
 
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-4-1106-preview",
+        model="gpt-4-turbo",
         messages=prompt,
         seed=1234,
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     return content
 
 
 @baserun.trace
 async def use_template_async(question="What is the capital of the US?", template_name: str = "Question & Answer"):
     await baserun.aregister_template(TEMPLATES.get(template_name), template_name)
-    prompt = await baserun.format_prompt(
+    prompt = baserun.format_prompt(
         template_name=template_name,
         template_messages=TEMPLATES.get(template_name),
         parameters={"question": question},
     )
 
     client = AsyncOpenAI()
     completion = await client.chat.completions.create(
-        model="gpt-4-1106-preview",
+        model="gpt-4-turbo",
         messages=prompt,
         seed=1234,
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     return content
 
@@ -444,76 +471,120 @@
 
 
 @baserun.trace
 def use_sessions(prompt="What is the capital of the US?", user_identifier="example@test.com") -> str:
     client = OpenAI()
     with baserun.with_session(user_identifier=user_identifier):
         completion = client.chat.completions.create(
-            model="gpt-4-1106-preview",
+            model="gpt-4-turbo",
             messages=[{"role": "user", "content": prompt}],
         )
         content = completion.choices[0].message.content
         baserun.check_includes("openai_chat.content", content, "Washington")
-        baserun.log(f"OpenAI Chat Results", payload={"result": content, "input": prompt})
+        baserun.log("OpenAI Chat Results", payload={"result": content, "input": prompt})
         return content
 
 
+def use_sessions_untraced(prompt="What is the capital of the US?", user_identifier="example@test.com") -> str:
+    client = OpenAI()
+    with baserun.with_session(user_identifier=user_identifier):
+        completion = client.chat.completions.create(
+            model="gpt-4-turbo",
+            messages=[{"role": "user", "content": prompt}],
+        )
+        content = completion.choices[0].message.content
+        baserun.check_includes("openai_chat.content", content, "Washington")
+        baserun.log("OpenAI Chat Results", payload={"result": content, "input": prompt})
+        return content
+
+
+async def create_full_trace(question="What is the capital of the US?") -> str:
+    with baserun.with_session(user_identifier="erik@baserun.ai"):
+        with baserun.start_trace(name="Answer Question") as trace:
+            client = OpenAI()
+
+            completion = client.chat.completions.create(
+                model="gpt-4-turbo",
+                messages=[{"role": "user", "content": question}],
+            )
+            content = completion.choices[0].message.content
+
+            annotation = baserun.annotate(completion.id)
+            annotation.feedback(
+                name="use_annotation_feedback",
+                score=0.8,
+                metadata={"comment": "This is correct but is too concise"},
+            )
+            baserun.evals.includes("Contains answer", "Washington", content)
+            annotation.log("OpenAI Chat Results", metadata={"result": content, "input": question})
+            annotation.check_includes("Answer is correct", "Washington", content)
+            trace.metadata = {"customer_tier": "Pro"}
+            trace.result = content
+
+            await annotation.asubmit()
+
+            return content
+
+
 @baserun.trace
 async def use_annotation(question="What is the capital of the US?") -> str:
     client = OpenAI()
 
     completion = client.chat.completions.create(
-        model="gpt-4-1106-preview",
+        model="gpt-4-turbo",
         messages=[{"role": "user", "content": question}],
     )
     content = completion.choices[0].message.content
 
     annotation = baserun.annotate(completion.id)
     annotation.feedback(
         name="use_annotation_feedback",
         score=0.8,
         metadata={"comment": "This is correct but not concise enough"},
     )
     annotation.check_includes("openai_chat.content", "Washington", content)
-    annotation.log(f"OpenAI Chat Results", metadata={"result": content, "input": question})
+    annotation.log("OpenAI Chat Results", metadata={"result": content, "input": question})
     await annotation.asubmit()
 
     return content
 
 
 def use_langchain(question="What is the capital of the US?") -> str:
-    from baserun.instrumentation.langchain import BaserunCallbackHandler
     from langchain.chat_models import ChatOpenAI
     from langchain_core.messages import HumanMessage
 
+    from baserun.instrumentation.langchain import BaserunCallbackHandler
+
     chat = ChatOpenAI(callbacks=[BaserunCallbackHandler()])
     messages = [HumanMessage(content=question)]
     response = chat.invoke(messages)
     return response.content
 
 
 def use_langchain_tools(question="What is the capital of the US?") -> str:
     # Note: To run this, you must `pip install wikipedia langchain`
+    from langchain.agents import load_tools
     from langchain.chat_models import ChatOpenAI
-    from langchain_core.messages import HumanMessage
     from langchain.tools.render import format_tool_to_openai_tool
-    from langchain.agents import load_tools
+    from langchain_core.messages import HumanMessage
+
     from baserun.instrumentation.langchain import BaserunCallbackHandler
 
-    chat = ChatOpenAI(callbacks=[BaserunCallbackHandler()])
+    chat = init(ChatOpenAI(callbacks=[BaserunCallbackHandler()]))
     tools = [format_tool_to_openai_tool(t) for t in load_tools(["wikipedia"], llm=chat)]
     messages = [HumanMessage(content=question)]
     response = chat.invoke(messages, tools=tools)
     return json.dumps(response.additional_kwargs.get("tool_calls"))
 
 
 def use_langchain_chain(question="What is the capital of {location}?") -> str:
+    from langchain.chains import LLMChain
     from langchain.chat_models import ChatOpenAI
     from langchain_core.prompts import PromptTemplate
-    from langchain.chains import LLMChain
+
     from baserun.instrumentation.langchain import BaserunCallbackHandler
 
     chat = ChatOpenAI()
 
     chain = LLMChain(
         llm=chat,
         prompt=PromptTemplate(template=question, input_variables=["location"]),
@@ -523,20 +594,19 @@
     chain.run(location="California")
     response = chain.run(location="Georgia")
     return response
 
 
 def use_langchain_agent_tools(question="Using Wikipedia, look up the population of {location} as of 2023.") -> str:
     # Note: To run this, you must `pip install wikipedia langchain`
+    from langchain.agents import AgentType, initialize_agent, load_tools
     from langchain.chat_models import ChatOpenAI
-    from langchain_core.prompts import PromptTemplate
-    from langchain.agents import initialize_agent
-    from langchain.agents import AgentType
-    from langchain.agents import load_tools
     from langchain_core.callbacks import BaseCallbackManager
+    from langchain_core.prompts import PromptTemplate
+
     from baserun.instrumentation.langchain import BaserunCallbackHandler
 
     chat = ChatOpenAI()
     tools = load_tools(["wikipedia"])
     prompt_template = PromptTemplate(template=question, input_variables=["location"])
 
     agent = initialize_agent(
@@ -563,15 +633,15 @@
     contains_injection = baserun.evals.check_injection("question_injection", question)
     if contains_injection:
         print("Prompt contains an attack / injection! Not running")
         return "Aborted"
 
     client = OpenAI()
     completion = client.chat.completions.create(
-        model="gpt-3.5-turbo",
+        model="gpt-4o",
         messages=[{"role": "user", "content": question}],
     )
     content = completion.choices[0].message.content
     return content
 
 
 @baserun.trace
@@ -585,14 +655,59 @@
         messages=[{"role": "user", "content": prompt}],
     )
     content = completion.choices[0].message.content
     baserun.check_includes("openai_chat.content", content, "Washington")
     return content
 
 
+@baserun.trace
+def openai_moderation():
+    client = OpenAI()
+    client.moderations.create(input="Sample text goes here.")
+
+
+@baserun.trace
+def openai_embedding():
+    client = OpenAI()
+    client.embeddings.create(input="Example text", model="text-embedding-ada-002")
+
+
+def use_input_variables():
+    template_name = "Question & Answer"
+    template = baserun.register_template(TEMPLATES.get(template_name), template_name)
+    baserun.submit_input_variable(key="a", value="b", label="A", template=template)
+
+
+@baserun.trace
+def use_annotated_input_variables():
+    client = OpenAI()
+    completion = client.chat.completions.create(
+        model="gpt-4o",
+        messages=[{"role": "user", "content": "What is the capital of the US?"}],
+    )
+    annotation = baserun.annotate(completion.id)
+    annotation.input("country", "the US")
+    # there's a race condition because submit happens before the span is processed (and the completion is created)
+    annotation.submit()
+
+
+def use_contextmanager_multiple_calls():
+    with baserun.start_trace():
+        OpenAI().chat.completions.create(
+            model="gpt-4o",
+            messages=[{"role": "user", "content": "What is the capital of the US?"}],
+        )
+
+    with baserun.start_trace():
+        OpenAI().chat.completions.create(
+            model="gpt-4o",
+            messages=[{"role": "user", "content": "What is the capital of the US?"}],
+        )
+
+
 def call_function(functions, function_name: str, parsed_args: argparse.Namespace):
     function_to_call = functions.get(function_name)
     if function_to_call is None:
         function_to_call = {f: globals().get(f) for f in globals()}.get(function_name)
 
     if inspect.iscoroutinefunction(function_to_call):
         if parsed_args.prompt:
@@ -608,36 +723,38 @@
     print(result)
     return result
 
 
 # Allows you to call any of these functions, e.g. python tests/testing_functions.py openai_chat_functions_streaming
 if __name__ == "__main__":
     from dotenv import load_dotenv
+
     from baserun import Baserun
 
     load_dotenv()
     openai.api_key = os.environ.get("OPENAI_API_KEY")
-    Baserun.init()
 
     parser = argparse.ArgumentParser(description="Execute a function with a prompt.")
     parser.add_argument("function_to_call", type=str, help="Name of the function to call")
     parser.add_argument("--prompt", type=str, help="Prompt to pass to the function", default=None)
+    parser.add_argument("--skip-init", action="store_true", help="Skip Baserun.init()")
 
     parsed_args = parser.parse_args()
 
+    if not parsed_args.skip_init:
+        Baserun.init()
+
     # Resolve the string function name to the function object
     function_name = parsed_args.function_to_call
     global_variables = {f: globals().get(f) for f in globals()}
     traced_functions = {n: f for n, f in global_variables.items() if callable(f) and f.__name__ == "wrapper"}
     if function_name == "all":
         for name, func in traced_functions.items():
             print(f"===== Calling function {name} =====\n")
             try:
                 result = call_function(traced_functions, name, parsed_args)
                 print(f"----- {name} result:\n{result}\n-----")
-            except Exception as e:
-                traceback.print_exception(e)
+            except Exception:
+                exc_type, exc_value, exc_traceback = sys.exc_info()
+                traceback.print_exception(exc_type, exc_value, exc_traceback)
     else:
         call_function(traced_functions, function_name, parsed_args)
-
-    # Give time for the worker to clear the queue
-    sleep(0.5)
```

