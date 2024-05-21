# Comparing `tmp/lavague_core-0.1.3.tar.gz` & `tmp/lavague_core-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.3.tar", max compression
+gzip compressed data, was "lavague_core-0.1.4.tar", max compression
```

## Comparing `lavague_core-0.1.3.tar` & `lavague_core-0.1.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0    11357 2024-05-16 06:03:22.535020 lavague_core-0.1.3/LICENSE
--rw-r--r--   0        0        0        0 2024-05-16 06:03:22.535047 lavague_core-0.1.3/README.md
--rw-r--r--   0        0        0      956 2024-05-16 06:03:22.535306 lavague_core-0.1.3/lavague/core/__init__.py
--rw-r--r--   0        0        0     4084 2024-05-16 06:03:22.535479 lavague_core-0.1.3/lavague/core/action_engine.py
--rw-r--r--   0        0        0     5873 2024-05-17 07:27:00.823259 lavague_core-0.1.3/lavague/core/agents.py
--rw-r--r--   0        0        0     2778 2024-05-16 06:03:22.535653 lavague_core-0.1.3/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1896 2024-05-16 06:03:22.535742 lavague_core-0.1.3/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-16 06:03:22.535814 lavague_core-0.1.3/lavague/core/extractors.py
--rw-r--r--   0        0        0      613 2024-05-16 06:03:22.535883 lavague_core-0.1.3/lavague/core/prompt_templates.py
--rw-r--r--   0        0        0    12117 2024-05-16 06:03:22.536134 lavague_core-0.1.3/lavague/core/retrievers.py
--rw-r--r--   0        0        0     3793 2024-05-16 06:03:22.536249 lavague_core-0.1.3/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3563 2024-05-17 07:27:58.340843 lavague_core-0.1.3/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-16 06:03:22.536457 lavague_core-0.1.3/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0      491 2024-05-16 06:03:22.536523 lavague_core-0.1.3/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     3445 2024-05-16 06:03:22.536696 lavague_core-0.1.3/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-17 17:57:46.869711 lavague_core-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 06:03:22.535020 lavague_core-0.1.4/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-16 06:03:22.535047 lavague_core-0.1.4/README.md
+-rw-r--r--   0        0        0      956 2024-05-16 06:03:22.535306 lavague_core-0.1.4/lavague/core/__init__.py
+-rw-r--r--   0        0        0     4084 2024-05-16 06:03:22.535479 lavague_core-0.1.4/lavague/core/action_engine.py
+-rw-r--r--   0        0        0     5873 2024-05-19 20:23:23.623772 lavague_core-0.1.4/lavague/core/agents.py
+-rw-r--r--   0        0        0     2778 2024-05-16 06:03:22.535653 lavague_core-0.1.4/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1896 2024-05-16 06:03:22.535742 lavague_core-0.1.4/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-16 06:03:22.535814 lavague_core-0.1.4/lavague/core/extractors.py
+-rw-r--r--   0        0        0      613 2024-05-16 06:03:22.535883 lavague_core-0.1.4/lavague/core/prompt_templates.py
+-rw-r--r--   0        0        0    12117 2024-05-16 06:03:22.536134 lavague_core-0.1.4/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     3793 2024-05-16 06:03:22.536249 lavague_core-0.1.4/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3709 2024-05-21 06:02:21.563242 lavague_core-0.1.4/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-16 06:03:22.536457 lavague_core-0.1.4/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0      491 2024-05-16 06:03:22.536523 lavague_core-0.1.4/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     3445 2024-05-16 06:03:22.536696 lavague_core-0.1.4/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1080 2024-05-21 06:18:35.433464 lavague_core-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.4/PKG-INFO
```

### Comparing `lavague_core-0.1.3/LICENSE` & `lavague_core-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/__init__.py` & `lavague_core-0.1.4/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/action_engine.py` & `lavague_core-0.1.4/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/agents.py` & `lavague_core-0.1.4/lavague/core/agents.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/base_driver.py` & `lavague_core-0.1.4/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/context.py` & `lavague_core-0.1.4/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/extractors.py` & `lavague_core-0.1.4/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/prompt_templates.py` & `lavague_core-0.1.4/lavague/core/prompt_templates.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/retrievers.py` & `lavague_core-0.1.4/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.4/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.4/lavague/core/utilities/telemetry.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 import msgpack
 from PIL import Image
 from io import BytesIO
 
 from .version_checker import get_installed_version
 
 TELEMETRY_VAR = os.getenv("LAVAGUE_TELEMETRY")
+UNIQUE_ID = os.getenv("LAVAGUE_UNIQUE_USER_ID")
 USER_ID = str(uuid.uuid4())
 
+if UNIQUE_ID is not None:
+    UNIQUE_ID = UNIQUE_ID[:256]
 
 def compress_img(img: Image):
     buffer: BytesIO = BytesIO()
     img_ret = img.resize((1024, 1024), Image.LANCZOS)
     img_ret = img_ret.convert("RGB")
     img_ret.save(buffer, "PNG", quality=50)
     return buffer.getvalue()
@@ -79,14 +82,15 @@
     try:
         if TELEMETRY_VAR is None:
             json_send = {
                 "action_id": action_id,
                 "version": get_installed_version("lavague"),
                 "code_produced": code,
                 "llm": model_name,
+                "unique_id": UNIQUE_ID,
                 "user_id": USER_ID,
                 "origin": origin,
                 "url": url,
                 "success": success_str,
                 "instruction": instruction,
                 "source_nodes": source_nodes,
                 "error_msg": error,
```

### Comparing `lavague_core-0.1.3/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.4/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/lavague/core/world_model.py` & `lavague_core-0.1.4/lavague/core/world_model.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.3/pyproject.toml` & `lavague_core-0.1.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.3"
+version = "0.1.4"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.1.3/PKG-INFO` & `lavague_core-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.3
+Version: 0.1.4
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

