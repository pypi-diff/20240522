# Comparing `tmp/hyperbee-0.0.2.2.tar.gz` & `tmp/hyperbee-0.0.2.3.tar.gz`

## Comparing `hyperbee-0.0.2.2.tar` & `hyperbee-0.0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/__init__.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/_client.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/_version.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/version.py
--rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/__init__.py
--rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/completions.py
--rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/models.py
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/batch_request/__init__.py
--rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/batch_request/batch_request.py
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/chat/__init__.py
--rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/chat/chat.py
--rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/chat/completions.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/pipeline/__init__.py
--rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/src/hyperbee/resources/pipeline/pipeline.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/.gitignore
--rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/README.md
--rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/pyproject.toml
--rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     6631 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/__init__.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/_client.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/_version.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/version.py
+-rw-r--r--   0        0        0     1336 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/__init__.py
+-rw-r--r--   0        0        0    30808 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/completions.py
+-rw-r--r--   0        0        0    10189 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/models.py
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/batch_request/__init__.py
+-rw-r--r--   0        0        0     2663 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/batch_request/batch_request.py
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/chat/__init__.py
+-rw-r--r--   0        0        0     2317 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/chat/chat.py
+-rw-r--r--   0        0        0    36597 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/chat/completions.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/pipeline/__init__.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/src/hyperbee/resources/pipeline/pipeline.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/.gitignore
+-rw-r--r--   0        0        0    11307 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/README.md
+-rw-r--r--   0        0        0     3894 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    12901 2020-02-02 00:00:00.000000 hyperbee-0.0.2.3/PKG-INFO
```

### Comparing `hyperbee-0.0.2.2/src/hyperbee/__init__.py` & `hyperbee-0.0.2.3/src/hyperbee/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/_client.py` & `hyperbee-0.0.2.3/src/hyperbee/_client.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/__init__.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/completions.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/models.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/models.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/batch_request/batch_request.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/batch_request/batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     def __init__(self, api_key):
         self.api_key = api_key  # Assuming you will use api_key somewhere
         self.base_url = "http://35.239.135.107:30001"
         self.base_url2 = "http://34.68.121.35:30001"
         self.base_url3 = "http://34.170.152.22:30001"
         self.thread_cnt = 120
         self.thread_cnt2 = 120
-        self.thread_cnt3 = 10
+        self.thread_cnt3 = 80
     async def sync_call(self, prompt_list: List[str], output_length: int):
         output_length = output_length + 1
         result_queue = queue.Queue()
         
         total_thread_cnt = self.thread_cnt + self.thread_cnt2 + self.thread_cnt3
         prompt_per_thread = (len(prompt_list) // total_thread_cnt) + 1
```

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/chat/__init__.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/chat/__init__.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/chat/chat.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/chat/chat.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/chat/completions.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/chat/completions.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/src/hyperbee/resources/pipeline/pipeline.py` & `hyperbee-0.0.2.3/src/hyperbee/resources/pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/README.md` & `hyperbee-0.0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `hyperbee-0.0.2.2/pyproject.toml` & `hyperbee-0.0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hyperbee"
-version = "0.0.2.2"
+version = "0.0.2.3"
 description = "The official Python library for the hyperbee API"
 readme = "README.md"
 license = "Apache-2.0"
 authors = [
 { name = "Hive", email = "support@hyperbee.ai" },
 ]
 dependencies = [
```

### Comparing `hyperbee-0.0.2.2/PKG-INFO` & `hyperbee-0.0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hyperbee
-Version: 0.0.2.2
+Version: 0.0.2.3
 Summary: The official Python library for the hyperbee API
 Project-URL: Homepage, https://github.com/HyperbeeAI/hive-python
 Project-URL: Repository, https://github.com/HyperbeeAI/hive-python
 Author-email: Hive <support@hyperbee.ai>
 License-Expression: Apache-2.0
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

