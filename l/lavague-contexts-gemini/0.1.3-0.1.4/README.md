# Comparing `tmp/lavague_contexts_gemini-0.1.3.tar.gz` & `tmp/lavague_contexts_gemini-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_gemini-0.1.3.tar", max compression
+gzip compressed data, was "lavague_contexts_gemini-0.1.4.tar", max compression
```

## Comparing `lavague_contexts_gemini-0.1.3.tar` & `lavague_contexts_gemini-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-16 06:05:44.166686 lavague_contexts_gemini-0.1.3/README.md
--rw-r--r--   0        0        0       55 2024-05-16 21:10:23.639638 lavague_contexts_gemini-0.1.3/lavague/contexts/gemini/__init__.py
--rw-r--r--   0        0        0     1738 2024-05-16 21:10:10.906372 lavague_contexts_gemini-0.1.3/lavague/contexts/gemini/base.py
--rw-r--r--   0        0        0     1108 2024-05-16 20:09:27.326208 lavague_contexts_gemini-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-16 14:49:01.030627 lavague_contexts_gemini-0.1.4/README.md
+-rw-r--r--   0        0        0       55 2024-05-16 14:49:01.030627 lavague_contexts_gemini-0.1.4/lavague/contexts/gemini/__init__.py
+-rw-r--r--   0        0        0     1115 2024-05-21 21:06:53.305594 lavague_contexts_gemini-0.1.4/lavague/contexts/gemini/base.py
+-rw-r--r--   0        0        0     1108 2024-05-21 23:05:31.830269 lavague_contexts_gemini-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1334 1970-01-01 00:00:00.000000 lavague_contexts_gemini-0.1.4/PKG-INFO
```

### Comparing `lavague_contexts_gemini-0.1.3/pyproject.toml` & `lavague_contexts_gemini-0.1.4/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-gemini"
-version = "0.1.3"
+version = "0.1.4"
 description = "gemini integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_contexts_gemini-0.1.3/PKG-INFO` & `lavague_contexts_gemini-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-gemini
-Version: 0.1.3
+Version: 0.1.4
 Summary: gemini integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

