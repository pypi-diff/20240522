# Comparing `tmp/owega-5.8.3.tar.gz` & `tmp/owega-5.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "owega-5.8.3.tar", last modified: Fri May 17 22:28:29 2024, max compression
+gzip compressed data, was "owega-5.8.4.tar", last modified: Tue May 21 22:51:09 2024, max compression
```

## Comparing `owega-5.8.3.tar` & `owega-5.8.4.tar`

### file list

```diff
@@ -1,69 +1,69 @@
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.936930 owega-5.8.3/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.8.3/LICENSE
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16889 2024-05-17 22:28:29.936930 owega-5.8.3/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-14 00:10:08.000000 owega-5.8.3/README.md
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.933930 owega-5.8.3/owega/
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/OweHandlers/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.8.3/owega/OweHandlers/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_add_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_commands.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_context.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_del_sysmem.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_dinput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_edit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1302 2024-05-17 22:06:07.000000 owega-5.8.3/owega/OweHandlers/handle_estimation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_finput.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_frequency.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_genconf.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.8.3/owega/OweHandlers/handle_history.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:20:56.000000 owega-5.8.3/owega/OweHandlers/handle_image.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_load.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_model.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_presence.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_quit.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_save.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_system.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_temperature.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-17 22:06:07.000000 owega-5.8.3/owega/OweHandlers/handle_time.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_tokens.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_top_p.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.8.3/owega/OweHandlers/handle_tts.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2470 2024-05-17 22:06:07.000000 owega-5.8.3/owega/OweHandlers/handlers.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/OwegaFun/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.8.3/owega/OwegaFun/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.8.3/owega/OwegaFun/functions.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.8.3/owega/OwegaFun/longTermSouvenirs.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.8.3/owega/OwegaFun/utility.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/OwegaSession/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.8.3/owega/OwegaSession/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3628 2024-05-17 22:06:07.000000 owega-5.8.3/owega/OwegaSession/main_bottom_toolbar.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.8.3/owega/OwegaSession/promptsession.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.8.3/owega/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.8.3/owega/__main__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10542 2024-05-17 22:27:03.000000 owega-5.8.3/owega/ask.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/changelog/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.8.3/owega/changelog/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    25751 2024-05-17 22:28:00.000000 owega-5.8.3/owega/changelog/changelog.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.8.3/owega/changelog/changelogEntry.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.8.3/owega/changelog/version.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/config/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.8.3/owega/config/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2655 2024-05-17 22:06:07.000000 owega-5.8.3/owega/config/baseConf.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega/conversation/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.8.3/owega/conversation/__init__.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.8.3/owega/conversation/conversation.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.8.3/owega/getLogger.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.8.3/owega/handlerBase.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.8.3/owega/license.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11780 2024-05-17 22:06:07.000000 owega-5.8.3/owega/owega.py
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:20:56.000000 owega-5.8.3/owega/utils.py
-drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-17 22:28:29.935930 owega-5.8.3/owega.egg-info/
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    16889 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/PKG-INFO
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/SOURCES.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/dependency_links.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/entry_points.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/requires.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-17 22:28:29.000000 owega-5.8.3/owega.egg-info/top_level.txt
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.8.3/pyproject.toml
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-17 22:28:29.936930 owega-5.8.3/setup.cfg
--rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2524 2024-05-17 22:16:16.000000 owega-5.8.3/setup.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.924870 owega-5.8.4/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6076 2024-05-10 14:44:53.000000 owega-5.8.4/LICENSE
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17070 2024-05-21 22:51:09.924870 owega-5.8.4/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5183 2024-05-14 00:10:08.000000 owega-5.8.4/README.md
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.922870 owega-5.8.4/owega/
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.923870 owega-5.8.4/owega/OweHandlers/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      156 2024-04-27 12:05:16.000000 owega-5.8.4/owega/OweHandlers/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      980 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_add_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1590 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_commands.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1185 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_context.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1601 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_del_sysmem.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_dinput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3457 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_edit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1302 2024-05-17 22:06:07.000000 owega-5.8.4/owega/OweHandlers/handle_estimation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5059 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_finput.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1816 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_frequency.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      521 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_genconf.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      523 2024-05-08 02:39:07.000000 owega-5.8.4/owega/OweHandlers/handle_history.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3246 2024-05-13 23:20:56.000000 owega-5.8.4/owega/OweHandlers/handle_image.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1118 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_load.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1698 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_model.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1791 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_presence.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      637 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_quit.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1090 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_save.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      945 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_system.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1739 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_temperature.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1339 2024-05-17 22:06:07.000000 owega-5.8.4/owega/OweHandlers/handle_time.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1404 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_tokens.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1556 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_top_p.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1245 2024-05-08 02:39:08.000000 owega-5.8.4/owega/OweHandlers/handle_tts.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2470 2024-05-17 22:06:07.000000 owega-5.8.4/owega/OweHandlers/handlers.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.923870 owega-5.8.4/owega/OwegaFun/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      873 2024-04-27 12:05:16.000000 owega-5.8.4/owega/OwegaFun/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3867 2024-04-17 02:21:38.000000 owega-5.8.4/owega/OwegaFun/functions.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     4342 2024-04-27 12:05:16.000000 owega-5.8.4/owega/OwegaFun/longTermSouvenirs.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5816 2024-04-27 12:05:16.000000 owega-5.8.4/owega/OwegaFun/utility.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.923870 owega-5.8.4/owega/OwegaSession/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      100 2024-04-17 02:21:38.000000 owega-5.8.4/owega/OwegaSession/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3628 2024-05-17 22:06:07.000000 owega-5.8.4/owega/OwegaSession/main_bottom_toolbar.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     5592 2024-04-27 12:05:16.000000 owega-5.8.4/owega/OwegaSession/promptsession.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      175 2024-05-08 02:39:08.000000 owega-5.8.4/owega/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       94 2024-04-17 02:21:38.000000 owega-5.8.4/owega/__main__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10542 2024-05-17 22:33:13.000000 owega-5.8.4/owega/ask.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.924870 owega-5.8.4/owega/changelog/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       80 2024-04-27 12:05:16.000000 owega-5.8.4/owega/changelog/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    26055 2024-05-21 22:50:17.000000 owega-5.8.4/owega/changelog/changelog.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1534 2024-04-27 12:05:16.000000 owega-5.8.4/owega/changelog/changelogEntry.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     3315 2024-04-17 02:21:38.000000 owega-5.8.4/owega/changelog/version.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.924870 owega-5.8.4/owega/config/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       86 2024-04-17 02:21:38.000000 owega-5.8.4/owega/config/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2655 2024-05-17 22:06:07.000000 owega-5.8.4/owega/config/baseConf.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.924870 owega-5.8.4/owega/conversation/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       83 2024-04-17 02:21:38.000000 owega-5.8.4/owega/conversation/__init__.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    10105 2024-05-13 22:26:17.000000 owega-5.8.4/owega/conversation/conversation.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1418 2024-05-10 10:34:51.000000 owega-5.8.4/owega/getLogger.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       64 2024-04-17 02:21:38.000000 owega-5.8.4/owega/handlerBase.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     6141 2024-05-10 14:44:53.000000 owega-5.8.4/owega/license.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    11827 2024-05-21 22:47:29.000000 owega-5.8.4/owega/owega.py
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     7504 2024-05-13 23:20:56.000000 owega-5.8.4/owega/utils.py
+drwxr-xr-x   0 darkgeem  (1000) darkgeem  (1000)        0 2024-05-21 22:51:09.924870 owega-5.8.4/owega.egg-info/
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)    17070 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/PKG-INFO
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     1689 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/SOURCES.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        1 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/dependency_links.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       43 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/entry_points.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)      173 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/requires.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)        6 2024-05-21 22:51:09.000000 owega-5.8.4/owega.egg-info/top_level.txt
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       90 2024-04-17 02:21:38.000000 owega-5.8.4/pyproject.toml
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)       38 2024-05-21 22:51:09.924870 owega-5.8.4/setup.cfg
+-rw-r--r--   0 darkgeem  (1000) darkgeem  (1000)     2524 2024-05-17 22:16:16.000000 owega-5.8.4/setup.py
```

### Comparing `owega-5.8.3/LICENSE` & `owega-5.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/PKG-INFO` & `owega-5.8.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.8.3
+Version: 5.8.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.8.3 CHANGELOG:
+OWEGA v5.8.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -384,9 +384,12 @@
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
 
 5.8.0: Added time-aware mode...
 5.8.1: Oops, I broke the build system again, my bad! :P
 5.8.2: Oops, I didn't completely fix it last time~ Awoo! >w<\
 5.8.3: Fixed some error handling.
+5.8.4: Fixed an issue with time-aware mode which would create
+       new lines with just the date when sending an empty
+       message, instead of just prompting with same history.
 
 ```
```

### Comparing `owega-5.8.3/README.md` & `owega-5.8.4/README.md`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_add_sysmem.py` & `owega-5.8.4/owega/OweHandlers/handle_add_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_commands.py` & `owega-5.8.4/owega/OweHandlers/handle_commands.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_context.py` & `owega-5.8.4/owega/OweHandlers/handle_context.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_del_sysmem.py` & `owega-5.8.4/owega/OweHandlers/handle_del_sysmem.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_dinput.py` & `owega-5.8.4/owega/OweHandlers/handle_dinput.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_edit.py` & `owega-5.8.4/owega/OweHandlers/handle_edit.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_estimation.py` & `owega-5.8.4/owega/OweHandlers/handle_estimation.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_finput.py` & `owega-5.8.4/owega/OweHandlers/handle_finput.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_frequency.py` & `owega-5.8.4/owega/OweHandlers/handle_frequency.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_genconf.py` & `owega-5.8.4/owega/OweHandlers/handle_genconf.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_history.py` & `owega-5.8.4/owega/OweHandlers/handle_history.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_image.py` & `owega-5.8.4/owega/OweHandlers/handle_image.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_load.py` & `owega-5.8.4/owega/OweHandlers/handle_load.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_model.py` & `owega-5.8.4/owega/OweHandlers/handle_model.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_presence.py` & `owega-5.8.4/owega/OweHandlers/handle_presence.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_quit.py` & `owega-5.8.4/owega/OweHandlers/handle_quit.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_save.py` & `owega-5.8.4/owega/OweHandlers/handle_save.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_system.py` & `owega-5.8.4/owega/OweHandlers/handle_system.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_temperature.py` & `owega-5.8.4/owega/OweHandlers/handle_temperature.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_time.py` & `owega-5.8.4/owega/OweHandlers/handle_time.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_tokens.py` & `owega-5.8.4/owega/OweHandlers/handle_tokens.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_top_p.py` & `owega-5.8.4/owega/OweHandlers/handle_top_p.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handle_tts.py` & `owega-5.8.4/owega/OweHandlers/handle_tts.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OweHandlers/handlers.py` & `owega-5.8.4/owega/OweHandlers/handlers.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaFun/__init__.py` & `owega-5.8.4/owega/OwegaFun/__init__.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaFun/functions.py` & `owega-5.8.4/owega/OwegaFun/functions.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaFun/longTermSouvenirs.py` & `owega-5.8.4/owega/OwegaFun/longTermSouvenirs.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaFun/utility.py` & `owega-5.8.4/owega/OwegaFun/utility.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaSession/main_bottom_toolbar.py` & `owega-5.8.4/owega/OwegaSession/main_bottom_toolbar.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/OwegaSession/promptsession.py` & `owega-5.8.4/owega/OwegaSession/promptsession.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/ask.py` & `owega-5.8.4/owega/ask.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/changelog/changelog.py` & `owega-5.8.4/owega/changelog/changelog.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,14 +13,20 @@
         self.version = Version(0, 0, 0)
         self.initLogs()
         self.genLog()
 
     def initLogs(self):
         """Fill the changelog."""
         self.logs.append(
+            ChangelogEntry(5, 8, 4)
+            .addLine("Fixed an issue with time-aware mode which would create")
+            .addLine("new lines with just the date when sending an empty")
+            .addLine("message, instead of just prompting with same history.")
+        )
+        self.logs.append(
             ChangelogEntry(5, 8, 3)
             .addLine("Fixed some error handling.")
         )
         self.logs.append(
             ChangelogEntry(5, 8, 2)
             .addLine("Oops, I didn't completely fix it last time~ Awoo! >w<\\")
         )
```

### Comparing `owega-5.8.3/owega/changelog/changelogEntry.py` & `owega-5.8.4/owega/changelog/changelogEntry.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/changelog/version.py` & `owega-5.8.4/owega/changelog/version.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/config/baseConf.py` & `owega-5.8.4/owega/config/baseConf.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/conversation/conversation.py` & `owega-5.8.4/owega/conversation/conversation.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/getLogger.py` & `owega-5.8.4/owega/getLogger.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/license.py` & `owega-5.8.4/owega/license.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega/owega.py` & `owega-5.8.4/owega/owega.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,17 +113,18 @@
                 messages = current_handler(
                     temp_file,
                     messages,
                     given,
                     temp_is_temp
                 )
         if not command_found:
-            if baseConf.get("time_awareness", False):
-                date_str = time.strftime("[%Y-%m-%d %H:%M:%S]")
-                user_input = f"{date_str}\n" + user_input
+            if user_input.strip():
+                if baseConf.get("time_awareness", False):
+                    date_str = time.strftime("[%Y-%m-%d %H:%M:%S]")
+                    user_input = f"{date_str}\n" + user_input
             if baseConf.get("estimation", False):
                 etkn, cost = estimated_tokens_and_cost(
                     user_input,
                     messages,
                     functionlist_to_toollist(existingFunctions.getEnabled()),
                     baseConf.get('model', ''),
                     baseConf.get("max_tokens", 4096)
```

### Comparing `owega-5.8.3/owega/utils.py` & `owega-5.8.4/owega/utils.py`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/owega.egg-info/PKG-INFO` & `owega-5.8.4/owega.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: owega
-Version: 5.8.3
+Version: 5.8.4
 Summary: A command-line interface for conversing with GPT models (from OpenAI)
 Home-page: https://git.pyrokinesis.fr/darkgeem/owega
 Author: darkgeem
 Author-email: darkgeem@pyrokinesis.fr
 License: DGPL-1.0
 Project-URL: Source, https://git.pyrokinesis.fr/darkgeem/owega
 Project-URL: Support, https://discord.gg/KdRmyRrA48
@@ -142,15 +142,15 @@
 See ΦωΦ in action!
 
 [![asciicast](https://asciinema.org/a/613143.png)](https://asciinema.org/a/613143)
 
 
 ## CHANGELOG: 
 ```
-OWEGA v5.8.3 CHANGELOG:
+OWEGA v5.8.4 CHANGELOG:
 
 
 2.0.0: WTFPL license
 2.0.1: added genconf command
 
 2.1.0: added file_input command
 2.1.1: added file_input in help command
@@ -384,9 +384,12 @@
        doesn't have enough columns.
        (also, added gpt-4o and mixtral-8x22b to default list)
 
 5.8.0: Added time-aware mode...
 5.8.1: Oops, I broke the build system again, my bad! :P
 5.8.2: Oops, I didn't completely fix it last time~ Awoo! >w<\
 5.8.3: Fixed some error handling.
+5.8.4: Fixed an issue with time-aware mode which would create
+       new lines with just the date when sending an empty
+       message, instead of just prompting with same history.
 
 ```
```

### Comparing `owega-5.8.3/owega.egg-info/SOURCES.txt` & `owega-5.8.4/owega.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `owega-5.8.3/setup.py` & `owega-5.8.4/setup.py`

 * *Files identical despite different names*

