# Comparing `tmp/vision_agent-0.2.8.tar.gz` & `tmp/vision_agent-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vision_agent-0.2.8.tar", max compression
+gzip compressed data, was "vision_agent-0.2.9.tar", max compression
```

## Comparing `vision_agent-0.2.8.tar` & `vision_agent-0.2.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0    11357 2024-04-26 04:03:18.769806 vision_agent-0.2.8/LICENSE
--rw-r--r--   0        0        0     6639 2024-04-26 04:03:18.769806 vision_agent-0.2.8/README.md
--rw-r--r--   0        0        0     2099 2024-04-26 04:03:19.333807 vision_agent-0.2.8/pyproject.toml
--rw-r--r--   0        0        0      108 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/__init__.py
--rw-r--r--   0        0        0      127 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/__init__.py
--rw-r--r--   0        0        0      529 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/agent.py
--rw-r--r--   0        0        0    11511 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/easytool.py
--rw-r--r--   0        0        0     4526 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/easytool_prompts.py
--rw-r--r--   0        0        0    10506 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/reflexion.py
--rw-r--r--   0        0        0     9342 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/reflexion_prompts.py
--rw-r--r--   0        0        0    26112 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/vision_agent.py
--rw-r--r--   0        0        0     7342 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/agent/vision_agent_prompts.py
--rw-r--r--   0        0        0        0 2024-04-26 04:03:18.781806 vision_agent-0.2.8/vision_agent/fonts/__init__.py
--rw-r--r--   0        0        0  1594400 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/fonts/default_font_ch_en.ttf
--rw-r--r--   0        0        0     7552 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/image_utils.py
--rw-r--r--   0        0        0       48 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/llm/__init__.py
--rw-r--r--   0        0        0     5383 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/llm/llm.py
--rw-r--r--   0        0        0       67 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/lmm/__init__.py
--rw-r--r--   0        0        0    10539 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/lmm/lmm.py
--rw-r--r--   0        0        0      413 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/__init__.py
--rw-r--r--   0        0        0     1430 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/prompts.py
--rw-r--r--   0        0        0    43013 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/tools.py
--rw-r--r--   0        0        0     7653 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/tools/video.py
--rw-r--r--   0        0        0     1792 2024-04-26 04:03:18.793806 vision_agent-0.2.8/vision_agent/type_defs.py
--rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-26 22:27:53.968212 vision_agent-0.2.9/LICENSE
+-rw-r--r--   0        0        0     6639 2024-04-26 22:27:53.968212 vision_agent-0.2.9/README.md
+-rw-r--r--   0        0        0     2099 2024-04-26 22:27:54.536213 vision_agent-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0      108 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/__init__.py
+-rw-r--r--   0        0        0      127 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/__init__.py
+-rw-r--r--   0        0        0      529 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/agent.py
+-rw-r--r--   0        0        0    11511 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/easytool.py
+-rw-r--r--   0        0        0     4656 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/easytool_prompts.py
+-rw-r--r--   0        0        0    10506 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/reflexion.py
+-rw-r--r--   0        0        0     9342 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/reflexion_prompts.py
+-rw-r--r--   0        0        0    26243 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/vision_agent.py
+-rw-r--r--   0        0        0     8570 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/agent/vision_agent_prompts.py
+-rw-r--r--   0        0        0        0 2024-04-26 22:27:53.980211 vision_agent-0.2.9/vision_agent/fonts/__init__.py
+-rw-r--r--   0        0        0  1594400 2024-04-26 22:27:53.988211 vision_agent-0.2.9/vision_agent/fonts/default_font_ch_en.ttf
+-rw-r--r--   0        0        0     7586 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/image_utils.py
+-rw-r--r--   0        0        0       48 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/llm/__init__.py
+-rw-r--r--   0        0        0     5383 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/llm/llm.py
+-rw-r--r--   0        0        0       67 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/lmm/__init__.py
+-rw-r--r--   0        0        0    10539 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/lmm/lmm.py
+-rw-r--r--   0        0        0      413 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1430 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/tools/prompts.py
+-rw-r--r--   0        0        0    43823 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/tools/tools.py
+-rw-r--r--   0        0        0     7653 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/tools/video.py
+-rw-r--r--   0        0        0     1792 2024-04-26 22:27:53.992211 vision_agent-0.2.9/vision_agent/type_defs.py
+-rw-r--r--   0        0        0     7697 1970-01-01 00:00:00.000000 vision_agent-0.2.9/PKG-INFO
```

### Comparing `vision_agent-0.2.8/LICENSE` & `vision_agent-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/README.md` & `vision_agent-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/pyproject.toml` & `vision_agent-0.2.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "vision-agent"
-version = "0.2.8"
+version = "0.2.9"
 description = "Toolset for Vision Agent"
 authors = ["Landing AI <dev@landing.ai>"]
 readme = "README.md"
 packages = [{include = "vision_agent"}]
 
 [tool.poetry.urls]
 "Homepage" = "https://landing.ai"
```

### Comparing `vision_agent-0.2.8/vision_agent/agent/agent.py` & `vision_agent-0.2.9/vision_agent/agent/agent.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/agent/easytool.py` & `vision_agent-0.2.9/vision_agent/agent/easytool.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/agent/easytool_prompts.py` & `vision_agent-0.2.9/vision_agent/agent/easytool_prompts.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 Example 1: {{"ID": 1}}
 Example 2: {{"ID": 2}}
 
 Output: """
 
 CHOOSE_PARAMETER = """Given a user's question and an API tool documentation, you need to output parameters according to the API tool documentation to successfully call the API to solve the user's question.
 Please note that:
-1. The Example in the API tool documentation can help you better understand the use of the API.
+1. The Example in the API tool documentation can help you better understand the use of the API. Pay attention to the examples which show how to parse the question and extract tool parameters such as prompts and visual inputs.
 2. Ensure the parameters you output are correct. The output must contain the required parameters, and can contain the optional parameters based on the question. If there are no paremters in the required parameters and optional parameters, just leave it as {{"Parameters":{{}}}}
 3. If the user's question mentions other APIs, you should ONLY consider the API tool documentation I give and do not consider other APIs.
 4. The question may have dependencies on answers of other questions, so we will provide logs of previous questions and answers for your reference.
 5. If you need to use this API multiple times, please set "Parameters" to a list.
 6. You must ONLY output in a parsible JSON format. Two example outputs looks like:
 
 Example 1: {{"Parameters":{{"input": [1,2,3]}}}}
```

### Comparing `vision_agent-0.2.8/vision_agent/agent/reflexion.py` & `vision_agent-0.2.9/vision_agent/agent/reflexion.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/agent/reflexion_prompts.py` & `vision_agent-0.2.9/vision_agent/agent/reflexion_prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/agent/vision_agent.py` & `vision_agent-0.2.9/vision_agent/agent/vision_agent.py`

 * *Files 1% similar despite different names*

```diff
@@ -304,14 +304,17 @@
 def _handle_extract_frames(
     image_to_data: Dict[str, Dict], tool_result: Dict
 ) -> Dict[str, Dict]:
     image_to_data = image_to_data.copy()
     # handle extract_frames_ case, useful if it extracts frames but doesn't do
     # any following processing
     for video_file_output in tool_result["call_results"]:
+        # When the video tool is run with wrong parameters, exit the loop
+        if len(video_file_output) < 2:
+            break
         for frame, _ in video_file_output:
             image = frame
             if image not in image_to_data:
                 image_to_data[image] = {
                     "bboxes": [],
                     "masks": [],
                     "heat_map": [],
@@ -443,15 +446,15 @@
     """
 
     def __init__(
         self,
         task_model: Optional[Union[LLM, LMM]] = None,
         answer_model: Optional[Union[LLM, LMM]] = None,
         reflect_model: Optional[Union[LLM, LMM]] = None,
-        max_retries: int = 3,
+        max_retries: int = 2,
         verbose: bool = False,
         report_progress_callback: Optional[Callable[[str], None]] = None,
     ):
         """VisionAgent constructor.
 
         Parameters:
             task_model: the model to use for task decomposition.
```

### Comparing `vision_agent-0.2.8/vision_agent/agent/vision_agent_prompts.py` & `vision_agent-0.2.9/vision_agent/agent/vision_agent_prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -22,80 +22,88 @@
 {tool_usage}
 
 Final answer:
 {final_answer}
 
 Reflection: """
 
-TASK_DECOMPOSE = """You need to decompose a user's complex question into some simple subtasks and let the model execute it step by step.
+TASK_DECOMPOSE = """You need to decompose a user's complex question into one or more simple subtasks and let the model execute it step by step.
 This is the user's question: {question}
 This is the tool list:
 {tools}
 
 Please note that:
-1. You should only decompose this user's complex question into some simple subtasks which can be executed easily by using one single tool in the tool list.
-2. If one subtask needs the results from another subtask, you should write clearly. For example:
+1. If the given task is simple and the answer can be provided by executing one tool, you should only use that tool to provide the answer.
+2. If the given task is complex, You should decompose this user's complex question into simple subtasks which can only be executed easily by using one single tool in the tool list.
+3. You should try to decompose the complex question into least number of subtasks.
+4. If one subtask needs the results from another subtask, you should write clearly. For example:
 {{"Tasks": ["Convert 23 km/h to X km/min by 'divide_'", "Multiply X km/min by 45 min to get Y by 'multiply_'"]}}
-3. You must ONLY output in a parsible JSON format. An example output looks like:
+5. You must ONLY output in a parsible JSON format. An example output looks like:
 
 {{"Tasks": ["Task 1", "Task 2", ...]}}
 
 Output: """
 
-TASK_DECOMPOSE_DEPENDS = """You need to decompose a user's complex question into some simple subtasks and let the model execute it step by step.
+TASK_DECOMPOSE_DEPENDS = """You need to decompose a user's complex question into one or more simple subtasks and let the model execute it step by step.
 This is the user's question: {question}
 
 This is the tool list:
 {tools}
 
 This is a reflection from a previous failed attempt:
 {reflections}
 
 Please note that:
-1. You should only decompose this user's complex question into some simple subtasks which can be executed easily by using one single tool in the tool list.
-2. If one subtask needs the results from another subtask, you should write clearly. For example:
+1. If the given task is simple and the answer can be provided by executing one tool, you should only use that tool to provide the answer.
+2. If the given task is complex, You should decompose this user's complex question into simple subtasks which can only be executed easily by using one single tool in the tool list.
+3. You should try to decompose the complex question into least number of subtasks.
+4. If one subtask needs the results from another subtask, you should write clearly. For example:
 {{"Tasks": ["Convert 23 km/h to X km/min by 'divide_'", "Multiply X km/min by 45 min to get Y by 'multiply_'"]}}
-3. You must ONLY output in a parsible JSON format. An example output looks like:
+5. You must ONLY output in a parsible JSON format. An example output looks like:
 
 {{"Tasks": ["Task 1", "Task 2", ...]}}
 
 Output: """
 
 CHOOSE_TOOL = """This is the user's question: {question}
 These are the tools you can select to solve the question:
 {tools}
 
 Please note that:
-1. You should only choose one tool from the Tool List to solve this question.
-2. You must ONLY output the ID of the tool you chose in a parsible JSON format. Two example outputs look like:
+1. You should only choose one tool from the Tool List to solve this question and it should have maximum chance of solving the question.
+2. You should only choose the tool whose parameters are most relevant to the user's question and are availale as part of the question.
+3. You should choose the tool whose return type is most relevant to the answer of the user's question.
+4. You must ONLY output the ID of the tool you chose in a parsible JSON format. Two example outputs look like:
 
 Example 1: {{"ID": 1}}
 Example 2: {{"ID": 2}}
 
 Output: """
 
 CHOOSE_TOOL_DEPENDS = """This is the user's question: {question}
 These are the tools you can select to solve the question:
 {tools}
 
 This is a reflection from a previous failed attempt:
 {reflections}
 
 Please note that:
-1. You should only choose one tool from the Tool List to solve this question.
-2. You must ONLY output the ID of the tool you chose in a parsible JSON format. Two example outputs look like:
+1. You should only choose one tool from the Tool List to solve this question and it should have maximum chance of solving the question.
+2. You should only choose the tool whose parameters are most relevant to the user's question and are availale as part of the question.
+3. You should choose the tool whose return type is most relevant to the answer of the user's question.
+4. You must ONLY output the ID of the tool you chose in a parsible JSON format. Two example outputs look like:
 
 Example 1: {{"ID": 1}}
 Example 2: {{"ID": 2}}
 
 Output: """
 
 CHOOSE_PARAMETER_DEPENDS = """Given a user's question and an API tool documentation, you need to output parameters according to the API tool documentation to successfully call the API to solve the user's question.
 Please note that:
-1. The Example in the API tool documentation can help you better understand the use of the API.
+1. The Example in the API tool documentation can help you better understand the use of the API. Pay attention to the examples which show how to parse the question and extract tool parameters such as prompts and visual inputs.
 2. Ensure the parameters you output are correct. The output must contain the required parameters, and can contain the optional parameters based on the question. If there are no paremters in the required parameters and optional parameters, just leave it as {{"Parameters":{{}}}}
 3. If the user's question mentions other APIs, you should ONLY consider the API tool documentation I give and do not consider other APIs.
 4. The question may have dependencies on answers of other questions, so we will provide logs of previous questions and answers for your reference.
 5. If you need to use this API multiple times, please set "Parameters" to a list.
 6. You must ONLY output in a parsible JSON format. Two example outputs look like:
 
 Example 1: {{"Parameters":{{"input": [1,2,3]}}}}
```

### Comparing `vision_agent-0.2.8/vision_agent/fonts/default_font_ch_en.ttf` & `vision_agent-0.2.9/vision_agent/fonts/default_font_ch_en.ttf`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/image_utils.py` & `vision_agent-0.2.9/vision_agent/image_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -234,15 +234,15 @@
         The image with the heatmap overlayed
     """
     if isinstance(image, (str, Path)):
         image = Image.open(image)
     elif isinstance(image, np.ndarray):
         image = Image.fromarray(image)
 
-    if "heat_map" not in heat_map:
+    if "heat_map" not in heat_map or len(heat_map["heat_map"]) == 0:
         return image.convert("RGB")
 
     image = image.convert("L")
     # Only one heat map per image, so no need to loop through masks
     mask = Image.fromarray(heat_map["heat_map"][0])
 
     overlay = Image.new("RGBA", mask.size)
```

### Comparing `vision_agent-0.2.8/vision_agent/llm/llm.py` & `vision_agent-0.2.9/vision_agent/llm/llm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/lmm/lmm.py` & `vision_agent-0.2.9/vision_agent/lmm/lmm.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/tools/prompts.py` & `vision_agent-0.2.9/vision_agent/tools/prompts.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/tools/tools.py` & `vision_agent-0.2.9/vision_agent/tools/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -171,38 +171,45 @@
         >>> t("red line. yellow dot", "ct_scan1.jpg")
         [{'labels': ['red line', 'yellow dot'],
         'bboxes': [[0.38, 0.15, 0.59, 0.7], [0.48, 0.25, 0.69, 0.71]],
         'scores': [0.98, 0.02]}]
     """
 
     name = "grounding_dino_"
-    description = "'grounding_dino_' is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. It returns a list of bounding boxes, label names and associated probability scores."
+    description = "'grounding_dino_' is a tool that can detect and count objects given a text prompt such as category names or referring expressions. It returns a list and count of bounding boxes, label names and associated probability scores."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
         ],
         "optional_parameters": [
             {"name": "box_threshold", "type": "float"},
             {"name": "iou_threshold", "type": "float"},
         ],
         "examples": [
             {
+                "scenario": "Can you detect and count the giraffes and zebras in this image? Image name: animal.jpg",
+                "parameters": {
+                    "prompt": "giraffe. zebra",
+                    "image": "person.jpg",
+                },
+            },
+            {
                 "scenario": "Can you build me a car detector?",
                 "parameters": {"prompt": "car", "image": ""},
             },
             {
                 "scenario": "Can you detect the person on the left and right? Image name: person.jpg",
                 "parameters": {
                     "prompt": "left person. right person",
                     "image": "person.jpg",
                 },
             },
             {
-                "scenario": "Detect the red shirts and green shirst. Image name: shirts.jpg",
+                "scenario": "Detect the red shirts and green shirt. Image name: shirts.jpg",
                 "parameters": {
                     "prompt": "red shirt. green shirt",
                     "image": "shirts.jpg",
                     "box_threshold": 0.20,
                     "iou_threshold": 0.75,
                 },
             },
@@ -267,26 +274,33 @@
            [0, 0, 0, ..., 0, 0, 0],
            ...,
            [1, 1, 1, ..., 1, 1, 1],
            [1, 1, 1, ..., 1, 1, 1]], dtype=uint8)]}]
     """
 
     name = "grounding_sam_"
-    description = "'grounding_sam_' is a tool that can detect arbitrary objects with inputs such as category names or referring expressions. It returns a list of bounding boxes, label names and masks file names and associated probability scores."
+    description = "'grounding_sam_' is a tool that can detect and segment objects given a text prompt such as category names or referring expressions. It returns a list of bounding boxes, label names and masks file names and associated probability scores."
     usage = {
         "required_parameters": [
             {"name": "prompt", "type": "str"},
             {"name": "image", "type": "str"},
         ],
         "optional_parameters": [
             {"name": "box_threshold", "type": "float"},
             {"name": "iou_threshold", "type": "float"},
         ],
         "examples": [
             {
+                "scenario": "Can you segment the apples and grapes in this image? Image name: fruits.jpg",
+                "parameters": {
+                    "prompt": "apple. grape",
+                    "image": "fruits.jpg",
+                },
+            },
+            {
                 "scenario": "Can you build me a car segmentor?",
                 "parameters": {"prompt": "car", "image": ""},
             },
             {
                 "scenario": "Can you segment the person on the left and right? Image name: person.jpg",
                 "parameters": {
                     "prompt": "left person. right person",
@@ -474,23 +488,23 @@
         >>> import vision_agent as va
         >>> zshot_count = va.tools.ZeroShotCounting()
         >>> zshot_count("image1.jpg")
         {'count': 45}
     """
 
     name = "zero_shot_counting_"
-    description = "'zero_shot_counting_' is a tool that counts and returns the total number of instances of an object present in an image belonging to the same class without a text or visual prompt."
+    description = "'zero_shot_counting_' is a tool that counts foreground items given only an image and no other information. It returns only the count of the objects in the image"
 
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
         ],
         "examples": [
             {
-                "scenario": "Can you count the lids in the image? Image name: lids.jpg",
+                "scenario": "Can you count the items in the image? Image name: lids.jpg",
                 "parameters": {"image": "lids.jpg"},
             },
             {
                 "scenario": "Can you count the total number of objects in this image? Image name: tray.jpg",
                 "parameters": {"image": "tray.jpg"},
             },
             {
@@ -531,32 +545,32 @@
         >>> import vision_agent as va
         >>> prompt_count = va.tools.VisualPromptCounting()
         >>> prompt_count(image="image1.jpg", prompt="0.1, 0.1, 0.4, 0.42")
         {'count': 23}
     """
 
     name = "visual_prompt_counting_"
-    description = "'visual_prompt_counting_' is a tool that can count and return total number of instances of an object present in an image belonging to the same class given an example bounding box."
+    description = "'visual_prompt_counting_' is a tool that counts foreground items in an image given a visual prompt which is a bounding box describing the object. It returns only the count of the objects in the image."
 
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
             {"name": "prompt", "type": "str"},
         ],
         "examples": [
             {
-                "scenario": "Here is an example of a lid '0.1, 0.1, 0.14, 0.2', Can you count the lids in the image ? Image name: lids.jpg",
+                "scenario": "Here is an example of a lid '0.1, 0.1, 0.14, 0.2', Can you count the items in the image ? Image name: lids.jpg",
                 "parameters": {"image": "lids.jpg", "prompt": "0.1, 0.1, 0.14, 0.2"},
             },
             {
                 "scenario": "Can you count the total number of objects in this image ? Image name: tray.jpg",
                 "parameters": {"image": "tray.jpg", "prompt": "0.1, 0.1, 0.2, 0.25"},
             },
             {
-                "scenario": "Can you build me a few shot object counting tool ? Image name: shirts.jpg",
+                "scenario": "Can you count this item based on an example, reference_data: '0.1, 0.15, 0.2, 0.2' ? Image name: shirts.jpg",
                 "parameters": {
                     "image": "shirts.jpg",
                     "prompt": "0.1, 0.15, 0.2, 0.2",
                 },
             },
             {
                 "scenario": "Can you build me a counting tool based on an example prompt ? Image name: shoes.jpg",
@@ -601,15 +615,15 @@
         >>> import vision_agent as va
         >>> vqa_tool = va.tools.VisualQuestionAnswering()
         >>> vqa_tool(image="image1.jpg", prompt="describe this image in detail")
         {'text': "The image contains a cat sitting on a table with a bowl of milk."}
     """
 
     name = "visual_question_answering_"
-    description = "'visual_question_answering_' is a tool that can describe the contents of the image and it can also answer basic questions about the image."
+    description = "'visual_question_answering_' is a tool that can answer basic questions about the image given a question and an image. It returns a text describing the image and the answer to the question"
 
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
             {"name": "prompt", "type": "str"},
         ],
         "examples": [
@@ -668,15 +682,15 @@
         >>> import vision_agent as va
         >>> vqa_tool = va.tools.ImageQuestionAnswering()
         >>> vqa_tool(image="image1.jpg", prompt="describe this image in detail")
         {'text': "The image contains a cat sitting on a table with a bowl of milk."}
     """
 
     name = "image_question_answering_"
-    description = "'image_question_answering_' is a tool that can describe the contents of the image and it can also answer basic questions about the image."
+    description = "'image_question_answering_' is a tool that can answer basic questions about the image given a question and an image. It returns a text describing the image and the answer to the question"
 
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
             {"name": "prompt", "type": "str"},
         ],
         "examples": [
@@ -769,15 +783,15 @@
         return {"image": tmp.name}
 
 
 class BboxArea(Tool):
     r"""BboxArea returns the area of the bounding box in pixels normalized to 2 decimal places."""
 
     name = "bbox_area_"
-    description = "'bbox_area_' returns the area of the bounding box in pixels normalized to 2 decimal places."
+    description = "'bbox_area_' returns the area of the given bounding box in pixels normalized to 2 decimal places."
     usage = {
         "required_parameters": [{"name": "bboxes", "type": "List[int]"}],
         "examples": [
             {
                 "scenario": "If you want to calculate the area of the bounding box [0.2, 0.21, 0.34, 0.42]",
                 "parameters": {"bboxes": [0.2, 0.21, 0.34, 0.42]},
             }
@@ -799,15 +813,15 @@
         return areas
 
 
 class SegArea(Tool):
     r"""SegArea returns the area of the segmentation mask in pixels normalized to 2 decimal places."""
 
     name = "seg_area_"
-    description = "'seg_area_' returns the area of the segmentation mask in pixels normalized to 2 decimal places."
+    description = "'seg_area_' returns the area of the given segmentation mask in pixels normalized to 2 decimal places."
     usage = {
         "required_parameters": [{"name": "masks", "type": "str"}],
         "examples": [
             {
                 "scenario": "If you want to calculate the area of the segmentation mask, pass the masks file name.",
                 "parameters": {"masks": "mask_file.jpg"},
             },
@@ -879,15 +893,15 @@
         union = np.logical_or(np_mask1, np_mask2)
         iou = np.sum(intersection) / np.sum(union)
         return cast(float, round(iou, 2))
 
 
 class BboxContains(Tool):
     name = "bbox_contains_"
-    description = "Given two bounding boxes, a target bounding box and a region bounding box, 'bbox_contains_' returns the intersection of the two bounding boxes over the target bounding box, reflects the percentage area of the target bounding box overlaps with the region bounding box. This is a good tool for determining if the region object contains the target object."
+    description = "Given two bounding boxes, a target bounding box and a region bounding box, 'bbox_contains_' returns the intersection of the two bounding boxes which is the percentage area of the target bounding box overlaps with the region bounding box. This is a good tool for determining if the region object contains the target object."
     usage = {
         "required_parameters": [
             {"name": "target", "type": "List[int]"},
             {"name": "target_class", "type": "str"},
             {"name": "region", "type": "List[int]"},
             {"name": "region_class", "type": "str"},
         ],
@@ -931,25 +945,23 @@
             "region_class": region_class,
             "intersection": area,
         }
 
 
 class BoxDistance(Tool):
     name = "box_distance_"
-    description = (
-        "'box_distance_' returns the minimum distance between two bounding boxes."
-    )
+    description = "'box_distance_' calculates distance between two bounding boxes. It returns the minumum distance between the given bounding boxes"
     usage = {
         "required_parameters": [
             {"name": "bbox1", "type": "List[int]"},
             {"name": "bbox2", "type": "List[int]"},
         ],
         "examples": [
             {
-                "scenario": "If you want to calculate the distance between the bounding boxes [0.2, 0.21, 0.34, 0.42] and [0.3, 0.31, 0.44, 0.52]",
+                "scenario": "Calculate the distance between the bounding boxes [0.2, 0.21, 0.34, 0.42] and [0.3, 0.31, 0.44, 0.52]",
                 "parameters": {
                     "bbox1": [0.2, 0.21, 0.34, 0.42],
                     "bbox2": [0.3, 0.31, 0.44, 0.52],
                 },
             }
         ],
     }
@@ -1004,15 +1016,15 @@
                 Image.fromarray(frame).save(file_name)
             result.append((str(file_name), ts))
         return result
 
 
 class OCR(Tool):
     name = "ocr_"
-    description = "'ocr_' extracts text from an image."
+    description = "'ocr_' extracts text from an image. It returns a list of detected text, bounding boxes, and confidence scores."
     usage = {
         "required_parameters": [
             {"name": "image", "type": "str"},
         ],
         "examples": [
             {
                 "scenario": "Can you extract the text from this image? Image name: image.png",
```

### Comparing `vision_agent-0.2.8/vision_agent/tools/video.py` & `vision_agent-0.2.9/vision_agent/tools/video.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/vision_agent/type_defs.py` & `vision_agent-0.2.9/vision_agent/type_defs.py`

 * *Files identical despite different names*

### Comparing `vision_agent-0.2.8/PKG-INFO` & `vision_agent-0.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vision-agent
-Version: 0.2.8
+Version: 0.2.9
 Summary: Toolset for Vision Agent
 Author: Landing AI
 Author-email: dev@landing.ai
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

