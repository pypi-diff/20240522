# Comparing `tmp/lavague_core-0.1.5.tar.gz` & `tmp/lavague_core-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lavague_core-0.1.5.tar", max compression
+gzip compressed data, was "lavague_core-0.1.6.tar", max compression
```

## Comparing `lavague_core-0.1.5.tar` & `lavague_core-0.1.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0    11357 2024-05-15 22:13:36.162566 lavague_core-0.1.5/LICENSE
--rw-r--r--   0        0        0        0 2024-05-15 22:13:36.162566 lavague_core-0.1.5/README.md
--rw-r--r--   0        0        0      903 2024-05-21 21:17:01.343089 lavague_core-0.1.5/lavague/core/__init__.py
--rw-r--r--   0        0        0     5603 2024-05-21 21:06:53.301594 lavague_core-0.1.5/lavague/core/action_engine.py
--rw-r--r--   0        0        0      374 2024-05-21 21:06:53.301594 lavague_core-0.1.5/lavague/core/action_template.py
--rw-r--r--   0        0        0     9339 2024-05-21 22:50:43.800201 lavague_core-0.1.5/lavague/core/agents.py
--rw-r--r--   0        0        0     2771 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/base_driver.py
--rw-r--r--   0        0        0     1189 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/context.py
--rw-r--r--   0        0        0     1296 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/extractors.py
--rw-r--r--   0        0        0     1070 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/navigation.py
--rw-r--r--   0        0        0     4153 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/python_engine.py
--rw-r--r--   0        0        0    12117 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/retrievers.py
--rw-r--r--   0        0        0     1795 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/rewriter.py
--rw-r--r--   0        0        0     5238 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/utilities/format_utils.py
--rw-r--r--   0        0        0     3710 2024-05-21 21:06:53.269595 lavague_core-0.1.5/lavague/core/utilities/telemetry.py
--rw-r--r--   0        0        0     1361 2024-05-15 22:13:36.162566 lavague_core-0.1.5/lavague/core/utilities/version_checker.py
--rw-r--r--   0        0        0     3074 2024-05-21 22:50:43.796201 lavague_core-0.1.5/lavague/core/utilities/web_utils.py
--rw-r--r--   0        0        0     9878 2024-05-21 21:06:53.305594 lavague_core-0.1.5/lavague/core/world_model.py
--rw-r--r--   0        0        0     1080 2024-05-21 23:06:09.391404 lavague_core-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-22 18:18:44.459968 lavague_core-0.1.6/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 18:18:44.460300 lavague_core-0.1.6/README.md
+-rw-r--r--   0        0        0      903 2024-05-22 18:18:44.460633 lavague_core-0.1.6/lavague/core/__init__.py
+-rw-r--r--   0        0        0     5603 2024-05-22 18:18:44.460900 lavague_core-0.1.6/lavague/core/action_engine.py
+-rw-r--r--   0        0        0      374 2024-05-22 18:18:44.460986 lavague_core-0.1.6/lavague/core/action_template.py
+-rw-r--r--   0        0        0     8412 2024-05-22 18:18:44.461124 lavague_core-0.1.6/lavague/core/agents.py
+-rw-r--r--   0        0        0     2771 2024-05-22 18:18:44.461208 lavague_core-0.1.6/lavague/core/base_driver.py
+-rw-r--r--   0        0        0     1189 2024-05-22 18:18:44.461308 lavague_core-0.1.6/lavague/core/context.py
+-rw-r--r--   0        0        0     1296 2024-05-22 18:18:44.461381 lavague_core-0.1.6/lavague/core/extractors.py
+-rw-r--r--   0        0        0     1070 2024-05-22 18:18:44.461454 lavague_core-0.1.6/lavague/core/navigation.py
+-rw-r--r--   0        0        0     1828 2024-05-22 18:18:44.461531 lavague_core-0.1.6/lavague/core/python_engine.py
+-rw-r--r--   0        0        0    12117 2024-05-22 18:18:44.461688 lavague_core-0.1.6/lavague/core/retrievers.py
+-rw-r--r--   0        0        0     1795 2024-05-22 18:18:44.462172 lavague_core-0.1.6/lavague/core/rewriter.py
+-rw-r--r--   0        0        0     5238 2024-05-22 18:18:44.462722 lavague_core-0.1.6/lavague/core/utilities/format_utils.py
+-rw-r--r--   0        0        0     3710 2024-05-22 18:18:44.470271 lavague_core-0.1.6/lavague/core/utilities/telemetry.py
+-rw-r--r--   0        0        0     1361 2024-05-22 18:18:44.470506 lavague_core-0.1.6/lavague/core/utilities/version_checker.py
+-rw-r--r--   0        0        0     3074 2024-05-22 18:18:44.470620 lavague_core-0.1.6/lavague/core/utilities/web_utils.py
+-rw-r--r--   0        0        0     9954 2024-05-22 18:18:44.470739 lavague_core-0.1.6/lavague/core/world_model.py
+-rw-r--r--   0        0        0     1080 2024-05-22 18:26:39.609090 lavague_core-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1295 1970-01-01 00:00:00.000000 lavague_core-0.1.6/PKG-INFO
```

### Comparing `lavague_core-0.1.5/LICENSE` & `lavague_core-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/__init__.py` & `lavague_core-0.1.6/lavague/core/__init__.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/action_engine.py` & `lavague_core-0.1.6/lavague/core/action_engine.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/agents.py` & `lavague_core-0.1.6/lavague/core/agents.py`

 * *Files 8% similar despite different names*

```diff
@@ -183,43 +183,23 @@
                             screenshot_after_action,
                         )
                 if not success:
                     instruction = "[FAILED] " + instruction
                 image_documents = SimpleDirectoryReader("./screenshots").load_data()
 
             elif "Python Engine" in next_engine:
-                state = {"html": self.driver.page_source}
-                success = False
-
-                for _ in range(n_attempts):
-                    try:
-                        python_code = python_engine.generate_code(instruction, state)
-                        output = python_engine.execute_code(python_code, state)
-
-                        if output:
-                            current_state["internal_state"]["agent_outputs"].append(
-                                output
-                            )
-                            success = True
-                            break
-                        else:
-                            print("Empty output of Python engine")
-                            print("Code generated by Python Engine: ", python_code)
-                            print("Output generated by Python Engine: ", output)
-                    except Exception as e:
-                        print(f"Python engine execution failed. Retrying...")
-                        print("Error: ", e)
-
-                if not success:
-                    instruction = "[FAILED] " + instruction
+                html = self.driver.page_source
+                output = python_engine.extract_information(instruction, html)
+                if output:
+                    current_state["internal_state"]["agent_outputs"].append(output)
 
             elif "Navigation Controls" in next_engine:
                 navigation_control.execute_instruction(instruction)
                 self.driver.save_screenshot(screenshot_path)
-                screenshot_before_action = screenshot_after_action
+                
                 screenshot_after_action = Image.open(screenshot_path)
                 if display:
                     display_screenshot(screenshot_after_action)
                 image_documents = SimpleDirectoryReader("./screenshots").load_data()
 
             elif next_engine == "STOP" or instruction == "STOP":
                 print("Objective reached. Stopping...")
```

### Comparing `lavague_core-0.1.5/lavague/core/base_driver.py` & `lavague_core-0.1.6/lavague/core/base_driver.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/context.py` & `lavague_core-0.1.6/lavague/core/context.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/extractors.py` & `lavague_core-0.1.6/lavague/core/extractors.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/navigation.py` & `lavague_core-0.1.6/lavague/core/navigation.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/retrievers.py` & `lavague_core-0.1.6/lavague/core/retrievers.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/rewriter.py` & `lavague_core-0.1.6/lavague/core/rewriter.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/utilities/format_utils.py` & `lavague_core-0.1.6/lavague/core/utilities/format_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/utilities/telemetry.py` & `lavague_core-0.1.6/lavague/core/utilities/telemetry.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/utilities/version_checker.py` & `lavague_core-0.1.6/lavague/core/utilities/version_checker.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/utilities/web_utils.py` & `lavague_core-0.1.6/lavague/core/utilities/web_utils.py`

 * *Files identical despite different names*

### Comparing `lavague_core-0.1.5/lavague/core/world_model.py` & `lavague_core-0.1.6/lavague/core/world_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,14 +163,15 @@
 # Python Engine guidelines
 - When providing an instruction to the Python Engine, do not provide any guideline on using visual information such as the screenshot, as the Python Engine does not have access to it.
 - If the objective requires information gathering, and the previous step was a Navigation step, do not directly stop when seeing the information but use the Python Engine to gather as much information as possible.
 
 # Navigation guidlines
 - If the screenshot provides information but seems insufficient, use navigation controls to further explore the page.
 - When providing information for the Navigation Engine, focus on elements that are most likely interactable, such as buttons, links, or forms and be precise in your description of the element to avoid ambiguitiy.
+- If several steps have to be taken, provide instructions in bullet points.
 
 Here are previous examples:
 {examples}
 
 Here is the next objective:
 Objective: {objective}
 Previous instructions:
```

### Comparing `lavague_core-0.1.5/pyproject.toml` & `lavague_core-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 build-backend = "poetry.core.masonry.api"
 requires = ["poetry-core"]
 
 [tool.poetry]
 name = "lavague-core"
-version = "0.1.5"
+version = "0.1.6"
 description = "automation code generation from text instructions"
 authors = ["lavague-ai"]
 readme = "README.md"
 license = "Apache-2.0"
 classifiers = [
   "Development Status :: 3 - Alpha",
   "Intended Audience :: Developers",
```

### Comparing `lavague_core-0.1.5/PKG-INFO` & `lavague_core-0.1.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lavague-core
-Version: 0.1.5
+Version: 0.1.6
 Summary: automation code generation from text instructions
 Home-page: https://lavague.ai
 License: Apache-2.0
 Keywords: LAM,action,automation,LLM,NLP,RAG,selenium,playwright
 Author: lavague-ai
 Requires-Python: >=3.10.0,<4.0.0
 Classifier: Development Status :: 3 - Alpha
```

