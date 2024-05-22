# Comparing `tmp/langchain_google_genai-1.0.4.tar.gz` & `tmp/langchain_google_genai-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_google_genai-1.0.4.tar", max compression
+gzip compressed data, was "langchain_google_genai-1.0.5.tar", max compression
```

## Comparing `langchain_google_genai-1.0.4.tar` & `langchain_google_genai-1.0.5.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     1072 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/LICENSE
--rw-r--r--   0        0        0     2875 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/README.md
--rw-r--r--   0        0        0     2758 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/__init__.py
--rw-r--r--   0        0        0     1576 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_common.py
--rw-r--r--   0        0        0      197 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_enums.py
--rw-r--r--   0        0        0     8232 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_function_utils.py
--rw-r--r--   0        0        0    20769 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_genai_extension.py
--rw-r--r--   0        0        0     4999 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/_image_utils.py
--rw-r--r--   0        0        0    33014 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/chat_models.py
--rw-r--r--   0        0        0     6578 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/embeddings.py
--rw-r--r--   0        0        0     4303 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/genai_aqa.py
--rw-r--r--   0        0        0    16139 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/google_vector_store.py
--rw-r--r--   0        0        0    13431 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/llms.py
--rw-r--r--   0        0        0        0 2024-05-16 13:42:50.386237 langchain_google_genai-1.0.4/langchain_google_genai/py.typed
--rw-r--r--   0        0        0     3019 2024-05-16 13:42:50.390237 langchain_google_genai-1.0.4/pyproject.toml
--rw-r--r--   0        0        0     3818 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2875 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/README.md
+-rw-r--r--   0        0        0     2758 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/__init__.py
+-rw-r--r--   0        0        0     1576 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/_common.py
+-rw-r--r--   0        0        0      197 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/_enums.py
+-rw-r--r--   0        0        0     8232 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/_function_utils.py
+-rw-r--r--   0        0        0    20769 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/_genai_extension.py
+-rw-r--r--   0        0        0     4999 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/_image_utils.py
+-rw-r--r--   0        0        0    33799 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/chat_models.py
+-rw-r--r--   0        0        0     6578 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/embeddings.py
+-rw-r--r--   0        0        0     4303 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/genai_aqa.py
+-rw-r--r--   0        0        0    16139 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/google_vector_store.py
+-rw-r--r--   0        0        0    13431 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/llms.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/langchain_google_genai/py.typed
+-rw-r--r--   0        0        0     3018 2024-05-21 23:57:08.144052 langchain_google_genai-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0     3817 1970-01-01 00:00:00.000000 langchain_google_genai-1.0.5/PKG-INFO
```

### Comparing `langchain_google_genai-1.0.4/LICENSE` & `langchain_google_genai-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/README.md` & `langchain_google_genai-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/__init__.py` & `langchain_google_genai-1.0.5/langchain_google_genai/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/_common.py` & `langchain_google_genai-1.0.5/langchain_google_genai/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/_function_utils.py` & `langchain_google_genai-1.0.5/langchain_google_genai/_function_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/_genai_extension.py` & `langchain_google_genai-1.0.5/langchain_google_genai/_genai_extension.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/_image_utils.py` & `langchain_google_genai-1.0.5/langchain_google_genai/_image_utils.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/chat_models.py` & `langchain_google_genai-1.0.5/langchain_google_genai/chat_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+import asyncio
 import base64
 import json
 import logging
 import os
 import uuid
 import warnings
 from io import BytesIO
@@ -554,14 +555,22 @@
                 message=(AIMessageChunk if stream else AIMessage)(content=""),
                 generation_info={},
             )
         ]
     return ChatResult(generations=generations, llm_output=llm_output)
 
 
+def _is_event_loop_running() -> bool:
+    try:
+        asyncio.get_running_loop()
+        return True
+    except RuntimeError:
+        return False
+
+
 class ChatGoogleGenerativeAI(_BaseGoogleGenerativeAI, BaseChatModel):
     """`Google Generative AI` Chat models API.
 
     To use, you must have either:
 
         1. The ``GOOGLE_API_KEY``` environment variable set with your API key, or
         2. Pass your API key using the google_api_key kwarg to the ChatGoogle
@@ -635,21 +644,30 @@
         values["client"] = genaix.build_generative_service(
             credentials=values.get("credentials"),
             api_key=google_api_key,
             client_info=client_info,
             client_options=values.get("client_options"),
             transport=transport,
         )
-        values["async_client"] = genaix.build_generative_async_service(
-            credentials=values.get("credentials"),
-            api_key=google_api_key,
-            client_info=client_info,
-            client_options=values.get("client_options"),
-            transport=transport,
-        )
+
+        # NOTE: genaix.build_generative_async_service requires
+        # a running event loop, which causes an error
+        # when initialized inside a ThreadPoolExecutor.
+        # this check ensures that async client is only initialized
+        # within an asyncio event loop to avoid the error
+        if _is_event_loop_running():
+            values["async_client"] = genaix.build_generative_async_service(
+                credentials=values.get("credentials"),
+                api_key=google_api_key,
+                client_info=client_info,
+                client_options=values.get("client_options"),
+                transport=transport,
+            )
+        else:
+            values["async_client"] = None
 
         return values
 
     @property
     def _identifying_params(self) -> Dict[str, Any]:
         """Get the identifying parameters."""
         return {
@@ -720,14 +738,20 @@
         tools: Optional[Sequence[Union[ToolDict, GoogleTool]]] = None,
         functions: Optional[Sequence[FunctionDeclarationType]] = None,
         safety_settings: Optional[SafetySettingDict] = None,
         tool_config: Optional[Union[Dict, _ToolConfigDict]] = None,
         generation_config: Optional[Dict[str, Any]] = None,
         **kwargs: Any,
     ) -> ChatResult:
+        if not self.async_client:
+            raise RuntimeError(
+                "Initialize ChatGoogleGenerativeAI with a running event loop "
+                "to use async methods."
+            )
+
         request = self._prepare_request(
             messages,
             stop=stop,
             tools=tools,
             functions=functions,
             safety_settings=safety_settings,
             tool_config=tool_config,
```

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/embeddings.py` & `langchain_google_genai-1.0.5/langchain_google_genai/embeddings.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/genai_aqa.py` & `langchain_google_genai-1.0.5/langchain_google_genai/genai_aqa.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/google_vector_store.py` & `langchain_google_genai-1.0.5/langchain_google_genai/google_vector_store.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/langchain_google_genai/llms.py` & `langchain_google_genai-1.0.5/langchain_google_genai/llms.py`

 * *Files identical despite different names*

### Comparing `langchain_google_genai-1.0.4/pyproject.toml` & `langchain_google_genai-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-google-genai"
-version = "1.0.4"
+version = "1.0.5"
 description = "An integration package connecting Google's genai package and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-google"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-google/tree/main/libs/genai"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
-langchain-core = ">=0.1.45,<0.3"
+langchain-core = ">=0.2.0,<0.3"
 google-generativeai = "^0.5.2"
 pillow = { version = "^10.1.0", optional = true }
 
 [tool.poetry.extras]
 images = ["pillow"]
 
 [tool.poetry.group.test]
```

### Comparing `langchain_google_genai-1.0.4/PKG-INFO` & `langchain_google_genai-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: langchain-google-genai
-Version: 1.0.4
+Version: 1.0.5
 Summary: An integration package connecting Google's genai package and LangChain
 Home-page: https://github.com/langchain-ai/langchain-google
 License: MIT
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: images
 Requires-Dist: google-generativeai (>=0.5.2,<0.6.0)
-Requires-Dist: langchain-core (>=0.1.45,<0.3)
+Requires-Dist: langchain-core (>=0.2.0,<0.3)
 Requires-Dist: pillow (>=10.1.0,<11.0.0) ; extra == "images"
 Project-URL: Repository, https://github.com/langchain-ai/langchain-google
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-google/tree/main/libs/genai
 Description-Content-Type: text/markdown
 
 # langchain-google-genai
```

