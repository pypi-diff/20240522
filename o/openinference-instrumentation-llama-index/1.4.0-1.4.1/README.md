# Comparing `tmp/openinference_instrumentation_llama_index-1.4.0.tar.gz` & `tmp/openinference_instrumentation_llama_index-1.4.1.tar.gz`

## Comparing `openinference_instrumentation_llama_index-1.4.0.tar` & `openinference_instrumentation_llama_index-1.4.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/__init__.py
--rw-r--r--   0        0        0    31854 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_callback.py
--rw-r--r--   0        0        0    23610 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_handler.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/version.py
--rw-r--r--   0        0        0    19611 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_callback.py
--rw-r--r--   0        0        0    20983 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_handler.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/LICENSE
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/README.md
--rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     4361 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/__init__.py
+-rw-r--r--   0        0        0    31901 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/_callback.py
+-rw-r--r--   0        0        0    23583 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/_handler.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/version.py
+-rw-r--r--   0        0        0    19611 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/tests/openinference/instrumentation/llama_index/test_callback.py
+-rw-r--r--   0        0        0    20983 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/tests/openinference/instrumentation/llama_index/test_handler.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/LICENSE
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/README.md
+-rw-r--r--   0        0        0     2082 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     4959 2020-02-02 00:00:00.000000 openinference_instrumentation_llama_index-1.4.1/PKG-INFO
```

### Comparing `openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/__init__.py` & `openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_callback.py` & `openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/_callback.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     Tuple,
     TypeVar,
     Union,
     cast,
 )
 from uuid import uuid4
 
-from openinference.instrumentation import get_attributes_from_context
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.semconv.trace import (
     DocumentAttributes,
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     RerankerAttributes,
@@ -100,15 +100,15 @@
     if event_type is not CBEventType.RERANKING and EventPayload.NODES in payload:
         attributes[RETRIEVAL_DOCUMENTS] = [
             {
                 DOCUMENT_ID: node_with_score.node.node_id,
                 DOCUMENT_SCORE: node_with_score.score,
                 DOCUMENT_CONTENT: node_with_score.node.text,
                 **(
-                    {DOCUMENT_METADATA: json.dumps(metadata)}
+                    {DOCUMENT_METADATA: safe_json_dumps(metadata)}
                     if (metadata := node_with_score.node.metadata)
                     else {}
                 ),
             }
             for node_with_score in payload[EventPayload.NODES]
         ]
     if EventPayload.PROMPT in payload:
@@ -147,38 +147,38 @@
         if nodes := payload.get(EventPayload.NODES):
             attributes[RERANKER_OUTPUT_DOCUMENTS if is_event_end else RERANKER_INPUT_DOCUMENTS] = [
                 {
                     DOCUMENT_ID: node_with_score.node.node_id,
                     DOCUMENT_SCORE: node_with_score.score,
                     DOCUMENT_CONTENT: node_with_score.node.text,
                     **(
-                        {DOCUMENT_METADATA: json.dumps(metadata)}
+                        {DOCUMENT_METADATA: safe_json_dumps(metadata)}
                         if (metadata := node_with_score.node.metadata)
                         else {}
                     ),
                 }
                 for node_with_score in nodes
             ]
     if EventPayload.TOOL in payload:
         tool_metadata = cast(ToolMetadata, payload.get(EventPayload.TOOL))
         attributes[TOOL_NAME] = tool_metadata.name
         attributes[TOOL_DESCRIPTION] = tool_metadata.description
         if tool_parameters := tool_metadata.to_openai_tool()["function"]["parameters"]:
-            attributes[TOOL_PARAMETERS] = json.dumps(tool_parameters)
+            attributes[TOOL_PARAMETERS] = safe_json_dumps(tool_parameters)
     if EventPayload.SERIALIZED in payload:
         serialized = payload[EventPayload.SERIALIZED]
         if event_type is CBEventType.EMBEDDING:
             if model_name := serialized.get("model_name"):
                 attributes[EMBEDDING_MODEL_NAME] = model_name
         if event_type is CBEventType.LLM:
             if model_name := serialized.get("model"):
                 attributes[LLM_MODEL_NAME] = model_name
                 invocation_parameters = _extract_invocation_parameters(serialized)
                 invocation_parameters["model"] = model_name
-                attributes[LLM_INVOCATION_PARAMETERS] = json.dumps(invocation_parameters)
+                attributes[LLM_INVOCATION_PARAMETERS] = safe_json_dumps(invocation_parameters)
     return attributes
 
 
 def _extract_invocation_parameters(serialized: Mapping[str, Any]) -> Dict[str, Any]:
     # FIXME: this is only based on openai. Other models have different parameters.
     if not hasattr(serialized, "get"):
         return {}
@@ -552,15 +552,15 @@
     the name of the function to call and the arguments to call it with.
     """
     if isinstance(response, ChatResponse):
         message = response.message
         if content := message.content:
             yield OUTPUT_VALUE, content
         else:
-            yield OUTPUT_VALUE, json.dumps(message.additional_kwargs, cls=_CustomJSONEncoder)
+            yield OUTPUT_VALUE, safe_json_dumps(message.additional_kwargs, cls=_CustomJSONEncoder)
             yield OUTPUT_MIME_TYPE, OpenInferenceMimeTypeValues.JSON.value
     elif isinstance(response, Response):
         if response.response:
             yield OUTPUT_VALUE, response.response
     elif isinstance(response, StreamingResponse):
         if response_txt := getattr(response, "response_txt", None):
             yield OUTPUT_VALUE, response_txt
@@ -640,15 +640,15 @@
 def _template_attributes(payload: Dict[str, Any]) -> Iterator[Tuple[str, Any]]:
     """
     Yields template attributes if present
     """
     if template := payload.get(EventPayload.TEMPLATE):
         yield LLM_PROMPT_TEMPLATE, template
     if template_vars := payload.get(EventPayload.TEMPLATE_VARS):
-        yield LLM_PROMPT_TEMPLATE_VARIABLES, json.dumps(template_vars)
+        yield LLM_PROMPT_TEMPLATE_VARIABLES, safe_json_dumps(template_vars)
 
 
 def _get_tool_call(tool_call: object) -> Iterator[Tuple[str, Any]]:
     if function := getattr(tool_call, "function", None):
         if name := getattr(function, "name", None):
             assert isinstance(name, str), f"name must be str, found {type(name)}"
             yield TOOL_CALL_FUNCTION_NAME, name
```

### Comparing `openinference_instrumentation_llama_index-1.4.0/src/openinference/instrumentation/llama_index/_handler.py` & `openinference_instrumentation_llama_index-1.4.1/src/openinference/instrumentation/llama_index/_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import inspect
-import json
 import logging
 from functools import singledispatch, singledispatchmethod
 from time import time_ns
 from typing import Any, Dict, Iterator, List, Mapping, Optional, Tuple, Union
 
-from openinference.instrumentation import get_attributes_from_context
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.semconv.trace import (
     DocumentAttributes,
     EmbeddingAttributes,
     MessageAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     RerankerAttributes,
@@ -171,15 +170,15 @@
 
     @process_event.register
     def _(self, event: AgentToolCallEvent) -> None:
         tool = event.tool
         if name := tool.name:
             self[TOOL_NAME] = name
         self[TOOL_DESCRIPTION] = tool.description
-        self[TOOL_PARAMETERS] = json.dumps(tool.get_parameters_dict(), default=str)
+        self[TOOL_PARAMETERS] = safe_json_dumps(tool.get_parameters_dict())
 
     @process_event.register
     def _(self, event: EmbeddingStartEvent) -> None:
         if not self._span_kind:
             self._span_kind = EMBEDDING
 
     @process_event.register
@@ -223,15 +222,15 @@
         }
         template_arguments = {
             variable_name: argument_value
             for variable_name in variable_names
             if (argument_value := argument_values.get(variable_name)) is not None
         }
         if template_arguments:
-            self[LLM_PROMPT_TEMPLATE_VARIABLES] = json.dumps(template_arguments, default=str)
+            self[LLM_PROMPT_TEMPLATE_VARIABLES] = safe_json_dumps(template_arguments)
 
     @process_event.register
     def _(self, event: LLMPredictEndEvent) -> None:
         self[OUTPUT_VALUE] = event.output
 
     @process_event.register
     def _(self, event: LLMStructuredPredictStartEvent) -> None:
@@ -358,15 +357,15 @@
         for i, node in enumerate(nodes):
             self[f"{prefix}.{i}.{DOCUMENT_ID}"] = node.node_id
             if content := node.get_content():
                 self[f"{prefix}.{i}.{DOCUMENT_CONTENT}"] = content
             if (score := node.get_score()) is not None:
                 self[f"{prefix}.{i}.{DOCUMENT_SCORE}"] = score
             if metadata := node.metadata:
-                self[f"{prefix}.{i}.{DOCUMENT_METADATA}"] = json.dumps(metadata, default=str)
+                self[f"{prefix}.{i}.{DOCUMENT_METADATA}"] = safe_json_dumps(metadata)
 
     def _process_messages(self, prefix: str, *messages: ChatMessage) -> None:
         for i, message in enumerate(messages):
             self[f"{prefix}.{i}.{MESSAGE_ROLE}"] = message.role.value
             if content := message.content:
                 self[f"{prefix}.{i}.{MESSAGE_CONTENT}"] = str(content)
             additional_kwargs = message.additional_kwargs
@@ -384,15 +383,15 @@
             self[INPUT_VALUE] = query
         elif isinstance(query, QueryBundle):
             query_dict = {k: v for k, v in query.to_dict().items() if v is not None}
             query_dict.pop("embedding", None)  # because it takes up too much space
             if len(query_dict) == 1 and query.query_str:
                 self[INPUT_VALUE] = query.query_str
             else:
-                self[INPUT_VALUE] = json.dumps(query_dict, default=str)
+                self[INPUT_VALUE] = safe_json_dumps(query_dict)
                 self[INPUT_MIME_TYPE] = JSON
         else:
             assert_never(query)
 
     def _process_response_type(self, response: Optional[RESPONSE_TYPE]) -> None:
         if response is None:
             return
```

### Comparing `openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_callback.py` & `openinference_instrumentation_llama_index-1.4.1/tests/openinference/instrumentation/llama_index/test_callback.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.4.0/tests/openinference/instrumentation/llama_index/test_handler.py` & `openinference_instrumentation_llama_index-1.4.1/tests/openinference/instrumentation/llama_index/test_handler.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.4.0/LICENSE` & `openinference_instrumentation_llama_index-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.4.0/README.md` & `openinference_instrumentation_llama_index-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_llama_index-1.4.0/pyproject.toml` & `openinference_instrumentation_llama_index-1.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
-  "openinference-instrumentation>=0.1.5",
+  "openinference-instrumentation>=0.1.7",
   "openinference-semantic-conventions",
   "typing-extensions",
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
```

### Comparing `openinference_instrumentation_llama_index-1.4.0/PKG-INFO` & `openinference_instrumentation_llama_index-1.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-llama-index
-Version: 1.4.0
+Version: 1.4.1
 Summary: OpenInference LlamaIndex Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-llama-index
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.8
-Requires-Dist: openinference-instrumentation>=0.1.5
+Requires-Dist: openinference-instrumentation>=0.1.7
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
```

