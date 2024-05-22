# Comparing `tmp/galileo_observe-1.1.0.tar.gz` & `tmp/galileo_observe-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galileo_observe-1.1.0.tar", max compression
+gzip compressed data, was "galileo_observe-1.1.1.tar", max compression
```

## Comparing `galileo_observe-1.1.0.tar` & `galileo_observe-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0    11357 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/LICENSE
--rw-r--r--   0        0        0      221 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/README.md
--rw-r--r--   0        0        0      372 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/__init__.py
--rw-r--r--   0        0        0    15663 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/async_handlers.py
--rw-r--r--   0        0        0        0 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/constants/__init__.py
--rw-r--r--   0        0        0      889 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/constants/routes.py
--rw-r--r--   0        0        0    17098 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/handlers.py
--rw-r--r--   0        0        0     7681 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/monitor.py
--rw-r--r--   0        0        0        0 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/schema/__init__.py
--rw-r--r--   0        0        0     1376 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/schema/transaction.py
--rw-r--r--   0        0        0       22 2024-05-16 17:54:34.549450 galileo_observe-1.1.0/galileo_observe/utils/__init__.py
--rw-r--r--   0        0        0     6746 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/utils/api_client.py
--rw-r--r--   0        0        0     2255 2024-05-16 17:54:33.557447 galileo_observe-1.1.0/galileo_observe/utils/request.py
--rw-r--r--   0        0        0     2554 2024-05-16 17:54:34.549450 galileo_observe-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1240 1970-01-01 00:00:00.000000 galileo_observe-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/LICENSE
+-rw-r--r--   0        0        0      221 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/README.md
+-rw-r--r--   0        0        0      372 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/__init__.py
+-rw-r--r--   0        0        0    15648 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/async_handlers.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/constants/__init__.py
+-rw-r--r--   0        0        0      889 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/constants/routes.py
+-rw-r--r--   0        0        0    17098 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/handlers.py
+-rw-r--r--   0        0        0     7681 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/monitor.py
+-rw-r--r--   0        0        0        0 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/schema/__init__.py
+-rw-r--r--   0        0        0     1376 2024-05-22 17:06:47.727115 galileo_observe-1.1.1/galileo_observe/schema/transaction.py
+-rw-r--r--   0        0        0       22 2024-05-22 17:06:48.583114 galileo_observe-1.1.1/galileo_observe/utils/__init__.py
+-rw-r--r--   0        0        0     6746 2024-05-22 17:06:47.731115 galileo_observe-1.1.1/galileo_observe/utils/api_client.py
+-rw-r--r--   0        0        0     2255 2024-05-22 17:06:47.731115 galileo_observe-1.1.1/galileo_observe/utils/request.py
+-rw-r--r--   0        0        0     2578 2024-05-22 17:06:48.583114 galileo_observe-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 galileo_observe-1.1.1/PKG-INFO
```

### Comparing `galileo_observe-1.1.0/LICENSE` & `galileo_observe-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/async_handlers.py` & `galileo_observe-1.1.1/galileo_observe/async_handlers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import asyncio
 import time
 from datetime import datetime
 from http import HTTPStatus
 from json import dumps
 from typing import Any, Dict, List, Optional, Sequence, Union
 from uuid import UUID
 
 import pytz
 import tiktoken
+from galileo_core.helpers.execution import async_run
 from langchain.callbacks.base import AsyncCallbackHandler
 from langchain.prompts.chat import ChatPromptValue
 from langchain.schema.agent import AgentAction, AgentFinish
 from langchain.schema.messages import BaseMessage
 from langchain.schema.messages import _message_to_dict as message_to_dict
 from langchain.schema.output import LLMResult
 from langchain_core.documents import Document
@@ -87,16 +87,15 @@
                     batch_records.append(v)
                     del self.records[k]
 
             transaction_batch = TransactionRecordBatch(
                 records=batch_records,
                 logging_method=TransactionLoggingMethod.py_langchain_async,
             )
-            loop = asyncio.get_running_loop()
-            loop.create_task(self.client.ingest_batch(transaction_batch))
+            async_run(self.client.ingest_batch(transaction_batch))
 
     async def on_llm_start(
         self,
         serialized: Dict[str, Any],
         prompts: List[str],
         run_id: UUID,
         parent_run_id: Optional[UUID] = None,
```

### Comparing `galileo_observe-1.1.0/galileo_observe/constants/routes.py` & `galileo_observe-1.1.1/galileo_observe/constants/routes.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/handlers.py` & `galileo_observe-1.1.1/galileo_observe/handlers.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/monitor.py` & `galileo_observe-1.1.1/galileo_observe/monitor.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/schema/transaction.py` & `galileo_observe-1.1.1/galileo_observe/schema/transaction.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/utils/api_client.py` & `galileo_observe-1.1.1/galileo_observe/utils/api_client.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/galileo_observe/utils/request.py` & `galileo_observe-1.1.1/galileo_observe/utils/request.py`

 * *Files identical despite different names*

### Comparing `galileo_observe-1.1.0/pyproject.toml` & `galileo_observe-1.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "galileo-observe"
-version = "1.1.0"
+version = "1.1.1"
 description = "📈 Monitor your LLM integration with Galileo Observe!"
 authors = ["Galileo Technologies Inc. <team@rungalileo.io>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.13"
 requests = "^2.31.0"
@@ -14,14 +14,15 @@
 pyjwt = "^2.8.0"
 cryptography = "^42.0.0"
 backoff = "^2.2.1"
 types-pytz = "^2023.3.1.1"
 tiktoken = "^0.5.2"
 langchain = ">=0.1,<0.2"
 httpx = "^0.27.0"
+galileo-core = "^1.0.0"
 
 [tool.poetry.extras]
 langchain = ["langchain"]
 
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.1"
```

### Comparing `galileo_observe-1.1.0/PKG-INFO` & `galileo_observe-1.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: galileo-observe
-Version: 1.1.0
+Version: 1.1.1
 Summary: 📈 Monitor your LLM integration with Galileo Observe!
 Author: Galileo Technologies Inc.
 Author-email: team@rungalileo.io
 Requires-Python: >=3.9,<3.13
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: langchain
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cryptography (>=42.0.0,<43.0.0)
+Requires-Dist: galileo-core (>=1.0.0,<2.0.0)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: langchain (>=0.1,<0.2) ; extra == "langchain"
 Requires-Dist: pydantic (>=2.5.2,<3.0.0)
 Requires-Dist: pyjwt (>=2.8.0,<3.0.0)
 Requires-Dist: pytz (>=2023.3,<2024.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: tiktoken (>=0.5.2,<0.6.0)
```

