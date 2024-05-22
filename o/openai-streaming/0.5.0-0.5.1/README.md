# Comparing `tmp/openai_streaming-0.5.0.tar.gz` & `tmp/openai_streaming-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_streaming-0.5.0.tar", last modified: Fri May 17 16:33:14 2024, max compression
+gzip compressed data, was "openai_streaming-0.5.1.tar", last modified: Wed May 22 10:28:14 2024, max compression
```

## Comparing `openai_streaming-0.5.0.tar` & `openai_streaming-0.5.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:33:14.410719 openai_streaming-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-17 16:33:14.406720 openai_streaming-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:33:14.406720 openai_streaming-0.5.0/openai_streaming/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/fn_dispatcher.py
--rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/stream_processing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:33:14.406720 openai_streaming-0.5.0/openai_streaming/struct/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/struct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5074 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/struct/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/struct/yaml_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/openai_streaming/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:33:14.406720 openai_streaming-0.5.0/openai_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7705 2024-05-17 16:33:14.000000 openai_streaming-0.5.0/openai_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-17 16:33:14.000000 openai_streaming-0.5.0/openai_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 16:33:14.000000 openai_streaming-0.5.0/openai_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-17 16:33:14.000000 openai_streaming-0.5.0/openai_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-17 16:33:14.000000 openai_streaming-0.5.0/openai_streaming.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-17 16:33:03.000000 openai_streaming-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 16:33:14.410719 openai_streaming-0.5.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 16:33:14.406720 openai_streaming-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/tests/test_with_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-17 16:33:02.000000 openai_streaming-0.5.0/tests/test_with_struct.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6931 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:28:14.091019 openai_streaming-0.5.1/openai_streaming/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3480 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/fn_dispatcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10514 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/stream_processing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/openai_streaming/struct/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/struct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5090 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/struct/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/struct/yaml_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3026 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/openai_streaming/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/openai_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7709 2024-05-22 10:28:14.000000 openai_streaming-0.5.1/openai_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      553 2024-05-22 10:28:14.000000 openai_streaming-0.5.1/openai_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:28:14.000000 openai_streaming-0.5.1/openai_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-05-22 10:28:14.000000 openai_streaming-0.5.1/openai_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 10:28:14.000000 openai_streaming-0.5.1/openai_streaming.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      857 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:28:14.095019 openai_streaming-0.5.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/tests/test_with_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-22 10:28:04.000000 openai_streaming-0.5.1/tests/test_with_struct.py
```

### Comparing `openai_streaming-0.5.0/LICENSE` & `openai_streaming-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/PKG-INFO` & `openai_streaming-0.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-streaming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Work with OpenAI's streaming API at ease, with Python generators
 Author-email: Almog Baku <almog.baku@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlmogBaku/openai-streaming
 Project-URL: Bug Reports, https://github.com/AlmogBaku/openai-streaming/issues
 Project-URL: Source, https://github.com/AlmogBaku/openai-streaming/
 Keywords: openai,gpt,llm,streaming,stream,generator
@@ -196,17 +196,17 @@
 
 You can also specify the output serialization format, either `json` or `yaml`, to parse the response (Friendly tip: YAML
 works better with LLMs).
 
 # 🤔 What's the big deal? Why use this library?
 
 The OpenAI Streaming API is robust but challenging to navigate. Using the `stream=True` flag, we get tokens as they are
-generated, instead of waiting for the entire response - this can create a much friendlier user experience with the
-illusion of quicker response times. However, this involves complex tasks like manual stream handling
-and response parsing, especially when using OpenAI Functions or complex outputs.
+generated, instead of waiting for the entire response — this can create a much friendlier user experience with the
+illusion of a quicker response time. However, this involves complex tasks like manual stream handling  and response
+parsing, especially when using OpenAI Functions or complex outputs.
 
 `openai-streaming` is a small library that simplifies this by offering a straightforward Python Generator interface for
 handling streaming responses.
 
 # 📑 Reference Documentation
 
 For more information, please refer to the [reference documentation](/docs/reference.md).
```

### Comparing `openai_streaming-0.5.0/README.md` & `openai_streaming-0.5.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -176,17 +176,17 @@
 
 You can also specify the output serialization format, either `json` or `yaml`, to parse the response (Friendly tip: YAML
 works better with LLMs).
 
 # 🤔 What's the big deal? Why use this library?
 
 The OpenAI Streaming API is robust but challenging to navigate. Using the `stream=True` flag, we get tokens as they are
-generated, instead of waiting for the entire response - this can create a much friendlier user experience with the
-illusion of quicker response times. However, this involves complex tasks like manual stream handling
-and response parsing, especially when using OpenAI Functions or complex outputs.
+generated, instead of waiting for the entire response — this can create a much friendlier user experience with the
+illusion of a quicker response time. However, this involves complex tasks like manual stream handling  and response
+parsing, especially when using OpenAI Functions or complex outputs.
 
 `openai-streaming` is a small library that simplifies this by offering a straightforward Python Generator interface for
 handling streaming responses.
 
 # 📑 Reference Documentation
 
 For more information, please refer to the [reference documentation](/docs/reference.md).
```

### Comparing `openai_streaming-0.5.0/openai_streaming/decorator.py` & `openai_streaming-0.5.1/openai_streaming/decorator.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/openai_streaming/fn_dispatcher.py` & `openai_streaming-0.5.1/openai_streaming/fn_dispatcher.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/openai_streaming/stream_processing.py` & `openai_streaming-0.5.1/openai_streaming/stream_processing.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/openai_streaming/struct/handler.py` & `openai_streaming-0.5.1/openai_streaming/struct/handler.py`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,15 @@
 
         :param part: A dictionary containing the parsed part of the response
         :return: The parsed part of the response as an `TModel` object, `Terminate` to terminate the handling,
         or `None` if the part is not valid
         """
         try:
             typ = get_args(type(self.handler).__orig_bases__[0])[0]
-            parsed = typ(**part)
+            parsed = typ.model_construct(**part)
         except (TypeError, ValueError):
             return
 
         ret = await self.handler.handle_partially_parsed(parsed)
         return ret if ret else parsed
 
     def get_last_response(self) -> Optional[Union[TModel, Terminate]]:
```

### Comparing `openai_streaming-0.5.0/openai_streaming/struct/yaml_parser.py` & `openai_streaming-0.5.1/openai_streaming/struct/yaml_parser.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/openai_streaming/utils.py` & `openai_streaming-0.5.1/openai_streaming/utils.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/openai_streaming.egg-info/PKG-INFO` & `openai_streaming-0.5.1/openai_streaming.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-streaming
-Version: 0.5.0
+Version: 0.5.1
 Summary: Work with OpenAI's streaming API at ease, with Python generators
 Author-email: Almog Baku <almog.baku@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/AlmogBaku/openai-streaming
 Project-URL: Bug Reports, https://github.com/AlmogBaku/openai-streaming/issues
 Project-URL: Source, https://github.com/AlmogBaku/openai-streaming/
 Keywords: openai,gpt,llm,streaming,stream,generator
@@ -196,17 +196,17 @@
 
 You can also specify the output serialization format, either `json` or `yaml`, to parse the response (Friendly tip: YAML
 works better with LLMs).
 
 # 🤔 What's the big deal? Why use this library?
 
 The OpenAI Streaming API is robust but challenging to navigate. Using the `stream=True` flag, we get tokens as they are
-generated, instead of waiting for the entire response - this can create a much friendlier user experience with the
-illusion of quicker response times. However, this involves complex tasks like manual stream handling
-and response parsing, especially when using OpenAI Functions or complex outputs.
+generated, instead of waiting for the entire response — this can create a much friendlier user experience with the
+illusion of a quicker response time. However, this involves complex tasks like manual stream handling  and response
+parsing, especially when using OpenAI Functions or complex outputs.
 
 `openai-streaming` is a small library that simplifies this by offering a straightforward Python Generator interface for
 handling streaming responses.
 
 # 📑 Reference Documentation
 
 For more information, please refer to the [reference documentation](/docs/reference.md).
```

### Comparing `openai_streaming-0.5.0/openai_streaming.egg-info/SOURCES.txt` & `openai_streaming-0.5.1/openai_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/pyproject.toml` & `openai_streaming-0.5.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "openai-streaming"
-version = "0.5.0"
+version = "0.5.1"
 description = "Work with OpenAI's streaming API at ease, with Python generators"
 authors = [{ name = "Almog Baku", email = "almog.baku@gmail.com" }]
 license = { text = "MIT" }
 readme = "README.md"
 keywords = ["openai", "gpt", "llm", "streaming", "stream", "generator"]
 dependencies = [
     "openai>=1.14.0,<2.0.0",
```

### Comparing `openai_streaming-0.5.0/tests/test_with_functions.py` & `openai_streaming-0.5.1/tests/test_with_functions.py`

 * *Files identical despite different names*

### Comparing `openai_streaming-0.5.0/tests/test_with_struct.py` & `openai_streaming-0.5.1/tests/test_with_struct.py`

 * *Files identical despite different names*

