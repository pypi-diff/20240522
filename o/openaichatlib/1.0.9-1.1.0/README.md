# Comparing `tmp/openaichatlib-1.0.9.tar.gz` & `tmp/openaichatlib-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openaichatlib-1.0.9.tar", last modified: Wed May 22 08:33:03 2024, max compression
+gzip compressed data, was "openaichatlib-1.1.0.tar", last modified: Wed May 22 09:04:05 2024, max compression
```

## Comparing `openaichatlib-1.0.9.tar` & `openaichatlib-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.680343 openaichatlib-1.0.9/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.9/LICENSE
--rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 08:33:03.679817 openaichatlib-1.0.9/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.9/README.md
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.676477 openaichatlib-1.0.9/openaichatlib/
--rw-r--r--   0 chenshuai   (501) staff       (20)     8147 2024-05-22 08:32:14.000000 openaichatlib-1.0.9/openaichatlib/V3.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/__init__.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/typings.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/utils.py
--rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/version.py
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.679233 openaichatlib-1.0.9/openaichatlib.egg-info/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       16 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/requires.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/top_level.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-05-22 08:33:03.680451 openaichatlib-1.0.9/setup.cfg
--rw-r--r--   0 chenshuai   (501) staff       (20)     1121 2024-05-22 08:32:14.000000 openaichatlib-1.0.9/setup.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 09:04:05.631219 openaichatlib-1.1.0/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.1.0/LICENSE
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 09:04:05.630694 openaichatlib-1.1.0/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.1.0/README.md
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 09:04:05.626771 openaichatlib-1.1.0/openaichatlib/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     8419 2024-05-22 09:04:02.000000 openaichatlib-1.1.0/openaichatlib/V3.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.1.0/openaichatlib/__init__.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.1.0/openaichatlib/typings.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.1.0/openaichatlib/utils.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.1.0/openaichatlib/version.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 09:04:05.630113 openaichatlib-1.1.0/openaichatlib.egg-info/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 09:04:05.000000 openaichatlib-1.1.0/openaichatlib.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-05-22 09:04:05.000000 openaichatlib-1.1.0/openaichatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-05-22 09:04:05.000000 openaichatlib-1.1.0/openaichatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       16 2024-05-22 09:04:05.000000 openaichatlib-1.1.0/openaichatlib.egg-info/requires.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-05-22 09:04:05.000000 openaichatlib-1.1.0/openaichatlib.egg-info/top_level.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-05-22 09:04:05.631344 openaichatlib-1.1.0/setup.cfg
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1121 2024-05-22 09:04:02.000000 openaichatlib-1.1.0/setup.py
```

### Comparing `openaichatlib-1.0.9/LICENSE` & `openaichatlib-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.9/PKG-INFO` & `openaichatlib-1.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.9
+Version: 1.1.0
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.9/README.md` & `openaichatlib-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.9/openaichatlib/V3.py` & `openaichatlib-1.1.0/openaichatlib/V3.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,15 @@
             self,
             prompt,
             role: str = "user",
             convo_id: str = "default",
             model: str = None,
             pass_history: bool = True,
             json_format: bool = False,
+            stream_include_usage: bool = True,
             stream: bool = True,
             **kwargs,
     ):
         """
         Ask a question
         """
         # Make conversation if it doesn't exist
@@ -112,15 +113,15 @@
         max_tokens = kwargs.get("max_tokens", self.max_tokens)
         if max_tokens:
             payload["max_tokens"] = max_tokens
         if json_format:
             payload["response_format"] = {
                 "type": "json_object"
             }
-        if stream:
+        if stream and stream_include_usage:
             payload["stream_options"] = {
                 "include_usage": True
             }
 
         presence_penalty = kwargs.get("presence_penalty", None)
         if presence_penalty:
             payload["presence_penalty"] = presence_penalty
@@ -154,16 +155,18 @@
                 # Remove "data: "
                 line = line.decode("utf-8")[6:]
                 if line == "[DONE]":
                     break
                 resp: dict = json.loads(line)
                 usage = resp.get("usage", None)
                 if usage:
-                    prompt_tokens = usage.get("prompt_tokens", 0)
-                    completion_tokens = usage.get("completion_tokens", 0)
+                    if prompt_tokens == 0:
+                        prompt_tokens = usage.get("prompt_tokens", 0)
+                    if completion_tokens == 0:
+                        completion_tokens = usage.get("completion_tokens", 0)
                 choices = resp.get("choices")
                 if not choices:
                     continue
                 delta = choices[0].get("delta")
                 if not delta:
                     continue
                 if "role" in delta:
@@ -194,26 +197,28 @@
             self,
             prompt,
             role: str = "user",
             convo_id: str = "default",
             model: str = None,
             pass_history: bool = True,
             json_format: bool = False,
+            stream_include_usage: bool = True,
             **kwargs,
     ) -> tuple:
         """
         Non-streaming ask
         """
         response = self.ask_stream(
             prompt=prompt,
             role=role,
             convo_id=convo_id,
             model=model,
             pass_history=pass_history,
             json_format=json_format,
+            stream_include_usage=stream_include_usage,
             stream=False,
             **kwargs,
         )
         full_response = ""
         prompt_tokens = 0
         completion_tokens = 0
         for content in response:
```

### Comparing `openaichatlib-1.0.9/openaichatlib/__init__.py` & `openaichatlib-1.1.0/openaichatlib/__init__.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.9/openaichatlib/typings.py` & `openaichatlib-1.1.0/openaichatlib/typings.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.9/openaichatlib/utils.py` & `openaichatlib-1.1.0/openaichatlib/utils.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.9/openaichatlib.egg-info/PKG-INFO` & `openaichatlib-1.1.0/openaichatlib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.9
+Version: 1.1.0
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `openaichatlib-1.0.9/setup.py` & `openaichatlib-1.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 install_requires = [
     "requests[socks]",
 ]
 
 setup(
     name="openaichatlib",
-    version="1.0.9",
+    version="1.1.0",
     description="OpenAI Chat API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IAn2018cs/OpenAIChatLib",
     author="IAn2018",
     author_email="ian2018cs@gmail.com",
     classifiers=[
```

