# Comparing `tmp/lavague_core-0.1.6.tar.gz` & `tmp/lavague_core-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.6.tar", max compression
+gzip compressed data, was "lavague_core-0.1.7.tar", max compression
```

## Comparing `lavague_core-0.1.6.tar` & `lavague_core-0.1.7.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-22 18:18:44.459968 lavague_core-0.1.6/LICENSE
--rw-r--r--   0        0        0        0 2024-05-22 18:18:44.460300 lavague_core-0.1.6/README.md
--rw-r--r--   0        0        0      903 2024-05-22 18:18:44.460633 lavague_core-0.1.6/lavague/core/__init__.py
--rw-r--r--   0        0        0     5603 2024-05-22 18:18:44.460900 lavague_core-0.1.6/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-22 18:18:44.460986 lavague_core-0.1.6/lavague/core/action_template.py
--rw-r--r--   0        0        0     8412 2024-05-22 18:18:44.461124 lavague_core-0.1.6/lavague/core/agents.py
--rw-r--r--   0        0        0     2771 2024-05-22 18:18:44.461208 lavague_core-0.1.6/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1189 2024-05-22 18:18:44.461308 lavague_core-0.1.6/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-22 18:18:44.461381 lavague_core-0.1.6/lavague/core/extractors.py
--rw-r--r--   0        0        0     1070 2024-05-22 18:18:44.461454 lavague_core-0.1.6/lavague/core/navigation.py
--rw-r--r--   0        0        0     1828 2024-05-22 18:18:44.461531 lavague_core-0.1.6/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-22 18:18:44.461688 lavague_core-0.1.6/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-22 18:18:44.462172 lavague_core-0.1.6/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5238 2024-05-22 18:18:44.462722 lavague_core-0.1.6/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3710 2024-05-22 18:18:44.470271 lavague_core-0.1.6/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-22 18:18:44.470506 lavague_core-0.1.6/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3074 2024-05-22 18:18:44.470620 lavague_core-0.1.6/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     9954 2024-05-22 18:18:44.470739 lavague_core-0.1.6/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-22 18:26:39.609090 lavague_core-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:18:44.459968 lavague_core-0.1.7/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 18:18:44.460300 lavague_core-0.1.7/README.md
+-rw-r--r--   0        0        0      903 2024-05-22 18:18:44.460633 lavague_core-0.1.7/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5603 2024-05-22 18:18:44.460900 lavague_core-0.1.7/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-22 18:18:44.460986 lavague_core-0.1.7/lavague/core/action_template.py
+-rw-r--r--   0        0        0     8412 2024-05-22 18:18:44.461124 lavague_core-0.1.7/lavague/core/agents.py
+-rw-r--r--   0        0        0     2771 2024-05-22 18:18:44.461208 lavague_core-0.1.7/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1189 2024-05-22 18:18:44.461308 lavague_core-0.1.7/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-22 18:18:44.461381 lavague_core-0.1.7/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1070 2024-05-22 18:18:44.461454 lavague_core-0.1.7/lavague/core/navigation.py
+-rw-r--r--   0        0        0     1828 2024-05-22 18:18:44.461531 lavague_core-0.1.7/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-22 18:18:44.461688 lavague_core-0.1.7/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-22 18:18:44.462172 lavague_core-0.1.7/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5238 2024-05-22 18:18:44.462722 lavague_core-0.1.7/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3710 2024-05-22 18:18:44.470271 lavague_core-0.1.7/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-22 18:18:44.470506 lavague_core-0.1.7/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3074 2024-05-22 18:18:44.470620 lavague_core-0.1.7/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     9954 2024-05-22 18:18:44.470739 lavague_core-0.1.7/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1102 2024-05-22 18:37:00.265774 lavague_core-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     1339 1970-01-01 00:00:00.000000 lavague_core-0.1.7/PKG-INFO
```

### Comparing `lavague_core-0.1.6/LICENSE` & `lavague_core-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/__init__.py` & `lavague_core-0.1.7/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/action_engine.py` & `lavague_core-0.1.7/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/agents.py` & `lavague_core-0.1.7/lavague/core/agents.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/base_driver.py` & `lavague_core-0.1.7/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/context.py` & `lavague_core-0.1.7/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/extractors.py` & `lavague_core-0.1.7/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/navigation.py` & `lavague_core-0.1.7/lavague/core/navigation.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/python_engine.py` & `lavague_core-0.1.7/lavague/core/python_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/retrievers.py` & `lavague_core-0.1.7/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/rewriter.py` & `lavague_core-0.1.7/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.7/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.7/lavague/core/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.7/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/utilities/web_utils.py` & `lavague_core-0.1.7/lavague/core/utilities/web_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/lavague/core/world_model.py` & `lavague_core-0.1.7/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.6/pyproject.toml` & `lavague_core-0.1.7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.6"
+version = "0.1.7"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
@@ -27,8 +27,8 @@
 python = "^3.10.0"
 llama-index = "^0.10.19"
 llama-index-retrievers-bm25 = "^0.1.3"
 lxml = "^5.2.2"
 langchain = "^0.1.20"
 ipython = "^7.34.0"
 msgpack = "^1.0.8"
-
+trafilatura = "^1.9.0"
```

### Comparing `lavague_core-0.1.6/PKG-INFO` & `lavague_core-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.6
+Version: 0.1.7
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
@@ -19,12 +19,13 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: ipython (>=7.34.0,<8.0.0)
 Requires-Dist: langchain (>=0.1.20,<0.2.0)
 Requires-Dist: llama-index (>=0.10.19,<0.11.0)
 Requires-Dist: llama-index-retrievers-bm25 (>=0.1.3,<0.2.0)
 Requires-Dist: lxml (>=5.2.2,<6.0.0)
 Requires-Dist: msgpack (>=1.0.8,<2.0.0)
+Requires-Dist: trafilatura (>=1.9.0,<2.0.0)
 Project-URL: Documentation, https://docs.lavague.ai/en/latest/
 Project-URL: Repository, https://github.com/lavague-ai/LaVague/
 Description-Content-Type: text/markdown
```

