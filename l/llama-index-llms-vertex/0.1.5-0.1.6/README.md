# Comparing `tmp/llama_index_llms_vertex-0.1.5.tar.gz` & `tmp/llama_index_llms_vertex-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_llms_vertex-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_llms_vertex-0.1.6.tar", max compression
```

## Comparing `llama_index_llms_vertex-0.1.5.tar` & `llama_index_llms_vertex-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       38 2024-03-15 17:45:47.142032 llama_index_llms_vertex-0.1.5/README.md
--rw-r--r--   0        0        0       70 2024-03-15 17:45:47.146032 llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/__init__.py
--rw-r--r--   0        0        0    13232 2024-03-15 17:45:47.146032 llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/base.py
--rw-r--r--   0        0        0     1925 2024-03-15 17:45:47.146032 llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/gemini_utils.py
--rw-r--r--   0        0        0     7793 2024-03-15 17:45:47.146032 llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/utils.py
--rw-r--r--   0        0        0     1457 2024-03-15 17:45:47.146032 llama_index_llms_vertex-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      642 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       38 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/README.md
+-rw-r--r--   0        0        0       70 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/__init__.py
+-rw-r--r--   0        0        0    13895 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/base.py
+-rw-r--r--   0        0        0     1925 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/gemini_utils.py
+-rw-r--r--   0        0        0     7793 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/utils.py
+-rw-r--r--   0        0        0     1477 2024-05-22 04:36:10.181454 llama_index_llms_vertex-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      684 1970-01-01 00:00:00.000000 llama_index_llms_vertex-0.1.6/PKG-INFO
```

### Comparing `llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/base.py` & `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,41 @@
     acompletion_with_retry,
     completion_with_retry,
     init_vertexai,
 )
 
 
 class Vertex(LLM):
+    """Vertext LLM.
+
+    Examples:
+        `pip install llama-index-llms-vertex`
+
+        ```python
+        from llama_index.llms.openai import Vertex
+
+        # Set up necessary variables
+        credentials = {
+            "project_id": "INSERT_PROJECT_ID",
+            "api_key": "INSERT_API_KEY",
+        }
+
+        # Create an instance of the Vertex class
+        llm = Vertex(
+            model="text-bison",
+            project=credentials["project_id"],
+            credentials=credentials,
+        )
+
+        # Access the complete method from the instance
+        response = llm.complete("Hello world!")
+        print(str(response))
+        ```
+    """
+
     model: str = Field(description="The vertex model to use.")
     temperature: float = Field(description="The temperature to use for sampling.")
     max_tokens: int = Field(description="The maximum number of tokens to generate.")
     examples: Optional[Sequence[ChatMessage]] = Field(
         description="Example messages for the chat model."
     )
     max_retries: int = Field(default=10, description="The maximum number of retries.")
```

### Comparing `llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/gemini_utils.py` & `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/gemini_utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_vertex-0.1.5/llama_index/llms/vertex/utils.py` & `llama_index_llms_vertex-0.1.6/llama_index/llms/vertex/utils.py`

 * *Files identical despite different names*

### Comparing `llama_index_llms_vertex-0.1.5/pyproject.toml` & `llama_index_llms_vertex-0.1.6/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -23,20 +23,21 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index llms vertex integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-llms-vertex"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 google-cloud-aiplatform = "^1.39.0"
+pyarrow = "^15.0.2"
 
 [tool.poetry.group.dev.dependencies]
 ipython = "8.10.0"
 jupyter = "^1.0.0"
 mypy = "0.991"
 pre-commit = "3.2.0"
 pylint = "2.15.10"
```

### Comparing `llama_index_llms_vertex-0.1.5/PKG-INFO` & `llama_index_llms_vertex-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: llama-index-llms-vertex
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index llms vertex integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: google-cloud-aiplatform (>=1.39.0,<2.0.0)
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
+Requires-Dist: pyarrow (>=15.0.2,<16.0.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Llms Integration: Vertex
```

