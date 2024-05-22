# Comparing `tmp/composio_claude-0.2.60.tar.gz` & `tmp/composio_claude-0.2.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_claude-0.2.60.tar", last modified: Tue May 14 10:58:39 2024, max compression
+gzip compressed data, was "composio_claude-0.2.61.tar", last modified: Tue May 21 20:13:14 2024, max compression
```

## Comparing `composio_claude-0.2.60.tar` & `composio_claude-0.2.61.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:39.256373 composio_claude-0.2.60/
--rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-14 10:58:39.256124 composio_claude-0.2.60/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     2027 2024-05-13 07:27:09.000000 composio_claude-0.2.60/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:39.254687 composio_claude-0.2.60/composio_claude/
--rw-r--r--   0 sawradip   (501) staff       (20)      157 2024-05-13 07:27:09.000000 composio_claude-0.2.60/composio_claude/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     1658 2024-05-14 10:46:59.000000 composio_claude-0.2.60/composio_claude/claude_toolset.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-14 10:58:39.255763 composio_claude-0.2.60/composio_claude.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-14 10:58:39.000000 composio_claude-0.2.60/composio_claude.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      274 2024-05-14 10:58:39.000000 composio_claude-0.2.60/composio_claude.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-14 10:58:39.000000 composio_claude-0.2.60/composio_claude.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       43 2024-05-14 10:58:39.000000 composio_claude-0.2.60/composio_claude.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-14 10:58:39.000000 composio_claude-0.2.60/composio_claude.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-14 10:58:39.256421 composio_claude-0.2.60/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      847 2024-05-14 10:58:34.000000 composio_claude-0.2.60/setup.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:14.812900 composio_claude-0.2.61/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-21 20:13:14.812686 composio_claude-0.2.61/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)     2027 2024-05-16 15:09:06.000000 composio_claude-0.2.61/README.md
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:14.811639 composio_claude-0.2.61/composio_claude/
+-rw-r--r--   0 sawradip   (501) staff       (20)      158 2024-05-20 14:09:13.000000 composio_claude-0.2.61/composio_claude/__init__.py
+-rw-r--r--   0 sawradip   (501) staff       (20)     1519 2024-05-20 14:09:13.000000 composio_claude-0.2.61/composio_claude/claude_toolset.py
+drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:14.812443 composio_claude-0.2.61/composio_claude.egg-info/
+-rw-r--r--   0 sawradip   (501) staff       (20)     2561 2024-05-21 20:13:14.000000 composio_claude-0.2.61/composio_claude.egg-info/PKG-INFO
+-rw-r--r--   0 sawradip   (501) staff       (20)      274 2024-05-21 20:13:14.000000 composio_claude-0.2.61/composio_claude.egg-info/SOURCES.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:14.000000 composio_claude-0.2.61/composio_claude.egg-info/dependency_links.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       43 2024-05-21 20:13:14.000000 composio_claude-0.2.61/composio_claude.egg-info/requires.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-21 20:13:14.000000 composio_claude-0.2.61/composio_claude.egg-info/top_level.txt
+-rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:14.812943 composio_claude-0.2.61/setup.cfg
+-rw-r--r--   0 sawradip   (501) staff       (20)      825 2024-05-21 20:12:30.000000 composio_claude-0.2.61/setup.py
```

### Comparing `composio_claude-0.2.60/PKG-INFO` & `composio_claude-0.2.61/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.60
+Requires-Dist: composio_openai===0.2.61
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.60/README.md` & `composio_claude-0.2.61/README.md`

 * *Files identical despite different names*

### Comparing `composio_claude-0.2.60/composio_claude/claude_toolset.py` & `composio_claude-0.2.61/composio_claude/claude_toolset.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,50 @@
+from anthropic.types.beta.tools import ToolUseBlock, ToolsBetaMessage
+from composio_openai import OpenaiStyleToolsetBase
 
-import json
-from json.decoder import JSONDecoder
 from composio import FrameworkEnum
 from composio.sdk import SchemaFormat
-from composio_openai import OpenaiStyleToolsetBase
 
-from anthropic.types.beta.tools import ToolUseBlock, ToolsBetaMessage
-        
+
 class ComposioToolset(OpenaiStyleToolsetBase):
-    def __init__(self, *args, framework=FrameworkEnum.CLAUDE, schema_format = SchemaFormat.CLAUDE, **kwargs):
-        super().__init__(*args, framework=framework, schema_format=schema_format, **kwargs)
-    
-    
-    def handle_tool_calls(self,
-                          llm_response: ToolsBetaMessage, 
-                          entity_id: str = "default") -> list[any]:
-        outputs = []        
+    def __init__(
+        self,
+        *args,
+        framework=FrameworkEnum.CLAUDE,
+        schema_format=SchemaFormat.CLAUDE,
+        **kwargs
+    ):
+        super().__init__(
+            *args, framework=framework, schema_format=schema_format, **kwargs
+        )
+
+    def handle_tool_calls(
+        self, llm_response: ToolsBetaMessage, entity_id: str = "default"
+    ) -> list[any]:
+        outputs = []
         # entity = self.client.sdk.get_entity(entity_id)
         entity_id = self.finalize_entity_id(entity_id)
-        
+
         for content in llm_response.content:
             if isinstance(content, ToolUseBlock):
                 action_name_to_execute = content.name
                 arguments = content.input
 
-
                 action = self.client.sdk.get_action_enum_without_tool(
                     action_name=action_name_to_execute
                 )
-                # account = entity.get_connection(app_name=action.service)
                 output = self.client.execute_action(action, arguments, entity_id)
                 outputs.append(output)
         if outputs == []:
             print("No tool call present in Claude Response")
 
         return outputs
-    
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     from pprint import pprint
+
     from composio import App
-    
+
     toolset = ComposioToolset()
     out = toolset.get_tools(tools=App.GITHUB)
     pprint(out)
```

### Comparing `composio_claude-0.2.60/composio_claude.egg-info/PKG-INFO` & `composio_claude-0.2.61/composio_claude.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_claude
-Version: 0.2.60
+Version: 0.2.61
 Summary: Use Composio to get an array of tools with your Claude LLMs.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_openai===0.2.60
+Requires-Dist: composio_openai===0.2.61
 Requires-Dist: anthropic>=0.25.7
 
 ## 🚀🔗 Leveraging Claude with Composio
 
 Facilitate the integration of Claude with Composio to empower Claude models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_claude-0.2.60/setup.py` & `composio_claude-0.2.61/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,26 +5,23 @@
 from pathlib import Path
 
 from setuptools import setup
 
 
 setup(
     name="composio_claude",
-    version="0.2.60",
+    version="0.2.61",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Claude LLMs.",
     long_description=(Path(__file__).parent / "README.md").read_text(encoding="utf-8"),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9,<4",
-    install_requires=[
-        "composio_openai===0.2.60",
-        "anthropic>=0.25.7"
-    ],
+    install_requires=["composio_openai===0.2.61", "anthropic>=0.25.7"],
     include_package_data=True,
 )
```

