# Comparing `tmp/arize_phoenix_evals-0.9.1.tar.gz` & `tmp/arize_phoenix_evals-0.9.2.tar.gz`

## Comparing `arize_phoenix_evals-0.9.1.tar` & `arize_phoenix_evals-0.9.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/__init__.py
--rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/classify.py
--rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/default_templates.py
--rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/evaluators.py
--rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/exceptions.py
--rw-r--r--   0        0        0    13403 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/executors.py
--rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/generate.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/py.typed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/retrievals.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/templates.py
--rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/utils.py
--rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/__init__.py
--rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/anthropic.py
--rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/base.py
--rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/bedrock.py
--rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/litellm.py
--rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/mistralai.py
--rw-r--r--   0        0        0    15585 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/openai.py
--rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/rate_limiters.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertex.py
--rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertexai.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/.gitignore
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/IP_NOTICE
--rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/LICENSE
--rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/README.md
--rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/pyproject.toml
--rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     2600 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/__init__.py
+-rw-r--r--   0        0        0    12446 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/classify.py
+-rw-r--r--   0        0        0    30282 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/default_templates.py
+-rw-r--r--   0        0        0    15651 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/evaluators.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/exceptions.py
+-rw-r--r--   0        0        0    14504 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/executors.py
+-rw-r--r--   0        0        0     5552 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/generate.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/py.typed
+-rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/retrievals.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/templates.py
+-rw-r--r--   0        0        0     5702 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/utils.py
+-rw-r--r--   0        0        0      483 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/__init__.py
+-rw-r--r--   0        0        0     5613 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/anthropic.py
+-rw-r--r--   0        0        0     3269 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/base.py
+-rw-r--r--   0        0        0     6856 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/bedrock.py
+-rw-r--r--   0        0        0     3517 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/litellm.py
+-rw-r--r--   0        0        0     5012 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/mistralai.py
+-rw-r--r--   0        0        0    15585 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/openai.py
+-rw-r--r--   0        0        0    10155 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/rate_limiters.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/vertex.py
+-rw-r--r--   0        0        0     5607 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/src/phoenix/evals/models/vertexai.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/.gitignore
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/IP_NOTICE
+-rw-r--r--   0        0        0     3794 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/LICENSE
+-rw-r--r--   0        0        0     2455 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/README.md
+-rw-r--r--   0        0        0     2425 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0     4381 2020-02-02 00:00:00.000000 arize_phoenix_evals-0.9.2/PKG-INFO
```

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/__init__.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/__init__.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/classify.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/classify.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/default_templates.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/default_templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/evaluators.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/evaluators.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/executors.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/executors.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,27 @@
 from __future__ import annotations
 
 import asyncio
 import logging
 import signal
+import threading
 import traceback
-from typing import Any, Callable, Coroutine, List, Optional, Protocol, Sequence, Tuple, Union
+from contextlib import contextmanager
+from typing import (
+    Any,
+    Callable,
+    Coroutine,
+    Generator,
+    List,
+    Optional,
+    Protocol,
+    Sequence,
+    Tuple,
+    Union,
+)
 
 from phoenix.evals.exceptions import PhoenixException
 from tqdm.auto import tqdm
 
 logger = logging.getLogger(__name__)
 
 
@@ -164,15 +177,15 @@
     async def execute(self, inputs: Sequence[Any]) -> List[Any]:
         termination_event = asyncio.Event()
 
         def termination_handler(signum: int, frame: Any) -> None:
             termination_event.set()
             tqdm.write("Process was interrupted. The return value will be incomplete...")
 
-        signal.signal(self.termination_signal, termination_handler)
+        original_handler = signal.signal(self.termination_signal, termination_handler)
         outputs = [self.fallback_return_value] * len(inputs)
         progress_bar = tqdm(total=len(inputs), bar_format=self.tqdm_bar_format)
 
         max_queue_size = 5 * self.concurrency  # limit the queue to bound memory usage
         max_fill = max_queue_size - (2 * self.concurrency)  # ensure there is always room to requeue
         queue: asyncio.PriorityQueue[Tuple[int, Any]] = asyncio.PriorityQueue(
             maxsize=max_queue_size
@@ -205,15 +218,15 @@
                 if not task.done():
                     task.cancel()
 
         if not termination_event_watcher.done():
             termination_event_watcher.cancel()
 
         # reset the SIGTERM handler
-        signal.signal(self.termination_signal, signal.SIG_DFL)  # reset the SIGTERM handler
+        signal.signal(self.termination_signal, original_handler)  # reset the SIGTERM handler
         return outputs
 
     def run(self, inputs: Sequence[Any]) -> List[Any]:
         return asyncio.run(self.execute(inputs))
 
 
 class SyncExecutor(Executor):
@@ -240,71 +253,97 @@
     def __init__(
         self,
         generation_fn: Callable[[Any], Any],
         tqdm_bar_format: Optional[str] = None,
         max_retries: int = 10,
         exit_on_error: bool = True,
         fallback_return_value: Union[Unset, Any] = _unset,
-        termination_signal: signal.Signals = signal.SIGINT,
+        termination_signal: Optional[signal.Signals] = signal.SIGINT,
     ):
         self.generate = generation_fn
         self.fallback_return_value = fallback_return_value
         self.tqdm_bar_format = tqdm_bar_format
         self.max_retries = max_retries
         self.exit_on_error = exit_on_error
         self.termination_signal = termination_signal
 
         self._TERMINATE = False
 
     def _signal_handler(self, signum: int, frame: Any) -> None:
         tqdm.write("Process was interrupted. The return value will be incomplete...")
         self._TERMINATE = True
 
+    @contextmanager
+    def _executor_signal_handling(self, signum: Optional[int]) -> Generator[None, None, None]:
+        original_handler = None
+        if signum is not None:
+            original_handler = signal.signal(signum, self._signal_handler)
+            try:
+                yield
+            finally:
+                signal.signal(signum, original_handler)
+        else:
+            yield
+
     def run(self, inputs: Sequence[Any]) -> List[Any]:
-        signal.signal(self.termination_signal, self._signal_handler)
-        outputs = [self.fallback_return_value] * len(inputs)
-        progress_bar = tqdm(total=len(inputs), bar_format=self.tqdm_bar_format)
+        with self._executor_signal_handling(self.termination_signal):
+            outputs = [self.fallback_return_value] * len(inputs)
+            progress_bar = tqdm(total=len(inputs), bar_format=self.tqdm_bar_format)
 
-        for index, input in enumerate(inputs):
-            try:
-                for attempt in range(self.max_retries + 1):
-                    if self._TERMINATE:
+            for index, input in enumerate(inputs):
+                try:
+                    for attempt in range(self.max_retries + 1):
+                        if self._TERMINATE:
+                            return outputs
+                        try:
+                            result = self.generate(input)
+                            outputs[index] = result
+                            progress_bar.update()
+                            break
+                        except Exception as exc:
+                            is_phoenix_exception = isinstance(exc, PhoenixException)
+                            if attempt >= self.max_retries or is_phoenix_exception:
+                                raise exc
+                            else:
+                                tqdm.write(f"Exception in worker on attempt {attempt + 1}: {exc}")
+                                tqdm.write("Retrying...")
+                except Exception as exc:
+                    tqdm.write(f"Exception in worker: {exc}")
+                    if self.exit_on_error:
                         return outputs
-                    try:
-                        result = self.generate(input)
-                        outputs[index] = result
+                    else:
                         progress_bar.update()
-                        break
-                    except Exception as exc:
-                        is_phoenix_exception = isinstance(exc, PhoenixException)
-                        if attempt >= self.max_retries or is_phoenix_exception:
-                            raise exc
-                        else:
-                            tqdm.write(f"Exception in worker on attempt {attempt + 1}: {exc}")
-                            tqdm.write("Retrying...")
-            except Exception as exc:
-                tqdm.write(f"Exception in worker: {exc}")
-                if self.exit_on_error:
-                    return outputs
-                else:
-                    progress_bar.update()
-        signal.signal(self.termination_signal, signal.SIG_DFL)  # reset the SIGTERM handler
         return outputs
 
 
 def get_executor_on_sync_context(
     sync_fn: Callable[[Any], Any],
     async_fn: Callable[[Any], Coroutine[Any, Any, Any]],
     run_sync: bool = False,
     concurrency: int = 3,
     tqdm_bar_format: Optional[str] = None,
     exit_on_error: bool = True,
     fallback_return_value: Union[Unset, Any] = _unset,
 ) -> Executor:
-    if run_sync:
+    if threading.current_thread() is not threading.main_thread():
+        # run evals synchronously if not in the main thread
+
+        if run_sync is False:
+            logger.warning(
+                "Async evals execution is not supported in non-main threads. Falling back to sync."
+            )
+        return SyncExecutor(
+            sync_fn,
+            tqdm_bar_format=tqdm_bar_format,
+            exit_on_error=exit_on_error,
+            fallback_return_value=fallback_return_value,
+            termination_signal=None,
+        )
+
+    if run_sync is True:
         return SyncExecutor(
             sync_fn,
             tqdm_bar_format=tqdm_bar_format,
             exit_on_error=exit_on_error,
             fallback_return_value=fallback_return_value,
         )
```

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/generate.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/generate.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/retrievals.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/retrievals.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/templates.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/templates.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/utils.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/utils.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/anthropic.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/anthropic.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/base.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/base.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/bedrock.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/bedrock.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/litellm.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/litellm.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/mistralai.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/mistralai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/openai.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/openai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/rate_limiters.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/rate_limiters.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertex.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/vertex.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/src/phoenix/evals/models/vertexai.py` & `arize_phoenix_evals-0.9.2/src/phoenix/evals/models/vertexai.py`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/LICENSE` & `arize_phoenix_evals-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/README.md` & `arize_phoenix_evals-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `arize_phoenix_evals-0.9.1/pyproject.toml` & `arize_phoenix_evals-0.9.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
   "Programming Language :: Python",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: 3.12",
 ]
-version = "0.9.1"
+version = "0.9.2"
 dependencies = [
   "pandas",
   "tqdm",
   "typing-extensions>=4.5, <5",
 ]
 
 [project.optional-dependencies]
```

### Comparing `arize_phoenix_evals-0.9.1/PKG-INFO` & `arize_phoenix_evals-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: arize-phoenix-evals
-Version: 0.9.1
+Version: 0.9.2
 Summary: LLM Evaluations
 Project-URL: Documentation, https://docs.arize.com/phoenix/
 Project-URL: Issues, https://github.com/Arize-ai/phoenix/issues
 Project-URL: Source, https://github.com/Arize-ai/phoenix
 Author-email: Arize AI <phoenix-devs@arize.com>
 License: Elastic-2.0
 License-File: IP_NOTICE
```

