# Comparing `tmp/langwatch-0.0.8.tar.gz` & `tmp/langwatch-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langwatch-0.0.8.tar", max compression
+gzip compressed data, was "langwatch-0.0.9.tar", max compression
```

## Comparing `langwatch-0.0.8.tar` & `langwatch-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1010 2024-01-27 13:42:07.098546 langwatch-0.0.8/README.md
--rw-r--r--   0        0        0      702 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/__init__.py
--rw-r--r--   0        0        0    11193 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/langchain.py
--rw-r--r--   0        0        0    18831 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/openai.py
--rw-r--r--   0        0        0     7511 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/tracer.py
--rw-r--r--   0        0        0     3080 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/types.py
--rw-r--r--   0        0        0     2589 2024-01-27 13:42:07.098546 langwatch-0.0.8/langwatch/utils.py
--rw-r--r--   0        0        0     1555 2024-01-27 13:42:07.098546 langwatch-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 langwatch-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1010 2024-01-28 20:41:12.145103 langwatch-0.0.9/README.md
+-rw-r--r--   0        0        0      688 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/__init__.py
+-rw-r--r--   0        0        0    11193 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/langchain.py
+-rw-r--r--   0        0        0    18831 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/openai.py
+-rw-r--r--   0        0        0     7530 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/tracer.py
+-rw-r--r--   0        0        0     3080 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/types.py
+-rw-r--r--   0        0        0     2589 2024-01-28 20:41:12.145103 langwatch-0.0.9/langwatch/utils.py
+-rw-r--r--   0        0        0     1555 2024-01-28 20:41:12.145103 langwatch-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2346 1970-01-01 00:00:00.000000 langwatch-0.0.9/PKG-INFO
```

### Comparing `langwatch-0.0.8/README.md` & `langwatch-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `langwatch-0.0.8/langwatch/__init__.py` & `langwatch-0.0.9/langwatch/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import os
 from warnings import warn
 
 from langwatch.tracer import span, create_span, capture_rag
 
 endpoint = (
-    os.environ.get("LANGWATCH_ENDPOINT") or "https://app.langwatch.ai/api/collector"
+    os.environ.get("LANGWATCH_ENDPOINT") or "https://app.langwatch.ai"
 )
 api_key = os.environ.get("LANGWATCH_API_KEY")
 
 if not api_key:
     warn("LANGWATCH_API_KEY is not set, LLMs traces will not be sent, go to https://langwatch.ai to set it up")
 
 __all__ = ("endpoint", "api_key", "span", "create_span")
```

### Comparing `langwatch-0.0.8/langwatch/langchain.py` & `langwatch-0.0.9/langwatch/langchain.py`

 * *Files identical despite different names*

### Comparing `langwatch-0.0.8/langwatch/openai.py` & `langwatch-0.0.9/langwatch/openai.py`

 * *Files identical despite different names*

### Comparing `langwatch-0.0.8/langwatch/tracer.py` & `langwatch-0.0.9/langwatch/tracer.py`

 * *Files 1% similar despite different names*

```diff
@@ -255,12 +255,12 @@
 @retry(tries=5, delay=0.5, backoff=3)
 def send_spans(data: CollectorRESTParams):
     if len(data["spans"]) == 0:
         return
     if not langwatch.api_key:
         return
     response = requests.post(
-        langwatch.endpoint,
+        langwatch.endpoint + "/api/collector",
         json=data,
         headers={"X-Auth-Token": str(langwatch.api_key)},
     )
     response.raise_for_status()
```

### Comparing `langwatch-0.0.8/langwatch/types.py` & `langwatch-0.0.9/langwatch/types.py`

 * *Files identical despite different names*

### Comparing `langwatch-0.0.8/langwatch/utils.py` & `langwatch-0.0.9/langwatch/utils.py`

 * *Files identical despite different names*

### Comparing `langwatch-0.0.8/pyproject.toml` & `langwatch-0.0.9/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langwatch"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python SDK for LangWatch for monitoring your LLMs"
 authors = ["Rogerio Chaves <rogerio@langwatch.ai>"]
 homepage = "https://github.com/langwatch/langwatch"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
```

### Comparing `langwatch-0.0.8/PKG-INFO` & `langwatch-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langwatch
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python SDK for LangWatch for monitoring your LLMs
 Home-page: https://github.com/langwatch/langwatch
 License: MIT
 Author: Rogerio Chaves
 Author-email: rogerio@langwatch.ai
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

