# Comparing `tmp/langchain_aws-0.1.3.tar.gz` & `tmp/langchain_aws-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_aws-0.1.3.tar", max compression
+gzip compressed data, was "langchain_aws-0.1.4.tar", max compression
```

## Comparing `langchain_aws-0.1.3.tar` & `langchain_aws-0.1.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1072 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/LICENSE
--rw-r--r--   0        0        0     1537 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/README.md
--rw-r--r--   0        0        0      611 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/__init__.py
--rw-r--r--   0        0        0      113 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/chat_models/__init__.py
--rw-r--r--   0        0        0    15869 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/chat_models/bedrock.py
--rw-r--r--   0        0        0       96 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/embeddings/__init__.py
--rw-r--r--   0        0        0     7282 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/embeddings/bedrock.py
--rw-r--r--   0        0        0     3808 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/function_calling.py
--rw-r--r--   0        0        0      191 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/__init__.py
--rw-r--r--   0        0        0    14347 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/neptune_graph.py
--rw-r--r--   0        0        0    10331 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/graphs/neptune_rdf_graph.py
--rw-r--r--   0        0        0      297 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/__init__.py
--rw-r--r--   0        0        0    31761 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/bedrock.py
--rw-r--r--   0        0        0    13595 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/llms/sagemaker_endpoint.py
--rw-r--r--   0        0        0        0 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/py.typed
--rw-r--r--   0        0        0      251 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/__init__.py
--rw-r--r--   0        0        0     4745 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/bedrock.py
--rw-r--r--   0        0        0    15189 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/retrievers/kendra.py
--rw-r--r--   0        0        0     1033 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/langchain_aws/utils.py
--rw-r--r--   0        0        0     2737 2024-05-08 01:29:22.769440 langchain_aws-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2380 1970-01-01 00:00:00.000000 langchain_aws-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-16 02:46:20.484413 langchain_aws-0.1.4/LICENSE
+-rw-r--r--   0        0        0     1537 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/README.md
+-rw-r--r--   0        0        0      611 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/__init__.py
+-rw-r--r--   0        0        0      113 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/chat_models/__init__.py
+-rw-r--r--   0        0        0    17269 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/chat_models/bedrock.py
+-rw-r--r--   0        0        0       96 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/embeddings/__init__.py
+-rw-r--r--   0        0        0     7282 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/embeddings/bedrock.py
+-rw-r--r--   0        0        0     3808 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/function_calling.py
+-rw-r--r--   0        0        0      191 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/graphs/__init__.py
+-rw-r--r--   0        0        0    14347 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/graphs/neptune_graph.py
+-rw-r--r--   0        0        0    10331 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/graphs/neptune_rdf_graph.py
+-rw-r--r--   0        0        0      297 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/llms/__init__.py
+-rw-r--r--   0        0        0    31838 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/llms/bedrock.py
+-rw-r--r--   0        0        0    13595 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/llms/sagemaker_endpoint.py
+-rw-r--r--   0        0        0        0 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/py.typed
+-rw-r--r--   0        0        0      251 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/retrievers/__init__.py
+-rw-r--r--   0        0        0     4745 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/retrievers/bedrock.py
+-rw-r--r--   0        0        0    15189 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/retrievers/kendra.py
+-rw-r--r--   0        0        0     1033 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/langchain_aws/utils.py
+-rw-r--r--   0        0        0     2743 2024-05-16 02:46:20.488413 langchain_aws-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2378 1970-01-01 00:00:00.000000 langchain_aws-0.1.4/PKG-INFO
```

### Comparing `langchain_aws-0.1.3/LICENSE` & `langchain_aws-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/README.md` & `langchain_aws-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/__init__.py` & `langchain_aws-0.1.4/langchain_aws/__init__.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/chat_models/bedrock.py` & `langchain_aws-0.1.4/langchain_aws/chat_models/bedrock.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,14 +60,49 @@
     """Convert a list of messages to a prompt for llama."""
 
     return "\n".join(
         [_convert_one_message_to_text_llama(message) for message in messages]
     )
 
 
+def _convert_one_message_to_text_llama3(message: BaseMessage) -> str:
+    if isinstance(message, ChatMessage):
+        message_text = (
+            f"<|start_header_id|>{message.role}"
+            f"<|end_header_id|>{message.content}<|eot_id|>"
+        )
+    elif isinstance(message, HumanMessage):
+        message_text = (
+            f"<|start_header_id|>user" f"<|end_header_id|>{message.content}<|eot_id|>"
+        )
+    elif isinstance(message, AIMessage):
+        message_text = (
+            f"<|start_header_id|>assistant"
+            f"<|end_header_id|>{message.content}<|eot_id|>"
+        )
+    elif isinstance(message, SystemMessage):
+        message_text = (
+            f"<|start_header_id|>system" f"<|end_header_id|>{message.content}<|eot_id|>"
+        )
+    else:
+        raise ValueError(f"Got unknown type {message}")
+
+    return message_text
+
+
+def convert_messages_to_prompt_llama3(messages: List[BaseMessage]) -> str:
+    """Convert a list of messages to a prompt for llama."""
+
+    return "\n".join(
+        ["<|begin_of_text|>"]
+        + [_convert_one_message_to_text_llama3(message) for message in messages]
+        + ["<|start_header_id|>assistant<|end_header_id|>\n\n"]
+    )
+
+
 def _convert_one_message_to_text_anthropic(
     message: BaseMessage,
     human_prompt: str,
     ai_prompt: str,
 ) -> str:
     content = cast(str, message.content)
     if isinstance(message, ChatMessage):
@@ -239,20 +274,23 @@
 class ChatPromptAdapter:
     """Adapter class to prepare the inputs from Langchain to prompt format
     that Chat model expects.
     """
 
     @classmethod
     def convert_messages_to_prompt(
-        cls, provider: str, messages: List[BaseMessage]
+        cls, provider: str, messages: List[BaseMessage], model: str
     ) -> str:
         if provider == "anthropic":
             prompt = convert_messages_to_prompt_anthropic(messages=messages)
         elif provider == "meta":
-            prompt = convert_messages_to_prompt_llama(messages=messages)
+            if "llama3" in model:
+                prompt = convert_messages_to_prompt_llama3(messages=messages)
+            else:
+                prompt = convert_messages_to_prompt_llama(messages=messages)
         elif provider == "mistral":
             prompt = convert_messages_to_prompt_mistral(messages=messages)
         elif provider == "amazon":
             prompt = convert_messages_to_prompt_anthropic(
                 messages=messages,
                 human_prompt="\n\nUser:",
                 ai_prompt="\n\nBot:",
@@ -329,15 +367,15 @@
             if self.system_prompt_with_tools:
                 if system:
                     system = self.system_prompt_with_tools + f"\n{system}"
                 else:
                     system = self.system_prompt_with_tools
         else:
             prompt = ChatPromptAdapter.convert_messages_to_prompt(
-                provider=provider, messages=messages
+                provider=provider, messages=messages, model=self._get_model()
             )
 
         for chunk in self._prepare_input_and_invoke_stream(
             prompt=prompt,
             system=system,
             messages=formatted_messages,
             stop=stop,
@@ -372,15 +410,15 @@
                 if self.system_prompt_with_tools:
                     if system:
                         system = self.system_prompt_with_tools + f"\n{system}"
                     else:
                         system = self.system_prompt_with_tools
             else:
                 prompt = ChatPromptAdapter.convert_messages_to_prompt(
-                    provider=provider, messages=messages
+                    provider=provider, messages=messages, model=self._get_model()
                 )
 
             if stop:
                 params["stop_sequences"] = stop
 
             completion, usage_info = self._prepare_input_and_invoke(
                 prompt=prompt,
```

### Comparing `langchain_aws-0.1.3/langchain_aws/embeddings/bedrock.py` & `langchain_aws-0.1.4/langchain_aws/embeddings/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/function_calling.py` & `langchain_aws-0.1.4/langchain_aws/function_calling.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/graphs/neptune_graph.py` & `langchain_aws-0.1.4/langchain_aws/graphs/neptune_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/graphs/neptune_rdf_graph.py` & `langchain_aws-0.1.4/langchain_aws/graphs/neptune_rdf_graph.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/llms/bedrock.py` & `langchain_aws-0.1.4/langchain_aws/llms/bedrock.py`

 * *Files 0% similar despite different names*

```diff
@@ -459,14 +459,17 @@
             raise ValueError(
                 "Model provider should be supplied when passing a model ARN as "
                 "model_id"
             )
 
         return self.model_id.split(".")[0]
 
+    def _get_model(self) -> str:
+        return self.model_id.split(".")[1]
+
     @property
     def _model_is_anthropic(self) -> bool:
         return self._get_provider() == "anthropic"
 
     @property
     def _guardrails_enabled(self) -> bool:
         """
```

### Comparing `langchain_aws-0.1.3/langchain_aws/llms/sagemaker_endpoint.py` & `langchain_aws-0.1.4/langchain_aws/llms/sagemaker_endpoint.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/retrievers/bedrock.py` & `langchain_aws-0.1.4/langchain_aws/retrievers/bedrock.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/retrievers/kendra.py` & `langchain_aws-0.1.4/langchain_aws/retrievers/kendra.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/langchain_aws/utils.py` & `langchain_aws-0.1.4/langchain_aws/utils.py`

 * *Files identical despite different names*

### Comparing `langchain_aws-0.1.3/pyproject.toml` & `langchain_aws-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "langchain-aws"
-version = "0.1.3"
+version = "0.1.4"
 description = "An integration package connecting AWS and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain-aws"
 license = "MIT"
 
 [tool.poetry.urls]
 "Source Code" = "https://github.com/langchain-ai/langchain-aws/tree/main/libs/aws"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
-langchain-core = "^0.1.45"
+langchain-core = ">=0.1.45,<0.3"
 boto3 = ">=1.34.51,<1.35.0"
 numpy = "^1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
```

### Comparing `langchain_aws-0.1.3/PKG-INFO` & `langchain_aws-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: langchain-aws
-Version: 0.1.3
+Version: 0.1.4
 Summary: An integration package connecting AWS and LangChain
 Home-page: https://github.com/langchain-ai/langchain-aws
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.51,<1.35.0)
-Requires-Dist: langchain-core (>=0.1.45,<0.2.0)
+Requires-Dist: langchain-core (>=0.1.45,<0.3)
 Requires-Dist: numpy (>=1,<2)
 Project-URL: Repository, https://github.com/langchain-ai/langchain-aws
 Project-URL: Source Code, https://github.com/langchain-ai/langchain-aws/tree/main/libs/aws
 Description-Content-Type: text/markdown
 
 # langchain-aws
```

