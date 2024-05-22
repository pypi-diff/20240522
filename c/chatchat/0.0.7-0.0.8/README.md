# Comparing `tmp/chatchat-0.0.7.tar.gz` & `tmp/chatchat-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.7.tar", last modified: Tue May 21 23:02:50 2024, max compression
+gzip compressed data, was "chatchat-0.0.8.tar", last modified: Wed May 22 10:58:40 2024, max compression
```

## Comparing `chatchat-0.0.7.tar` & `chatchat-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 23:02:47.000000 chatchat-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 23:02:50.852342 chatchat-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:47.000000 chatchat-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:02:50.852342 chatchat-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 23:02:47.000000 chatchat-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-22 10:58:34.000000 chatchat-0.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 10:58:40.843257 chatchat-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:34.000000 chatchat-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6012 2024-05-22 10:58:34.000000 chatchat-0.0.8/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 10:58:40.843257 chatchat-0.0.8/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 10:58:40.000000 chatchat-0.0.8/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 10:58:40.843257 chatchat-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-22 10:58:34.000000 chatchat-0.0.8/setup.py
```

### Comparing `chatchat-0.0.7/LICENSE` & `chatchat-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.7/PKG-INFO` & `chatchat-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.7/chatchat/baidu.py` & `chatchat-0.0.8/chatchat/baidu.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from chatchat.base import Base
-import httpx, time, json
+import httpx, time
 
 class Completion(Base):
     def __init__(self, jfile, model='ERNIE-Speed-8K'):
         # https://console.bce.baidu.com/qianfan/ais/console/onlineService
         self.api_list = {
             'ERNIE-Speed-8K': 'ernie_speed',
             'ERNIE-Speed-128K': 'ernie-speed-128k',
```

### Comparing `chatchat-0.0.7/chatchat/xunfei.py` & `chatchat-0.0.8/chatchat/xunfei.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,15 +3,42 @@
 from chatchat.base import Base
 import base64, hashlib, hmac
 from datetime import datetime
 from time import mktime
 import time, websocket, json, ssl
 
 class Completion(Base):
-    def __init__(self, jfile, version='2.0'):
+    def __init__(self, jfile, model='Spark Lite'):
+        # https://www.xfyun.cn/doc/spark/Web.html#_1-接口说明
+        self.api_list = {
+            'Spark3.5 Max': {
+                'path': '/v3.5/chat',
+                'domain': 'generalv3.5',
+            },
+            'Spark Pro': {
+                'path': '/v3.1/chat',
+                'domain': 'generalv3',
+            },
+            'Spark V2.0': {
+                'path': '/v2.1/chat',
+                'domain': 'generalv2',
+            },
+            'Spark Lite': {
+                'path': '/v1.1/chat',
+                'domain': 'general',
+            },
+        }
+
+        if model not in self.api_list:
+            raise RuntimeError(f'supported chat type: {self.api_list.keys()}')
+        self.host = 'spark-api.xf-yun.com'
+        self.api = self.api_list[model]
+        self.path = self.api['path']
+        self.domain = self.api['domain']
+
         # jfile: https://console.xfyun.cn/services/bm2
         # "xunfei": {
         #     "app_id": "x",
         #     "api_secret": "y",
         #     "api_key": "z"
         # }
         self.jfile = jfile
@@ -21,16 +48,14 @@
             'Content-Type': 'application/json',
             'Accept': 'application/json'
         }
 
         if "api_key" not in self.jdata or "api_secret" not in self.jdata:
             raise RuntimeError(f'please check <xunfei> api_key and api_secret in {jfile}')
 
-        self.host = 'spark-api.xf-yun.com'
-        self.path = '/v2.1/chat' if version != '1.5' else '/v1.1/chat'
         self.update_url()
         websocket.enableTrace(False)
         self.answer = ''
 
     def create_url(self):
         # https://www.xfyun.cn/doc/spark/general_url_authentication.html
         now = datetime.now()
@@ -95,22 +120,67 @@
             status = choices["status"]
             content = choices["text"][0]["content"]
             self.answer += content
             if wsapp.stream: print(content, end='')
             if status == 2:
                 wsapp.close()
 
-    def create(self, json, stream=False):
+    def make_message(self, history: list):
+        jmsg = {
+            "header": {
+                "app_id": self.jdata['app_id'],
+            },
+            "parameter": {
+                "chat": {
+                    "domain": self.domain,
+                }
+            },
+            "payload": {
+                "message": {
+                    "text": history
+                }
+            }
+        }
+        return jmsg
+
+    def create(self, message, stream=False):
+        jmsg = self.make_message([{
+            "role": "user", "content": message
+        }])
+
         self.answer = ''
         url = self.get_url()
         ws = websocket.WebSocketApp(
             url, on_message=self.on_message, on_error=self.on_error,
             on_close=self.on_close, on_open=self.on_open,
         )
-        ws.json = json
+        ws.json = jmsg
         ws.stream = stream
         ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
         return self.answer
 
-class Chat():
-    def __init__(self):
-        ...
+class Chat(Completion):
+    def __init__(self, jfile, model='Spark Lite', history=[]):
+        super().__init__(jfile, model=model)
+        self.history = history
+
+    def chat(self, message, stream=False):
+        self.history.append({
+            "role": "user", "content": message
+        })
+        jmsg = self.make_message(self.history)
+
+        self.answer = ''
+        url = self.get_url()
+        ws = websocket.WebSocketApp(
+            url, on_message=self.on_message, on_error=self.on_error,
+            on_close=self.on_close, on_open=self.on_open,
+        )
+        ws.json = jmsg
+        ws.stream = stream
+        ws.run_forever(sslopt={"cert_reqs": ssl.CERT_NONE})
+
+        self.history.append({
+            "role": "assistant", "content": self.answer,
+        })
+
+        return self.answer
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `chatchat-0.0.7/chatchat.egg-info/PKG-INFO` & `chatchat-0.0.8/chatchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.7
+Version: 0.0.8
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.7/setup.py` & `chatchat-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.7',
+    version = '0.0.8',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

