# Comparing `tmp/nonebot_plugin_authrespond-1.0.tar.gz` & `tmp/nonebot_plugin_authrespond-1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nonebot_plugin_authrespond-1.0.tar", last modified: Tue May 21 07:22:09 2024, max compression
+gzip compressed data, was "nonebot_plugin_authrespond-1.1.tar", last modified: Wed May 22 07:51:49 2024, max compression
```

## Comparing `nonebot_plugin_authrespond-1.0.tar` & `nonebot_plugin_authrespond-1.1.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:09.605194 nonebot_plugin_authrespond-1.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    44009 2024-05-21 07:22:09.605194 nonebot_plugin_authrespond-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2829 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:09.601194 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1754 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/cubp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/perm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/plugins_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/run.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 07:22:09.605194 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    44009 2024-05-21 07:22:09.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-05-21 07:22:09.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 07:22:09.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-21 07:22:09.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-21 07:22:09.000000 nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-21 07:22:05.000000 nonebot_plugin_authrespond-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 07:22:09.605194 nonebot_plugin_authrespond-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2944 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2203 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/cubp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/perm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/plugins_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/session.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44124 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-22 07:51:49.000000 nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-22 07:51:45.000000 nonebot_plugin_authrespond-1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:51:49.763566 nonebot_plugin_authrespond-1.1/setup.cfg
```

### Comparing `nonebot_plugin_authrespond-1.0/LICENSE` & `nonebot_plugin_authrespond-1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.0/PKG-INFO` & `nonebot_plugin_authrespond-1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.0
+Version: 1.1
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,31 +682,29 @@
 Project-URL: repository, https://github.com/cubstaryow/nonebot-plugin-authrespond
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
+Requires-Dist: nonebot-plugin-session
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-<div align="center">
-
 # nonebot-plugin-authrespond
 
-_✨ nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局 ✨_
+_✨ nonebot简单易用的黑名单插件，全平台支持，实现分插件拉黑用户/群聊/全局 ✨_
 
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/owner/nonebot-plugin-authrespond.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-authrespond">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-authrespond.svg" alt="pypi">
@@ -718,14 +716,18 @@
 
 ## 📖 介绍
 
 简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局,无需修改插件源码
 
 原理为插件运行前监听Matcher响应器属性
 
+全平台支持,但是 二级群组可能存在问题
+
+仅在 onebotV11 测试过,其余平台出现问题请提issue
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-authrespond
```

### Comparing `nonebot_plugin_authrespond-1.0/README.md` & `nonebot_plugin_authrespond-1.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -2,19 +2,17 @@
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-<div align="center">
-
 # nonebot-plugin-authrespond
 
-_✨ nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局 ✨_
+_✨ nonebot简单易用的黑名单插件，全平台支持，实现分插件拉黑用户/群聊/全局 ✨_
 
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/owner/nonebot-plugin-authrespond.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-authrespond">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-authrespond.svg" alt="pypi">
@@ -26,14 +24,18 @@
 
 ## 📖 介绍
 
 简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局,无需修改插件源码
 
 原理为插件运行前监听Matcher响应器属性
 
+全平台支持,但是 二级群组可能存在问题
+
+仅在 onebotV11 测试过,其余平台出现问题请提issue
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-authrespond
```

#### html2text {}

```diff
@@ -1,29 +1,31 @@
                               _[_N_o_n_e_B_o_t_P_l_u_g_i_n_L_o_g_o_]
                               [NoneBotPluginText]
                        # nonebot-plugin-authrespond _â¨
-  nonebotç®åæç¨çé»ååæä»¶ï¼å®ç°åæä»¶æé»ç¨æ·/ç¾¤è/
-                      å¨å± â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
- ## ð ä»ç» ç®åæç¨çé»ååæä»¶ï¼å®ç°åæä»¶æé»ç¨æ·/
-                    ç¾¤è/å¨å±,æ éä¿®æ¹æä»¶æºç 
-åçä¸ºæä»¶è¿è¡åçå¬Matcherååºå¨å±æ§ ## ð¿ å®è£ ä½¿ç¨ nb-
-         cli å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
-  è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-authrespond
-        ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
- æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
-    pip pip install nonebot-plugin-authrespond pdm pdm add nonebot-plugin-
- authrespond poetry poetry add nonebot-plugin-authrespond conda conda install
-       nonebot-plugin-authrespond æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
-  `pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
-         ["nonebot_plugin_authrespond"] ## âï¸ éç½® å¨ nonebot2
- é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
+nonebotç®åæç¨çé»ååæä»¶ï¼å¨å¹³å°æ¯æï¼å®ç°åæä»¶æé»ç¨æ·/
+                   ç¾¤è/å¨å± â¨__[_l_i_c_e_n_s_e_]_[_p_y_p_i_][python]
+## ð ä»ç» ç®åæç¨çé»ååæä»¶ï¼å®ç°åæä»¶æé»ç¨æ·/
+ç¾¤è/å¨å±,æ éä¿®æ¹æä»¶æºç 
+åçä¸ºæä»¶è¿è¡åçå¬Matcherååºå¨å±æ§ å¨å¹³å°æ¯æ,ä½æ¯
+äºçº§ç¾¤ç»å¯è½å­å¨é®é¢ ä»å¨ onebotV11
+æµè¯è¿,å¶ä½å¹³å°åºç°é®é¢è¯·æissue ## ð¿ å®è£ ä½¿ç¨ nb-cli
+å®è£ å¨ nonebot2 é¡¹ç®çæ ¹ç®å½ä¸æå¼å½ä»¤è¡,
+è¾å¥ä»¥ä¸æä»¤å³å¯å®è£ nb plugin install nonebot-plugin-authrespond
+ä½¿ç¨åç®¡çå¨å®è£ å¨ nonebot2 é¡¹ç®çæä»¶ç®å½ä¸,
+æå¼å½ä»¤è¡, æ ¹æ®ä½ ä½¿ç¨çåç®¡çå¨, è¾å¥ç¸åºçå®è£å½ä»¤
+pip pip install nonebot-plugin-authrespond pdm pdm add nonebot-plugin-
+authrespond poetry poetry add nonebot-plugin-authrespond conda conda install
+nonebot-plugin-authrespond æå¼ nonebot2 é¡¹ç®æ ¹ç®å½ä¸ç
+`pyproject.toml` æä»¶, å¨ `[tool.nonebot]` é¨åè¿½å åå¥ plugins =
+["nonebot_plugin_authrespond"] ## âï¸ éç½® å¨ nonebot2
+é¡¹ç®ç`.env`æä»¶ä¸­æ·»å ä¸è¡¨ä¸­çå¿å¡«éç½® | éç½®é¡¹ | å¿å¡« |
 é»è®¤å¼ | è¯´æ | |:-----:|:----:|:----:|:----:| | cubplugin_datadir | å¦ |
-    "" | èªå®ä¹éç½®æä»¶è·¯å¾,é»è®¤localstore | ## ð ä½¿ç¨ ###
+"" | èªå®ä¹éç½®æä»¶è·¯å¾,é»è®¤localstore | ## ð ä½¿ç¨ ###
 æä»¤è¡¨ | æä»¤ | æé | éè¦@ | èå´ | è¯´æ | |:-----:|:----:|:---
- -:|:----:|:----:| | #(å¨å±/æä»¶åç§°)(æé»/è§£é»)(å¨å/ç¨æ·id) |
- ä¸»äºº | å¦ | ç§è/ç¾¤è | ç¨æ·æä½æ¨¡å¼ | | #(å¨å±/æä»¶åç§°)
- (å°ç¦ç¾¤/è§£ç¦ç¾¤)(ç¾¤å·/çç©ºå°ç¦æå¨ç¾¤) | ä¸»äºº | å¦ | ç§è/
-                   ç¾¤è | ç¾¤èæä½æ¨¡å¼ | > [!tips] >
-    æä»¶åç§°ä¸ºnonebotå¯¼å¥çæä»¶,æ¯å¦nonebot_plugin_cyberfurry >
-             ä¹å¯ä»¥ä½¿ç¨cyberfurry(å³å»ænonebot_plugin_) >
-   æä»¶åç§°æ£æ¥æ¥æºä¸º: nonebot.get_loaded_plugins() ä¸­åå±æ§ç
-                                  plugin.name
+-:|:----:|:----:| | #(å¨å±/æä»¶åç§°)(æé»/è§£é»)(å¨å/ç¨æ·id) |
+ä¸»äºº | å¦ | ç§è/ç¾¤è | ç¨æ·æä½æ¨¡å¼ | | #(å¨å±/æä»¶åç§°)
+(å°ç¦ç¾¤/è§£ç¦ç¾¤)(ç¾¤å·/çç©ºå°ç¦æå¨ç¾¤) | ä¸»äºº | å¦ | ç§è/
+ç¾¤è | ç¾¤èæä½æ¨¡å¼ | > [!tips] >
+æä»¶åç§°ä¸ºnonebotå¯¼å¥çæä»¶,æ¯å¦nonebot_plugin_cyberfurry >
+ä¹å¯ä»¥ä½¿ç¨cyberfurry(å³å»ænonebot_plugin_) >
+æä»¶åç§°æ£æ¥æ¥æºä¸º: nonebot.get_loaded_plugins() ä¸­åå±æ§ç
+plugin.name
```

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/__init__.py` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,14 @@
 
     homepage="https://github.com/cubstaryow/nonebot-plugin-authrespond",
     # 发布必填。
 
     config=cubplugins_permission,
     # 插件配置项类，如无需配置可不填写。
 
-    supported_adapters={"~onebot.v11"},
+    supported_adapters={},
     # 支持的适配器集合，其中 `~` 在此处代表前缀 `nonebot.adapters.`，其余适配器亦按此格式填写。
     # 若插件可以保证兼容所有适配器（即仅使用基本适配器功能）可不填写，否则应该列出插件支持的适配器。
 )
 
 from .run import *
 from .perm import *
```

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/cubp.py` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/cubp.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,39 +8,53 @@
 class cubplugins_permission:
     cubplugins_P = rdata(conf_name)
 
     def __init__(self):
         pass
     
     def savedata(self):
+        '''保存数据至本地文件
+        '''
         wdata(conf_name,self.cubplugins_P)
     
     def checkperm(self , modulename:str , user_id:str ):
+        '''
+        检查对用户是否阻断响应 True 阻断 False 响应
+        '''
         globaldata = self.cubplugins_P.get('global',[])
         if user_id in globaldata:
             return True
         if self.cubplugins_P.get(modulename,None) == None:
             return False
         data = self.cubplugins_P[modulename]
         if user_id in data or '0' in data:
             return True
         return False
     
     def checkpermgroup(self , modulename:str , group_id:str ):
+        '''
+        检查对群组是否阻断响应 True 阻断 False 响应
+        '''
         groupdata = self.cubplugins_P.get('group-global',[])
         if group_id in groupdata:
             return True
         if self.cubplugins_P.get('group-'+modulename,None) == None:
             return False
         data = self.cubplugins_P['group-'+modulename]
         if group_id in data:
             return True
         return False
     
     def setperm(self , modulename:str , user_id:str , allow : bool =False):
+        '''
+        设定权限
+        modulename : 插件名称 (组模式则为group-xxxxxx)
+        user_id : 用户id (组模式传入组ID)
+        allow : 是否允许响应 (False则将id拉黑)
+        '''
         if self.cubplugins_P.get(modulename,None) == None:
             self.cubplugins_P[modulename] =[]
         data = self.cubplugins_P[modulename]
         check = False
         if allow:
             if user_id in data:
                 data.remove(user_id)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/perm.py` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/perm.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,97 @@
 from nonebot import get_loaded_plugins, on_regex
-from nonebot.adapters.onebot.v11 import(
-    Bot,
-    Message,
-    MessageEvent,
-    GroupMessageEvent
-)
+
+from nonebot.adapters import Message ,Event
 from nonebot.matcher import Matcher
 from nonebot.permission import SUPERUSER
 from nonebot.params import RegexGroup
 from .cubp import cubp
+from .session import  EventSession
+try :
+    from nonebot.adapters.onebot.v11 import Message as V11Message
+except:
+    V11Message = Message
+    pass
 
 turn_push = on_regex(
-    r"^#(.*)(拉黑|解黑|封禁群|解禁群)(.*)$",
+    r"^#([\S|-]*)(拉黑|解黑|封禁群|解禁群)([\S|-]*)$",
     block=True,
     priority=2,
     permission=SUPERUSER
 )
 @turn_push.handle()
 async def _(
-    event : MessageEvent,
+    event:Event,
     matcher : Matcher,
+    session: EventSession,
     args : list = RegexGroup(),
 ):
+    
     modulename = args[0]
     if modulename.startswith("nonebot_plugin_"):
         modulename = modulename.replace("nonebot_plugin_", "")
     pluginslist = await getpluginslist()
     if  modulename not in pluginslist and modulename not in ["全局","all"]:
         await matcher.finish("[Failed]不存在此模块")
     if modulename in ["全局","all"] :
         modulename = "global"
     isgroupmode = False
+    
+    
     if "群" in str(args[1]):
         modulename = "group-"+modulename
         isgroupmode =True
     
-    uid = Message(args[2].strip())
+    if session.platform == "qq":
+        uid = V11Message(args[2].strip())
+        atuid = uid['at']
+    else:
+        #其余平台的AT以后再说（
+        atuid = []
+        
+        
     if args[2] =="":
         if isgroupmode:
-            if isinstance(event , GroupMessageEvent):
-                user_id = str(event.group_id)
+            if session.level >=2:
+                user_id = str(session.id2)
             else:
                 await matcher.finish("[Failed]群组操作模式下缺失关键参数")
         else:
             await matcher.finish("[Failed]用户操作模式下缺失关键参数")
     elif  args[2] in ["全员","全体成员" , "all"]:
         if isgroupmode:
             await matcher.finish("[Failed]群组操作模式下无法操作全体(虽然支持但是请使用用户模式)")
         else:
             user_id = "0"
-    elif len(uid['at']) == 0:
+    elif len(atuid) == 0:
         user_id = args[2].strip()
     else:
-        user_id = uid['at'][0].data["qq"]
+        user_id = atuid[0].data["qq"]
+
 
-    user = user_id if user_id != "0" else "全局(插件停用)"
+    user = user_id if user_id != "0" else "全局(插件停启用)"
     user = "群"+user if isgroupmode else user
     check = False
     mode="禁止"
     if str(args[1]) in ["解禁","解黑","解禁群"]:
         check = True
         mode="允许"
+        
     ret = cubp.setperm(modulename,user_id,check)
+    
+    
     msg = f"[cubp-W]操作失败,可能已经{str(args[1])}"
     if ret:
         msg = f"[cubp-I]已{mode}{modulename}响应{user}"
     await matcher.finish(msg)
     
 async def getpluginslist():
+    """获取插件列表
+        return: list[pluginname]
+    """
     plugin_set = get_loaded_plugins()
     plugin_names = []
     for plugin in plugin_set:
         if plugin.name.startswith("nonebot_plugin_"):
             plugin_names.append(plugin.name.replace("nonebot_plugin_", ""))
         else:
             plugin_names.append(plugin.name)
```

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/plugins_data.py` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/plugins_data.py`

 * *Files identical despite different names*

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond/run.py` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond/run.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,44 +1,58 @@
 from loguru import logger
 from nonebot import get_driver
 from nonebot.matcher import Matcher
-from nonebot.adapters.onebot.v11 import (
-    MessageEvent , GroupMessageEvent
-)
-from nonebot.message import  run_preprocessor
+from nonebot.adapters import Message, Event, Bot
+from nonebot.message import run_preprocessor
 from nonebot.exception import IgnoredException
 from .cubp import cubp
+from .session import EventSession
 
 superusers = get_driver().config.superusers
 
+
 @run_preprocessor
-async def pass_rule(event: MessageEvent,matcher:Matcher):
-    user_id = str(event.user_id)
+async def pass_run(
+    bot: Bot,
+    event: Event,
+    matcher: Matcher,
+    session: EventSession,
+):
+    user_id = str(session.id1)
+    await pass_rule(user_id, matcher)
+    if session.level >= 2:
+        await passgroup_rule(user_id, session.id2, matcher)
+        if session.level == 3:
+            await passgroup_rule(user_id, session.id3, matcher)
+            #子ID也支持但是可能会有冲突
+    pass
+
+
+async def pass_rule(user_id: str, matcher: Matcher):
+
     modulename = matcher.plugin.name
     if modulename.startswith("nonebot_plugin_"):
         modulename = modulename.replace("nonebot_plugin_", "")
-    msg =f"plugin {modulename} is responses by {user_id}, check permission!"
+    msg = f"plugin {modulename} is responses by {user_id}, check permission!"
     logger.opt(colors=True).debug(msg)
-    if  cubp.checkperm(modulename,user_id):
+    if cubp.checkperm(modulename, user_id):
         msg = f"ID {user_id} is not allow run {modulename}"
         logger.opt(colors=True).warning(msg)
         if user_id in superusers:
             return
         raise IgnoredException(msg) from None
     return True
 
-@run_preprocessor
-async def passgroup_rule(event: GroupMessageEvent,matcher:Matcher):
-    group_id = str(event.group_id)
-    user_id = str(event.user_id)
+
+async def passgroup_rule(user_id: str, group_id: str, matcher: Matcher):
     modulename = matcher.plugin.name
     if modulename.startswith("nonebot_plugin_"):
         modulename = modulename.replace("nonebot_plugin_", "")
-    msg =f"plugin {modulename} is responses by group {group_id}, check permission!"
+    msg = f"plugin {modulename} is responses by group {group_id}, check permission!"
     logger.opt(colors=True).debug(msg)
-    if  cubp.checkpermgroup(modulename,group_id):
+    if cubp.checkpermgroup(modulename, group_id):
         msg = f"ID {group_id} group is not allow run {modulename}"
         logger.opt(colors=True).warning(msg)
         if user_id in superusers:
             return
         raise IgnoredException(msg) from None
     return True
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `nonebot_plugin_authrespond-1.0/nonebot_plugin_authrespond.egg-info/PKG-INFO` & `nonebot_plugin_authrespond-1.1/nonebot_plugin_authrespond.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nonebot-plugin-authrespond
-Version: 1.0
+Version: 1.1
 Summary: nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局
 Author: cubstaryow
 Author-email: cub_staryow@outlook.com
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -682,31 +682,29 @@
 Project-URL: repository, https://github.com/cubstaryow/nonebot-plugin-authrespond
 Keywords: egg,bacon,sausage,tomatoes,Lobster Thermidor
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: nonebot-adapter-onebot
 Requires-Dist: nonebot2
 Requires-Dist: nonebot-plugin-localstore
+Requires-Dist: nonebot-plugin-session
 
 <div align="center">
   <a href="https://v2.nonebot.dev/store"><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/nbp_logo.png" width="180" height="180" alt="NoneBotPluginLogo"></a>
   <br>
   <p><img src="https://github.com/cubstaryow/nonebot-plugin-authrespond/blob/master/.github/NoneBotPlugin.svg" width="240" alt="NoneBotPluginText"></p>
 </div>
 
 <div align="center">
 
-<div align="center">
-
 # nonebot-plugin-authrespond
 
-_✨ nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局 ✨_
+_✨ nonebot简单易用的黑名单插件，全平台支持，实现分插件拉黑用户/群聊/全局 ✨_
 
 
 <a href="./LICENSE">
     <img src="https://img.shields.io/github/license/owner/nonebot-plugin-authrespond.svg" alt="license">
 </a>
 <a href="https://pypi.python.org/pypi/nonebot-plugin-authrespond">
     <img src="https://img.shields.io/pypi/v/nonebot-plugin-authrespond.svg" alt="pypi">
@@ -718,14 +716,18 @@
 
 ## 📖 介绍
 
 简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局,无需修改插件源码
 
 原理为插件运行前监听Matcher响应器属性
 
+全平台支持,但是 二级群组可能存在问题
+
+仅在 onebotV11 测试过,其余平台出现问题请提issue
+
 ## 💿 安装
 
 <details open>
 <summary>使用 nb-cli 安装</summary>
 在 nonebot2 项目的根目录下打开命令行, 输入以下指令即可安装
 
     nb plugin install nonebot-plugin-authrespond
```

### Comparing `nonebot_plugin_authrespond-1.0/pyproject.toml` & `nonebot_plugin_authrespond-1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nonebot-plugin-authrespond"
-version = "1.0"
+version = "1.1"
 description = "nonebot简单易用的黑名单插件，实现分插件拉黑用户/群聊/全局"
 readme = "README.md"
 requires-python = ">=3.10"
 license = {file = "LICENSE"}
 keywords = ["egg", "bacon", "sausage", "tomatoes", "Lobster Thermidor"]
 authors = [
   {email = "cub_staryow@outlook.com"},
@@ -12,14 +12,14 @@
 ]
 classifiers = [
   "Development Status :: 4 - Beta",
   "Programming Language :: Python"
 ]
 
 dependencies = [
-  "nonebot-adapter-onebot",
   "nonebot2",
-  "nonebot-plugin-localstore"
+  "nonebot-plugin-localstore",
+  "nonebot-plugin-session"
 ]
 
 [project.urls]
 repository = "https://github.com/cubstaryow/nonebot-plugin-authrespond"
```

