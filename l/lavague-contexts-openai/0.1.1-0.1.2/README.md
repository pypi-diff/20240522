# Comparing `tmp/lavague_contexts_openai-0.1.1.tar.gz` & `tmp/lavague_contexts_openai-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_contexts_openai-0.1.1.tar", max compression
+gzip compressed data, was "lavague_contexts_openai-0.1.2.tar", max compression
```

## Comparing `lavague_contexts_openai-0.1.1.tar` & `lavague_contexts_openai-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       32 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/README.md
--rw-r--r--   0        0        0       75 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/lavague/contexts/openai/__init__.py
--rw-r--r--   0        0        0     3021 2024-05-15 19:17:05.222186 lavague_contexts_openai-0.1.1/lavague/contexts/openai/base.py
--rw-r--r--   0        0        0     1171 2024-05-15 21:18:44.468045 lavague_contexts_openai-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0       32 2024-05-15 22:13:36.166566 lavague_contexts_openai-0.1.2/README.md
+-rw-r--r--   0        0        0       75 2024-05-15 22:13:36.166566 lavague_contexts_openai-0.1.2/lavague/contexts/openai/__init__.py
+-rw-r--r--   0        0        0     2193 2024-05-21 21:06:53.305594 lavague_contexts_openai-0.1.2/lavague/contexts/openai/base.py
+-rw-r--r--   0        0        0     1171 2024-05-21 23:05:42.411752 lavague_contexts_openai-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1418 1970-01-01 00:00:00.000000 lavague_contexts_openai-0.1.2/PKG-INFO
```

### Comparing `lavague_contexts_openai-0.1.1/lavague/contexts/openai/base.py` & `lavague_contexts_openai-0.1.2/lavague/contexts/openai/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,70 +1,51 @@
 from typing import Optional
 from llama_index.llms.openai import OpenAI
 from llama_index.llms.azure_openai import AzureOpenAI
 from llama_index.core.base.embeddings.base import BaseEmbedding
 from llama_index.embeddings.openai import OpenAIEmbedding
 from llama_index.multi_modal_llms.openai import OpenAIMultiModal
 from llama_index.multi_modal_llms.azure_openai import AzureOpenAIMultiModal
-from llama_index.core import PromptTemplate
 import os
-from lavague.core import (
-    OpsmSplitRetriever,
-    DefaultPromptTemplate,
-    PythonFromMarkdownExtractor,
-    Context,
-    get_default_context,
-)
-from lavague.core.extractors import BaseExtractor
-from lavague.core.retrievers import BaseHtmlRetriever
-from lavague.core.context import DEFAULT_MAX_TOKENS, DEFAULT_TEMPERATURE
+from lavague.core.context import Context, DEFAULT_MAX_TOKENS, DEFAULT_TEMPERATURE
 
 
 class OpenaiContext(Context):
     def __init__(
         self,
         api_key: Optional[str] = None,
         llm: str = "gpt-3.5-turbo",
         mm_llm: str = "gpt-4o",
         embedding: str = "text-embedding-3-large",
-        retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
-        prompt_template: PromptTemplate = DefaultPromptTemplate(),
-        extractor: BaseExtractor = PythonFromMarkdownExtractor(),
     ) -> Context:
         if api_key is None:
             api_key = os.getenv("OPENAI_API_KEY")
             if api_key is None:
                 raise ValueError("OPENAI_API_KEY is not set")
         return super().__init__(
             OpenAI(
                 api_key=api_key,
                 model=llm,
                 max_tokens=DEFAULT_MAX_TOKENS,
                 temperature=DEFAULT_TEMPERATURE,
             ),
             OpenAIMultiModal(api_key=api_key, model=mm_llm),
             OpenAIEmbedding(api_key=api_key, model=embedding),
-            retriever,
-            prompt_template,
-            extractor,
         )
 
 
 class AzureOpenaiContext(Context):
     def __init__(
         self,
         api_key: Optional[str] = None,
         endpoint: Optional[str] = None,
         deployment: Optional[str] = None,
         llm: Optional[str] = None,
         mm_llm: Optional[str] = None,
         embedding: BaseEmbedding = OpenAIEmbedding(model="text-embedding-3-large"),
-        retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
-        prompt_template: PromptTemplate = DefaultPromptTemplate(),
-        extractor: BaseExtractor = PythonFromMarkdownExtractor(),
     ):
         if api_key is None:
             api_key = os.getenv("AZURE_OPENAI_KEY")
         if endpoint is None:
             endpoint = os.getenv("AZURE_OPENAI_ENDPOINT")
         if deployment is None:
             deployment = os.getenv("AZURE_OPENAI_DEPLOYMENT")
@@ -72,11 +53,8 @@
             AzureOpenAI(
                 model=llm, api_key=api_key, endpoint=endpoint, deployment=deployment
             ),
             AzureOpenAIMultiModal(
                 model=mm_llm, api_key=api_key, endpoint=endpoint, deployment=deployment
             ),
             embedding,
-            retriever,
-            prompt_template,
-            extractor,
         )
```

### Comparing `lavague_contexts_openai-0.1.1/pyproject.toml` & `lavague_contexts_openai-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lavague-contexts-openai"
-version = "0.1.1"
+version = "0.1.2"
 description = "Openai integration for lavague"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_contexts_openai-0.1.1/PKG-INFO` & `lavague_contexts_openai-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-contexts-openai
-Version: 0.1.1
+Version: 0.1.2
 Summary: Openai integration for lavague
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

