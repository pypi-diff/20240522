# Comparing `tmp/baserun-1.0.0b0.tar.gz` & `tmp/baserun-1.0.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "baserun-1.0.0b0.tar", last modified: Wed May 22 19:34:56 2024, max compression
+gzip compressed data, was "baserun-1.0.0b1.tar", last modified: Wed May 22 21:32:15 2024, max compression
```

## Comparing `baserun-1.0.0b0.tar` & `baserun-1.0.0b1.tar`

### file list

```diff
@@ -1,65 +1,27 @@
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.648162 baserun-1.0.0b0/
--rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b0/LICENSE
--rw-r--r--   0 epeterson   (501) staff       (20)     6317 2024-05-22 19:34:56.647938 baserun-1.0.0b0/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b0/README.md
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.611697 baserun-1.0.0b0/baserun/
--rw-r--r--   0 epeterson   (501) staff       (20)     1554 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     7551 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/annotation.py
--rw-r--r--   0 epeterson   (501) staff       (20)      408 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/api_key.py
--rw-r--r--   0 epeterson   (501) staff       (20)    20750 2024-05-10 18:35:59.000000 baserun-1.0.0b0/baserun/baserun.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1601 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/checks.py
--rw-r--r--   0 epeterson   (501) staff       (20)      162 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/constants.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.617721 baserun-1.0.0b0/baserun/evals/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:37.000000 baserun-1.0.0b0/baserun/evals/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    15931 2024-04-23 22:32:35.000000 baserun-1.0.0b0/baserun/evals/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)      154 2023-12-01 13:51:37.000000 baserun-1.0.0b0/baserun/evals/json.py
--rw-r--r--   0 epeterson   (501) staff       (20)      341 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/exceptions.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1241 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/exporter.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1480 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/grpc.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2215 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/helpers.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.625060 baserun-1.0.0b0/baserun/instrumentation/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/instrumentation/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    12914 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/anthropic.py
--rw-r--r--   0 epeterson   (501) staff       (20)    10699 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/google.py
--rw-r--r--   0 epeterson   (501) staff       (20)      333 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/instrumentation.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1908 2024-04-18 23:13:20.000000 baserun-1.0.0b0/baserun/instrumentation/instrumentation_manager.py
--rw-r--r--   0 epeterson   (501) staff       (20)     4063 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/instrumentation/langchain.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1971 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/instrumentation/llamaindex.py
--rw-r--r--   0 epeterson   (501) staff       (20)    19347 2024-05-07 19:10:43.000000 baserun-1.0.0b0/baserun/instrumentation/openai.py
--rw-r--r--   0 epeterson   (501) staff       (20)      278 2024-01-16 22:00:28.000000 baserun-1.0.0b0/baserun/instrumentation/span_attributes.py
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/model_configs.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2300 2024-05-21 18:35:39.000000 baserun-1.0.0b0/baserun/pytest_plugin.py
--rw-r--r--   0 epeterson   (501) staff       (20)     5812 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/sessions.py
--rw-r--r--   0 epeterson   (501) staff       (20)     9843 2024-04-30 23:03:56.000000 baserun-1.0.0b0/baserun/templates.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3177 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/templates_util.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1262 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/thread_wrapper.py
--rw-r--r--   0 epeterson   (501) staff       (20)     1159 2024-03-20 17:26:14.000000 baserun-1.0.0b0/baserun/users.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.628105 baserun-1.0.0b0/baserun/v1/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2023-12-01 13:51:58.000000 baserun-1.0.0b0/baserun/v1/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    20908 2024-02-27 18:04:42.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2.py
--rw-r--r--   0 epeterson   (501) staff       (20)    31564 2024-04-17 22:55:57.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2.pyi
--rw-r--r--   0 epeterson   (501) staff       (20)    25825 2024-02-26 22:37:29.000000 baserun-1.0.0b0/baserun/v1/baserun_pb2_grpc.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.632193 baserun-1.0.0b0/baserun/v2/
--rw-r--r--   0 epeterson   (501) staff       (20)     1379 2024-05-21 19:00:10.000000 baserun-1.0.0b0/baserun/v2/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     8311 2024-05-22 19:23:13.000000 baserun-1.0.0b0/baserun/v2/api.py
--rw-r--r--   0 epeterson   (501) staff       (20)     6656 2024-05-22 19:30:28.000000 baserun-1.0.0b0/baserun/v2/mixins.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.634858 baserun-1.0.0b0/baserun/v2/models/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/models/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)     3303 2024-05-22 16:52:14.000000 baserun-1.0.0b0/baserun/v2/models/evals.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2428 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/models/tags.py
--rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-20 19:09:07.000000 baserun-1.0.0b0/baserun/v2/utils.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.636205 baserun-1.0.0b0/baserun/v2/wrappers/
--rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-17 23:20:42.000000 baserun-1.0.0b0/baserun/v2/wrappers/__init__.py
--rw-r--r--   0 epeterson   (501) staff       (20)    16188 2024-05-22 19:03:50.000000 baserun-1.0.0b0/baserun/v2/wrappers/openai.py
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.646796 baserun-1.0.0b0/baserun.egg-info/
--rw-r--r--   0 epeterson   (501) staff       (20)     6317 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/PKG-INFO
--rw-r--r--   0 epeterson   (501) staff       (20)     1401 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/SOURCES.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/dependency_links.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/entry_points.txt
--rw-r--r--   0 epeterson   (501) staff       (20)       52 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/requires.txt
--rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-22 19:34:56.000000 baserun-1.0.0b0/baserun.egg-info/top_level.txt
--rw-r--r--   0 epeterson   (501) staff       (20)     1319 2024-05-22 19:34:45.000000 baserun-1.0.0b0/pyproject.toml
--rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-22 19:34:56.649147 baserun-1.0.0b0/setup.cfg
-drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 19:34:56.639753 baserun-1.0.0b0/tests/
--rw-r--r--   0 epeterson   (501) staff       (20)    25911 2024-05-20 18:23:17.000000 baserun-1.0.0b0/tests/testing_functions.py
--rw-r--r--   0 epeterson   (501) staff       (20)    13581 2024-05-22 19:09:40.000000 baserun-1.0.0b0/tests/testing_functions_v2.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.249307 baserun-1.0.0b1/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1073 2023-08-04 18:23:26.000000 baserun-1.0.0b1/LICENSE
+-rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-22 21:32:15.249057 baserun-1.0.0b1/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)     4569 2024-03-20 17:26:14.000000 baserun-1.0.0b1/README.md
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.235027 baserun-1.0.0b1/baserun/
+-rw-r--r--   0 epeterson   (501) staff       (20)     1381 2024-05-22 21:27:26.000000 baserun-1.0.0b1/baserun/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     8252 2024-05-22 21:26:13.000000 baserun-1.0.0b1/baserun/api.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     6754 2024-05-22 21:15:55.000000 baserun-1.0.0b1/baserun/mixins.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.243688 baserun-1.0.0b1/baserun/models/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:03:15.000000 baserun-1.0.0b1/baserun/models/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     3292 2024-05-22 21:17:36.000000 baserun-1.0.0b1/baserun/models/evals.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2390 2024-05-22 21:17:36.000000 baserun-1.0.0b1/baserun/models/tags.py
+-rw-r--r--   0 epeterson   (501) staff       (20)     2086 2024-05-22 21:03:15.000000 baserun-1.0.0b1/baserun/utils.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.245209 baserun-1.0.0b1/baserun/wrappers/
+-rw-r--r--   0 epeterson   (501) staff       (20)        0 2024-05-22 21:03:15.000000 baserun-1.0.0b1/baserun/wrappers/__init__.py
+-rw-r--r--   0 epeterson   (501) staff       (20)    16173 2024-05-22 21:16:07.000000 baserun-1.0.0b1/baserun/wrappers/openai.py
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.247813 baserun-1.0.0b1/baserun.egg-info/
+-rw-r--r--   0 epeterson   (501) staff       (20)     6223 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/PKG-INFO
+-rw-r--r--   0 epeterson   (501) staff       (20)      457 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/SOURCES.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        1 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/dependency_links.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       44 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/entry_points.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)       21 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/requires.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)        8 2024-05-22 21:32:15.000000 baserun-1.0.0b1/baserun.egg-info/top_level.txt
+-rw-r--r--   0 epeterson   (501) staff       (20)     1091 2024-05-22 21:32:06.000000 baserun-1.0.0b1/pyproject.toml
+-rw-r--r--   0 epeterson   (501) staff       (20)       81 2024-05-22 21:32:15.250080 baserun-1.0.0b1/setup.cfg
+drwxr-xr-x   0 epeterson   (501) staff       (20)        0 2024-05-22 21:32:15.246460 baserun-1.0.0b1/tests/
+-rw-r--r--   0 epeterson   (501) staff       (20)    13540 2024-05-22 21:17:36.000000 baserun-1.0.0b1/tests/testing_functions.py
```

### Comparing `baserun-1.0.0b0/LICENSE` & `baserun-1.0.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b0/PKG-INFO` & `baserun-1.0.0b1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: tools for testing, debugging, and evaluating llm features.
-Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
+Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,17 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: openai>=1.7.2
-Requires-Dist: httpx[http2]>=0.24.1
+Requires-Dist: httpx[http2]>=0.20.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-1.0.0b0/README.md` & `baserun-1.0.0b1/README.md`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b0/baserun/v2/__init__.py` & `baserun-1.0.0b1/baserun/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,37 +1,33 @@
-from typing import Any, Optional, TypeVar, Union
+from typing import Optional, TypeVar
 
-from baserun.v2.mixins import ClientMixin
+from baserun.mixins import ClientMixin
 
 T = TypeVar("T")
 
 try:
     from openai import AsyncOpenAI as BaseAsyncOpenAI
 
-    from baserun.v2.wrappers.openai import (
-        OpenAI as WrappedOpenAI,
-        AsyncOpenAI as WrappedAsyncOpenAI,
+    from baserun.wrappers.openai import AsyncOpenAI as WrappedAsyncOpenAI
+    from baserun.wrappers.openai import OpenAI as WrappedOpenAI
+    from baserun.wrappers.openai import (
+        WrappedAsyncOpenAIClient,
         WrappedOpenAIBaseClient,
         WrappedSyncOpenAIClient,
-        WrappedAsyncOpenAIClient,
     )
 
     OpenAI = WrappedOpenAI
     AsyncOpenAI = WrappedAsyncOpenAI
 
     def init(client: T, name: Optional[str] = None, api_key: Optional[str] = None, **kwargs) -> WrappedOpenAIBaseClient:
         if isinstance(client, BaseAsyncOpenAI):
             return WrappedAsyncOpenAIClient(**kwargs, name=name, api_key=api_key, client=client)
         return WrappedSyncOpenAIClient(**kwargs, name=name, api_key=api_key, client=client)
 
-except ImportError as e:
-    import pdb
-
-    pdb.set_trace()
-
+except ImportError:
     # TODO: Handle anthropic and other providers here (in case they've installed any of those alongside openai)
 
     class BaseOpenAI:
         pass
 
     class WrappedSyncOpenAIClient(ClientMixin):  # type: ignore
         pass
```

### Comparing `baserun-1.0.0b0/baserun/v2/api.py` & `baserun-1.0.0b1/baserun/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,18 +10,18 @@
 from time import sleep
 from typing import TYPE_CHECKING, Any, Dict, Optional, Union
 
 import httpx
 import tiktoken
 from openai.types.chat import ChatCompletionMessageParam
 
-from baserun.v2.utils import deep_merge
+from baserun.utils import deep_merge
 
 if TYPE_CHECKING:
-    from baserun.v2.wrappers.openai import (
+    from baserun.wrappers.openai import (
         WrappedAsyncStream,
         WrappedChatCompletion,
         WrappedOpenAIBaseClient,
         WrappedSyncStream,
     )
 
 logger = logging.getLogger(__name__)
@@ -76,15 +76,18 @@
 
 def start_worker(base_url: str, api_key: str):
     global exporter_thread
     with thread_lock:
         if exporter_thread is None:
             loop = asyncio.new_event_loop()
             asyncio.set_event_loop(loop)
-            exporter_thread = Thread(target=loop.run_until_complete, args=(worker(exporter_queue, base_url, api_key),))
+            exporter_thread = Thread(
+                target=loop.run_until_complete,
+                args=(worker(exporter_queue, base_url, api_key),),
+            )
             exporter_thread.daemon = True
             exporter_thread.start()
 
 
 class ApiClient:
     def __init__(
         self,
@@ -143,20 +146,15 @@
             "input_messages": input_messages,
             "trace": self._trace_data(),
             "start_timestamp": start_timestamp.isoformat(),
             "end_timestamp": end_timestamp.isoformat() if end_timestamp else None,
             "first_token_timestamp": first_token_timestamp.isoformat() if first_token_timestamp else None,
             "request_id": self.client.request_ids.get(completion.id),
         }
-        try:
-            logger.debug(f"Submitting completion:\n{json.dumps(output, indent=2)}")
-        except Exception as e:
-            import pdb
-
-            pdb.set_trace()
+        logger.debug(f"Submitting completion:\n{json.dumps(output, indent=2)}")
         self._post("completions", output)
 
     def submit_stream(self, stream: Union["WrappedAsyncStream", "WrappedSyncStream"]):
         if not stream.id:
             return
 
         merged_choice = deep_merge([c.model_dump() for c in stream.captured_choices])
```

### Comparing `baserun-1.0.0b0/baserun/v2/mixins.py` & `baserun-1.0.0b1/baserun/mixins.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,24 @@
+import json
 from abc import ABC
-from baserun.v2.models.evals import CompletionEval, TraceEval
-from baserun.v2.models.tags import Log, Tag, Transform, Variable
-
+from typing import Any, Dict, List, Optional, overload
 
 from openai.types.chat import ChatCompletionMessageToolCall
 
-
-import json
-from typing import Any, Dict, List, Optional, overload
+from baserun.models.evals import CompletionEval, TraceEval
+from baserun.models.tags import Log, Tag, Transform, Variable
 
 
 class CompletionMixin(ABC):
     tags: List[Tag]
     evals: List[CompletionEval]
     completion_id: str
     tool_results: List[Dict[str, Any]]
 
+    # TODO: Should this be an ABC? Or have an ABC somewhere (to define tags, evals, etc without pydantic)
     def annotate(self, key: str, value: str, metadata: Optional[Dict[str, Any]] = None):
         self.tags.append(
             Tag(
                 target_type="completion",
                 target_id=self.completion_id,
                 tag_type="annotation",
                 key=key,
```

### Comparing `baserun-1.0.0b0/baserun/v2/models/evals.py` & `baserun-1.0.0b1/baserun/models/evals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from datetime import datetime, timezone
-from typing import TYPE_CHECKING, Optional, Dict, Any, Union
+from typing import TYPE_CHECKING, Any, Dict, Optional
 from uuid import uuid4
 
 from pydantic import BaseModel, ConfigDict, Field
 
-
 if TYPE_CHECKING:
-    from baserun.v2.mixins import CompletionMixin, ClientMixin
+    from baserun.mixins import ClientMixin, CompletionMixin
 
 
 class CompletionEval(BaseModel):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     id: str = Field(default_factory=lambda: str(uuid4()))
     target: "CompletionMixin" = Field(exclude=True)
     target_type: str
```

### Comparing `baserun-1.0.0b0/baserun/v2/models/tags.py` & `baserun-1.0.0b1/baserun/models/tags.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import json
 from datetime import datetime, timezone
-from typing import Dict, Any
-from typing_extensions import Literal
+from typing import Any, Dict
 from uuid import uuid4
 
 from pydantic import BaseModel, Field
 
 
 class Tag(BaseModel):
     id: str = Field(default_factory=lambda: str(uuid4()))
```

### Comparing `baserun-1.0.0b0/baserun/v2/utils.py` & `baserun-1.0.0b1/baserun/utils.py`

 * *Files identical despite different names*

### Comparing `baserun-1.0.0b0/baserun/v2/wrappers/openai.py` & `baserun-1.0.0b1/baserun/wrappers/openai.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,19 @@
 from openai._streaming import Stream, extract_stream_chunk_type
 from openai._types import ResponseT
 from openai.resources.chat import AsyncChat, AsyncCompletions, Chat, Completions
 from openai.types.chat import ChatCompletion, ChatCompletionChunk, ChatCompletionMessageParam
 from openai.types.chat.chat_completion_chunk import Choice
 from pydantic import BaseModel, ConfigDict, Field
 
-from baserun.v2.api import ApiClient
-from baserun.v2.mixins import ClientMixin, CompletionMixin
-from baserun.v2.models.evals import CompletionEval, TraceEval
-from baserun.v2.models.tags import Tag
-from baserun.v2.utils import copy_type_hints
+from baserun.api import ApiClient
+from baserun.mixins import ClientMixin, CompletionMixin
+from baserun.models.evals import CompletionEval, TraceEval
+from baserun.models.tags import Tag
+from baserun.utils import copy_type_hints
 
 logger = logging.getLogger(__name__)
 
 
 class WrappedChatCompletion(ChatCompletion, CompletionMixin):
     model_config = ConfigDict(arbitrary_types_allowed=True)
     client: "WrappedOpenAIBaseClient"
```

### Comparing `baserun-1.0.0b0/baserun.egg-info/PKG-INFO` & `baserun-1.0.0b1/baserun.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: baserun
-Version: 1.0.0b0
+Version: 1.0.0b1
 Summary: tools for testing, debugging, and evaluating llm features.
-Author-email: Adam Ginzberg <adam@baserun.ai>, Erik Peterson <erik@baserun.ai>
+Author-email: Erik Peterson <erik@baserun.ai>
 License: MIT License
         
         Copyright (c) 2023 Mochi Labs, Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
@@ -26,17 +26,15 @@
         SOFTWARE.
         
 Project-URL: Homepage, https://baserun.ai
 Project-URL: Repository, https://github.com/baserun-ai/baserun-py
 Requires-Python: <3.12,>=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: requests>=2.31.0
-Requires-Dist: openai>=1.7.2
-Requires-Dist: httpx[http2]>=0.24.1
+Requires-Dist: httpx[http2]>=0.20.0
 
 # Baserun
 
 
 [![](https://img.shields.io/badge/Visit%20Us-baserun.ai-brightgreen)](https://baserun.ai)
 [![](https://img.shields.io/badge/View%20Documentation-Docs-yellow)](https://docs.baserun.ai)
 [![](https://img.shields.io/badge/Join%20our%20community-Discord-blue)](https://discord.gg/xEPFsvSmkb)
```

### Comparing `baserun-1.0.0b0/pyproject.toml` & `baserun-1.0.0b1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "baserun"
-version = "1.0.0b0"
+version = "1.0.0b1"
 description = "tools for testing, debugging, and evaluating llm features."
 readme = "README.md"
 license = { file = "LICENSE" }
 authors = [
-    { name = "Adam Ginzberg", email = "adam@baserun.ai" },
     { name = "Erik Peterson", email = "erik@baserun.ai" }
 ]
 requires-python = ">=3.8, <3.12"
 dependencies = [
-    "requests>=2.31.0",
-    "openai>=1.7.2",
-    "httpx[http2]>=0.24.1",
+    "httpx[http2]>=0.20.0",
 ]
 
 [project.urls]
 Homepage = "https://baserun.ai"
 Repository = "https://github.com/baserun-ai/baserun-py"
 
 [project.entry-points.pytest11]
 pbaserun = "baserun.pytest_plugin"
 
-[tool.ruff]
+[lint]
 extend-select = ["I", "T20"]  # isort, flake8-print
 target-version = "py38"
 line-length = 120
-extend-exclude = [
-    "baserun/v1/*", # autogenerated
-    "baserun/__init__.py", # it makes it look bad for multiple "as" imports in a single from statement
-]
+extend-exclude = []
+[lint.per-file-ignores]
+"baserun/v1/baserun_pb2.py" = "E501"  # Line too long
+"tests/*" = "T201"  # `print` found
 
-[tool.ruff.per-file-ignores]
-"baserun/v1/baserun_pb2.py" = ["E501"]  # Line too long
-"tests/*" = ["T201"]  # `print` found
+[tool.ruff]
+line-length = 120
 
 [tool.black]
 line-length = 120
 
 [tool.mypy]
 exclude = ["baserun/v1/*", "tests"]
 ignore_missing_imports = true
```

### Comparing `baserun-1.0.0b0/tests/testing_functions_v2.py` & `baserun-1.0.0b1/tests/testing_functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import argparse
 import asyncio
 import inspect
 import json
 import os
 import sys
-from time import sleep
 import traceback
+from time import sleep
 
 import openai
 from openai import AsyncOpenAI, NotFoundError, OpenAI
 from openai.types import CreateEmbeddingResponse
 from openai.types.chat.chat_completion_message import FunctionCall
 
-from baserun.v2 import init
+from baserun import init
 
 
 def openai_chat(prompt="What is the capital of the US?") -> str:
     client = init(OpenAI(), name="openai_chat")
     completion = client.chat.completions.create(
         name="openai_chat completion", model="gpt-4o", messages=[{"role": "user", "content": prompt}]
     )
@@ -30,15 +30,15 @@
         model="gpt-4o",
         messages=[{"role": "user", "content": prompt}],
     )
     return completion.choices[0].message.content
 
 
 def openai_chat_import(prompt="What is the capital of the US?") -> str:
-    from baserun.v2 import OpenAI
+    from baserun import OpenAI
 
     client = OpenAI()
     completion = client.chat.completions.create(model="gpt-4o", messages=[{"role": "user", "content": prompt}])
     return completion.choices[0].message.content
 
 
 def openai_chat_with_log(prompt="What is the capital of the US?") -> str:
@@ -127,15 +127,15 @@
         tools=tools,
     )
 
     return tool_calls
 
 
 def openai_chat_tools_streaming(prompt="Say 'hello world'") -> FunctionCall:
-    from baserun.v2 import OpenAI
+    from baserun import OpenAI
 
     client = OpenAI()
     tools = [
         {
             "type": "function",
             "function": {
                 "name": "say",
@@ -356,15 +356,14 @@
     return result
 
 
 # Allows you to call any of these functions, e.g. python tests/testing_functions.py openai_chat_functions_streaming
 if __name__ == "__main__":
     from dotenv import load_dotenv
 
-    from baserun import Baserun
 
     load_dotenv()
     openai.api_key = os.environ.get("OPENAI_API_KEY")
 
     parser = argparse.ArgumentParser(description="Execute a function with a prompt.")
     parser.add_argument("function_to_call", type=str, help="Name of the function to call")
     parser.add_argument("--prompt", type=str, help="Prompt to pass to the function", default=None)
```

