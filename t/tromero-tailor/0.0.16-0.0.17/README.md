# Comparing `tmp/tromero_tailor-0.0.16.tar.gz` & `tmp/tromero_tailor-0.0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tromero_tailor-0.0.16.tar", last modified: Fri May 17 14:21:25 2024, max compression
+gzip compressed data, was "tromero_tailor-0.0.17.tar", last modified: Wed May 22 12:41:29 2024, max compression
```

## Comparing `tromero_tailor-0.0.16.tar` & `tromero_tailor-0.0.17.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.193234 tromero_tailor-0.0.16/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-17 14:21:25.193012 tromero_tailor-0.0.16/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.16/README.md
--rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-17 14:21:25.193286 tromero_tailor-0.0.16/setup.cfg
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-17 14:20:53.000000 tromero_tailor-0.0.16/setup.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.191402 tromero_tailor-0.0.16/tests/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.16/tests/test.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.191953 tromero_tailor-0.0.16/tromero_tailor/
--rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.16/tromero_tailor/__init__.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1630 2024-05-17 14:18:24.000000 tromero_tailor-0.0.16/tromero_tailor/tromero_requests.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.16/tromero_tailor/tromero_utils.py
--rw-r--r--   0 tadhgamin   (501) staff       (20)     3024 2024-05-17 14:16:30.000000 tromero_tailor-0.0.16/tromero_tailor/wrapper.py
-drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-17 14:21:25.192768 tromero_tailor-0.0.16/tromero_tailor.egg-info/
--rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/PKG-INFO
--rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/SOURCES.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/dependency_links.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/requires.txt
--rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-17 14:21:25.000000 tromero_tailor-0.0.16/tromero_tailor.egg-info/top_level.txt
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 12:41:29.587859 tromero_tailor-0.0.17/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-22 12:41:29.587656 tromero_tailor-0.0.17/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      942 2024-04-08 16:49:32.000000 tromero_tailor-0.0.17/README.md
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       38 2024-05-22 12:41:29.587902 tromero_tailor-0.0.17/setup.cfg
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1633 2024-05-22 12:41:04.000000 tromero_tailor-0.0.17/setup.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 12:41:29.586131 tromero_tailor-0.0.17/tests/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3672 2024-04-17 14:55:07.000000 tromero_tailor-0.0.17/tests/test.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 12:41:29.586616 tromero_tailor-0.0.17/tromero_tailor/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       30 2024-04-08 15:07:54.000000 tromero_tailor-0.0.17/tromero_tailor/__init__.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     2149 2024-05-22 12:27:35.000000 tromero_tailor-0.0.17/tromero_tailor/tromero_requests.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      446 2024-04-12 11:06:15.000000 tromero_tailor-0.0.17/tromero_tailor/tromero_utils.py
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     3247 2024-05-22 12:24:04.000000 tromero_tailor-0.0.17/tromero_tailor/wrapper.py
+drwxr-xr-x   0 tadhgamin   (501) staff       (20)        0 2024-05-22 12:41:29.587420 tromero_tailor-0.0.17/tromero_tailor.egg-info/
+-rw-r--r--   0 tadhgamin   (501) staff       (20)     1937 2024-05-22 12:41:29.000000 tromero_tailor-0.0.17/tromero_tailor.egg-info/PKG-INFO
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      341 2024-05-22 12:41:29.000000 tromero_tailor-0.0.17/tromero_tailor.egg-info/SOURCES.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)        1 2024-05-22 12:41:29.000000 tromero_tailor-0.0.17/tromero_tailor.egg-info/dependency_links.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)      304 2024-05-22 12:41:29.000000 tromero_tailor-0.0.17/tromero_tailor.egg-info/requires.txt
+-rw-r--r--   0 tadhgamin   (501) staff       (20)       15 2024-05-22 12:41:29.000000 tromero_tailor-0.0.17/tromero_tailor.egg-info/top_level.txt
```

### Comparing `tromero_tailor-0.0.16/PKG-INFO` & `tromero_tailor-0.0.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.16
+Version: 0.0.17
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `tromero_tailor-0.0.16/README.md` & `tromero_tailor-0.0.17/README.md`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.16/setup.py` & `tromero_tailor-0.0.17/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="tromero_tailor",  # Replace with your package name
-    version="0.0.16",  # Replace with your package's version
+    version="0.0.17",  # Replace with your package's version
     author="Tromero",  # Replace with your name
     author_email="tadhg.amin@tromero.ai",  # Replace with your email address
     description="A short description of your package",  # Provide a short description
     long_description=open('README.md').read(),  # This will read your long description from README.md
     long_description_content_type='text/markdown',  # Indicates that the long description is in Markdown
     url="http://yourpackagehomepage.com",  # Replace with the URL to your package's homepage
     license="MIT",  # Replace with your chosen license
```

### Comparing `tromero_tailor-0.0.16/tests/test.py` & `tromero_tailor-0.0.17/tests/test.py`

 * *Files identical despite different names*

### Comparing `tromero_tailor-0.0.16/tromero_tailor/tromero_requests.py` & `tromero_tailor-0.0.17/tromero_tailor/tromero_requests.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,55 @@
 import requests
 
 data_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1/data"
 models_url = "http://35.246.163.71:5000/generate"
 self_hosted_models_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1/generate"
+base_url = "https://midyear-grid-402910.lm.r.appspot.com/tailor/v1"
 
 def post_data(data, auth_token):
     headers = {
         'X-API-KEY': auth_token,
         'Content-Type': 'application/json'
     }
     try:
         response = requests.post(data_url, json=data, headers=headers)
         response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
         return response.json()  # Return the JSON response if request was successful
     except Exception as e:
         return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
     
 
-def tromero_model_create(model, messages, tromero_key, parameters={}, self_hosted=False):
-    url = self_hosted_models_url if self_hosted else models_url
+def tromero_model_create(model, model_url, messages, tromero_key, parameters={}):
     headers = {'Content-Type': 'application/json'}
     data = {
         "adapter_name": model,
         "messages": messages,
         "parameters": parameters
     }
     headers['X-API-KEY'] = tromero_key
-    if self_hosted:
-        url = self_hosted_models_url 
-    else:
-        url = models_url
     try:
-        response = requests.post(url, json=data, headers=headers)
+        response = requests.post(f"{model_url}/generate", json=data, headers=headers)
         response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
         return response.json()  # Return the JSON response if request was successful
     except Exception as e:
         return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
+    
+
+def get_model_url(model_name, auth_token):
+    print("here")
+    headers = {
+        'X-API-KEY': auth_token,
+        'Content-Type': 'application/json'
+    }
+    try:
+        response = requests.get(f"{base_url}/model/{model_name}/url", headers=headers)
+        response.raise_for_status()  # Raises HTTPError for bad responses (4XX, 5XX)
+        return response.json()['url']  # Return the JSON response if request was successful
+    except Exception as e:
+        return {'error': f'An error occurred: {e}', 'status_code': response.status_code if 'response' in locals() else 'N/A'}
+
```

### Comparing `tromero_tailor-0.0.16/tromero_tailor/wrapper.py` & `tromero_tailor-0.0.17/tromero_tailor/wrapper.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from openai import OpenAI
 from openai.resources import Chat
 from openai.resources.chat.completions import (
     Completions
 )
 from openai._compat import cached_property
 import datetime
-from .tromero_requests import post_data, tromero_model_create
+from .tromero_requests import post_data, tromero_model_create, get_model_url
 from .tromero_utils import mock_openai_format
 
     
 
 class MockCompletions(Completions):
     def __init__(self, client):
         super().__init__(client)
@@ -52,16 +52,20 @@
                                     "model": input['model'],
                                     "kwargs": formatted_kwargs,
                                     "creation_time": str(datetime.datetime.now().isoformat()),
                                     "usage": usage,
                                     "tags": tags
                                     })
         else:
+            model_name = kwargs['model']
+            if model_name not in self._client.model_urls:
+                url = get_model_url(model_name, self._client.tromero_key)
+                self._client.model_urls[model_name] = url
             messages = kwargs['messages']
-            res = tromero_model_create(kwargs['model'], messages, self._client.tromero_key, formatted_kwargs, self._client.self_hosted)
+            res = tromero_model_create(model_name, self._client.model_urls[model_name], messages, self._client.tromero_key, formatted_kwargs)
             # check if res has field 'generated_text'
             if 'generated_text' in res:
                 res = mock_openai_format(res['generated_text'])
         return res
 
 
 class MockChat(Chat):
@@ -71,13 +75,13 @@
     @cached_property
     def completions(self) -> Completions:
         return MockCompletions(self._client)
 
 
 class TailorAI(OpenAI):
     chat: MockChat
-    def __init__(self, api_key, tromero_key, self_hosted=False):
+    def __init__(self, api_key, tromero_key):
         super().__init__(api_key=api_key)
         self.current_prompt = []
-        self.chat = MockChat(self)
+        self.model_urls = {}
         self.tromero_key = tromero_key
-        self.self_hosted = self_hosted
+        self.chat = MockChat(self)
```

### Comparing `tromero_tailor-0.0.16/tromero_tailor.egg-info/PKG-INFO` & `tromero_tailor-0.0.17/tromero_tailor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tromero_tailor
-Version: 0.0.16
+Version: 0.0.17
 Summary: A short description of your package
 Home-page: http://yourpackagehomepage.com
 Author: Tromero
 Author-email: tadhg.amin@tromero.ai
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

