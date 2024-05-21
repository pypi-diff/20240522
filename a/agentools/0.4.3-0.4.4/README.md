# Comparing `tmp/agentools-0.4.3.tar.gz` & `tmp/agentools-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agentools-0.4.3.tar", max compression
+gzip compressed data, was "agentools-0.4.4.tar", max compression
```

## Comparing `agentools-0.4.3.tar` & `agentools-0.4.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0    20214 2024-05-17 15:19:29.218333 agentools-0.4.3/README.md
--rw-r--r--   0        0        0     1867 2024-05-03 06:37:11.682106 agentools-0.4.3/agentools/__init__.py
--rw-r--r--   0        0        0      590 2024-05-03 06:23:27.168756 agentools-0.4.3/agentools/api/__init__.py
--rw-r--r--   0        0        0     4224 2024-03-31 00:37:28.264533 agentools-0.4.3/agentools/api/mocking.py
--rw-r--r--   0        0        0     7658 2024-05-03 06:22:53.797079 agentools-0.4.3/agentools/api/openai.py
--rw-r--r--   0        0        0      151 2024-04-02 02:06:29.901315 agentools-0.4.3/agentools/assistants/__init__.py
--rw-r--r--   0        0        0    11730 2024-05-03 05:54:10.067310 agentools-0.4.3/agentools/assistants/chatgpt.py
--rw-r--r--   0        0        0     4328 2024-04-02 02:02:02.825310 agentools-0.4.3/agentools/assistants/core.py
--rw-r--r--   0        0        0     3595 2024-04-27 13:12:23.439238 agentools-0.4.3/agentools/assistants/structgpt.py
--rw-r--r--   0        0        0      479 2024-03-31 00:37:46.713979 agentools-0.4.3/agentools/assistants/utils.py
--rw-r--r--   0        0        0      107 2024-05-03 06:24:56.023734 agentools-0.4.3/agentools/messages/__init__.py
--rw-r--r--   0        0        0     3631 2024-03-31 00:37:53.927940 agentools-0.4.3/agentools/messages/core.py
--rw-r--r--   0        0        0      309 2024-05-03 06:29:28.435564 agentools-0.4.3/agentools/retrieval/__init__.py
--rw-r--r--   0        0        0      327 2024-05-01 18:11:26.493421 agentools-0.4.3/agentools/retrieval/db/__init__.py
--rw-r--r--   0        0        0     5659 2024-04-27 00:41:29.844323 agentools-0.4.3/agentools/retrieval/db/collection.py
--rw-r--r--   0        0        0     3163 2024-04-27 00:41:29.846068 agentools-0.4.3/agentools/retrieval/db/data.py
--rw-r--r--   0        0        0     1188 2024-04-27 00:41:29.850286 agentools-0.4.3/agentools/retrieval/db/embedding.py
--rw-r--r--   0        0        0      496 2024-04-02 04:27:33.809212 agentools-0.4.3/agentools/tools/__init__.py
--rw-r--r--   0        0        0     6001 2024-04-02 06:57:54.540986 agentools-0.4.3/agentools/tools/core.py
--rw-r--r--   0        0        0     1354 2024-03-31 01:24:18.875057 agentools-0.4.3/agentools/tools/decorators/fail_with_message.py
--rw-r--r--   0        0        0     5194 2024-04-02 04:07:23.757891 agentools-0.4.3/agentools/tools/decorators/function_tool.py
--rw-r--r--   0        0        0     3770 2024-04-02 07:01:15.990059 agentools-0.4.3/agentools/tools/decorators/streaming_function_tool.py
--rw-r--r--   0        0        0     4903 2024-03-31 01:11:04.598758 agentools-0.4.3/agentools/tools/decorators/utils.py
--rw-r--r--   0        0        0      144 2024-03-31 00:38:13.569875 agentools-0.4.3/agentools/utils/tokens.py
--rw-r--r--   0        0        0     2339 2024-03-31 00:38:15.875070 agentools-0.4.3/agentools/utils/trackers.py
--rw-r--r--   0        0        0      554 2024-05-17 15:20:55.636851 agentools-0.4.3/pyproject.toml
--rw-r--r--   0        0        0    20966 1970-01-01 00:00:00.000000 agentools-0.4.3/PKG-INFO
+-rw-r--r--   0        0        0    20214 2024-05-17 15:19:29.218333 agentools-0.4.4/README.md
+-rw-r--r--   0        0        0     1867 2024-05-03 06:37:11.682106 agentools-0.4.4/agentools/__init__.py
+-rw-r--r--   0        0        0      590 2024-05-03 06:23:27.168756 agentools-0.4.4/agentools/api/__init__.py
+-rw-r--r--   0        0        0     4224 2024-03-31 00:37:28.264533 agentools-0.4.4/agentools/api/mocking.py
+-rw-r--r--   0        0        0     7658 2024-05-03 06:22:53.797079 agentools-0.4.4/agentools/api/openai.py
+-rw-r--r--   0        0        0      151 2024-04-02 02:06:29.901315 agentools-0.4.4/agentools/assistants/__init__.py
+-rw-r--r--   0        0        0    11730 2024-05-03 05:54:10.067310 agentools-0.4.4/agentools/assistants/chatgpt.py
+-rw-r--r--   0        0        0     4328 2024-04-02 02:02:02.825310 agentools-0.4.4/agentools/assistants/core.py
+-rw-r--r--   0        0        0     3595 2024-04-27 13:12:23.439238 agentools-0.4.4/agentools/assistants/structgpt.py
+-rw-r--r--   0        0        0      479 2024-03-31 00:37:46.713979 agentools-0.4.4/agentools/assistants/utils.py
+-rw-r--r--   0        0        0      107 2024-05-03 06:24:56.023734 agentools-0.4.4/agentools/messages/__init__.py
+-rw-r--r--   0        0        0     3650 2024-05-21 18:28:32.899293 agentools-0.4.4/agentools/messages/core.py
+-rw-r--r--   0        0        0      309 2024-05-03 06:29:28.435564 agentools-0.4.4/agentools/retrieval/__init__.py
+-rw-r--r--   0        0        0      327 2024-05-01 18:11:26.493421 agentools-0.4.4/agentools/retrieval/db/__init__.py
+-rw-r--r--   0        0        0     5659 2024-04-27 00:41:29.844323 agentools-0.4.4/agentools/retrieval/db/collection.py
+-rw-r--r--   0        0        0     3163 2024-04-27 00:41:29.846068 agentools-0.4.4/agentools/retrieval/db/data.py
+-rw-r--r--   0        0        0     1188 2024-04-27 00:41:29.850286 agentools-0.4.4/agentools/retrieval/db/embedding.py
+-rw-r--r--   0        0        0      496 2024-04-02 04:27:33.809212 agentools-0.4.4/agentools/tools/__init__.py
+-rw-r--r--   0        0        0     6001 2024-04-02 06:57:54.540986 agentools-0.4.4/agentools/tools/core.py
+-rw-r--r--   0        0        0     1354 2024-03-31 01:24:18.875057 agentools-0.4.4/agentools/tools/decorators/fail_with_message.py
+-rw-r--r--   0        0        0     5194 2024-04-02 04:07:23.757891 agentools-0.4.4/agentools/tools/decorators/function_tool.py
+-rw-r--r--   0        0        0     3770 2024-04-02 07:01:15.990059 agentools-0.4.4/agentools/tools/decorators/streaming_function_tool.py
+-rw-r--r--   0        0        0     4903 2024-03-31 01:11:04.598758 agentools-0.4.4/agentools/tools/decorators/utils.py
+-rw-r--r--   0        0        0      144 2024-03-31 00:38:13.569875 agentools-0.4.4/agentools/utils/tokens.py
+-rw-r--r--   0        0        0     2339 2024-03-31 00:38:15.875070 agentools-0.4.4/agentools/utils/trackers.py
+-rw-r--r--   0        0        0      554 2024-05-21 18:29:45.177225 agentools-0.4.4/pyproject.toml
+-rw-r--r--   0        0        0    20966 1970-01-01 00:00:00.000000 agentools-0.4.4/PKG-INFO
```

### Comparing `agentools-0.4.3/README.md` & `agentools-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/__init__.py` & `agentools-0.4.4/agentools/__init__.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/api/__init__.py` & `agentools-0.4.4/agentools/api/__init__.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/api/mocking.py` & `agentools-0.4.4/agentools/api/mocking.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/api/openai.py` & `agentools-0.4.4/agentools/api/openai.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/assistants/chatgpt.py` & `agentools-0.4.4/agentools/assistants/chatgpt.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/assistants/core.py` & `agentools-0.4.4/agentools/assistants/core.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/assistants/structgpt.py` & `agentools-0.4.4/agentools/assistants/structgpt.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/messages/core.py` & `agentools-0.4.4/agentools/messages/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from typing import overload
 from abc import ABC, abstractmethod
 from copy import deepcopy
 
+from pydantic import BaseModel
 from openai.types.chat import ChatCompletionMessage
 
 
 @overload
 def msg(*, system: str) -> dict[str, str]: ...
 
 
@@ -55,15 +56,15 @@
     async def reset(self):
         """Reset the history"""
         ...
 
     @staticmethod
     def ensure_dict(message: dict | ChatCompletionMessage):
         """Convert assistant pydantic message to dict"""
-        if isinstance(message, ChatCompletionMessage):
+        if isinstance(message, BaseModel):
             message = message.model_dump()
             # remove any None values (tool calls)
             message = {k: v for k, v in message.items() if v is not None}
         return message
 
 
 class SimpleHistory(MessageHistory):
```

### Comparing `agentools-0.4.3/agentools/retrieval/db/collection.py` & `agentools-0.4.4/agentools/retrieval/db/collection.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/retrieval/db/data.py` & `agentools-0.4.4/agentools/retrieval/db/data.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/retrieval/db/embedding.py` & `agentools-0.4.4/agentools/retrieval/db/embedding.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/tools/core.py` & `agentools-0.4.4/agentools/tools/core.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/tools/decorators/fail_with_message.py` & `agentools-0.4.4/agentools/tools/decorators/fail_with_message.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/tools/decorators/function_tool.py` & `agentools-0.4.4/agentools/tools/decorators/function_tool.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/tools/decorators/streaming_function_tool.py` & `agentools-0.4.4/agentools/tools/decorators/streaming_function_tool.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/tools/decorators/utils.py` & `agentools-0.4.4/agentools/tools/decorators/utils.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/agentools/utils/trackers.py` & `agentools-0.4.4/agentools/utils/trackers.py`

 * *Files identical despite different names*

### Comparing `agentools-0.4.3/pyproject.toml` & `agentools-0.4.4/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "agentools"
-version = "0.4.3"
+version = "0.4.4"
 description = ""
 authors = ["Joong-Won Seo <joong.won.seo@gmail.com>"]
 readme = "README.md"
 packages = [{include = "agentools"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `agentools-0.4.3/PKG-INFO` & `agentools-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: agentools
-Version: 0.4.3
+Version: 0.4.4
 Summary: 
 Author: Joong-Won Seo
 Author-email: joong.won.seo@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

