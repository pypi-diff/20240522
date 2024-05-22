# Comparing `tmp/handyllm-0.7.2.tar.gz` & `tmp/handyllm-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "handyllm-0.7.2.tar", last modified: Mon May 20 09:17:42 2024, max compression
+gzip compressed data, was "handyllm-0.7.3.tar", last modified: Wed May 22 07:29:13 2024, max compression
```

## Comparing `handyllm-0.7.2.tar` & `handyllm-0.7.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-20 09:17:32.000000 handyllm-0.7.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 09:17:42.248525 handyllm-0.7.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-20 09:17:32.000000 handyllm-0.7.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-05-20 09:17:32.000000 handyllm-0.7.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 09:17:42.248525 handyllm-0.7.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.244525 handyllm-0.7.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/HandyLLM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2867 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 09:17:42.000000 handyllm-0.7.2/src/HandyLLM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/handyllm/
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_str_enum.py
--rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/src/handyllm/deprecated/
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/deprecated/api_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/deprecated/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/endpoint_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    32490 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/openai_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/openai_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7544 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/prompt_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/requestor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-20 09:17:32.000000 handyllm-0.7.2/src/handyllm/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 09:17:42.248525 handyllm-0.7.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_azure.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_client_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_hprompt.py
--rw-r--r--   0 runner    (1001) docker     (127)      842 2024-05-20 09:17:32.000000 handyllm-0.7.2/tests/test_prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.528764 handyllm-0.7.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-22 07:29:06.000000 handyllm-0.7.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-22 07:29:13.528764 handyllm-0.7.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-22 07:29:06.000000 handyllm-0.7.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 07:29:06.000000 handyllm-0.7.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:29:13.528764 handyllm-0.7.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.520764 handyllm-0.7.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.524764 handyllm-0.7.3/src/HandyLLM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 07:29:13.000000 handyllm-0.7.3/src/HandyLLM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.524764 handyllm-0.7.3/src/handyllm/
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      143 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      637 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/_str_enum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8549 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2757 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.524764 handyllm-0.7.3/src/handyllm/deprecated/
+-rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/deprecated/api_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14098 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/deprecated/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/endpoint_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32522 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3880 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/openai_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15434 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/openai_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7384 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/prompt_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11059 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/requestor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3695 2024-05-22 07:29:06.000000 handyllm-0.7.3/src/handyllm/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:29:13.524764 handyllm-0.7.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-05-22 07:29:06.000000 handyllm-0.7.3/tests/test_azure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-05-22 07:29:06.000000 handyllm-0.7.3/tests/test_client_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2296 2024-05-22 07:29:06.000000 handyllm-0.7.3/tests/test_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-22 07:29:06.000000 handyllm-0.7.3/tests/test_hprompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 07:29:06.000000 handyllm-0.7.3/tests/test_prompt.py
```

### Comparing `handyllm-0.7.2/LICENSE` & `handyllm-0.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/PKG-INFO` & `handyllm-0.7.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.2
+Version: 0.7.3
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: python-frontmatter
```

### Comparing `handyllm-0.7.2/README.md` & `handyllm-0.7.3/README.md`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/pyproject.toml` & `handyllm-0.7.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HandyLLM"
-version = "0.7.2"
+version = "0.7.3"
 authors = [
   { name="Atomie CHEN", email="atomic_cwh@163.com" },
 ]
 description = "A handy toolkit for using LLM."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
-    # "License :: OSI Approved :: MIT License",
+    "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 keywords = ["LLM", "Large Language Model", "Prompt", "OpenAI", "API"]
 dependencies = [
   "requests",
   "httpx",
   "python-frontmatter",
```

### Comparing `handyllm-0.7.2/src/HandyLLM.egg-info/PKG-INFO` & `handyllm-0.7.3/src/HandyLLM.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: HandyLLM
-Version: 0.7.2
+Version: 0.7.3
 Summary: A handy toolkit for using LLM.
 Author-email: Atomie CHEN <atomic_cwh@163.com>
 Project-URL: Homepage, https://github.com/atomiechen/HandyLLM
 Project-URL: Bug Tracker, https://github.com/atomiechen/HandyLLM/issues
 Keywords: LLM,Large Language Model,Prompt,OpenAI,API
 Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: httpx
 Requires-Dist: python-frontmatter
```

### Comparing `handyllm-0.7.2/src/HandyLLM.egg-info/SOURCES.txt` & `handyllm-0.7.3/src/HandyLLM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/_str_enum.py` & `handyllm-0.7.3/src/handyllm/_str_enum.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/_utils.py` & `handyllm-0.7.3/src/handyllm/_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,17 +76,17 @@
     if exception.args:
         print(f"\nException arguments: {exception.args}")
     return err_msg
 
 def _chat_log_response_final(logger, log_marks, kwargs, messages, start_time, role, content, err_msg=None):
     end_time = time.perf_counter()
     duration = end_time - start_time
-    input_content = PromptConverter.chat2raw(messages)
+    input_content = PromptConverter.msgs2raw(messages)
     if not err_msg:
-        output_content = PromptConverter.chat2raw([{'role': role, 'content': content}])
+        output_content = PromptConverter.msgs2raw([{'role': role, 'content': content}])
         log_result(logger, "Chat request", duration, log_marks, kwargs, input_content, output_content)
     else:
         log_exception(logger, "Chat request", duration, log_marks, kwargs, input_content, err_msg)
 
 def _chat_log_response(logger, log_marks, kwargs, messages, start_time, response, stream):
     if logger is not None:
         if stream:
@@ -133,15 +133,15 @@
             _chat_log_response_final(logger, log_marks, kwargs, messages, start_time, role, content, err_msg)
     return response
 
 def _chat_log_exception(logger, log_marks, kwargs, messages, start_time, exception: Exception):
     if logger is not None:
         end_time = time.perf_counter()
         duration = end_time - start_time
-        input_content = PromptConverter.chat2raw(messages)
+        input_content = PromptConverter.msgs2raw(messages)
         err_msg = exception2err_msg(exception)
         log_exception(logger, "Chat request", duration, log_marks, kwargs, input_content, err_msg)
 
 def _completions_log_response_final(logger, log_marks, kwargs, prompt, start_time, text, err_msg=None):
     end_time = time.perf_counter()
     duration = end_time - start_time
     input_content = prompt
```

### Comparing `handyllm-0.7.2/src/handyllm/deprecated/api_request.py` & `handyllm-0.7.3/src/handyllm/deprecated/api_request.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/deprecated/openai_api.py` & `handyllm-0.7.3/src/handyllm/deprecated/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/endpoint_manager.py` & `handyllm-0.7.3/src/handyllm/endpoint_manager.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/hprompt.py` & `handyllm-0.7.3/src/handyllm/hprompt.py`

 * *Files 8% similar despite different names*

```diff
@@ -39,15 +39,18 @@
     astream_chat_all, astream_completions, 
     stream_chat_all, stream_completions, 
 )
 from ._str_enum import AutoStrEnum
 
 
 PromptType = TypeVar('PromptType', bound='HandyPrompt')
-PathType = Union[str, os.PathLike[str]]
+if sys.version_info >= (3, 9):
+    PathType = Union[str, os.PathLike[str]]
+else:
+    PathType = Union[str, os.PathLike]
 
 converter = PromptConverter()
 handler = frontmatter.YAMLHandler()
 p_var_map = re.compile(r'(%\w+%)')
 
 DEFAULT_BLACKLIST = (
     "api_key", "organization", "api_base", "api_type", "api_version", 
@@ -80,16 +83,16 @@
         if converter.detect(content):
             api = "chat"
         else:
             api = "completions"
     if api == "completions":
         return CompletionsPrompt(content, request, meta, base_path)
     else:
-        chat = converter.raw2chat(content)
-        return ChatPrompt(chat, request, meta, base_path)
+        messages = converter.raw2msgs(content)
+        return ChatPrompt(messages, request, meta, base_path)
 
 def load(
     fd: io.IOBase, 
     encoding: str = "utf-8",
     base_path: Optional[PathType] = None
 ) -> HandyPrompt:
     text = fd.read()
@@ -554,71 +557,71 @@
             )
         return var_map
 
 
 class ChatPrompt(HandyPrompt):
         
     def __init__(
-        self, chat: list, request: dict, meta: Union[dict, RunConfig], 
+        self, messages: list, request: dict, meta: Union[dict, RunConfig], 
         base_path: Optional[PathType] = None,
         response: Optional[dict] = None,
         ):
-        super().__init__(chat, request, meta, base_path, response)
+        super().__init__(messages, request, meta, base_path, response)
     
     @property
-    def chat(self) -> list:
+    def messages(self) -> list:
         return self.data
     
-    @chat.setter
-    def chat(self, value: list):
+    @messages.setter
+    def messages(self, value: list):
         self.data = value
     
     @property
     def result_str(self) -> str:
-        if len(self.chat) == 0:
+        if len(self.messages) == 0:
             return ""
-        return self.chat[-1]['content']
+        return self.messages[-1]['content']
     
     def _serialize_data(self, data) -> str:
-        return converter.chat2raw(data)
+        return converter.msgs2raw(data)
     
     def _eval_data(self, run_config: RunConfig) -> list:
         var_map = self._parse_var_map(run_config)
         if var_map:
-            return converter.chat_replace_variables(
-                self.chat, var_map, inplace=False)
+            return converter.msgs_replace_variables(
+                self.messages, var_map, inplace=False)
         else:
-            return self.chat
+            return self.messages
     
     def _run_with_client(
         self, client: OpenAIClient, 
         run_config: RunConfig,
         new_request: dict,
         stream: bool,
         ) -> ChatPrompt:
         response = client.chat(
             messages=self._eval_data(run_config),
             **new_request
             ).call()
         new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
-            if run_config.output_path:
+            if run_config.output_fd:
+                # dump frontmatter, no base_path
+                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                # stream response to a file descriptor
+                role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), run_config.output_fd)
+            elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     # dump frontmatter
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response), fout)
-            elif run_config.output_fd:
-                # dump frontmatter, no base_path
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                # stream response to a file descriptor
-                role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response), run_config.output_fd)
+                    role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response), fout)
             else:
-                role, content, tool_calls = converter.stream_chat2raw(stream_chat_all(response))
+                role, content, tool_calls = converter.stream_msgs2raw(stream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
             [{"role": role, "content": content, "tool_calls": tool_calls}],
             new_request, run_config, base_path,
@@ -634,70 +637,70 @@
         response = await client.chat(
             messages=self._eval_data(run_config),
             **new_request
             ).acall()
         new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
-            if run_config.output_path:
+            if run_config.output_fd:
+                # stream response to a file descriptor
+                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), run_config.output_fd)
+            elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
-                    role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response), fout)
-            elif run_config.output_fd:
-                # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response), run_config.output_fd)
+                    role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response), fout)
             else:
-                role, content, tool_calls = await converter.astream_chat2raw(astream_chat_all(response))
+                role, content, tool_calls = await converter.astream_msgs2raw(astream_chat_all(response))
         else:
             role = response['choices'][0]['message']['role']
             content = response['choices'][0]['message'].get('content')
             tool_calls = response['choices'][0]['message'].get('tool_calls')
         return ChatPrompt(
             [{"role": role, "content": content, "tool_calls": tool_calls}],
             new_request, run_config, base_path,
             response=response
         )
 
     def __add__(self, other: Union[str, list, ChatPrompt]):
         # support concatenation with string, list or another ChatPrompt
         if isinstance(other, str):
             return ChatPrompt(
-                self.chat + [{"role": "user", "content": other}],
+                self.messages + [{"role": "user", "content": other}],
                 copy.deepcopy(self.request),
                 replace(self.run_config),
                 self.base_path
             )
         elif isinstance(other, list):
             return ChatPrompt(
-                self.chat + [{"role": msg['role'], "content": msg['content']} for msg in other],
+                self.messages + other,
                 copy.deepcopy(self.request),
                 replace(self.run_config),
                 self.base_path
             )
         elif isinstance(other, ChatPrompt):
             # merge two ChatPrompt objects
             merged_request, merged_run_config = self._merge_non_data(other)
             return ChatPrompt(
-                self.chat + other.chat, merged_request, merged_run_config, 
+                self.messages + other.messages, merged_request, merged_run_config, 
                 self.base_path
             )
         else:
             raise TypeError(f"unsupported operand type(s) for +: 'ChatPrompt' and '{type(other)}'")
     
     def __iadd__(self, other: Union[str, list, ChatPrompt]):
         # support concatenation with string, list or another ChatPrompt
         if isinstance(other, str):
-            self.chat.append({"role": "user", "content": other})
+            self.messages.append({"role": "user", "content": other})
         elif isinstance(other, list):
-            self.chat += [{"role": msg['role'], "content": msg['content']} for msg in other]
+            self.messages += other
         elif isinstance(other, ChatPrompt):
             # merge two ChatPrompt objects
-            self.chat += other.chat
+            self.messages += other.messages
             self._merge_non_data(other, inplace=True)
         else:
             raise TypeError(f"unsupported operand type(s) for +: 'ChatPrompt' and '{type(other)}'")
         return self
 
 
 class CompletionsPrompt(HandyPrompt):
@@ -745,23 +748,23 @@
         response = client.completions(
             prompt=self._eval_data(run_config),
             **new_request
             ).call()
         new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
-            if run_config.output_path:
+            if run_config.output_fd:
+                # stream response to a file descriptor
+                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                content = self._stream_completions_proc(response, run_config.output_fd)
+            elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
                     content = self._stream_completions_proc(response, fout)
-            elif run_config.output_fd:
-                # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                content = self._stream_completions_proc(response, run_config.output_fd)
             else:
                 content = self._stream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
@@ -784,23 +787,23 @@
         response = await client.completions(
             prompt=self._eval_data(run_config),
             **new_request
             ).acall()
         new_request = self._filter_request(new_request, run_config)
         base_path = Path(run_config.output_path).parent.resolve() if run_config.output_path else None
         if stream:
-            if run_config.output_path:
+            if run_config.output_fd:
+                # stream response to a file descriptor
+                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
+                content = await self._astream_completions_proc(response, run_config.output_fd)
+            elif run_config.output_path:
                 # stream response to a file
                 with open(run_config.output_path, 'w', encoding='utf-8') as fout:
                     fout.write(self._dumps_frontmatter(new_request, run_config, base_path))
                     content = await self._astream_completions_proc(response, fout)
-            elif run_config.output_fd:
-                # stream response to a file descriptor
-                run_config.output_fd.write(self._dumps_frontmatter(new_request, run_config))
-                content = await self._astream_completions_proc(response, run_config.output_fd)
             else:
                 content = await self._astream_completions_proc(response)
         else:
             content = response['choices'][0]['text']
         return CompletionsPrompt(
             content, new_request, run_config, base_path, response=response
             )
```

### Comparing `handyllm-0.7.2/src/handyllm/openai_api.py` & `handyllm-0.7.3/src/handyllm/openai_api.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/openai_client.py` & `handyllm-0.7.3/src/handyllm/openai_client.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/prompt_converter.py` & `handyllm-0.7.3/src/handyllm/prompt_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import io
 import re
-from typing import Optional
+from typing import Optional, Tuple
 import yaml
 
 
 class PromptConverter:
     
     role_keys = ['system', 'user', 'assistant', 'tool']
 
@@ -31,21 +31,21 @@
         self.substitute_map = {}
         blocks = re.split(r'(%\w+%)', content)
         for idx in range(1, len(blocks), 2):
             key = blocks[idx]
             value = blocks[idx+1]
             self.substitute_map[key] = value.strip()
 
-    def raw2chat(self, raw_prompt: str):
+    def raw2msgs(self, raw_prompt: str):
         # substitute pre-defined variables
         for key, value in self.substitute_map.items():
             raw_prompt = raw_prompt.replace(key, value)
 
-        # convert plain text to chat format
-        chat = []
+        # convert plain text to messages format
+        msgs = []
         blocks = re.split(self.split_pattern, raw_prompt, flags=re.MULTILINE)
         for idx in range(1, len(blocks), 3):
             role = blocks[idx]
             extra = blocks[idx+1]
             content = blocks[idx+2]
             if content:
                 content = content.strip()
@@ -64,29 +64,29 @@
                         msg['tool_calls'] = yaml.safe_load(content)
                         msg['content'] = None
                     elif type_of_msg == 'content_array':
                         # parse content array
                         msg['content'] = yaml.safe_load(content)
                 for key in extra_properties:
                     msg[key] = extra_properties[key]
-            chat.append(msg)
+            msgs.append(msg)
         
-        return chat
+        return msgs
     
-    def rawfile2chat(self, raw_prompt_path: str):
+    def rawfile2msgs(self, raw_prompt_path: str):
         with open(raw_prompt_path, 'r', encoding='utf-8') as fin:
             raw_prompt = fin.read()
         
-        return self.raw2chat(raw_prompt)
+        return self.raw2msgs(raw_prompt)
     
     @staticmethod
-    def chat2raw(chat):
-        # convert chat format to plain text
+    def msgs2raw(msgs):
+        # convert messages format to plain text
         messages = []
-        for message in chat:
+        for message in msgs:
             role = message.get('role')
             content = message.get('content')
             tool_calls = message.get('tool_calls')
             extra_properties = {key: message[key] for key in message if key not in ['role', 'content', 'tool_calls']}
             if tool_calls:
                 extra_properties['type'] = 'tool_calls'
                 content = yaml.dump(tool_calls)
@@ -98,15 +98,15 @@
             else:
                 extra = ""
             messages.append(f"${role}${extra}\n{content}")
         raw_prompt = "\n\n".join(messages)
         return raw_prompt
 
     @staticmethod
-    def stream_chat2raw(gen_sync, fd: Optional[io.IOBase] = None) -> tuple[str, str]:
+    def stream_msgs2raw(gen_sync, fd: Optional[io.IOBase] = None) -> Tuple[str, str]:
         # stream response to fd
         role = ""
         content = ""
         tool_calls = []
         role_completed = False
         for r, text, tool_call in gen_sync:
             if r != role:
@@ -129,15 +129,15 @@
                 content += text
         if tool_calls and fd:
             # dump tool calls
             fd.write(yaml.dump(tool_calls))
         return role, content, tool_calls
 
     @staticmethod
-    async def astream_chat2raw(gen_async, fd: Optional[io.IOBase] = None) -> tuple[str, str]:
+    async def astream_msgs2raw(gen_async, fd: Optional[io.IOBase] = None) -> Tuple[str, str]:
         # stream response to fd
         role = ""
         content = ""
         tool_calls = []
         role_completed = False
         async for r, text, tool_call in gen_async:
             if r != role:
@@ -160,40 +160,36 @@
                 content += text
         if tool_calls and fd:
             # dump tool calls
             fd.write(yaml.dump(tool_calls))
         return role, content, tool_calls
     
     @classmethod
-    def chat2rawfile(cls, chat, raw_prompt_path: str):
-        raw_prompt = cls.chat2raw(chat)
+    def msgs2rawfile(cls, msgs, raw_prompt_path: str):
+        raw_prompt = cls.msgs2raw(msgs)
         with open(raw_prompt_path, 'w', encoding='utf-8') as fout:
             fout.write(raw_prompt)
     
     @staticmethod
-    def chat_replace_variables(chat, variable_map: dict, inplace=False):
-        # replace every variable in chat content
+    def msgs_replace_variables(msgs, variable_map: dict, inplace=False):
+        # replace every variable in messages content
         if inplace:
-            for message in chat:
+            for message in msgs:
                 for var, value in variable_map.items():
                     if message.get('content') and var in message['content']:
                         message['content'] = message['content'].replace(var, value)
-            return chat
+            return msgs
         else:
-            new_chat = []
-            for message in chat:
+            new_msgs = []
+            for message in msgs:
                 new_message = message.copy()
                 for var, value in variable_map.items():
                     if new_message.get('content') and var in new_message['content']:
                         new_message['content'] = new_message['content'].replace(var, value)
-                new_chat.append(new_message)
-            return new_chat
+                new_msgs.append(new_message)
+            return new_msgs
     
-    @staticmethod
-    def chat_append_msg(chat, content: str, role: str = 'user', inplace=False):
-        if inplace:
-            chat.append({"role": role, "content": content})
-            return chat
-        else:
-            new_chat = chat.copy()
-            new_chat.append({"role": role, "content": content})
-            return new_chat
+    raw2chat = raw2msgs
+    rawfile2chat = rawfile2msgs
+    chat2raw = msgs2raw
+    chat2rawfile = msgs2rawfile
+    chat_replace_variables = msgs_replace_variables
```

### Comparing `handyllm-0.7.2/src/handyllm/requestor.py` & `handyllm-0.7.3/src/handyllm/requestor.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/src/handyllm/utils.py` & `handyllm-0.7.3/src/handyllm/utils.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/tests/test_azure.py` & `handyllm-0.7.3/tests/test_azure.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/tests/test_client_async_sync.py` & `handyllm-0.7.3/tests/test_client_async_sync.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/tests/test_endpoint.py` & `handyllm-0.7.3/tests/test_endpoint.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/tests/test_hprompt.py` & `handyllm-0.7.3/tests/test_hprompt.py`

 * *Files identical despite different names*

### Comparing `handyllm-0.7.2/tests/test_prompt.py` & `handyllm-0.7.3/tests/test_prompt.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,26 +1,21 @@
-import json
 from handyllm import PromptConverter
 converter = PromptConverter()
 
 converter.read_substitute_content('./assets/substitute.txt')  # read substitute map
 
-# chat can be used as the message parameter for OpenAI API
-chat = converter.rawfile2chat('./assets/prompt.txt')  # variables are substituted according to map
-# print(json.dumps(chat, indent=2))
-print(converter.chat2raw(chat))
+# msgs can be used as the message parameter for OpenAI API
+msgs = converter.rawfile2msgs('./assets/prompt.txt')  # variables are substituted according to map
+# print(json.dumps(msgs, indent=2))
+print(converter.msgs2raw(msgs))
 print('-----')
 
 # variables wrapped in %s can be replaced at runtime
-new_chat = converter.chat_replace_variables(
-    chat, 
+new_msgs = converter.msgs_replace_variables(
+    msgs, 
     {
         r'%misc1%': 'Note1: do not use any bad word.',
         r'%misc2%': 'Note2: be optimistic.',
     }
 )
-# print(json.dumps(new_chat, indent=2))
-print(converter.chat2raw(new_chat))
-print(converter.chat_append_msg(new_chat, '''{
-    "item1": "It is really a good day.",
-    "item2": "Indeed."
-}''', role='assistant'))
+# print(json.dumps(new_msgs, indent=2))
+print(converter.msgs2raw(new_msgs))
```

