# Comparing `tmp/openinference_instrumentation_dspy-0.1.8.tar.gz` & `tmp/openinference_instrumentation_dspy-0.1.9.tar.gz`

## Comparing `openinference_instrumentation_dspy-0.1.8.tar` & `openinference_instrumentation_dspy-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0    24446 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/version.py
--rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/tests/openinference/instrumentation/dspy/test_instrumentor.py
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/.gitignore
--rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/LICENSE
--rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/README.md
--rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    24493 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/version.py
+-rw-r--r--   0        0        0    28449 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/tests/openinference/instrumentation/dspy/test_instrumentor.py
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/.gitignore
+-rw-r--r--   0        0        0    10840 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/LICENSE
+-rw-r--r--   0        0        0     3416 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/README.md
+-rw-r--r--   0        0        0     2003 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 openinference_instrumentation_dspy-0.1.9/PKG-INFO
```

### Comparing `openinference_instrumentation_dspy-0.1.8/src/openinference/instrumentation/dspy/__init__.py` & `openinference_instrumentation_dspy-0.1.9/src/openinference/instrumentation/dspy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     List,
     Mapping,
     Optional,
     Tuple,
 )
 
 import opentelemetry.context as context_api
-from openinference.instrumentation import get_attributes_from_context
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.instrumentation.dspy.package import _instruments
 from openinference.instrumentation.dspy.version import __version__
 from openinference.semconv.trace import (
     DocumentAttributes,
     OpenInferenceMimeTypeValues,
     OpenInferenceSpanKindValues,
     SpanAttributes,
@@ -211,15 +211,15 @@
         with self._tracer.start_as_current_span(
             span_name,
             attributes=dict(
                 _flatten(
                     {
                         OPENINFERENCE_SPAN_KIND: LLM.value,
                         LLM_MODEL_NAME: instance.kwargs.get("model"),
-                        LLM_INVOCATION_PARAMETERS: json.dumps(invocation_parameters),
+                        LLM_INVOCATION_PARAMETERS: safe_json_dumps(invocation_parameters),
                         INPUT_VALUE: str(prompt),
                         INPUT_MIME_TYPE: OpenInferenceMimeTypeValues.TEXT.value,
                     }
                 )
             ),
         ) as span:
             span.set_attributes(dict(get_attributes_from_context()))
@@ -309,15 +309,15 @@
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
                 dict(
                     _flatten(
                         {
-                            OUTPUT_VALUE: json.dumps(
+                            OUTPUT_VALUE: safe_json_dumps(
                                 self._prediction_to_output_dict(prediction, signature)
                             ),
                             OUTPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                         }
                     )
                 )
             )
@@ -379,15 +379,15 @@
                 span.set_status(trace_api.Status(trace_api.StatusCode.ERROR, str(exception)))
                 span.record_exception(exception)
                 raise
             span.set_attributes(
                 dict(
                     _flatten(
                         {
-                            OUTPUT_VALUE: json.dumps(prediction, cls=DSPyJSONEncoder),
+                            OUTPUT_VALUE: safe_json_dumps(prediction, cls=DSPyJSONEncoder),
                             OUTPUT_MIME_TYPE: OpenInferenceMimeTypeValues.JSON.value,
                         }
                     )
                 )
             )
             span.set_status(trace_api.StatusCode.OK)
         return prediction
@@ -563,15 +563,15 @@
             [None]  # the value bound to the method's self argument is discarded below, so pass None
             if signature_contains_self_parameter
             else []  # no self parameter, so no need to pass a value
         ),
         *args,
         **kwargs,
     )
-    return json.dumps(
+    return safe_json_dumps(
         {
             **{
                 argument_name: argument_value
                 for argument_name, argument_value in bound_arguments.arguments.items()
                 if argument_name not in ["self", "kwargs"]
             },
             **bound_arguments.arguments.get("kwargs", {}),
@@ -625,16 +625,16 @@
 
 
 def _jsonify_output(response: Any) -> str:
     """
     Converts output to JSON string.
     """
     if _is_google_response(response):
-        return json.dumps(_parse_google_response(response))
-    return json.dumps(response, cls=SafeJSONEncoder)
+        return safe_json_dumps(_parse_google_response(response))
+    return safe_json_dumps(response, cls=SafeJSONEncoder)
 
 
 def _is_google_response(response: Any) -> TypeGuard["GenerateContentResponseType"]:
     """
     Checks whether a candidate response is an instance of
     GenerateContentResponse returned by the Google generative AI SDK.
     """
```

### Comparing `openinference_instrumentation_dspy-0.1.8/tests/openinference/instrumentation/dspy/test_instrumentor.py` & `openinference_instrumentation_dspy-0.1.9/tests/openinference/instrumentation/dspy/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.8/LICENSE` & `openinference_instrumentation_dspy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.8/README.md` & `openinference_instrumentation_dspy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_dspy-0.1.8/pyproject.toml` & `openinference_instrumentation_dspy-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

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
   "typing-extensions",
 ]
 
 [project.optional-dependencies]
 instruments = [
```

### Comparing `openinference_instrumentation_dspy-0.1.8/PKG-INFO` & `openinference_instrumentation_dspy-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-dspy
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenInference DSPy Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-dspy
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
 Requires-Dist: typing-extensions
 Requires-Dist: wrapt
 Provides-Extra: instruments
```

