# Comparing `tmp/openai_responses-0.3.4.tar.gz` & `tmp/openai_responses-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openai_responses-0.3.4.tar", max compression
+gzip compressed data, was "openai_responses-0.4.0.tar", max compression
```

## Comparing `openai_responses-0.3.4.tar` & `openai_responses-0.4.0.tar`

### file list

```diff
@@ -1,45 +1,49 @@
--rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.3.4/LICENSE
--rw-r--r--   0        0        0     3016 2024-05-14 18:14:24.699878 openai_responses-0.3.4/README.md
--rw-r--r--   0        0        0     1406 2024-05-21 13:17:05.421179 openai_responses-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      310 2024-05-03 15:30:48.556901 openai_responses-0.3.4/src/openai_responses/__init__.py
--rw-r--r--   0        0        0      606 2024-05-10 15:24:55.095526 openai_responses-0.3.4/src/openai_responses/_api.py
--rw-r--r--   0        0        0     1925 2024-05-21 13:16:58.185717 openai_responses-0.3.4/src/openai_responses/_mock.py
--rw-r--r--   0        0        0     3864 2024-05-13 15:32:42.633551 openai_responses-0.3.4/src/openai_responses/_routes/__init__.py
--rw-r--r--   0        0        0     5161 2024-05-14 17:51:42.173434 openai_responses-0.3.4/src/openai_responses/_routes/_base.py
--rw-r--r--   0        0        0     6193 2024-05-21 13:16:58.185984 openai_responses-0.3.4/src/openai_responses/_routes/assistants.py
--rw-r--r--   0        0        0     1120 2024-05-21 13:16:58.186179 openai_responses-0.3.4/src/openai_responses/_routes/chat.py
--rw-r--r--   0        0        0     1382 2024-05-21 13:16:58.186384 openai_responses-0.3.4/src/openai_responses/_routes/embeddings.py
--rw-r--r--   0        0        0     4966 2024-05-21 13:16:58.186635 openai_responses-0.3.4/src/openai_responses/_routes/files.py
--rw-r--r--   0        0        0     8026 2024-05-21 13:16:58.186877 openai_responses-0.3.4/src/openai_responses/_routes/messages.py
--rw-r--r--   0        0        0     3761 2024-05-21 13:16:58.187047 openai_responses-0.3.4/src/openai_responses/_routes/run_steps.py
--rw-r--r--   0        0        0    11460 2024-05-21 13:16:58.187334 openai_responses-0.3.4/src/openai_responses/_routes/runs.py
--rw-r--r--   0        0        0     5279 2024-05-21 13:16:58.187572 openai_responses-0.3.4/src/openai_responses/_routes/threads.py
--rw-r--r--   0        0        0       62 2024-05-02 16:25:57.355893 openai_responses-0.3.4/src/openai_responses/_stores/__init__.py
--rw-r--r--   0        0        0     6151 2024-05-16 18:37:01.157176 openai_responses-0.3.4/src/openai_responses/_stores/state_store.py
--rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.3.4/src/openai_responses/_types/generics.py
--rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.3.4/src/openai_responses/_types/partials/assistants.py
--rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.3.4/src/openai_responses/_types/partials/chat.py
--rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.3.4/src/openai_responses/_types/partials/embeddings.py
--rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.3.4/src/openai_responses/_types/partials/files.py
--rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.3.4/src/openai_responses/_types/partials/messages.py
--rw-r--r--   0        0        0     2993 2024-05-20 20:53:53.219560 openai_responses-0.3.4/src/openai_responses/_types/partials/run_steps.py
--rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.3.4/src/openai_responses/_types/partials/runs.py
--rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.3.4/src/openai_responses/_types/partials/threads.py
--rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.3.4/src/openai_responses/_utils/copy.py
--rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.3.4/src/openai_responses/_utils/faker.py
--rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.3.4/src/openai_responses/_utils/serde.py
--rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.3.4/src/openai_responses/_utils/time.py
--rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.3.4/src/openai_responses/helpers/builders/_base.py
--rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.3.4/src/openai_responses/helpers/builders/assistants.py
--rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.3.4/src/openai_responses/helpers/builders/chat.py
--rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.3.4/src/openai_responses/helpers/builders/embeddings.py
--rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.3.4/src/openai_responses/helpers/builders/messages.py
--rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.3.4/src/openai_responses/helpers/builders/run_steps.py
--rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.3.4/src/openai_responses/helpers/builders/runs.py
--rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.3.4/src/openai_responses/helpers/builders/threads.py
--rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.3.4/src/openai_responses/helpers/mergers/_base.py
--rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.3.4/src/openai_responses/helpers/mergers/runs.py
--rw-r--r--   0        0        0     1271 2024-05-16 18:04:24.511337 openai_responses-0.3.4/src/openai_responses/helpers/state_store.py
--rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.3.4/src/openai_responses/plugin.py
--rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.3.4/src/openai_responses/py.typed
--rw-r--r--   0        0        0     4077 1970-01-01 00:00:00.000000 openai_responses-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1059 2024-05-16 18:41:10.309100 openai_responses-0.4.0/LICENSE
+-rw-r--r--   0        0        0     3018 2024-05-22 17:28:25.530560 openai_responses-0.4.0/README.md
+-rw-r--r--   0        0        0     1447 2024-05-21 21:02:28.184779 openai_responses-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      214 2024-05-21 20:36:49.837714 openai_responses-0.4.0/src/openai_responses/__init__.py
+-rw-r--r--   0        0        0      605 2024-05-21 20:36:49.838025 openai_responses-0.4.0/src/openai_responses/_api.py
+-rw-r--r--   0        0        0     2045 2024-05-21 20:36:49.838327 openai_responses-0.4.0/src/openai_responses/_mock.py
+-rw-r--r--   0        0        0     3863 2024-05-21 20:36:49.838619 openai_responses-0.4.0/src/openai_responses/_routes/__init__.py
+-rw-r--r--   0        0        0     5240 2024-05-22 13:56:11.130530 openai_responses-0.4.0/src/openai_responses/_routes/_base.py
+-rw-r--r--   0        0        0     6450 2024-05-21 20:36:49.839256 openai_responses-0.4.0/src/openai_responses/_routes/assistants.py
+-rw-r--r--   0        0        0     1120 2024-05-21 13:16:58.186179 openai_responses-0.4.0/src/openai_responses/_routes/chat.py
+-rw-r--r--   0        0        0     1382 2024-05-21 15:25:22.334161 openai_responses-0.4.0/src/openai_responses/_routes/embeddings.py
+-rw-r--r--   0        0        0     5008 2024-05-21 20:36:49.839510 openai_responses-0.4.0/src/openai_responses/_routes/files.py
+-rw-r--r--   0        0        0     8746 2024-05-21 20:36:49.839861 openai_responses-0.4.0/src/openai_responses/_routes/messages.py
+-rw-r--r--   0        0        0     3780 2024-05-21 20:36:49.840137 openai_responses-0.4.0/src/openai_responses/_routes/run_steps.py
+-rw-r--r--   0        0        0    11523 2024-05-21 20:36:49.840446 openai_responses-0.4.0/src/openai_responses/_routes/runs.py
+-rw-r--r--   0        0        0     5369 2024-05-21 20:36:49.840740 openai_responses-0.4.0/src/openai_responses/_routes/threads.py
+-rw-r--r--   0        0        0      233 2024-05-01 20:36:53.215071 openai_responses-0.4.0/src/openai_responses/_types/generics.py
+-rw-r--r--   0        0        0     2354 2024-05-03 17:59:52.024893 openai_responses-0.4.0/src/openai_responses/_types/partials/assistants.py
+-rw-r--r--   0        0        0     1590 2024-05-01 19:44:50.385563 openai_responses-0.4.0/src/openai_responses/_types/partials/chat.py
+-rw-r--r--   0        0        0      525 2024-05-01 21:48:18.770982 openai_responses-0.4.0/src/openai_responses/_types/partials/embeddings.py
+-rw-r--r--   0        0        0      837 2024-05-03 18:00:04.674371 openai_responses-0.4.0/src/openai_responses/_types/partials/files.py
+-rw-r--r--   0        0        0     2628 2024-05-10 14:25:16.712414 openai_responses-0.4.0/src/openai_responses/_types/partials/messages.py
+-rw-r--r--   0        0        0     2993 2024-05-20 20:53:53.219560 openai_responses-0.4.0/src/openai_responses/_types/partials/run_steps.py
+-rw-r--r--   0        0        0     3805 2024-05-10 18:42:46.808227 openai_responses-0.4.0/src/openai_responses/_types/partials/runs.py
+-rw-r--r--   0        0        0      832 2024-05-03 18:46:19.770456 openai_responses-0.4.0/src/openai_responses/_types/partials/threads.py
+-rw-r--r--   0        0        0      304 2024-05-21 20:36:49.840984 openai_responses-0.4.0/src/openai_responses/_utils/aio.py
+-rw-r--r--   0        0        0      186 2024-05-10 19:13:20.627809 openai_responses-0.4.0/src/openai_responses/_utils/copy.py
+-rw-r--r--   0        0        0      199 2024-05-01 18:05:53.366742 openai_responses-0.4.0/src/openai_responses/_utils/faker.py
+-rw-r--r--   0        0        0      627 2024-05-16 18:36:55.633057 openai_responses-0.4.0/src/openai_responses/_utils/serde.py
+-rw-r--r--   0        0        0      108 2024-05-01 18:02:02.875630 openai_responses-0.4.0/src/openai_responses/_utils/time.py
+-rw-r--r--   0        0        0       56 2024-05-21 20:36:49.841206 openai_responses-0.4.0/src/openai_responses/ext/__init__.py
+-rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841452 openai_responses-0.4.0/src/openai_responses/ext/httpx.py
+-rw-r--r--   0        0        0       34 2024-05-21 20:36:49.841757 openai_responses-0.4.0/src/openai_responses/ext/respx.py
+-rw-r--r--   0        0        0      331 2024-05-10 15:48:24.334885 openai_responses-0.4.0/src/openai_responses/helpers/builders/_base.py
+-rw-r--r--   0        0        0      489 2024-05-10 15:51:53.484991 openai_responses-0.4.0/src/openai_responses/helpers/builders/assistants.py
+-rw-r--r--   0        0        0      527 2024-05-10 15:49:32.318317 openai_responses-0.4.0/src/openai_responses/helpers/builders/chat.py
+-rw-r--r--   0        0        0      590 2024-05-10 15:50:34.652155 openai_responses-0.4.0/src/openai_responses/helpers/builders/embeddings.py
+-rw-r--r--   0        0        0     1011 2024-05-13 15:26:15.980608 openai_responses-0.4.0/src/openai_responses/helpers/builders/messages.py
+-rw-r--r--   0        0        0      563 2024-05-13 15:19:21.740278 openai_responses-0.4.0/src/openai_responses/helpers/builders/run_steps.py
+-rw-r--r--   0        0        0      543 2024-05-13 14:41:41.519321 openai_responses-0.4.0/src/openai_responses/helpers/builders/runs.py
+-rw-r--r--   0        0        0      456 2024-05-10 15:56:07.151021 openai_responses-0.4.0/src/openai_responses/helpers/builders/threads.py
+-rw-r--r--   0        0        0      317 2024-05-20 16:30:34.412882 openai_responses-0.4.0/src/openai_responses/helpers/mergers/_base.py
+-rw-r--r--   0        0        0      290 2024-05-20 16:30:34.413017 openai_responses-0.4.0/src/openai_responses/helpers/mergers/runs.py
+-rw-r--r--   0        0        0      267 2024-05-03 18:11:52.021670 openai_responses-0.4.0/src/openai_responses/plugin.py
+-rw-r--r--   0        0        0        0 2024-03-18 16:34:03.471292 openai_responses-0.4.0/src/openai_responses/py.typed
+-rw-r--r--   0        0        0       62 2024-05-21 20:36:49.841864 openai_responses-0.4.0/src/openai_responses/stores/__init__.py
+-rw-r--r--   0        0        0     6151 2024-05-21 20:36:49.841986 openai_responses-0.4.0/src/openai_responses/stores/state_store.py
+-rw-r--r--   0        0        0     4855 2024-05-22 14:04:35.946588 openai_responses-0.4.0/src/openai_responses/streaming.py
+-rw-r--r--   0        0        0     4079 1970-01-01 00:00:00.000000 openai_responses-0.4.0/PKG-INFO
```

### Comparing `openai_responses-0.3.4/LICENSE` & `openai_responses-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/README.md` & `openai_responses-0.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 - `/v1/chat/completions`
 - `/v1/embeddings`
 - `/v1/files`
 - `/v1/assistants`
 - `/v1/threads` (+ messages, runs, and steps)
 
-View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/routes).
+View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/coverage).
 
 ## Usage
 
 Just decorate any test function that makes a call to the OpenAI API (either using [openai-python](https://github.com/openai/openai-python) or with [HTTPX](https://www.python-httpx.org/)).
 
 ```python
 import openai
@@ -42,15 +42,15 @@
 
 ## Installation
 
 [![PyPI version](https://badge.fury.io/py/openai-responses.svg)](https://badge.fury.io/py/openai-responses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openai-responses.svg)](https://pypi.org/project/openai-responses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/openai-responses)](https://pypi.org/project/openai-responses/)
 
-Available on [PyPi](https://pypi.org/project/openai-responses/)
+Available on [PyPI](https://pypi.org/project/openai-responses/)
 
 ```bash
 pip install openai-responses
 ```
 
 ## Documentation
```

### Comparing `openai_responses-0.3.4/pyproject.toml` & `openai_responses-0.4.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openai-responses"
-version = "0.3.4"
+version = "0.4.0"
 description = "Automatically mock OpenAI requests"
 authors = ["Michael Harris <mharris@definite.app>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mharrisb1/openai-responses-python"
 homepage = "https://mharrisb1.github.io/openai-responses-python/"
 documentation = "https://mharrisb1.github.io/openai-responses-python/"
@@ -45,7 +45,8 @@
 venv = ".venv"
 strictListInference = true
 strictDictionaryInference = true
 strictSetInference = true
 reportMissingTypeStubs = false
 reportUnusedImport = "error"
 reportPrivateUsage = "none"
+reportWildcardImportFromLibrary = "none"
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_api.py` & `openai_responses-0.4.0/src/openai_responses/_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Any, Awaitable, Callable, Optional, Union
 
 from ._mock import OpenAIMock
-from ._stores import StateStore
+from .stores import StateStore
 
 WrappedFn = Callable[..., Union[Callable[..., Any], Awaitable[Callable[..., Any]]]]
 
 
 def mock(
     *,
     base_url: Optional[str] = None,
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_mock.py` & `openai_responses-0.4.0/src/openai_responses/_mock.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import inspect
 from functools import wraps
 from typing import Any, Callable, Optional
 
 import respx
 
 from ._routes import BetaRoutes, ChatRoutes, EmbeddingsRoutes, FileRoutes
-from ._stores import StateStore
+from .stores import StateStore
 
 
 class OpenAIMock:
     def __init__(
         self,
         base_url: Optional[str] = None,
         state: Optional[StateStore] = None,
@@ -29,14 +29,19 @@
         self._router.routes._routes.sort(key=lambda r: len(repr(r._pattern)), reverse=True)  # type: ignore
 
     @property
     def router(self) -> respx.MockRouter:
         """[RESPX](https://lundberg.github.io/respx) router with patched OpenAI routes"""
         return self._router
 
+    @property
+    def state(self) -> StateStore:
+        """State store for API resources"""
+        return self._state
+
     def _start_mock(self):
         def wrapper(fn: Callable[..., Any]):
             is_async = inspect.iscoroutinefunction(fn)
             argspec = inspect.getfullargspec(fn)
             needs_ref = "openai_mock" in argspec.args
 
             @wraps(fn)
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/__init__.py` & `openai_responses-0.4.0/src/openai_responses/_routes/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import respx
 
-from .._stores import StateStore
+from ..stores import StateStore
 
 from .chat import ChatCompletionsCreateRoute
 from .embeddings import EmbeddingsCreateRoute
 from .files import FileCreateRoute, FileListRoute, FileRetrieveRoute, FileDeleteRoute
 from .assistants import (
     AssistantCreateRoute,
     AssistantListRoute,
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/_base.py` & `openai_responses-0.4.0/src/openai_responses/_routes/_base.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from typing_extensions import override
 
 import httpx
 import respx
 
 from openai import BaseModel
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.generics import M, P
 from .._utils.serde import model_dict
 
 __all__ = ["StatelessRoute", "StatefulRoute"]
 
 
 class Route(ABC, Generic[M, P]):
@@ -26,16 +26,16 @@
         self._status_code = status_code
         self._response: Union[httpx.Response, M, P, Callable[..., httpx.Response]] = (
             self._handler
         )
         self._route.side_effect = self._response
 
     @property
-    def calls(self):
-        return self._route.calls
+    def route(self) -> respx.Route:
+        return self._route
 
     @property
     def response(self) -> Union[httpx.Response, M, P, Callable[..., httpx.Response]]:
         return self._response
 
     @response.setter
     def response(
@@ -129,15 +129,17 @@
         self._state = state
 
     @property
     @override
     def _side_effect(self) -> Callable[..., httpx.Response]:
         if callable(self._response):
             argspec = inspect.getfullargspec(self._response)
-            needs_store = "state_store" in argspec.args
+            needs_store = (
+                "state_store" in argspec.args or "state_store" in argspec.kwonlyargs
+            )
             if needs_store:
                 return partial(self._response, state_store=self._state)
             else:
                 return self._response
 
         def _handler(request: httpx.Request, route: respx.Route, **kwargs: Any):
             if isinstance(self._response, BaseModel):
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/assistants.py` & `openai_responses-0.4.0/src/openai_responses/_routes/assistants.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from openai.pagination import SyncCursorPage
 from openai.types.beta.assistant import Assistant
 from openai.types.beta.assistant_deleted import AssistantDeleted
 from openai.types.beta.assistant_update_params import AssistantUpdateParams
 
 from ._base import StatefulRoute
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.assistants import (
     PartialAssistant,
     PartialAssistantList,
     PartialAssistantDeleted,
 )
 
 from .._utils.faker import faker
@@ -101,57 +101,61 @@
     ) -> SyncCursorPage[Assistant]:
         raise NotImplementedError
 
 
 class AssistantRetrieveRoute(StatefulRoute[Assistant, PartialAssistant]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.get(url__regex=r"/assistants/(?P<id>[a-zA-Z0-9\_]+)"),
+            route=router.get(
+                url__regex=r"/assistants/(?P<assistant_id>[a-zA-Z0-9\_]+)"
+            ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        found = self._state.beta.assistants.get(id)
+        assistant_id = kwargs["assistant_id"]
+        found = self._state.beta.assistants.get(assistant_id)
         if not found:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found))
 
     @staticmethod
     def _build(partial: PartialAssistant, request: httpx.Request) -> Assistant:
         raise NotImplementedError
 
 
 class AssistantUpdateRoute(StatefulRoute[Assistant, PartialAssistant]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.post(url__regex=r"/assistants/(?P<id>[a-zA-Z0-9\_]+)"),
+            route=router.post(
+                url__regex=r"/assistants/(?P<assistant_id>[a-zA-Z0-9\_]+)"
+            ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        found = self._state.beta.assistants.get(id)
+        assistant_id = kwargs["assistant_id"]
+        found = self._state.beta.assistants.get(assistant_id)
         if not found:
             return httpx.Response(404)
 
         content: AssistantUpdateParams = json_loads(request.content)
         deserialized = model_dict(found)
         updated = model_parse(Assistant, deserialized | content)
         self._state.beta.assistants.put(updated)
@@ -162,33 +166,37 @@
     def _build(partial: PartialAssistant, request: httpx.Request) -> Assistant:
         raise NotImplementedError
 
 
 class AssistantDeleteRoute(StatefulRoute[AssistantDeleted, PartialAssistantDeleted]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.delete(url__regex=r"/assistants/(?P<id>[a-zA-Z0-9\_]+)"),
+            route=router.delete(
+                url__regex=r"/assistants/(?P<assistant_id>[a-zA-Z0-9\_]+)"
+            ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        deleted = self._state.beta.assistants.delete(id)
+        assistant_id = kwargs["assistant_id"]
+        deleted = self._state.beta.assistants.delete(assistant_id)
         return httpx.Response(
             status_code=200,
             json=model_dict(
-                AssistantDeleted(id=id, deleted=deleted, object="assistant.deleted")
+                AssistantDeleted(
+                    id=assistant_id, deleted=deleted, object="assistant.deleted"
+                )
             ),
         )
 
     @staticmethod
     def _build(
         partial: PartialAssistantDeleted,
         request: httpx.Request,
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/chat.py` & `openai_responses-0.4.0/src/openai_responses/_routes/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/embeddings.py` & `openai_responses-0.4.0/src/openai_responses/_routes/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/files.py` & `openai_responses-0.4.0/src/openai_responses/_routes/files.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 from openai.pagination import SyncPage
 from openai.types.file_object import FileObject
 from openai.types.file_deleted import FileDeleted
 
 from ._base import StatefulRoute
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.files import (
     PartialFileObject,
     PartialFileList,
     PartialFileDeleted,
 )
 
 from .._utils.faker import faker
@@ -98,29 +98,29 @@
     ) -> SyncPage[FileObject]:
         raise NotImplementedError
 
 
 class FileRetrieveRoute(StatefulRoute[FileObject, PartialFileObject]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.get(url__regex=r"/files/(?P<id>[a-zA-Z0-9\-]+)"),
+            route=router.get(url__regex=r"/files/(?P<file_id>[a-zA-Z0-9\-]+)"),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        found = self._state.files.get(id)
+        fil_id = kwargs["file_id"]
+        found = self._state.files.get(fil_id)
         if not found:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found))
 
     @staticmethod
     def _build(
@@ -129,32 +129,32 @@
     ) -> FileObject:
         raise NotImplementedError
 
 
 class FileDeleteRoute(StatefulRoute[FileObject, PartialFileDeleted]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.delete(url__regex=r"/files/(?P<id>[a-zA-Z0-9\-]+)"),
+            route=router.delete(url__regex=r"/files/(?P<file_id>[a-zA-Z0-9\-]+)"),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        deleted = self._state.files.delete(id)
+        file_id = kwargs["file_id"]
+        deleted = self._state.files.delete(file_id)
         return httpx.Response(
             status_code=200,
-            json=model_dict(FileDeleted(id=id, deleted=deleted, object="file")),
+            json=model_dict(FileDeleted(id=file_id, deleted=deleted, object="file")),
         )
 
     @staticmethod
     def _build(
         partial: PartialFileDeleted,
         request: httpx.Request,
     ) -> FileObject:
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/messages.py` & `openai_responses-0.4.0/src/openai_responses/_routes/messages.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from openai.pagination import SyncCursorPage
 from openai.types.beta.threads.message import Message
 from openai.types.beta.threads.message_deleted import MessageDeleted
 from openai.types.beta.threads.message_update_params import MessageUpdateParams
 
 from ._base import StatefulRoute
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.messages import (
     PartialMessage,
     PartialMessageList,
     PartialMessageDeleted,
 )
 
 from .._utils.faker import faker
@@ -70,21 +70,37 @@
             "content": [],
             "created_at": utcnow_unix_timestamp_s(),
             "object": "thread.message",
             "role": "user",
             "status": "completed",
         }
         if content.get("content"):
-            defaults["content"].append(
-                {
-                    "type": "text",
-                    "text": {"annotations": [], "value": content.get("content")},
-                }
-            )
+            value = content.get("content")
+            if isinstance(value, str):
+                defaults["content"].append(
+                    {
+                        "type": "text",
+                        "text": {"annotations": [], "value": value},
+                    }
+                )
+            else:
+                for block in value:
+                    if block.get("type") == "text":
+                        defaults["content"].append(
+                            {
+                                "type": "text",
+                                "text": {
+                                    "annotations": [],
+                                    "value": block.get("text"),
+                                },
+                            }
+                        )
+
             del content["content"]
+
         return model_parse(Message, defaults | partial | content)
 
 
 class MessageListRoute(StatefulRoute[SyncCursorPage[Message], PartialMessageList]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.get(
@@ -143,15 +159,15 @@
         raise NotImplementedError
 
 
 class MessageRetrieveRoute(StatefulRoute[Message, PartialMessage]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.get(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<message_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -163,31 +179,31 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_message = self._state.beta.threads.messages.get(id)
+        message_id = kwargs["message_id"]
+        found_message = self._state.beta.threads.messages.get(message_id)
         if not found_message:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found_message))
 
     @staticmethod
     def _build(partial: PartialMessage, request: httpx.Request) -> Message:
         raise NotImplementedError
 
 
 class MessageUpdateRoute(StatefulRoute[Message, PartialMessage]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.post(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<message_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -199,16 +215,16 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_message = self._state.beta.threads.messages.get(id)
+        message_id = kwargs["message_id"]
+        found_message = self._state.beta.threads.messages.get(message_id)
         if not found_message:
             return httpx.Response(404)
 
         content: MessageUpdateParams = json_loads(request.content)
         deserialized = model_dict(found_message)
         updated = model_parse(Message, deserialized | content)
         self._state.beta.threads.messages.put(updated)
@@ -220,15 +236,15 @@
         raise NotImplementedError
 
 
 class MessageDeleteRoute(StatefulRoute[MessageDeleted, PartialMessageDeleted]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.delete(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/messages/(?P<message_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -240,20 +256,22 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        deleted = self._state.beta.threads.messages.delete(id)
+        message_id = kwargs["message_id"]
+        deleted = self._state.beta.threads.messages.delete(message_id)
         return httpx.Response(
             status_code=200,
             json=model_dict(
-                MessageDeleted(id=id, deleted=deleted, object="thread.message.deleted")
+                MessageDeleted(
+                    id=message_id, deleted=deleted, object="thread.message.deleted"
+                )
             ),
         )
 
     @staticmethod
     def _build(
         partial: PartialMessageDeleted,
         request: httpx.Request,
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/run_steps.py` & `openai_responses-0.4.0/src/openai_responses/_routes/run_steps.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import respx
 
 from openai.pagination import SyncCursorPage
 from openai.types.beta.threads.runs.run_step import RunStep
 
 from ._base import StatefulRoute
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.run_steps import PartialRunStep, PartialRunStepList
 
 from .._utils.serde import model_dict
 
 
 __all__ = ["RunStepListRoute", "RunStepRetrieveRoute"]
 
@@ -81,15 +81,15 @@
         raise NotImplementedError
 
 
 class RunStepRetrieveRoute(StatefulRoute[RunStep, PartialRunStep]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.get(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)/steps/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)/steps/(?P<step_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -106,16 +106,16 @@
             return httpx.Response(404)
 
         run_id = kwargs["run_id"]
         found_run = self._state.beta.threads.runs.get(run_id)
         if not found_run:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_run_step = self._state.beta.threads.runs.steps.get(id)
+        step_id = kwargs["step_id"]
+        found_run_step = self._state.beta.threads.runs.steps.get(step_id)
         if not found_run_step:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found_run_step))
 
     @staticmethod
     def _build(partial: PartialRunStep, request: httpx.Request) -> RunStep:
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/runs.py` & `openai_responses-0.4.0/src/openai_responses/_routes/runs.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 from openai.types.beta.thread_create_and_run_params import ThreadCreateAndRunParams
 
 from ._base import StatefulRoute
 
 from ..helpers.builders.messages import message_from_create_request
 from ..helpers.builders.threads import thread_from_create_request
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.runs import PartialRun, PartialRunList
 
 from .._utils.copy import model_copy
 from .._utils.faker import faker
 from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
@@ -200,15 +200,15 @@
         raise NotImplementedError
 
 
 class RunRetrieveRoute(StatefulRoute[Run, PartialRun]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.get(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -220,31 +220,31 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_run = self._state.beta.threads.runs.get(id)
+        run_id = kwargs["run_id"]
+        found_run = self._state.beta.threads.runs.get(run_id)
         if not found_run:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found_run))
 
     @staticmethod
     def _build(partial: PartialRun, request: httpx.Request) -> Run:
         raise NotImplementedError
 
 
 class RunUpdateRoute(StatefulRoute[Run, PartialRun]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.post(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<id>[a-zA-Z0-9\_]+)"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -256,16 +256,16 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_run = self._state.beta.threads.runs.get(id)
+        run_id = kwargs["run_id"]
+        found_run = self._state.beta.threads.runs.get(run_id)
         if not found_run:
             return httpx.Response(404)
 
         content: RunUpdateParams = json_loads(request.content)
         deserialized = model_dict(found_run)
         updated = model_parse(Run, deserialized | content)
         self._state.beta.threads.runs.put(updated)
@@ -277,15 +277,15 @@
         raise NotImplementedError
 
 
 class RunSubmitToolOutputsRoute(StatefulRoute[Run, PartialRun]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.post(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<id>[a-zA-Z0-9\_]+)/submit_tool_outputs"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)/submit_tool_outputs"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -298,31 +298,31 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_run = self._state.beta.threads.runs.get(id)
+        run_id = kwargs["run_id"]
+        found_run = self._state.beta.threads.runs.get(run_id)
         if not found_run:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found_run))
 
     @staticmethod
     def _build(partial: PartialRun, request: httpx.Request) -> Run:
         raise NotImplementedError
 
 
 class RunCancelRoute(StatefulRoute[Run, PartialRun]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.post(
-                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<id>[a-zA-Z0-9\_]+)/cancel"
+                url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)/runs/(?P<run_id>[a-zA-Z0-9\_]+)/cancel"
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
@@ -335,16 +335,16 @@
         self._route = route
 
         thread_id = kwargs["thread_id"]
         found_thread = self._state.beta.threads.get(thread_id)
         if not found_thread:
             return httpx.Response(404)
 
-        id = kwargs["id"]
-        found_run = self._state.beta.threads.runs.get(id)
+        run_id = kwargs["run_id"]
+        found_run = self._state.beta.threads.runs.get(run_id)
         if not found_run:
             return httpx.Response(404)
 
         found_run.status = "cancelled"
         self._state.beta.threads.runs.put(found_run)
         copy = model_copy(found_run)
         copy.status = "cancelling"
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_routes/threads.py` & `openai_responses-0.4.0/src/openai_responses/_routes/threads.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from openai.types.beta.thread_update_params import ThreadUpdateParams
 from openai.types.beta.thread_deleted import ThreadDeleted
 
 from ._base import StatefulRoute
 
 from ..helpers.builders.messages import message_from_create_request
 
-from .._stores import StateStore
+from ..stores import StateStore
 from .._types.partials.threads import PartialThread, PartialThreadDeleted
 
 from .._utils.faker import faker
 from .._utils.serde import json_loads, model_dict, model_parse
 from .._utils.time import utcnow_unix_timestamp_s
 
 
@@ -71,59 +71,59 @@
         }
         return model_parse(Thread, defaults | partial | content)
 
 
 class ThreadRetrieveRoute(StatefulRoute[Thread, PartialThread]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.get(url__regex=r"/threads/(?P<id>[a-zA-Z0-9\_]+)"),
+            route=router.get(url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)"),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        found = self._state.beta.threads.get(id)
+        thread_id = kwargs["thread_id"]
+        found = self._state.beta.threads.get(thread_id)
         if not found:
             return httpx.Response(404)
 
         return httpx.Response(status_code=200, json=model_dict(found))
 
     @staticmethod
     def _build(partial: PartialThread, request: httpx.Request) -> Thread:
         raise NotImplementedError
 
 
 class ThreadUpdateRoute(StatefulRoute[Thread, PartialThread]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
             route=router.post(
-                url__regex=r"/threads/(?P<id>(?!.*runs)[a-zA-Z0-9_]+)"  # NOTE: avoids match on /threads/runs
+                url__regex=r"/threads/(?P<thread_id>(?!.*runs)[a-zA-Z0-9_]+)"  # NOTE: avoids match on /threads/runs
             ),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        found = self._state.beta.threads.get(id)
+        thread_id = kwargs["thread_id"]
+        found = self._state.beta.threads.get(thread_id)
         if not found:
             return httpx.Response(404)
 
         content: ThreadUpdateParams = json.loads(request.content)
         deserialized = model_dict(found)
         updated = model_parse(Thread, deserialized | content)
         self._state.beta.threads.put(updated)
@@ -134,32 +134,32 @@
     def _build(partial: PartialThread, request: httpx.Request) -> Thread:
         raise NotImplementedError
 
 
 class ThreadDeleteRoute(StatefulRoute[ThreadDeleted, PartialThreadDeleted]):
     def __init__(self, router: respx.MockRouter, state: StateStore) -> None:
         super().__init__(
-            route=router.delete(url__regex=r"/threads/(?P<id>[a-zA-Z0-9\_]+)"),
+            route=router.delete(url__regex=r"/threads/(?P<thread_id>[a-zA-Z0-9\_]+)"),
             status_code=200,
             state=state,
         )
 
     @override
     def _handler(
         self,
         request: httpx.Request,
         route: respx.Route,
         **kwargs: Any,
     ) -> httpx.Response:
         self._route = route
-        id = kwargs["id"]
-        deleted = self._state.beta.threads.delete(id)
+        thread_id = kwargs["thread_id"]
+        deleted = self._state.beta.threads.delete(thread_id)
         return httpx.Response(
             status_code=200,
             json=model_dict(
-                ThreadDeleted(id=id, deleted=deleted, object="thread.deleted")
+                ThreadDeleted(id=thread_id, deleted=deleted, object="thread.deleted")
             ),
         )
 
     @staticmethod
     def _build(partial: PartialThreadDeleted, request: httpx.Request) -> ThreadDeleted:
         raise NotImplementedError
```

### Comparing `openai_responses-0.3.4/src/openai_responses/_stores/state_store.py` & `openai_responses-0.4.0/src/openai_responses/stores/state_store.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/assistants.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/assistants.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/chat.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/embeddings.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/files.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/files.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/messages.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/run_steps.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/runs.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_types/partials/threads.py` & `openai_responses-0.4.0/src/openai_responses/_types/partials/threads.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/_utils/serde.py` & `openai_responses-0.4.0/src/openai_responses/_utils/serde.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/helpers/builders/chat.py` & `openai_responses-0.4.0/src/openai_responses/helpers/builders/chat.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/helpers/builders/embeddings.py` & `openai_responses-0.4.0/src/openai_responses/helpers/builders/embeddings.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/helpers/builders/messages.py` & `openai_responses-0.4.0/src/openai_responses/helpers/builders/messages.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/helpers/builders/run_steps.py` & `openai_responses-0.4.0/src/openai_responses/helpers/builders/run_steps.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/src/openai_responses/helpers/builders/runs.py` & `openai_responses-0.4.0/src/openai_responses/helpers/builders/runs.py`

 * *Files identical despite different names*

### Comparing `openai_responses-0.3.4/PKG-INFO` & `openai_responses-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai-responses
-Version: 0.3.4
+Version: 0.4.0
 Summary: Automatically mock OpenAI requests
 Home-page: https://mharrisb1.github.io/openai-responses-python/
 License: MIT
 Keywords: openai,pytest,testing
 Author: Michael Harris
 Author-email: mharris@definite.app
 Requires-Python: >=3.9,<4.0
@@ -33,15 +33,15 @@
 
 - `/v1/chat/completions`
 - `/v1/embeddings`
 - `/v1/files`
 - `/v1/assistants`
 - `/v1/threads` (+ messages, runs, and steps)
 
-View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/routes).
+View full support coverage [here](https://mharrisb1.github.io/openai-responses-python/coverage).
 
 ## Usage
 
 Just decorate any test function that makes a call to the OpenAI API (either using [openai-python](https://github.com/openai/openai-python) or with [HTTPX](https://www.python-httpx.org/)).
 
 ```python
 import openai
@@ -67,15 +67,15 @@
 
 ## Installation
 
 [![PyPI version](https://badge.fury.io/py/openai-responses.svg)](https://badge.fury.io/py/openai-responses)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/openai-responses.svg)](https://pypi.org/project/openai-responses/)
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/openai-responses)](https://pypi.org/project/openai-responses/)
 
-Available on [PyPi](https://pypi.org/project/openai-responses/)
+Available on [PyPI](https://pypi.org/project/openai-responses/)
 
 ```bash
 pip install openai-responses
 ```
 
 ## Documentation
```

