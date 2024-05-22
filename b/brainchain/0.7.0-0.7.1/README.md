# Comparing `tmp/brainchain-0.7.0.tar.gz` & `tmp/brainchain-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "brainchain-0.7.0.tar", max compression
+gzip compressed data, was "brainchain-0.7.1.tar", max compression
```

## Comparing `brainchain-0.7.0.tar` & `brainchain-0.7.1.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.7.0/brainchain/README.md
--rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.7.0/brainchain/__init__.py
--rw-r--r--   0        0        0    13624 2024-05-21 22:55:20.072457 brainchain-0.7.0/brainchain/assistants.py
--rw-r--r--   0        0        0    11704 2024-05-22 17:23:08.619843 brainchain-0.7.0/brainchain/brainchain.py
--rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.7.0/brainchain/carnivore.py
--rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.7.0/brainchain/coredata.py
--rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.7.0/brainchain/embeddings.py
--rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.7.0/brainchain/graph/base.py
--rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.7.0/brainchain/graph/schema.py
--rw-r--r--   0        0        0     3949 2024-05-21 23:34:38.931062 brainchain-0.7.0/brainchain/logger.py
--rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.7.0/brainchain/products.py
--rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.7.0/brainchain/requirements.txt
--rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.7.0/brainchain/sales_intel.py
--rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.7.0/brainchain/search_v2.py
--rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.7.0/brainchain/tools/__init__.py
--rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.7.0/brainchain/tools/coding.py
--rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.7.0/brainchain/tools/diffbot.py
--rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.7.0/brainchain/tools/factual.py
--rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.7.0/brainchain/tools/fts.py
--rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.7.0/brainchain/tools/graph.py
--rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.7.0/brainchain/tools/memory.py
--rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.7.0/brainchain/tools/plan.py
--rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.7.0/brainchain/tools/tokens.py
--rw-r--r--   0        0        0    21273 2024-05-21 21:16:24.442049 brainchain-0.7.0/brainchain/tools/tools.py
--rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.7.0/brainchain/tools/web.py
--rw-r--r--   0        0        0      734 2024-05-21 22:23:01.506213 brainchain-0.7.0/brainchain/tools.py
--rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.7.0/brainchain/webapp/__init__.py
--rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.7.0/brainchain/webapp/agents.py
--rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.7.0/brainchain/webapp/base.py
--rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.7.0/brainchain/webapp/business_ideas.py
--rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.7.0/brainchain/webapp/contents.py
--rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.7.0/brainchain/webapp/conversations.py
--rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.7.0/brainchain/webapp/embedding_models.py
--rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.7.0/brainchain/webapp/embeddings.py
--rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.7.0/brainchain/webapp/files.py
--rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.7.0/brainchain/webapp/health.py
--rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.7.0/brainchain/webapp/language_models.py
--rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.7.0/brainchain/webapp/laws.py
--rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.7.0/brainchain/webapp/messages.py
--rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.7.0/brainchain/webapp/namespaces.py
--rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.7.0/brainchain/webapp/programs.py
--rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.7.0/brainchain/webapp/tasks.py
--rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.7.0/brainchain/webapp/tools.py
--rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.7.0/brainchain/webapp/users.py
--rw-r--r--   0        0        0      538 2024-05-22 17:23:28.243670 brainchain-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      556 1970-01-01 00:00:00.000000 brainchain-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1732 2023-06-20 22:57:22.671703 brainchain-0.7.1/brainchain/README.md
+-rw-r--r--   0        0        0     2982 2024-05-10 17:23:42.151722 brainchain-0.7.1/brainchain/__init__.py
+-rw-r--r--   0        0        0    13624 2024-05-21 22:55:20.072457 brainchain-0.7.1/brainchain/assistants.py
+-rw-r--r--   0        0        0    11704 2024-05-22 17:36:20.544530 brainchain-0.7.1/brainchain/brainchain.py
+-rw-r--r--   0        0        0     5663 2024-05-09 05:35:25.596909 brainchain-0.7.1/brainchain/carnivore.py
+-rw-r--r--   0        0        0     2243 2024-02-14 04:10:52.129450 brainchain-0.7.1/brainchain/coredata.py
+-rw-r--r--   0        0        0     2155 2023-09-12 01:13:30.915323 brainchain-0.7.1/brainchain/embeddings.py
+-rw-r--r--   0        0        0    17861 2024-05-11 18:01:39.002320 brainchain-0.7.1/brainchain/graph/base.py
+-rw-r--r--   0        0        0     7386 2024-05-10 17:23:37.046295 brainchain-0.7.1/brainchain/graph/schema.py
+-rw-r--r--   0        0        0     3949 2024-05-21 23:34:38.931062 brainchain-0.7.1/brainchain/logger.py
+-rw-r--r--   0        0        0    11959 2024-05-07 16:51:46.072448 brainchain-0.7.1/brainchain/products.py
+-rw-r--r--   0        0        0    15070 2023-07-05 18:42:36.359889 brainchain-0.7.1/brainchain/requirements.txt
+-rw-r--r--   0        0        0     6024 2024-05-07 16:20:56.058058 brainchain-0.7.1/brainchain/sales_intel.py
+-rw-r--r--   0        0        0     1977 2024-02-29 23:10:12.854747 brainchain-0.7.1/brainchain/search_v2.py
+-rw-r--r--   0        0        0      595 2024-04-12 19:05:17.907126 brainchain-0.7.1/brainchain/tools/__init__.py
+-rw-r--r--   0        0        0     2118 2024-05-09 17:28:37.403805 brainchain-0.7.1/brainchain/tools/coding.py
+-rw-r--r--   0        0        0     3948 2024-05-07 16:51:46.073351 brainchain-0.7.1/brainchain/tools/diffbot.py
+-rw-r--r--   0        0        0      632 2024-02-29 23:10:12.855578 brainchain-0.7.1/brainchain/tools/factual.py
+-rw-r--r--   0        0        0     5800 2024-04-10 01:04:48.531327 brainchain-0.7.1/brainchain/tools/fts.py
+-rw-r--r--   0        0        0     1450 2024-02-29 23:10:12.856798 brainchain-0.7.1/brainchain/tools/graph.py
+-rw-r--r--   0        0        0     1029 2024-02-29 23:10:12.857047 brainchain-0.7.1/brainchain/tools/memory.py
+-rw-r--r--   0        0        0     2154 2024-02-29 23:10:12.857190 brainchain-0.7.1/brainchain/tools/plan.py
+-rw-r--r--   0        0        0     1660 2024-04-15 19:40:33.833814 brainchain-0.7.1/brainchain/tools/tokens.py
+-rw-r--r--   0        0        0    21273 2024-05-21 21:16:24.442049 brainchain-0.7.1/brainchain/tools/tools.py
+-rw-r--r--   0        0        0    12159 2024-05-07 16:51:46.074887 brainchain-0.7.1/brainchain/tools/web.py
+-rw-r--r--   0        0        0      734 2024-05-21 22:23:01.506213 brainchain-0.7.1/brainchain/tools.py
+-rw-r--r--   0        0        0      791 2024-05-07 16:51:51.752365 brainchain-0.7.1/brainchain/webapp/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 16:51:51.752653 brainchain-0.7.1/brainchain/webapp/agents.py
+-rw-r--r--   0        0        0      173 2024-05-07 16:51:51.752960 brainchain-0.7.1/brainchain/webapp/base.py
+-rw-r--r--   0        0        0      977 2024-05-07 16:51:51.753234 brainchain-0.7.1/brainchain/webapp/business_ideas.py
+-rw-r--r--   0        0        0     1282 2024-05-07 16:51:51.753423 brainchain-0.7.1/brainchain/webapp/contents.py
+-rw-r--r--   0        0        0      895 2024-05-07 16:51:51.753590 brainchain-0.7.1/brainchain/webapp/conversations.py
+-rw-r--r--   0        0        0       91 2024-05-07 16:51:51.753815 brainchain-0.7.1/brainchain/webapp/embedding_models.py
+-rw-r--r--   0        0        0     2709 2024-05-07 16:51:51.753990 brainchain-0.7.1/brainchain/webapp/embeddings.py
+-rw-r--r--   0        0        0     1138 2024-05-07 16:51:51.754142 brainchain-0.7.1/brainchain/webapp/files.py
+-rw-r--r--   0        0        0      218 2024-05-07 16:51:51.754320 brainchain-0.7.1/brainchain/webapp/health.py
+-rw-r--r--   0        0        0       90 2024-05-07 16:51:51.754539 brainchain-0.7.1/brainchain/webapp/language_models.py
+-rw-r--r--   0        0        0      622 2024-05-07 16:51:51.754700 brainchain-0.7.1/brainchain/webapp/laws.py
+-rw-r--r--   0        0        0     1110 2024-05-07 16:51:51.754849 brainchain-0.7.1/brainchain/webapp/messages.py
+-rw-r--r--   0        0        0     2220 2024-05-07 16:51:51.755068 brainchain-0.7.1/brainchain/webapp/namespaces.py
+-rw-r--r--   0        0        0     1029 2024-05-07 16:51:51.755220 brainchain-0.7.1/brainchain/webapp/programs.py
+-rw-r--r--   0        0        0      626 2024-05-07 16:51:51.755369 brainchain-0.7.1/brainchain/webapp/tasks.py
+-rw-r--r--   0        0        0      853 2024-05-07 16:51:51.755565 brainchain-0.7.1/brainchain/webapp/tools.py
+-rw-r--r--   0        0        0      677 2024-05-07 16:51:51.755730 brainchain-0.7.1/brainchain/webapp/users.py
+-rw-r--r--   0        0        0      537 2024-05-22 19:01:02.011328 brainchain-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      555 1970-01-01 00:00:00.000000 brainchain-0.7.1/PKG-INFO
```

### Comparing `brainchain-0.7.0/brainchain/README.md` & `brainchain-0.7.1/brainchain/README.md`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/__init__.py` & `brainchain-0.7.1/brainchain/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/assistants.py` & `brainchain-0.7.1/brainchain/assistants.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/brainchain.py` & `brainchain-0.7.1/brainchain/brainchain.py`

 * *Files 10% similar despite different names*

```diff
@@ -57,35 +57,35 @@
         self.name = name
         self.function = function
         self.schema = schema
 
 
 class Brainchain:
     def _init_component(self, component_cls):
-        return component_cls(self.session, self.base_url, self.user_id)
+        return component_cls(self.session, self.api_host, self.user_id)
 
     def __init__(
         self,
         env: str = "prod",
         # brainchain_api_key: str = os.environ["BRAINCHAIN_API_KEY"],
         salesintel_api_key: str = os.environ["SALESINTEL_API_KEY"],
         api_host: str = os.getenv("API_HOST", "https://api.brainchain.cloud"),
         assistants_api_host: str = os.getenv("ASSISTANTS_API_HOST", "https://assistants-api.brainchain.cloud")
     ):
         if env == "prod":
             self.api_host = api_host
             self.assistants_api_host = assistants_api_host
-            print("Brainchain API URL: ", self.base_url)
+            print("Brainchain API URL: ", self.api_host)
         elif env == "dev":
             self.api_host = "http://localhost:8000"
             self.assistants_api_host = "http://localhost:42069"
-            print("Brainchain API URL: ", self.base_url)
+            print("Brainchain API URL: ", self.api_host)
         elif env == "test":
-            self.api_host = self.base_url.replace("api", "api-test")
-            print("Brainchain API URL: ", self.base_url)
+            self.api_host = self.api_host.replace("api", "api-test")
+            print("Brainchain API URL: ", self.api_host)
 
         self.web_data_client = WebDataClient()
         self.session = requests.Session()
         self.access_token = None
         self.user_id = None
         self.user_email = None
 
@@ -170,15 +170,15 @@
         if self.access_token:
             self.session.headers.update({"Authorization": f"Bearer {self.access_token}"})
         else:
             self.session.headers.pop("Authorization", None)
 
     # Authentication
     def login_user(self, email: str = None, password: str = None):
-        url = f"{self.base_url}/v1/users/login"
+        url = f"{self.api_host}/v1/users/login"
         response = self.session.post(url, json={"email": email, "password": password})
         response_data = response.json()
         self.access_token = response_data.get('access_token')
         # expanduser
         with open(os.path.expanduser("~/.config/brainchain/.access_token"), "w") as f:
             f.write(self.access_token)
             f.close()
@@ -187,70 +187,70 @@
         self.user_email = response_data.get("user_email")
 
         self.set_auth_header()  # Update headers with new token
         return response_data
 
     # Users API
     def get_users(self):
-        url = f"{self.base_url}/v1/users/"
+        url = f"{self.api_host}/v1/users/"
         response = self.session.get(url)
         return response.json()
 
     # Conversations API
     def get_all_conversations(self):
-        url = f"{self.base_url}/v1/conversations/list"
+        url = f"{self.api_host}/v1/conversations/list"
         response = self.session.get(url)
         return response.json()
 
     def get_conversation_by_id(self, conversation_id):
-        url = f"{self.base_url}/v1/conversations/{conversation_id}"
+        url = f"{self.api_host}/v1/conversations/{conversation_id}"
         response = self.session.get(url)
         return response.json()
 
     # Messages API
     def get_all_messages(self):
-        url = f"{self.base_url}/v1/messages/"
+        url = f"{self.api_host}/v1/messages/"
         response = self.session.get(url)
         return response.json()
 
     def get_message_by_id(self, message_id):
-        url = f"{self.base_url}/v1/messages/{message_id}"
+        url = f"{self.api_host}/v1/messages/{message_id}"
         response = self.session.get(url)
         return response.json()
 
     # Tools API
     def get_all_tools(self):
-        url = f"{self.base_url}/v1/tools/"
+        url = f"{self.api_host}/v1/tools/"
         response = self.session.get(url)
         return response.json()
 
     # Language Models API
     def get_all_language_models(self):
-        url = f"{self.base_url}/v1/language_models/list"
+        url = f"{self.api_host}/v1/language_models/list"
         response = self.session.get(url)
         return response.json()
 
     # Conversations API
     def create_conversation(self, messages=[]):
-        url = f"{self.base_url}/v1/conversations/"
+        url = f"{self.api_host}/v1/conversations/"
         data = {"user_id": self.user_id, "messages": messages}
         response = self.session.post(url, json=data)
         return response.json()
 
     # Messages API
     def create_message(self, conversation_uuid, role, content):
-        url = f"{self.base_url}/v1/messages/create"
+        url = f"{self.api_host}/v1/messages/create"
         data = {"conversation_uuid": conversation_uuid, "user_id": self.user_id, "role": role, "content": content}
         response = self.session.post(url, json=data)
         resp = response.json()
         print(resp)
         return response.json()
 
     def stream_chat_completion(self, language_model_id, conversation_uuid, mode='single_token', **params):
-        url = f"{self.base_url}" + "/v1/language_models/chat/completions/stream"
+        url = f"{self.api_host}" + "/v1/language_models/chat/completions/stream"
         params = {
             "llm_id": language_model_id,
             "conversation_uuid": conversation_uuid,
             "mode": mode,
             **params,
         }
         with self.session.get(url, stream=True, params=params) as response:
@@ -269,34 +269,34 @@
                 # Handle manual interruption
                 pass
 
         yield json.dumps({"status": "done", "data": "".join(full_completion)})
 
     # Language Models API
     def get_llm_by_id(self, language_model_id):
-        url = f"{self.base_url}/v1/language_models/{language_model_id}/"
+        url = f"{self.api_host}/v1/language_models/{language_model_id}/"
         response = self.session.get(url)
         return response.json()
 
     def get_conversation_messages(self, conversation_id):
         """
         Retrieve messages from a specific conversation.
 
         Args:
             conversation_id (int): The ID of the conversation.
 
         Returns:
             dict: A JSON response containing the conversation messages.
         """
-        url = f"{self.base_url}/v1/conversations/{conversation_id}/messages"
+        url = f"{self.api_host}/v1/conversations/{conversation_id}/messages"
         response = self.session.get(url)
         return response.json()
 
     def get_llm_by_model_name(self, language_model_name):
-        url = f"{self.base_url}/v1/language_models/{language_model_name}/name"
+        url = f"{self.api_host}/v1/language_models/{language_model_name}/name"
         response = self.session.get(url)
         return response.json()
 
     def enforce_login(self):
         if not self.access_token:
             try:
                 # change this to expanduser
```

### Comparing `brainchain-0.7.0/brainchain/carnivore.py` & `brainchain-0.7.1/brainchain/carnivore.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/coredata.py` & `brainchain-0.7.1/brainchain/coredata.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/embeddings.py` & `brainchain-0.7.1/brainchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/graph/base.py` & `brainchain-0.7.1/brainchain/graph/base.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/graph/schema.py` & `brainchain-0.7.1/brainchain/graph/schema.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/logger.py` & `brainchain-0.7.1/brainchain/logger.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/products.py` & `brainchain-0.7.1/brainchain/products.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/requirements.txt` & `brainchain-0.7.1/brainchain/requirements.txt`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/sales_intel.py` & `brainchain-0.7.1/brainchain/sales_intel.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/search_v2.py` & `brainchain-0.7.1/brainchain/search_v2.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/__init__.py` & `brainchain-0.7.1/brainchain/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/coding.py` & `brainchain-0.7.1/brainchain/tools/coding.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/diffbot.py` & `brainchain-0.7.1/brainchain/tools/diffbot.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/factual.py` & `brainchain-0.7.1/brainchain/tools/factual.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/fts.py` & `brainchain-0.7.1/brainchain/tools/fts.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/graph.py` & `brainchain-0.7.1/brainchain/tools/graph.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/memory.py` & `brainchain-0.7.1/brainchain/tools/memory.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/plan.py` & `brainchain-0.7.1/brainchain/tools/plan.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/tokens.py` & `brainchain-0.7.1/brainchain/tools/tokens.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/tools.py` & `brainchain-0.7.1/brainchain/tools/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools/web.py` & `brainchain-0.7.1/brainchain/tools/web.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/tools.py` & `brainchain-0.7.1/brainchain/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/__init__.py` & `brainchain-0.7.1/brainchain/webapp/__init__.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/business_ideas.py` & `brainchain-0.7.1/brainchain/webapp/business_ideas.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/contents.py` & `brainchain-0.7.1/brainchain/webapp/contents.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/conversations.py` & `brainchain-0.7.1/brainchain/webapp/conversations.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/embeddings.py` & `brainchain-0.7.1/brainchain/webapp/embeddings.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/files.py` & `brainchain-0.7.1/brainchain/webapp/files.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/laws.py` & `brainchain-0.7.1/brainchain/webapp/laws.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/messages.py` & `brainchain-0.7.1/brainchain/webapp/messages.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/namespaces.py` & `brainchain-0.7.1/brainchain/webapp/namespaces.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/programs.py` & `brainchain-0.7.1/brainchain/webapp/programs.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/tasks.py` & `brainchain-0.7.1/brainchain/webapp/tasks.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/tools.py` & `brainchain-0.7.1/brainchain/webapp/tools.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/brainchain/webapp/users.py` & `brainchain-0.7.1/brainchain/webapp/users.py`

 * *Files identical despite different names*

### Comparing `brainchain-0.7.0/pyproject.toml` & `brainchain-0.7.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "brainchain"
-version = "0.7.0"
+version = "0.7.1"
 description = "Brainchain API client"
 authors = ["Arthur M. Collé <arthur@brainchain.ai>"]
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 urllib3 = "2.0.6"
 requests = "2.31.0"
-promptlayer = "0.3.3"
-modal-client = "0.53.3722"
+promptlayer = "1.0.2"
+modal-client = "0.62.180"
 tiktoken = ">=0.5.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
```

### Comparing `brainchain-0.7.0/PKG-INFO` & `brainchain-0.7.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: brainchain
-Version: 0.7.0
+Version: 0.7.1
 Summary: Brainchain API client
 Author: Arthur M. Collé
 Author-email: arthur@brainchain.ai
 Requires-Python: >=3.8.1,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: modal-client (==0.53.3722)
-Requires-Dist: promptlayer (==0.3.3)
+Requires-Dist: modal-client (==0.62.180)
+Requires-Dist: promptlayer (==1.0.2)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: tiktoken (>=0.5.0)
 Requires-Dist: urllib3 (==2.0.6)
```

