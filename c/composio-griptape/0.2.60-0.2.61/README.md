# Comparing `tmp/composio_griptape-0.2.60.tar.gz` & `tmp/composio_griptape-0.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_griptape-0.2.60.tar", last modified: Tue May 14 10:58:43 2024, max compression
+gzip compressed data, was "composio_griptape-0.2.61.tar", last modified: Tue May 21 20:13:19 2024, max compression
```

## Comparing `composio_griptape-0.2.60.tar` & `composio_griptape-0.2.61.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.163425 composio_griptape-0.2.60/
--rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-14 10:58:43.163194 composio_griptape-0.2.60/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     1851 2024-05-13 07:27:09.000000 composio_griptape-0.2.60/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.161930 composio_griptape-0.2.60/composio_griptape/
--rw-r--r--   0 sawradip   (501) staff       (20)      161 2024-05-13 07:27:09.000000 composio_griptape-0.2.60/composio_griptape/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     5395 2024-05-14 10:49:45.000000 composio_griptape-0.2.60/composio_griptape/griptape_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:43.162954 composio_griptape-0.2.60/composio_griptape.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      291 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       40 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       18 2024-05-14 10:58:43.000000 composio_griptape-0.2.60/composio_griptape.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:43.163473 composio_griptape-0.2.60/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      853 2024-05-14 10:58:34.000000 composio_griptape-0.2.60/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:19.609948 composio_griptape-0.2.61/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-21 20:13:19.609703 composio_griptape-0.2.61/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     1851 2024-05-16 15:09:06.000000 composio_griptape-0.2.61/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:19.608555 composio_griptape-0.2.61/composio_griptape/
+-rw-r--r--   0 sawradip   (501) staff       (20)      161 2024-05-16 15:09:06.000000 composio_griptape-0.2.61/composio_griptape/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     5101 2024-05-20 14:09:13.000000 composio_griptape-0.2.61/composio_griptape/griptape_toolspec.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:19.609454 composio_griptape-0.2.61/composio_griptape.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2389 2024-05-21 20:13:19.000000 composio_griptape-0.2.61/composio_griptape.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      291 2024-05-21 20:13:19.000000 composio_griptape-0.2.61/composio_griptape.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:19.000000 composio_griptape-0.2.61/composio_griptape.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       40 2024-05-21 20:13:19.000000 composio_griptape-0.2.61/composio_griptape.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       18 2024-05-21 20:13:19.000000 composio_griptape-0.2.61/composio_griptape.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:19.609985 composio_griptape-0.2.61/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      831 2024-05-21 20:12:30.000000 composio_griptape-0.2.61/setup.py
```

### Comparing `composio_griptape-0.2.60/PKG-INFO` & `composio_griptape-0.2.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.60
+Requires-Dist: composio_core===0.2.61
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

### Comparing `composio_griptape-0.2.60/README.md` & `composio_griptape-0.2.61/README.md`

 * *Files identical despite different names*

### Comparing `composio_griptape-0.2.60/composio_griptape/griptape_toolspec.py` & `composio_griptape-0.2.61/composio_griptape/griptape_toolspec.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,123 +1,120 @@
-import os
 import logging
+import os
 from typing import List, Union
-from schema import Schema, Literal
+
 from griptape.tools import BaseTool
 from griptape.utils.decorators import activity
-from griptape.artifacts import BaseArtifact
+from schema import Literal, Schema
 
-from composio.sdk import SchemaFormat
-from composio.sdk.shared_utils import schema_type_python_type_dict
 from composio import Action, App, ComposioCore, FrameworkEnum, Tag
+from composio.sdk.shared_utils import schema_type_python_type_dict
+
 
 logger = logging.getLogger(__name__)
 
 
 class ComposioToolset:
-    def __init__(self, framework = FrameworkEnum.GRIPTAPE, entity_id: str = "default"):
+    def __init__(self, framework=FrameworkEnum.GRIPTAPE, entity_id: str = "default"):
         self.entity_id = entity_id
         self.client = ComposioCore(
-                            framework=framework, api_key=os.environ.get("COMPOSIO_API_KEY", None)
-                            )
+            framework=framework, api_key=os.environ.get("COMPOSIO_API_KEY", None)
+        )
 
     def get_actions(self, actions: Union[Action, List[Action]]):
         if isinstance(actions, Action):
             actions = [actions]
-        
+
         action_schemas = self.client.sdk.get_list_of_actions(actions=actions)
-        
 
-        formatted_schemas = [self.action_schema_to_griptape(action_schema)() 
-                             for action_schema in action_schemas]
+        formatted_schemas = [
+            self.action_schema_to_griptape(action_schema)()
+            for action_schema in action_schemas
+        ]
         return formatted_schemas
-    
-    def get_tools(self, 
-        tools: Union[App, List[App]],
-        tags: List[Union[str, Tag]] = None):
+
+    def get_tools(
+        self, tools: Union[App, List[App]], tags: List[Union[str, Tag]] = None
+    ):
         if isinstance(tools, App):
             tools = [tools]
-        
-        action_schemas = self.client.sdk.get_list_of_actions(apps=tools, 
-                                                             tags=tags)
-        formatted_schemas = [self.action_schema_to_griptape(action_schema)() 
-                             for action_schema in action_schemas]
+
+        action_schemas = self.client.sdk.get_list_of_actions(apps=tools, tags=tags)
+        formatted_schemas = [
+            self.action_schema_to_griptape(action_schema)()
+            for action_schema in action_schemas
+        ]
         return formatted_schemas
-    
-    def action_schema_to_griptape(self, action_schema):
 
+    def action_schema_to_griptape(self, action_schema):
         schema_dict = {}
         name = action_schema["name"]
         appName = action_schema["appName"]
         description = action_schema["description"]
 
         for param_name, param_body in action_schema["parameters"]["properties"].items():
-            description =param_body["description"] 
+            description = param_body["description"]
             dtype = param_body["type"]
 
             schema_key = Literal(param_name, description=description)
             if dtype in schema_type_python_type_dict:
                 schema_dtype = schema_type_python_type_dict.get(dtype)
             elif dtype == "array":
-                schema_array_dtype = schema_type_python_type_dict.get(param_body["items"].get("type"), None)
+                schema_array_dtype = schema_type_python_type_dict.get(
+                    param_body["items"].get("type"), None
+                )
                 schema_dtype = list[schema_array_dtype] if schema_array_dtype else list
             else:
-                raise TypeError(f"Some dtype of current schema are not handled yet. Current Schema: {param_body}")
-            
+                raise TypeError(
+                    f"Some dtype of current schema are not handled yet. Current Schema: {param_body}"
+                )
+
             schema_dict[schema_key] = schema_dtype
 
         griptape_activity_config = {
             "description": description,
             "schema": Schema(schema_dict),
         }
 
         class tool_class(BaseTool):
-            @activity(
-                config=griptape_activity_config
-            )
+            @activity(config=griptape_activity_config)
             def execute_task(nested_self, params: dict):
-                # print(params)
                 params_dict = params["values"]
                 return self.client.execute_action(
-                            self.client.get_action_enum(name, appName), 
-                            params_dict, 
-                            entity_id= self.entity_id
-                        )
-            
+                    self.client.get_action_enum(name, appName),
+                    params_dict,
+                    entity_id=self.entity_id,
+                )
+
             @property
             def manifest(self) -> dict:
                 return {
-                    'version': 'v1',
-                    'name': name,
-                    'description': description,
-                    'contact_email': 'hello@composio.dev',
-                    'legal_info_url': 'https://www.composio.dev/legal'
-                    }
+                    "version": "v1",
+                    "name": name,
+                    "description": description,
+                    "contact_email": "hello@composio.dev",
+                    "legal_info_url": "https://www.composio.dev/legal",
+                }
 
         griptape_tool_class = type(f"{name}_client", (tool_class,), {})
 
         # setattr(griptape_tool_class, 'execute_task', execute_task)
         # setattr(griptape_tool_class, 'manifest', manifest)
 
         return griptape_tool_class
 
 
-
-    
-
-        
-        
 # class ComposioToolset(OpenaiStyleToolsetBase):
 #     def __init__(self, *args, framework=FrameworkEnum.OPENAI, **kwargs):
 #         super().__init__(*args, framework=framework, **kwargs)
 
 #     def handle_tool_calls(self,
-#                           llm_response: ChatCompletion, 
+#                           llm_response: ChatCompletion,
 #                           entity_id: str = "default") -> list[any]:
-#         output = []        
+#         output = []
 #         entity = self.client.sdk.get_entity(entity_id)
 #         try:
 #             if llm_response.choices:
 #                 for choice in llm_response.choices:
 #                     if choice.message.tool_calls:
 #                         for tool_call in choice.message.tool_calls:
 #                             action_name_to_execute = tool_call.function.name
@@ -129,13 +126,13 @@
 #                             output.append(account.execute_action(action, arguments))
 
 #         except Exception as e:
 #             raise e from e
 
 #         return output
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from pprint import pprint
-    
+
     toolset = ComposioToolset()
     out = toolset.get_tools(tools=App.GITHUB)
     pprint(out)
```

### Comparing `composio_griptape-0.2.60/composio_griptape.egg-info/PKG-INFO` & `composio_griptape-0.2.61/composio_griptape.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_griptape
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Griptape wokflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.60
+Requires-Dist: composio_core===0.2.61
 Requires-Dist: griptape>=0.24.2
 
 ## 🚀🔗 Integrating Composio with Griptape
 
 Streamline the integration of Composio within the Griptape agentic framework to enhance the interaction capabilities of Griptape agents with external applications, significantly extending their operational range and efficiency.
 
 ### Objective
```

