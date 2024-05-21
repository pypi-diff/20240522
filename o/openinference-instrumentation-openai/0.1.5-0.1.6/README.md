# Comparing `tmp/openinference_instrumentation_openai-0.1.5.tar.gz` & `tmp/openinference_instrumentation_openai-0.1.6.tar.gz`

## Comparing `openinference_instrumentation_openai-0.1.5.tar` & `openinference_instrumentation_openai-0.1.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request.py
--rw-r--r--   0        0        0     7675 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request_attributes_extractor.py
--rw-r--r--   0        0        0     9090 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_accumulator.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_attributes_extractor.py
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_stream.py
--rw-r--r--   0        0        0     4592 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_utils.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_with_span.py
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/version.py
--rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/tests/openinference/instrumentation/openai/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/LICENSE
--rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/README.md
--rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0    17823 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_request.py
+-rw-r--r--   0        0        0     7746 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_request_attributes_extractor.py
+-rw-r--r--   0        0        0     9146 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_response_accumulator.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_response_attributes_extractor.py
+-rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_stream.py
+-rw-r--r--   0        0        0     4643 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_utils.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_with_span.py
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/version.py
+-rw-r--r--   0        0        0    35160 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/tests/openinference/instrumentation/openai/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2703 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/README.md
+-rw-r--r--   0        0        0     2035 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 openinference_instrumentation_openai-0.1.6/PKG-INFO
```

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/__init__.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_request.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_request_attributes_extractor.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_request_attributes_extractor.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import json
 import logging
 from enum import Enum
 from types import ModuleType
 from typing import (
     TYPE_CHECKING,
     Any,
     Iterable,
     Iterator,
     List,
     Mapping,
     Tuple,
     Type,
 )
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.instrumentation.openai._utils import _get_openai_version
 from openinference.semconv.trace import MessageAttributes, SpanAttributes, ToolCallAttributes
 from opentelemetry.util.types import AttributeValue
 
 if TYPE_CHECKING:
     from openai.types import Completion, CreateEmbeddingResponse
     from openai.types.chat import ChatCompletion
@@ -54,15 +54,15 @@
             yield from _get_attributes_from_chat_completion_create_param(request_parameters)
         elif cast_to is self._create_embedding_response_type:
             yield from _get_attributes_from_embedding_create_param(request_parameters)
         elif cast_to is self._completion_type:
             yield from _get_attributes_from_completion_create_param(request_parameters)
         else:
             try:
-                yield SpanAttributes.LLM_INVOCATION_PARAMETERS, json.dumps(request_parameters)
+                yield SpanAttributes.LLM_INVOCATION_PARAMETERS, safe_json_dumps(request_parameters)
             except Exception:
                 logger.exception("Failed to serialize request options")
 
 
 def _get_attributes_from_chat_completion_create_param(
     params: Mapping[str, Any],
 ) -> Iterator[Tuple[str, AttributeValue]]:
@@ -70,15 +70,15 @@
     # See https://github.com/openai/openai-python/blob/f1c7d714914e3321ca2e72839fe2d132a8646e7f/src/openai/types/chat/completion_create_params.py#L28  # noqa: E501
     if not isinstance(params, Mapping):
         return
     invocation_params = dict(params)
     invocation_params.pop("messages", None)
     invocation_params.pop("functions", None)
     invocation_params.pop("tools", None)
-    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, json.dumps(invocation_params)
+    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, safe_json_dumps(invocation_params)
     if (input_messages := params.get("messages")) and isinstance(input_messages, Iterable):
         # Use reversed() to get the last message first. This is because OTEL has a default limit of
         # 128 attributes per span, and flattening increases the number of attributes very quickly.
         for index, input_message in reversed(list(enumerate(input_messages))):
             for key, value in _get_attributes_from_message_param(input_message):
                 yield f"{SpanAttributes.LLM_INPUT_MESSAGES}.{index}.{key}", value
 
@@ -97,15 +97,15 @@
         )
     if content := message.get("content"):
         if isinstance(content, str):
             yield MessageAttributes.MESSAGE_CONTENT, content
         elif isinstance(content, List):
             # See https://github.com/openai/openai-python/blob/f1c7d714914e3321ca2e72839fe2d132a8646e7f/src/openai/types/chat/chat_completion_user_message_param.py#L14  # noqa: E501
             try:
-                json_string = json.dumps(content)
+                json_string = safe_json_dumps(content)
             except Exception:
                 logger.exception("Failed to serialize message content")
             else:
                 yield MessageAttributes.MESSAGE_CONTENT, json_string
     if name := message.get("name"):
         yield MessageAttributes.MESSAGE_NAME, name
     if (function_call := message.get("function_call")) and hasattr(function_call, "get"):
@@ -147,20 +147,20 @@
 ) -> Iterator[Tuple[str, AttributeValue]]:
     # openai.types.completion_create_params.CompletionCreateParamsBase
     # See https://github.com/openai/openai-python/blob/f1c7d714914e3321ca2e72839fe2d132a8646e7f/src/openai/types/completion_create_params.py#L11  # noqa: E501
     if not isinstance(params, Mapping):
         return
     invocation_params = dict(params)
     invocation_params.pop("prompt", None)
-    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, json.dumps(invocation_params)
+    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, safe_json_dumps(invocation_params)
 
 
 def _get_attributes_from_embedding_create_param(
     params: Mapping[str, Any],
 ) -> Iterator[Tuple[str, AttributeValue]]:
     # openai.types.EmbeddingCreateParams
     # See https://github.com/openai/openai-python/blob/f1c7d714914e3321ca2e72839fe2d132a8646e7f/src/openai/types/embedding_create_params.py#L11  # noqa: E501
     if not isinstance(params, Mapping):
         return
     invocation_params = dict(params)
     invocation_params.pop("input", None)
-    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, json.dumps(invocation_params)
+    yield SpanAttributes.LLM_INVOCATION_PARAMETERS, safe_json_dumps(invocation_params)
```

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_accumulator.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_response_accumulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import warnings
 from collections import defaultdict
 from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
@@ -14,14 +13,15 @@
     Mapping,
     Optional,
     Protocol,
     Tuple,
     Type,
 )
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.instrumentation.openai._utils import (
     _as_output_attributes,
     _ValueAndType,
 )
 from openinference.semconv.trace import OpenInferenceMimeTypeValues
 from opentelemetry.util.types import AttributeValue
 
@@ -98,15 +98,15 @@
         if not self._cached_result:
             self._cached_result = dict(self._values)
         return self._cached_result
 
     def get_attributes(self) -> Iterator[Tuple[str, AttributeValue]]:
         if not (result := self._result()):
             return
-        json_string = json.dumps(result)
+        json_string = safe_json_dumps(result)
         yield from _as_output_attributes(
             _ValueAndType(json_string, OpenInferenceMimeTypeValues.JSON)
         )
 
     def get_extra_attributes(self) -> Iterator[Tuple[str, AttributeValue]]:
         if not (result := self._result()):
             return
@@ -157,15 +157,15 @@
         if not self._cached_result:
             self._cached_result = dict(self._values)
         return self._cached_result
 
     def get_attributes(self) -> Iterator[Tuple[str, AttributeValue]]:
         if not (result := self._result()):
             return
-        json_string = json.dumps(result)
+        json_string = safe_json_dumps(result)
         yield from _as_output_attributes(
             _ValueAndType(json_string, OpenInferenceMimeTypeValues.JSON)
         )
 
     def get_extra_attributes(self) -> Iterator[Tuple[str, AttributeValue]]:
         if not (result := self._result()):
             return
```

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_response_attributes_extractor.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_response_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_stream.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_stream.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_utils.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 import logging
 import warnings
 from functools import lru_cache
 from importlib.metadata import version
 from typing import (
     Any,
     Iterator,
@@ -13,14 +12,15 @@
     Protocol,
     Sequence,
     Tuple,
     Union,
     cast,
 )
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.instrumentation.openai._with_span import _WithSpan
 from openinference.semconv.trace import OpenInferenceMimeTypeValues, SpanAttributes
 from opentelemetry import trace as trace_api
 from opentelemetry.util.types import Attributes, AttributeValue
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
@@ -46,15 +46,15 @@
             assert isinstance(value, str)
         except Exception:
             logger.exception("Failed to get model dump json")
         else:
             return _ValueAndType(value, OpenInferenceMimeTypeValues.JSON)
     if not isinstance(obj, str) and isinstance(obj, (Sequence, Mapping)):
         try:
-            value = json.dumps(obj)
+            value = safe_json_dumps(obj)
         except Exception:
             logger.exception("Failed to dump json")
         else:
             return _ValueAndType(value, OpenInferenceMimeTypeValues.JSON)
     return _ValueAndType(str(obj), OpenInferenceMimeTypeValues.TEXT)
```

### Comparing `openinference_instrumentation_openai-0.1.5/src/openinference/instrumentation/openai/_with_span.py` & `openinference_instrumentation_openai-0.1.6/src/openinference/instrumentation/openai/_with_span.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/tests/openinference/instrumentation/openai/test_instrumentor.py` & `openinference_instrumentation_openai-0.1.6/tests/openinference/instrumentation/openai/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/LICENSE` & `openinference_instrumentation_openai-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/README.md` & `openinference_instrumentation_openai-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_openai-0.1.5/pyproject.toml` & `openinference_instrumentation_openai-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

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

### Comparing `openinference_instrumentation_openai-0.1.5/PKG-INFO` & `openinference_instrumentation_openai-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-openai
-Version: 0.1.5
+Version: 0.1.6
 Summary: OpenInference OpenAI Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-openai
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

