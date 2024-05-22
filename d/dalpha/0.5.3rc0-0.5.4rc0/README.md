# Comparing `tmp/dalpha-0.5.3rc0.tar.gz` & `tmp/dalpha-0.5.4rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dalpha-0.5.3rc0.tar", max compression
+gzip compressed data, was "dalpha-0.5.4rc0.tar", max compression
```

## Comparing `dalpha-0.5.3rc0.tar` & `dalpha-0.5.4rc0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
--rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.3rc0/README.md
--rw-r--r--   0        0        0     2077 2024-05-16 07:16:07.976796 dalpha-0.5.3rc0/dalpha/__init__.py
--rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.3rc0/dalpha/agent.py
--rw-r--r--   0        0        0     7019 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/backend_cli.py
--rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.3rc0/dalpha/cobra_cls.py
--rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/context.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/data_update_cls.py
--rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/dto.py
--rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.3rc0/dalpha/exception.py
--rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.3rc0/dalpha/inference_cls.py
--rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.3rc0/dalpha/kafka_cli.py
--rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.3rc0/dalpha/logging/__init__.py
--rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/events.py
--rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/log_formatter.py
--rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/logging/utils.py
--rw-r--r--   0        0        0     6687 2024-05-16 17:41:28.081119 dalpha-0.5.3rc0/dalpha/message_consumer.py
--rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/openai_cls.py
--rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/redis_cli.py
--rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.3rc0/dalpha/redis_cls.py
--rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/request.py
--rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/s3.py
--rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.3rc0/dalpha/signal_handler.py
--rw-r--r--   0        0        0      767 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/slack.py
--rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.3rc0/dalpha/update_agent.py
--rw-r--r--   0        0        0      952 2024-05-18 12:36:17.240345 dalpha-0.5.3rc0/pyproject.toml
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.3rc0/PKG-INFO
+-rw-r--r--   0        0        0      578 2023-12-18 04:10:26.318635 dalpha-0.5.4rc0/README.md
+-rw-r--r--   0        0        0     2090 2024-05-22 02:06:09.763823 dalpha-0.5.4rc0/dalpha/__init__.py
+-rw-r--r--   0        0        0     8282 2024-05-16 17:41:28.081119 dalpha-0.5.4rc0/dalpha/agent.py
+-rw-r--r--   0        0        0     7889 2024-05-22 02:06:09.763823 dalpha-0.5.4rc0/dalpha/backend_cli.py
+-rw-r--r--   0        0        0      555 2024-05-08 06:25:10.211719 dalpha-0.5.4rc0/dalpha/cobra_cls.py
+-rw-r--r--   0        0        0      573 2024-02-28 08:10:55.063883 dalpha-0.5.4rc0/dalpha/context.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:23:00.795089 dalpha-0.5.4rc0/dalpha/data_update_cls.py
+-rw-r--r--   0        0        0      940 2024-05-02 07:23:00.795089 dalpha-0.5.4rc0/dalpha/dto.py
+-rw-r--r--   0        0        0      616 2024-05-16 07:16:07.980796 dalpha-0.5.4rc0/dalpha/exception.py
+-rw-r--r--   0        0        0     6000 2024-05-18 12:36:17.240345 dalpha-0.5.4rc0/dalpha/inference_cls.py
+-rw-r--r--   0        0        0      233 2024-03-25 02:37:47.094337 dalpha-0.5.4rc0/dalpha/kafka_cli.py
+-rw-r--r--   0        0        0     1861 2024-03-11 02:52:37.986799 dalpha-0.5.4rc0/dalpha/logging/__init__.py
+-rw-r--r--   0        0        0      229 2024-02-28 08:10:55.063883 dalpha-0.5.4rc0/dalpha/logging/events.py
+-rw-r--r--   0        0        0     1116 2024-02-28 08:10:55.063883 dalpha-0.5.4rc0/dalpha/logging/log_formatter.py
+-rw-r--r--   0        0        0     1817 2024-02-28 08:10:55.063883 dalpha-0.5.4rc0/dalpha/logging/utils.py
+-rw-r--r--   0        0        0     6689 2024-05-22 02:06:09.767823 dalpha-0.5.4rc0/dalpha/message_consumer.py
+-rw-r--r--   0        0        0     1703 2024-05-10 10:54:52.512416 dalpha-0.5.4rc0/dalpha/openai_cls.py
+-rw-r--r--   0        0        0     6079 2024-05-02 07:23:00.795089 dalpha-0.5.4rc0/dalpha/redis_cli.py
+-rw-r--r--   0        0        0     1886 2024-05-02 07:23:00.795089 dalpha-0.5.4rc0/dalpha/redis_cls.py
+-rw-r--r--   0        0        0      776 2024-05-10 10:54:52.512416 dalpha-0.5.4rc0/dalpha/request.py
+-rw-r--r--   0        0        0     2689 2024-05-10 10:54:52.512416 dalpha-0.5.4rc0/dalpha/s3.py
+-rw-r--r--   0        0        0      497 2024-02-28 08:10:55.063883 dalpha-0.5.4rc0/dalpha/signal_handler.py
+-rw-r--r--   0        0        0     2355 2024-05-10 10:54:52.512416 dalpha-0.5.4rc0/dalpha/update_agent.py
+-rw-r--r--   0        0        0      952 2024-05-22 02:06:09.767823 dalpha-0.5.4rc0/pyproject.toml
+-rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 dalpha-0.5.4rc0/PKG-INFO
```

### Comparing `dalpha-0.5.3rc0/README.md` & `dalpha-0.5.4rc0/README.md`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/__init__.py` & `dalpha-0.5.4rc0/dalpha/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,10 +46,10 @@
 
 from dalpha.agent import Agent
 from dalpha.cobra_cls import Cobra
 from dalpha.data_update_cls import DalphaDataUpdater
 from dalpha.inference_cls import DalphaAI
 from dalpha.redis_cls import DalphaRedis
 from dalpha.openai_cls import DalphaOpenAI
-from dalpha.backend_cli import BackendCli, internal_call
+from dalpha.backend_cli import BackendCli, internal_call, slack_alert
 from dalpha.message_consumer import EvaluateItem
 import dalpha.s3 as s3
```

### Comparing `dalpha-0.5.3rc0/dalpha/agent.py` & `dalpha-0.5.4rc0/dalpha/agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/backend_cli.py` & `dalpha-0.5.4rc0/dalpha/backend_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,25 +59,42 @@
                 message = f'error from internal_call(get) / response status_code {response.status_code}: {response.text}'
                 sentry_sdk.capture_message(message)
                 raise Exception(message)
     message = f'internal call result is not returned in timeout({time_out}) seconds.'
     sentry_sdk.capture_message(message)
     raise Exception(message)
 
+def slack_alert(self, channel_name, text):
+    url = os.path.join(self.base_url, f'slack/message')
+    payload = {
+        "channelName": channel_name,
+        "message": text
+    }
+    with RetrySession() as s:
+        response = s.post(url, headers=self.header, data=json.dumps(payload))
+    if response.status_code == 200:
+        return response.json()
+    elif response.status_code < 500: # 400대 에러일 때는 확실히 유효하지 않은 메세지로 판단
+        logger.warning(f'error from slack_alert / response status_code {response.status_code}: {response.text}')
+        return None
+    else: # 5회 재시도해도 500대 에러일 때는 유효한지 알 수 없으므로 유효하지 않은 메세지로 판단
+        logger.error(f'error from slack_alert / response status_code {response.status_code}: {response.text}')
+        return None
+
 class BackendCli:
     def __init__(self, api_id, dev_server, token):
         self.api_id = api_id
         self.dev_server = dev_server
         self.base_url = os.environ.get('DEV_BASE_URL', 'https://api.exp.dalpha.so') if dev_server else os.environ.get('BASE_URL', 'https://api.dalpha.so')
         self.token = token
         self.header = {
             'token': self.token,
             'Content-Type': 'application/json'
         }
-    
+        
     def get_internal_slack(self):
         try:
             url = os.path.join(self.base_url, f'inferences/{self.api_id}/owner')
             response = requests.request("GET", url, headers=self.header)
             account_id = response.json()
             if account_id == -1:
                 return "<!subteam^S05EP7HQ18V>"
```

### Comparing `dalpha-0.5.3rc0/dalpha/cobra_cls.py` & `dalpha-0.5.4rc0/dalpha/cobra_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/context.py` & `dalpha-0.5.4rc0/dalpha/context.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/data_update_cls.py` & `dalpha-0.5.4rc0/dalpha/data_update_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/dto.py` & `dalpha-0.5.4rc0/dalpha/dto.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/exception.py` & `dalpha-0.5.4rc0/dalpha/exception.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/inference_cls.py` & `dalpha-0.5.4rc0/dalpha/inference_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/logging/__init__.py` & `dalpha-0.5.4rc0/dalpha/logging/__init__.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/logging/log_formatter.py` & `dalpha-0.5.4rc0/dalpha/logging/log_formatter.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/logging/utils.py` & `dalpha-0.5.4rc0/dalpha/logging/utils.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/message_consumer.py` & `dalpha-0.5.4rc0/dalpha/message_consumer.py`

 * *Files 6% similar despite different names*

```diff
@@ -95,22 +95,22 @@
         self.evaluates = {}
 
     def _batch(self, iterable, n):
         # Yield successive n-sized chunks from iterable.
         for i in range(0, len(iterable), n):
             yield iterable[i:i + n]
 
-    def _delete_messages(self, message_ids):
+    def _delete_messages(self, evaluate_ids):
         '''
-            message_id를 10개씩 끊어서 sqs에 batch delete 요청으로 메세지 삭제
+            evaluate_id를 10개씩 끊어서 sqs에 batch delete 요청으로 메세지 삭제
         '''
-        entries = list(map(lambda message_id: {
-            'Id': str(message_id),
-            'ReceiptHandle': self.evaluates[message_id]
-        }, message_ids))
+        entries = list(map(lambda evaluate_id: {
+            'Id': str(evaluate_id),
+            'ReceiptHandle': self.evaluates[evaluate_id]
+        }, evaluate_ids))
         for group in self._batch(entries, 10):
             try:
                 self.sqs_consumer.delete_message_batch(
                     QueueUrl = self.queue_url,
                     Entries = group
                 )
             except Exception as e:
@@ -127,18 +127,18 @@
         messages = response.get('Messages', [])
         # invalid message를 제외한 message를 evaluate_items에 추가
         for message in messages:
             message_body = message['Body']
             try:
                 # message_body를 딕셔너리로 변환
                 message_dict = json.loads(message_body)
+                self.evaluates[message_dict['id']] = message['ReceiptHandle']
                 evaluate = self.backend_cli.get_evaluate(message_dict.get('id'))
                 if evaluate != None:
                     evaluate_items.append(to_evaluate_item(evaluate))
-                    self.evaluates[message_dict['id']] = message['ReceiptHandle']
                 else:
                     invalid_messages.append(message_dict)
             except json.JSONDecodeError:
                 logger.error("유효한 JSON 형식이 아닙니다.")
 
         # sqs에서 invalid messages 삭제
         if (len(invalid_messages) > 0):
```

### Comparing `dalpha-0.5.3rc0/dalpha/openai_cls.py` & `dalpha-0.5.4rc0/dalpha/openai_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/redis_cli.py` & `dalpha-0.5.4rc0/dalpha/redis_cli.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/redis_cls.py` & `dalpha-0.5.4rc0/dalpha/redis_cls.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/request.py` & `dalpha-0.5.4rc0/dalpha/request.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/s3.py` & `dalpha-0.5.4rc0/dalpha/s3.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/dalpha/update_agent.py` & `dalpha-0.5.4rc0/dalpha/update_agent.py`

 * *Files identical despite different names*

### Comparing `dalpha-0.5.3rc0/pyproject.toml` & `dalpha-0.5.4rc0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dalpha"
-version = "0.5.3rc0"
+version = "0.5.4rc0"
 description = ""
 authors = ["devops <devops@dalpha.so>"]
 readme = "README.md"
 packages = [{include = "dalpha"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -17,15 +17,15 @@
 pydantic = "^2.7.1"
 
 [tool.poetry.group.dev.dependencies]
 twine = "^4.0.2"
 
 [project]
 name = "dalpha"
-version = "0.5.3rc0"
+version = "0.5.4rc0"
 authors = [
   { name="Beomseok", email="beomseok.kim@dalpha.so" },
   { name="Gideok", email="gideok.kim@dalpha.so" },
 ]
 description = "Dalpha internal sdk"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `dalpha-0.5.3rc0/PKG-INFO` & `dalpha-0.5.4rc0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dalpha
-Version: 0.5.3rc0
+Version: 0.5.4rc0
 Summary: 
 Author: devops
 Author-email: devops@dalpha.so
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

