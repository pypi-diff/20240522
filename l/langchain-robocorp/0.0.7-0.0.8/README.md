# Comparing `tmp/langchain_robocorp-0.0.7.tar.gz` & `tmp/langchain_robocorp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_robocorp-0.0.7.tar", max compression
+gzip compressed data, was "langchain_robocorp-0.0.8.tar", max compression
```

## Comparing `langchain_robocorp-0.0.7.tar` & `langchain_robocorp-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1072 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/LICENSE
--rw-r--r--   0        0        0      420 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/README.md
--rw-r--r--   0        0        0      102 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/__init__.py
--rw-r--r--   0        0        0     4568 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/_common.py
--rw-r--r--   0        0        0      525 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/_prompts.py
--rw-r--r--   0        0        0        0 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/py.typed
--rw-r--r--   0        0        0     7500 2024-05-15 21:31:05.494281 langchain_robocorp-0.0.7/langchain_robocorp/toolkits.py
--rw-r--r--   0        0        0     2558 2024-05-15 21:31:05.498281 langchain_robocorp-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/LICENSE
+-rw-r--r--   0        0        0      420 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/README.md
+-rw-r--r--   0        0        0      102 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/__init__.py
+-rw-r--r--   0        0        0     4568 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/_common.py
+-rw-r--r--   0        0        0      525 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/_prompts.py
+-rw-r--r--   0        0        0        0 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/py.typed
+-rw-r--r--   0        0        0     7675 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/langchain_robocorp/toolkits.py
+-rw-r--r--   0        0        0     2558 2024-05-22 16:53:16.582901 langchain_robocorp-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     1312 1970-01-01 00:00:00.000000 langchain_robocorp-0.0.8/PKG-INFO
```

### Comparing `langchain_robocorp-0.0.7/LICENSE` & `langchain_robocorp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.7/langchain_robocorp/_common.py` & `langchain_robocorp-0.0.8/langchain_robocorp/_common.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.7/langchain_robocorp/_prompts.py` & `langchain_robocorp-0.0.8/langchain_robocorp/_prompts.py`

 * *Files identical despite different names*

### Comparing `langchain_robocorp-0.0.7/langchain_robocorp/toolkits.py` & `langchain_robocorp-0.0.8/langchain_robocorp/toolkits.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,14 +99,16 @@
 class ActionServerToolkit(BaseModel):
     """Toolkit exposing Robocorp Action Server provided actions as individual tools."""
 
     url: str = Field(exclude=True)
     """Action Server URL"""
     api_key: str = Field(exclude=True, default="")
     """Action Server request API key"""
+    additional_headers: dict = Field(exclude=True, default_factory=dict)
+    """Additional headers to be passed to the Action Server"""
     report_trace: bool = Field(exclude=True, default=False)
     """Enable reporting Langsmith trace to Action Server runs"""
     _run_details: dict = PrivateAttr({})
 
     class Config:
         arbitrary_types_allowed = True
 
@@ -222,14 +224,15 @@
             **tools_args,
         )
 
     def _action_request(self, endpoint: str, **data: dict[str, Any]) -> str:
         headers = {
             "Authorization": f"Bearer {self.api_key}",
             "Content-Type": "application/json",
+            **self.additional_headers,
         }
 
         try:
             if self.report_trace and "run_id" in self._run_details:
                 client = Client()
                 run = client.read_run(self._run_details["run_id"])
                 if run.url:
```

### Comparing `langchain_robocorp-0.0.7/pyproject.toml` & `langchain_robocorp-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "langchain-robocorp"
-version = "0.0.7"
+version = "0.0.8"
 description = "An integration package connecting Robocorp Action Server and LangChain"
 authors = []
 readme = "README.md"
 repository = "https://github.com/langchain-ai/langchain"
 license = "MIT"
 
 [tool.poetry.urls]
```

### Comparing `langchain_robocorp-0.0.7/PKG-INFO` & `langchain_robocorp-0.0.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langchain-robocorp
-Version: 0.0.7
+Version: 0.0.8
 Summary: An integration package connecting Robocorp Action Server and LangChain
 Home-page: https://github.com/langchain-ai/langchain
 License: MIT
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

