# Comparing `tmp/lavague_core-0.1.4.tar.gz` & `tmp/lavague_core-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.4.tar", max compression
+gzip compressed data, was "lavague_core-0.1.5.tar", max compression
```

## Comparing `lavague_core-0.1.4.tar` & `lavague_core-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-16 06:03:22.535020 lavague_core-0.1.4/LICENSE
--rw-r--r--   0        0        0        0 2024-05-16 06:03:22.535047 lavague_core-0.1.4/README.md
--rw-r--r--   0        0        0      956 2024-05-16 06:03:22.535306 lavague_core-0.1.4/lavague/core/__init__.py
--rw-r--r--   0        0        0     4084 2024-05-16 06:03:22.535479 lavague_core-0.1.4/lavague/core/action_engine.py
--rw-r--r--   0        0        0     5873 2024-05-19 20:23:23.623772 lavague_core-0.1.4/lavague/core/agents.py
--rw-r--r--   0        0        0     2778 2024-05-16 06:03:22.535653 lavague_core-0.1.4/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1896 2024-05-16 06:03:22.535742 lavague_core-0.1.4/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-16 06:03:22.535814 lavague_core-0.1.4/lavague/core/extractors.py
--rw-r--r--   0        0        0      613 2024-05-16 06:03:22.535883 lavague_core-0.1.4/lavague/core/prompt_templates.py
--rw-r--r--   0        0        0    12117 2024-05-16 06:03:22.536134 lavague_core-0.1.4/lavague/core/retrievers.py
--rw-r--r--   0        0        0     3793 2024-05-16 06:03:22.536249 lavague_core-0.1.4/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3709 2024-05-21 06:02:21.563242 lavague_core-0.1.4/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-16 06:03:22.536457 lavague_core-0.1.4/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0      491 2024-05-16 06:03:22.536523 lavague_core-0.1.4/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     3445 2024-05-16 06:03:22.536696 lavague_core-0.1.4/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-21 06:18:35.433464 lavague_core-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-15 22:13:36.162566 lavague_core-0.1.5/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-15 22:13:36.162566 lavague_core-0.1.5/README.md
+-rw-r--r--   0        0        0      903 2024-05-21 21:17:01.343089 lavague_core-0.1.5/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5603 2024-05-21 21:06:53.301594 lavague_core-0.1.5/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-21 21:06:53.301594 lavague_core-0.1.5/lavague/core/action_template.py
+-rw-r--r--   0        0        0     9339 2024-05-21 22:50:43.800201 lavague_core-0.1.5/lavague/core/agents.py
+-rw-r--r--   0        0        0     2771 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1189 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1070 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/navigation.py
+-rw-r--r--   0        0        0     4153 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5238 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3710 2024-05-21 21:06:53.269595 lavague_core-0.1.5/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3074 2024-05-21 22:50:43.796201 lavague_core-0.1.5/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     9878 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1080 2024-05-21 23:06:09.391404 lavague_core-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.5/PKG-INFO
```

### Comparing `lavague_core-0.1.4/LICENSE` & `lavague_core-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.4/lavague/core/__init__.py` & `lavague_core-0.1.5/lavague/core/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from lavague.core.action_engine import ActionEngine
+from lavague.core.python_engine import PythonEngine
 from lavague.core.context import Context, get_default_context
 from lavague.core.extractors import PythonFromMarkdownExtractor
-from lavague.core.prompt_templates import DefaultPromptTemplate
 from lavague.core.retrievers import OpsmSplitRetriever
 from lavague.core.world_model import WorldModel
-from lavague.core.agents import WebAgent
 
 import os
 import warnings
 
 
 def telemetry_warning():
     telemetry_var = os.getenv("TELEMETRY_VAR")
```

### Comparing `lavague_core-0.1.4/lavague/core/action_engine.py` & `lavague_core-0.1.5/lavague/core/action_engine.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,90 @@
 from __future__ import annotations
 from typing import Optional, Generator, List
 from llama_index.core.query_engine import RetrieverQueryEngine
-from llama_index.core import get_response_synthesizer, PromptTemplate, QueryBundle
+from llama_index.core import get_response_synthesizer, QueryBundle, PromptTemplate
 from llama_index.core.base.llms.base import BaseLLM
 from llama_index.core.base.embeddings.base import BaseEmbedding
-from lavague.core.extractors import BaseExtractor
-from lavague.core.retrievers import BaseHtmlRetriever
+from lavague.core.extractors import BaseExtractor, PythonFromMarkdownExtractor
+from lavague.core.retrievers import BaseHtmlRetriever, OpsmSplitRetriever
 from lavague.core.base_driver import BaseDriver
+from lavague.core.action_template import ActionTemplate
 from lavague.core.context import Context, get_default_context
 
+ACTION_ENGINE_PROMPT_TEMPLATE = ActionTemplate(
+    """
+{driver_capability}
+
+HTML:
+{context_str}
+Query: {query_str}
+Completion:
+
+""",
+    PythonFromMarkdownExtractor(),
+)
+
 
 class ActionEngine:
     """
     ActionEngine leverages the llm model and the embedding model to output code from the prompt and the html page.
 
     Args:
         driver (`BaseDriver`):
             The Web driver used to interact with the headless browser
+        llm (`BaseLLM`)
+            llama-index LLM that will generate the action
+        embedding (`BaseEmbedding`)
+            llama-index Embedding model
+        retriever (`BaseHtmlRetriever`)
+            Specify which algorithm will be used for RAG
+        prompt_template (`PromptTemplate`)
+            Squelette of the final prompt
+        extractor (`BaseExtractor`)
+            Specify how to extract the final code from the llm answer
     """
 
     def __init__(
         self,
         driver: BaseDriver,
-        context: Optional[Context] = None,
+        llm: BaseLLM = get_default_context().llm,
+        embedding: BaseEmbedding = get_default_context().embedding,
+        retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
+        prompt_template: PromptTemplate = ACTION_ENGINE_PROMPT_TEMPLATE.prompt_template,
+        extractor: BaseExtractor = ACTION_ENGINE_PROMPT_TEMPLATE.extractor,
     ):
-        if context is None:
-            context = get_default_context()
         self.driver: BaseDriver = driver
-        self.llm: BaseLLM = context.llm
-        self.embedding: BaseEmbedding = context.embedding
-        self.retriever: BaseHtmlRetriever = context.retriever
-        self.prompt_template: PromptTemplate = context.prompt_template.partial_format(
+        self.llm: BaseLLM = llm
+        self.embedding: BaseEmbedding = embedding
+        self.retriever: BaseHtmlRetriever = retriever
+        self.prompt_template: PromptTemplate = prompt_template.partial_format(
             driver_capability=driver.get_capability()
         )
-        self.extractor: BaseExtractor = context.extractor
+        self.extractor: BaseExtractor = extractor
+
+    @classmethod
+    def from_context(
+        cls,
+        context: Context,
+        driver: BaseDriver,
+        retriever: BaseHtmlRetriever = OpsmSplitRetriever(),
+        prompt_template: PromptTemplate = ACTION_ENGINE_PROMPT_TEMPLATE.prompt_template,
+        extractor: BaseExtractor = ACTION_ENGINE_PROMPT_TEMPLATE.extractor,
+    ) -> ActionEngine:
+        """
+        Create an ActionEngine from a context
+        """
+        return cls(
+            driver,
+            context.llm,
+            context.embedding,
+            retriever,
+            prompt_template,
+            extractor,
+        )
 
     def _get_query_engine(self, streaming: bool = True) -> RetrieverQueryEngine:
         """
         Get the llama-index query engine
 
         Args:
             html: (`str`)
```

### Comparing `lavague_core-0.1.4/lavague/core/base_driver.py` & `lavague_core-0.1.5/lavague/core/base_driver.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Tuple, Any, Callable, Optional
+from typing import Any, Callable, Optional
 from abc import ABC, abstractmethod
 from lavague.core.utilities.format_utils import (
     extract_code_from_funct,
     extract_imports_from_lines,
 )
```

### Comparing `lavague_core-0.1.4/lavague/core/extractors.py` & `lavague_core-0.1.5/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.4/lavague/core/retrievers.py` & `lavague_core-0.1.5/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.4/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.5/lavague/core/utilities/format_utils.py`

 * *Files 26% similar despite different names*

```diff
@@ -58,23 +58,55 @@
 def extract_imports_from_lines(lines: List[str]) -> str:
     """Only keep import lines from python code lines and join them"""
     return "\n".join(
         [line for line in lines if line.startswith("from") or line.startswith("import")]
     )
 
 
-def extract_instruction(text):
+import re
+
+
+def extract_world_model_instruction(text):
     # Use a regular expression to find the content after "Instruction:"
-    match = re.search(r"Instruction:\s*(.*)", text)
-    if match:
-        return match.group(
-            1
-        ).strip()  # Return the matched group, stripping any excess whitespace
-    else:
-        raise ValueError("No instruction found in the text.")
+    instruction_patterns = [
+        r"Instruction:\s*((?:- .*\n?)+)",  # For multi-line hyphenated instructions
+        r"### Instruction:\s*((?:- .*\n?)+)",  # For multi-line hyphenated instructions with ### prefix
+        r"Instruction:\s*((?:\d+\.\s.*\n?)+)",  # For multi-line numbered instructions
+        r"### Instruction:\s*((?:\d+\.\s.*\n?)+)",  # For multi-line numbered instructions with ### prefix
+        r"Instruction:\s*(.*)",  # For single-line instructions
+        r"### Instruction:\s*(.*)",  # For single-line instructions with ### prefix
+    ]
+
+    for pattern in instruction_patterns:
+        instruction_match = re.search(pattern, text, re.MULTILINE)
+        if instruction_match:
+            instruction_text = instruction_match.group(1).strip()
+            # Check if the instruction is multi-line or single-line
+            if "\n" in instruction_text:
+                # Remove newlines and extra spaces for multi-line instructions
+                instruction_str = " ".join(
+                    line.strip() for line in instruction_text.split("\n")
+                )
+            else:
+                instruction_str = instruction_text
+            return instruction_str
+
+    raise ValueError("No instruction found in the text.")
+
+
+def extract_next_engine(text):
+    # Use a regular expression to find the content after "Next engine:"
+
+    next_engine_patterns = [r"Next engine:\s*(.*)", r"### Next Engine:\s*(.*)"]
+
+    for pattern in next_engine_patterns:
+        next_engine_match = re.search(pattern, text)
+        if next_engine_match:
+            return next_engine_match.group(1).strip()
+    raise ValueError("No next engine found in the text.")
 
 
 def clean_html(
     html_to_clean: str,
     tags_to_remove: List[str] = ["style", "svg", "script"],
     attributes_to_keep: List[str] = ["id", "href"],
 ) -> str:
```

### Comparing `lavague_core-0.1.4/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.5/lavague/core/utilities/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 TELEMETRY_VAR = os.getenv("LAVAGUE_TELEMETRY")
 UNIQUE_ID = os.getenv("LAVAGUE_UNIQUE_USER_ID")
 USER_ID = str(uuid.uuid4())
 
 if UNIQUE_ID is not None:
     UNIQUE_ID = UNIQUE_ID[:256]
 
+
 def compress_img(img: Image):
     buffer: BytesIO = BytesIO()
     img_ret = img.resize((1024, 1024), Image.LANCZOS)
     img_ret = img_ret.convert("RGB")
     img_ret.save(buffer, "PNG", quality=50)
     return buffer.getvalue()
```

### Comparing `lavague_core-0.1.4/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.5/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.4/pyproject.toml` & `lavague_core-0.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.4"
+version = "0.1.5"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.1.4/PKG-INFO` & `lavague_core-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.4
+Version: 0.1.5
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

