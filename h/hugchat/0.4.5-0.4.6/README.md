# Comparing `tmp/hugchat-0.4.5.tar.gz` & `tmp/hugchat-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.4.5.tar", last modified: Sat May  4 02:54:09 2024, max compression
+gzip compressed data, was "hugchat-0.4.6.tar", last modified: Wed May 22 03:08:33 2024, max compression
```

## Comparing `hugchat-0.4.5.tar` & `hugchat-0.4.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:09.410078 hugchat-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-04 02:54:05.000000 hugchat-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-04 02:54:09.406078 hugchat-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-04 02:54:05.000000 hugchat-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 02:54:09.410078 hugchat-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-04 02:54:05.000000 hugchat-0.4.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:09.406078 hugchat-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:09.406078 hugchat-0.4.5/src/hugchat/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/hugchat.py
--rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/message.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:09.406078 hugchat-0.4.5/src/hugchat/types/
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/types/assistant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/types/message.py
--rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-04 02:54:05.000000 hugchat-0.4.5/src/hugchat/types/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 02:54:09.406078 hugchat-0.4.5/src/hugchat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-04 02:54:09.000000 hugchat-0.4.5/src/hugchat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-04 02:54:09.000000 hugchat-0.4.5/src/hugchat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 02:54:09.000000 hugchat-0.4.5/src/hugchat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-04 02:54:09.000000 hugchat-0.4.5/src/hugchat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 02:54:09.000000 hugchat-0.4.5/src/hugchat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    34523 2024-05-22 03:08:29.000000 hugchat-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 03:08:33.041164 hugchat-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5729 2024-05-22 03:08:29.000000 hugchat-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 03:08:33.041164 hugchat-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-22 03:08:29.000000 hugchat-0.4.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.037163 hugchat-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10354 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30347 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/hugchat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8696 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7455 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/message.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/assistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/message.py
+-rw-r--r--   0 runner    (1001) docker     (127)      988 2024-05-22 03:08:29.000000 hugchat-0.4.6/src/hugchat/types/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 03:08:33.041164 hugchat-0.4.6/src/hugchat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 03:08:33.000000 hugchat-0.4.6/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.4.5/LICENSE` & `hugchat-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/PKG-INFO` & `hugchat-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.5
+Version: 0.4.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `hugchat-0.4.5/README.md` & `hugchat-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/setup.py` & `hugchat-0.4.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.4.5",
+    version="0.4.6",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.4.5/src/hugchat/cli.py` & `hugchat-0.4.6/src/hugchat/cli.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat/exceptions.py` & `hugchat-0.4.6/src/hugchat/exceptions.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat/hugchat.py` & `hugchat-0.4.6/src/hugchat/hugchat.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat/login.py` & `hugchat-0.4.6/src/hugchat/login.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat/message.py` & `hugchat-0.4.6/src/hugchat/message.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,21 +13,19 @@
 MSGSTATUS_RESOLVED = 1
 MSGSTATUS_REJECTED = 2
 
 
 class WebSearchSource:
     title: str
     link: str
-    hostname: str
 
     def __str__(self):
         return json.dumps({
             "title": self.title,
             "link": self.link,
-            "hostname": self.hostname,
         })
 
 
 class Message(Generator):
     """
     :Args:
         * g: Generator
@@ -108,15 +106,14 @@
                 if message_type != MSGTYPE_ERROR and a.__contains__("sources"):
                     self.web_search_sources.clear()
                     sources = a["sources"]
                     for source in sources:
                         wss = WebSearchSource()
                         wss.title = source["title"]
                         wss.link = source["link"]
-                        wss.hostname = source["hostname"]
                         self.web_search_sources.append(wss)
             elif "messageType" in a:
                 message_type: str = a["messageType"]
                 if message_type == MSGTYPE_ERROR:
                     self.error = ChatError(a["message"])
                     self.msg_status = MSGSTATUS_REJECTED
                 if t == RESPONSE_TYPE_STREAM:
```

### Comparing `hugchat-0.4.5/src/hugchat/types/message.py` & `hugchat-0.4.6/src/hugchat/types/message.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat/types/model.py` & `hugchat-0.4.6/src/hugchat/types/model.py`

 * *Files identical despite different names*

### Comparing `hugchat-0.4.5/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.4.6/src/hugchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.4.5
+Version: 0.4.6
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

