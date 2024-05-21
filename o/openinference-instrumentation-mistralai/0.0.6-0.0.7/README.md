# Comparing `tmp/openinference_instrumentation_mistralai-0.0.6.tar.gz` & `tmp/openinference_instrumentation_mistralai-0.0.7.tar.gz`

## Comparing `openinference_instrumentation_mistralai-0.0.6.tar` & `openinference_instrumentation_mistralai-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/__init__.py
--rw-r--r--   0        0        0    15245 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_chat_wrapper.py
--rw-r--r--   0        0        0     4164 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py
--rw-r--r--   0        0        0     6761 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_accumulator.py
--rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py
--rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_stream.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_utils.py
--rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_with_span.py
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/version.py
--rw-r--r--   0        0        0    78196 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/tests/openinference/instrumentation/mistralai/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/LICENSE
--rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/README.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0     3160 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/__init__.py
+-rw-r--r--   0        0        0    15267 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_chat_wrapper.py
+-rw-r--r--   0        0        0     4220 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py
+-rw-r--r--   0        0        0     6812 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_response_accumulator.py
+-rw-r--r--   0        0        0     3954 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py
+-rw-r--r--   0        0        0     5308 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_stream.py
+-rw-r--r--   0        0        0     2733 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_utils.py
+-rw-r--r--   0        0        0     2553 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_with_span.py
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/version.py
+-rw-r--r--   0        0        0    78196 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/tests/openinference/instrumentation/mistralai/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/LICENSE
+-rw-r--r--   0        0        0     2932 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/README.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 openinference_instrumentation_mistralai-0.0.7/PKG-INFO
```

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/__init__.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/__init__.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_chat_wrapper.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_chat_wrapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     Dict,
     Iterable,
     Iterator,
     Mapping,
     Tuple,
 )
 
-from openinference.instrumentation import get_attributes_from_context
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.instrumentation.mistralai._request_attributes_extractor import (
     _RequestAttributesExtractor,
 )
 from openinference.instrumentation.mistralai._response_accumulator import _ChatCompletionAccumulator
 from openinference.instrumentation.mistralai._response_attributes_extractor import (
     _ResponseAttributesExtractor,
 )
@@ -152,15 +152,15 @@
                 elif key == "tool_choice":
                     request_data[key] = mistral_client._parse_tool_choice(value)
                 elif key == "response_format" and value is not None:
                     request_data[key] = mistral_client._parse_response_format(value)
                 elif value is not None:
                     try:
                         # ensure the value is JSON-serializable
-                        json.dumps(value)
+                        safe_json_dumps(value)
                         request_data[key] = value
                     except json.JSONDecodeError:
                         request_data[key] = str(value)
             except Exception:
                 request_data[key] = str(value)
         return request_data
```

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_request_attributes_extractor.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import json
 import logging
 from enum import Enum
 from types import ModuleType
 from typing import (
     Any,
     Iterable,
     Iterator,
     List,
     Mapping,
     Tuple,
 )
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.semconv.trace import MessageAttributes, SpanAttributes, ToolCallAttributes
 from opentelemetry.util.types import AttributeValue
 
 __all__ = ("_RequestAttributesExtractor",)
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
@@ -45,15 +45,15 @@
 ) -> Iterator[Tuple[str, AttributeValue]]:
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
 
@@ -69,15 +69,15 @@
             role.value if isinstance(role, Enum) else role,
         )
     if content := message.get("content"):
         if isinstance(content, str):
             yield MessageAttributes.MESSAGE_CONTENT, content
         elif isinstance(content, List):
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
```

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_accumulator.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_response_accumulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-import json
 from collections import defaultdict
 from copy import deepcopy
 from typing import (
     TYPE_CHECKING,
     Any,
     Callable,
     DefaultDict,
@@ -13,14 +12,15 @@
     Mapping,
     Optional,
     Protocol,
     Tuple,
     Type,
 )
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.instrumentation.mistralai._utils import (
     _as_output_attributes,
     _ValueAndType,
 )
 from openinference.semconv.trace import OpenInferenceMimeTypeValues
 from opentelemetry.util.types import AttributeValue
 
@@ -89,15 +89,15 @@
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

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_response_attributes_extractor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_stream.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_stream.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_utils.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-import json
 import logging
 from typing import Any, Iterator, NamedTuple, Optional, Protocol, Tuple
 
+from openinference.instrumentation import safe_json_dumps
 from openinference.instrumentation.mistralai._with_span import _WithSpan
 from openinference.semconv.trace import OpenInferenceMimeTypeValues, SpanAttributes
 from opentelemetry import trace as trace_api
 from opentelemetry.util.types import Attributes, AttributeValue
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
@@ -45,15 +45,15 @@
         )
     except Exception:
         logger.exception("Failed to finish tracing")
 
 
 def _io_value_and_type(obj: Any) -> _ValueAndType:
     try:
-        return _ValueAndType(json.dumps(obj), OpenInferenceMimeTypeValues.JSON)
+        return _ValueAndType(safe_json_dumps(obj), OpenInferenceMimeTypeValues.JSON)
     except Exception:
         logger.exception("Failed to get input attributes from request parameters.")
     return _ValueAndType(str(obj), OpenInferenceMimeTypeValues.TEXT)
 
 
 def _as_input_attributes(
     value_and_type: Optional[_ValueAndType],
```

### Comparing `openinference_instrumentation_mistralai-0.0.6/src/openinference/instrumentation/mistralai/_with_span.py` & `openinference_instrumentation_mistralai-0.0.7/src/openinference/instrumentation/mistralai/_with_span.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/tests/openinference/instrumentation/mistralai/test_instrumentor.py` & `openinference_instrumentation_mistralai-0.0.7/tests/openinference/instrumentation/mistralai/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/LICENSE` & `openinference_instrumentation_mistralai-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/README.md` & `openinference_instrumentation_mistralai-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_mistralai-0.0.6/pyproject.toml` & `openinference_instrumentation_mistralai-0.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -23,15 +23,15 @@
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
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "mistralai",
```

### Comparing `openinference_instrumentation_mistralai-0.0.6/PKG-INFO` & `openinference_instrumentation_mistralai-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-mistralai
-Version: 0.0.6
+Version: 0.0.7
 Summary: OpenInference Mistral AI Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-mistralai
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: <3.13,>=3.9
-Requires-Dist: openinference-instrumentation>=0.1.5
+Requires-Dist: openinference-instrumentation>=0.1.7
 Requires-Dist: openinference-semantic-conventions
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
 Requires-Dist: wrapt
 Provides-Extra: instruments
 Requires-Dist: mistralai; extra == 'instruments'
```

