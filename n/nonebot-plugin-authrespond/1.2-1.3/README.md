# Comparing `tmp/nonebot_plugin_authrespond-1.2.tar.gz` & `tmp/nonebot_plugin_authrespond-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_authrespond-1.2.tar", last modified: Wed May 22 08:06:28 2024, max compression
+gzip compressed data, was "nonebot_plugin_authrespond-1.3.tar", last modified: Wed May 22 09:38:42 2024, max compression
```

## Comparing `nonebot_plugin_authrespond-1.2.tar` & `nonebot_plugin_authrespond-1.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.982124 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/cubp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/plugins_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:38:42.874385 nonebot_plugin_authrespond-1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-22 09:38:42.874385 nonebot_plugin_authrespond-1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:38:42.874385 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/cubp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3008 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/plugins_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:38:42.874385 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44162 2024-05-22 09:38:42.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 09:38:42.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:38:42.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 09:38:42.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 09:38:42.000000 nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-05-22 09:38:38.000000 nonebot_plugin_authrespond-1.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:38:42.874385 nonebot_plugin_authrespond-1.3/setup.cfg
```

### Comparing `nonebot_plugin_authrespond-1.2/LICENSE` & `nonebot_plugin_authrespond-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/PKG-INFO` & `nonebot_plugin_authrespond-1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.2
+Version: 1.3
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: nonebot-plugin-session
+Requires-Dist: nonebot-plugin-alconna
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

### Comparing `nonebot_plugin_authrespond-1.2/README.md` & `nonebot_plugin_authrespond-1.3/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/__init__.py` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,8 +31,9 @@
         "~dodo"
         }
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 from .run import *
-from .perm import *
+
+from .perm import *
```

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/cubp.py` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/cubp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/perm.py` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/perm.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from nonebot.adapters import Message ,Event
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.params import RegexGroup
 from .cubp import cubp
 from .session import  EventSession
+from nonebot_plugin_alconna import UniMessage , At
 try :
     from nonebot.adapters.onebot.v11 import Message as V11Message
 except:
     V11Message = Message
     pass
 
 turn_push = on_regex(
@@ -36,23 +37,21 @@
         modulename = "global"
     isgroupmode = False
     
     
     if "群" in str(args[1]):
         modulename = "group-"+modulename
         isgroupmode =True
-    
-    if session.platform == "qq":
-        uid = V11Message(args[2].strip())
-        atuid = uid['at']
-    else:
-        #其余平台的AT以后再说（
-        atuid = []
-        
         
+    uni_msg = UniMessage()
+    if args[2]:
+        msg: Message = event.get_message()
+        uni_msg = UniMessage.generate_without_reply(message=msg)
+    atuid = uni_msg.get(At)
+
     if args[2] =="":
         if isgroupmode:
             if session.level >=2:
                 user_id = str(session.id2)
             else:
                 await matcher.finish("[Failed]群组操作模式下缺失关键参数")
         else:
@@ -61,15 +60,16 @@
         if isgroupmode:
             await matcher.finish("[Failed]群组操作模式下无法操作全体(虽然支持但是请使用用户模式)")
         else:
             user_id = "0"
     elif len(atuid) == 0:
         user_id = args[2].strip()
     else:
-        user_id = atuid[0].data["qq"]
+        atmsg :At= atuid[0]
+        user_id = atmsg.target
 
 
     user = user_id if user_id != "0" else "全局(插件停启用)"
     user = "群"+user if isgroupmode else user
     check = False
     mode="禁止"
     if str(args[1]) in ["解禁","解黑","解禁群"]:
```

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/plugins_data.py` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/run.py` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond/run.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/PKG-INFO` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.2
+Version: 1.3
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -685,14 +685,15 @@
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
 Requires-Dist: nonebot-plugin-session
+Requires-Dist: nonebot-plugin-alconna
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
```

### Comparing `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/SOURCES.txt` & `nonebot_plugin_authrespond-1.3/nonebot_plugin_authrespond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.2/pyproject.toml` & `nonebot_plugin_authrespond-1.3/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-authrespond"
-version = "1.2"
+version = "1.3"
 description = "nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -14,12 +14,13 @@
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
   "nonebot2",
   "nonebot-plugin-localstore",
-  "nonebot-plugin-session"
+  "nonebot-plugin-session",
+  "nonebot-plugin-alconna"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-authrespond"
```

