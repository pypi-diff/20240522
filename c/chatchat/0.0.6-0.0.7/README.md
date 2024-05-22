# Comparing `tmp/chatchat-0.0.6.tar.gz` & `tmp/chatchat-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatchat-0.0.6.tar", last modified: Tue May 21 11:53:33 2024, max compression
+gzip compressed data, was "chatchat-0.0.7.tar", last modified: Tue May 21 23:02:50 2024, max compression
```

## Comparing `chatchat-0.0.6.tar` & `chatchat-0.0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:53:33.341897 chatchat-0.0.6/
--rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 11:53:27.000000 chatchat-0.0.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 11:53:33.341897 chatchat-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 11:53:27.000000 chatchat-0.0.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:53:33.341897 chatchat-0.0.6/chatchat/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 11:53:27.000000 chatchat-0.0.6/chatchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4013 2024-05-21 11:53:27.000000 chatchat-0.0.6/chatchat/baidu.py
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 11:53:27.000000 chatchat-0.0.6/chatchat/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 11:53:27.000000 chatchat-0.0.6/chatchat/xunfei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 11:53:33.341897 chatchat-0.0.6/chatchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 11:53:33.000000 chatchat-0.0.6/chatchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 11:53:33.000000 chatchat-0.0.6/chatchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 11:53:33.000000 chatchat-0.0.6/chatchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 11:53:33.000000 chatchat-0.0.6/chatchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 11:53:33.000000 chatchat-0.0.6/chatchat.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 11:53:33.341897 chatchat-0.0.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 11:53:27.000000 chatchat-0.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (127)    18092 2024-05-21 23:02:47.000000 chatchat-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 23:02:50.852342 chatchat-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:47.000000 chatchat-0.0.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/chatchat/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/baidu.py
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3971 2024-05-21 23:02:47.000000 chatchat-0.0.7/chatchat/xunfei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:02:50.852342 chatchat-0.0.7/chatchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      518 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      260 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-21 23:02:50.000000 chatchat-0.0.7/chatchat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:02:50.852342 chatchat-0.0.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-21 23:02:47.000000 chatchat-0.0.7/setup.py
```

### Comparing `chatchat-0.0.6/LICENSE` & `chatchat-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.6/PKG-INFO` & `chatchat-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.6/chatchat/baidu.py` & `chatchat-0.0.7/chatchat/baidu.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,41 +67,40 @@
             jdata.update({'baidu': self.jdata})
             self.write_json(self.jfile, jdata)
 
     def get_access_token(self):
         self.update_access_token()
         return self.jdata['access_token']
 
-    def create(self, message):
-        jmsg = {
-            "messages": [
-                {
-                    "role": "user",
-                    "content": message,
-                }
-            ]
-        }
+    def send_messages(self, messages: list):
+        jmsg = {"messages": messages}
         url = f'{self.api}?access_token={self.get_access_token()}'
         r = self.client.post(url, headers=self.headers, json=jmsg)
         return r.json()
 
+    def create(self, message):
+        messages = [
+            {
+                "role": "user",
+                "content": message,
+            }
+        ]
+        return self.send_messages(messages)
+
 class Chat(Completion):
     def __init__(self, jfile, model='ERNIE-Speed-8K', history=[]):
         super().__init__(jfile, model=model)
         self.history = history
 
     def chat(self, message):
         self.history.append({
             "role": "user",
             "content": message,
         })
-        message = {"messages": self.history}
-        payload = json.dumps(message)
-        url = f'{self.api}?access_token={self.get_access_token()}'
-        r = self.client.post(url, headers=self.headers, data=payload).json()
+        r = self.send_messages(self.history)
         if 'result' in r:
             self.history.append({
                 "role": "assistant",
                 "content": r['result']
             })
 
         return r
```

### Comparing `chatchat-0.0.6/chatchat/xunfei.py` & `chatchat-0.0.7/chatchat/xunfei.py`

 * *Files identical despite different names*

### Comparing `chatchat-0.0.6/chatchat.egg-info/PKG-INFO` & `chatchat-0.0.7/chatchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chatchat
-Version: 0.0.6
+Version: 0.0.7
 Summary: Large Language Model API
 Home-page: https://github.com/JiauZhang/chatchat
 Author: JiauZhang
 Author-email: jiauzhang@163.com
 License: GPL-2.0
 Keywords: llm,chatapi,chatbot
 Classifier: Intended Audience :: Developers
```

### Comparing `chatchat-0.0.6/setup.py` & `chatchat-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name = 'chatchat',
     packages = find_packages(exclude=['examples']),
-    version = '0.0.6',
+    version = '0.0.7',
     license = 'GPL-2.0',
     description = 'Large Language Model API',
     author = 'JiauZhang',
     author_email = 'jiauzhang@163.com',
     url = 'https://github.com/JiauZhang/chatchat',
     long_description=open("README.md", "r", encoding="utf-8").read(),
     long_description_content_type = 'text/markdown',
```

