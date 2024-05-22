# Comparing `tmp/wwbot-0.0.8rc0.tar.gz` & `tmp/wwbot-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwbot-0.0.8rc0.tar", last modified: Mon May 20 13:54:53 2024, max compression
+gzip compressed data, was "wwbot-0.0.9.tar", last modified: Mon May 20 14:27:50 2024, max compression
```

## Comparing `wwbot-0.0.8rc0.tar` & `wwbot-0.0.9.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:53.110141 wwbot-0.0.8rc0/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-20 13:54:53.110141 wwbot-0.0.8rc0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 13:54:53.110141 wwbot-0.0.8rc0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1114 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:53.106141 wwbot-0.0.8rc0/wwbot/
--rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:53.106141 wwbot-0.0.8rc0/wwbot/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/lib/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:53.110141 wwbot-0.0.8rc0/wwbot/msg/
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/file_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/image_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/link_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/location_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/markdown_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/mpnews_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/news_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/text_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/textcard_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/video_msg.py
--rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 13:54:47.000000 wwbot-0.0.8rc0/wwbot/msg/voice_msg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 13:54:53.110141 wwbot-0.0.8rc0/wwbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-20 13:54:53.000000 wwbot-0.0.8rc0/wwbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 13:54:53.000000 wwbot-0.0.8rc0/wwbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 13:54:53.000000 wwbot-0.0.8rc0/wwbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 13:54:53.000000 wwbot-0.0.8rc0/wwbot.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:50.608247 wwbot-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 14:27:50.608247 wwbot-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 14:27:50.608247 wwbot-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-20 14:27:45.000000 wwbot-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:50.604247 wwbot-0.0.9/wwbot/
+-rw-r--r--   0 runner    (1001) docker     (127)    12360 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:50.604247 wwbot-0.0.9/wwbot/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4505 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/lib/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:50.608247 wwbot-0.0.9/wwbot/msg/
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/file_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/image_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/link_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1770 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/location_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/markdown_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/mpnews_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/news_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/text_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/textcard_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/video_msg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1812 2024-05-20 14:27:45.000000 wwbot-0.0.9/wwbot/msg/voice_msg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 14:27:50.608247 wwbot-0.0.9/wwbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-20 14:27:50.000000 wwbot-0.0.9/wwbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      465 2024-05-20 14:27:50.000000 wwbot-0.0.9/wwbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 14:27:50.000000 wwbot-0.0.9/wwbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-20 14:27:50.000000 wwbot-0.0.9/wwbot.egg-info/top_level.txt
```

### Comparing `wwbot-0.0.8rc0/PKG-INFO` & `wwbot-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.8rc0
+Version: 0.0.9
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

### Comparing `wwbot-0.0.8rc0/setup.py` & `wwbot-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 long_description = '''
 Please refer to the homepage of the library
 '''
 
 setuptools.setup(
   name="wwbot",
-  version="0.0.8c",
+  version="0.0.9",
   author="tbbatbb",
   author_email="20682299+tbbatbb@users.noreply.github.com",
   description="A library for dealing with messages in WeWork",
   url="https://github.com/tbbatbb/WeWorkBot",
   long_description_content_type='text/markdown',
   long_description=long_description,
   packages=setuptools.find_packages(),
```

### Comparing `wwbot-0.0.8rc0/wwbot/__init__.py` & `wwbot-0.0.9/wwbot/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/lib/logger.py` & `wwbot-0.0.9/wwbot/lib/logger.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/__init__.py` & `wwbot-0.0.9/wwbot/msg/__init__.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/file_msg.py` & `wwbot-0.0.9/wwbot/msg/file_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/image_msg.py` & `wwbot-0.0.9/wwbot/msg/image_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/link_msg.py` & `wwbot-0.0.9/wwbot/msg/link_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/location_msg.py` & `wwbot-0.0.9/wwbot/msg/location_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/markdown_msg.py` & `wwbot-0.0.9/wwbot/msg/markdown_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/mpnews_msg.py` & `wwbot-0.0.9/wwbot/msg/mpnews_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/news_msg.py` & `wwbot-0.0.9/wwbot/msg/news_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/text_msg.py` & `wwbot-0.0.9/wwbot/msg/text_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/textcard_msg.py` & `wwbot-0.0.9/wwbot/msg/textcard_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/video_msg.py` & `wwbot-0.0.9/wwbot/msg/video_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot/msg/voice_msg.py` & `wwbot-0.0.9/wwbot/msg/voice_msg.py`

 * *Files identical despite different names*

### Comparing `wwbot-0.0.8rc0/wwbot.egg-info/PKG-INFO` & `wwbot-0.0.9/wwbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwbot
-Version: 0.0.8rc0
+Version: 0.0.9
 Summary: A library for dealing with messages in WeWork
 Home-page: https://github.com/tbbatbb/WeWorkBot
 Author: tbbatbb
 Author-email: 20682299+tbbatbb@users.noreply.github.com
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
```

