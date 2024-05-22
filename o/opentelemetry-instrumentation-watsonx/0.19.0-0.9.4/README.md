# Comparing `tmp/opentelemetry_instrumentation_watsonx-0.19.0.tar.gz` & `tmp/opentelemetry_instrumentation_watsonx-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrumentation_watsonx-0.19.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrumentation_watsonx-0.9.4.tar", max compression
```

## Comparing `opentelemetry_instrumentation_watsonx-0.19.0.tar` & `opentelemetry_instrumentation_watsonx-0.9.4.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     1495 2024-05-22 14:59:30.715421 opentelemetry_instrumentation_watsonx-0.19.0/README.md
--rw-r--r--   0        0        0    17928 2024-05-22 14:59:30.715421 opentelemetry_instrumentation_watsonx-0.19.0/opentelemetry/instrumentation/watsonx/__init__.py
--rw-r--r--   0        0        0       42 2024-05-22 14:59:30.715421 opentelemetry_instrumentation_watsonx-0.19.0/opentelemetry/instrumentation/watsonx/config.py
--rw-r--r--   0        0        0      701 2024-05-22 14:59:30.715421 opentelemetry_instrumentation_watsonx-0.19.0/opentelemetry/instrumentation/watsonx/utils.py
--rw-r--r--   0        0        0       23 2024-05-22 14:59:30.715421 opentelemetry_instrumentation_watsonx-0.19.0/opentelemetry/instrumentation/watsonx/version.py
--rw-r--r--   0        0        0     1259 2024-05-22 14:59:56.103365 opentelemetry_instrumentation_watsonx-0.19.0/pyproject.toml
--rw-r--r--   0        0        0     2581 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_watsonx-0.19.0/PKG-INFO
+-rw-r--r--   0        0        0      880 2024-01-22 09:18:14.865253 opentelemetry_instrumentation_watsonx-0.9.4/README.md
+-rw-r--r--   0        0        0     6485 2024-01-22 09:18:14.865487 opentelemetry_instrumentation_watsonx-0.9.4/opentelemetry/instrumentation/watsonx/__init__.py
+-rw-r--r--   0        0        0       22 2024-01-22 09:18:34.075879 opentelemetry_instrumentation_watsonx-0.9.4/opentelemetry/instrumentation/watsonx/version.py
+-rw-r--r--   0        0        0      669 2024-01-22 09:18:34.076307 opentelemetry_instrumentation_watsonx-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 opentelemetry_instrumentation_watsonx-0.9.4/PKG-INFO
```

### Comparing `opentelemetry_instrumentation_watsonx-0.19.0/README.md` & `opentelemetry_instrumentation_watsonx-0.9.4/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,43 +1,21 @@
 # OpenTelemetry IBM Watsonx Instrumentation
 
-This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/) and [IBM watsonx.ai library](https://ibm.github.io/watsonx-ai-python-sdk/).
+This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/).
 
 ## Installation
 
 ```bash
 pip install opentelemetry-instrumentation-watsonx
 ```
 
-## Example usage
-
-```python
-from opentelemetry.instrumentation.watsonx import WatsonxInstrumentor
-
-WatsonxInstrumentor().instrument()
-```
-
 ## Privacy
 
 **By default, this instrumentation logs prompts, completions, and embeddings to span attributes**. This gives you a clear visibility into how your LLM application is working, and can make it easy to debug and evaluate the quality of the outputs.
 
 However, you may want to disable this logging for privacy reasons, as they may contain highly sensitive data from your users. You may also simply want to reduce the size of your traces.
 
 To disable logging, set the `TRACELOOP_TRACE_CONTENT` environment variable to `false`.
 
 ```bash
 TRACELOOP_TRACE_CONTENT=false
 ```
-
-## SSL Issue
-
-In case of SSL handshake issues (or similar ones) as follows:
-
-```
-E0423 17:04:25.197068000 6150713344 ssl_transport_security.cc:1420]    Handshake failed with fatal error SSL_ERROR_SSL: error:100000f7:SSL routines:OPENSSL_internal:WRONG_VERSION_NUMBER.
-```
-
-You can instruct the exporter with an environment variable to ignore SSL errors:
-
-```bash
-OTEL_EXPORTER_OTLP_INSECURE=true
-```
```

### Comparing `opentelemetry_instrumentation_watsonx-0.19.0/pyproject.toml` & `opentelemetry_instrumentation_watsonx-0.9.4/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,26 @@
 [tool.poetry]
 name = "opentelemetry-instrumentation-watsonx"
-version = "0.19.0"
+version = "0.9.4"
 description = "OpenTelemetry IBM Watsonx Instrumentation"
 authors = ["Guangya Liu <gyliu@ibm.com>"]
-repository = "https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-watsonx"
 license = "Apache-2.0"
 readme = "README.md"
 
 [[tool.poetry.packages]]
 include = "opentelemetry/instrumentation/watsonx"
 
 [tool.poetry.dependencies]
-python = ">=3.9,<4"
-opentelemetry-api = "^1.24.0"
-opentelemetry-instrumentation = "^0.45b0"
-opentelemetry-semantic-conventions = "^0.45b0"
-opentelemetry-semantic-conventions-ai = "0.2.0"
+python = ">=3.8.1,<4"
+opentelemetry-api = "^1.22.0"
+opentelemetry-instrumentation = "0.43b0"
+opentelemetry-semantic-conventions-ai = "^0.0.15"
 
 [tool.poetry.group.dev.dependencies]
-autopep8 = "2.1.0"
+autopep8 = "2.0.4"
 flake8 = "7.0.0"
-pytest = "8.1.1"
-pytest-sugar = "1.0.0"
-
-[tool.poetry.group.test.dependencies]
-pytest = "8.1.1"
-pytest-sugar = "1.0.0"
-vcrpy = "^6.0.1"
-pytest-recording = "^0.13.1"
-opentelemetry-sdk = "^1.23.0"
-pytest-asyncio = "^0.23.5"
-ibm-watson-machine-learning = "1.0.333"
+pytest = "7.4.4"
+pytest-sugar = "0.9.7"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
-
-[tool.poetry.extras]
-instruments = ["ibm-watson-machine-learning"]
-
-[tool.poetry.plugins."opentelemetry_instrumentor"]
-ibm-watson-machine-learning = "opentelemetry.instrumentation.watsonx:WatsonxInstrumentor"
```

### Comparing `opentelemetry_instrumentation_watsonx-0.19.0/PKG-INFO` & `opentelemetry_instrumentation_watsonx-0.9.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,67 +1,41 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrumentation-watsonx
-Version: 0.19.0
+Version: 0.9.4
 Summary: OpenTelemetry IBM Watsonx Instrumentation
-Home-page: https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-watsonx
 License: Apache-2.0
 Author: Guangya Liu
 Author-email: gyliu@ibm.com
-Requires-Python: >=3.9,<4
+Requires-Python: >=3.8.1,<4
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: instruments
-Requires-Dist: opentelemetry-api (>=1.24.0,<2.0.0)
-Requires-Dist: opentelemetry-instrumentation (>=0.45b0,<0.46)
-Requires-Dist: opentelemetry-semantic-conventions (>=0.45b0,<0.46)
-Requires-Dist: opentelemetry-semantic-conventions-ai (==0.2.0)
-Project-URL: Repository, https://github.com/traceloop/openllmetry/tree/main/packages/opentelemetry-instrumentation-watsonx
+Requires-Dist: opentelemetry-api (>=1.22.0,<2.0.0)
+Requires-Dist: opentelemetry-instrumentation (==0.43b0)
+Requires-Dist: opentelemetry-semantic-conventions-ai (>=0.0.15,<0.0.16)
 Description-Content-Type: text/markdown
 
 # OpenTelemetry IBM Watsonx Instrumentation
 
-This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/) and [IBM watsonx.ai library](https://ibm.github.io/watsonx-ai-python-sdk/).
+This library allows tracing IBM Watsonx prompts and completions sent with the official [IBM Watson Machine Learning library](https://ibm.github.io/watson-machine-learning-sdk/).
 
 ## Installation
 
 ```bash
 pip install opentelemetry-instrumentation-watsonx
 ```
 
-## Example usage
-
-```python
-from opentelemetry.instrumentation.watsonx import WatsonxInstrumentor
-
-WatsonxInstrumentor().instrument()
-```
-
 ## Privacy
 
 **By default, this instrumentation logs prompts, completions, and embeddings to span attributes**. This gives you a clear visibility into how your LLM application is working, and can make it easy to debug and evaluate the quality of the outputs.
 
 However, you may want to disable this logging for privacy reasons, as they may contain highly sensitive data from your users. You may also simply want to reduce the size of your traces.
 
 To disable logging, set the `TRACELOOP_TRACE_CONTENT` environment variable to `false`.
 
 ```bash
 TRACELOOP_TRACE_CONTENT=false
 ```
 
-## SSL Issue
-
-In case of SSL handshake issues (or similar ones) as follows:
-
-```
-E0423 17:04:25.197068000 6150713344 ssl_transport_security.cc:1420]    Handshake failed with fatal error SSL_ERROR_SSL: error:100000f7:SSL routines:OPENSSL_internal:WRONG_VERSION_NUMBER.
-```
-
-You can instruct the exporter with an environment variable to ignore SSL errors:
-
-```bash
-OTEL_EXPORTER_OTLP_INSECURE=true
-```
-
```

