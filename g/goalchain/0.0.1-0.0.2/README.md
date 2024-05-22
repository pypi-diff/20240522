# Comparing `tmp/goalchain-0.0.1.tar.gz` & `tmp/goalchain-0.0.2.tar.gz`

## Comparing `goalchain-0.0.1.tar` & `goalchain-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 goalchain-0.0.1/src/goalchain/__init__.py
--rw-r--r--   0        0        0    11792 2020-02-02 00:00:00.000000 goalchain-0.0.1/src/goalchain/goalchain.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 goalchain-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 goalchain-0.0.1/LICENSE
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 goalchain-0.0.1/README.md
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 goalchain-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 goalchain-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      210 2020-02-02 00:00:00.000000 goalchain-0.0.2/src/goalchain/__init__.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 goalchain-0.0.2/src/goalchain/goalchain.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 goalchain-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 goalchain-0.0.2/LICENSE
+-rw-r--r--   0        0        0    13340 2020-02-02 00:00:00.000000 goalchain-0.0.2/README.md
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 goalchain-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    14458 2020-02-02 00:00:00.000000 goalchain-0.0.2/PKG-INFO
```

### Comparing `goalchain-0.0.1/src/goalchain/goalchain.py` & `goalchain-0.0.2/src/goalchain/goalchain.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,27 +37,29 @@
     def __init__(self,
                  label,
                  goal,
                  opener, 
                  out_of_scope=None, 
                  confirm=True, 
                  model="gpt-4-1106-preview", 
-                 json_model="gpt-4-1106-preview"):
+                 json_model="gpt-4-1106-preview",
+                 params = {}):
         self.label = label
         self.goal = goal
         self.opener = opener
         self.confirm = confirm
         self.out_of_scope = out_of_scope
         self.model = model
         self.json_model = json_model
         self.messages = []
         self.connected_goals = []
         self.completed_string = "completed"
         self.hand_over = False    
         self.completed = False
+        self.params = params
         
         self.goal_prompt = Prompt("""Your role is to continue the conversation below as the Assistant.
 Goal: {{goal}}
 {% if information_list %}
 Information to be gathered: {{information_list|join(", ")}}
 This is all of the information you are to gather, do not ask for anything else.
 {% if confirmation %}
@@ -172,15 +174,20 @@
         ]
         if json_mode:
             response_format = {"type": "json_object"}
             model = self.json_model
         else:
             response_format = None
             model = self.model
-        llm_response = completion(messages=llm_messages, model=model, response_format=response_format)
+        llm_response = completion(
+            messages=llm_messages,
+            model=model, 
+            response_format=response_format,
+            **self.params
+        )
         llm_response_text = llm_response["choices"][0]["message"]["content"]
         return llm_response_text
     
     def simulate_response(self, response, rephrase = False, message_history = []):
         if rephrase:
             rephrase_details = {
                 "response": response,
```

### Comparing `goalchain-0.0.1/.gitignore` & `goalchain-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `goalchain-0.0.1/LICENSE` & `goalchain-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `goalchain-0.0.1/pyproject.toml` & `goalchain-0.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "goalchain"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   {name="Adrian Lucas Malec", email="dr.adrian@gmail.com"},
 ]
 description = "GoalChain is a simple but effective framework for enabling goal-orientated conversation flows for human-LLM and LLM-LLM interaction."
 readme = "README.md"
 requires-python = ">=3.9"
 license = {text="MIT"}
```

