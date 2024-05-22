# Comparing `tmp/nonebot_plugin_authrespond-1.1.tar.gz` & `tmp/nonebot_plugin_authrespond-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_authrespond-1.1.tar", last modified: Wed May 22 07:51:49 2024, max compression
+gzip compressed data, was "nonebot_plugin_authrespond-1.2.tar", last modified: Wed May 22 08:06:28 2024, max compression
```

## Comparing `nonebot_plugin_authrespond-1.1.tar` & `nonebot_plugin_authrespond-1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/
--rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/cubp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/plugins_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/session.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.982124 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/cubp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/plugins_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 08:06:28.000000 nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 08:06:20.000000 nonebot_plugin_authrespond-1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:06:28.986124 nonebot_plugin_authrespond-1.2/setup.cfg
```

### Comparing `nonebot_plugin_authrespond-1.1/LICENSE` & `nonebot_plugin_authrespond-1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/PKG-INFO` & `nonebot_plugin_authrespond-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.1
+Version: 1.2
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.1/README.md` & `nonebot_plugin_authrespond-1.2/README.md`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/cubp.py` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/cubp.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/perm.py` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/perm.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/plugins_data.py` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/run.py` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond/run.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/PKG-INFO` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.1
+Version: 1.2
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/SOURCES.txt` & `nonebot_plugin_authrespond-1.2/nonebot_plugin_authrespond.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.1/pyproject.toml` & `nonebot_plugin_authrespond-1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-authrespond"
-version = "1.1"
+version = "1.2"
 description = "nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
```

