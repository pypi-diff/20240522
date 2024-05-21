# Comparing `tmp/openinference_instrumentation_langchain-0.1.8.tar.gz` & `tmp/openinference_instrumentation_langchain-0.1.9.tar.gz`

## Comparing `openinference_instrumentation_langchain-0.1.8.tar` & `openinference_instrumentation_langchain-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/__init__.py
--rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/_tracer.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/package.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/py.typed
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/version.py
--rw-r--r--   0        0        0    15665 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/tests/openinference/instrumentation/langchain/test_instrumentor.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/.gitignore
--rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/LICENSE
--rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/README.rst
--rw-r--r--   0        0        0     1919 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2419 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/__init__.py
+-rw-r--r--   0        0        0    23814 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/_tracer.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/package.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/py.typed
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/version.py
+-rw-r--r--   0        0        0    15665 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/tests/openinference/instrumentation/langchain/test_instrumentor.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/.gitignore
+-rw-r--r--   0        0        0    10870 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/LICENSE
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/README.rst
+-rw-r--r--   0        0        0     1930 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 openinference_instrumentation_langchain-0.1.9/PKG-INFO
```

### Comparing `openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/__init__.py` & `openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import logging
-from typing import TYPE_CHECKING, Any, Callable, Collection
+from typing import TYPE_CHECKING, Any, Callable, Collection, Type
 
-from openinference.instrumentation.langchain._tracer import OpenInferenceTracer
 from openinference.instrumentation.langchain.package import _instruments
 from openinference.instrumentation.langchain.version import __version__
 from opentelemetry import trace as trace_api
 from opentelemetry.instrumentation.instrumentor import BaseInstrumentor  # type: ignore
 from wrapt import wrap_function_wrapper
 
 if TYPE_CHECKING:
     from langchain_core.callbacks import BaseCallbackManager
+    from openinference.instrumentation.langchain._tracer import OpenInferenceTracer
 
 logger = logging.getLogger(__name__)
 logger.addHandler(logging.NullHandler())
 
 
 class LangChainInstrumentor(BaseInstrumentor):  # type: ignore
     """
@@ -23,39 +23,42 @@
     def instrumentation_dependencies(self) -> Collection[str]:
         return _instruments
 
     def _instrument(self, **kwargs: Any) -> None:
         if not (tracer_provider := kwargs.get("tracer_provider")):
             tracer_provider = trace_api.get_tracer_provider()
         tracer = trace_api.get_tracer(__name__, __version__, tracer_provider)
+        from openinference.instrumentation.langchain._tracer import OpenInferenceTracer
+
         wrap_function_wrapper(
             module="langchain_core.callbacks",
             name="BaseCallbackManager.__init__",
-            wrapper=_BaseCallbackManagerInit(tracer=tracer),
+            wrapper=_BaseCallbackManagerInit(tracer=tracer, cls=OpenInferenceTracer),
         )
 
     def _uninstrument(self, **kwargs: Any) -> None:
         pass
 
 
 class _BaseCallbackManagerInit:
-    __slots__ = ("_tracer",)
+    __slots__ = ("_tracer", "_cls")
 
-    def __init__(self, tracer: trace_api.Tracer):
+    def __init__(self, tracer: trace_api.Tracer, cls: Type["OpenInferenceTracer"]):
         self._tracer = tracer
+        self._cls = cls
 
     def __call__(
         self,
         wrapped: Callable[..., None],
         instance: "BaseCallbackManager",
         args: Any,
         kwargs: Any,
     ) -> None:
         wrapped(*args, **kwargs)
         for handler in instance.inheritable_handlers:
             # Handlers may be copied when new managers are created, so we
             # don't want to keep adding. E.g. see the following location.
             # https://github.com/langchain-ai/langchain/blob/5c2538b9f7fb64afed2a918b621d9d8681c7ae32/libs/core/langchain_core/callbacks/manager.py#L1876  # noqa: E501
-            if isinstance(handler, OpenInferenceTracer):
+            if isinstance(handler, self._cls):
                 break
         else:
-            instance.add_handler(OpenInferenceTracer(tracer=self._tracer), True)
+            instance.add_handler(self._cls(tracer=self._tracer), True)
```

### Comparing `openinference_instrumentation_langchain-0.1.8/src/openinference/instrumentation/langchain/_tracer.py` & `openinference_instrumentation_langchain-0.1.9/src/openinference/instrumentation/langchain/_tracer.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_langchain-0.1.8/tests/openinference/instrumentation/langchain/test_instrumentor.py` & `openinference_instrumentation_langchain-0.1.9/tests/openinference/instrumentation/langchain/test_instrumentor.py`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_langchain-0.1.8/LICENSE` & `openinference_instrumentation_langchain-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openinference_instrumentation_langchain-0.1.8/pyproject.toml` & `openinference_instrumentation_langchain-0.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
   "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
   "opentelemetry-api",
   "opentelemetry-instrumentation",
   "opentelemetry-semantic-conventions",
   "openinference-semantic-conventions>=0.1.3",
+  "wrapt",
 ]
 
 [project.optional-dependencies]
 instruments = [
   "langchain_core >= 0.1.0",
 ]
 test = [
```

### Comparing `openinference_instrumentation_langchain-0.1.8/PKG-INFO` & `openinference_instrumentation_langchain-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openinference-instrumentation-langchain
-Version: 0.1.8
+Version: 0.1.9
 Summary: OpenInference LangChain Instrumentation
 Project-URL: Homepage, https://github.com/Arize-ai/openinference/tree/main/python/instrumentation/openinference-instrumentation-langchain
 Author-email: OpenInference Authors <oss@arize.com>
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
@@ -16,14 +16,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <3.12,>=3.8
 Requires-Dist: openinference-semantic-conventions>=0.1.3
 Requires-Dist: opentelemetry-api
 Requires-Dist: opentelemetry-instrumentation
 Requires-Dist: opentelemetry-semantic-conventions
+Requires-Dist: wrapt
 Provides-Extra: instruments
 Requires-Dist: langchain-core>=0.1.0; extra == 'instruments'
 Provides-Extra: test
 Requires-Dist: langchain-community==0.0.10; extra == 'test'
 Requires-Dist: langchain-core==0.1.8; extra == 'test'
 Requires-Dist: langchain-openai==0.0.2; extra == 'test'
 Requires-Dist: langchain==0.1.0; extra == 'test'
```

