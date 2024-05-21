# Comparing `tmp/openinference_instrumentation_bedrock-0.1.5.tar.gz` & `tmp/openinference_instrumentation_bedrock-0.1.6.tar.gz`

## Comparing `openinference_instrumentation_bedrock-0.1.5.tar` & `openinference_instrumentation_bedrock-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     8052 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/__init__.py
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/version.py
--rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/tests/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/LICENSE
--rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/README.md
--rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0     8074 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/src/openinference/instrumentation/bedrock/__init__.py
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/src/openinference/instrumentation/bedrock/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/src/openinference/instrumentation/bedrock/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/src/openinference/instrumentation/bedrock/version.py
+-rw-r--r--   0        0        0    11168 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/tests/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2855 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/README.md
+-rw-r--r--   0        0        0     2024 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     4321 2020-02-02 00:00:00.000000 openinference_instrumentation_bedrock-0.1.6/PKG-INFO
```

### Comparing `openinference_instrumentation_bedrock-0.1.5/src/openinference/instrumentation/bedrock/__init__.py` & `openinference_instrumentation_bedrock-0.1.6/src/openinference/instrumentation/bedrock/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from functools import wraps
 from importlib import import_module
 from inspect import signature
 from typing import IO, Any, Callable, Collection, Dict, Optional, Tuple, TypeVar, cast
 
 from botocore.client import BaseClient
 from botocore.response import StreamingBody
-from openinference.instrumentation import get_attributes_from_context
+from openinference.instrumentation import get_attributes_from_context, safe_json_dumps
 from openinference.instrumentation.bedrock.package import _instruments
 from openinference.instrumentation.bedrock.version import __version__
 from openinference.semconv.trace import (
     OpenInferenceSpanKindValues,
     SpanAttributes,
 )
 from opentelemetry import context as context_api
@@ -101,15 +101,15 @@
                 )
                 if raw_request_body := kwargs.get("body"):
                     request_body = json.loads(raw_request_body)
                 response_body = json.loads(response.get("body").read())
                 response["body"].reset()
 
                 prompt = request_body.pop("prompt")
-                invocation_parameters = json.dumps(request_body)
+                invocation_parameters = safe_json_dumps(request_body)
 
                 _set_span_attribute(span, SpanAttributes.INPUT_VALUE, prompt)
                 _set_span_attribute(
                     span, SpanAttributes.LLM_INVOCATION_PARAMETERS, invocation_parameters
                 )
 
                 if metadata := response.get("ResponseMetadata"):
```

### Comparing `openinference_instrumentation_bedrock-0.1.5/tests/test_instrumentor.py` & `openinference_instrumentation_bedrock-0.1.6/tests/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.5/LICENSE` & `openinference_instrumentation_bedrock-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.5/README.md` & `openinference_instrumentation_bedrock-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_bedrock-0.1.5/pyproject.toml` & `openinference_instrumentation_bedrock-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

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
   "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "boto3 >= 11.28.57",
```

### Comparing `openinference_instrumentation_bedrock-0.1.5/PKG-INFO` & `openinference_instrumentation_bedrock-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: openinference-instrumentation-bedrock
-Version: 0.1.5
+Version: 0.1.6
 Summary: OpenInference Bedrock Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-bedrock
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
 Requires-Dist: wrapt
 Provides-Extra: instruments
 Requires-Dist: boto3>=11.28.57; extra == 'instruments'
```

