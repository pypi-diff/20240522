# Comparing `tmp/dragonlog-1.1.3.tar.gz` & `tmp/dragonlog-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dragonlog-1.1.3.tar", last modified: Sat May  4 07:20:06 2024, max compression
+gzip compressed data, was "dragonlog-1.2.tar", last modified: Wed May 22 19:13:36 2024, max compression
```

## Comparing `dragonlog-1.1.3.tar` & `dragonlog-1.2.tar`

### file list

```diff
@@ -1,66 +1,69 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/DragonLog.egg-info/
--rw-rw-rw-   0        0        0     7401 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1603 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       79 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 07:20:05.000000 dragonlog-1.1.3/DragonLog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.1.3/LICENCE.txt
--rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.1.3/MANIFEST.in
--rw-rw-rw-   0        0        0     7401 2024-05-04 07:20:06.155683 dragonlog-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.071051 dragonlog-1.1.3/dragonlog/
--rw-rw-rw-   0        0        0    10600 2024-04-30 18:45:39.000000 dragonlog-1.1.3/dragonlog/CallBook.py
--rw-rw-rw-   0        0        0    63825 2024-05-02 14:23:02.000000 dragonlog-1.1.3/dragonlog/DragonLog.py
--rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.1.3/dragonlog/DragonLog_AppSelect.py
--rw-rw-rw-   0        0        0     3041 2024-05-04 07:18:54.000000 dragonlog-1.1.3/dragonlog/DragonLog_AppSelect_ui.py
--rw-rw-rw-   0        0        0    17410 2024-05-04 07:18:53.000000 dragonlog-1.1.3/dragonlog/DragonLog_MainWindow_ui.py
--rw-rw-rw-   0        0        0    47609 2024-05-03 15:13:12.000000 dragonlog-1.1.3/dragonlog/DragonLog_QSOForm.py
--rw-rw-rw-   0        0        0    38980 2024-05-04 07:18:53.000000 dragonlog-1.1.3/dragonlog/DragonLog_QSOForm_ui.py
--rw-rw-rw-   0        0        0    22179 2024-05-03 15:13:12.000000 dragonlog-1.1.3/dragonlog/DragonLog_Settings.py
--rw-rw-rw-   0        0        0    39219 2024-05-04 07:18:54.000000 dragonlog-1.1.3/dragonlog/DragonLog_Settings_ui.py
--rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/LoTW.py
--rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.1.3/dragonlog/Logger.py
--rw-rw-rw-   0        0        0     1134 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/RegEx.py
--rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.1.3/dragonlog/__init__.py
--rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.1.3/dragonlog/__main__.py
--rw-rw-rw-   0        0        0       65 2024-05-04 07:18:52.000000 dragonlog-1.1.3/dragonlog/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.086675 dragonlog-1.1.3/dragonlog/data/
--rw-rw-rw-   0        0        0     6399 2024-04-03 17:19:13.000000 dragonlog-1.1.3/dragonlog/data/README.md
--rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.1.3/dragonlog/data/bands.json
--rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.1.3/dragonlog/data/cb_channels.json
--rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.1.3/dragonlog/data/color_map.json
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.086675 dragonlog-1.1.3/dragonlog/data/i18n/
--rw-rw-rw-   0        0        0    24719 2024-05-04 07:18:57.000000 dragonlog-1.1.3/dragonlog/data/i18n/DragonLog_de.qm
--rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.1.3/dragonlog/data/i18n/ascii_replace_de.json
--rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.1.3/dragonlog/data/modes.json
--rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.1.3/dragonlog/eQSL.py
-drwxrwxrwx   0        0        0        0 2024-05-04 07:20:06.155683 dragonlog-1.1.3/dragonlog/icons/
--rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.1.3/dragonlog/icons/Screenshot.png
--rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.1.3/dragonlog/icons/db.png
--rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.1.3/dragonlog/icons/edit.png
--rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.1.3/dragonlog/icons/edit_add.png
--rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.1.3/dragonlog/icons/edit_addmulti.png
--rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.1.3/dragonlog/icons/edit_addmulti.xcf
--rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.1.3/dragonlog/icons/edit_remove.png
--rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.1.3/dragonlog/icons/exit.png
--rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.1.3/dragonlog/icons/file_doc.png
--rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.1.3/dragonlog/icons/fileexport.png
--rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.1.3/dragonlog/icons/fileimport.png
--rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.1.3/dragonlog/icons/gear.png
--rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.1.3/dragonlog/icons/help.png
--rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.png
--rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.xcf
--rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.1.3/dragonlog/icons/info.png
--rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.1.3/dragonlog/icons/logo.ico
--rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.1.3/dragonlog/icons/no.png
--rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.1.3/dragonlog/icons/ok.png
--rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.1.3/dragonlog/icons/player_play.png
--rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.1.3/dragonlog/icons/player_stop.png
--rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.1.3/dragonlog/icons/upload_lotw.png
--rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.1.3/dragonlog/icons/upload_lotw.xcf
--rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.1.3/dragonlog/icons/watch.png
--rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-04 07:20:06.155683 dragonlog-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.1.3/setup_msi.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.615077 dragonlog-1.2/
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.610587 dragonlog-1.2/DragonLog.egg-info/
+-rw-rw-rw-   0        0        0     7453 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1677 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       79 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 19:13:36.000000 dragonlog-1.2/DragonLog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      158 2024-03-19 12:18:34.000000 dragonlog-1.2/LICENCE.txt
+-rw-rw-rw-   0        0        0       93 2023-11-21 13:44:18.000000 dragonlog-1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     7453 2024-05-22 19:13:36.613081 dragonlog-1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     6453 2024-05-04 08:39:54.000000 dragonlog-1.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.522760 dragonlog-1.2/dragonlog/
+-rw-rw-rw-   0        0        0    10600 2024-04-30 18:45:39.000000 dragonlog-1.2/dragonlog/CallBook.py
+-rw-rw-rw-   0        0        0    67866 2024-05-22 18:55:58.000000 dragonlog-1.2/dragonlog/DragonLog.py
+-rw-rw-rw-   0        0        0     2062 2024-02-20 17:06:17.000000 dragonlog-1.2/dragonlog/DragonLog_AppSelect.py
+-rw-rw-rw-   0        0        0     3041 2024-05-22 19:12:34.000000 dragonlog-1.2/dragonlog/DragonLog_AppSelect_ui.py
+-rw-rw-rw-   0        0        0    26239 2024-05-22 19:12:32.000000 dragonlog-1.2/dragonlog/DragonLog_MainWindow_ui.py
+-rw-rw-rw-   0        0        0    48993 2024-05-22 11:32:26.000000 dragonlog-1.2/dragonlog/DragonLog_QSOForm.py
+-rw-rw-rw-   0        0        0    42694 2024-05-22 19:12:33.000000 dragonlog-1.2/dragonlog/DragonLog_QSOForm_ui.py
+-rw-rw-rw-   0        0        0    23629 2024-05-22 18:55:58.000000 dragonlog-1.2/dragonlog/DragonLog_Settings.py
+-rw-rw-rw-   0        0        0    40061 2024-05-22 19:12:33.000000 dragonlog-1.2/dragonlog/DragonLog_Settings_ui.py
+-rw-rw-rw-   0        0        0     1833 2024-05-22 18:55:58.000000 dragonlog-1.2/dragonlog/ListEdit.py
+-rw-rw-rw-   0        0        0     2891 2024-05-22 19:12:34.000000 dragonlog-1.2/dragonlog/ListEdit_ui.py
+-rw-rw-rw-   0        0        0     7403 2024-04-15 17:33:29.000000 dragonlog-1.2/dragonlog/LoTW.py
+-rw-rw-rw-   0        0        0     2585 2024-04-12 05:48:01.000000 dragonlog-1.2/dragonlog/Logger.py
+-rw-rw-rw-   0        0        0     1232 2024-05-21 13:42:58.000000 dragonlog-1.2/dragonlog/RegEx.py
+-rw-rw-rw-   0        0        0        0 2023-11-21 18:25:24.000000 dragonlog-1.2/dragonlog/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-11-21 18:20:52.000000 dragonlog-1.2/dragonlog/__main__.py
+-rw-rw-rw-   0        0        0       63 2024-05-22 19:12:32.000000 dragonlog-1.2/dragonlog/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.536233 dragonlog-1.2/dragonlog/data/
+-rw-rw-rw-   0        0        0     6453 2024-05-04 08:39:54.000000 dragonlog-1.2/dragonlog/data/README.md
+-rw-rw-rw-   0        0        0     1816 2023-10-08 14:01:05.000000 dragonlog-1.2/dragonlog/data/bands.json
+-rw-rw-rw-   0        0        0     6834 2023-10-09 17:58:49.000000 dragonlog-1.2/dragonlog/data/cb_channels.json
+-rw-rw-rw-   0        0        0     1115 2023-11-15 18:59:09.000000 dragonlog-1.2/dragonlog/data/color_map.json
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.541723 dragonlog-1.2/dragonlog/data/i18n/
+-rw-rw-rw-   0        0        0    26024 2024-05-22 19:12:37.000000 dragonlog-1.2/dragonlog/data/i18n/DragonLog_de.qm
+-rw-rw-rw-   0        0        0      108 2024-03-28 07:19:36.000000 dragonlog-1.2/dragonlog/data/i18n/ascii_replace_de.json
+-rw-rw-rw-   0        0        0     4275 2023-10-11 18:47:43.000000 dragonlog-1.2/dragonlog/data/modes.json
+-rw-rw-rw-   0        0        0     5348 2024-04-15 17:33:29.000000 dragonlog-1.2/dragonlog/eQSL.py
+drwxrwxrwx   0        0        0        0 2024-05-22 19:13:36.607093 dragonlog-1.2/dragonlog/icons/
+-rw-rw-rw-   0        0        0    84255 2024-04-03 05:47:08.000000 dragonlog-1.2/dragonlog/icons/Screenshot.png
+-rw-rw-rw-   0        0        0     2775 2006-10-09 18:29:54.000000 dragonlog-1.2/dragonlog/icons/db.png
+-rw-rw-rw-   0        0        0      935 2006-10-09 18:46:20.000000 dragonlog-1.2/dragonlog/icons/edit.png
+-rw-rw-rw-   0        0        0     1501 2006-10-09 18:51:24.000000 dragonlog-1.2/dragonlog/icons/edit_add.png
+-rw-rw-rw-   0        0        0     4853 2023-10-06 05:04:50.000000 dragonlog-1.2/dragonlog/icons/edit_addmulti.png
+-rw-rw-rw-   0        0        0     4222 2023-10-06 05:13:53.000000 dragonlog-1.2/dragonlog/icons/edit_addmulti.xcf
+-rw-rw-rw-   0        0        0      901 2006-07-05 03:36:10.000000 dragonlog-1.2/dragonlog/icons/edit_remove.png
+-rw-rw-rw-   0        0        0     2360 2007-05-26 19:17:06.000000 dragonlog-1.2/dragonlog/icons/exit.png
+-rw-rw-rw-   0        0        0      697 2024-03-23 19:55:25.000000 dragonlog-1.2/dragonlog/icons/file_doc.png
+-rw-rw-rw-   0        0        0     2321 2006-10-09 18:55:14.000000 dragonlog-1.2/dragonlog/icons/fileexport.png
+-rw-rw-rw-   0        0        0     2076 2006-10-09 19:11:50.000000 dragonlog-1.2/dragonlog/icons/fileimport.png
+-rw-rw-rw-   0        0        0     1900 2006-07-05 03:36:10.000000 dragonlog-1.2/dragonlog/icons/filter.png
+-rw-rw-rw-   0        0        0     2166 2006-10-09 16:32:12.000000 dragonlog-1.2/dragonlog/icons/gear.png
+-rw-rw-rw-   0        0        0     2461 2006-10-09 18:22:00.000000 dragonlog-1.2/dragonlog/icons/help.png
+-rw-rw-rw-   0        0        0     4652 2023-10-04 17:16:16.000000 dragonlog-1.2/dragonlog/icons/icons8-dragon-96.png
+-rw-rw-rw-   0        0        0    19186 2023-10-06 12:24:58.000000 dragonlog-1.2/dragonlog/icons/icons8-dragon-96.xcf
+-rw-rw-rw-   0        0        0     2184 2006-10-09 19:49:00.000000 dragonlog-1.2/dragonlog/icons/info.png
+-rw-rw-rw-   0        0        0    54470 2023-10-06 12:25:24.000000 dragonlog-1.2/dragonlog/icons/logo.ico
+-rw-rw-rw-   0        0        0     2443 2006-10-09 19:00:44.000000 dragonlog-1.2/dragonlog/icons/no.png
+-rw-rw-rw-   0        0        0     1518 2006-10-09 20:22:10.000000 dragonlog-1.2/dragonlog/icons/ok.png
+-rw-rw-rw-   0        0        0     2225 2006-10-09 18:20:08.000000 dragonlog-1.2/dragonlog/icons/player_play.png
+-rw-rw-rw-   0        0        0     2112 2024-03-05 19:18:39.000000 dragonlog-1.2/dragonlog/icons/player_stop.png
+-rw-rw-rw-   0        0        0    21406 2024-03-25 10:49:08.000000 dragonlog-1.2/dragonlog/icons/upload_lotw.png
+-rw-rw-rw-   0        0        0     7906 2024-03-25 10:48:26.000000 dragonlog-1.2/dragonlog/icons/upload_lotw.xcf
+-rw-rw-rw-   0        0        0     1819 2006-10-17 07:09:30.000000 dragonlog-1.2/dragonlog/icons/watch.png
+-rw-rw-rw-   0        0        0     1159 2024-03-23 19:55:25.000000 dragonlog-1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 19:13:36.615576 dragonlog-1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1498 2024-03-19 12:15:10.000000 dragonlog-1.2/setup_msi.py
```

### Comparing `dragonlog-1.1.3/DragonLog.egg-info/PKG-INFO` & `dragonlog-1.2/DragonLog.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.3
+Version: 1.2
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,16 @@
 * log 11m band QSOs
 * filter recent QSOs (last week, month, half year, year)
 * UTF-8 (i.e. use german umlauts)
 * convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
-The installation requires a python installation (>= 3.9).
+The installation requires a python installation (>= 3.10). 
+On Linux you may have to install libxcb-cursor0.
     
     # python3 -m pip install DragonLog
 
 If you want to be able to export/import to/from Excel files install the extra packages
 
     # python3 -m pip install DragonLog[extra]
 
@@ -79,14 +80,15 @@
 Or if your python scripts folder is on PATH you can start DragonLog with 
 
     # DragonLog
 
 
 For windows there is also an installable MSI and ZIP package available for convenience.
 
+
 First start
 -----------
 Before you can start to log QSOs a database has to be selected.
 It can be placed on a path where you wish to.
 The database is created and initialised.
 
 At the next start of the program the last database gets opened automatically.
```

### Comparing `dragonlog-1.1.3/DragonLog.egg-info/SOURCES.txt` & `dragonlog-1.2/DragonLog.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -14,14 +14,16 @@
 dragonlog/DragonLog_AppSelect.py
 dragonlog/DragonLog_AppSelect_ui.py
 dragonlog/DragonLog_MainWindow_ui.py
 dragonlog/DragonLog_QSOForm.py
 dragonlog/DragonLog_QSOForm_ui.py
 dragonlog/DragonLog_Settings.py
 dragonlog/DragonLog_Settings_ui.py
+dragonlog/ListEdit.py
+dragonlog/ListEdit_ui.py
 dragonlog/LoTW.py
 dragonlog/Logger.py
 dragonlog/RegEx.py
 dragonlog/__init__.py
 dragonlog/__main__.py
 dragonlog/__version__.py
 dragonlog/eQSL.py
@@ -39,14 +41,15 @@
 dragonlog/icons/edit_addmulti.png
 dragonlog/icons/edit_addmulti.xcf
 dragonlog/icons/edit_remove.png
 dragonlog/icons/exit.png
 dragonlog/icons/file_doc.png
 dragonlog/icons/fileexport.png
 dragonlog/icons/fileimport.png
+dragonlog/icons/filter.png
 dragonlog/icons/gear.png
 dragonlog/icons/help.png
 dragonlog/icons/icons8-dragon-96.png
 dragonlog/icons/icons8-dragon-96.xcf
 dragonlog/icons/info.png
 dragonlog/icons/logo.ico
 dragonlog/icons/no.png
```

### Comparing `dragonlog-1.1.3/PKG-INFO` & `dragonlog-1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DragonLog
-Version: 1.1.3
+Version: 1.2
 Summary: Log QSO for Ham radio
 Author-email: "Andreas Schawo, DF1ASC" <andreas@schawo.de>
 Project-URL: Homepage, https://github.com/gitandy/DragonLog
 Project-URL: Bug Tracker, https://github.com/gitandy/DragonLog/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Other Audience
 Classifier: Operating System :: OS Independent
@@ -60,15 +60,16 @@
 * log 11m band QSOs
 * filter recent QSOs (last week, month, half year, year)
 * UTF-8 (i.e. use german umlauts)
 * convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
-The installation requires a python installation (>= 3.9).
+The installation requires a python installation (>= 3.10). 
+On Linux you may have to install libxcb-cursor0.
     
     # python3 -m pip install DragonLog
 
 If you want to be able to export/import to/from Excel files install the extra packages
 
     # python3 -m pip install DragonLog[extra]
 
@@ -79,14 +80,15 @@
 Or if your python scripts folder is on PATH you can start DragonLog with 
 
     # DragonLog
 
 
 For windows there is also an installable MSI and ZIP package available for convenience.
 
+
 First start
 -----------
 Before you can start to log QSOs a database has to be selected.
 It can be placed on a path where you wish to.
 The database is created and initialised.
 
 At the next start of the program the last database gets opened automatically.
```

### Comparing `dragonlog-1.1.3/README.md` & `dragonlog-1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 * log 11m band QSOs
 * filter recent QSOs (last week, month, half year, year)
 * UTF-8 (i.e. use german umlauts)
 * convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
-The installation requires a python installation (>= 3.9).
+The installation requires a python installation (>= 3.10). 
+On Linux you may have to install libxcb-cursor0.
     
     # python3 -m pip install DragonLog
 
 If you want to be able to export/import to/from Excel files install the extra packages
 
     # python3 -m pip install DragonLog[extra]
 
@@ -52,14 +53,15 @@
 Or if your python scripts folder is on PATH you can start DragonLog with 
 
     # DragonLog
 
 
 For windows there is also an installable MSI and ZIP package available for convenience.
 
+
 First start
 -----------
 Before you can start to log QSOs a database has to be selected.
 It can be placed on a path where you wish to.
 The database is created and initialised.
 
 At the next start of the program the last database gets opened automatically.
```

### Comparing `dragonlog-1.1.3/dragonlog/CallBook.py` & `dragonlog-1.2/dragonlog/CallBook.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog.py` & `dragonlog-1.2/dragonlog/DragonLog.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     OPTION_OPENPYXL = True
 except ImportError:
     pass
 
 from . import DragonLog_MainWindow_ui
 from .Logger import Logger
-from .RegEx import find_non_ascii
+from .RegEx import find_non_ascii, check_format, REGEX_DATE
 from .DragonLog_QSOForm import QSOForm
 from .DragonLog_Settings import Settings
 from .DragonLog_AppSelect import AppSelect
 from .LoTW import LoTW, LoTWADIFFieldException, LoTWRequestException, LoTWCommunicationException
 
 __prog_name__ = 'DragonLog'
 __prog_desc__ = 'Log QSO for Ham radio'
@@ -94,15 +94,15 @@
 
         self.prop_col = prop_col
         self.prop_translation = prop_tr
 
         self.ok_icon = QtGui.QIcon(self.parent().searchFile('icons:ok.png'))
         self.no_icon = QtGui.QIcon(self.parent().searchFile('icons:no.png'))
 
-    def data(self, idx, role = QtCore.Qt.ItemDataRole.DisplayRole):
+    def data(self, idx, role=QtCore.Qt.ItemDataRole.DisplayRole):
         value = super().data(idx, role)
         if role == QtCore.Qt.ItemDataRole.DisplayRole:
             if idx.column() in self.status_cols and value in self.status_translation:
                 return self.status_translation[value]
             elif idx.column() == self.prop_col and value in self.prop_translation:
                 return self.prop_translation[value]
 
@@ -114,28 +114,33 @@
                 else:
                     return self.no_icon
 
         return value
 
 
 class DragonLog(QtWidgets.QMainWindow, DragonLog_MainWindow_ui.Ui_MainWindow):
-    __sql_cols__ = ('id', 'date_time', 'date_time_off', 'own_callsign', 'call_sign', 'name', 'qth', 'locator',
-                    'rst_sent', 'rst_rcvd', 'band', 'mode', 'submode', 'freq', 'channel', 'power', 'propagation',
-                    'own_name', 'own_qth', 'own_locator', 'radio', 'antenna',
-                    'remarks', 'comments', 'dist',
-                    'qsl_via', 'qsl_path', 'qsl_msg', 'qsl_sent', 'qsl_rcvd',
-                    'eqsl_sent', 'eqsl_rcvd', 'lotw_sent', 'lotw_rcvd', 'hamqth')
+    __sql_cols__ = (
+        'id', 'date_time', 'date_time_off', 'own_callsign', 'call_sign', 'name', 'qth', 'locator',
+        'rst_sent', 'rst_rcvd', 'band', 'mode', 'submode', 'freq', 'channel', 'power', 'propagation',
+        'own_name', 'own_qth', 'own_locator', 'radio', 'antenna',
+        'remarks', 'comments', 'dist',
+        'qsl_via', 'qsl_path', 'qsl_msg', 'qsl_sent', 'qsl_rcvd',
+        'eqsl_sent', 'eqsl_rcvd', 'lotw_sent', 'lotw_rcvd', 'hamqth',
+        'contest_id', 'ctx_qso_id', 'crx_qso_id', 'crx_data',
+    )
 
     __adx_cols__ = (
         'QSO_DATE/TIME_ON', 'QSO_DATE/TIME_OFF', 'STATION_CALLSIGN', 'CALL', 'NAME_INTL', 'QTH_INTL', 'GRIDSQUARE',
         'RST_SENT', 'RST_RCVD', 'BAND', 'MODE', 'SUBMODE', 'FREQ', 'APP_DRAGONLOG_CBCHANNEL', 'TX_PWR', 'PROP_MODE',
         'MY_NAME_INTL', 'MY_CITY_INTL', 'MY_GRIDSQUARE', 'MY_RIG_INTL', 'MY_ANTENNA_INTL',
         'NOTES_INTL', 'COMMENT_INTL', 'DISTANCE',
         'QSL_VIA', 'QSL_SENT_VIA', 'QSLMSG_INTL', 'QSL_SENT', 'QSL_RCVD',
-        'EQSL_QSL_SENT', 'EQSL_QSL_RCVD', 'LOTW_QSL_SENT', 'LOTW_QSL_RCVD', 'HAMQTH_QSO_UPLOAD_STATUS')
+        'EQSL_QSL_SENT', 'EQSL_QSL_RCVD', 'LOTW_QSL_SENT', 'LOTW_QSL_RCVD', 'HAMQTH_QSO_UPLOAD_STATUS',
+        'CONTEST_ID', 'STX', 'SRX', 'SRX_STRING',
+    )
 
     __db_create_stmnt__ = '''CREATE TABLE IF NOT EXISTS "qsos" (
                             "id"    INTEGER PRIMARY KEY NOT NULL,
                             "date_time"   NUMERIC,
                             "date_time_off"   NUMERIC,
                             "own_callsign" TEXT,
                             "call_sign"  TEXT,
@@ -164,15 +169,19 @@
                             "qsl_msg"   TEXT,
                             "qsl_sent"   TEXT,
                             "qsl_rcvd"   TEXT,
                             "eqsl_sent"   TEXT,
                             "eqsl_rcvd"   TEXT,
                             "lotw_sent"   TEXT,
                             "lotw_rcvd"   TEXT,
-                            "hamqth"   TEXT
+                            "hamqth"   TEXT,
+                            "contest_id" TEXT,
+                            "ctx_qso_id" INTEGER,
+                            "crx_qso_id" INTEGER,
+                            "crx_data" TEXT
                         );'''
 
     __db_create_idx_stmnt__ = '''CREATE INDEX IF NOT EXISTS "find_qso" ON "qsos" (
                                     "date_time",
                                     "call_sign"
                                 )'''
 
@@ -203,18 +212,30 @@
         self.log.info(f'Starting {__prog_name__} {__version__}...')
 
         if int(self.settings.value('ui/log_dock_float', 0)):
             self.logDockWidget.setFloating(True)
         else:
             log_dock_area = self.int2dock_area(int(self.settings.value('ui/log_dock_area',
                                                                        QtCore.Qt.DockWidgetArea.BottomDockWidgetArea.value)))
-            self.addDockWidget(log_dock_area,
-                               self.logDockWidget)
+            self.addDockWidget(log_dock_area, self.logDockWidget)
         self.logDockWidget.setVisible(bool(int(self.settings.value('ui/show_log', 0))))
 
+        if int(self.settings.value('ui/filter_dock_float', 0)):
+            self.filterDockWidget.setFloating(True)
+            self.filterDockWidget.resize(10, 10)
+        else:
+            filter_dock_area = self.int2dock_area(int(self.settings.value('ui/filter_dock_area',
+                                                                          QtCore.Qt.DockWidgetArea.TopDockWidgetArea.value)))
+            self.addDockWidget(filter_dock_area, self.filterDockWidget)
+        self.filterDockWidget.setVisible(bool(int(self.settings.value('ui/show_filter', 0))))
+
+        self.__table_filter__ = ''
+        self.filterDockWidget.visibilityChanged.connect(self.resetTableFilter)
+        self.filterDockWidget.dockLocationChanged.connect(self.filterWidgetResize)
+
         self.dummy_status = QtWidgets.QLabel()
         self.statusBar().addPermanentWidget(self.dummy_status)
         self.watch_status = QtWidgets.QLabel(self.tr('Watching file') + ': ' + self.tr('inactiv'))
         self.statusBar().addPermanentWidget(self.watch_status)
         self.hamlib_status = QtWidgets.QLabel(self.tr('Hamlib') + ': ' + self.tr('inactiv'))
         self.statusBar().addPermanentWidget(self.hamlib_status)
         self.hamlib_error = QtWidgets.QLabel('')
@@ -226,14 +247,19 @@
             self.modes: dict = json.load(mj)
         with open(self.searchFile('data:cb_channels.json')) as cj:
             self.cb_channels: dict = json.load(cj)
         with open(self.searchFile('data:color_map.json')) as cmj:
             color_map: dict = json.load(cmj)
         self.QSOTableView.setItemDelegate(BackgroundBrushDelegate(color_map, self.__sql_cols__.index('band')))
 
+        self.fBandComboBox.insertItem(0, '')
+        self.fModeComboBox.insertItem(0, '')
+        self.fBandComboBox.insertItems(1, self.bands.keys())
+        self.fModeComboBox.insertItems(1, self.modes['AFU'].keys())
+
         self.prop: dict = {
             '': '',
             'AS': self.tr('Aircraft Scatter'),
             'AUE': self.tr('Aurora-E'),
             'AUR': self.tr('Aurora'),
             'BS': self.tr('Back scatter'),
             'ECH': self.tr('EchoLink'),
@@ -295,14 +321,18 @@
             self.tr('QSL sent'),
             self.tr('QSL rcvd'),
             self.tr('eQSL sent'),
             self.tr('eQSL rcvd'),
             self.tr('LoTW sent'),
             self.tr('LoTW rcvd'),
             self.tr('HamQTH'),
+            self.tr('Contest'),
+            self.tr('Tx QSO ID'),
+            self.tr('Rx QSO ID'),
+            self.tr('Rx data'),
         )
 
         self.__header_map__ = dict(zip(self.__sql_cols__, self.__headers__))
 
         self.settings_form = Settings(self, self.settings, self.hamlib_status, self.__headers__, self.log)
 
         # QSOForm
@@ -341,14 +371,17 @@
         self.watchTimer = QtCore.QTimer(self)
         self.watchTimer.timeout.connect(self.watchFile)
         self.watchPos = 0
         self.watchFileName = ''
 
         self.lotw = LoTW(self.log)
 
+        self.settings_form.settingsStored.connect(self.qso_form.refreshRadioList)
+        self.settings_form.settingsStored.connect(self.qso_form.refreshAntennaList)
+
     @staticmethod
     def int2dock_area(value: int) -> QtCore.Qt.DockWidgetArea:
         dock_area = QtCore.Qt.DockWidgetArea.NoDockWidgetArea
         match value:
             case 1:
                 dock_area = QtCore.Qt.DockWidgetArea.LeftDockWidgetArea
             case 2:
@@ -356,14 +389,18 @@
             case 4:
                 dock_area = QtCore.Qt.DockWidgetArea.TopDockWidgetArea
             case 8:
                 dock_area = QtCore.Qt.DockWidgetArea.BottomDockWidgetArea
 
         return dock_area
 
+    def filterWidgetResize(self):
+        if self.filterDockWidget.isFloating():
+            self.filterDockWidget.resize(10, 10)
+
     def showSettings(self):
         if self.settings_form.exec():
             self.refreshTableView()
 
     def selectDB(self):
         res = QtWidgets.QFileDialog.getSaveFileName(
             self,
@@ -480,15 +517,15 @@
                 raise DatabaseOpenException(self.__db_con__.lastError().text())
 
             if not self.checkDB(db_file):
                 return
 
             model = TranslatedTableModel(self, self.__db_con__,
                                          status_cols=tuple(range(self.__sql_cols__.index('qsl_sent'),
-                                                                 self.__sql_cols__.index('hamqth')+1)),
+                                                                 self.__sql_cols__.index('hamqth') + 1)),
                                          prop_col=self.__sql_cols__.index('propagation'),
                                          prop_tr=self.prop)
             model.setTable('qsos')
             self.QSOTableView.setModel(model)
 
             for c in self.__sql_cols__:
                 model.setHeaderData(self.__sql_cols__.index(c),
@@ -535,37 +572,70 @@
         view_filter = self.getFilter()
         if view_filter:
             return f"SELECT * FROM qsos WHERE {view_filter}"
         else:
             return "SELECT * FROM qsos"
 
     def getFilter(self):
-        recent_filter = self.settings.value('ui/recent_qsos', self.tr('Show all'))
-        if recent_filter == self.tr('Last week'):
-            return "DATE(date_time) > DATE('now', '-7 days')"
-        elif recent_filter == self.tr('Last month'):
-            return "DATE(date_time) > DATE('now', '-31 days')"
-        elif recent_filter == self.tr('Last half year'):
-            return "DATE(date_time) > DATE('now', '-183 days')"
-        elif recent_filter == self.tr('Last year'):
-            return "DATE(date_time) > DATE('now', '-365 days')"
+        if self.__table_filter__:
+            return self.__table_filter__
         else:
-            return ""
+            recent_filter = self.settings.value('ui/recent_qsos', self.tr('Show all'))
+            if recent_filter == self.tr('Last week'):
+                return "DATE(date_time) > DATE('now', '-7 days')"
+            elif recent_filter == self.tr('Last month'):
+                return "DATE(date_time) > DATE('now', '-31 days')"
+            elif recent_filter == self.tr('Last half year'):
+                return "DATE(date_time) > DATE('now', '-183 days')"
+            elif recent_filter == self.tr('Last year'):
+                return "DATE(date_time) > DATE('now', '-365 days')"
+            else:
+                return ""
 
     def setFilter(self):
         self.QSOTableView.model().setFilter(self.getFilter())
 
+    def setTableFilter(self):
+        filter_set = []
+
+        if self.fDateFromLineEdit.text() and check_format(REGEX_DATE, self.fDateFromLineEdit.text()):
+            filter_set.append(f"DATE(date_time) >= DATE('{self.fDateFromLineEdit.text()}')")
+        if self.fDateToLineEdit.text() and check_format(REGEX_DATE, self.fDateToLineEdit.text()):
+            filter_set.append(f"DATE(date_time) <= DATE('{self.fDateToLineEdit.text()}')")
+
+        if self.fCallsignLineEdit.text():
+            filter_set.append(f'call_sign LIKE "%{self.fCallsignLineEdit.text()}%"')
+        if self.fBandComboBox.currentText():
+            filter_set.append(f'band = "{self.fBandComboBox.currentText()}"')
+        if self.fModeComboBox.currentText():
+            filter_set.append(f'mode = "{self.fModeComboBox.currentText()}"')
+
+        self.__table_filter__ = ' AND '.join(filter_set)
+
+        self.setFilter()
+
+    def resetTableFilter(self):
+        self.__table_filter__ = ''
+        self.setFilter()
+
+        self.fDateFromLineEdit.clear()
+        self.fDateToLineEdit.clear()
+        self.fCallsignLineEdit.clear()
+        self.fBandComboBox.setCurrentIndex(0)
+        self.fModeComboBox.setCurrentIndex(0)
+
     def ctrlHamlib(self, start):
         self.settings_form.ctrlRigctld(start)
 
     def logQSO(self):
         self.qso_form.clear()
         self.qso_form.setChangeMode(False)
         self.qso_form.reset()
         self.qsoDockWidget.setVisible(True)
+        self.qso_form.callSignLineEdit.setFocus()
 
     def fetchQSO(self):
         self.log.info('Logging QSO...')
         query = QtSql.QSqlQuery(self.__db_con__)
         query.prepare(self.__db_insert_stmnt__)
         for i, val in enumerate(self.qso_form.values):
             query.bindValue(i, val)
@@ -915,14 +985,22 @@
                 record['EQSL_QSL_RCVD'] = query.value(self.__sql_cols__.index('eqsl_rcvd'))
             if query.value(self.__sql_cols__.index('lotw_sent')):
                 record['LOTW_QSL_SENT'] = query.value(self.__sql_cols__.index('lotw_sent'))
             if query.value(self.__sql_cols__.index('lotw_rcvd')):
                 record['LOTW_QSL_RCVD'] = query.value(self.__sql_cols__.index('lotw_rcvd'))
             if query.value(self.__sql_cols__.index('hamqth')):
                 record['HAMQTH_QSO_UPLOAD_STATUS'] = query.value(self.__sql_cols__.index('hamqth'))
+            if query.value(self.__sql_cols__.index('contest_id')):
+                record['CONTEST_ID'] = query.value(self.__sql_cols__.index('contest_id'))
+            if query.value(self.__sql_cols__.index('ctx_qso_id')):
+                record['STX'] = query.value(self.__sql_cols__.index('ctx_qso_id'))
+            if query.value(self.__sql_cols__.index('crx_qso_id')):
+                record['SRX'] = query.value(self.__sql_cols__.index('crx_qso_id'))
+            if query.value(self.__sql_cols__.index('crx_data')):
+                record['SRX_STRING'] = query.value(self.__sql_cols__.index('crx_data'))
 
             if not record['APP']:
                 record.pop('APP')
 
             records.append(record)
         doc['RECORDS'] = records
         return doc
@@ -1388,14 +1466,18 @@
         self.log.info(f'Quiting {__prog_name__}...')
         self.__db_con__.close()
 
         self.settings.setValue('ui/show_log', int(self.logDockWidget.isVisible()))
         self.settings.setValue('ui/log_dock_area', self.dockWidgetArea(self.logDockWidget).value)
         self.settings.setValue('ui/log_dock_float', int(self.logDockWidget.isFloating()))
 
+        self.settings.setValue('ui/show_filter', int(self.filterDockWidget.isVisible()))
+        self.settings.setValue('ui/filter_dock_area', self.dockWidgetArea(self.filterDockWidget).value)
+        self.settings.setValue('ui/filter_dock_float', int(self.filterDockWidget.isFloating()))
+
         self.settings.setValue('ui/show_qso', int(self.qsoDockWidget.isVisible()))
         self.settings.setValue('ui/qso_dock_area', self.dockWidgetArea(self.qsoDockWidget).value)
         self.settings.setValue('ui/qso_dock_float', int(self.qsoDockWidget.isFloating()))
 
         self.settings_form.ctrlRigctld(False)
         e.accept()
```

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_AppSelect.py` & `dragonlog-1.2/dragonlog/DragonLog_AppSelect.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_AppSelect_ui.py` & `dragonlog-1.2/dragonlog/DragonLog_AppSelect_ui.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_QSOForm.py` & `dragonlog-1.2/dragonlog/DragonLog_QSOForm.py`

 * *Files 3% similar despite different names*

```diff
@@ -124,16 +124,27 @@
             self.lotwRcvdCheckBox,
         )
 
         for w in view_only_widgets:
             w.setAttribute(QtCore.Qt.WidgetAttribute.WA_TransparentForMouseEvents)
             w.setFocusPolicy(QtCore.Qt.FocusPolicy.NoFocus)
 
+        self.refreshRadioList()
+        self.refreshAntennaList()
+
         self.clear()
 
+    def refreshRadioList(self):
+        self.radioComboBox.clear()
+        self.radioComboBox.insertItems(0, self.settings.value('listings/rigs'))
+
+    def refreshAntennaList(self):
+        self.antennaComboBox.clear()
+        self.antennaComboBox.insertItems(0, self.settings.value('listings/antennas'))
+
     def rigctldChanged(self, state):
         self.__last_mode__ = ''
         self.__last_band__ = ''
         self.__last_freq__ = 0.0
         self.__last_pwr__ = ''
 
     def startTimers(self, start: bool):
@@ -324,23 +335,30 @@
         self.lotwGroupBox.setChecked(False)
         self.lotwSentCheckBox.setChecked(False)
         self.lotwRcvdCheckBox.setChecked(False)
         self.lotwInboxPushButton.setEnabled(False)
 
         self.hamQTHCheckBox.setChecked(False)
 
+        self.contestComboBox.setCurrentText('')
+        self.sentQSOSpinBox.setValue(0)
+        self.rcvdQSOSpinBox.setValue(0)
+        self.rcvdDataLineEdit.clear()
+
         self.toolBox.setCurrentIndex(0)
-        self.callSignLineEdit.setFocus()
 
     def reset(self):
         self.autoDateCheckBox.setEnabled(True)
         self.autoDateCheckBox.setChecked(True)
         self.stationGroupBox.setChecked(True)
         self.identityGroupBox.setChecked(True)
 
+        self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
+        self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
+
     def setChangeMode(self, activate=True):
         self.__change_mode__ = activate
         self.startTimers(not activate)
 
         if activate:
             self.stationGroupBox.setChecked(False)
             self.stationGroupBox.setCheckable(False)
@@ -380,16 +398,16 @@
             self.searchQRZCQPushButton.setEnabled(False)
             self.uploadPushButton.setEnabled(False)
             self.qslPage.setEnabled(False)
             self.channelComboBox.setCurrentIndex(-1)
             self.channelComboBox.setCurrentIndex(0)
 
             if self.stationGroupBox.isChecked():
-                self.radioLineEdit.setText(self.settings.value('station_cb/radio', ''))
-                self.antennaLineEdit.setText(self.settings.value('station_cb/antenna', ''))
+                self.radioComboBox.setCurrentText(self.settings.value('station_cb/radio', ''))
+                self.antennaComboBox.setCurrentText(self.settings.value('station_cb/antenna', ''))
 
             if self.identityGroupBox.isChecked():
                 self.ownCallSignLineEdit.setText(self.settings.value('station_cb/callSign', ''))
         else:
             self.modeComboBox.insertItems(0, self.modes['AFU'].keys())
             self.modeComboBox.setCurrentIndex(0)
             self.powerSpinBox.setMaximum(1000)
@@ -398,16 +416,16 @@
             self.freqDoubleSpinBox.setEnabled(True)
             self.searchHamQTHPushButton.setEnabled(True)
             self.searchQRZCQPushButton.setEnabled(True)
             self.uploadPushButton.setEnabled(True)
             self.qslPage.setEnabled(True)
 
             if self.stationGroupBox.isChecked():
-                self.radioLineEdit.setText(self.settings.value('station/radio', ''))
-                self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
+                self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
+                self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
 
             if self.identityGroupBox.isChecked():
                 self.ownCallSignLineEdit.setText(self.settings.value('station/callSign', ''))
 
     def modeChanged(self, mode: str):
         self.__last_mode__ = mode
         self.submodeComboBox.clear()
@@ -425,19 +443,19 @@
 
     def stationChanged(self, checked):
         if checked:
             self.ownQTHLineEdit.setText(self.settings.value('station/QTH', ''))
             self.ownLocatorLineEdit.setText(self.settings.value('station/locator', ''))
 
             if self.bandComboBox.currentText() == '11m':
-                self.radioLineEdit.setText(self.settings.value('station_cb/radio', ''))
-                self.antennaLineEdit.setText(self.settings.value('station_cb/antenna', ''))
+                self.radioComboBox.setCurrentText(self.settings.value('station_cb/radio', ''))
+                self.antennaComboBox.setCurrentText(self.settings.value('station_cb/antenna', ''))
             else:
-                self.radioLineEdit.setText(self.settings.value('station/radio', ''))
-                self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
+                self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
+                self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
 
     def identityChanged(self, checked):
         if checked:
             self.ownNameLineEdit.setText(self.settings.value('station/name', ''))
 
             if self.bandComboBox.currentText() == '11m':
                 self.ownCallSignLineEdit.setText(self.settings.value('station_cb/callSign', ''))
@@ -609,29 +627,33 @@
                 0] else '',
             self.channelComboBox.currentText() if band == '11m' else '-',
             self.powerSpinBox.value() if self.powerSpinBox.value() > 0 else '',
             prop,
             self.ownNameLineEdit.text(),
             self.ownQTHLineEdit.text(),
             self.ownLocatorLineEdit.text(),
-            self.radioLineEdit.text(),
-            self.antennaLineEdit.text(),
+            self.radioComboBox.currentText(),
+            self.antennaComboBox.currentText(),
             self.remarksTextEdit.toPlainText().strip(),
             self.commentLineEdit.text().strip(),
             self.calc_distance(self.locatorLineEdit.text(), self.ownLocatorLineEdit.text()),
             qsl_via,
             qsl_path,
             qsl_msg,
             qsl_sent,
             qsl_rcvd,
             eqsl_sent,
             eqsl_rcvd,
             lotw_sent,
             lotw_rcvd,
             'Y' if self.hamQTHCheckBox.isChecked() else 'N',
+            self.contestComboBox.currentText(),
+            self.sentQSOSpinBox.value(),
+            self.rcvdQSOSpinBox.value(),
+            self.rcvdDataLineEdit.text(),
         )
 
     @values.setter
     def values(self, values: dict):
         """Set all form values"""
         self.__old_values__ = values.copy()
 
@@ -697,16 +719,16 @@
 
         if values['propagation']:
             self.propComboBox.setCurrentText(self.prop[values['propagation']])
 
         self.ownNameLineEdit.setText(values['own_name'])
         self.ownQTHLineEdit.setText(values['own_qth'])
         self.ownLocatorLineEdit.setText(values['own_locator'])
-        self.radioLineEdit.setText(values['radio'])
-        self.antennaLineEdit.setText(values['antenna'])
+        self.radioComboBox.setCurrentText(values['radio'])
+        self.antennaComboBox.setCurrentText(values['antenna'])
         self.remarksTextEdit.setText(values['remarks'])
         self.commentLineEdit.setText(values['comments'].replace('\n', ' ').replace('\r', ''))
 
         if (values['qsl_sent'] in ('R', 'Y') or values['qsl_rcvd'] in ('R', 'Y') or
                 values['eqsl_sent'] in ('R', 'Y') or values['eqsl_rcvd'] in ('R', 'Y')):
 
             self.qslViaLineEdit.setText(values['qsl_via'])
@@ -735,14 +757,19 @@
 
         match values['hamqth']:
             case 'Y' | 'M':
                 self.hamQTHCheckBox.setChecked(True)
             case _:
                 self.hamQTHCheckBox.setChecked(False)
 
+        self.contestComboBox.setCurrentText(values['contest_id'])
+        self.sentQSOSpinBox.setValue(values['ctx_qso_id'] if values['ctx_qso_id'] else -1)
+        self.rcvdQSOSpinBox.setValue(values['crx_qso_id'] if values['crx_qso_id'] else -1)
+        self.rcvdDataLineEdit.setText(values['crx_data'])
+
     def searchHamQTH(self):
         self.searchCallbook(self.callbook_hamqth)
 
     def searchQRZCQ(self):
         self.searchCallbook(self.callbook_qrzcq)
 
     def searchCallbook(self, callbook):
@@ -1001,7 +1028,11 @@
         except LoTWRequestException as exc:
             QtWidgets.QMessageBox.warning(self, self.tr('Check LoTW Inbox error'),
                                           self.tr('Bad request result') + f'\n{exc}')
         except LoTWLoginException as exc:
             QtWidgets.QMessageBox.warning(self, self.tr('Check LoTW Inbox error'),
                                           self.tr('Login failed for user') + ': ' + self.settings.value(
                                               'lotw/username', '') + f'\n{exc}')
+
+    def keyPressEvent(self, e):
+        if e.key() != QtCore.Qt.Key.Key_Escape:
+            super().keyPressEvent(e)
```

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_QSOForm_ui.py` & `dragonlog-1.2/dragonlog/DragonLog_QSOForm_ui.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         QSOForm.setSizePolicy(sizePolicy)
         QSOForm.setMinimumSize(QtCore.QSize(500, 600))
         self.verticalLayout = QtWidgets.QVBoxLayout(QSOForm)
         self.verticalLayout.setObjectName("verticalLayout")
         self.toolBox = QtWidgets.QToolBox(parent=QSOForm)
         self.toolBox.setObjectName("toolBox")
         self.mainPage = QtWidgets.QWidget()
-        self.mainPage.setGeometry(QtCore.QRect(0, -3, 465, 493))
+        self.mainPage.setGeometry(QtCore.QRect(0, 0, 465, 493))
         self.mainPage.setObjectName("mainPage")
         self.verticalLayout_5 = QtWidgets.QVBoxLayout(self.mainPage)
         self.verticalLayout_5.setObjectName("verticalLayout_5")
         self.verticalLayout_2 = QtWidgets.QVBoxLayout()
         self.verticalLayout_2.setObjectName("verticalLayout_2")
         self.gridLayout_3 = QtWidgets.QGridLayout()
         self.gridLayout_3.setObjectName("gridLayout_3")
@@ -163,22 +163,24 @@
         self.ownLocatorLineEdit = QtWidgets.QLineEdit(parent=self.stationGroupBox)
         self.ownLocatorLineEdit.setEnabled(False)
         self.ownLocatorLineEdit.setObjectName("ownLocatorLineEdit")
         self.horizontalLayout_7.addWidget(self.ownLocatorLineEdit)
         self.verticalLayout_4.addLayout(self.horizontalLayout_7)
         self.horizontalLayout_6 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_6.setObjectName("horizontalLayout_6")
-        self.radioLineEdit = QtWidgets.QLineEdit(parent=self.stationGroupBox)
-        self.radioLineEdit.setEnabled(False)
-        self.radioLineEdit.setObjectName("radioLineEdit")
-        self.horizontalLayout_6.addWidget(self.radioLineEdit)
-        self.antennaLineEdit = QtWidgets.QLineEdit(parent=self.stationGroupBox)
-        self.antennaLineEdit.setEnabled(False)
-        self.antennaLineEdit.setObjectName("antennaLineEdit")
-        self.horizontalLayout_6.addWidget(self.antennaLineEdit)
+        self.radioComboBox = QtWidgets.QComboBox(parent=self.stationGroupBox)
+        self.radioComboBox.setEnabled(False)
+        self.radioComboBox.setEditable(True)
+        self.radioComboBox.setObjectName("radioComboBox")
+        self.horizontalLayout_6.addWidget(self.radioComboBox)
+        self.antennaComboBox = QtWidgets.QComboBox(parent=self.stationGroupBox)
+        self.antennaComboBox.setEnabled(False)
+        self.antennaComboBox.setEditable(True)
+        self.antennaComboBox.setObjectName("antennaComboBox")
+        self.horizontalLayout_6.addWidget(self.antennaComboBox)
         self.verticalLayout_4.addLayout(self.horizontalLayout_6)
         self.verticalLayout_2.addWidget(self.stationGroupBox)
         self.gridLayout = QtWidgets.QGridLayout()
         self.gridLayout.setObjectName("gridLayout")
         self.timeNowPushButton = QtWidgets.QPushButton(parent=self.mainPage)
         sizePolicy = QtWidgets.QSizePolicy(QtWidgets.QSizePolicy.Policy.Maximum, QtWidgets.QSizePolicy.Policy.Fixed)
         sizePolicy.setHorizontalStretch(0)
@@ -229,15 +231,15 @@
         self.remarksTextEdit.setAcceptRichText(False)
         self.remarksTextEdit.setTextInteractionFlags(QtCore.Qt.TextInteractionFlag.LinksAccessibleByKeyboard|QtCore.Qt.TextInteractionFlag.LinksAccessibleByMouse|QtCore.Qt.TextInteractionFlag.TextBrowserInteraction|QtCore.Qt.TextInteractionFlag.TextEditable|QtCore.Qt.TextInteractionFlag.TextEditorInteraction|QtCore.Qt.TextInteractionFlag.TextSelectableByKeyboard|QtCore.Qt.TextInteractionFlag.TextSelectableByMouse)
         self.remarksTextEdit.setObjectName("remarksTextEdit")
         self.verticalLayout_2.addWidget(self.remarksTextEdit)
         self.verticalLayout_5.addLayout(self.verticalLayout_2)
         self.toolBox.addItem(self.mainPage, "")
         self.qslPage = QtWidgets.QWidget()
-        self.qslPage.setGeometry(QtCore.QRect(0, 0, 482, 490))
+        self.qslPage.setGeometry(QtCore.QRect(0, 0, 465, 484))
         self.qslPage.setObjectName("qslPage")
         self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.qslPage)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
         self.qslGroupBox = QtWidgets.QGroupBox(parent=self.qslPage)
         self.qslGroupBox.setObjectName("qslGroupBox")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.qslGroupBox)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
@@ -362,19 +364,66 @@
         self.horizontalLayout_3.addWidget(self.hamQTHCheckBox)
         spacerItem10 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_3.addItem(spacerItem10)
         self.verticalLayout_6.addWidget(self.callbookGroupBox)
         spacerItem11 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_6.addItem(spacerItem11)
         self.toolBox.addItem(self.qslPage, "")
+        self.contestPage = QtWidgets.QWidget()
+        self.contestPage.setGeometry(QtCore.QRect(0, 0, 482, 460))
+        self.contestPage.setObjectName("contestPage")
+        self.formLayout = QtWidgets.QFormLayout(self.contestPage)
+        self.formLayout.setObjectName("formLayout")
+        self.label_10 = QtWidgets.QLabel(parent=self.contestPage)
+        self.label_10.setObjectName("label_10")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_10)
+        self.contestComboBox = QtWidgets.QComboBox(parent=self.contestPage)
+        self.contestComboBox.setEditable(True)
+        self.contestComboBox.setObjectName("contestComboBox")
+        self.formLayout.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.contestComboBox)
+        self.label_6 = QtWidgets.QLabel(parent=self.contestPage)
+        self.label_6.setObjectName("label_6")
+        self.formLayout.setWidget(3, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
+        self.horizontalLayout = QtWidgets.QHBoxLayout()
+        self.horizontalLayout.setObjectName("horizontalLayout")
+        self.sentQSOSpinBox = QtWidgets.QSpinBox(parent=self.contestPage)
+        self.sentQSOSpinBox.setMinimum(0)
+        self.sentQSOSpinBox.setMaximum(999)
+        self.sentQSOSpinBox.setProperty("value", 0)
+        self.sentQSOSpinBox.setObjectName("sentQSOSpinBox")
+        self.horizontalLayout.addWidget(self.sentQSOSpinBox)
+        spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout.addItem(spacerItem12)
+        self.formLayout.setLayout(3, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout)
+        self.label_9 = QtWidgets.QLabel(parent=self.contestPage)
+        self.label_9.setObjectName("label_9")
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_9)
+        self.rcvdDataLineEdit = QtWidgets.QLineEdit(parent=self.contestPage)
+        self.rcvdDataLineEdit.setObjectName("rcvdDataLineEdit")
+        self.formLayout.setWidget(5, QtWidgets.QFormLayout.ItemRole.FieldRole, self.rcvdDataLineEdit)
+        self.label_8 = QtWidgets.QLabel(parent=self.contestPage)
+        self.label_8.setObjectName("label_8")
+        self.formLayout.setWidget(8, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_8)
+        self.horizontalLayout_4 = QtWidgets.QHBoxLayout()
+        self.horizontalLayout_4.setObjectName("horizontalLayout_4")
+        self.rcvdQSOSpinBox = QtWidgets.QSpinBox(parent=self.contestPage)
+        self.rcvdQSOSpinBox.setMinimum(0)
+        self.rcvdQSOSpinBox.setMaximum(999)
+        self.rcvdQSOSpinBox.setProperty("value", 0)
+        self.rcvdQSOSpinBox.setObjectName("rcvdQSOSpinBox")
+        self.horizontalLayout_4.addWidget(self.rcvdQSOSpinBox)
+        spacerItem13 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_4.addItem(spacerItem13)
+        self.formLayout.setLayout(8, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout_4)
+        self.toolBox.addItem(self.contestPage, "")
         self.verticalLayout.addWidget(self.toolBox)
         self.horizontalLayout_2 = QtWidgets.QHBoxLayout()
         self.horizontalLayout_2.setObjectName("horizontalLayout_2")
-        spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
-        self.horizontalLayout_2.addItem(spacerItem12)
+        spacerItem14 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
+        self.horizontalLayout_2.addItem(spacerItem14)
         self.uploadPushButton = QtWidgets.QPushButton(parent=QSOForm)
         self.uploadPushButton.setObjectName("uploadPushButton")
         self.horizontalLayout_2.addWidget(self.uploadPushButton)
         self.savePushButton = QtWidgets.QPushButton(parent=QSOForm)
         self.savePushButton.setObjectName("savePushButton")
         self.horizontalLayout_2.addWidget(self.savePushButton)
         self.cancelPushButton = QtWidgets.QPushButton(parent=QSOForm)
@@ -384,16 +433,14 @@
 
         self.retranslateUi(QSOForm)
         self.toolBox.setCurrentIndex(0)
         self.savePushButton.clicked.connect(QSOForm.saveLog) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(self.dateOffEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownLocatorLineEdit.setDisabled) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(self.ownQTHLineEdit.setDisabled) # type: ignore
-        self.stationGroupBox.toggled['bool'].connect(self.radioLineEdit.setDisabled) # type: ignore
-        self.stationGroupBox.toggled['bool'].connect(self.antennaLineEdit.setDisabled) # type: ignore
         self.bandComboBox.currentTextChanged['QString'].connect(QSOForm.bandChanged) # type: ignore
         self.stationGroupBox.toggled['bool'].connect(QSOForm.stationChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(QSOForm.identityChanged) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownCallSignLineEdit.setDisabled) # type: ignore
         self.identityGroupBox.toggled['bool'].connect(self.ownNameLineEdit.setDisabled) # type: ignore
         self.channelComboBox.currentTextChanged['QString'].connect(QSOForm.channelChanged) # type: ignore
         self.RSTRcvdLineEdit.textEdited['QString'].connect(QSOForm.rstRcvdChanged) # type: ignore
@@ -412,17 +459,20 @@
         self.cancelPushButton.clicked.connect(QSOForm.clear) # type: ignore
         self.modeComboBox.currentTextChanged['QString'].connect(QSOForm.modeChanged) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(self.timeOffEdit.setDisabled) # type: ignore
         self.timeOnEdit.textEdited['QString'].connect(QSOForm.timeOnChanged) # type: ignore
         self.timeOffEdit.textEdited['QString'].connect(QSOForm.timeOffChanged) # type: ignore
         self.autoDateCheckBox.toggled['bool'].connect(QSOForm.autoDateCBChanged) # type: ignore
         self.searchQRZCQPushButton.clicked.connect(QSOForm.searchQRZCQ) # type: ignore
+        self.stationGroupBox.toggled['bool'].connect(self.antennaComboBox.setDisabled) # type: ignore
+        self.stationGroupBox.toggled['bool'].connect(self.radioComboBox.setDisabled) # type: ignore
         QtCore.QMetaObject.connectSlotsByName(QSOForm)
         QSOForm.setTabOrder(self.callSignLineEdit, self.searchHamQTHPushButton)
-        QSOForm.setTabOrder(self.searchHamQTHPushButton, self.RSTSentLineEdit)
+        QSOForm.setTabOrder(self.searchHamQTHPushButton, self.searchQRZCQPushButton)
+        QSOForm.setTabOrder(self.searchQRZCQPushButton, self.RSTSentLineEdit)
         QSOForm.setTabOrder(self.RSTSentLineEdit, self.RSTRcvdLineEdit)
         QSOForm.setTabOrder(self.RSTRcvdLineEdit, self.bandComboBox)
         QSOForm.setTabOrder(self.bandComboBox, self.channelComboBox)
         QSOForm.setTabOrder(self.channelComboBox, self.freqDoubleSpinBox)
         QSOForm.setTabOrder(self.freqDoubleSpinBox, self.modeComboBox)
         QSOForm.setTabOrder(self.modeComboBox, self.submodeComboBox)
         QSOForm.setTabOrder(self.submodeComboBox, self.nameLineEdit)
@@ -432,17 +482,15 @@
         QSOForm.setTabOrder(self.powerSpinBox, self.propComboBox)
         QSOForm.setTabOrder(self.propComboBox, self.identityGroupBox)
         QSOForm.setTabOrder(self.identityGroupBox, self.ownCallSignLineEdit)
         QSOForm.setTabOrder(self.ownCallSignLineEdit, self.ownNameLineEdit)
         QSOForm.setTabOrder(self.ownNameLineEdit, self.stationGroupBox)
         QSOForm.setTabOrder(self.stationGroupBox, self.ownQTHLineEdit)
         QSOForm.setTabOrder(self.ownQTHLineEdit, self.ownLocatorLineEdit)
-        QSOForm.setTabOrder(self.ownLocatorLineEdit, self.radioLineEdit)
-        QSOForm.setTabOrder(self.radioLineEdit, self.antennaLineEdit)
-        QSOForm.setTabOrder(self.antennaLineEdit, self.timeNowPushButton)
+        QSOForm.setTabOrder(self.ownLocatorLineEdit, self.timeNowPushButton)
         QSOForm.setTabOrder(self.timeNowPushButton, self.autoDateCheckBox)
         QSOForm.setTabOrder(self.autoDateCheckBox, self.dateOnEdit)
         QSOForm.setTabOrder(self.dateOnEdit, self.dateOffEdit)
         QSOForm.setTabOrder(self.dateOffEdit, self.eqslSentCheckBox)
         QSOForm.setTabOrder(self.eqslSentCheckBox, self.lotwSentCheckBox)
         QSOForm.setTabOrder(self.lotwSentCheckBox, self.qslAccBureauCheckBox)
         QSOForm.setTabOrder(self.qslAccBureauCheckBox, self.qslViaLineEdit)
@@ -496,16 +544,14 @@
         self.propComboBox.setPlaceholderText(_translate("QSOForm", "Propagation"))
         self.identityGroupBox.setTitle(_translate("QSOForm", "Configured identity"))
         self.ownCallSignLineEdit.setPlaceholderText(_translate("QSOForm", "Own call sign"))
         self.ownNameLineEdit.setPlaceholderText(_translate("QSOForm", "Own name"))
         self.stationGroupBox.setTitle(_translate("QSOForm", "Configured station"))
         self.ownQTHLineEdit.setPlaceholderText(_translate("QSOForm", "Own QTH"))
         self.ownLocatorLineEdit.setPlaceholderText(_translate("QSOForm", "Own locator"))
-        self.radioLineEdit.setPlaceholderText(_translate("QSOForm", "Radio"))
-        self.antennaLineEdit.setPlaceholderText(_translate("QSOForm", "Antenna"))
         self.timeNowPushButton.setText(_translate("QSOForm", "Now"))
         self.label_4.setText(_translate("QSOForm", "End"))
         self.timeOnEdit.setPlaceholderText(_translate("QSOForm", "Time start"))
         self.autoDateCheckBox.setText(_translate("QSOForm", "Automatically"))
         self.label_3.setText(_translate("QSOForm", "Start"))
         self.dateOnEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
         self.dateOffEdit.setDisplayFormat(_translate("QSOForm", "yyyy-MM-dd"))
@@ -537,11 +583,19 @@
         self.lotwGroupBox.setTitle(_translate("QSOForm", "LoTW"))
         self.lotwSentCheckBox.setText(_translate("QSOForm", "LoTW sent"))
         self.lotwRcvdCheckBox.setText(_translate("QSOForm", "LoTW received"))
         self.lotwInboxPushButton.setText(_translate("QSOForm", "Check Inbox"))
         self.callbookGroupBox.setTitle(_translate("QSOForm", "Logbook"))
         self.hamQTHCheckBox.setText(_translate("QSOForm", "HamQTH"))
         self.toolBox.setItemText(self.toolBox.indexOf(self.qslPage), _translate("QSOForm", "QSL && Log upload"))
+        self.label_10.setText(_translate("QSOForm", "Contest ID"))
+        self.contestComboBox.setPlaceholderText(_translate("QSOForm", "Contest ID"))
+        self.label_6.setText(_translate("QSOForm", "Sent QSO ID"))
+        self.sentQSOSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
+        self.label_9.setText(_translate("QSOForm", "Data"))
+        self.label_8.setText(_translate("QSOForm", "Rcvd QSO ID"))
+        self.rcvdQSOSpinBox.setSpecialValueText(_translate("QSOForm", "n.a."))
+        self.toolBox.setItemText(self.toolBox.indexOf(self.contestPage), _translate("QSOForm", "Contest"))
         self.uploadPushButton.setToolTip(_translate("QSOForm", "Uploads only if selected on QSL page"))
         self.uploadPushButton.setText(_translate("QSOForm", "Save && Upload"))
         self.savePushButton.setText(_translate("QSOForm", "Save"))
         self.cancelPushButton.setText(_translate("QSOForm", "Clear"))
```

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_Settings.py` & `dragonlog-1.2/dragonlog/DragonLog_Settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,39 +9,48 @@
 from PyQt6 import QtWidgets, QtCore, QtGui
 import keyring
 
 from . import DragonLog_Settings_ui
 from .Logger import Logger
 from .RegEx import REGEX_CALL, REGEX_LOCATOR, check_format
 from .CallBook import CallBookType
+from .ListEdit import ListEdit
 
 # Fix problems with importing win32 in frozen executable
 if getattr(sys, 'frozen', False):
     # noinspection PyUnresolvedReferences
     import win32timezone
     from keyring.backends import Windows
 
     keyring.set_keyring(Windows.WinVaultKeyring())
 
 
 class Settings(QtWidgets.QDialog, DragonLog_Settings_ui.Ui_Dialog):
     callbookChanged = QtCore.pyqtSignal(str)
     rigctldStatusChanged = QtCore.pyqtSignal(bool)
+    settingsStored = QtCore.pyqtSignal()
 
     def __init__(self, parent, settings: QtCore.QSettings, rig_status: QtWidgets.QLabel, cols: typing.Iterable,
                  logger: Logger):
         super().__init__(parent)
         self.setupUi(self)
 
         self.log = logging.getLogger('Settings')
         self.log.addHandler(logger)
         self.log.setLevel(logger.loglevel)
         self.logger = logger
         self.log.debug('Initialising...')
 
+        self.rigsListEdit = ListEdit(self.listingsWidget, self.tr('Radios'))
+        self.listingsWidget.layout().addWidget(self.rigsListEdit, 0, 0, 1, 1)
+        self.rigsListEdit.listChanged.connect(self.refreshRigsComboBox)
+        self.antsListEdit = ListEdit(self.listingsWidget, self.tr('Antennas'))
+        self.listingsWidget.layout().addWidget(self.antsListEdit, 0, 1, 1, 1)
+        self.antsListEdit.listChanged.connect(self.refreshAntsComboBox)
+
         self.settings = settings
         self.rig_ids = None
         self.rigs = None
         self.rigctld_path = None
         self.rigctld = None
         self.rig_caps = []
         self.rig_status = rig_status
@@ -81,14 +90,24 @@
 
         self.columns = cols
         self.sortComboBox.insertItems(0, cols)
 
         self.callbooks = dict([(cbt.value, cbt.name) for cbt in set(CallBookType)])
         self.callbookComboBox.insertItems(0, self.callbooks.keys())
 
+    def refreshRigsComboBox(self):
+        self.radioComboBox.clear()
+        self.radioComboBox.insertItems(0, self.rigsListEdit.items())
+        self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
+
+    def refreshAntsComboBox(self):
+        self.antennaComboBox.clear()
+        self.antennaComboBox.insertItems(0, self.antsListEdit.items())
+        self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
+
     def calcLocator(self):
         self.locatorLineEdit.setText(maidenhead.to_maiden(self.latitudeDoubleSpinBox.value(),
                                                           self.longitudeDoubleSpinBox.value(),
                                                           4))
 
     def checkRigctld(self):
         if self.rigctld and self.rigctld.poll():
@@ -305,20 +324,25 @@
         self.callbookUserLineEdit.setText(self.settings.value(f'callbook/{self.callbooks[service]}_user', ''))
 
     def exec(self):
         self.log.info('Loading settings...')
         self.catInterfaceLineEdit.setText(self.settings.value('cat/interface', ''))
         self.catBaudComboBox.setCurrentText(self.settings.value('cat/baud', ''))
 
+        self.rigsListEdit.clear()
+        self.rigsListEdit.setItems(self.settings.value('listings/rigs'))
+        self.antsListEdit.clear()
+        self.antsListEdit.setItems(self.settings.value('listings/antennas'))
+
         self.callsignLineEdit.setText(self.settings.value('station/callSign', ''))
         self.nameLineEdit.setText(self.settings.value('station/name', ''))
         self.QTHLineEdit.setText(self.settings.value('station/QTH', ''))
         self.locatorLineEdit.setText(self.settings.value('station/locator', ''))
-        self.radioLineEdit.setText(self.settings.value('station/radio', ''))
-        self.antennaLineEdit.setText(self.settings.value('station/antenna', ''))
+        self.radioComboBox.setCurrentText(self.settings.value('station/radio', ''))
+        self.antennaComboBox.setCurrentText(self.settings.value('station/antenna', ''))
 
         self.callsignCBLineEdit.setText(self.settings.value('station_cb/callSign', ''))
         self.radioCBLineEdit.setText(self.settings.value('station_cb/radio', ''))
         self.antennaCBLineEdit.setText(self.settings.value('station_cb/antenna', ''))
         self.cbDefaultCheckBox.setChecked(bool(self.settings.value('station_cb/cb_by_default', 0)))
         self.expCBQSOsCheckBox.setChecked(bool(self.settings.value('station_cb/cb_exp_adif', 0)))
 
@@ -389,16 +413,19 @@
         self.settings.setValue('cat/rigMfr', self.manufacturerComboBox.currentText())
         self.settings.setValue('cat/rigModel', self.modelComboBox.currentText())
 
         self.settings.setValue('station/callSign', self.callsignLineEdit.text())
         self.settings.setValue('station/name', self.nameLineEdit.text())
         self.settings.setValue('station/QTH', self.QTHLineEdit.text())
         self.settings.setValue('station/locator', self.locatorLineEdit.text())
-        self.settings.setValue('station/radio', self.radioLineEdit.text())
-        self.settings.setValue('station/antenna', self.antennaLineEdit.text())
+        self.settings.setValue('station/radio', self.radioComboBox.currentText())
+        self.settings.setValue('station/antenna', self.antennaComboBox.currentText())
+
+        self.settings.setValue('listings/rigs', self.rigsListEdit.items())
+        self.settings.setValue('listings/antennas', self.antsListEdit.items())
 
         self.settings.setValue('station_cb/callSign', self.callsignCBLineEdit.text())
         self.settings.setValue('station_cb/radio', self.radioCBLineEdit.text())
         self.settings.setValue('station_cb/antenna', self.antennaCBLineEdit.text())
         self.settings.setValue('station_cb/cb_by_default', int(self.cbDefaultCheckBox.isChecked()))
         self.settings.setValue('station_cb/cb_exp_adif', int(self.expCBQSOsCheckBox.isChecked()))
 
@@ -437,8 +464,9 @@
         if self.lotwUserLineEdit.text() and self.lotwPasswdLineEdit.text():
             keyring.set_password('lotw.arrl.org',
                                  self.lotwUserLineEdit.text(),
                                  self.lotwPasswdLineEdit.text())
         self.lotwPasswdLineEdit.clear()
         self.settings.value('lotw/cert_needs_pwd', int(self.lotwCertPwdCheckBox.isChecked()))
 
+        self.settingsStored.emit()
         super().accept()
```

### Comparing `dragonlog-1.1.3/dragonlog/DragonLog_Settings_ui.py` & `dragonlog-1.2/dragonlog/DragonLog_Settings_ui.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,34 +74,44 @@
         self.setLocatorPushButton = QtWidgets.QPushButton(parent=self.station)
         self.setLocatorPushButton.setObjectName("setLocatorPushButton")
         self.horizontalLayout.addWidget(self.setLocatorPushButton)
         self.formLayout.setLayout(4, QtWidgets.QFormLayout.ItemRole.FieldRole, self.horizontalLayout)
         self.label_5 = QtWidgets.QLabel(parent=self.station)
         self.label_5.setObjectName("label_5")
         self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_5)
-        self.radioLineEdit = QtWidgets.QLineEdit(parent=self.station)
-        self.radioLineEdit.setObjectName("radioLineEdit")
-        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.radioLineEdit)
         self.label_6 = QtWidgets.QLabel(parent=self.station)
         self.label_6.setObjectName("label_6")
         self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_6)
-        self.antennaLineEdit = QtWidgets.QLineEdit(parent=self.station)
-        self.antennaLineEdit.setObjectName("antennaLineEdit")
-        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.antennaLineEdit)
         spacerItem1 = QtWidgets.QSpacerItem(20, 20, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Minimum)
         self.formLayout.setItem(5, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem1)
         self.label_2 = QtWidgets.QLabel(parent=self.station)
         self.label_2.setObjectName("label_2")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_2)
         self.nameLineEdit = QtWidgets.QLineEdit(parent=self.station)
         self.nameLineEdit.setObjectName("nameLineEdit")
         self.formLayout.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.nameLineEdit)
         spacerItem2 = QtWidgets.QSpacerItem(20, 500, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.formLayout.setItem(8, QtWidgets.QFormLayout.ItemRole.FieldRole, spacerItem2)
+        self.radioComboBox = QtWidgets.QComboBox(parent=self.station)
+        self.radioComboBox.setObjectName("radioComboBox")
+        self.formLayout.setWidget(6, QtWidgets.QFormLayout.ItemRole.FieldRole, self.radioComboBox)
+        self.antennaComboBox = QtWidgets.QComboBox(parent=self.station)
+        self.antennaComboBox.setObjectName("antennaComboBox")
+        self.formLayout.setWidget(7, QtWidgets.QFormLayout.ItemRole.FieldRole, self.antennaComboBox)
         self.tabWidget.addTab(self.station, "")
+        self.listings = QtWidgets.QWidget()
+        self.listings.setObjectName("listings")
+        self.verticalLayout_12 = QtWidgets.QVBoxLayout(self.listings)
+        self.verticalLayout_12.setObjectName("verticalLayout_12")
+        self.listingsWidget = QtWidgets.QWidget(parent=self.listings)
+        self.listingsWidget.setObjectName("listingsWidget")
+        self.gridLayout = QtWidgets.QGridLayout(self.listingsWidget)
+        self.gridLayout.setObjectName("gridLayout")
+        self.verticalLayout_12.addWidget(self.listingsWidget)
+        self.tabWidget.addTab(self.listings, "")
         self.cb_station = QtWidgets.QWidget()
         self.cb_station.setObjectName("cb_station")
         self.formLayout_2 = QtWidgets.QFormLayout(self.cb_station)
         self.formLayout_2.setObjectName("formLayout_2")
         self.label_10 = QtWidgets.QLabel(parent=self.cb_station)
         self.label_10.setObjectName("label_10")
         self.formLayout_2.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_10)
@@ -334,48 +344,48 @@
         self.logToFileCheckBox.setObjectName("logToFileCheckBox")
         self.horizontalLayout_10.addWidget(self.logToFileCheckBox)
         spacerItem12 = QtWidgets.QSpacerItem(40, 20, QtWidgets.QSizePolicy.Policy.Expanding, QtWidgets.QSizePolicy.Policy.Minimum)
         self.horizontalLayout_10.addItem(spacerItem12)
         self.verticalLayout_5.addWidget(self.groupBox_8)
         self.horizontalLayout_6.addLayout(self.verticalLayout_5)
         self.tabWidget.addTab(self.userinterface, "")
-        self.tab = QtWidgets.QWidget()
-        self.tab.setObjectName("tab")
-        self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.tab)
+        self.import_export = QtWidgets.QWidget()
+        self.import_export.setObjectName("import_export")
+        self.verticalLayout_6 = QtWidgets.QVBoxLayout(self.import_export)
         self.verticalLayout_6.setObjectName("verticalLayout_6")
-        self.groupBox_3 = QtWidgets.QGroupBox(parent=self.tab)
+        self.groupBox_3 = QtWidgets.QGroupBox(parent=self.import_export)
         self.groupBox_3.setObjectName("groupBox_3")
         self.verticalLayout_7 = QtWidgets.QVBoxLayout(self.groupBox_3)
         self.verticalLayout_7.setObjectName("verticalLayout_7")
         self.expOwnNotesADIFCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_3)
         self.expOwnNotesADIFCheckBox.setObjectName("expOwnNotesADIFCheckBox")
         self.verticalLayout_7.addWidget(self.expOwnNotesADIFCheckBox)
         self.expRecentOnlyCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_3)
         self.expRecentOnlyCheckBox.setObjectName("expRecentOnlyCheckBox")
         self.verticalLayout_7.addWidget(self.expRecentOnlyCheckBox)
         self.verticalLayout_6.addWidget(self.groupBox_3)
-        self.groupBox_4 = QtWidgets.QGroupBox(parent=self.tab)
+        self.groupBox_4 = QtWidgets.QGroupBox(parent=self.import_export)
         self.groupBox_4.setObjectName("groupBox_4")
         self.verticalLayout_8 = QtWidgets.QVBoxLayout(self.groupBox_4)
         self.verticalLayout_8.setObjectName("verticalLayout_8")
         self.useCfgIDWatchCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_4)
         self.useCfgIDWatchCheckBox.setObjectName("useCfgIDWatchCheckBox")
         self.verticalLayout_8.addWidget(self.useCfgIDWatchCheckBox)
         self.useCfgStationWatchCheckBox = QtWidgets.QCheckBox(parent=self.groupBox_4)
         self.useCfgStationWatchCheckBox.setObjectName("useCfgStationWatchCheckBox")
         self.verticalLayout_8.addWidget(self.useCfgStationWatchCheckBox)
         self.verticalLayout_6.addWidget(self.groupBox_4)
         spacerItem13 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_6.addItem(spacerItem13)
-        self.tabWidget.addTab(self.tab, "")
-        self.tab_2 = QtWidgets.QWidget()
-        self.tab_2.setObjectName("tab_2")
-        self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.tab_2)
+        self.tabWidget.addTab(self.import_export, "")
+        self.credentials = QtWidgets.QWidget()
+        self.credentials.setObjectName("credentials")
+        self.verticalLayout_9 = QtWidgets.QVBoxLayout(self.credentials)
         self.verticalLayout_9.setObjectName("verticalLayout_9")
-        self.groupBox_5 = QtWidgets.QGroupBox(parent=self.tab_2)
+        self.groupBox_5 = QtWidgets.QGroupBox(parent=self.credentials)
         self.groupBox_5.setObjectName("groupBox_5")
         self.formLayout_4 = QtWidgets.QFormLayout(self.groupBox_5)
         self.formLayout_4.setObjectName("formLayout_4")
         self.label_16 = QtWidgets.QLabel(parent=self.groupBox_5)
         self.label_16.setObjectName("label_16")
         self.formLayout_4.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_16)
         self.callbookUserLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_5)
@@ -391,15 +401,15 @@
         self.callbookComboBox = QtWidgets.QComboBox(parent=self.groupBox_5)
         self.callbookComboBox.setObjectName("callbookComboBox")
         self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.FieldRole, self.callbookComboBox)
         self.label_24 = QtWidgets.QLabel(parent=self.groupBox_5)
         self.label_24.setObjectName("label_24")
         self.formLayout_4.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_24)
         self.verticalLayout_9.addWidget(self.groupBox_5)
-        self.groupBox_6 = QtWidgets.QGroupBox(parent=self.tab_2)
+        self.groupBox_6 = QtWidgets.QGroupBox(parent=self.credentials)
         self.groupBox_6.setObjectName("groupBox_6")
         self.formLayout_5 = QtWidgets.QFormLayout(self.groupBox_6)
         self.formLayout_5.setObjectName("formLayout_5")
         self.label_18 = QtWidgets.QLabel(parent=self.groupBox_6)
         self.label_18.setObjectName("label_18")
         self.formLayout_5.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_18)
         self.eqslUserLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_6)
@@ -409,15 +419,15 @@
         self.label_19.setObjectName("label_19")
         self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_19)
         self.eqslPasswdLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_6)
         self.eqslPasswdLineEdit.setEchoMode(QtWidgets.QLineEdit.EchoMode.PasswordEchoOnEdit)
         self.eqslPasswdLineEdit.setObjectName("eqslPasswdLineEdit")
         self.formLayout_5.setWidget(1, QtWidgets.QFormLayout.ItemRole.FieldRole, self.eqslPasswdLineEdit)
         self.verticalLayout_9.addWidget(self.groupBox_6)
-        self.groupBox_81 = QtWidgets.QGroupBox(parent=self.tab_2)
+        self.groupBox_81 = QtWidgets.QGroupBox(parent=self.credentials)
         self.groupBox_81.setObjectName("groupBox_81")
         self.formLayout_6 = QtWidgets.QFormLayout(self.groupBox_81)
         self.formLayout_6.setObjectName("formLayout_6")
         self.label_22 = QtWidgets.QLabel(parent=self.groupBox_81)
         self.label_22.setObjectName("label_22")
         self.formLayout_6.setWidget(0, QtWidgets.QFormLayout.ItemRole.LabelRole, self.label_22)
         self.lotwUserLineEdit = QtWidgets.QLineEdit(parent=self.groupBox_81)
@@ -440,15 +450,15 @@
         self.line.setFrameShape(QtWidgets.QFrame.Shape.HLine)
         self.line.setFrameShadow(QtWidgets.QFrame.Shadow.Sunken)
         self.line.setObjectName("line")
         self.formLayout_6.setWidget(2, QtWidgets.QFormLayout.ItemRole.FieldRole, self.line)
         self.verticalLayout_9.addWidget(self.groupBox_81)
         spacerItem14 = QtWidgets.QSpacerItem(20, 40, QtWidgets.QSizePolicy.Policy.Minimum, QtWidgets.QSizePolicy.Policy.Expanding)
         self.verticalLayout_9.addItem(spacerItem14)
-        self.tabWidget.addTab(self.tab_2, "")
+        self.tabWidget.addTab(self.credentials, "")
         self.verticalLayout.addWidget(self.tabWidget)
         self.buttonBox = QtWidgets.QDialogButtonBox(parent=Dialog)
         self.buttonBox.setOrientation(QtCore.Qt.Orientation.Horizontal)
         self.buttonBox.setStandardButtons(QtWidgets.QDialogButtonBox.StandardButton.Cancel|QtWidgets.QDialogButtonBox.StandardButton.Ok)
         self.buttonBox.setObjectName("buttonBox")
         self.verticalLayout.addWidget(self.buttonBox)
 
@@ -485,14 +495,15 @@
         self.label_7.setText(_translate("Dialog", "Lon"))
         self.longitudeDoubleSpinBox.setSuffix(_translate("Dialog", "°"))
         self.setLocatorPushButton.setText(_translate("Dialog", "Set locator"))
         self.label_5.setText(_translate("Dialog", "Radio"))
         self.label_6.setText(_translate("Dialog", "Antenna"))
         self.label_2.setText(_translate("Dialog", "Name"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.station), _translate("Dialog", "Station"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.listings), _translate("Dialog", "Listings"))
         self.label_10.setText(_translate("Dialog", "Call sign"))
         self.label_9.setText(_translate("Dialog", "Radio"))
         self.label_11.setText(_translate("Dialog", "Antenna"))
         self.cbDefaultCheckBox.setText(_translate("Dialog", "Select CB band by default"))
         self.expCBQSOsCheckBox.setToolTip(_translate("Dialog", "On import CB QSOs will always be handled"))
         self.expCBQSOsCheckBox.setText(_translate("Dialog", "Export CB QSOs to ADIF"))
         self.tabWidget.setTabText(self.tabWidget.indexOf(self.cb_station), _translate("Dialog", "CB-Station"))
@@ -535,23 +546,23 @@
         self.groupBox_3.setTitle(_translate("Dialog", "Export"))
         self.expOwnNotesADIFCheckBox.setText(_translate("Dialog", "Export own notes to ADIF"))
         self.expRecentOnlyCheckBox.setToolTip(_translate("Dialog", "See settings page \"User interface\""))
         self.expRecentOnlyCheckBox.setText(_translate("Dialog", "Export only recent QSOs"))
         self.groupBox_4.setTitle(_translate("Dialog", "Watch File"))
         self.useCfgIDWatchCheckBox.setText(_translate("Dialog", "Use configured ID for missing values"))
         self.useCfgStationWatchCheckBox.setText(_translate("Dialog", "Use configured Station for missing values"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab), _translate("Dialog", "Import/Export"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.import_export), _translate("Dialog", "Import/Export"))
         self.groupBox_5.setTitle(_translate("Dialog", "Callbook"))
         self.label_16.setText(_translate("Dialog", "Username"))
         self.label_17.setText(_translate("Dialog", "Password"))
         self.label_24.setText(_translate("Dialog", "Service"))
         self.groupBox_6.setTitle(_translate("Dialog", "eQSL"))
         self.label_18.setText(_translate("Dialog", "Username"))
         self.label_19.setText(_translate("Dialog", "Password"))
         self.groupBox_81.setTitle(_translate("Dialog", "LoTW"))
         self.label_22.setText(_translate("Dialog", "Username"))
         self.lotwUserLineEdit.setToolTip(_translate("Dialog", "Username for LoTW online account not for the certificate"))
         self.label_211.setText(_translate("Dialog", "Password"))
         self.lotwPasswdLineEdit.setToolTip(_translate("Dialog", "Password for LoTW online account not for the certificate"))
         self.lotwCertPwdCheckBox.setText(_translate("Dialog", "Certificate needs password"))
         self.label_23.setText(_translate("Dialog", "TQSL"))
-        self.tabWidget.setTabText(self.tabWidget.indexOf(self.tab_2), _translate("Dialog", "Credentials"))
+        self.tabWidget.setTabText(self.tabWidget.indexOf(self.credentials), _translate("Dialog", "Credentials"))
```

### Comparing `dragonlog-1.1.3/dragonlog/LoTW.py` & `dragonlog-1.2/dragonlog/LoTW.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/Logger.py` & `dragonlog-1.2/dragonlog/Logger.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/RegEx.py` & `dragonlog-1.2/dragonlog/RegEx.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import re
 
 REGEX_CALL = re.compile(r'([a-zA-Z0-9]{1,3}?/)?([a-zA-Z0-9]{1,3}?[0-9][a-zA-Z0-9]{0,3}?[a-zA-Z])(/[aAmMpPrRtT]{1,2}?)?')
 REGEX_RSTFIELD = re.compile(r'([1-5][1-9][1-9aAcCkKmMsSxX]?)|([rR]?[-+]?[0-9]{1,2})')
 REGEX_LOCATOR = re.compile(r'[a-rA-R]{2}[0-9]{2}([a-xA-X]{2}([0-9]{2})?)?')
 REGEX_NONASCII = re.compile(r'[ -~\n\r]*(.)?')
 REGEX_TIME = re.compile(r'(([0-1][0-9])|(2[0-3])):([0-5][0-9])(:[0-5][0-9])?')
+REGEX_DATE = re.compile(r'([1-9][0-9]{3})-((0[1-9])|(1[0-2]))-((0[1-9])|([1-2][0-9])|(3[0-2]))')
 
 def check_format(exp: re.Pattern, txt: str) -> bool:
     """Test the given text against a regular expression
     :param exp: a compiled pattern
     :param txt: a text
     :return: true if pattern matches"""
     return bool(re.fullmatch(exp, txt))
```

### Comparing `dragonlog-1.1.3/dragonlog/data/README.md` & `dragonlog-1.2/dragonlog/data/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -33,15 +33,16 @@
 * log 11m band QSOs
 * filter recent QSOs (last week, month, half year, year)
 * UTF-8 (i.e. use german umlauts)
 * convert non ASCII characters for ADIF export (for supported languages)
 
 Installation
 ------------
-The installation requires a python installation (>= 3.9).
+The installation requires a python installation (>= 3.10). 
+On Linux you may have to install libxcb-cursor0.
     
     # python3 -m pip install DragonLog
 
 If you want to be able to export/import to/from Excel files install the extra packages
 
     # python3 -m pip install DragonLog[extra]
 
@@ -52,14 +53,15 @@
 Or if your python scripts folder is on PATH you can start DragonLog with 
 
     # DragonLog
 
 
 For windows there is also an installable MSI and ZIP package available for convenience.
 
+
 First start
 -----------
 Before you can start to log QSOs a database has to be selected.
 It can be placed on a path where you wish to.
 The database is created and initialised.
 
 At the next start of the program the last database gets opened automatically.
```

### Comparing `dragonlog-1.1.3/dragonlog/data/bands.json` & `dragonlog-1.2/dragonlog/data/bands.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/data/cb_channels.json` & `dragonlog-1.2/dragonlog/data/cb_channels.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/data/color_map.json` & `dragonlog-1.2/dragonlog/data/color_map.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/data/i18n/DragonLog_de.qm` & `dragonlog-1.2/dragonlog/data/i18n/DragonLog_de.qm`

 * *Files 3% similar despite different names*

```diff
@@ -1,1545 +1,1627 @@
 00000000: 3cb8 6418 caef 9c95 cd21 1cbf 60a1 bddd  <.d......!..`...
-00000010: a700 0000 0564 655f 4445 4200 0009 f800  .....de_DEB.....
+00000010: a700 0000 0564 655f 4445 4200 000a a800  .....de_DEB.....
 00000020: 0000 3c00 0001 5c00 0000 3e00 0001 7800  ..<...\...>...x.
-00000030: 0000 4d00 0054 8a00 0000 4e00 0054 c400  ..M..T....N..T..
-00000040: 0000 5200 0054 f600 0000 5900 0055 3200  ..R..T....Y..U2.
-00000050: 0002 5700 0035 7400 0003 8900 0035 b200  ..W..5t......5..
-00000060: 0005 5b00 0023 9900 000c d000 0011 7100  ..[..#........q.
+00000030: 0000 4d00 0058 f300 0000 4e00 0059 2d00  ..M..X....N..Y-.
+00000040: 0000 5200 0059 5f00 0000 5900 0059 9b00  ..R..Y_...Y..Y..
+00000050: 0002 5700 0038 c800 0003 8900 0039 0600  ..W..8.......9..
+00000060: 0005 5b00 0023 f300 000c d000 0011 a600  ..[..#..........
 00000070: 0031 0e00 0000 0000 0047 6400 0001 fe00  .1.......Gd.....
-00000080: 004c 4400 003e aa00 0052 8400 0007 8600  .LD..>...R......
-00000090: 0053 5e00 0008 b400 0055 6700 0043 2d00  .S^......Ug..C-.
-000000a0: 0056 7c00 0045 3500 0056 7f00 0026 5600  .V|..E5..V...&V.
-000000b0: 0056 8800 000a 9200 0056 8800 0026 fe00  .V.......V...&..
-000000c0: 0056 8800 0047 8700 0058 f700 000b 0e00  .V...G...X......
-000000d0: 026f fa00 0035 9200 0345 3000 0000 3f00  .o...5...E0...?.
+00000080: 004c 4400 0042 4c00 0052 8400 0007 8c00  .LD..BL..R......
+00000090: 0053 5e00 0008 e900 0055 6700 0046 cf00  .S^......Ug..F..
+000000a0: 0056 7c00 0048 d700 0056 7f00 0026 b000  .V|..H...V...&..
+000000b0: 0056 8800 000a c700 0056 8800 0027 5800  .V.......V...'X.
+000000c0: 0056 8800 004b 2900 0058 f700 000b 4300  .V...K)..X....C.
+000000d0: 026f fa00 0038 e600 0345 3000 0000 3f00  .o...8...E0...?.
 000000e0: 0357 3000 0000 bf00 037b 3000 0000 fe00  .W0......{0.....
-000000f0: 03c9 3000 0001 3d00 0488 4400 0015 1900  ..0...=...D.....
-00000100: 0488 4400 0039 2f00 04bb 0400 0031 1600  ..D..9/......1..
-00000110: 04cf 0400 0031 4d00 04d0 2500 0031 e700  .....1M...%..1..
-00000120: 04e7 1000 001e 1d00 04ec 3000 001d f100  ..........0.....
-00000130: 04ec 3000 0032 1400 0534 9700 0007 da00  ..0..2...4......
-00000140: 0534 9700 0040 1f00 0545 a500 0022 bb00  .4...@...E..."..
-00000150: 0545 a500 0042 4a00 0548 3500 0008 dc00  .E...BJ..H5.....
-00000160: 0548 3500 0022 dd00 0548 3500 0042 6a00  .H5.."...H5..Bj.
-00000170: 0596 7c00 000e 5800 0598 c500 0048 8900  ..|...X......H..
-00000180: 05ab 6000 0052 d900 06a6 7c00 0011 5200  ..`..R....|...R.
-00000190: 06a6 7c00 004d df00 06fb 2100 0042 1100  ..|..M....!..B..
-000001a0: 0714 3e00 004e 8300 144b 9e00 000d c500  ..>..N...K......
-000001b0: 144e e600 0021 1300 3477 3000 0000 7f00  .N...!..4w0.....
-000001c0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
-000001d0: 376f f400 004b b800 38a9 3000 0001 1d00  7o...K..8.0.....
-000001e0: 4796 c400 0013 7f00 4796 c400 002e eb00  G.......G.......
-000001f0: 47ab 7600 002e b800 47ab 7600 0053 6800  G.v.....G.v..Sh.
-00000200: 4a2b 8200 003c a800 4c99 6200 001b a400  J+...<..L.b.....
-00000210: 4c99 6200 003e d100 52cc bc00 0007 b000  L.b..>..R.......
-00000220: 556a c300 0023 6800 567e 8100 0045 1400  Uj...#h.V~...E..
-00000230: 56ae c200 0055 8b00 576d c200 0024 c800  V....U..Wm...$..
-00000240: 576d c200 0044 9e00 587a ff00 000a b000  Wm...D..Xz......
-00000250: 587a ff00 0027 8d00 587a ff00 0048 6800  Xz...'..Xz...Hh.
-00000260: 5aa8 9400 000e 1600 5aa8 9400 0049 cf00  Z.......Z....I..
-00000270: 5aa8 9400 0052 7400 67ab 0600 0053 3c00  Z....Rt.g....S<.
-00000280: 6d92 9400 0051 1400 753c 2300 0044 5d00  m....Q..u<#..D].
-00000290: 8cd2 1500 0010 4200 aa80 2500 001a 6300  ......B...%...c.
-000002a0: ab72 4500 0009 cf00 bf5b b400 0005 f700  .rE......[......
-000002b0: c656 de00 003d 3000 ff2c 7700 001c 2c01  .V...=0..,w...,.
-000002c0: 30ed a300 001c c301 48c4 ff00 001a 9d01  0.......H.......
-000002d0: 4d8a bc00 0021 8801 5478 6c00 0022 1e01  M....!..Txl.."..
-000002e0: 945e f800 0029 3301 9942 b500 0042 8a01  .^...)3..B...B..
-000002f0: 9ce8 5e00 004a 9801 e578 e300 000d 5601  ..^..J...x....V.
-00000300: e907 4500 0042 da01 fdeb 5400 004d ff02  ..E..B....T..M..
-00000310: 3222 f900 0038 8a02 33a9 3400 0008 fb02  2"...8..3.4.....
-00000320: ac2b 0200 0041 7e02 e7d6 5e00 0002 4102  .+...A~...^...A.
-00000330: e7d6 5e00 0015 8b02 e7d6 5e00 0039 b802  ..^.......^..9..
-00000340: e81d 2400 003d fb03 004d 1200 000c 5d03  ..$..=...M....].
-00000350: 0149 e600 0021 4003 0cac 0500 000f cc03  .I...!@.........
-00000360: 0f6b 1200 0043 dc03 0f6b 3200 0023 b903  .k...C...k2..#..
-00000370: 1bec 1200 0013 de03 4485 3000 0000 1e03  ........D.0.....
-00000380: 45b3 3000 0000 5e03 4ecb 9200 0034 0f03  E.0...^.N....4..
-00000390: 4ecb 9200 0052 9603 533f be00 0055 b403  N....R..S?...U..
-000003a0: 598b 3200 0007 f903 598b 3200 0020 ee03  Y.2.....Y.2.. ..
-000003b0: 598b 3200 0040 c503 5d96 0b00 0040 e803  Y.2..@..]....@..
-000003c0: 6cc3 0400 000b c703 881f d400 0006 2003  l............. .
-000003d0: 9ce3 f400 001e 3f03 9ce9 a500 0025 3a03  ......?......%:.
-000003e0: f5e0 0700 002d 9804 07f6 ee00 0024 7904  .....-.......$y.
-000003f0: 07f6 ee00 0043 8f04 2b4e 0500 001d 6c04  .....C..+N....l.
-00000400: 6c90 3200 0041 0b04 8c96 8100 0014 5f04  l.2..A........_.
-00000410: 8caf 6200 0014 a904 9c8b 8500 0039 4f04  ..b..........9O.
-00000420: a472 8400 002b 4704 ab8e f500 002f e804  .r...+G....../..
-00000430: ab8e fc00 0030 0d04 ab8f 0100 0030 3204  .....0.......02.
-00000440: ab8f 0700 0030 5704 ab8f 0800 0030 7c04  .....0W......0|.
-00000450: b08b a400 003d 8804 b2b6 6400 0008 6d04  .....=....d...m.
-00000460: c4a9 a900 0013 4604 cf76 9400 0004 9404  ......F..v......
-00000470: cf76 9400 0031 7e04 e826 8800 001d a904  .v...1~..&......
-00000480: e826 8800 003f 8204 e842 f200 001d cd04  .&...?...B......
-00000490: e842 f200 0051 8a04 edd3 6400 0036 5604  .B...Q....d..6V.
-000004a0: f5b6 e700 002a 3705 0476 9400 0032 4105  .....*7..v...2A.
-000004b0: 1f06 1500 0051 ad05 3268 c400 0004 1805  .....Q..2h......
-000004c0: 34db 8200 0021 d605 3ddf a300 000a d005  4....!..=.......
-000004d0: 4466 8200 0049 0b05 5776 4500 0045 a305  Df...I..WvE..E..
-000004e0: 6336 9e00 0032 aa05 647d 0e00 002f 9405  c6...2..d}.../..
-000004f0: 7865 9800 0047 a605 7865 b800 0047 c805  xe...G..xe...G..
-00000500: 8ed0 0500 0054 1f05 c7f7 2800 0056 1805  .....T....(..V..
-00000510: c984 e900 0030 a106 011e c400 0002 9c06  .....0..........
-00000520: 778d 0800 0006 cf06 778d 0800 001f 2106  w.......w.....!.
-00000530: 7e7c a100 0026 2306 7e7c a100 0046 6906  ~|...&#.~|...Fi.
-00000540: 830d be00 0029 f106 bdf0 a400 0019 8f06  .....)..........
-00000550: be94 d200 0052 fa06 d2af d900 0056 4206  .....R.......VB.
-00000560: db4d 4200 0027 f206 e056 d800 0024 3e06  .MB..'...V...$>.
-00000570: e056 d800 0043 5606 f895 8e00 0015 f507  .V...CV.........
-00000580: 2f4a 1500 004a 3607 366b 9300 0005 1a07  /J...J6.6k......
-00000590: 50be 3900 0053 9a07 68f8 4400 004e ab07  P.9..S..h.D..N..
-000005a0: 693d fe00 0031 a307 6941 4e00 0032 6607  i=...1..iAN..2f.
-000005b0: 6cbb 6300 000e 7707 7f18 a400 004b ec07  l.c...w......K..
-000005c0: 86be 4800 0036 d507 8f3a 3e00 0024 fb07  ..H..6...:>..$..
-000005d0: 8f3a 3e00 0044 cf07 e67a d700 0030 ee07  .:>..D...z...0..
-000005e0: e76d c800 0025 7d07 e78f a400 0025 b307  .m...%}......%..
-000005f0: e79f 3400 0025 eb07 e79f 3400 0046 2d07  ..4..%....4..F-.
-00000600: e7e0 a400 002e 4207 e7f2 3400 002e 7d07  ......B...4...}.
-00000610: e7f2 3400 004e 4408 14d3 ed00 0032 eb08  ..4..ND......2..
-00000620: 14d3 ed00 0046 9a08 3292 cb00 0002 7908  .....F..2.....y.
-00000630: 3587 6a00 002b a608 36b6 5400 0012 8a08  5.j..+..6.T.....
-00000640: 5ac5 0100 0001 9408 5ac5 0100 0014 2c08  Z.......Z.....,.
-00000650: 5ac5 0100 0038 5908 678f b400 0027 1f08  Z....8Y.g....'..
-00000660: 679f 2400 0027 5708 679f 2400 0048 2c08  g.$..'W.g.$..H,.
-00000670: 7f52 2500 002a e608 8879 1400 0019 2108  .R%..*...y....!.
-00000680: aae3 e400 0009 9c08 b63d de00 0034 fd08  .........=...4..
-00000690: bd74 5e00 0022 ff08 d39b 6400 0040 3f08  .t^.."....d..@?.
-000006a0: f89a cb00 0035 d009 14be 9200 0049 6309  .....5.......Ic.
-000006b0: 1c52 9500 002d f709 238c 7500 0016 f209  .R...-..#.u.....
-000006c0: 3f8c ad00 000c da09 564e 4200 004c 2409  ?.......VNB..L$.
-000006d0: 6c61 f400 0013 aa09 6c61 f400 002f 1709  la......la.../..
-000006e0: 6fe6 7e00 0011 8e09 8fa3 8700 002f 4c09  o.~........../L.
-000006f0: 97c9 1400 0020 b309 97c9 1400 0040 8409  ..... .......@..
-00000700: 97d9 8400 0020 7809 9c7f 1a00 0037 7209  ..... x......7r.
-00000710: a118 8500 0011 0d09 c004 d700 0003 df09  ................
-00000720: c4e8 d700 0001 c409 c8df a200 001e 9409  ................
-00000730: c943 f500 0010 0709 c9cf c500 000c 2f09  .C............/.
-00000740: df31 3800 0047 1709 e854 fc00 0015 c609  .18..G...T......
-00000750: e854 fc00 003b 1a09 f42c fb00 001b 7e0a  .T...;...,....~.
-00000760: 16bb 3400 0046 d60a 2087 bc00 003b f80a  ..4..F.. ....;..
-00000770: 2190 e200 0006 860a 2190 e200 001e d50a  !.......!.......
-00000780: 3f0e 9500 0028 ea0a 5e68 d900 0026 770a  ?....(..^h...&w.
-00000790: 643c 1400 0016 bb0a 6789 3b00 0007 0e0a  d<......g.;.....
-000007a0: 6789 3b00 001f 630a 67a9 0200 0007 4a0a  g.;...c.g.....J.
-000007b0: 67a9 0200 001f a20a 6dc8 3e00 0034 960a  g.......m.>..4..
-000007c0: 7833 e400 0039 790a 7d6b 2400 0018 550a  x3...9y.}k$...U.
-000007d0: 92a2 e500 0029 9d0a 9612 e500 0028 900a  .....).......(..
-000007e0: a8b0 0e00 000e 360a a8b0 0e00 0049 f00a  ......6......I..
-000007f0: acdb 7e00 0002 1c0a b945 f500 002b 220a  ..~......E...+".
-00000800: b945 f500 004a 130a c389 2500 0028 590a  .E...J....%..(Y.
-00000810: c5b4 4900 003f a40a c897 c500 0006 480a  ..I..?........H.
-00000820: d2f0 b500 0003 090a d382 7700 0003 570a  ..........w...W.
-00000830: e2b5 9600 0004 b50a f31c 2200 003b 840b  .........."..;..
-00000840: 1562 0700 004f 300b 1805 3900 0015 3b0b  .b...O0...9...;.
-00000850: 4597 5500 0008 1b0b 5d8a f400 001f e10b  E.U.....].......
-00000860: 6628 d200 0034 540b 7fe2 de00 0033 2a0b  f(...4T......3*.
-00000870: ad17 7800 001b 500b ff25 ce00 001c 7e0c  ..x...P..%....~.
-00000880: 08f5 6c00 003d b60c 107d 9300 0003 a10c  ..l..=...}......
-00000890: 10ba b200 0027 b00c 1536 f700 002d 190c  .....'...6...-..
-000008a0: 1f2f 0200 004c 750c 29f2 a400 004f 0a0c  ./...Lu.)....O..
-000008b0: 6a19 e900 003c e10c 8c09 2900 001d 350c  j....<....)...5.
-000008c0: 8c09 2900 003f 4d0c 9688 9500 0014 830c  ..)..?M.........
-000008d0: a3fa 5f00 001a 250c a6e8 d400 003a 5e0c  .._...%......:^.
-000008e0: bb01 7300 000c 9d0c bb01 7300 0033 810c  ..s.......s..3..
-000008f0: c9a0 0e00 002d 730d 0218 6400 0048 bb0d  .....-s...d..H..
-00000900: 07a4 f800 003b 470d 1f27 b200 0014 d70d  .....;G..'......
-00000910: 3504 b400 003a ba0d 76f7 5900 001b d30d  5....:..v.Y.....
-00000920: 825f 7300 000f 1a0d a03c 1200 0050 020d  ._s......<...P..
-00000930: d0ff 4c00 002c cd0d f2ea c200 003c 3e0d  ..L..,.......<>.
-00000940: fe4e 2400 0019 d80d fe4e 2400 0050 c80e  .N$......N$..P..
-00000950: 0543 5500 0024 000e 05d1 b500 0050 610e  .CU..$.......Pa.
-00000960: 0743 5500 0044 210e 0906 8800 0037 ac0e  .CU..D!......7..
-00000970: 233d d500 004c bb0e 87ac 6400 0020 2a0e  #=...L....d.. *.
-00000980: 93fa 5200 0017 970e a32f e400 003e fe0e  ..R....../...>..
-00000990: c497 a200 000b 3e0e c72a a600 0005 820e  ......>..*......
-000009a0: de3d a200 0039 f10e e46b 3400 0047 ea0e  .=...9...k4..G..
-000009b0: fdeb 3400 0045 eb0f 165e c400 0045 540f  ..4..E...^...ET.
-000009c0: 3562 ce00 0017 f80f 6963 bc00 000d 1f0f  5b......ic......
-000009d0: 6963 bc00 002a ac0f 6963 bc00 0052 3b0f  ic...*..ic...R;.
-000009e0: 6978 c700 0033 c20f 6c98 6c00 0055 600f  ix...3..l.l..U`.
-000009f0: 7ddd 2800 004d 630f 8007 d400 0038 c90f  }.(..Mc......8..
-00000a00: 8313 8900 0013 130f cb15 5200 0018 d70f  ..........R.....
-00000a10: e6f6 3400 003f cc69 0000 566c 03ff ffff  ..4..?.i..Vl....
-00000a20: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
-00000a30: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000a40: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
-00000a50: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000a60: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
-00000a70: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000a80: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
-00000a90: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000aa0: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
-00000ab0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000ac0: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
-00000ad0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
-00000ae0: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
-00000af0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000b00: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
-00000b10: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000b20: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
-00000b30: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000b40: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
-00000b50: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
-00000b60: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
-00000b70: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000b80: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
-00000b90: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00000ba0: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
-00000bb0: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
-00000bc0: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
-00000bd0: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
-00000be0: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
-00000bf0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
-00000c00: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
-00000c10: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
-00000c20: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
-00000c30: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00000c40: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
-00000c50: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
-00000c60: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
-00000c70: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
-00000c80: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
-00000c90: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
-00000ca0: 0000 0008 4361 6c6c 626f 6f6b 0700 0000  ....Callbook....
-00000cb0: 0644 6961 6c6f 6701 0300 0000 3800 5a00  .Dialog.....8.Z.
-00000cc0: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
-00000cd0: 7400 2000 6200 6500 6e00 f600 7400 6900  t. .b.e.n...t.i.
-00000ce0: 6700 7400 2000 5000 6100 7300 7300 7700  g.t. .P.a.s.s.w.
-00000cf0: 6f00 7200 7408 0000 0000 0600 0000 1a43  o.r.t..........C
-00000d00: 6572 7469 6669 6361 7465 206e 6565 6473  ertificate needs
-00000d10: 2070 6173 7377 6f72 6407 0000 0006 4469   password.....Di
-00000d20: 616c 6f67 0103 0000 0024 0053 0070 0061  alog.....$.S.p.a
-00000d30: 006c 0074 0065 006e 0020 0076 0065 0072  .l.t.e.n. .v.e.r
-00000d40: 0073 0074 0065 0063 006b 0065 006e 0800  .s.t.e.c.k.e.n..
-00000d50: 0000 0006 0000 000f 436f 6c75 6d6e 7320  ........Columns 
-00000d60: 746f 2068 6964 6507 0000 0006 4469 616c  to hide.....Dial
-00000d70: 6f67 0103 0000 0020 0053 0070 0061 006c  og..... .S.p.a.l
-00000d80: 0074 0065 006e 0020 0061 006e 007a 0065  .t.e.n. .a.n.z.e
-00000d90: 0069 0067 0065 006e 0800 0000 0006 0000  .i.g.e.n........
-00000da0: 000f 436f 6c75 6d6e 7320 746f 2073 686f  ..Columns to sho
-00000db0: 7707 0000 0006 4469 616c 6f67 0103 0000  w.....Dialog....
-00000dc0: 0018 0041 006e 006d 0065 006c 0064 0065  ...A.n.m.e.l.d.e
-00000dd0: 0064 0061 0074 0065 006e 0800 0000 0006  .d.a.t.e.n......
-00000de0: 0000 000b 4372 6564 656e 7469 616c 7307  ....Credentials.
-00000df0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
-00000e00: 0041 0062 0073 0074 0065 0069 0067 0065  .A.b.s.t.e.i.g.e
-00000e10: 006e 0064 0800 0000 0006 0000 000a 4465  .n.d..........De
-00000e20: 7363 656e 6469 6e67 0700 0000 0644 6961  scending.....Dia
-00000e30: 6c6f 6701 0300 0000 3e00 5700 6900 7200  log.....>.W.i.r.
-00000e40: 6b00 7300 6100 6d00 2000 6e00 6100 6300  k.s.a.m. .n.a.c.
-00000e50: 6800 2000 4100 6e00 7700 6500 6e00 6400  h. .A.n.w.e.n.d.
-00000e60: 7500 6e00 6700 7300 6e00 6500 7500 7300  u.n.g.s.n.e.u.s.
-00000e70: 7400 6100 7200 7408 0000 0000 0600 0000  t.a.r.t.........
-00000e80: 2345 6666 6563 7469 7665 2061 6674 6572  #Effective after
-00000e90: 2061 7070 6c69 6361 7469 6f6e 2072 6573   application res
-00000ea0: 7461 7274 0700 0000 0644 6961 6c6f 6701  tart.....Dialog.
-00000eb0: 03ff ffff ff08 0000 0000 0600 0000 0645  ...............E
-00000ec0: 7870 6f72 7407 0000 0006 4469 616c 6f67  xport.....Dialog
-00000ed0: 0103 0000 0034 0045 0078 0070 006f 0072  .....4.E.x.p.o.r
-00000ee0: 0074 0069 0065 0072 0065 0020 0043 0042  .t.i.e.r.e. .C.B
-00000ef0: 002d 0051 0053 004f 0073 0020 0069 006e  .-.Q.S.O.s. .i.n
-00000f00: 0020 0041 0044 0049 0046 0800 0000 0006  . .A.D.I.F......
-00000f10: 0000 0016 4578 706f 7274 2043 4220 5153  ....Export CB QS
-00000f20: 4f73 2074 6f20 4144 4946 0700 0000 0644  Os to ADIF.....D
-00000f30: 6961 6c6f 6701 0300 0000 3600 4500 7800  ialog.....6.E.x.
-00000f40: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
-00000f50: 2000 6e00 7500 7200 2000 6e00 6500 7500   .n.u.r. .n.e.u.
-00000f60: 6500 7300 7400 6500 2000 5100 5300 4f00  e.s.t.e. .Q.S.O.
-00000f70: 7308 0000 0000 0600 0000 1745 7870 6f72  s..........Expor
-00000f80: 7420 6f6e 6c79 2072 6563 656e 7420 5153  t only recent QS
-00000f90: 4f73 0700 0000 0644 6961 6c6f 6701 0300  Os.....Dialog...
-00000fa0: 0000 4200 4500 7800 7000 6f00 7200 7400  ..B.E.x.p.o.r.t.
-00000fb0: 6900 6500 7200 6500 2000 6500 6900 6700  i.e.r.e. .e.i.g.
-00000fc0: 6500 6e00 6500 2000 4e00 6f00 7400 6900  e.n.e. .N.o.t.i.
-00000fd0: 7a00 6500 6e00 2000 6900 6e00 2000 4100  z.e.n. .i.n. .A.
-00000fe0: 4400 4900 4608 0000 0000 0600 0000 1845  D.I.F..........E
-00000ff0: 7870 6f72 7420 6f77 6e20 6e6f 7465 7320  xport own notes 
-00001000: 746f 2041 4449 4607 0000 0006 4469 616c  to ADIF.....Dial
-00001010: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
-00001020: 000e 4861 6d6c 6962 2072 6967 6374 6c64  ..Hamlib rigctld
-00001030: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-00001040: ff08 0000 0000 0600 0000 0d49 6d70 6f72  ...........Impor
-00001050: 742f 4578 706f 7274 0700 0000 0644 6961  t/Export.....Dia
-00001060: 6c6f 6701 0300 0000 1a00 5300 6300 6800  log.......S.c.h.
-00001070: 6e00 6900 7400 7400 7300 7400 6500 6c00  n.i.t.t.s.t.e.l.
-00001080: 6c00 6508 0000 0000 0600 0000 0949 6e74  l.e..........Int
-00001090: 6572 6661 6365 0700 0000 0644 6961 6c6f  erface.....Dialo
-000010a0: 6701 0300 0000 2000 6c00 6500 7400 7a00  g..... .l.e.t.z.
-000010b0: 7400 6500 7300 2000 4800 6100 6c00 6200  t.e.s. .H.a.l.b.
-000010c0: 6a00 6100 6800 7208 0000 0000 0600 0000  j.a.h.r.........
-000010d0: 0e4c 6173 7420 6861 6c66 2079 6561 7207  .Last half year.
-000010e0: 0000 0006 4469 616c 6f67 0103 0000 001a  ....Dialog......
-000010f0: 006c 0065 0074 007a 0074 0065 006e 0020  .l.e.t.z.t.e.n. 
-00001100: 004d 006f 006e 0061 0074 0800 0000 0006  .M.o.n.a.t......
-00001110: 0000 000a 4c61 7374 206d 6f6e 7468 0700  ....Last month..
-00001120: 0000 0644 6961 6c6f 6701 0300 0000 1800  ...Dialog.......
-00001130: 6c00 6500 7400 7a00 7400 6500 2000 5700  l.e.t.z.t.e. .W.
-00001140: 6f00 6300 6800 6508 0000 0000 0600 0000  o.c.h.e.........
-00001150: 094c 6173 7420 7765 656b 0700 0000 0644  .Last week.....D
-00001160: 6961 6c6f 6701 0300 0000 1800 6c00 6500  ialog.......l.e.
-00001170: 7400 7a00 7400 6500 7300 2000 4a00 6100  t.z.t.e.s. .J.a.
-00001180: 6800 7208 0000 0000 0600 0000 094c 6173  h.r..........Las
-00001190: 7420 7965 6172 0700 0000 0644 6961 6c6f  t year.....Dialo
-000011a0: 6701 0300 0000 0c00 4200 7200 6500 6900  g.......B.r.e.i.
-000011b0: 7400 6508 0000 0000 0600 0000 034c 6174  t.e..........Lat
-000011c0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-000011d0: 0a00 5300 7400 7500 6600 6508 0000 0000  ..S.t.u.f.e.....
-000011e0: 0600 0000 054c 6576 656c 0700 0000 0644  .....Level.....D
-000011f0: 6961 6c6f 6701 03ff ffff ff08 0000 0000  ialog...........
-00001200: 0600 0000 044c 6f54 5707 0000 0006 4469  .....LoTW.....Di
-00001210: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
-00001220: 0000 0007 4c6f 6361 746f 7207 0000 0006  ....Locator.....
-00001230: 4469 616c 6f67 0103 0000 002c 004c 006f  Dialog.....,.L.o
-00001240: 0067 0020 0069 006e 0020 0044 0061 0074  .g. .i.n. .D.a.t
-00001250: 0065 0069 0020 0073 0063 0068 0072 0065  .e.i. .s.c.h.r.e
-00001260: 0069 0062 0065 006e 0800 0000 0006 0000  .i.b.e.n........
-00001270: 000b 4c6f 6720 746f 2066 696c 6507 0000  ..Log to file...
-00001280: 0006 4469 616c 6f67 0103 0000 001e 004c  ..Dialog.......L
-00001290: 006f 0067 0067 0069 006e 0067 002d 0041  .o.g.g.i.n.g.-.A
-000012a0: 0075 0073 0067 0061 0062 0065 0800 0000  .u.s.g.a.b.e....
-000012b0: 0006 0000 000e 4c6f 6767 696e 6720 6f75  ......Logging ou
-000012c0: 7470 7574 0700 0000 0644 6961 6c6f 6701  tput.....Dialog.
-000012d0: 0300 0000 0a00 4c00 e400 6e00 6700 6508  ......L...n.g.e.
-000012e0: 0000 0000 0600 0000 034c 6f6e 0700 0000  .........Lon....
-000012f0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
-00001300: 0000 0600 0000 044e 616d 6507 0000 0006  .......Name.....
-00001310: 4469 616c 6f67 0103 0000 005e 0043 0042  Dialog.....^.C.B
-00001320: 0020 0051 0053 004f 0073 0020 0077 0065  . .Q.S.O.s. .w.e
-00001330: 0072 0064 0065 006e 0020 0062 0065 0069  .r.d.e.n. .b.e.i
-00001340: 006d 0020 0049 006d 0070 006f 0072 0074  .m. .I.m.p.o.r.t
-00001350: 0020 0069 006d 006d 0065 0072 0020 0062  . .i.m.m.e.r. .b
-00001360: 0065 0072 00fc 0063 006b 0073 0069 0063  .e.r...c.k.s.i.c
-00001370: 0068 0074 0069 0067 0074 0800 0000 0006  .h.t.i.g.t......
-00001380: 0000 0028 4f6e 2069 6d70 6f72 7420 4342  ...(On import CB
-00001390: 2051 534f 7320 7769 6c6c 2061 6c77 6179   QSOs will alway
-000013a0: 7320 6265 2068 616e 646c 6564 0700 0000  s be handled....
-000013b0: 0644 6961 6c6f 6701 0300 0000 1000 5000  .Dialog.......P.
-000013c0: 6100 7300 7300 7700 6f00 7200 7408 0000  a.s.s.w.o.r.t...
-000013d0: 0000 0600 0000 0850 6173 7377 6f72 6407  .......Password.
-000013e0: 0000 0006 4469 616c 6f67 0103 0000 0070  ....Dialog.....p
-000013f0: 0050 0061 0073 0073 0077 006f 0072 0074  .P.a.s.s.w.o.r.t
-00001400: 0020 0064 0065 0073 0020 004c 006f 0054  . .d.e.s. .L.o.T
-00001410: 0057 002d 004f 006e 006c 0069 006e 0065  .W.-.O.n.l.i.n.e
-00001420: 002d 0041 0063 0063 006f 0075 006e 0074  .-.A.c.c.o.u.n.t
-00001430: 0073 002c 0020 006e 0069 0063 0068 0074  .s.,. .n.i.c.h.t
-00001440: 0020 0064 0065 0073 0020 005a 0065 0072  . .d.e.s. .Z.e.r
-00001450: 0074 0069 0066 0069 006b 0061 0074 0073  .t.i.f.i.k.a.t.s
-00001460: 0800 0000 0006 0000 0038 5061 7373 776f  .........8Passwo
-00001470: 7264 2066 6f72 204c 6f54 5720 6f6e 6c69  rd for LoTW onli
-00001480: 6e65 2061 6363 6f75 6e74 206e 6f74 2066  ne account not f
-00001490: 6f72 2074 6865 2063 6572 7469 6669 6361  or the certifica
-000014a0: 7465 0700 0000 0644 6961 6c6f 6701 03ff  te.....Dialog...
-000014b0: ffff ff08 0000 0000 0600 0000 0351 5448  .............QTH
-000014c0: 0700 0000 0644 6961 6c6f 6701 03ff ffff  .....Dialog.....
-000014d0: ff08 0000 0000 0600 0000 0552 6164 696f  ...........Radio
-000014e0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
-000014f0: 1800 4e00 6500 7500 6500 7300 7400 6500  ..N.e.u.e.s.t.e.
-00001500: 2000 5100 5300 4f00 7308 0000 0000 0600   .Q.S.O.s.......
-00001510: 0000 0b52 6563 656e 7420 5153 4f73 0700  ...Recent QSOs..
-00001520: 0000 0644 6961 6c6f 6701 0300 0000 1200  ...Dialog.......
-00001530: 4600 7500 6e00 6b00 6700 6500 7200 e400  F.u.n.k.g.e.r...
-00001540: 7408 0000 0000 0600 0000 0352 6967 0700  t..........Rig..
-00001550: 0000 0644 6961 6c6f 6701 0300 0000 4c00  ...Dialog.....L.
-00001560: 5300 6900 6500 6800 6500 2000 4500 6900  S.i.e.h.e. .E.i.
-00001570: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
-00001580: 6700 6500 6e00 2000 5200 6500 6900 7400  g.e.n. .R.e.i.t.
-00001590: 6500 7200 2000 2200 4100 6e00 7700 6500  e.r. .".A.n.w.e.
-000015a0: 6e00 6400 7500 6e00 6700 2208 0000 0000  n.d.u.n.g.".....
-000015b0: 0600 0000 2253 6565 2073 6574 7469 6e67  ...."See setting
-000015c0: 7320 7061 6765 2022 5573 6572 2069 6e74  s page "User int
-000015d0: 6572 6661 6365 2207 0000 0006 4469 616c  erface".....Dial
-000015e0: 6f67 0103 0000 0034 0043 0042 002d 0042  og.....4.C.B.-.B
-000015f0: 0061 006e 0064 0020 0061 0075 0074 006f  .a.n.d. .a.u.t.o
-00001600: 006d 0061 0074 0069 0073 0063 0068 0020  .m.a.t.i.s.c.h. 
-00001610: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
-00001620: 0006 0000 0019 5365 6c65 6374 2043 4220  ......Select CB 
-00001630: 6261 6e64 2062 7920 6465 6661 756c 7407  band by default.
-00001640: 0000 0006 4469 616c 6f67 0103 0000 000c  ....Dialog......
-00001650: 0044 0069 0065 006e 0073 0074 0800 0000  .D.i.e.n.s.t....
-00001660: 0006 0000 0007 5365 7276 6963 6507 0000  ......Service...
-00001670: 0006 4469 616c 6f67 0103 0000 001a 0053  ..Dialog.......S
-00001680: 0065 0074 007a 0065 0020 004c 006f 0063  .e.t.z.e. .L.o.c
-00001690: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-000016a0: 000b 5365 7420 6c6f 6361 746f 7207 0000  ..Set locator...
-000016b0: 0006 4469 616c 6f67 0103 0000 001a 0045  ..Dialog.......E
-000016c0: 0069 006e 0073 0074 0065 006c 006c 0075  .i.n.s.t.e.l.l.u
-000016d0: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
-000016e0: 0008 5365 7474 696e 6773 0700 0000 0644  ..Settings.....D
-000016f0: 6961 6c6f 6701 0300 0000 1c00 5a00 6500  ialog.......Z.e.
-00001700: 6900 6700 6500 2000 5100 5300 4f00 7300  i.g.e. .Q.S.O.s.
-00001710: 2000 6600 fc00 7208 0000 0000 0600 0000   .f...r.........
-00001720: 0e53 686f 7720 5153 4f73 2066 726f 6d07  .Show QSOs from.
-00001730: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
-00001740: 007a 0065 0069 0067 0065 0020 0061 006c  .z.e.i.g.e. .a.l
-00001750: 006c 0065 0800 0000 0006 0000 0008 5368  .l.e..........Sh
-00001760: 6f77 2061 6c6c 0700 0000 0644 6961 6c6f  ow all.....Dialo
-00001770: 6701 0300 0000 4000 5300 7000 6100 6c00  g.....@.S.p.a.l.
-00001780: 7400 6500 6e00 2000 6100 6e00 7a00 6500  t.e.n. .a.n.z.e.
-00001790: 6900 6700 6500 6e00 2000 6f00 6400 6500  i.g.e.n. .o.d.e.
-000017a0: 7200 2000 7600 6500 7200 7300 7400 6500  r. .v.e.r.s.t.e.
-000017b0: 6300 6b00 6500 6e08 0000 0000 0600 0000  c.k.e.n.........
-000017c0: 1453 686f 7720 6f72 2068 6964 6520 636f  .Show or hide co
-000017d0: 6c75 6d6e 7307 0000 0006 4469 616c 6f67  lumns.....Dialog
-000017e0: 0103 0000 0028 0053 006f 0072 0074 0069  .....(.S.o.r.t.i
-000017f0: 0065 0072 0065 0020 006e 0061 0063 0068  .e.r.e. .n.a.c.h
-00001800: 0020 0053 0070 0061 006c 0074 0065 0800  . .S.p.a.l.t.e..
-00001810: 0000 0006 0000 000e 536f 7274 206f 6e20  ........Sort on 
-00001820: 636f 6c75 6d6e 0700 0000 0644 6961 6c6f  column.....Dialo
-00001830: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001840: 0553 7461 7274 0700 0000 0644 6961 6c6f  .Start.....Dialo
-00001850: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001860: 0753 7461 7469 6f6e 0700 0000 0644 6961  .Station.....Dia
-00001870: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00001880: 0000 0454 5153 4c07 0000 0006 4469 616c  ...TQSL.....Dial
-00001890: 6f67 0103 0000 0064 0056 0065 0072 0077  og.....d.V.e.r.w
-000018a0: 0065 006e 0064 0065 0020 0064 0069 0065  .e.n.d.e. .d.i.e
-000018b0: 0020 006b 006f 006e 0066 0069 0067 0075  . .k.o.n.f.i.g.u
-000018c0: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
-000018d0: 0044 0020 0062 0065 0069 0020 0066 0065  .D. .b.e.i. .f.e
-000018e0: 0068 006c 0065 006e 0064 0065 006e 0020  .h.l.e.n.d.e.n. 
-000018f0: 0057 0065 0072 0074 0065 006e 0800 0000  .W.e.r.t.e.n....
-00001900: 0006 0000 0024 5573 6520 636f 6e66 6967  .....$Use config
-00001910: 7572 6564 2049 4420 666f 7220 6d69 7373  ured ID for miss
-00001920: 696e 6720 7661 6c75 6573 0700 0000 0644  ing values.....D
-00001930: 6961 6c6f 6701 0300 0000 6e00 5600 6500  ialog.....n.V.e.
-00001940: 7200 7700 6500 6e00 6400 6500 2000 6400  r.w.e.n.d.e. .d.
-00001950: 6900 6500 2000 6b00 6f00 6e00 6600 6900  i.e. .k.o.n.f.i.
-00001960: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
-00001970: 2000 5300 7400 6100 7400 6900 6f00 6e00   .S.t.a.t.i.o.n.
-00001980: 2000 6200 6500 6900 2000 6600 6500 6800   .b.e.i. .f.e.h.
-00001990: 6c00 6500 6e00 6400 6500 6e00 2000 5700  l.e.n.d.e.n. .W.
-000019a0: 6500 7200 7400 6500 6e08 0000 0000 0600  e.r.t.e.n.......
-000019b0: 0000 2955 7365 2063 6f6e 6669 6775 7265  ..)Use configure
-000019c0: 6420 5374 6174 696f 6e20 666f 7220 6d69  d Station for mi
-000019d0: 7373 696e 6720 7661 6c75 6573 0700 0000  ssing values....
-000019e0: 0644 6961 6c6f 6701 0300 0000 1200 4100  .Dialog.......A.
-000019f0: 6e00 7700 6500 6e00 6400 7500 6e00 6708  n.w.e.n.d.u.n.g.
-00001a00: 0000 0000 0600 0000 0e55 7365 7220 696e  .........User in
-00001a10: 7465 7266 6163 6507 0000 0006 4469 616c  terface.....Dial
-00001a20: 6f67 0103 0000 0018 0042 0065 006e 0075  og.......B.e.n.u
-00001a30: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
-00001a40: 0800 0000 0006 0000 0008 5573 6572 6e61  ..........Userna
-00001a50: 6d65 0700 0000 0644 6961 6c6f 6701 0300  me.....Dialog...
-00001a60: 0000 7800 4200 6500 6e00 7500 7400 7a00  ..x.B.e.n.u.t.z.
-00001a70: 6500 7200 6e00 6100 6d00 6500 2000 6400  e.r.n.a.m.e. .d.
-00001a80: 6500 7300 2000 4c00 6f00 5400 5700 2d00  e.s. .L.o.T.W.-.
-00001a90: 4f00 6e00 6c00 6900 6e00 6500 2d00 4100  O.n.l.i.n.e.-.A.
-00001aa0: 6300 6300 6f00 7500 6e00 7400 7300 2c00  c.c.o.u.n.t.s.,.
-00001ab0: 2000 6e00 6900 6300 6800 7400 2000 6400   .n.i.c.h.t. .d.
-00001ac0: 6500 7300 2000 5a00 6500 7200 7400 6900  e.s. .Z.e.r.t.i.
-00001ad0: 6600 6900 6b00 6100 7400 7308 0000 0000  f.i.k.a.t.s.....
-00001ae0: 0600 0000 3855 7365 726e 616d 6520 666f  ....8Username fo
-00001af0: 7220 4c6f 5457 206f 6e6c 696e 6520 6163  r LoTW online ac
-00001b00: 636f 756e 7420 6e6f 7420 666f 7220 7468  count not for th
-00001b10: 6520 6365 7274 6966 6963 6174 6507 0000  e certificate...
-00001b20: 0006 4469 616c 6f67 0103 0000 0020 0044  ..Dialog..... .D
-00001b30: 0061 0074 0065 0069 00fc 0062 0065 0072  .a.t.e.i...b.e.r
-00001b40: 0077 0061 0063 0068 0075 006e 0067 0800  .w.a.c.h.u.n.g..
-00001b50: 0000 0006 0000 000a 5761 7463 6820 4669  ........Watch Fi
-00001b60: 6c65 0700 0000 0644 6961 6c6f 6701 03ff  le.....Dialog...
-00001b70: ffff ff08 0000 0000 0600 0000 0465 5153  .............eQS
-00001b80: 4c07 0000 0006 4469 616c 6f67 0103 ffff  L.....Dialog....
-00001b90: ffff 0800 0000 0006 0000 0002 c2b0 0700  ................
-00001ba0: 0000 0644 6961 6c6f 6701 0300 0000 9e00  ...Dialog.......
-00001bb0: 4500 6900 6e00 2000 4400 6100 7400 6500  E.i.n. .D.a.t.e.
-00001bc0: 6e00 6200 6100 6e00 6b00 2d00 4200 6100  n.b.a.n.k.-.B.a.
-00001bd0: 6300 6b00 7500 7000 2000 6b00 6f00 6e00  c.k.u.p. .k.o.n.
-00001be0: 6e00 7400 6500 2000 6e00 6900 6300 6800  n.t.e. .n.i.c.h.
-00001bf0: 7400 2000 6500 7200 7300 7400 6500 6c00  t. .e.r.s.t.e.l.
-00001c00: 6c00 7400 2000 7700 6500 7200 6400 6500  l.t. .w.e.r.d.e.
-00001c10: 6e00 2e00 0a00 4400 6900 6500 2000 4400  n.....D.i.e. .D.
-00001c20: 6100 7400 6500 6900 2000 6500 7800 6900  a.t.e.i. .e.x.i.
-00001c30: 7300 7400 6900 6500 7200 7400 2000 6200  s.t.i.e.r.t. .b.
-00001c40: 6500 7200 6500 6900 7400 7300 2e08 0000  e.r.e.i.t.s.....
-00001c50: 0000 0600 0000 4041 2064 6174 6162 6173  ......@A databas
-00001c60: 6520 6261 636b 7570 2063 6f75 6c64 206e  e backup could n
-00001c70: 6f74 2062 6520 6372 6561 7465 642e 0a54  ot be created..T
-00001c80: 6865 2066 696c 6520 616c 7265 6164 7920  he file already 
-00001c90: 6578 6973 7473 2e07 0000 0009 4472 6167  exists......Drag
-00001ca0: 6f6e 4c6f 6701 0300 0000 4e00 4500 6900  onLog.....N.E.i.
-00001cb0: 6e00 2000 4100 4400 4900 4600 2d00 4600  n. .A.D.I.F.-.F.
-00001cc0: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
-00001cd0: 7400 2000 6600 fc00 7200 2000 6400 6500  t. .f...r. .d.e.
-00001ce0: 6e00 2000 4c00 6f00 5400 5700 2d00 5500  n. .L.o.T.W.-.U.
-00001cf0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
-00001d00: 0000 1d41 2066 6965 6c64 2069 7320 6d69  ...A field is mi
-00001d10: 7373 696e 6720 666f 7220 7570 6c6f 6164  ssing for upload
-00001d20: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001d30: ffff ffff 0800 0000 0006 0000 0015 4144  ..............AD
-00001d40: 4946 2033 2028 2a2e 6164 6920 2a2e 6164  IF 3 (*.adi *.ad
-00001d50: 6966 2907 0000 0009 4472 6167 6f6e 4c6f  if).....DragonLo
-00001d60: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00001d70: 1b41 4449 4620 3320 282a 2e61 6478 202a  .ADIF 3 (*.adx *
-00001d80: 2e61 6469 202a 2e61 6469 6629 0700 0000  .adi *.adif)....
-00001d90: 0944 7261 676f 6e4c 6f67 0103 0000 0008  .DragonLog......
-00001da0: 00dc 0062 0065 0072 0800 0000 0006 0000  ...b.e.r........
-00001db0: 0005 4162 6f75 7407 0000 0009 4472 6167  ..About.....Drag
-00001dc0: 6f6e 4c6f 6701 0300 0000 0e00 dc00 6200  onLog.........b.
-00001dd0: 6500 7200 2000 5100 7408 0000 0000 0600  e.r. .Q.t.......
-00001de0: 0000 0841 626f 7574 2051 7407 0000 0009  ...About Qt.....
-00001df0: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
-00001e00: 4100 6900 7200 6300 7200 6100 6600 7400  A.i.r.c.r.a.f.t.
-00001e10: 2d00 5300 6300 6100 7400 7400 6500 7208  -.S.c.a.t.t.e.r.
-00001e20: 0000 0000 0600 0000 1041 6972 6372 6166  .........Aircraf
-00001e30: 7420 5363 6174 7465 7207 0000 0009 4472  t Scatter.....Dr
-00001e40: 6167 6f6e 4c6f 6701 0300 0000 0e00 4100  agonLog.......A.
-00001e50: 6e00 7400 6500 6e00 6e00 6508 0000 0000  n.t.e.n.n.e.....
-00001e60: 0600 0000 0741 6e74 656e 6e61 0700 0000  .....Antenna....
-00001e70: 0944 7261 676f 6e4c 6f67 0103 ffff ffff  .DragonLog......
-00001e80: 0800 0000 0006 0000 0006 4175 726f 7261  ..........Aurora
-00001e90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00001ea0: ffff ffff 0800 0000 0006 0000 0008 4175  ..............Au
-00001eb0: 726f 7261 2d45 0700 0000 0944 7261 676f  rora-E.....Drago
-00001ec0: 6e4c 6f67 0103 0000 000a 0041 0075 0074  nLog.......A.u.t
-00001ed0: 006f 0072 0800 0000 0006 0000 0006 4175  .o.r..........Au
-00001ee0: 7468 6f72 0700 0000 0944 7261 676f 6e4c  thor.....DragonL
-00001ef0: 6f67 0103 0000 0018 0042 0061 0063 006b  og.......B.a.c.k
-00001f00: 002d 0053 0063 0061 0074 0074 0065 0072  .-.S.c.a.t.t.e.r
-00001f10: 0800 0000 0006 0000 000c 4261 636b 2073  ..........Back s
-00001f20: 6361 7474 6572 0700 0000 0944 7261 676f  catter.....Drago
-00001f30: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-00001f40: 0000 0004 4261 6e64 0700 0000 0944 7261  ....Band.....Dra
-00001f50: 676f 6e4c 6f67 0103 0000 0022 0043 0053  gonLog.....".C.S
-00001f60: 0056 002d 0044 0061 0074 0065 0069 0020  .V.-.D.a.t.e.i. 
-00001f70: 0028 002a 002e 0063 0073 0076 0029 0800  .(.*...c.s.v.)..
-00001f80: 0000 0006 0000 0010 4353 562d 4669 6c65  ........CSV-File
-00001f90: 2028 2a2e 6373 7629 0700 0000 0944 7261   (*.csv).....Dra
-00001fa0: 676f 6e4c 6f67 0103 0000 0014 0052 0075  gonLog.......R.u
-00001fb0: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
-00001fc0: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
-00001fd0: 6967 6e07 0000 0009 4472 6167 6f6e 4c6f  ign.....DragonLo
-00001fe0: 6701 0300 0000 0a00 4b00 6100 6e00 6100  g.......K.a.n.a.
-00001ff0: 6c08 0000 0000 0600 0000 0743 6861 6e6e  l..........Chann
-00002000: 656c 0700 0000 0944 7261 676f 6e4c 6f67  el.....DragonLog
-00002010: 0103 0000 0074 0050 0072 00fc 0066 0075  .....t.P.r...f.u
-00002020: 006e 0067 0020 0064 0065 0072 0020 0044  .n.g. .d.e.r. .D
-00002030: 0061 0074 0065 006e 0062 0061 006e 006b  .a.t.e.n.b.a.n.k
-00002040: 0020 0066 0065 0068 006c 0067 0065 0073  . .f.e.h.l.g.e.s
-00002050: 0063 0068 006c 0061 0067 0065 006e 002e  .c.h.l.a.g.e.n..
-00002060: 0020 0049 006e 0068 0061 006c 0074 0020  . .I.n.h.a.l.t. 
-00002070: 006e 0069 0063 0068 0074 0020 006c 0065  .n.i.c.h.t. .l.e
-00002080: 0073 0062 0061 0072 002e 0800 0000 0006  .s.b.a.r........
-00002090: 0000 0034 4368 6563 6b69 6e67 2064 6174  ...4Checking dat
-000020a0: 6162 6173 6520 6661 696c 6564 2e20 436f  abase failed. Co
-000020b0: 6e74 656e 7420 6973 206e 6f74 2061 6363  ntent is not acc
-000020c0: 6573 7361 626c 652e 0700 0000 0944 7261  essable......Dra
-000020d0: 676f 6e4c 6f67 0103 0000 0012 004b 006f  gonLog.......K.o
-000020e0: 006d 006d 0065 006e 0074 0061 0072 0800  .m.m.e.n.t.a.r..
-000020f0: 0000 0006 0000 0007 436f 6d6d 656e 7407  ........Comment.
-00002100: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00002110: 0000 6000 5600 6500 7200 6200 6900 6e00  ..`.V.e.r.b.i.n.
-00002120: 6400 7500 6e00 6700 7300 6600 6500 6800  d.u.n.g.s.f.e.h.
-00002130: 6c00 6500 7200 2000 6f00 6400 6500 7200  l.e.r. .o.d.e.r.
-00002140: 2000 4e00 6500 7400 7a00 7700 6500 7200   .N.e.t.z.w.e.r.
-00002150: 6b00 2000 6e00 6900 6300 6800 7400 2000  k. .n.i.c.h.t. .
-00002160: 6500 7200 7200 6500 6900 6300 6800 6200  e.r.r.e.i.c.h.b.
-00002170: 6100 7208 0000 0000 0600 0000 2743 6f6e  a.r.........'Con
-00002180: 6e65 6374 696f 6e20 6572 726f 7220 6f72  nection error or
-00002190: 206e 6574 776f 726b 2075 6e72 6561 6368   network unreach
-000021a0: 6162 6c65 0700 0000 0944 7261 676f 6e4c  able.....DragonL
-000021b0: 6f67 0103 0000 002e 0044 0061 0074 0065  og.......D.a.t.e
-000021c0: 006e 0062 0061 006e 006b 002d 0042 0061  .n.b.a.n.k.-.B.a
-000021d0: 0063 006b 0075 0070 0020 0046 0065 0068  .c.k.u.p. .F.e.h
-000021e0: 006c 0065 0072 0800 0000 0006 0000 0015  .l.e.r..........
-000021f0: 4461 7461 6261 7365 2062 6163 6b75 7020  Database backup 
-00002200: 6572 726f 7207 0000 0009 4472 6167 6f6e  error.....Dragon
-00002210: 4c6f 6701 0300 0000 2c00 4400 6100 7400  Log.....,.D.a.t.
-00002220: 6500 6e00 6200 6100 6e00 6b00 6b00 6f00  e.n.b.a.n.k.k.o.
-00002230: 6e00 7600 6500 7200 7400 6900 6500 7200  n.v.e.r.t.i.e.r.
-00002240: 7500 6e00 6708 0000 0000 0600 0000 1344  u.n.g..........D
-00002250: 6174 6162 6173 6520 636f 6e76 6572 7369  atabase conversi
-00002260: 6f6e 0700 0000 0944 7261 676f 6e4c 6f67  on.....DragonLog
-00002270: 0103 0000 0048 0044 0061 0074 0065 006e  .....H.D.a.t.e.n
-00002280: 0062 0061 006e 006b 006b 006f 006e 0076  .b.a.n.k.k.o.n.v
-00002290: 0065 0072 0074 0069 0065 0072 0075 006e  .e.r.t.i.e.r.u.n
-000022a0: 0067 0020 0061 0062 0067 0065 0073 0063  .g. .a.b.g.e.s.c
-000022b0: 0068 006c 006f 0073 0073 0065 006e 0800  .h.l.o.s.s.e.n..
-000022c0: 0000 0006 0000 001c 4461 7461 6261 7365  ........Database
-000022d0: 2063 6f6e 7665 7273 696f 6e20 6669 6e69   conversion fini
-000022e0: 7368 6564 0700 0000 0944 7261 676f 6e4c  shed.....DragonL
-000022f0: 6f67 0103 0000 001e 0044 0061 0074 0065  og.......D.a.t.e
-00002300: 006e 0062 0061 006e 006b 0066 0065 0068  .n.b.a.n.k.f.e.h
-00002310: 006c 0065 0072 0800 0000 0006 0000 000e  .l.e.r..........
-00002320: 4461 7461 6261 7365 2065 7272 6f72 0700  Database error..
-00002330: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002340: 0034 0044 0061 0074 0065 006e 0062 0061  .4.D.a.t.e.n.b.a
-00002350: 006e 006b 0073 0074 0072 0075 006b 0074  .n.k.s.t.r.u.k.t
-00002360: 0075 0072 0020 0076 0065 0072 0061 006c  .u.r. .v.e.r.a.l
-00002370: 0074 0065 0074 0800 0000 0006 0000 001c  .t.e.t..........
-00002380: 4461 7461 6261 7365 2073 7472 7563 7475  Database structu
-00002390: 7265 206f 7574 2d64 6174 6564 0700 0000  re out-dated....
-000023a0: 0944 7261 676f 6e4c 6f67 0103 0000 001e  .DragonLog......
-000023b0: 0044 0061 0074 0075 006d 002f 005a 0065  .D.a.t.u.m./.Z.e
-000023c0: 0069 0074 0020 0045 006e 0064 0065 0800  .i.t. .E.n.d.e..
-000023d0: 0000 0006 0000 000d 4461 7465 2f54 696d  ........Date/Tim
-000023e0: 6520 656e 6407 0000 0009 4472 6167 6f6e  e end.....Dragon
-000023f0: 4c6f 6701 0300 0000 2000 4400 6100 7400  Log..... .D.a.t.
-00002400: 7500 6d00 2f00 5a00 6500 6900 7400 2000  u.m./.Z.e.i.t. .
-00002410: 5300 7400 6100 7200 7408 0000 0000 0600  S.t.a.r.t.......
-00002420: 0000 0f44 6174 652f 5469 6d65 2073 7461  ...Date/Time sta
-00002430: 7274 0700 0000 0944 7261 676f 6e4c 6f67  rt.....DragonLog
-00002440: 0103 0000 0016 0051 0053 004f 0020 006c  .......Q.S.O. .l
-00002450: 00f6 0073 0063 0068 0065 006e 0800 0000  ...s.c.h.e.n....
-00002460: 0006 0000 000a 4465 6c65 7465 2051 534f  ......Delete QSO
-00002470: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002480: 0000 0014 0045 006e 0074 0066 0065 0072  .....E.n.t.f.e.r
-00002490: 006e 0075 006e 0067 0800 0000 0006 0000  .n.u.n.g........
-000024a0: 0008 4469 7374 616e 6365 0700 0000 0944  ..Distance.....D
-000024b0: 7261 676f 6e4c 6f67 0103 0000 0064 0057  ragonLog.....d.W
-000024c0: 006f 006c 006c 0065 006e 0020 0073 0069  .o.l.l.e.n. .s.i
-000024d0: 0065 0020 0064 0069 0065 0020 0073 0065  .e. .d.i.e. .s.e
-000024e0: 006c 0065 006b 0074 0069 0065 0072 0074  .l.e.k.t.i.e.r.t
-000024f0: 0065 006e 0020 0051 0053 004f 0073 0020  .e.n. .Q.S.O.s. 
-00002500: 0077 0069 0072 006b 006c 0069 0063 0068  .w.i.r.k.l.i.c.h
-00002510: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
-00002520: 003f 0800 0000 0006 0000 0031 446f 2079  .?.........1Do y
-00002530: 6f75 2072 6561 6c6c 7920 7761 6e74 2074  ou really want t
-00002540: 6f20 6465 6c65 7465 2074 6865 2073 656c  o delete the sel
-00002550: 6563 7465 6420 5153 4f28 7329 3f07 0000  ected QSO(s)?...
-00002560: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
-00002570: ff08 0000 0000 0600 0000 1045 6172 7468  ...........Earth
-00002580: 2d4d 6f6f 6e2d 4561 7274 6807 0000 0009  -Moon-Earth.....
-00002590: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-000025a0: 0000 0000 0600 0000 0845 6368 6f4c 696e  .........EchoLin
-000025b0: 6b07 0000 0009 4472 6167 6f6e 4c6f 6701  k.....DragonLog.
-000025c0: 0300 0000 0c00 4600 6500 6800 6c00 6500  ......F.e.h.l.e.
-000025d0: 7208 0000 0000 0600 0000 0545 7272 6f72  r..........Error
-000025e0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-000025f0: 0000 0028 0045 0078 0063 0065 006c 002d  ...(.E.x.c.e.l.-
-00002600: 0044 0061 0074 0065 0069 0020 0028 002a  .D.a.t.e.i. .(.*
-00002610: 002e 0078 006c 0073 0078 0029 0800 0000  ...x.l.s.x.)....
-00002620: 0006 0000 0013 4578 6365 6c2d 4669 6c65  ......Excel-File
-00002630: 2028 2a2e 786c 7378 2907 0000 0009 4472   (*.xlsx).....Dr
-00002640: 6167 6f6e 4c6f 6701 0300 0000 2400 4500  agonLog.....$.E.
-00002650: 7800 7000 6f00 7200 7400 6900 6500 7200  x.p.o.r.t.i.e.r.
-00002660: 6500 2000 5100 5300 4f00 2000 6c00 6f00  e. .Q.S.O. .l.o.
-00002670: 6708 0000 0000 0600 0000 1045 7870 6f72  g..........Expor
-00002680: 7465 6420 5153 4f20 6c6f 6707 0000 0009  ted QSO log.....
-00002690: 4472 6167 6f6e 4c6f 6701 0300 0000 1a00  DragonLog.......
-000026a0: 4600 3200 2d00 5200 6500 6600 6c00 6500  F.2.-.R.e.f.l.e.
-000026b0: 6b00 7400 6900 6f00 6e08 0000 0000 0600  k.t.i.o.n.......
-000026c0: 0000 0d46 3220 5265 666c 6563 7469 6f6e  ...F2 Reflection
-000026d0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-000026e0: 0000 0038 0046 0069 0065 006c 0064 002d  ...8.F.i.e.l.d.-
-000026f0: 0041 006c 0069 0067 006e 0065 0064 002d  .A.l.i.g.n.e.d.-
-00002700: 0049 0072 0072 0065 0067 0075 006c 0061  .I.r.r.e.g.u.l.a
-00002710: 0072 0069 0074 0069 0065 0073 0800 0000  .r.i.t.i.e.s....
-00002720: 0006 0000 001c 4669 656c 6420 416c 6967  ......Field Alig
-00002730: 6e65 6420 4972 7265 6775 6c61 7269 7469  ned Irregulariti
-00002740: 6573 0700 0000 0944 7261 676f 6e4c 6f67  es.....DragonLog
-00002750: 0103 0000 0010 0046 0072 0065 0071 0075  .......F.r.e.q.u
-00002760: 0065 006e 007a 0800 0000 0006 0000 0009  .e.n.z..........
-00002770: 4672 6571 7565 6e63 7907 0000 0009 4472  Frequency.....Dr
-00002780: 6167 6f6e 4c6f 6701 0300 0000 1400 4200  agonLog.......B.
-00002790: 6f00 6400 6500 6e00 7700 6500 6c00 6c00  o.d.e.n.w.e.l.l.
-000027a0: 6508 0000 0000 0600 0000 0b47 726f 756e  e..........Groun
-000027b0: 6420 5761 7665 0700 0000 0944 7261 676f  d Wave.....Drago
-000027c0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-000027d0: 0000 0006 4861 6d51 5448 0700 0000 0944  ....HamQTH.....D
-000027e0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
-000027f0: 0000 0006 0000 0006 4861 6d6c 6962 0700  ........Hamlib..
-00002800: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002810: 000a 0048 0069 006c 0066 0065 0800 0000  ...H.i.l.f.e....
-00002820: 0006 0000 0004 4865 6c70 0700 0000 0944  ......Help.....D
-00002830: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
-00002840: 0000 0006 0000 0004 4952 4c50 0700 0000  ........IRLP....
-00002850: 0944 7261 676f 6e4c 6f67 0103 0000 0026  .DragonLog.....&
-00002860: 0049 006e 0074 0065 0072 006e 0065 0074  .I.n.t.e.r.n.e.t
-00002870: 0075 006e 0074 0065 0072 0073 0074 00fc  .u.n.t.e.r.s.t..
-00002880: 0074 007a 0074 0800 0000 0006 0000 0011  .t.z.t..........
-00002890: 496e 7465 726e 6574 2d61 7373 6973 7465  Internet-assiste
-000028a0: 6407 0000 0009 4472 6167 6f6e 4c6f 6701  d.....DragonLog.
-000028b0: 0300 0000 1800 4900 6f00 6e00 6f00 2d00  ......I.o.n.o.-.
-000028c0: 5300 6300 6100 7400 7400 6500 7208 0000  S.c.a.t.t.e.r...
-000028d0: 0000 0600 0000 0b49 6f6e 6f73 6361 7474  .......Ionoscatt
-000028e0: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
-000028f0: 0103 0000 0020 006c 0065 0074 007a 0074  ..... .l.e.t.z.t
-00002900: 0065 0073 0020 0048 0061 006c 0062 006a  .e.s. .H.a.l.b.j
-00002910: 0061 0068 0072 0800 0000 0006 0000 000e  .a.h.r..........
-00002920: 4c61 7374 2068 616c 6620 7965 6172 0700  Last half year..
-00002930: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002940: 001a 006c 0065 0074 007a 0074 0065 006e  ...l.e.t.z.t.e.n
-00002950: 0020 004d 006f 006e 0061 0074 0800 0000  . .M.o.n.a.t....
-00002960: 0006 0000 000a 4c61 7374 206d 6f6e 7468  ......Last month
-00002970: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002980: 0000 0018 006c 0065 0074 007a 0074 0065  .....l.e.t.z.t.e
-00002990: 0020 0057 006f 0063 0068 0065 0800 0000  . .W.o.c.h.e....
-000029a0: 0006 0000 0009 4c61 7374 2077 6565 6b07  ......Last week.
-000029b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-000029c0: 0000 1800 6c00 6500 7400 7a00 7400 6500  ....l.e.t.z.t.e.
-000029d0: 7300 2000 4a00 6100 6800 7208 0000 0000  s. .J.a.h.r.....
-000029e0: 0600 0000 094c 6173 7420 7965 6172 0700  .....Last year..
-000029f0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00002a00: 001e 0053 0069 0063 0068 0074 0076 0065  ...S.i.c.h.t.v.e
-00002a10: 0072 0062 0069 006e 0064 0075 006e 0067  .r.b.i.n.d.u.n.g
-00002a20: 0800 0000 0006 0000 000d 4c69 6e65 206f  ..........Line o
-00002a30: 6620 5369 6768 7407 0000 0009 4472 6167  f Sight.....Drag
-00002a40: 6f6e 4c6f 6701 0300 0000 2000 4c00 6f00  onLog..... .L.o.
-00002a50: 5400 5700 2d00 4100 4400 4900 4600 2d00  T.W.-.A.D.I.F.-.
-00002a60: 5500 7000 6c00 6f00 6100 6408 0000 0000  U.p.l.o.a.d.....
-00002a70: 0600 0000 104c 6f54 5720 4144 4946 2075  .....LoTW ADIF u
-00002a80: 706c 6f61 6407 0000 0009 4472 6167 6f6e  pload.....Dragon
-00002a90: 4c6f 6701 0300 0000 1400 4c00 6f00 5400  Log.......L.o.T.
-00002aa0: 5700 2000 6500 6d00 7000 6600 2e08 0000  W. .e.m.p.f.....
-00002ab0: 0000 0600 0000 094c 6f54 5720 7263 7664  .......LoTW rcvd
-00002ac0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002ad0: 0000 0014 004c 006f 0054 0057 0020 0076  .....L.o.T.W. .v
-00002ae0: 0065 0072 0073 002e 0800 0000 0006 0000  .e.r.s..........
-00002af0: 0009 4c6f 5457 2073 656e 7407 0000 0009  ..LoTW sent.....
-00002b00: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00002b10: 0000 0000 0600 0000 074c 6f63 6174 6f72  .........Locator
-00002b20: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002b30: ffff ffff 0800 0000 0006 0000 000f 4c6f  ..............Lo
-00002b40: 6720 696d 706f 7274 2041 4449 4607 0000  g import ADIF...
-00002b50: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002b60: 1c00 4c00 6f00 6700 2000 4900 6d00 7000  ..L.o.g. .I.m.p.
-00002b70: 6f00 7200 7400 2000 4300 5300 5608 0000  o.r.t. .C.S.V...
-00002b80: 0000 0600 0000 0e4c 6f67 2069 6d70 6f72  .......Log impor
-00002b90: 7420 4353 5607 0000 0009 4472 6167 6f6e  t CSV.....Dragon
-00002ba0: 4c6f 6701 0300 0000 2000 4c00 6f00 6700  Log..... .L.o.g.
-00002bb0: 2000 4900 6d00 7000 6f00 7200 7400 2000   .I.m.p.o.r.t. .
-00002bc0: 4500 7800 6300 6500 6c08 0000 0000 0600  E.x.c.e.l.......
-00002bd0: 0000 104c 6f67 2069 6d70 6f72 7420 4578  ...Log import Ex
-00002be0: 6365 6c07 0000 0009 4472 6167 6f6e 4c6f  cel.....DragonLo
-00002bf0: 6701 0300 0000 1c00 4d00 6500 7400 6500  g.......M.e.t.e.
-00002c00: 6f00 7200 2d00 5300 6300 6100 7400 7400  o.r.-.S.c.a.t.t.
-00002c10: 6500 7208 0000 0000 0600 0000 0e4d 6574  e.r..........Met
-00002c20: 656f 7220 7363 6174 7465 7207 0000 0009  eor scatter.....
-00002c30: 4472 6167 6f6e 4c6f 6701 0300 0000 5a00  DragonLog.....Z.
-00002c40: 4b00 6500 6900 6e00 6500 2000 5300 7400  K.e.i.n.e. .S.t.
-00002c50: 6100 7400 6900 6f00 6e00 7300 6b00 6f00  a.t.i.o.n.s.k.o.
-00002c60: 6e00 6600 6900 6700 7500 7200 6100 7400  n.f.i.g.u.r.a.t.
-00002c70: 6900 6f00 6e00 2000 6900 6e00 2000 5400  i.o.n. .i.n. .T.
-00002c80: 5100 5300 4c00 2000 7600 6500 7200 6600  Q.S.L. .v.e.r.f.
-00002c90: fc00 6700 6200 6100 7208 0000 0000 0600  ..g.b.a.r.......
-00002ca0: 0000 254d 6973 7369 6e67 2073 7461 7469  ..%Missing stati
-00002cb0: 6f6e 2063 6f6e 6669 6775 7261 7469 6f6e  on configuration
-00002cc0: 2069 6e20 5451 534c 0700 0000 0944 7261   in TQSL.....Dra
-00002cd0: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
-00002ce0: 0006 0000 0004 4d6f 6465 0700 0000 0944  ......Mode.....D
-00002cf0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
-00002d00: 0000 0006 0000 0004 4e61 6d65 0700 0000  ........Name....
-00002d10: 0944 7261 676f 6e4c 6f67 0103 0000 0034  .DragonLog.....4
-00002d20: 004b 0065 0069 006e 0065 0020 0051 0053  .K.e.i.n.e. .Q.S
-00002d30: 004f 0073 0020 0066 00fc 0072 0020 0064  .O.s. .f...r. .d
-00002d40: 0065 006e 0020 004c 006f 0063 0061 0074  .e.n. .L.o.c.a.t
-00002d50: 006f 0072 0800 0000 0006 0000 0017 4e6f  .o.r..........No
-00002d60: 2072 6563 6f72 6473 2066 6f72 206c 6f63   records for loc
-00002d70: 6174 696f 6e07 0000 0009 4472 6167 6f6e  ation.....Dragon
-00002d80: 4c6f 6701 0300 0000 0e00 4e00 6f00 7400  Log.......N.o.t.
-00002d90: 6900 7a00 6500 6e08 0000 0000 0600 0000  i.z.e.n.........
-00002da0: 054e 6f74 6573 0700 0000 0944 7261 676f  .Notes.....Drago
-00002db0: 6e4c 6f67 0103 ffff ffff 0800 0000 0006  nLog............
-00002dc0: 0000 0002 4f6b 0700 0000 0944 7261 676f  ....Ok.....Drago
-00002dd0: 6e4c 6f67 0103 0000 001e 0045 0069 0067  nLog.......E.i.g
-00002de0: 0065 006e 0065 0072 0020 004c 006f 0063  .e.n.e.r. .L.o.c
-00002df0: 0061 0074 006f 0072 0800 0000 0006 0000  .a.t.o.r........
-00002e00: 000b 4f77 6e20 4c6f 6361 746f 7207 0000  ..Own Locator...
-00002e10: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-00002e20: 1800 4500 6900 6700 6500 6e00 6500 7200  ..E.i.g.e.n.e.r.
-00002e30: 2000 4e00 6100 6d00 6508 0000 0000 0600   .N.a.m.e.......
-00002e40: 0000 084f 776e 204e 616d 6507 0000 0009  ...Own Name.....
-00002e50: 4472 6167 6f6e 4c6f 6701 0300 0000 1600  DragonLog.......
-00002e60: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
-00002e70: 5100 5400 4808 0000 0000 0600 0000 074f  Q.T.H..........O
-00002e80: 776e 2051 5448 0700 0000 0944 7261 676f  wn QTH.....Drago
-00002e90: 6e4c 6f67 0103 0000 0024 0045 0069 0067  nLog.....$.E.i.g
-00002ea0: 0065 006e 0065 0073 0020 0052 0075 0066  .e.n.e.s. .R.u.f
-00002eb0: 007a 0065 0069 0063 0068 0065 006e 0800  .z.e.i.c.h.e.n..
-00002ec0: 0000 0006 0000 000d 4f77 6e20 6361 6c6c  ........Own call
-00002ed0: 2073 6967 6e07 0000 0009 4472 6167 6f6e   sign.....Dragon
-00002ee0: 4c6f 6701 0300 0000 1000 4c00 6500 6900  Log.......L.e.i.
-00002ef0: 7300 7400 7500 6e00 6708 0000 0000 0600  s.t.u.n.g.......
-00002f00: 0000 0550 6f77 6572 0700 0000 0944 7261  ...Power.....Dra
-00002f10: 676f 6e4c 6f67 0103 0000 0016 0041 0075  gonLog.......A.u
-00002f20: 0073 0062 0072 0065 0069 0074 0075 006e  .s.b.r.e.i.t.u.n
-00002f30: 0067 0800 0000 0006 0000 000b 5072 6f70  .g..........Prop
-00002f40: 6167 6174 696f 6e07 0000 0009 4472 6167  agation.....Drag
-00002f50: 6f6e 4c6f 6701 0300 0000 1a00 5100 5300  onLog.......Q.S.
-00002f60: 4c00 2d00 4e00 6100 6300 6800 7200 6900  L.-.N.a.c.h.r.i.
-00002f70: 6300 6800 7408 0000 0000 0600 0000 0b51  c.h.t..........Q
-00002f80: 534c 206d 6573 7361 6765 0700 0000 0944  SL message.....D
-00002f90: 7261 676f 6e4c 6f67 0103 0000 0010 0051  ragonLog.......Q
-00002fa0: 0053 004c 002d 0050 0066 0061 0064 0800  .S.L.-.P.f.a.d..
-00002fb0: 0000 0006 0000 0008 5153 4c20 7061 7468  ........QSL path
-00002fc0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00002fd0: 0000 0012 0051 0053 004c 0020 0065 006d  .....Q.S.L. .e.m
-00002fe0: 0070 0066 002e 0800 0000 0006 0000 0008  .p.f............
-00002ff0: 5153 4c20 7263 7664 0700 0000 0944 7261  QSL rcvd.....Dra
-00003000: 676f 6e4c 6f67 0103 0000 0012 0051 0053  gonLog.......Q.S
-00003010: 004c 0020 0076 0065 0072 0073 002e 0800  .L. .v.e.r.s....
-00003020: 0000 0006 0000 0008 5153 4c20 7365 6e74  ........QSL sent
-00003030: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003040: 0000 000e 0051 0053 004c 002d 0056 0069  .....Q.S.L.-.V.i
-00003050: 0061 0800 0000 0006 0000 0007 5153 4c20  .a..........QSL 
-00003060: 7669 6107 0000 0009 4472 6167 6f6e 4c6f  via.....DragonLo
-00003070: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
-00003080: 0351 534f 0700 0000 0944 7261 676f 6e4c  .QSO.....DragonL
-00003090: 6f67 0103 0000 0048 0051 0053 004f 002d  og.....H.Q.S.O.-
-000030a0: 004c 006f 0067 0020 0028 002a 002e 0071  .L.o.g. .(.*...q
-000030b0: 006c 006f 0067 0029 003b 003b 0041 006c  .l.o.g.).;.;.A.l
-000030c0: 006c 0065 0020 0044 0061 0074 0065 0069  .l.e. .D.a.t.e.i
-000030d0: 0065 006e 0020 0028 002a 002e 002a 0029  .e.n. .(.*...*.)
-000030e0: 0800 0000 0006 0000 0021 5153 4f2d 4c6f  .........!QSO-Lo
-000030f0: 6720 282a 2e71 6c6f 6729 3b3b 416c 6c20  g (*.qlog);;All 
-00003100: 4669 6c65 7320 282a 2e2a 2907 0000 0009  Files (*.*).....
-00003110: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
-00003120: 0000 0000 0600 0000 0351 5448 0700 0000  .........QTH....
-00003130: 0944 7261 676f 6e4c 6f67 0103 0000 0012  .DragonLog......
-00003140: 0052 0053 0054 0020 0065 006d 0070 0066  .R.S.T. .e.m.p.f
-00003150: 002e 0800 0000 0006 0000 0008 5253 5420  ............RST 
-00003160: 7263 7664 0700 0000 0944 7261 676f 6e4c  rcvd.....DragonL
-00003170: 6f67 0103 0000 0010 0052 0053 0054 0020  og.......R.S.T. 
-00003180: 0067 0065 0073 002e 0800 0000 0006 0000  .g.e.s..........
-00003190: 0008 5253 5420 7365 6e74 0700 0000 0944  ..RST sent.....D
-000031a0: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
-000031b0: 0000 0006 0000 0005 5261 6469 6f07 0000  ........Radio...
-000031c0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000031d0: 1800 5200 6100 6900 6e00 2d00 5300 6300  ..R.a.i.n.-.S.c.
-000031e0: 6100 7400 7400 6500 7208 0000 0000 0600  a.t.t.e.r.......
-000031f0: 0000 0c52 6169 6e20 7363 6174 7465 7207  ...Rain scatter.
-00003200: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00003210: 0000 3200 5200 6500 7000 6500 6100 7400  ..2.R.e.p.e.a.t.
-00003220: 6500 7200 2000 6f00 6400 6500 7200 2000  e.r. .o.d.e.r. .
-00003230: 5400 7200 6100 6e00 7300 7000 6f00 6e00  T.r.a.n.s.p.o.n.
-00003240: 6400 6500 7208 0000 0000 0600 0000 1752  d.e.r..........R
-00003250: 6570 6561 7465 7220 6f72 2054 7261 6e73  epeater or Trans
-00003260: 706f 6e64 6572 0700 0000 0944 7261 676f  ponder.....Drago
-00003270: 6e4c 6f67 0103 0000 0010 0053 0061 0074  nLog.......S.a.t
-00003280: 0065 006c 006c 0069 0074 0800 0000 0006  .e.l.l.i.t......
-00003290: 0000 0009 5361 7465 6c6c 6974 6507 0000  ....Satellite...
-000032a0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
-000032b0: 2a00 4500 7800 7000 6f00 7200 7400 6400  *.E.x.p.o.r.t.d.
-000032c0: 6100 7400 6500 6900 2000 7300 7000 6500  a.t.e.i. .s.p.e.
-000032d0: 6900 6300 6800 6500 7200 6e08 0000 0000  i.c.h.e.r.n.....
-000032e0: 0600 0000 1253 656c 6563 7420 6578 706f  .....Select expo
-000032f0: 7274 2066 696c 6507 0000 0009 4472 6167  rt file.....Drag
-00003300: 6f6e 4c6f 6701 0300 0000 2000 4400 6100  onLog..... .D.a.
-00003310: 7400 6500 6e00 6200 6100 6e00 6b00 2000  t.e.n.b.a.n.k. .
-00003320: f600 6600 6600 6e00 6500 6e08 0000 0000  ..f.f.n.e.n.....
-00003330: 0600 0000 0b53 656c 6563 7420 6669 6c65  .....Select file
-00003340: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003350: 0000 0038 005a 0075 0020 00fc 0062 0065  ...8.Z.u. ...b.e
-00003360: 0072 0077 0061 0063 0068 0065 006e 0064  .r.w.a.c.h.e.n.d
-00003370: 0065 0020 0044 0061 0074 0065 0069 0020  .e. .D.a.t.e.i. 
-00003380: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
-00003390: 0006 0000 0014 5365 6c65 6374 2066 696c  ......Select fil
-000033a0: 6520 746f 2077 6174 6368 0700 0000 0944  e to watch.....D
-000033b0: 7261 676f 6e4c 6f67 0103 0000 0024 0049  ragonLog.....$.I
-000033c0: 006d 0070 006f 0072 0074 0064 0061 0074  .m.p.o.r.t.d.a.t
-000033d0: 0065 0069 0020 00f6 0066 0066 006e 0065  .e.i. ...f.f.n.e
-000033e0: 006e 0800 0000 0006 0000 0012 5365 6c65  .n..........Sele
-000033f0: 6374 2069 6d70 6f72 7420 6669 6c65 0700  ct import file..
-00003400: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
-00003410: 001a 0057 00e4 0068 006c 0065 0020 0053  ...W...h.l.e. .S
-00003420: 0074 0061 0074 0069 006f 006e 0800 0000  .t.a.t.i.o.n....
-00003430: 0006 0000 000e 5365 6c65 6374 2073 7461  ......Select sta
-00003440: 7469 6f6e 0700 0000 0944 7261 676f 6e4c  tion.....DragonL
-00003450: 6f67 0103 0000 0044 004c 006f 0054 0057  og.....D.L.o.T.W
-00003460: 002d 0053 0065 0072 0076 0065 0072 0020  .-.S.e.r.v.e.r. 
-00003470: 0068 0061 0074 0020 0064 0061 0073 0020  .h.a.t. .d.a.s. 
-00003480: 004c 006f 0067 0020 0061 0062 0067 0065  .L.o.g. .a.b.g.e
-00003490: 0077 0069 0065 0073 0065 006e 0800 0000  .w.i.e.s.e.n....
-000034a0: 0006 0000 0013 5365 7276 6572 2072 656a  ......Server rej
-000034b0: 6563 7465 6420 6c6f 6707 0000 0009 4472  ected log.....Dr
-000034c0: 6167 6f6e 4c6f 6701 0300 0000 1400 7a00  agonLog.......z.
-000034d0: 6500 6900 6700 6500 2000 6100 6c00 6c00  e.i.g.e. .a.l.l.
-000034e0: 6508 0000 0000 0600 0000 0853 686f 7720  e..........Show 
-000034f0: 616c 6c07 0000 0009 4472 6167 6f6e 4c6f  all.....DragonLo
-00003500: 6701 0300 0000 1400 5300 7000 6f00 7200  g.......S.p.o.r.
-00003510: 6100 6400 6900 6300 2d00 4508 0000 0000  a.d.i.c.-.E.....
-00003520: 0600 0000 0a53 706f 7261 6469 6320 4507  .....Sporadic E.
-00003530: 0000 0009 4472 6167 6f6e 4c6f 6701 03ff  ....DragonLog...
-00003540: ffff ff08 0000 0000 0600 0000 0753 7562  .............Sub
-00003550: 6d6f 6465 0700 0000 0944 7261 676f 6e4c  mode.....DragonL
-00003560: 6f67 0103 0000 002a 0054 0051 0053 004c  og.....*.T.Q.S.L
-00003570: 002d 0053 0069 0067 006e 0061 0074 0075  .-.S.i.g.n.a.t.u
-00003580: 0072 0070 0061 0073 0073 0077 006f 0072  .r.p.a.s.s.w.o.r
-00003590: 0074 0800 0000 0006 0000 0017 5451 534c  .t..........TQSL
-000035a0: 2073 6967 6e61 7475 7265 2070 6173 7377   signature passw
-000035b0: 6f72 6407 0000 0009 4472 6167 6f6e 4c6f  ord.....DragonLo
-000035c0: 6701 0300 0000 b200 4400 6900 6500 2000  g.......D.i.e. .
-000035d0: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
-000035e0: 6b00 7300 7400 7200 7500 6b00 7400 7500  k.s.t.r.u.k.t.u.
-000035f0: 7200 2000 6900 7300 7400 2000 7600 6500  r. .i.s.t. .v.e.
-00003600: 7200 6100 6c00 7400 6500 7400 2000 7500  r.a.l.t.e.t. .u.
-00003610: 6e00 6400 2000 6d00 7500 7300 7300 2000  n.d. .m.u.s.s. .
-00003620: 6b00 6f00 6e00 7600 6500 7200 7400 6900  k.o.n.v.e.r.t.i.
-00003630: 6500 7200 7400 2000 7700 6500 7200 6400  e.r.t. .w.e.r.d.
-00003640: 6500 6e00 0a00 0a00 4500 6900 6e00 2000  e.n.....E.i.n. .
-00003650: 4200 6100 6300 6b00 7500 7000 2000 7700  B.a.c.k.u.p. .w.
-00003660: 6900 7200 6400 2000 6500 7200 7300 7400  i.r.d. .e.r.s.t.
-00003670: 6500 6c00 6c00 7400 3a08 0000 0000 0600  e.l.l.t.:.......
-00003680: 0000 5754 6865 2064 6174 6162 6173 6520  ..WThe database 
-00003690: 7374 7275 6374 7572 6520 6973 206f 7574  structure is out
-000036a0: 2d64 6174 6564 2061 6e64 206e 6565 6473  -dated and needs
-000036b0: 2061 2063 6f6e 7665 7273 696f 6e0a 0a41   a conversion..A
-000036c0: 2062 6163 6b75 7020 7769 6c6c 2062 6520   backup will be 
-000036d0: 6765 6e65 7261 7465 643a 0700 0000 0944  generated:.....D
-000036e0: 7261 676f 6e4c 6f67 0103 0000 001e 0054  ragonLog.......T
-000036f0: 0072 0061 006e 0073 0065 0071 0075 0061  .r.a.n.s.e.q.u.a
-00003700: 0074 006f 0072 0069 0061 006c 0800 0000  .t.o.r.i.a.l....
-00003710: 0006 0000 0010 5472 616e 732d 6571 7561  ......Trans-equa
-00003720: 746f 7269 616c 0700 0000 0944 7261 676f  torial.....Drago
-00003730: 6e4c 6f67 0103 0000 0028 0054 0072 006f  nLog.....(.T.r.o
-00003740: 0070 006f 0073 0070 0068 0065 0072 0069  .p.o.s.p.h.e.r.i
-00003750: 0063 002d 0044 0075 0063 0074 0069 006e  .c.-.D.u.c.t.i.n
-00003760: 0067 0800 0000 0006 0000 0014 5472 6f70  .g..........Trop
-00003770: 6f73 7068 6572 6963 2064 7563 7469 6e67  ospheric ducting
-00003780: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
-00003790: ffff ffff 0800 0000 0006 0000 0007 5665  ..............Ve
-000037a0: 7273 696f 6e07 0000 0009 4472 6167 6f6e  rsion.....Dragon
-000037b0: 4c6f 6701 0300 0000 2c00 5000 7200 6f00  Log.....,.P.r.o.
-000037c0: 6700 7200 6100 6d00 6d00 6c00 6f00 6700  g.r.a.m.m.l.o.g.
-000037d0: 2000 fc00 6200 6500 7200 7700 6100 6300   ...b.e.r.w.a.c.
-000037e0: 6800 6500 6e08 0000 0000 0600 0000 1557  h.e.n..........W
-000037f0: 6174 6368 2061 7070 6c69 6361 7469 6f6e  atch application
-00003800: 206c 6f67 0700 0000 0944 7261 676f 6e4c   log.....DragonL
-00003810: 6f67 0103 0000 0020 0044 0061 0074 0065  og..... .D.a.t.e
-00003820: 0069 00fc 0062 0065 0072 0077 0061 0063  .i...b.e.r.w.a.c
-00003830: 0068 0075 006e 0067 0800 0000 0006 0000  .h.u.n.g........
-00003840: 000d 5761 7463 6869 6e67 2066 696c 6507  ..Watching file.
-00003850: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
-00003860: 0000 1400 6500 5100 5300 4c00 2000 6500  ....e.Q.S.L. .e.
-00003870: 6d00 7000 6600 2e08 0000 0000 0600 0000  m.p.f...........
-00003880: 0965 5153 4c20 7263 7664 0700 0000 0944  .eQSL rcvd.....D
-00003890: 7261 676f 6e4c 6f67 0103 0000 0014 0065  ragonLog.......e
-000038a0: 0051 0053 004c 0020 0076 0065 0072 0073  .Q.S.L. .v.e.r.s
-000038b0: 002e 0800 0000 0006 0000 0009 6551 534c  ............eQSL
-000038c0: 2073 656e 7407 0000 0009 4472 6167 6f6e   sent.....Dragon
-000038d0: 4c6f 6701 0300 0000 0e00 6900 6e00 6100  Log.......i.n.a.
-000038e0: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
-000038f0: 0769 6e61 6374 6976 0700 0000 0944 7261  .inactiv.....Dra
-00003900: 676f 6e4c 6f67 0103 0000 0008 00dc 0062  gonLog.........b
-00003910: 0065 0072 0800 0000 0006 0000 0005 4162  .e.r..........Ab
-00003920: 6f75 7407 0000 000a 4d61 696e 5769 6e64  out.....MainWind
-00003930: 6f77 0103 0000 000e 00dc 0062 0065 0072  ow.........b.e.r
-00003940: 0020 0051 0074 0800 0000 0006 0000 0008  . .Q.t..........
-00003950: 4162 6f75 7420 5174 0700 0000 0a4d 6169  About Qt.....Mai
-00003960: 6e57 696e 646f 7701 0300 0000 1a00 4100  nWindow.......A.
-00003970: 6e00 7700 6500 6e00 6400 7500 6e00 6700  n.w.e.n.d.u.n.g.
-00003980: 7300 6c00 6f00 6708 0000 0000 0600 0000  s.l.o.g.........
-00003990: 0f41 7070 6c69 6361 7469 6f6e 204c 6f67  .Application Log
-000039a0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-000039b0: 0300 0000 2200 4500 6900 6e00 7400 7200  ....".E.i.n.t.r.
-000039c0: 6100 6700 2000 e400 6e00 6400 6500 7200  a.g. ...n.d.e.r.
-000039d0: 6e00 2e00 2e00 2e08 0000 0000 0600 0000  n...............
-000039e0: 1343 6861 6e67 6520 6c6f 6720 656e 7472  .Change log entr
-000039f0: 792e 2e2e 0700 0000 0a4d 6169 6e57 696e  y........MainWin
-00003a00: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
-00003a10: 0000 0643 7472 6c2b 4507 0000 000a 4d61  ...Ctrl+E.....Ma
-00003a20: 696e 5769 6e64 6f77 0103 ffff ffff 0800  inWindow........
-00003a30: 0000 0006 0000 0006 4374 726c 2b4c 0700  ........Ctrl+L..
-00003a40: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
-00003a50: ffff ff08 0000 0000 0600 0000 0643 7472  .............Ctr
-00003a60: 6c2b 5107 0000 000a 4d61 696e 5769 6e64  l+Q.....MainWind
-00003a70: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
-00003a80: 0006 4374 726c 2b57 0700 0000 0a4d 6169  ..Ctrl+W.....Mai
-00003a90: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
-00003aa0: 0000 0600 0000 0643 7472 6c2b 5807 0000  .......Ctrl+X...
-00003ab0: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-00003ac0: 001e 0045 0069 006e 0074 0072 0061 0067  ...E.i.n.t.r.a.g
-00003ad0: 0020 006c 00f6 0073 0063 0068 0065 006e  . .l...s.c.h.e.n
-00003ae0: 0800 0000 0006 0000 0010 4465 6c65 7465  ..........Delete
-00003af0: 206c 6f67 2065 6e74 7279 0700 0000 0a4d   log entry.....M
-00003b00: 6169 6e57 696e 646f 7701 03ff ffff ff08  ainWindow.......
-00003b10: 0000 0000 0600 0000 0944 7261 676f 6e4c  .........DragonL
-00003b20: 6f67 0700 0000 0a4d 6169 6e57 696e 646f  og.....MainWindo
-00003b30: 7701 0300 0000 1400 4200 6500 6100 7200  w.......B.e.a.r.
-00003b40: 6200 6500 6900 7400 6500 6e08 0000 0000  b.e.i.t.e.n.....
-00003b50: 0600 0000 0445 6469 7407 0000 000a 4d61  .....Edit.....Ma
-00003b60: 696e 5769 6e64 6f77 0103 0000 000e 0042  inWindow.......B
-00003b70: 0065 0065 006e 0064 0065 006e 0800 0000  .e.e.n.d.e.n....
-00003b80: 0006 0000 0004 4578 6974 0700 0000 0a4d  ......Exit.....M
-00003b90: 6169 6e57 696e 646f 7701 03ff ffff ff08  ainWindow.......
-00003ba0: 0000 0000 0600 0000 0645 7870 6f72 7407  .........Export.
-00003bb0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
-00003bc0: 0000 001c 0045 0078 0070 006f 0072 0074  .....E.x.p.o.r.t
-00003bd0: 0069 0065 0072 0065 006e 002e 002e 002e  .i.e.r.e.n......
-00003be0: 0800 0000 0006 0000 0009 4578 706f 7274  ..........Export
-00003bf0: 2e2e 2e07 0000 000a 4d61 696e 5769 6e64  ........MainWind
-00003c00: 6f77 0103 0000 000a 0044 0061 0074 0065  ow.......D.a.t.e
-00003c10: 0069 0800 0000 0006 0000 0004 4669 6c65  .i..........File
-00003c20: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003c30: 0300 0000 0a00 4800 6900 6c00 6600 6508  ......H.i.l.f.e.
-00003c40: 0000 0000 0600 0000 0448 656c 7007 0000  .........Help...
-00003c50: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
-00003c60: ffff 0800 0000 0006 0000 0006 496d 706f  ............Impo
-00003c70: 7274 0700 0000 0a4d 6169 6e57 696e 646f  rt.....MainWindo
-00003c80: 7701 0300 0000 1c00 4900 6d00 7000 6f00  w.......I.m.p.o.
-00003c90: 7200 7400 6900 6500 7200 6500 6e00 2e00  r.t.i.e.r.e.n...
-00003ca0: 2e00 2e08 0000 0000 0600 0000 0949 6d70  .............Imp
-00003cb0: 6f72 742e 2e2e 0700 0000 0a4d 6169 6e57  ort........MainW
-00003cc0: 696e 646f 7701 0300 0000 1800 4c00 6f00  indow.......L.o.
-00003cd0: 6700 6700 6500 2000 5100 5300 4f00 2e00  g.g.e. .Q.S.O...
-00003ce0: 2e00 2e08 0000 0000 0600 0000 0a4c 6f67  .............Log
-00003cf0: 2051 534f 2e2e 2e07 0000 000a 4d61 696e   QSO........Main
-00003d00: 5769 6e64 6f77 0103 0000 0018 0051 0053  Window.......Q.S
-00003d10: 004f 002d 0046 006f 0072 006d 0075 006c  .O.-.F.o.r.m.u.l
-00003d20: 0061 0072 0800 0000 0006 0000 0008 5153  .a.r..........QS
-00003d30: 4f20 466f 726d 0700 0000 0a4d 6169 6e57  O Form.....MainW
-00003d40: 696e 646f 7701 0300 0000 2600 4400 6100  indow.....&.D.a.
-00003d50: 7400 6500 6e00 6200 6100 6e00 6b00 2000  t.e.n.b.a.n.k. .
-00003d60: 7700 e400 6800 6c00 6500 6e00 2e00 2e00  w...h.l.e.n.....
-00003d70: 2e08 0000 0000 0600 0000 1253 656c 6563  ...........Selec
-00003d80: 7420 6461 7461 6261 7365 2e2e 2e07 0000  t database......
-00003d90: 000a 4d61 696e 5769 6e64 6f77 0103 0000  ..MainWindow....
-00003da0: 001a 0045 0069 006e 0073 0074 0065 006c  ...E.i.n.s.t.e.l
-00003db0: 006c 0075 006e 0067 0065 006e 0800 0000  .l.u.n.g.e.n....
-00003dc0: 0006 0000 0008 5365 7474 696e 6773 0700  ......Settings..
-00003dd0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
-00003de0: 0000 2600 5a00 6500 6900 6700 6500 2000  ..&.Z.e.i.g.e. .
-00003df0: 4100 6e00 7700 6500 6e00 6400 7500 6e00  A.n.w.e.n.d.u.n.
-00003e00: 6700 7300 6c00 6f00 6708 0000 0000 0600  g.s.l.o.g.......
-00003e10: 0000 0853 686f 7720 6c6f 6707 0000 000a  ...Show log.....
-00003e20: 4d61 696e 5769 6e64 6f77 0103 0000 001a  MainWindow......
-00003e30: 0053 0074 0061 0072 0074 0065 0020 0048  .S.t.a.r.t.e. .H
-00003e40: 0061 006d 006c 0069 0062 0800 0000 0006  .a.m.l.i.b......
-00003e50: 0000 000c 5374 6172 7420 6861 6d6c 6962  ....Start hamlib
-00003e60: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003e70: 0300 0000 1c00 5700 6500 7200 6b00 7a00  ......W.e.r.k.z.
-00003e80: 6500 7500 6700 6c00 6500 6900 7300 7400  e.u.g.l.e.i.s.t.
-00003e90: 6508 0000 0000 0600 0000 0754 6f6f 6c62  e..........Toolb
-00003ea0: 6172 0700 0000 0a4d 6169 6e57 696e 646f  ar.....MainWindo
-00003eb0: 7701 0300 0000 3200 4c00 6f00 6700 7300  w.....2.L.o.g.s.
-00003ec0: 2000 7a00 7500 2000 4c00 6f00 5400 5700   .z.u. .L.o.T.W.
-00003ed0: 2000 6800 6f00 6300 6800 6c00 6100 6400   .h.o.c.h.l.a.d.
-00003ee0: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
-00003ef0: 0000 1655 706c 6f61 6420 6c6f 6773 2074  ...Upload logs t
-00003f00: 6f20 4c6f 5457 2e2e 2e07 0000 000a 4d61  o LoTW........Ma
-00003f10: 696e 5769 6e64 6f77 0103 0000 0042 0044  inWindow.....B.D
-00003f20: 0061 0074 0065 0069 0020 0061 0075 0066  .a.t.e.i. .a.u.f
-00003f30: 0020 006e 0065 0075 0065 0020 0051 0053  . .n.e.u.e. .Q.S
-00003f40: 004f 0073 0020 00fc 0062 0065 0072 0077  .O.s. ...b.e.r.w
-00003f50: 0061 0063 0068 0065 006e 002e 002e 002e  .a.c.h.e.n......
-00003f60: 0800 0000 0006 0000 0016 5761 7463 6820  ..........Watch 
-00003f70: 6669 6c65 2066 6f72 2051 534f 732e 2e2e  file for QSOs...
-00003f80: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
-00003f90: 03ff ffff ff08 0000 0000 0600 0000 0220  ............... 
-00003fa0: 5707 0000 0007 5153 4f46 6f72 6d01 03ff  W.....QSOForm...
-00003fb0: ffff ff08 0000 0000 0600 0000 0420 6b48  ............. kH
-00003fc0: 7a07 0000 0007 5153 4f46 6f72 6d01 03ff  z.....QSOForm...
-00003fd0: ffff ff08 0000 0000 0600 0000 0235 3907  .............59.
-00003fe0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00003ff0: 4800 4500 6900 6e00 2000 4600 6500 6c00  H.E.i.n. .F.e.l.
-00004000: 6400 2000 6600 6500 6800 6c00 7400 2000  d. .f.e.h.l.t. .
-00004010: 6600 fc00 7200 2000 6400 6900 6500 2000  f...r. .d.i.e. .
-00004020: 4900 6e00 6200 6f00 7800 2d00 5000 7200  I.n.b.o.x.-.P.r.
-00004030: fc00 6600 7500 6e00 6708 0000 0000 0600  ..f.u.n.g.......
-00004040: 0000 2241 2066 6965 6c64 2069 7320 6d69  .."A field is mi
-00004050: 7373 696e 6720 666f 7220 696e 626f 7820  ssing for inbox 
-00004060: 6368 6563 6b07 0000 0007 5153 4f46 6f72  check.....QSOFor
-00004070: 6d01 0300 0000 4200 4600 6500 6800 6c00  m.....B.F.e.h.l.
-00004080: 6500 6e00 6400 6500 7300 2000 4600 6500  e.n.d.e.s. .F.e.
-00004090: 6c00 6400 2000 6600 fc00 7200 2000 6400  l.d. .f...r. .d.
-000040a0: 6500 6e00 2000 4c00 6f00 6700 2d00 5500  e.n. .L.o.g.-.U.
-000040b0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
-000040c0: 0000 2141 2066 6965 6c64 2069 7320 6d69  ..!A field is mi
-000040d0: 7373 696e 6720 666f 7220 6c6f 6720 7570  ssing for log up
-000040e0: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
-000040f0: 0103 0000 0056 0046 0065 0068 006c 0065  .....V.F.e.h.l.e
-00004100: 006e 0064 0065 0073 0020 0046 0065 006c  .n.d.e.s. .F.e.l
-00004110: 0064 0020 0066 00fc 0072 0020 0064 0065  .d. .f...r. .d.e
-00004120: 006e 0020 004c 006f 0067 002d 0055 0070  .n. .L.o.g.-.U.p
-00004130: 006c 006f 0061 0064 0020 007a 0075 0020  .l.o.a.d. .z.u. 
-00004140: 0048 0061 006d 0051 0054 0048 0800 0000  .H.a.m.Q.T.H....
-00004150: 0006 0000 002b 4120 6669 656c 6420 6973  .....+A field is
-00004160: 206d 6973 7369 6e67 2066 6f72 206c 6f67   missing for log
-00004170: 2075 706c 6f61 6420 746f 2048 616d 5154   upload to HamQT
-00004180: 4807 0000 0007 5153 4f46 6f72 6d01 0300  H.....QSOForm...
-00004190: 0000 1600 4100 6b00 7a00 6500 7000 7400  ....A.k.z.e.p.t.
-000041a0: 6900 6500 7200 7400 3a08 0000 0000 0600  i.e.r.t.:.......
-000041b0: 0000 0841 6363 6570 7473 3a07 0000 0007  ...Accepts:.....
-000041c0: 5153 4f46 6f72 6d01 0300 0000 6a00 4500  QSOForm.....j.E.
-000041d0: 6900 6e00 2000 4600 6500 6800 6c00 6500  i.n. .F.e.h.l.e.
-000041e0: 7200 2000 7400 7200 6100 7400 2000 7700  r. .t.r.a.t. .w.
-000041f0: e400 6800 7200 6500 6e00 6400 2000 6400  ..h.r.e.n.d. .d.
-00004200: 6500 7200 2000 dc00 6200 6500 7200 7400  e.r. ...b.e.r.t.
-00004210: 7200 6100 6700 7500 6e00 6700 2000 7a00  r.a.g.u.n.g. .z.
-00004220: 7500 2000 4800 6100 6d00 5100 5400 4800  u. .H.a.m.Q.T.H.
-00004230: 2000 6100 7500 6608 0000 0000 0600 0000   .a.u.f.........
-00004240: 2741 6e20 6572 726f 7220 6f63 6375 7265  'An error occure
-00004250: 6420 6f6e 2075 706c 6f61 6469 6e67 2074  d on uploading t
-00004260: 6f20 4861 6d51 5448 0700 0000 0751 534f  o HamQTH.....QSO
-00004270: 466f 726d 0103 0000 000e 0041 006e 0074  Form.......A.n.t
-00004280: 0065 006e 006e 0065 0800 0000 0006 0000  .e.n.n.e........
-00004290: 0007 416e 7465 6e6e 6107 0000 0007 5153  ..Antenna.....QS
-000042a0: 4f46 6f72 6d01 0300 0000 1600 4100 7500  OForm.......A.u.
-000042b0: 7400 6f00 6d00 6100 7400 6900 7300 6300  t.o.m.a.t.i.s.c.
-000042c0: 6808 0000 0000 0600 0000 0d41 7574 6f6d  h..........Autom
-000042d0: 6174 6963 616c 6c79 0700 0000 0751 534f  atically.....QSO
-000042e0: 466f 726d 0103 0000 0038 0046 0065 0068  Form.....8.F.e.h
-000042f0: 006c 0065 0072 0068 0061 0066 0074 0065  .l.e.r.h.a.f.t.e
-00004300: 0073 0020 0041 0062 0066 0072 0061 0067  .s. .A.b.f.r.a.g
-00004310: 0065 0065 0072 0067 0065 0062 006e 0069  .e.e.r.g.e.b.n.i
-00004320: 0073 0800 0000 0006 0000 0012 4261 6420  .s..........Bad 
-00004330: 7265 7175 6573 7420 7265 7375 6c74 0700  request result..
-00004340: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-00004350: 0800 0000 0006 0000 0004 4261 6e64 0700  ..........Band..
-00004360: 0000 0751 534f 466f 726d 0103 0000 0008  ...QSOForm......
-00004370: 0042 00fc 0072 006f 0800 0000 0006 0000  .B...r.o........
-00004380: 0006 4275 7265 6175 0700 0000 0751 534f  ..Bureau.....QSO
-00004390: 466f 726d 0103 0000 0016 0042 00fc 0072  Form.......B...r
-000043a0: 006f 002f 0044 0069 0072 0065 006b 0074  .o./.D.i.r.e.k.t
-000043b0: 0800 0000 0006 0000 000d 4275 7265 6175  ..........Bureau
-000043c0: 2f44 6972 6563 7407 0000 0007 5153 4f46  /Direct.....QSOF
-000043d0: 6f72 6d01 0300 0000 1400 5200 7500 6600  orm.......R.u.f.
-000043e0: 7a00 6500 6900 6300 6800 6500 6e08 0000  z.e.i.c.h.e.n...
-000043f0: 0000 0600 0000 0943 616c 6c20 7369 676e  .......Call sign
-00004400: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004410: 003c 0046 0065 0068 006c 0065 0072 0020  .<.F.e.h.l.e.r. 
-00004420: 0062 0065 0069 0020 0064 0065 0072 0020  .b.e.i. .d.e.r. 
-00004430: 0052 0075 0066 007a 0065 0069 0063 0068  .R.u.f.z.e.i.c.h
-00004440: 0065 006e 0073 0075 0063 0068 0065 0800  .e.n.s.u.c.h.e..
-00004450: 0000 0006 0000 0015 4361 6c6c 626f 6f6b  ........Callbook
-00004460: 2073 6561 7263 6820 6572 726f 7207 0000   search error...
-00004470: 0007 5153 4f46 6f72 6d01 0300 0000 2a00  ..QSOForm.....*.
-00004480: 4300 6100 6c00 6c00 6200 6f00 6f00 6b00  C.a.l.l.b.o.o.k.
-00004490: 2d00 5300 7500 6300 6800 6500 7200 6700  -.S.u.c.h.e.r.g.
-000044a0: 6500 6200 6e00 6900 7308 0000 0000 0600  e.b.n.i.s.......
-000044b0: 0000 1643 616c 6c62 6f6f 6b20 7365 6172  ...Callbook sear
-000044c0: 6368 2072 6573 756c 7407 0000 0007 5153  ch result.....QS
-000044d0: 4f46 6f72 6d01 0300 0000 3200 5200 7500  OForm.....2.R.u.
-000044e0: 6600 7a00 6500 6900 6300 6800 6500 6e00  f.z.e.i.c.h.e.n.
-000044f0: 2000 6e00 6900 6300 6800 7400 2000 6700   .n.i.c.h.t. .g.
-00004500: 6500 6600 7500 6e00 6400 6500 6e08 0000  e.f.u.n.d.e.n...
-00004510: 0000 0600 0000 1243 616c 6c73 6967 6e20  .......Callsign 
-00004520: 6e6f 7420 666f 756e 6407 0000 0007 5153  not found.....QS
-00004530: 4f46 6f72 6d01 0300 0000 0a00 4b00 6100  OForm.......K.a.
-00004540: 6e00 6100 6c08 0000 0000 0600 0000 0743  n.a.l..........C
-00004550: 6861 6e6e 656c 0700 0000 0751 534f 466f  hannel.....QSOFo
-00004560: 726d 0103 0000 0016 0050 0072 00fc 0066  rm.......P.r...f
-00004570: 0065 0020 0049 006e 0062 006f 0078 0800  .e. .I.n.b.o.x..
-00004580: 0000 0006 0000 000b 4368 6563 6b20 496e  ........Check In
-00004590: 626f 7807 0000 0007 5153 4f46 6f72 6d01  box.....QSOForm.
-000045a0: 0300 0000 4200 4600 6500 6800 6c00 6500  ....B.F.e.h.l.e.
-000045b0: 7200 2000 6200 6500 6900 6d00 2000 5000  r. .b.e.i.m. .P.
-000045c0: 7200 fc00 6600 6500 6e00 2000 6400 6500  r...f.e.n. .d.e.
-000045d0: 7200 2000 4c00 6f00 5400 5700 2d00 4900  r. .L.o.T.W.-.I.
-000045e0: 6e00 6200 6f00 7808 0000 0000 0600 0000  n.b.o.x.........
-000045f0: 1643 6865 636b 204c 6f54 5720 496e 626f  .Check LoTW Inbo
-00004600: 7820 6572 726f 7207 0000 0007 5153 4f46  x error.....QSOF
-00004610: 6f72 6d01 0300 0000 1c00 5000 7200 fc00  orm.......P.r...
-00004620: 6600 6500 2000 4c00 6f00 5400 5700 2000  f.e. .L.o.T.W. .
-00004630: 5100 5300 4c08 0000 0000 0600 0000 0e43  Q.S.L..........C
-00004640: 6865 636b 204c 6f54 5720 5153 4c07 0000  heck LoTW QSL...
-00004650: 0007 5153 4f46 6f72 6d01 0300 0000 3800  ..QSOForm.....8.
-00004660: 6500 5100 5300 4c00 2d00 4600 6500 6800  e.Q.S.L.-.F.e.h.
-00004670: 6c00 6500 7200 2000 7000 7200 fc00 6600  l.e.r. .p.r...f.
-00004680: 6500 6e00 2000 6400 6500 7200 2000 4900  e.n. .d.e.r. .I.
-00004690: 6e00 6200 6f00 7808 0000 0000 0600 0000  n.b.o.x.........
-000046a0: 1643 6865 636b 2065 5153 4c20 496e 626f  .Check eQSL Inbo
-000046b0: 7820 6572 726f 7207 0000 0007 5153 4f46  x error.....QSOF
-000046c0: 6f72 6d01 0300 0000 1800 5a00 7500 7200  orm.......Z.u.r.
-000046d0: fc00 6300 6b00 7300 6500 7400 7a00 6500  ..c.k.s.e.t.z.e.
-000046e0: 6e08 0000 0000 0600 0000 0543 6c65 6172  n..........Clear
-000046f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004700: 0020 004b 006f 006e 0066 0069 0067 0075  . .K.o.n.f.i.g.u
-00004710: 0072 0069 0065 0072 0074 0065 0020 0049  .r.i.e.r.t.e. .I
-00004720: 0044 0800 0000 0006 0000 0013 436f 6e66  .D..........Conf
-00004730: 6967 7572 6564 2069 6465 6e74 6974 7907  igured identity.
-00004740: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00004750: 2a00 4b00 6f00 6e00 6600 6900 6700 7500  *.K.o.n.f.i.g.u.
-00004760: 7200 6900 6500 7200 7400 6500 2000 5300  r.i.e.r.t.e. .S.
-00004770: 7400 6100 7400 6900 6f00 6e08 0000 0000  t.a.t.i.o.n.....
-00004780: 0600 0000 1243 6f6e 6669 6775 7265 6420  .....Configured 
-00004790: 7374 6174 696f 6e07 0000 0007 5153 4f46  station.....QSOF
-000047a0: 6f72 6d01 0300 0000 0c00 6400 6900 7200  orm.......d.i.r.
-000047b0: 6500 6b00 7408 0000 0000 0600 0000 0644  e.k.t..........D
-000047c0: 6972 6563 7407 0000 0007 5153 4f46 6f72  irect.....QSOFor
-000047d0: 6d01 0300 0000 1c00 6500 5100 5300 4c00  m.......e.Q.S.L.
-000047e0: 2000 7300 7000 6500 6900 6300 6800 6500   .s.p.e.i.c.h.e.
-000047f0: 7200 6e08 0000 0000 0600 0000 0d44 6f77  r.n..........Dow
-00004800: 6e6c 6f61 6420 6551 534c 0700 0000 0751  nload eQSL.....Q
-00004810: 534f 466f 726d 0103 0000 006c 0057 00e4  SOForm.....l.W..
-00004820: 0068 0072 0065 006e 0064 0020 0064 0065  .h.r.e.n.d. .d.e
-00004830: 0072 0020 0052 0075 0066 007a 0065 0069  .r. .R.u.f.z.e.i
-00004840: 0063 0068 0065 006e 0073 0075 0063 0068  .c.h.e.n.s.u.c.h
-00004850: 0065 0020 0069 0073 0074 0020 0065 0069  .e. .i.s.t. .e.i
-00004860: 006e 0020 0046 0065 0068 006c 0065 0072  .n. .F.e.h.l.e.r
-00004870: 0020 0061 0075 0066 0067 0065 0074 0072  . .a.u.f.g.e.t.r
-00004880: 0065 0074 0065 006e 0800 0000 0006 0000  .e.t.e.n........
-00004890: 0027 4475 7269 6e67 2063 616c 6c62 6f6f  .'During callboo
-000048a0: 6b20 7365 6172 6368 2061 6e20 6572 726f  k search an erro
-000048b0: 7220 6f63 6375 7265 6407 0000 0007 5153  r occured.....QS
-000048c0: 4f46 6f72 6d01 0300 0000 0800 4500 6e00  OForm.......E.n.
-000048d0: 6400 6508 0000 0000 0600 0000 0345 6e64  d.e..........End
-000048e0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-000048f0: 000c 0046 0065 0068 006c 0065 0072 0800  ...F.e.h.l.e.r..
-00004900: 0000 0006 0000 0005 4572 726f 7207 0000  ........Error...
-00004910: 0007 5153 4f46 6f72 6d01 0300 0000 2400  ..QSOForm.....$.
-00004920: 6500 5100 5300 4c00 2d00 5500 7000 6c00  e.Q.S.L.-.U.p.l.
-00004930: 6f00 6100 6400 2d00 4600 6500 6800 6c00  o.a.d.-.F.e.h.l.
-00004940: 6500 7208 0000 0000 0600 0000 0f45 7272  e.r..........Err
-00004950: 6f72 206f 6e20 7570 6c6f 6164 0700 0000  or on upload....
-00004960: 0751 534f 466f 726d 0103 0000 0010 0046  .QSOForm.......F
-00004970: 0072 0065 0071 0075 0065 006e 007a 0800  .r.e.q.u.e.n.z..
-00004980: 0000 0006 0000 0009 4672 6571 7565 6e63  ........Frequenc
-00004990: 7907 0000 0007 5153 4f46 6f72 6d01 03ff  y.....QSOForm...
-000049a0: ffff ff08 0000 0000 0600 0000 0648 616d  .............Ham
-000049b0: 5154 4807 0000 0007 5153 4f46 6f72 6d01  QTH.....QSOForm.
-000049c0: 0300 0000 0400 4900 4408 0000 0000 0600  ......I.D.......
-000049d0: 0000 0849 6465 6e74 6974 7907 0000 0007  ...Identity.....
-000049e0: 5153 4f46 6f72 6d01 0300 0000 2600 4c00  QSOForm.....&.L.
-000049f0: 6900 6e00 6b00 2000 7a00 7500 7200 2000  i.n.k. .z.u.r. .
-00004a00: 6500 5100 5300 4c00 2d00 4b00 6100 7200  e.Q.S.L.-.K.a.r.
-00004a10: 7400 6508 0000 0000 0600 0000 114c 696e  t.e..........Lin
-00004a20: 6b20 746f 2065 5153 4c20 4361 7264 0700  k to eQSL Card..
-00004a30: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-00004a40: 0800 0000 0006 0000 0004 4c6f 5457 0700  ..........LoTW..
-00004a50: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
-00004a60: 004c 006f 0054 0057 0020 0065 006d 0070  .L.o.T.W. .e.m.p
-00004a70: 0066 0061 006e 0067 0065 006e 0800 0000  .f.a.n.g.e.n....
-00004a80: 0006 0000 000d 4c6f 5457 2072 6563 6569  ......LoTW recei
-00004a90: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
-00004aa0: 0300 0000 1c00 4c00 6f00 5400 5700 2000  ......L.o.T.W. .
-00004ab0: 7600 6500 7200 7300 6500 6e00 6400 6500  v.e.r.s.e.n.d.e.
-00004ac0: 7408 0000 0000 0600 0000 094c 6f54 5720  t..........LoTW 
-00004ad0: 7365 6e74 0700 0000 0751 534f 466f 726d  sent.....QSOForm
-00004ae0: 0103 ffff ffff 0800 0000 0006 0000 0007  ................
-00004af0: 4c6f 6361 746f 7207 0000 0007 5153 4f46  Locator.....QSOF
-00004b00: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-00004b10: 0000 074c 6f67 626f 6f6b 0700 0000 0751  ...Logbook.....Q
-00004b20: 534f 466f 726d 0103 0000 0042 004c 006f  SOForm.....B.L.o
-00004b30: 0067 0069 006e 0020 0066 0065 0068 006c  .g.i.n. .f.e.h.l
-00004b40: 0067 0065 0073 0063 0068 006c 0061 0067  .g.e.s.c.h.l.a.g
-00004b50: 0065 006e 0020 0066 00fc 0072 0020 0042  .e.n. .f...r. .B
-00004b60: 0065 006e 0075 0074 007a 0065 0072 0800  .e.n.u.t.z.e.r..
-00004b70: 0000 0006 0000 0015 4c6f 6769 6e20 6661  ........Login fa
-00004b80: 696c 6564 2066 6f72 2075 7365 7207 0000  iled for user...
-00004b90: 0007 5153 4f46 6f72 6d01 0300 0000 5800  ..QSOForm.....X.
-00004ba0: 4c00 6f00 6700 6900 6e00 2000 6200 6500  L.o.g.i.n. .b.e.
-00004bb0: 6900 2000 4800 6100 6d00 5100 5400 4800  i. .H.a.m.Q.T.H.
-00004bc0: 2000 6600 6500 6800 6c00 6700 6500 7300   .f.e.h.l.g.e.s.
-00004bd0: 6300 6800 6c00 6100 6700 6500 6e00 2000  c.h.l.a.g.e.n. .
-00004be0: 6600 fc00 7200 2000 4200 6500 6e00 7500  f...r. .B.e.n.u.
-00004bf0: 7400 7a00 6500 7208 0000 0000 0600 0000  t.z.e.r.........
-00004c00: 1f4c 6f67 696e 2074 6f20 4861 6d51 5448  .Login to HamQTH
-00004c10: 2066 6169 6c65 6420 666f 7220 7573 6572   failed for user
-00004c20: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004c30: 0014 0048 0061 0075 0070 0074 0064 0061  ...H.a.u.p.t.d.a
-00004c40: 0074 0065 006e 0800 0000 0006 0000 0009  .t.e.n..........
-00004c50: 4d61 696e 2064 6174 6107 0000 0007 5153  Main data.....QS
-00004c60: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00004c70: 0600 0000 044d 6f64 6507 0000 0007 5153  .....Mode.....QS
-00004c80: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00004c90: 0600 0000 044e 616d 6507 0000 0007 5153  .....Name.....QS
-00004ca0: 4f46 6f72 6d01 0300 0000 2400 4b00 6500  OForm.....$.K.e.
-00004cb0: 6900 6e00 2000 5100 5300 4c00 2000 7600  i.n. .Q.S.L. .v.
-00004cc0: 6500 7200 6600 fc00 6700 6200 6100 7208  e.r.f...g.b.a.r.
-00004cd0: 0000 0000 0600 0000 104e 6f20 5153 4c20  .........No QSL 
-00004ce0: 6176 6169 6c61 626c 6507 0000 0007 5153  available.....QS
-00004cf0: 4f46 6f72 6d01 0300 0000 2600 4b00 6500  OForm.....&.K.e.
-00004d00: 6900 6e00 2000 6500 5100 5300 4c00 2000  i.n. .e.Q.S.L. .
-00004d10: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
-00004d20: 7208 0000 0000 0600 0000 114e 6f20 6551  r..........No eQ
-00004d30: 534c 2061 7661 696c 6162 6c65 0700 0000  SL available....
-00004d40: 0751 534f 466f 726d 0103 0000 000a 004a  .QSOForm.......J
-00004d50: 0065 0074 007a 0074 0800 0000 0006 0000  .e.t.z.t........
-00004d60: 0003 4e6f 7707 0000 0007 5153 4f46 6f72  ..Now.....QSOFor
-00004d70: 6d01 0300 0000 1600 4500 6900 6700 6500  m.......E.i.g.e.
-00004d80: 6e00 6500 7200 2000 5100 5400 4808 0000  n.e.r. .Q.T.H...
-00004d90: 0000 0600 0000 074f 776e 2051 5448 0700  .......Own QTH..
-00004da0: 0000 0751 534f 466f 726d 0103 0000 0024  ...QSOForm.....$
-00004db0: 0045 0069 0067 0065 006e 0065 0073 0020  .E.i.g.e.n.e.s. 
-00004dc0: 0052 0075 0066 007a 0065 0069 0063 0068  .R.u.f.z.e.i.c.h
-00004dd0: 0065 006e 0800 0000 0006 0000 000d 4f77  .e.n..........Ow
-00004de0: 6e20 6361 6c6c 2073 6967 6e07 0000 0007  n call sign.....
-00004df0: 5153 4f46 6f72 6d01 0300 0000 1e00 4500  QSOForm.......E.
-00004e00: 6900 6700 6500 6e00 6500 7200 2000 4c00  i.g.e.n.e.r. .L.
-00004e10: 6f00 6300 6100 7400 6f00 7208 0000 0000  o.c.a.t.o.r.....
-00004e20: 0600 0000 0b4f 776e 206c 6f63 6174 6f72  .....Own locator
-00004e30: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
-00004e40: 0018 0045 0069 0067 0065 006e 0065 0072  ...E.i.g.e.n.e.r
-00004e50: 0020 004e 0061 006d 0065 0800 0000 0006  . .N.a.m.e......
-00004e60: 0000 0008 4f77 6e20 6e61 6d65 0700 0000  ....Own name....
-00004e70: 0751 534f 466f 726d 0103 0000 001c 0045  .QSOForm.......E
-00004e80: 0069 0067 0065 006e 0065 0020 004e 006f  .i.g.e.n.e. .N.o
-00004e90: 0074 0069 007a 0065 006e 0800 0000 0006  .t.i.z.e.n......
-00004ea0: 0000 0009 4f77 6e20 6e6f 7465 7307 0000  ....Own notes...
-00004eb0: 0007 5153 4f46 6f72 6d01 0300 0000 1000  ..QSOForm.......
-00004ec0: 4c00 6500 6900 7300 7400 7500 6e00 6708  L.e.i.s.t.u.n.g.
-00004ed0: 0000 0000 0600 0000 0550 6f77 6572 0700  .........Power..
-00004ee0: 0000 0751 534f 466f 726d 0103 0000 001e  ...QSOForm......
-00004ef0: 0041 0075 0073 0062 0072 0065 0069 0074  .A.u.s.b.r.e.i.t
-00004f00: 0075 006e 0067 0073 0061 0072 0074 0800  .u.n.g.s.a.r.t..
-00004f10: 0000 0006 0000 000b 5072 6f70 6167 6174  ........Propagat
-00004f20: 696f 6e07 0000 0007 5153 4f46 6f72 6d01  ion.....QSOForm.
-00004f30: 03ff ffff ff08 0000 0000 0600 0000 0551  ...............Q
-00004f40: 525a 4351 0700 0000 0751 534f 466f 726d  RZCQ.....QSOForm
-00004f50: 0103 ffff ffff 0800 0000 0006 0000 0003  ................
-00004f60: 5153 4c07 0000 0007 5153 4f46 6f72 6d01  QSL.....QSOForm.
-00004f70: 0300 0000 2200 5100 5300 4c00 2000 2600  ....".Q.S.L. .&.
-00004f80: 2600 2000 4c00 6f00 6700 2d00 5500 7000  &. .L.o.g.-.U.p.
-00004f90: 6c00 6f00 6100 6408 0000 0000 0600 0000  l.o.a.d.........
-00004fa0: 1151 534c 2026 2620 4c6f 6720 7570 6c6f  .QSL && Log uplo
-00004fb0: 6164 0700 0000 0751 534f 466f 726d 0103  ad.....QSOForm..
-00004fc0: 0000 001c 0051 0053 004c 002d 004b 0061  .....Q.S.L.-.K.a
-00004fd0: 0072 0074 0065 006e 0074 0065 0078 0074  .r.t.e.n.t.e.x.t
-00004fe0: 0800 0000 0006 0000 0010 5153 4c20 6361  ..........QSL ca
-00004ff0: 7264 206d 6573 7361 6765 0700 0000 0751  rd message.....Q
-00005000: 534f 466f 726d 0103 0000 001a 0051 0053  SOForm.......Q.S
-00005010: 004c 0020 0065 006d 0070 0066 0061 006e  .L. .e.m.p.f.a.n
-00005020: 0067 0065 006e 0800 0000 0006 0000 000c  .g.e.n..........
-00005030: 5153 4c20 7265 6365 6976 6564 0700 0000  QSL received....
-00005040: 0751 534f 466f 726d 0103 0000 0018 0051  .QSOForm.......Q
-00005050: 0053 004c 0020 0067 0065 0073 0065 006e  .S.L. .g.e.s.e.n
-00005060: 0064 0065 0074 0800 0000 0006 0000 0008  .d.e.t..........
-00005070: 5153 4c20 7365 6e74 0700 0000 0751 534f  QSL sent.....QSO
-00005080: 466f 726d 0103 0000 000e 0051 0053 004c  Form.......Q.S.L
-00005090: 002d 0056 0069 0061 0800 0000 0006 0000  .-.V.i.a........
-000050a0: 0007 5153 4c20 7669 6107 0000 0007 5153  ..QSL via.....QS
-000050b0: 4f46 6f72 6d01 0300 0000 1800 5100 5300  OForm.......Q.S.
-000050c0: 4f00 2d00 4600 6f00 7200 6d00 7500 6c00  O.-.F.o.r.m.u.l.
-000050d0: 6100 7208 0000 0000 0600 0000 0851 534f  a.r..........QSO
-000050e0: 2046 6f72 6d07 0000 0007 5153 4f46 6f72   Form.....QSOFor
-000050f0: 6d01 0300 0000 1a00 5100 5300 4f00 2d00  m.......Q.S.O.-.
-00005100: 4b00 6f00 6d00 6d00 6500 6e00 7400 6100  K.o.m.m.e.n.t.a.
-00005110: 7208 0000 0000 0600 0000 0b51 534f 2063  r..........QSO c
-00005120: 6f6d 6d65 6e74 0700 0000 0751 534f 466f  omment.....QSOFo
-00005130: 726d 0103 0000 003e 0051 0053 004f 0020  rm.....>.Q.S.O. 
-00005140: 0077 0075 0072 0064 0065 0020 0076 006f  .w.u.r.d.e. .v.o
-00005150: 006e 0020 0048 0061 006d 0051 0054 0048  .n. .H.a.m.Q.T.H
-00005160: 0020 0061 0062 0067 0065 0077 0069 0065  . .a.b.g.e.w.i.e
-00005170: 0073 0065 006e 0800 0000 0006 0000 0016  .s.e.n..........
-00005180: 5153 4f20 7265 6a65 6374 6564 206f 6e20  QSO rejected on 
-00005190: 4861 6d51 5448 0700 0000 0751 534f 466f  HamQTH.....QSOFo
-000051a0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
-000051b0: 0003 5154 4807 0000 0007 5153 4f46 6f72  ..QTH.....QSOFor
-000051c0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
-000051d0: 0652 5354 2052 7807 0000 0007 5153 4f46  .RST Rx.....QSOF
-000051e0: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-000051f0: 0000 0652 5354 2054 7807 0000 0007 5153  ...RST Tx.....QS
-00005200: 4f46 6f72 6d01 0300 0000 1a00 5200 5300  OForm.......R.S.
-00005210: 5400 2000 6500 6d00 7000 6600 6100 6e00  T. .e.m.p.f.a.n.
-00005220: 6700 6500 6e08 0000 0000 0600 0000 0c52  g.e.n..........R
-00005230: 5354 2072 6563 6569 7665 6407 0000 0007  ST received.....
-00005240: 5153 4f46 6f72 6d01 0300 0000 1800 5200  QSOForm.......R.
-00005250: 5300 5400 2000 6700 6500 7300 6500 6e00  S.T. .g.e.s.e.n.
-00005260: 6400 6500 7408 0000 0000 0600 0000 0852  d.e.t..........R
-00005270: 5354 2073 656e 7407 0000 0007 5153 4f46  ST sent.....QSOF
-00005280: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
-00005290: 0000 0552 6164 696f 0700 0000 0751 534f  ...Radio.....QSO
-000052a0: 466f 726d 0103 0000 0012 0053 0070 0065  Form.......S.p.e
-000052b0: 0069 0063 0068 0065 0072 006e 0800 0000  .i.c.h.e.r.n....
-000052c0: 0006 0000 0004 5361 7665 0700 0000 0751  ......Save.....Q
-000052d0: 534f 466f 726d 0103 0000 0026 0053 0070  SOForm.....&.S.p
-000052e0: 0065 0069 0063 0068 0065 0072 006e 0020  .e.i.c.h.e.r.n. 
-000052f0: 0026 0026 0020 0055 0070 006c 006f 0061  .&.&. .U.p.l.o.a
-00005300: 0064 0800 0000 0006 0000 000e 5361 7665  .d..........Save
-00005310: 2026 2620 5570 6c6f 6164 0700 0000 0751   && Upload.....Q
-00005320: 534f 466f 726d 0103 0000 002a 0065 0051  SOForm.....*.e.Q
-00005330: 0053 004c 002d 004f 0072 0064 006e 0065  .S.L.-.O.r.d.n.e
-00005340: 0072 0020 0061 0075 0073 0077 00e4 0068  .r. .a.u.s.w...h
-00005350: 006c 0065 006e 0800 0000 0006 0000 0012  .l.e.n..........
-00005360: 5365 6c65 6374 2065 5153 4c20 666f 6c64  Select eQSL fold
-00005370: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
-00005380: 0000 0036 0053 0065 0072 0076 0065 0072  ...6.S.e.r.v.e.r
-00005390: 006b 006f 006d 006d 0075 006e 0069 006b  .k.o.m.m.u.n.i.k
-000053a0: 0061 0074 0069 006f 006e 0073 002d 0046  .a.t.i.o.n.s.-.F
-000053b0: 0065 0068 006c 0065 0072 0800 0000 0006  .e.h.l.e.r......
-000053c0: 0000 001a 5365 7276 6572 2063 6f6d 6d75  ....Server commu
-000053d0: 6e69 6361 7469 6f6e 2065 7272 6f72 0700  nication error..
-000053e0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-000053f0: 0800 0000 0006 0000 0005 5374 6172 7407  ..........Start.
-00005400: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
-00005410: ff08 0000 0000 0600 0000 0753 7461 7469  ...........Stati
-00005420: 6f6e 0700 0000 0751 534f 466f 726d 0103  on.....QSOForm..
-00005430: ffff ffff 0800 0000 0006 0000 0007 5375  ..............Su
-00005440: 626d 6f64 6507 0000 0007 5153 4f46 6f72  bmode.....QSOFor
-00005450: 6d01 0300 0000 3000 4400 6100 7300 2000  m.....0.D.a.s. .
-00005460: 5100 5300 4f00 2000 6900 7300 7400 2000  Q.S.O. .i.s.t. .
-00005470: 6500 6900 6e00 2000 4400 7500 7000 6c00  e.i.n. .D.u.p.l.
-00005480: 6900 6b00 6100 7408 0000 0000 0600 0000  i.k.a.t.........
-00005490: 1654 6865 2051 534f 2069 7320 6120 6475  .The QSO is a du
-000054a0: 706c 6963 6174 6507 0000 0007 5153 4f46  plicate.....QSOF
-000054b0: 6f72 6d01 0300 0000 b800 4400 6900 6500  orm.......D.i.e.
-000054c0: 2000 5100 5300 4c00 2d00 5200 6f00 7500   .Q.S.L.-.R.o.u.
-000054d0: 7400 6500 2000 6400 6500 7200 2000 6b00  t.e. .d.e.r. .k.
-000054e0: 6f00 6e00 7400 6100 6b00 7400 6900 6500  o.n.t.a.k.t.i.e.
-000054f0: 7200 7400 6500 6e00 2000 5300 7400 6100  r.t.e.n. .S.t.a.
-00005500: 7400 6900 6f00 6e00 2e00 0a00 4400 6900  t.i.o.n.....D.i.
-00005510: 6500 7300 2000 6900 7300 7400 2000 6e00  e.s. .i.s.t. .n.
-00005520: 6900 6300 6800 7400 2000 6400 6900 6500  i.c.h.t. .d.i.e.
-00005530: 2000 4100 6400 7200 6500 7300 7300 6500   .A.d.r.e.s.s.e.
-00005540: 2000 6400 6500 7300 2000 5100 5300 4c00   .d.e.s. .Q.S.L.
-00005550: 2d00 4d00 6100 6e00 6100 6700 6500 7200  -.M.a.n.a.g.e.r.
-00005560: 7300 2f00 2d00 4200 fc00 7200 6f00 7300  s./.-.B...r.o.s.
-00005570: 2e08 0000 0000 0600 0000 4c54 6865 2063  ..........LThe c
-00005580: 6f6e 7461 6374 6564 2073 7461 7469 6f6e  ontacted station
-00005590: 2051 534c 2072 6f75 7465 2e0a 5468 6973   QSL route..This
-000055a0: 2069 7320 6e6f 7420 7468 6520 5153 4c20   is not the QSL 
-000055b0: 6d61 6e61 6765 722f 6275 7265 6175 2061  manager/bureau a
-000055c0: 6464 7265 7373 2e07 0000 0007 5153 4f46  ddress......QSOF
-000055d0: 6f72 6d01 0300 0000 1000 4500 6e00 6400  orm.......E.n.d.
-000055e0: 6500 7a00 6500 6900 7408 0000 0000 0600  e.z.e.i.t.......
-000055f0: 0000 0854 696d 6520 656e 6407 0000 0007  ...Time end.....
-00005600: 5153 4f46 6f72 6d01 0300 0000 1200 5300  QSOForm.......S.
-00005610: 7400 6100 7200 7400 7a00 6500 6900 7408  t.a.r.t.z.e.i.t.
-00005620: 0000 0000 0600 0000 0a54 696d 6520 7374  .........Time st
-00005630: 6172 7407 0000 0007 5153 4f46 6f72 6d01  art.....QSOForm.
-00005640: 0300 0000 2400 6500 5100 5300 4c00 2d00  ....$.e.Q.S.L.-.
-00005650: 5500 7000 6c00 6f00 6100 6400 2d00 4600  U.p.l.o.a.d.-.F.
-00005660: 6500 6800 6c00 6500 7208 0000 0000 0600  e.h.l.e.r.......
-00005670: 0000 1155 706c 6f61 6420 6551 534c 2065  ...Upload eQSL e
-00005680: 7272 6f72 0700 0000 0751 534f 466f 726d  rror.....QSOForm
-00005690: 0103 0000 001a 0055 0070 006c 006f 0061  .......U.p.l.o.a
-000056a0: 0064 002d 0046 0065 0068 006c 0065 0072  .d.-.F.e.h.l.e.r
-000056b0: 0800 0000 0006 0000 0010 5570 6c6f 6164  ..........Upload
-000056c0: 206c 6f67 2065 7272 6f72 0700 0000 0751   log error.....Q
-000056d0: 534f 466f 726d 0103 0000 0068 0055 0070  SOForm.....h.U.p
-000056e0: 006c 006f 0061 0064 0020 0065 0072 0066  .l.o.a.d. .e.r.f
-000056f0: 006f 006c 0067 0074 0020 006e 0075 0072  .o.l.g.t. .n.u.r
-00005700: 0020 0077 0065 006e 006e 0020 0061 0075  . .w.e.n.n. .a.u
-00005710: 0066 0020 0064 0065 0072 0020 0051 0053  .f. .d.e.r. .Q.S
-00005720: 004c 002d 0053 0065 0069 0074 0065 0020  .L.-.S.e.i.t.e. 
-00005730: 0061 0075 0073 0067 0065 0077 00e4 0068  .a.u.s.g.e.w...h
-00005740: 006c 0074 0800 0000 0006 0000 0024 5570  .l.t.........$Up
-00005750: 6c6f 6164 7320 6f6e 6c79 2069 6620 7365  loads only if se
-00005760: 6c65 6374 6564 206f 6e20 5153 4c20 7061  lected on QSL pa
-00005770: 6765 0700 0000 0751 534f 466f 726d 0103  ge.....QSOForm..
-00005780: 0000 0048 0044 0065 0072 0020 004e 0075  ...H.D.e.r. .N.u
-00005790: 0074 007a 0065 0072 0020 0043 0061 006c  .t.z.e.r. .C.a.l
-000057a0: 006c 0020 0073 0074 0069 006d 006d 0074  .l. .s.t.i.m.m.t
-000057b0: 0020 006e 0069 0063 0068 0074 0020 00fc  . .n.i.c.h.t. ..
-000057c0: 0062 0065 0072 0065 0069 006e 0800 0000  .b.e.r.e.i.n....
-000057d0: 0006 0000 0018 5573 6572 2063 616c 6c20  ......User call 
-000057e0: 646f 6573 206e 6f74 206d 6174 6368 0700  does not match..
-000057f0: 0000 0751 534f 466f 726d 0103 ffff ffff  ...QSOForm......
-00005800: 0800 0000 0006 0000 0004 6551 534c 0700  ..........eQSL..
-00005810: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
-00005820: 0065 0051 0053 004c 0020 0065 006d 0070  .e.Q.S.L. .e.m.p
-00005830: 0066 0061 006e 0067 0065 006e 0800 0000  .f.a.n.g.e.n....
-00005840: 0006 0000 000d 6551 534c 2072 6563 6569  ......eQSL recei
-00005850: 7665 6407 0000 0007 5153 4f46 6f72 6d01  ved.....QSOForm.
-00005860: 0300 0000 1a00 6500 5100 5300 4c00 2000  ......e.Q.S.L. .
-00005870: 6700 6500 7300 6500 6e00 6400 6500 7408  g.e.s.e.n.d.e.t.
-00005880: 0000 0000 0600 0000 0965 5153 4c20 7365  .........eQSL se
-00005890: 6e74 0700 0000 0751 534f 466f 726d 0103  nt.....QSOForm..
-000058a0: 0000 0008 006b 002e 0041 002e 0800 0000  .....k...A......
-000058b0: 0006 0000 0004 6e2e 612e 0700 0000 0751  ......n.a......Q
-000058c0: 534f 466f 726d 0103 0000 0034 0072 0069  SOForm.....4.r.i
-000058d0: 0067 0063 0074 006c 0064 0020 005a 0065  .g.c.t.l.d. .Z.e
-000058e0: 0069 0074 00fc 0062 0065 0072 0073 0063  .i.t...b.e.r.s.c
-000058f0: 0068 0072 0065 0069 0074 0075 006e 0067  .h.r.e.i.t.u.n.g
-00005900: 0800 0000 0006 0000 000f 7269 6763 746c  ..........rigctl
-00005910: 6420 7469 6d65 6f75 7407 0000 0007 5153  d timeout.....QS
-00005920: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
-00005930: 0600 0000 0a79 7979 792d 4d4d 2d64 6407  .....yyyy-MM-dd.
-00005940: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
-00005950: 7a00 4300 4100 5400 2d00 4500 6900 6e00  z.C.A.T.-.E.i.n.
-00005960: 7300 7400 6500 6c00 6c00 7500 6e00 6700  s.t.e.l.l.u.n.g.
-00005970: 2000 7700 7500 7200 6400 2000 6e00 6f00   .w.u.r.d. .n.o.
-00005980: 6300 6800 2000 6e00 6900 6500 2000 6700  c.h. .n.i.e. .g.
-00005990: 6500 7300 7000 6500 6900 6300 6800 6500  e.s.p.e.i.c.h.e.
-000059a0: 7200 7400 2000 6f00 7200 2000 5000 6100  r.t. .o.r. .P.a.
-000059b0: 7200 6100 6d00 6500 7400 6500 7200 2000  r.a.m.e.t.e.r. .
-000059c0: 6600 6500 6800 6c00 6500 6e08 0000 0000  f.e.h.l.e.n.....
-000059d0: 0600 0000 3b43 4154 2063 6f6e 6669 6775  ....;CAT configu
-000059e0: 7261 7469 6f6e 2077 6173 206e 6576 6572  ration was never
-000059f0: 2073 6176 6564 206f 7220 6120 7061 7261   saved or a para
-00005a00: 6d65 7465 7220 6973 206d 6973 7369 6e67  meter is missing
-00005a10: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
-00005a20: 0000 3000 4300 4100 5400 2d00 4500 6900  ..0.C.A.T.-.E.i.
-00005a30: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
-00005a40: 6700 6500 6e00 2000 4600 6500 6800 6c00  g.e.n. .F.e.h.l.
-00005a50: 6500 7208 0000 0000 0600 0000 1243 4154  e.r..........CAT
-00005a60: 2073 6574 7469 6e67 7320 6572 726f 7207   settings error.
-00005a70: 0000 0008 5365 7474 696e 6773 0103 0000  ....Settings....
-00005a80: 002a 0048 0061 006d 006c 0069 0062 0020  .*.H.a.m.l.i.b. 
-00005a90: 0072 0069 0067 0063 0074 006c 0064 0020  .r.i.g.c.t.l.d. 
-00005aa0: 0077 00e4 0068 006c 0065 006e 0800 0000  .w...h.l.e.n....
-00005ab0: 0006 0000 0020 4368 6f6f 7365 2068 616d  ..... Choose ham
-00005ac0: 6c69 6220 7269 6763 746c 6420 6578 6563  lib rigctld exec
-00005ad0: 7574 6162 6c65 0700 0000 0853 6574 7469  utable.....Setti
-00005ae0: 6e67 7301 0300 0000 2000 4400 6100 7400  ngs..... .D.a.t.
-00005af0: 7500 6d00 2f00 5a00 6500 6900 7400 2000  u.m./.Z.e.i.t. .
-00005b00: 5300 7400 6100 7200 7408 0000 0000 0600  S.t.a.r.t.......
-00005b10: 0000 0f44 6174 652f 5469 6d65 2073 7461  ...Date/Time sta
-00005b20: 7274 0700 0000 0853 6574 7469 6e67 7301  rt.....Settings.
-00005b30: 0300 0000 4200 4600 6500 6800 6c00 6500  ....B.F.e.h.l.e.
-00005b40: 7200 2000 6200 6500 6900 6d00 2000 4100  r. .b.e.i.m. .A.
-00005b50: 7500 7300 6600 fc00 6800 7200 6500 6e00  u.s.f...h.r.e.n.
-00005b60: 2000 7600 6f00 6e00 2000 7200 6900 6700   .v.o.n. .r.i.g.
-00005b70: 6300 7400 6c00 6408 0000 0000 0600 0000  c.t.l.d.........
-00005b80: 1745 7272 6f72 2065 7865 6375 7469 6e67  .Error executing
-00005b90: 2072 6967 6374 6c64 0700 0000 0853 6574   rigctld.....Set
-00005ba0: 7469 6e67 7301 03ff ffff ff08 0000 0000  tings...........
-00005bb0: 0600 0000 0648 616d 6c69 6207 0000 0008  .....Hamlib.....
-00005bc0: 5365 7474 696e 6773 0103 0000 004e 0044  Settings.....N.D
-00005bd0: 0069 0065 0020 0067 0065 0077 00e4 0068  .i.e. .g.e.w...h
-00005be0: 006c 0074 0065 0020 0044 0061 0074 0065  .l.t.e. .D.a.t.e
-00005bf0: 0069 0020 0069 0073 0074 0020 006e 0069  .i. .i.s.t. .n.i
-00005c00: 0063 0068 0074 0020 0061 0075 0073 0066  .c.h.t. .a.u.s.f
-00005c10: 00fc 0068 0072 0062 0061 0072 0800 0000  ...h.r.b.a.r....
-00005c20: 0006 0000 0023 5365 6c65 6374 6564 2066  .....#Selected f
-00005c30: 696c 6520 6973 206e 6f74 2074 6865 2065  ile is not the e
-00005c40: 7865 6375 7461 626c 6507 0000 0008 5365  xecutable.....Se
-00005c50: 7474 696e 6773 0103 0000 0014 007a 0065  ttings.......z.e
-00005c60: 0069 0067 0065 0020 0061 006c 006c 0065  .i.g.e. .a.l.l.e
-00005c70: 0800 0000 0006 0000 0008 5368 6f77 2061  ..........Show a
-00005c80: 6c6c 0700 0000 0853 6574 7469 6e67 7301  ll.....Settings.
-00005c90: 03ff ffff ff08 0000 0000 0600 0000 0553  ...............S
-00005ca0: 7461 7274 0700 0000 0853 6574 7469 6e67  tart.....Setting
-00005cb0: 7301 0300 0000 1a00 5300 7400 6100 7200  s.......S.t.a.r.
-00005cc0: 7400 6500 2000 4800 6100 6d00 6c00 6900  t.e. .H.a.m.l.i.
-00005cd0: 6208 0000 0000 0600 0000 0c53 7461 7274  b..........Start
-00005ce0: 2068 616d 6c69 6207 0000 0008 5365 7474   hamlib.....Sett
-00005cf0: 696e 6773 0103 ffff ffff 0800 0000 0006  ings............
-00005d00: 0000 0004 5374 6f70 0700 0000 0853 6574  ....Stop.....Set
-00005d10: 7469 6e67 7301 0300 0000 1a00 5300 7400  tings.......S.t.
-00005d20: 6f00 7000 7000 6500 2000 4800 6100 6d00  o.p.p.e. .H.a.m.
-00005d30: 6c00 6900 6208 0000 0000 0600 0000 0b53  l.i.b..........S
-00005d40: 746f 7020 6861 6d6c 6962 0700 0000 0853  top hamlib.....S
-00005d50: 6574 7469 6e67 7301 0300 0000 0a00 6100  ettings.......a.
-00005d60: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
-00005d70: 0561 6374 6976 0700 0000 0853 6574 7469  .activ.....Setti
-00005d80: 6e67 7301 0300 0000 0e00 6900 6e00 6100  ngs.......i.n.a.
-00005d90: 6b00 7400 6900 7608 0000 0000 0600 0000  k.t.i.v.........
-00005da0: 0769 6e61 6374 6976 0700 0000 0853 6574  .inactiv.....Set
-00005db0: 7469 6e67 7301 0300 0000 4a00 7200 6900  tings.....J.r.i.
-00005dc0: 6700 6300 7400 6c00 6400 2000 6b00 6f00  g.c.t.l.d. .k.o.
-00005dd0: 6e00 6e00 7400 6500 2000 6e00 6900 6300  n.n.t.e. .n.i.c.
-00005de0: 6800 7400 2000 6700 6500 7300 7400 6100  h.t. .g.e.s.t.a.
-00005df0: 7200 7400 6500 7400 2000 7700 6500 7200  r.t.e.t. .w.e.r.
-00005e00: 6400 6500 6e08 0000 0000 0600 0000 1e72  d.e.n..........r
-00005e10: 6967 6374 6c64 2064 6964 206e 6f74 2073  igctld did not s
-00005e20: 7461 7274 2070 726f 7065 726c 7907 0000  tart properly...
-00005e30: 0008 5365 7474 696e 6773 0103 0000 0036  ..Settings.....6
-00005e40: 0072 0069 0067 0063 0074 006c 0064 0020  .r.i.g.c.t.l.d. 
-00005e50: 0069 0073 0074 0020 006e 0069 0063 0068  .i.s.t. .n.i.c.h
-00005e60: 0074 0020 0076 0065 0072 0066 00fc 0067  .t. .v.e.r.f...g
-00005e70: 0062 0061 0072 0800 0000 0006 0000 0018  .b.a.r..........
-00005e80: 7269 6763 746c 6420 6973 206e 6f74 2061  rigctld is not a
-00005e90: 7661 696c 6162 6c65 0700 0000 0853 6574  vailable.....Set
-00005ea0: 7469 6e67 7301 0300 0000 1000 6700 6500  tings.......g.e.
-00005eb0: e400 6e00 6400 6500 7200 7408 0000 0000  ..n.d.e.r.t.....
-00005ec0: 0600 0000 014d 0700 0000 1454 7261 6e73  .....M.....Trans
-00005ed0: 6c61 7465 6454 6162 6c65 4d6f 6465 6c01  latedTableModel.
-00005ee0: 0300 0000 0800 4e00 6500 6900 6e08 0000  ......N.e.i.n...
-00005ef0: 0000 0600 0000 014e 0700 0000 1454 7261  .......N.....Tra
-00005f00: 6e73 6c61 7465 6454 6162 6c65 4d6f 6465  nslatedTableMode
-00005f10: 6c01 0300 0000 1200 6100 6e00 6700 6500  l.......a.n.g.e.
-00005f20: 6600 7200 6100 6700 7408 0000 0000 0600  f.r.a.g.t.......
-00005f30: 0000 0152 0700 0000 1454 7261 6e73 6c61  ...R.....Transla
-00005f40: 7465 6454 6162 6c65 4d6f 6465 6c01 0300  tedTableModel...
-00005f50: 0000 0400 4a00 6108 0000 0000 0600 0000  ....J.a.........
-00005f60: 0159 0700 0000 1454 7261 6e73 6c61 7465  .Y.....Translate
-00005f70: 6454 6162 6c65 4d6f 6465 6c01 03ff ffff  dTableModel.....
-00005f80: ff08 0000 0000 0600 0000 074a 5338 4361  ...........JS8Ca
-00005f90: 6c6c 0700 0000 0f61 7070 5365 6c65 6374  ll.....appSelect
-00005fa0: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
-00005fb0: 0006 0000 0005 4f74 6865 7207 0000 000f  ......Other.....
-00005fc0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
-00005fd0: 0300 0000 2a00 4100 7500 7300 7700 6100  ....*.A.u.s.w.a.
-00005fe0: 6800 6c00 2000 6400 6500 7300 2000 5000  h.l. .d.e.s. .P.
-00005ff0: 7200 6f00 6700 7200 6100 6d00 6d00 7308  r.o.g.r.a.m.m.s.
-00006000: 0000 0000 0600 0000 1653 656c 6563 7420  .........Select 
-00006010: 7468 6520 6170 706c 6963 6174 696f 6e07  the application.
-00006020: 0000 000f 6170 7053 656c 6563 7444 6961  ....appSelectDia
-00006030: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
-00006040: 0000 0657 534a 542d 5807 0000 000f 6170  ...WSJT-X.....ap
-00006050: 7053 656c 6563 7444 6961 6c6f 6701 03ff  pSelectDialog...
-00006060: ffff ff08 0000 0000 0600 0000 0666 6c64  .............fld
-00006070: 6967 6907 0000 000f 6170 7053 656c 6563  igi.....appSelec
-00006080: 7444 6961 6c6f 6701 8800 0000 0201 01    tDialog........
+000000f0: 03c9 3000 0001 3d00 0488 4400 0015 4e00  ..0...=...D...N.
+00000100: 0488 4400 0031 2000 0488 4400 003c 5200  ..D..1 ...D..<R.
+00000110: 04a8 a100 0040 f400 04bb 0400 0033 9700  .....@.......3..
+00000120: 04cf 0400 0033 ce00 04d0 2500 0034 6800  .....3....%..4h.
+00000130: 04d6 8d00 0030 2c00 04e7 1000 001e 7700  .....0,.......w.
+00000140: 04ec 3000 001e 4b00 04ec 3000 0034 ba00  ..0...K...0..4..
+00000150: 0534 9700 0008 0f00 0534 9700 0043 c100  .4.......4...C..
+00000160: 0545 a500 0023 1500 0545 a500 0035 9100  .E...#...E...5..
+00000170: 0545 a500 0045 ec00 0548 3500 0009 1100  .E...E...H5.....
+00000180: 0548 3500 0023 3700 0548 3500 0046 0c00  .H5..#7..H5..F..
+00000190: 0596 7c00 000e 8d00 0598 c500 004c 4900  ..|..........LI.
+000001a0: 05ab 6000 0057 4200 06a6 7c00 0011 8700  ..`..WB...|.....
+000001b0: 06a6 7c00 0051 dc00 06fb 2100 0045 b300  ..|..Q....!..E..
+000001c0: 0714 3e00 0052 8000 144b 9e00 000d fa00  ..>..R...K......
+000001d0: 144e e600 0021 6d00 3477 3000 0000 7f00  .N...!m.4w0.....
+000001e0: 34c5 3000 0000 9f00 36b7 3000 0000 de00  4.0.....6.0.....
+000001f0: 376f f400 004f b500 38a9 3000 0001 1d00  7o...O..8.0.....
+00000200: 4796 c400 0013 b400 4796 c400 0030 7700  G.......G....0w.
+00000210: 47ab 7600 002f c900 47ab 7600 0057 d100  G.v../..G.v..W..
+00000220: 4a2b 8200 003f cb00 4c99 6200 001b fe00  J+...?..L.b.....
+00000230: 4c99 6200 0042 7300 5278 bc00 0030 5100  L.b..Bs.Rx...0Q.
+00000240: 52cc bc00 0007 b600 556a c300 0023 c200  R.......Uj...#..
+00000250: 567e 8100 0048 b600 56ae c200 0059 f400  V~...H..V....Y..
+00000260: 576d c200 0025 2200 576d c200 0048 4000  Wm...%".Wm...H@.
+00000270: 587a ff00 000a e500 587a ff00 0027 e700  Xz......Xz...'..
+00000280: 5aa8 9400 000e 4b00 5aa8 9400 004d cc00  Z.....K.Z....M..
+00000290: 5aa8 9400 0056 dd00 67ab 0600 0057 a500  Z....V..g....W..
+000002a0: 6d92 9400 0055 4600 753c 2300 0047 ff00  m....UF.u<#..G..
+000002b0: 8cd2 1500 0010 7700 aa80 2500 001a bd00  ......w...%.....
+000002c0: ab01 d300 0007 e000 ab72 4500 000a 0400  .........rE.....
+000002d0: bf5b b400 0005 fd00 c656 de00 0040 5300  .[.......V...@S.
+000002e0: ff2c 7700 001c 8601 30ed a300 001d 1d01  .,w.....0.......
+000002f0: 48c4 ff00 001a f701 4d8a bc00 0021 e201  H.......M....!..
+00000300: 5478 6c00 0022 7801 945e f800 002a 0701  Txl.."x..^...*..
+00000310: 9942 b500 0046 2c01 9ce8 5e00 004e 9501  .B...F,...^..N..
+00000320: e578 e300 000d 8b01 e907 4500 0046 7c01  .x........E..F|.
+00000330: fdeb 5400 0051 fc02 3222 f900 003b ad02  ..T..Q..2"...;..
+00000340: 33a9 3400 0009 3002 ac2b 0200 0045 2002  3.4...0..+...E .
+00000350: e7d6 5e00 0002 4102 e7d6 5e00 0015 c002  ..^...A...^.....
+00000360: e7d6 5e00 003c db02 e81d 2400 0041 9d03  ..^..<....$..A..
+00000370: 004d 1200 000c 9203 0149 e600 0021 9a03  .M.......I...!..
+00000380: 0cac 0500 0010 0103 0f6b 1200 0047 7e03  .........k...G~.
+00000390: 0f6b 3200 0024 1303 1bec 1200 0014 1303  .k2..$..........
+000003a0: 4485 3000 0000 1e03 45b3 3000 0000 5e03  D.0.....E.0...^.
+000003b0: 4ecb 9200 0037 2603 4ecb 9200 0056 ff03  N....7&.N....V..
+000003c0: 533f be00 005a 1d03 598b 3200 0008 2e03  S?...Z..Y.2.....
+000003d0: 598b 3200 0021 4803 598b 3200 0044 6703  Y.2..!H.Y.2..Dg.
+000003e0: 5d96 0b00 0044 8a03 6cc3 0400 000b fc03  ]....D..l.......
+000003f0: 881f d400 0006 2603 9ce3 f400 001e 9903  ......&.........
+00000400: 9ce9 a500 0025 9403 f5e0 0700 002e a904  .....%..........
+00000410: 07f6 ee00 0024 d304 07f6 ee00 0047 3104  .....$.......G1.
+00000420: 2b4e 0500 001d c604 6c90 3200 0044 ad04  +N......l.2..D..
+00000430: 8c96 8100 0014 9404 8caf 6200 0014 de04  ..........b.....
+00000440: 9c8b 8500 003c 7204 a472 8400 002c 1b04  .....<r..r...,..
+00000450: ab8e f500 0031 d204 ab8e f600 0031 f704  .....1.......1..
+00000460: ab8e fc00 0032 1c04 ab8f 0100 0032 4104  .....2.......2A.
+00000470: ab8f 0700 0032 6604 ab8f 0800 0032 8b04  .....2f......2..
+00000480: b08b a400 0041 2a04 b2b6 6400 0008 a204  .....A*...d.....
+00000490: c4a9 a900 0013 7b04 cf76 9400 0004 9404  ......{..v......
+000004a0: cf76 9400 0033 ff04 d03a c200 0034 9504  .v...3...:...4..
+000004b0: e826 8800 001e 0304 e826 8800 0043 2404  .&.......&...C$.
+000004c0: e842 f200 001e 2704 e842 f200 0055 bc04  .B....'..B...U..
+000004d0: edd3 6400 0039 aa04 f5b6 e700 002b 0b05  ..d..9.......+..
+000004e0: 0476 9400 0034 e705 1f06 1500 0056 1605  .v...4.......V..
+000004f0: 3268 c400 0004 1805 34db 8200 0022 3005  2h......4...."0.
+00000500: 3ddf a300 000b 0505 3fd1 b400 004d 2305  =.......?....M#.
+00000510: 40b8 b400 004c 0a05 4466 8200 004c cb05  @....L..Df...L..
+00000520: 5776 4500 0049 4505 6336 9e00 0035 5005  WvE..IE.c6...5P.
+00000530: 647d 0e00 0031 7e05 684d 7400 0028 b305  d}...1~.hMt..(..
+00000540: 684f 7400 002e 4705 7865 9800 004b 4805  hOt...G.xe...KH.
+00000550: 7865 b800 004b 6a05 87b0 6300 0055 df05  xe...Kj...c..U..
+00000560: 8ed0 0500 0058 8805 ac50 0300 0053 2d05  .....X...P...S-.
+00000570: c7f7 2800 005a 8105 c984 e900 0033 2206  ..(..Z.......3".
+00000580: 011e c400 0002 9c06 778d 0800 0006 d506  ........w.......
+00000590: 778d 0800 001f 7b06 7e7c a100 0026 7d06  w.....{.~|...&}.
+000005a0: 7e7c a100 004a 0b06 830d be00 002a c506  ~|...J.......*..
+000005b0: 97cc 5200 0036 8b06 bdf0 a400 0019 e906  ..R..6..........
+000005c0: be94 d200 0057 6306 d2af d900 005a ab06  .....Wc......Z..
+000005d0: db4d 4200 0028 4c06 e056 d800 0024 9806  .MB..(L..V...$..
+000005e0: e056 d800 0046 f806 f895 8e00 0016 2a07  .V...F........*.
+000005f0: 2f4a 1500 004e 3307 366b 9300 0005 1a07  /J...N3.6k......
+00000600: 50be 3900 0058 0307 68f8 4400 0052 a807  P.9..X..h.D..R..
+00000610: 693d fe00 0034 2407 6941 4e00 0035 0c07  i=...4$.iAN..5..
+00000620: 6cbb 6300 000e ac07 7f18 a400 004f e907  l.c..........O..
+00000630: 86be 4800 003a 2907 8f3a 3e00 0025 5507  ..H..:)..:>..%U.
+00000640: 8f3a 3e00 0048 7107 e67a d700 0033 6f07  .:>..Hq..z...3o.
+00000650: e76d c800 0025 d707 e78f a400 0026 0d07  .m...%.......&..
+00000660: e79f 3400 0026 4507 e79f 3400 0049 cf07  ..4..&E...4..I..
+00000670: e7e0 a400 002f 5307 e7f2 3400 002f 8e07  ...../S...4../..
+00000680: e7f2 3400 0052 4108 14d3 ed00 0035 b408  ..4..RA......5..
+00000690: 14d3 ed00 004a 3c08 3292 cb00 0002 7908  .....J<.2.....y.
+000006a0: 339b 4e00 0031 4308 3587 6a00 002c 7a08  3.N..1C.5.j..,z.
+000006b0: 36b6 5400 0012 bf08 5ac5 0100 0001 9408  6.T.....Z.......
+000006c0: 5ac5 0100 0014 6108 678f b400 0027 7908  Z.....a.g....'y.
+000006d0: 679f 2400 0027 b108 679f 2400 004b ce08  g.$..'..g.$..K..
+000006e0: 7f52 2500 002b ba08 8879 1400 0019 7b08  .R%..+...y....{.
+000006f0: aae3 e400 0009 d108 b63d de00 0038 1408  .........=...8..
+00000700: bd74 5e00 0023 5908 d39b 6400 0043 e108  .t^..#Y...d..C..
+00000710: f89a cb00 0039 2409 14be 9200 004d 6009  .....9$......M`.
+00000720: 1c52 9500 002f 0809 238c 7500 0017 2709  .R.../..#.u...'.
+00000730: 3f8c ad00 000d 0f09 564e 4200 0050 2109  ?.......VNB..P!.
+00000740: 6c61 f400 0013 df09 6c61 f400 0030 a309  la......la...0..
+00000750: 6fe6 7e00 0011 c309 8fa3 8700 0030 d809  o.~..........0..
+00000760: 97c9 1400 0021 0d09 97c9 1400 0044 2609  .....!.......D&.
+00000770: 97d9 8400 0020 d209 9c7f 1a00 003a c609  ..... .......:..
+00000780: a118 8500 0011 4209 a6a8 f100 0028 f209  ......B......(..
+00000790: c004 d700 0003 df09 c4e8 d700 0001 c409  ................
+000007a0: c8df a200 001e ee09 c943 f500 0010 3c09  .........C....<.
+000007b0: c9cf c500 000c 6409 df31 3800 004a b909  ......d..18..J..
+000007c0: e854 fc00 0015 fb09 e854 fc00 003e 3d09  .T.......T...>=.
+000007d0: f42c fb00 001b d80a 16bb 3400 004a 780a  .,........4..Jx.
+000007e0: 2087 bc00 003f 1b0a 2190 e200 0006 8c0a   ....?..!.......
+000007f0: 2190 e200 001f 2f0a 3f0e 9500 0029 be0a  !...../.?....)..
+00000800: 5e68 d900 0026 d10a 643c 1400 0016 f00a  ^h...&..d<......
+00000810: 65ac e400 0017 cc0a 65ac e400 0040 ab0a  e.......e....@..
+00000820: 6789 3b00 0007 140a 6789 3b00 001f bd0a  g.;.....g.;.....
+00000830: 67a9 0200 0007 500a 67a9 0200 001f fc0a  g.....P.g.......
+00000840: 6dc8 3e00 0037 ad0a 7693 dd00 0032 b00a  m.>..7..v....2..
+00000850: 7833 e400 003c 9c0a 7d6b 2400 0018 af0a  x3...<..}k$.....
+00000860: 8a77 ef00 0032 ea0a 92a2 e500 002a 710a  .w...2.......*q.
+00000870: 9612 e500 0029 640a a8b0 0e00 000e 6b0a  .....)d.......k.
+00000880: a8b0 0e00 004d ed0a acdb 7e00 0002 1c0a  .....M....~.....
+00000890: b945 f500 002b f60a b945 f500 004e 100a  .E...+...E...N..
+000008a0: c389 2500 0029 2d0a c5b4 4900 0043 460a  ..%..)-...I..CF.
+000008b0: c897 c500 0006 4e0a cec2 8400 0040 ce0a  ......N......@..
+000008c0: d2f0 b500 0003 090a d382 7700 0003 570a  ..........w...W.
+000008d0: e2b5 9600 0004 b50a f31c 2200 003e a70b  .........."..>..
+000008e0: 1562 0700 0053 620b 1805 3900 0015 700b  .b...Sb...9...p.
+000008f0: 4597 5500 0008 500b 5d8a f400 0020 3b0b  E.U...P.].... ;.
+00000900: 6628 d200 0037 6b0b 7fe2 de00 0035 f30b  f(...7k......5..
+00000910: ad17 7800 001b aa0b ff25 ce00 001c d80c  ..x......%......
+00000920: 08f5 6c00 0041 580c 107d 9300 0003 a10c  ..l..AX..}......
+00000930: 10ba b200 0028 0a0c 1536 f700 002d ed0c  .....(...6...-..
+00000940: 1f2f 0200 0050 720c 242f 6400 0038 8b0c  ./...Pr.$/d..8..
+00000950: 29f2 a400 0053 070c 6a19 e900 0040 040c  )....S..j....@..
+00000960: 8c09 2900 001d 8f0c 8c09 2900 0042 ef0c  ..).......)..B..
+00000970: 9688 9500 0014 b80c a3fa 5f00 001a 7f0c  .........._.....
+00000980: a6e8 d400 003d 810c bb01 7300 000c d20c  .....=....s.....
+00000990: bb01 7300 0036 4a0c c9a0 0e00 002e 840d  ..s..6J.........
+000009a0: 0218 6400 004c 7b0d 07a4 f800 003e 6a0d  ..d..L{......>j.
+000009b0: 1f27 b200 0015 0c0d 3504 b400 003d dd0d  .'......5....=..
+000009c0: 76f7 5900 001c 2d0d 825f 7300 000f 4f0d  v.Y...-.._s...O.
+000009d0: a03c 1200 0054 340d d0ff 4c00 002d a10d  .<...T4...L..-..
+000009e0: f2ea c200 003f 610d fe4e 2400 001a 320d  .....?a..N$...2.
+000009f0: fe4e 2400 0054 fa0e 0543 5500 0024 5a0e  .N$..T...CU..$Z.
+00000a00: 05d1 b500 0054 930e 0743 5500 0047 c30e  .....T...CU..G..
+00000a10: 0906 8800 003b 000e 233d d500 0050 b80e  .....;..#=...P..
+00000a20: 87ac 6400 0020 840e 93fa 5200 0017 f10e  ..d.. ....R.....
+00000a30: a32f e400 0042 a00e c47b 9900 002f fc0e  ./...B...{.../..
+00000a40: c497 a200 000b 730e c72a a600 0005 880e  ......s..*......
+00000a50: de3d a200 003d 140e e46b 3400 004b 8c0e  .=...=...k4..K..
+00000a60: fdeb 3400 0049 8d0f 165e c400 0048 f60f  ..4..I...^...H..
+00000a70: 3562 ce00 0018 520f 6963 bc00 000d 540f  5b....R.ic....T.
+00000a80: 6963 bc00 002b 800f 6963 bc00 0056 a40f  ic...+..ic...V..
+00000a90: 6978 c700 0036 d90f 6c98 6c00 0059 c90f  ix...6..l.l..Y..
+00000aa0: 7ddd 2800 0051 600f 8007 d400 003b ec0f  }.(..Q`......;..
+00000ab0: 8313 8900 0013 480f cb15 5200 0019 310f  ......H...R...1.
+00000ac0: e6f6 3400 0043 6e69 0000 5ad5 03ff ffff  ..4..Cni..Z.....
+00000ad0: ff08 0000 0000 0600 0000 032e 2e2e 0700  ................
+00000ae0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000af0: 0000 0000 0600 0000 0631 3135 3230 3007  .........115200.
+00000b00: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000b10: 0800 0000 0006 0000 0004 3132 3030 0700  ..........1200..
+00000b20: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000b30: 0000 0000 0600 0000 0631 3238 3030 3007  .........128000.
+00000b40: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000b50: 0800 0000 0006 0000 0005 3134 3430 3007  ..........14400.
+00000b60: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000b70: 0800 0000 0006 0000 0005 3139 3230 3007  ..........19200.
+00000b80: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+00000b90: 0800 0000 0006 0000 0004 3234 3030 0700  ..........2400..
+00000ba0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000bb0: 0000 0000 0600 0000 0533 3834 3030 0700  .........38400..
+00000bc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000bd0: 0000 0000 0600 0000 0434 3830 3007 0000  .........4800...
+00000be0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000bf0: 0000 0006 0000 0005 3537 3630 3007 0000  ........57600...
+00000c00: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00000c10: 0000 0006 0000 0004 3936 3030 0700 0000  ........9600....
+00000c20: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000c30: 0000 0600 0000 013c 0700 0000 0644 6961  .......<.....Dia
+00000c40: 6c6f 6701 03ff ffff ff08 0000 0000 0600  log.............
+00000c50: 0000 013e 0700 0000 0644 6961 6c6f 6701  ...>.....Dialog.
+00000c60: 0300 0000 0e00 4100 6e00 7400 6500 6e00  ......A.n.t.e.n.
+00000c70: 6e00 6508 0000 0000 0600 0000 0741 6e74  n.e..........Ant
+00000c80: 656e 6e61 0700 0000 0644 6961 6c6f 6701  enna.....Dialog.
+00000c90: 0300 0000 1600 4100 7500 6600 7300 7400  ......A.u.f.s.t.
+00000ca0: 6500 6900 6700 6500 6e00 6408 0000 0000  e.i.g.e.n.d.....
+00000cb0: 0600 0000 0941 7363 656e 6469 6e67 0700  .....Ascending..
+00000cc0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00000cd0: 0000 0000 0600 0000 0343 4154 0700 0000  .........CAT....
+00000ce0: 0644 6961 6c6f 6701 03ff ffff ff08 0000  .Dialog.........
+00000cf0: 0000 0600 0000 0a43 422d 5374 6174 696f  .......CB-Statio
+00000d00: 6e07 0000 0006 4469 616c 6f67 0103 0000  n.....Dialog....
+00000d10: 0014 0052 0075 0066 007a 0065 0069 0063  ...R.u.f.z.e.i.c
+00000d20: 0068 0065 006e 0800 0000 0006 0000 0009  .h.e.n..........
+00000d30: 4361 6c6c 2073 6967 6e07 0000 0006 4469  Call sign.....Di
+00000d40: 616c 6f67 0103 ffff ffff 0800 0000 0006  alog............
+00000d50: 0000 0008 4361 6c6c 626f 6f6b 0700 0000  ....Callbook....
+00000d60: 0644 6961 6c6f 6701 0300 0000 3800 5a00  .Dialog.....8.Z.
+00000d70: 6500 7200 7400 6900 6600 6900 6b00 6100  e.r.t.i.f.i.k.a.
+00000d80: 7400 2000 6200 6500 6e00 f600 7400 6900  t. .b.e.n...t.i.
+00000d90: 6700 7400 2000 5000 6100 7300 7300 7700  g.t. .P.a.s.s.w.
+00000da0: 6f00 7200 7408 0000 0000 0600 0000 1a43  o.r.t..........C
+00000db0: 6572 7469 6669 6361 7465 206e 6565 6473  ertificate needs
+00000dc0: 2070 6173 7377 6f72 6407 0000 0006 4469   password.....Di
+00000dd0: 616c 6f67 0103 0000 0024 0053 0070 0061  alog.....$.S.p.a
+00000de0: 006c 0074 0065 006e 0020 0076 0065 0072  .l.t.e.n. .v.e.r
+00000df0: 0073 0074 0065 0063 006b 0065 006e 0800  .s.t.e.c.k.e.n..
+00000e00: 0000 0006 0000 000f 436f 6c75 6d6e 7320  ........Columns 
+00000e10: 746f 2068 6964 6507 0000 0006 4469 616c  to hide.....Dial
+00000e20: 6f67 0103 0000 0020 0053 0070 0061 006c  og..... .S.p.a.l
+00000e30: 0074 0065 006e 0020 0061 006e 007a 0065  .t.e.n. .a.n.z.e
+00000e40: 0069 0067 0065 006e 0800 0000 0006 0000  .i.g.e.n........
+00000e50: 000f 436f 6c75 6d6e 7320 746f 2073 686f  ..Columns to sho
+00000e60: 7707 0000 0006 4469 616c 6f67 0103 0000  w.....Dialog....
+00000e70: 0018 0041 006e 006d 0065 006c 0064 0065  ...A.n.m.e.l.d.e
+00000e80: 0064 0061 0074 0065 006e 0800 0000 0006  .d.a.t.e.n......
+00000e90: 0000 000b 4372 6564 656e 7469 616c 7307  ....Credentials.
+00000ea0: 0000 0006 4469 616c 6f67 0103 0000 0014  ....Dialog......
+00000eb0: 0041 0062 0073 0074 0065 0069 0067 0065  .A.b.s.t.e.i.g.e
+00000ec0: 006e 0064 0800 0000 0006 0000 000a 4465  .n.d..........De
+00000ed0: 7363 656e 6469 6e67 0700 0000 0644 6961  scending.....Dia
+00000ee0: 6c6f 6701 0300 0000 3e00 5700 6900 7200  log.....>.W.i.r.
+00000ef0: 6b00 7300 6100 6d00 2000 6e00 6100 6300  k.s.a.m. .n.a.c.
+00000f00: 6800 2000 4100 6e00 7700 6500 6e00 6400  h. .A.n.w.e.n.d.
+00000f10: 7500 6e00 6700 7300 6e00 6500 7500 7300  u.n.g.s.n.e.u.s.
+00000f20: 7400 6100 7200 7408 0000 0000 0600 0000  t.a.r.t.........
+00000f30: 2345 6666 6563 7469 7665 2061 6674 6572  #Effective after
+00000f40: 2061 7070 6c69 6361 7469 6f6e 2072 6573   application res
+00000f50: 7461 7274 0700 0000 0644 6961 6c6f 6701  tart.....Dialog.
+00000f60: 03ff ffff ff08 0000 0000 0600 0000 0645  ...............E
+00000f70: 7870 6f72 7407 0000 0006 4469 616c 6f67  xport.....Dialog
+00000f80: 0103 0000 0034 0045 0078 0070 006f 0072  .....4.E.x.p.o.r
+00000f90: 0074 0069 0065 0072 0065 0020 0043 0042  .t.i.e.r.e. .C.B
+00000fa0: 002d 0051 0053 004f 0073 0020 0069 006e  .-.Q.S.O.s. .i.n
+00000fb0: 0020 0041 0044 0049 0046 0800 0000 0006  . .A.D.I.F......
+00000fc0: 0000 0016 4578 706f 7274 2043 4220 5153  ....Export CB QS
+00000fd0: 4f73 2074 6f20 4144 4946 0700 0000 0644  Os to ADIF.....D
+00000fe0: 6961 6c6f 6701 0300 0000 3c00 4500 7800  ialog.....<.E.x.
+00000ff0: 7000 6f00 7200 7400 6900 6500 7200 6500  p.o.r.t.i.e.r.e.
+00001000: 2000 6e00 7500 7200 2000 6700 6500 6600   .n.u.r. .g.e.f.
+00001010: 6900 6c00 7400 6500 7200 7400 6500 2000  i.l.t.e.r.t.e. .
+00001020: 5100 5300 4f00 7308 0000 0000 0600 0000  Q.S.O.s.........
+00001030: 1745 7870 6f72 7420 6f6e 6c79 2072 6563  .Export only rec
+00001040: 656e 7420 5153 4f73 0700 0000 0644 6961  ent QSOs.....Dia
+00001050: 6c6f 6701 0300 0000 4200 4500 7800 7000  log.....B.E.x.p.
+00001060: 6f00 7200 7400 6900 6500 7200 6500 2000  o.r.t.i.e.r.e. .
+00001070: 6500 6900 6700 6500 6e00 6500 2000 4e00  e.i.g.e.n.e. .N.
+00001080: 6f00 7400 6900 7a00 6500 6e00 2000 6900  o.t.i.z.e.n. .i.
+00001090: 6e00 2000 4100 4400 4900 4608 0000 0000  n. .A.D.I.F.....
+000010a0: 0600 0000 1845 7870 6f72 7420 6f77 6e20  .....Export own 
+000010b0: 6e6f 7465 7320 746f 2041 4449 4607 0000  notes to ADIF...
+000010c0: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+000010d0: 0000 0006 0000 000e 4861 6d6c 6962 2072  ........Hamlib r
+000010e0: 6967 6374 6c64 0700 0000 0644 6961 6c6f  igctld.....Dialo
+000010f0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001100: 0d49 6d70 6f72 742f 4578 706f 7274 0700  .Import/Export..
+00001110: 0000 0644 6961 6c6f 6701 0300 0000 1a00  ...Dialog.......
+00001120: 5300 6300 6800 6e00 6900 7400 7400 7300  S.c.h.n.i.t.t.s.
+00001130: 7400 6500 6c00 6c00 6508 0000 0000 0600  t.e.l.l.e.......
+00001140: 0000 0949 6e74 6572 6661 6365 0700 0000  ...Interface....
+00001150: 0644 6961 6c6f 6701 0300 0000 2000 6c00  .Dialog..... .l.
+00001160: 6500 7400 7a00 7400 6500 7300 2000 4800  e.t.z.t.e.s. .H.
+00001170: 6100 6c00 6200 6a00 6100 6800 7208 0000  a.l.b.j.a.h.r...
+00001180: 0000 0600 0000 0e4c 6173 7420 6861 6c66  .......Last half
+00001190: 2079 6561 7207 0000 0006 4469 616c 6f67   year.....Dialog
+000011a0: 0103 0000 001a 006c 0065 0074 007a 0074  .......l.e.t.z.t
+000011b0: 0065 006e 0020 004d 006f 006e 0061 0074  .e.n. .M.o.n.a.t
+000011c0: 0800 0000 0006 0000 000a 4c61 7374 206d  ..........Last m
+000011d0: 6f6e 7468 0700 0000 0644 6961 6c6f 6701  onth.....Dialog.
+000011e0: 0300 0000 1800 6c00 6500 7400 7a00 7400  ......l.e.t.z.t.
+000011f0: 6500 2000 5700 6f00 6300 6800 6508 0000  e. .W.o.c.h.e...
+00001200: 0000 0600 0000 094c 6173 7420 7765 656b  .......Last week
+00001210: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001220: 1800 6c00 6500 7400 7a00 7400 6500 7300  ..l.e.t.z.t.e.s.
+00001230: 2000 4a00 6100 6800 7208 0000 0000 0600   .J.a.h.r.......
+00001240: 0000 094c 6173 7420 7965 6172 0700 0000  ...Last year....
+00001250: 0644 6961 6c6f 6701 0300 0000 0c00 4200  .Dialog.......B.
+00001260: 7200 6500 6900 7400 6508 0000 0000 0600  r.e.i.t.e.......
+00001270: 0000 034c 6174 0700 0000 0644 6961 6c6f  ...Lat.....Dialo
+00001280: 6701 0300 0000 0a00 5300 7400 7500 6600  g.......S.t.u.f.
+00001290: 6508 0000 0000 0600 0000 054c 6576 656c  e..........Level
+000012a0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+000012b0: 0c00 4c00 6900 7300 7400 6500 6e08 0000  ..L.i.s.t.e.n...
+000012c0: 0000 0600 0000 084c 6973 7469 6e67 7307  .......Listings.
+000012d0: 0000 0006 4469 616c 6f67 0103 ffff ffff  ....Dialog......
+000012e0: 0800 0000 0006 0000 0004 4c6f 5457 0700  ..........LoTW..
+000012f0: 0000 0644 6961 6c6f 6701 03ff ffff ff08  ...Dialog.......
+00001300: 0000 0000 0600 0000 074c 6f63 6174 6f72  .........Locator
+00001310: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001320: 2c00 4c00 6f00 6700 2000 6900 6e00 2000  ,.L.o.g. .i.n. .
+00001330: 4400 6100 7400 6500 6900 2000 7300 6300  D.a.t.e.i. .s.c.
+00001340: 6800 7200 6500 6900 6200 6500 6e08 0000  h.r.e.i.b.e.n...
+00001350: 0000 0600 0000 0b4c 6f67 2074 6f20 6669  .......Log to fi
+00001360: 6c65 0700 0000 0644 6961 6c6f 6701 0300  le.....Dialog...
+00001370: 0000 1e00 4c00 6f00 6700 6700 6900 6e00  ....L.o.g.g.i.n.
+00001380: 6700 2d00 4100 7500 7300 6700 6100 6200  g.-.A.u.s.g.a.b.
+00001390: 6508 0000 0000 0600 0000 0e4c 6f67 6769  e..........Loggi
+000013a0: 6e67 206f 7574 7075 7407 0000 0006 4469  ng output.....Di
+000013b0: 616c 6f67 0103 0000 000a 004c 00e4 006e  alog.......L...n
+000013c0: 0067 0065 0800 0000 0006 0000 0003 4c6f  .g.e..........Lo
+000013d0: 6e07 0000 0006 4469 616c 6f67 0103 ffff  n.....Dialog....
+000013e0: ffff 0800 0000 0006 0000 0004 4e61 6d65  ............Name
+000013f0: 0700 0000 0644 6961 6c6f 6701 0300 0000  .....Dialog.....
+00001400: 5e00 4300 4200 2000 5100 5300 4f00 7300  ^.C.B. .Q.S.O.s.
+00001410: 2000 7700 6500 7200 6400 6500 6e00 2000   .w.e.r.d.e.n. .
+00001420: 6200 6500 6900 6d00 2000 4900 6d00 7000  b.e.i.m. .I.m.p.
+00001430: 6f00 7200 7400 2000 6900 6d00 6d00 6500  o.r.t. .i.m.m.e.
+00001440: 7200 2000 6200 6500 7200 fc00 6300 6b00  r. .b.e.r...c.k.
+00001450: 7300 6900 6300 6800 7400 6900 6700 7408  s.i.c.h.t.i.g.t.
+00001460: 0000 0000 0600 0000 284f 6e20 696d 706f  ........(On impo
+00001470: 7274 2043 4220 5153 4f73 2077 696c 6c20  rt CB QSOs will 
+00001480: 616c 7761 7973 2062 6520 6861 6e64 6c65  always be handle
+00001490: 6407 0000 0006 4469 616c 6f67 0103 0000  d.....Dialog....
+000014a0: 0010 0050 0061 0073 0073 0077 006f 0072  ...P.a.s.s.w.o.r
+000014b0: 0074 0800 0000 0006 0000 0008 5061 7373  .t..........Pass
+000014c0: 776f 7264 0700 0000 0644 6961 6c6f 6701  word.....Dialog.
+000014d0: 0300 0000 7000 5000 6100 7300 7300 7700  ....p.P.a.s.s.w.
+000014e0: 6f00 7200 7400 2000 6400 6500 7300 2000  o.r.t. .d.e.s. .
+000014f0: 4c00 6f00 5400 5700 2d00 4f00 6e00 6c00  L.o.T.W.-.O.n.l.
+00001500: 6900 6e00 6500 2d00 4100 6300 6300 6f00  i.n.e.-.A.c.c.o.
+00001510: 7500 6e00 7400 7300 2c00 2000 6e00 6900  u.n.t.s.,. .n.i.
+00001520: 6300 6800 7400 2000 6400 6500 7300 2000  c.h.t. .d.e.s. .
+00001530: 5a00 6500 7200 7400 6900 6600 6900 6b00  Z.e.r.t.i.f.i.k.
+00001540: 6100 7400 7308 0000 0000 0600 0000 3850  a.t.s.........8P
+00001550: 6173 7377 6f72 6420 666f 7220 4c6f 5457  assword for LoTW
+00001560: 206f 6e6c 696e 6520 6163 636f 756e 7420   online account 
+00001570: 6e6f 7420 666f 7220 7468 6520 6365 7274  not for the cert
+00001580: 6966 6963 6174 6507 0000 0006 4469 616c  ificate.....Dial
+00001590: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+000015a0: 0003 5154 4807 0000 0006 4469 616c 6f67  ..QTH.....Dialog
+000015b0: 0103 ffff ffff 0800 0000 0006 0000 0005  ................
+000015c0: 5261 6469 6f07 0000 0006 4469 616c 6f67  Radio.....Dialog
+000015d0: 0103 0000 0018 004e 0065 0075 0065 0073  .......N.e.u.e.s
+000015e0: 0074 0065 0020 0051 0053 004f 0073 0800  .t.e. .Q.S.O.s..
+000015f0: 0000 0006 0000 000b 5265 6365 6e74 2051  ........Recent Q
+00001600: 534f 7307 0000 0006 4469 616c 6f67 0103  SOs.....Dialog..
+00001610: 0000 0012 0046 0075 006e 006b 0067 0065  .....F.u.n.k.g.e
+00001620: 0072 00e4 0074 0800 0000 0006 0000 0003  .r...t..........
+00001630: 5269 6707 0000 0006 4469 616c 6f67 0103  Rig.....Dialog..
+00001640: 0000 004c 0053 0069 0065 0068 0065 0020  ...L.S.i.e.h.e. 
+00001650: 0045 0069 006e 0073 0074 0065 006c 006c  .E.i.n.s.t.e.l.l
+00001660: 0075 006e 0067 0065 006e 0020 0052 0065  .u.n.g.e.n. .R.e
+00001670: 0069 0074 0065 0072 0020 0022 0041 006e  .i.t.e.r. .".A.n
+00001680: 0077 0065 006e 0064 0075 006e 0067 0022  .w.e.n.d.u.n.g."
+00001690: 0800 0000 0006 0000 0022 5365 6520 7365  ........."See se
+000016a0: 7474 696e 6773 2070 6167 6520 2255 7365  ttings page "Use
+000016b0: 7220 696e 7465 7266 6163 6522 0700 0000  r interface"....
+000016c0: 0644 6961 6c6f 6701 0300 0000 3400 4300  .Dialog.....4.C.
+000016d0: 4200 2d00 4200 6100 6e00 6400 2000 6100  B.-.B.a.n.d. .a.
+000016e0: 7500 7400 6f00 6d00 6100 7400 6900 7300  u.t.o.m.a.t.i.s.
+000016f0: 6300 6800 2000 7700 e400 6800 6c00 6500  c.h. .w...h.l.e.
+00001700: 6e08 0000 0000 0600 0000 1953 656c 6563  n..........Selec
+00001710: 7420 4342 2062 616e 6420 6279 2064 6566  t CB band by def
+00001720: 6175 6c74 0700 0000 0644 6961 6c6f 6701  ault.....Dialog.
+00001730: 0300 0000 0c00 4400 6900 6500 6e00 7300  ......D.i.e.n.s.
+00001740: 7408 0000 0000 0600 0000 0753 6572 7669  t..........Servi
+00001750: 6365 0700 0000 0644 6961 6c6f 6701 0300  ce.....Dialog...
+00001760: 0000 1a00 5300 6500 7400 7a00 6500 2000  ....S.e.t.z.e. .
+00001770: 4c00 6f00 6300 6100 7400 6f00 7208 0000  L.o.c.a.t.o.r...
+00001780: 0000 0600 0000 0b53 6574 206c 6f63 6174  .......Set locat
+00001790: 6f72 0700 0000 0644 6961 6c6f 6701 0300  or.....Dialog...
+000017a0: 0000 1a00 4500 6900 6e00 7300 7400 6500  ....E.i.n.s.t.e.
+000017b0: 6c00 6c00 7500 6e00 6700 6500 6e08 0000  l.l.u.n.g.e.n...
+000017c0: 0000 0600 0000 0853 6574 7469 6e67 7307  .......Settings.
+000017d0: 0000 0006 4469 616c 6f67 0103 0000 001c  ....Dialog......
+000017e0: 005a 0065 0069 0067 0065 0020 0051 0053  .Z.e.i.g.e. .Q.S
+000017f0: 004f 0073 0020 0066 00fc 0072 0800 0000  .O.s. .f...r....
+00001800: 0006 0000 000e 5368 6f77 2051 534f 7320  ......Show QSOs 
+00001810: 6672 6f6d 0700 0000 0644 6961 6c6f 6701  from.....Dialog.
+00001820: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
+00001830: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
+00001840: 0000 0853 686f 7720 616c 6c07 0000 0006  ...Show all.....
+00001850: 4469 616c 6f67 0103 0000 0040 0053 0070  Dialog.....@.S.p
+00001860: 0061 006c 0074 0065 006e 0020 0061 006e  .a.l.t.e.n. .a.n
+00001870: 007a 0065 0069 0067 0065 006e 0020 006f  .z.e.i.g.e.n. .o
+00001880: 0064 0065 0072 0020 0076 0065 0072 0073  .d.e.r. .v.e.r.s
+00001890: 0074 0065 0063 006b 0065 006e 0800 0000  .t.e.c.k.e.n....
+000018a0: 0006 0000 0014 5368 6f77 206f 7220 6869  ......Show or hi
+000018b0: 6465 2063 6f6c 756d 6e73 0700 0000 0644  de columns.....D
+000018c0: 6961 6c6f 6701 0300 0000 2800 5300 6f00  ialog.....(.S.o.
+000018d0: 7200 7400 6900 6500 7200 6500 2000 6e00  r.t.i.e.r.e. .n.
+000018e0: 6100 6300 6800 2000 5300 7000 6100 6c00  a.c.h. .S.p.a.l.
+000018f0: 7400 6508 0000 0000 0600 0000 0e53 6f72  t.e..........Sor
+00001900: 7420 6f6e 2063 6f6c 756d 6e07 0000 0006  t on column.....
+00001910: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00001920: 0006 0000 0005 5374 6172 7407 0000 0006  ......Start.....
+00001930: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00001940: 0006 0000 0007 5374 6174 696f 6e07 0000  ......Station...
+00001950: 0006 4469 616c 6f67 0103 ffff ffff 0800  ..Dialog........
+00001960: 0000 0006 0000 0004 5451 534c 0700 0000  ........TQSL....
+00001970: 0644 6961 6c6f 6701 0300 0000 6400 5600  .Dialog.....d.V.
+00001980: 6500 7200 7700 6500 6e00 6400 6500 2000  e.r.w.e.n.d.e. .
+00001990: 6400 6900 6500 2000 6b00 6f00 6e00 6600  d.i.e. .k.o.n.f.
+000019a0: 6900 6700 7500 7200 6900 6500 7200 7400  i.g.u.r.i.e.r.t.
+000019b0: 6500 2000 4900 4400 2000 6200 6500 6900  e. .I.D. .b.e.i.
+000019c0: 2000 6600 6500 6800 6c00 6500 6e00 6400   .f.e.h.l.e.n.d.
+000019d0: 6500 6e00 2000 5700 6500 7200 7400 6500  e.n. .W.e.r.t.e.
+000019e0: 6e08 0000 0000 0600 0000 2455 7365 2063  n.........$Use c
+000019f0: 6f6e 6669 6775 7265 6420 4944 2066 6f72  onfigured ID for
+00001a00: 206d 6973 7369 6e67 2076 616c 7565 7307   missing values.
+00001a10: 0000 0006 4469 616c 6f67 0103 0000 006e  ....Dialog.....n
+00001a20: 0056 0065 0072 0077 0065 006e 0064 0065  .V.e.r.w.e.n.d.e
+00001a30: 0020 0064 0069 0065 0020 006b 006f 006e  . .d.i.e. .k.o.n
+00001a40: 0066 0069 0067 0075 0072 0069 0065 0072  .f.i.g.u.r.i.e.r
+00001a50: 0074 0065 0020 0053 0074 0061 0074 0069  .t.e. .S.t.a.t.i
+00001a60: 006f 006e 0020 0062 0065 0069 0020 0066  .o.n. .b.e.i. .f
+00001a70: 0065 0068 006c 0065 006e 0064 0065 006e  .e.h.l.e.n.d.e.n
+00001a80: 0020 0057 0065 0072 0074 0065 006e 0800  . .W.e.r.t.e.n..
+00001a90: 0000 0006 0000 0029 5573 6520 636f 6e66  .......)Use conf
+00001aa0: 6967 7572 6564 2053 7461 7469 6f6e 2066  igured Station f
+00001ab0: 6f72 206d 6973 7369 6e67 2076 616c 7565  or missing value
+00001ac0: 7307 0000 0006 4469 616c 6f67 0103 0000  s.....Dialog....
+00001ad0: 0012 0041 006e 0077 0065 006e 0064 0075  ...A.n.w.e.n.d.u
+00001ae0: 006e 0067 0800 0000 0006 0000 000e 5573  .n.g..........Us
+00001af0: 6572 2069 6e74 6572 6661 6365 0700 0000  er interface....
+00001b00: 0644 6961 6c6f 6701 0300 0000 1800 4200  .Dialog.......B.
+00001b10: 6500 6e00 7500 7400 7a00 6500 7200 6e00  e.n.u.t.z.e.r.n.
+00001b20: 6100 6d00 6508 0000 0000 0600 0000 0855  a.m.e..........U
+00001b30: 7365 726e 616d 6507 0000 0006 4469 616c  sername.....Dial
+00001b40: 6f67 0103 0000 0078 0042 0065 006e 0075  og.....x.B.e.n.u
+00001b50: 0074 007a 0065 0072 006e 0061 006d 0065  .t.z.e.r.n.a.m.e
+00001b60: 0020 0064 0065 0073 0020 004c 006f 0054  . .d.e.s. .L.o.T
+00001b70: 0057 002d 004f 006e 006c 0069 006e 0065  .W.-.O.n.l.i.n.e
+00001b80: 002d 0041 0063 0063 006f 0075 006e 0074  .-.A.c.c.o.u.n.t
+00001b90: 0073 002c 0020 006e 0069 0063 0068 0074  .s.,. .n.i.c.h.t
+00001ba0: 0020 0064 0065 0073 0020 005a 0065 0072  . .d.e.s. .Z.e.r
+00001bb0: 0074 0069 0066 0069 006b 0061 0074 0073  .t.i.f.i.k.a.t.s
+00001bc0: 0800 0000 0006 0000 0038 5573 6572 6e61  .........8Userna
+00001bd0: 6d65 2066 6f72 204c 6f54 5720 6f6e 6c69  me for LoTW onli
+00001be0: 6e65 2061 6363 6f75 6e74 206e 6f74 2066  ne account not f
+00001bf0: 6f72 2074 6865 2063 6572 7469 6669 6361  or the certifica
+00001c00: 7465 0700 0000 0644 6961 6c6f 6701 0300  te.....Dialog...
+00001c10: 0000 2000 4400 6100 7400 6500 6900 fc00  .. .D.a.t.e.i...
+00001c20: 6200 6500 7200 7700 6100 6300 6800 7500  b.e.r.w.a.c.h.u.
+00001c30: 6e00 6708 0000 0000 0600 0000 0a57 6174  n.g..........Wat
+00001c40: 6368 2046 696c 6507 0000 0006 4469 616c  ch File.....Dial
+00001c50: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00001c60: 0004 6551 534c 0700 0000 0644 6961 6c6f  ..eQSL.....Dialo
+00001c70: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+00001c80: 02c2 b007 0000 0006 4469 616c 6f67 0103  ........Dialog..
+00001c90: 0000 009e 0045 0069 006e 0020 0044 0061  .....E.i.n. .D.a
+00001ca0: 0074 0065 006e 0062 0061 006e 006b 002d  .t.e.n.b.a.n.k.-
+00001cb0: 0042 0061 0063 006b 0075 0070 0020 006b  .B.a.c.k.u.p. .k
+00001cc0: 006f 006e 006e 0074 0065 0020 006e 0069  .o.n.n.t.e. .n.i
+00001cd0: 0063 0068 0074 0020 0065 0072 0073 0074  .c.h.t. .e.r.s.t
+00001ce0: 0065 006c 006c 0074 0020 0077 0065 0072  .e.l.l.t. .w.e.r
+00001cf0: 0064 0065 006e 002e 000a 0044 0069 0065  .d.e.n.....D.i.e
+00001d00: 0020 0044 0061 0074 0065 0069 0020 0065  . .D.a.t.e.i. .e
+00001d10: 0078 0069 0073 0074 0069 0065 0072 0074  .x.i.s.t.i.e.r.t
+00001d20: 0020 0062 0065 0072 0065 0069 0074 0073  . .b.e.r.e.i.t.s
+00001d30: 002e 0800 0000 0006 0000 0040 4120 6461  ...........@A da
+00001d40: 7461 6261 7365 2062 6163 6b75 7020 636f  tabase backup co
+00001d50: 756c 6420 6e6f 7420 6265 2063 7265 6174  uld not be creat
+00001d60: 6564 2e0a 5468 6520 6669 6c65 2061 6c72  ed..The file alr
+00001d70: 6561 6479 2065 7869 7374 732e 0700 0000  eady exists.....
+00001d80: 0944 7261 676f 6e4c 6f67 0103 0000 004e  .DragonLog.....N
+00001d90: 0045 0069 006e 0020 0041 0044 0049 0046  .E.i.n. .A.D.I.F
+00001da0: 002d 0046 0065 006c 0064 0020 0066 0065  .-.F.e.l.d. .f.e
+00001db0: 0068 006c 0074 0020 0066 00fc 0072 0020  .h.l.t. .f...r. 
+00001dc0: 0064 0065 006e 0020 004c 006f 0054 0057  .d.e.n. .L.o.T.W
+00001dd0: 002d 0055 0070 006c 006f 0061 0064 0800  .-.U.p.l.o.a.d..
+00001de0: 0000 0006 0000 001d 4120 6669 656c 6420  ........A field 
+00001df0: 6973 206d 6973 7369 6e67 2066 6f72 2075  is missing for u
+00001e00: 706c 6f61 6407 0000 0009 4472 6167 6f6e  pload.....Dragon
+00001e10: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+00001e20: 0000 1541 4449 4620 3320 282a 2e61 6469  ...ADIF 3 (*.adi
+00001e30: 202a 2e61 6469 6629 0700 0000 0944 7261   *.adif).....Dra
+00001e40: 676f 6e4c 6f67 0103 ffff ffff 0800 0000  gonLog..........
+00001e50: 0006 0000 001b 4144 4946 2033 2028 2a2e  ......ADIF 3 (*.
+00001e60: 6164 7820 2a2e 6164 6920 2a2e 6164 6966  adx *.adi *.adif
+00001e70: 2907 0000 0009 4472 6167 6f6e 4c6f 6701  ).....DragonLog.
+00001e80: 0300 0000 0800 dc00 6200 6500 7208 0000  ........b.e.r...
+00001e90: 0000 0600 0000 0541 626f 7574 0700 0000  .......About....
+00001ea0: 0944 7261 676f 6e4c 6f67 0103 0000 000e  .DragonLog......
+00001eb0: 00dc 0062 0065 0072 0020 0051 0074 0800  ...b.e.r. .Q.t..
+00001ec0: 0000 0006 0000 0008 4162 6f75 7420 5174  ........About Qt
+00001ed0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00001ee0: 0000 0020 0041 0069 0072 0063 0072 0061  ... .A.i.r.c.r.a
+00001ef0: 0066 0074 002d 0053 0063 0061 0074 0074  .f.t.-.S.c.a.t.t
+00001f00: 0065 0072 0800 0000 0006 0000 0010 4169  .e.r..........Ai
+00001f10: 7263 7261 6674 2053 6361 7474 6572 0700  rcraft Scatter..
+00001f20: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00001f30: 000e 0041 006e 0074 0065 006e 006e 0065  ...A.n.t.e.n.n.e
+00001f40: 0800 0000 0006 0000 0007 416e 7465 6e6e  ..........Antenn
+00001f50: 6107 0000 0009 4472 6167 6f6e 4c6f 6701  a.....DragonLog.
+00001f60: 03ff ffff ff08 0000 0000 0600 0000 0641  ...............A
+00001f70: 7572 6f72 6107 0000 0009 4472 6167 6f6e  urora.....Dragon
+00001f80: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+00001f90: 0000 0841 7572 6f72 612d 4507 0000 0009  ...Aurora-E.....
+00001fa0: 4472 6167 6f6e 4c6f 6701 0300 0000 0a00  DragonLog.......
+00001fb0: 4100 7500 7400 6f00 7208 0000 0000 0600  A.u.t.o.r.......
+00001fc0: 0000 0641 7574 686f 7207 0000 0009 4472  ...Author.....Dr
+00001fd0: 6167 6f6e 4c6f 6701 0300 0000 1800 4200  agonLog.......B.
+00001fe0: 6100 6300 6b00 2d00 5300 6300 6100 7400  a.c.k.-.S.c.a.t.
+00001ff0: 7400 6500 7208 0000 0000 0600 0000 0c42  t.e.r..........B
+00002000: 6163 6b20 7363 6174 7465 7207 0000 0009  ack scatter.....
+00002010: 4472 6167 6f6e 4c6f 6701 03ff ffff ff08  DragonLog.......
+00002020: 0000 0000 0600 0000 0442 616e 6407 0000  .........Band...
+00002030: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002040: 2200 4300 5300 5600 2d00 4400 6100 7400  ".C.S.V.-.D.a.t.
+00002050: 6500 6900 2000 2800 2a00 2e00 6300 7300  e.i. .(.*...c.s.
+00002060: 7600 2908 0000 0000 0600 0000 1043 5356  v.)..........CSV
+00002070: 2d46 696c 6520 282a 2e63 7376 2907 0000  -File (*.csv)...
+00002080: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002090: 1400 5200 7500 6600 7a00 6500 6900 6300  ..R.u.f.z.e.i.c.
+000020a0: 6800 6500 6e08 0000 0000 0600 0000 0943  h.e.n..........C
+000020b0: 616c 6c20 7369 676e 0700 0000 0944 7261  all sign.....Dra
+000020c0: 676f 6e4c 6f67 0103 0000 000a 004b 0061  gonLog.......K.a
+000020d0: 006e 0061 006c 0800 0000 0006 0000 0007  .n.a.l..........
+000020e0: 4368 616e 6e65 6c07 0000 0009 4472 6167  Channel.....Drag
+000020f0: 6f6e 4c6f 6701 0300 0000 7400 5000 7200  onLog.....t.P.r.
+00002100: fc00 6600 7500 6e00 6700 2000 6400 6500  ..f.u.n.g. .d.e.
+00002110: 7200 2000 4400 6100 7400 6500 6e00 6200  r. .D.a.t.e.n.b.
+00002120: 6100 6e00 6b00 2000 6600 6500 6800 6c00  a.n.k. .f.e.h.l.
+00002130: 6700 6500 7300 6300 6800 6c00 6100 6700  g.e.s.c.h.l.a.g.
+00002140: 6500 6e00 2e00 2000 4900 6e00 6800 6100  e.n... .I.n.h.a.
+00002150: 6c00 7400 2000 6e00 6900 6300 6800 7400  l.t. .n.i.c.h.t.
+00002160: 2000 6c00 6500 7300 6200 6100 7200 2e08   .l.e.s.b.a.r...
+00002170: 0000 0000 0600 0000 3443 6865 636b 696e  ........4Checkin
+00002180: 6720 6461 7461 6261 7365 2066 6169 6c65  g database faile
+00002190: 642e 2043 6f6e 7465 6e74 2069 7320 6e6f  d. Content is no
+000021a0: 7420 6163 6365 7373 6162 6c65 2e07 0000  t accessable....
+000021b0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+000021c0: 1200 4b00 6f00 6d00 6d00 6500 6e00 7400  ..K.o.m.m.e.n.t.
+000021d0: 6100 7208 0000 0000 0600 0000 0743 6f6d  a.r..........Com
+000021e0: 6d65 6e74 0700 0000 0944 7261 676f 6e4c  ment.....DragonL
+000021f0: 6f67 0103 0000 0060 0056 0065 0072 0062  og.....`.V.e.r.b
+00002200: 0069 006e 0064 0075 006e 0067 0073 0066  .i.n.d.u.n.g.s.f
+00002210: 0065 0068 006c 0065 0072 0020 006f 0064  .e.h.l.e.r. .o.d
+00002220: 0065 0072 0020 004e 0065 0074 007a 0077  .e.r. .N.e.t.z.w
+00002230: 0065 0072 006b 0020 006e 0069 0063 0068  .e.r.k. .n.i.c.h
+00002240: 0074 0020 0065 0072 0072 0065 0069 0063  .t. .e.r.r.e.i.c
+00002250: 0068 0062 0061 0072 0800 0000 0006 0000  .h.b.a.r........
+00002260: 0027 436f 6e6e 6563 7469 6f6e 2065 7272  .'Connection err
+00002270: 6f72 206f 7220 6e65 7477 6f72 6b20 756e  or or network un
+00002280: 7265 6163 6861 626c 6507 0000 0009 4472  reachable.....Dr
+00002290: 6167 6f6e 4c6f 6701 03ff ffff ff08 0000  agonLog.........
+000022a0: 0000 0600 0000 0743 6f6e 7465 7374 0700  .......Contest..
+000022b0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+000022c0: 002e 0044 0061 0074 0065 006e 0062 0061  ...D.a.t.e.n.b.a
+000022d0: 006e 006b 002d 0042 0061 0063 006b 0075  .n.k.-.B.a.c.k.u
+000022e0: 0070 0020 0046 0065 0068 006c 0065 0072  .p. .F.e.h.l.e.r
+000022f0: 0800 0000 0006 0000 0015 4461 7461 6261  ..........Databa
+00002300: 7365 2062 6163 6b75 7020 6572 726f 7207  se backup error.
+00002310: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002320: 0000 2c00 4400 6100 7400 6500 6e00 6200  ..,.D.a.t.e.n.b.
+00002330: 6100 6e00 6b00 6b00 6f00 6e00 7600 6500  a.n.k.k.o.n.v.e.
+00002340: 7200 7400 6900 6500 7200 7500 6e00 6708  r.t.i.e.r.u.n.g.
+00002350: 0000 0000 0600 0000 1344 6174 6162 6173  .........Databas
+00002360: 6520 636f 6e76 6572 7369 6f6e 0700 0000  e conversion....
+00002370: 0944 7261 676f 6e4c 6f67 0103 0000 0048  .DragonLog.....H
+00002380: 0044 0061 0074 0065 006e 0062 0061 006e  .D.a.t.e.n.b.a.n
+00002390: 006b 006b 006f 006e 0076 0065 0072 0074  .k.k.o.n.v.e.r.t
+000023a0: 0069 0065 0072 0075 006e 0067 0020 0061  .i.e.r.u.n.g. .a
+000023b0: 0062 0067 0065 0073 0063 0068 006c 006f  .b.g.e.s.c.h.l.o
+000023c0: 0073 0073 0065 006e 0800 0000 0006 0000  .s.s.e.n........
+000023d0: 001c 4461 7461 6261 7365 2063 6f6e 7665  ..Database conve
+000023e0: 7273 696f 6e20 6669 6e69 7368 6564 0700  rsion finished..
+000023f0: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00002400: 001e 0044 0061 0074 0065 006e 0062 0061  ...D.a.t.e.n.b.a
+00002410: 006e 006b 0066 0065 0068 006c 0065 0072  .n.k.f.e.h.l.e.r
+00002420: 0800 0000 0006 0000 000e 4461 7461 6261  ..........Databa
+00002430: 7365 2065 7272 6f72 0700 0000 0944 7261  se error.....Dra
+00002440: 676f 6e4c 6f67 0103 0000 0034 0044 0061  gonLog.....4.D.a
+00002450: 0074 0065 006e 0062 0061 006e 006b 0073  .t.e.n.b.a.n.k.s
+00002460: 0074 0072 0075 006b 0074 0075 0072 0020  .t.r.u.k.t.u.r. 
+00002470: 0076 0065 0072 0061 006c 0074 0065 0074  .v.e.r.a.l.t.e.t
+00002480: 0800 0000 0006 0000 001c 4461 7461 6261  ..........Databa
+00002490: 7365 2073 7472 7563 7475 7265 206f 7574  se structure out
+000024a0: 2d64 6174 6564 0700 0000 0944 7261 676f  -dated.....Drago
+000024b0: 6e4c 6f67 0103 0000 001e 0044 0061 0074  nLog.......D.a.t
+000024c0: 0075 006d 002f 005a 0065 0069 0074 0020  .u.m./.Z.e.i.t. 
+000024d0: 0045 006e 0064 0065 0800 0000 0006 0000  .E.n.d.e........
+000024e0: 000d 4461 7465 2f54 696d 6520 656e 6407  ..Date/Time end.
+000024f0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002500: 0000 2000 4400 6100 7400 7500 6d00 2f00  .. .D.a.t.u.m./.
+00002510: 5a00 6500 6900 7400 2000 5300 7400 6100  Z.e.i.t. .S.t.a.
+00002520: 7200 7408 0000 0000 0600 0000 0f44 6174  r.t..........Dat
+00002530: 652f 5469 6d65 2073 7461 7274 0700 0000  e/Time start....
+00002540: 0944 7261 676f 6e4c 6f67 0103 0000 0016  .DragonLog......
+00002550: 0051 0053 004f 0020 006c 00f6 0073 0063  .Q.S.O. .l...s.c
+00002560: 0068 0065 006e 0800 0000 0006 0000 000a  .h.e.n..........
+00002570: 4465 6c65 7465 2051 534f 0700 0000 0944  Delete QSO.....D
+00002580: 7261 676f 6e4c 6f67 0103 0000 0014 0045  ragonLog.......E
+00002590: 006e 0074 0066 0065 0072 006e 0075 006e  .n.t.f.e.r.n.u.n
+000025a0: 0067 0800 0000 0006 0000 0008 4469 7374  .g..........Dist
+000025b0: 616e 6365 0700 0000 0944 7261 676f 6e4c  ance.....DragonL
+000025c0: 6f67 0103 0000 0064 0057 006f 006c 006c  og.....d.W.o.l.l
+000025d0: 0065 006e 0020 0073 0069 0065 0020 0064  .e.n. .s.i.e. .d
+000025e0: 0069 0065 0020 0073 0065 006c 0065 006b  .i.e. .s.e.l.e.k
+000025f0: 0074 0069 0065 0072 0074 0065 006e 0020  .t.i.e.r.t.e.n. 
+00002600: 0051 0053 004f 0073 0020 0077 0069 0072  .Q.S.O.s. .w.i.r
+00002610: 006b 006c 0069 0063 0068 0020 006c 00f6  .k.l.i.c.h. .l..
+00002620: 0073 0063 0068 0065 006e 003f 0800 0000  .s.c.h.e.n.?....
+00002630: 0006 0000 0031 446f 2079 6f75 2072 6561  .....1Do you rea
+00002640: 6c6c 7920 7761 6e74 2074 6f20 6465 6c65  lly want to dele
+00002650: 7465 2074 6865 2073 656c 6563 7465 6420  te the selected 
+00002660: 5153 4f28 7329 3f07 0000 0009 4472 6167  QSO(s)?.....Drag
+00002670: 6f6e 4c6f 6701 03ff ffff ff08 0000 0000  onLog...........
+00002680: 0600 0000 1045 6172 7468 2d4d 6f6f 6e2d  .....Earth-Moon-
+00002690: 4561 7274 6807 0000 0009 4472 6167 6f6e  Earth.....Dragon
+000026a0: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+000026b0: 0000 0845 6368 6f4c 696e 6b07 0000 0009  ...EchoLink.....
+000026c0: 4472 6167 6f6e 4c6f 6701 0300 0000 0c00  DragonLog.......
+000026d0: 4600 6500 6800 6c00 6500 7208 0000 0000  F.e.h.l.e.r.....
+000026e0: 0600 0000 0545 7272 6f72 0700 0000 0944  .....Error.....D
+000026f0: 7261 676f 6e4c 6f67 0103 0000 0028 0045  ragonLog.....(.E
+00002700: 0078 0063 0065 006c 002d 0044 0061 0074  .x.c.e.l.-.D.a.t
+00002710: 0065 0069 0020 0028 002a 002e 0078 006c  .e.i. .(.*...x.l
+00002720: 0073 0078 0029 0800 0000 0006 0000 0013  .s.x.)..........
+00002730: 4578 6365 6c2d 4669 6c65 2028 2a2e 786c  Excel-File (*.xl
+00002740: 7378 2907 0000 0009 4472 6167 6f6e 4c6f  sx).....DragonLo
+00002750: 6701 0300 0000 2400 4500 7800 7000 6f00  g.....$.E.x.p.o.
+00002760: 7200 7400 6900 6500 7200 6500 2000 5100  r.t.i.e.r.e. .Q.
+00002770: 5300 4f00 2000 6c00 6f00 6708 0000 0000  S.O. .l.o.g.....
+00002780: 0600 0000 1045 7870 6f72 7465 6420 5153  .....Exported QS
+00002790: 4f20 6c6f 6707 0000 0009 4472 6167 6f6e  O log.....Dragon
+000027a0: 4c6f 6701 0300 0000 1a00 4600 3200 2d00  Log.......F.2.-.
+000027b0: 5200 6500 6600 6c00 6500 6b00 7400 6900  R.e.f.l.e.k.t.i.
+000027c0: 6f00 6e08 0000 0000 0600 0000 0d46 3220  o.n..........F2 
+000027d0: 5265 666c 6563 7469 6f6e 0700 0000 0944  Reflection.....D
+000027e0: 7261 676f 6e4c 6f67 0103 0000 0038 0046  ragonLog.....8.F
+000027f0: 0069 0065 006c 0064 002d 0041 006c 0069  .i.e.l.d.-.A.l.i
+00002800: 0067 006e 0065 0064 002d 0049 0072 0072  .g.n.e.d.-.I.r.r
+00002810: 0065 0067 0075 006c 0061 0072 0069 0074  .e.g.u.l.a.r.i.t
+00002820: 0069 0065 0073 0800 0000 0006 0000 001c  .i.e.s..........
+00002830: 4669 656c 6420 416c 6967 6e65 6420 4972  Field Aligned Ir
+00002840: 7265 6775 6c61 7269 7469 6573 0700 0000  regularities....
+00002850: 0944 7261 676f 6e4c 6f67 0103 0000 0010  .DragonLog......
+00002860: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
+00002870: 0800 0000 0006 0000 0009 4672 6571 7565  ..........Freque
+00002880: 6e63 7907 0000 0009 4472 6167 6f6e 4c6f  ncy.....DragonLo
+00002890: 6701 0300 0000 1400 4200 6f00 6400 6500  g.......B.o.d.e.
+000028a0: 6e00 7700 6500 6c00 6c00 6508 0000 0000  n.w.e.l.l.e.....
+000028b0: 0600 0000 0b47 726f 756e 6420 5761 7665  .....Ground Wave
+000028c0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+000028d0: ffff ffff 0800 0000 0006 0000 0006 4861  ..............Ha
+000028e0: 6d51 5448 0700 0000 0944 7261 676f 6e4c  mQTH.....DragonL
+000028f0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00002900: 0006 4861 6d6c 6962 0700 0000 0944 7261  ..Hamlib.....Dra
+00002910: 676f 6e4c 6f67 0103 0000 000a 0048 0069  gonLog.......H.i
+00002920: 006c 0066 0065 0800 0000 0006 0000 0004  .l.f.e..........
+00002930: 4865 6c70 0700 0000 0944 7261 676f 6e4c  Help.....DragonL
+00002940: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00002950: 0004 4952 4c50 0700 0000 0944 7261 676f  ..IRLP.....Drago
+00002960: 6e4c 6f67 0103 0000 0026 0049 006e 0074  nLog.....&.I.n.t
+00002970: 0065 0072 006e 0065 0074 0075 006e 0074  .e.r.n.e.t.u.n.t
+00002980: 0065 0072 0073 0074 00fc 0074 007a 0074  .e.r.s.t...t.z.t
+00002990: 0800 0000 0006 0000 0011 496e 7465 726e  ..........Intern
+000029a0: 6574 2d61 7373 6973 7465 6407 0000 0009  et-assisted.....
+000029b0: 4472 6167 6f6e 4c6f 6701 0300 0000 1800  DragonLog.......
+000029c0: 4900 6f00 6e00 6f00 2d00 5300 6300 6100  I.o.n.o.-.S.c.a.
+000029d0: 7400 7400 6500 7208 0000 0000 0600 0000  t.t.e.r.........
+000029e0: 0b49 6f6e 6f73 6361 7474 6572 0700 0000  .Ionoscatter....
+000029f0: 0944 7261 676f 6e4c 6f67 0103 0000 0020  .DragonLog..... 
+00002a00: 006c 0065 0074 007a 0074 0065 0073 0020  .l.e.t.z.t.e.s. 
+00002a10: 0048 0061 006c 0062 006a 0061 0068 0072  .H.a.l.b.j.a.h.r
+00002a20: 0800 0000 0006 0000 000e 4c61 7374 2068  ..........Last h
+00002a30: 616c 6620 7965 6172 0700 0000 0944 7261  alf year.....Dra
+00002a40: 676f 6e4c 6f67 0103 0000 001a 006c 0065  gonLog.......l.e
+00002a50: 0074 007a 0074 0065 006e 0020 004d 006f  .t.z.t.e.n. .M.o
+00002a60: 006e 0061 0074 0800 0000 0006 0000 000a  .n.a.t..........
+00002a70: 4c61 7374 206d 6f6e 7468 0700 0000 0944  Last month.....D
+00002a80: 7261 676f 6e4c 6f67 0103 0000 0018 006c  ragonLog.......l
+00002a90: 0065 0074 007a 0074 0065 0020 0057 006f  .e.t.z.t.e. .W.o
+00002aa0: 0063 0068 0065 0800 0000 0006 0000 0009  .c.h.e..........
+00002ab0: 4c61 7374 2077 6565 6b07 0000 0009 4472  Last week.....Dr
+00002ac0: 6167 6f6e 4c6f 6701 0300 0000 1800 6c00  agonLog.......l.
+00002ad0: 6500 7400 7a00 7400 6500 7300 2000 4a00  e.t.z.t.e.s. .J.
+00002ae0: 6100 6800 7208 0000 0000 0600 0000 094c  a.h.r..........L
+00002af0: 6173 7420 7965 6172 0700 0000 0944 7261  ast year.....Dra
+00002b00: 676f 6e4c 6f67 0103 0000 001e 0053 0069  gonLog.......S.i
+00002b10: 0063 0068 0074 0076 0065 0072 0062 0069  .c.h.t.v.e.r.b.i
+00002b20: 006e 0064 0075 006e 0067 0800 0000 0006  .n.d.u.n.g......
+00002b30: 0000 000d 4c69 6e65 206f 6620 5369 6768  ....Line of Sigh
+00002b40: 7407 0000 0009 4472 6167 6f6e 4c6f 6701  t.....DragonLog.
+00002b50: 0300 0000 2000 4c00 6f00 5400 5700 2d00  .... .L.o.T.W.-.
+00002b60: 4100 4400 4900 4600 2d00 5500 7000 6c00  A.D.I.F.-.U.p.l.
+00002b70: 6f00 6100 6408 0000 0000 0600 0000 104c  o.a.d..........L
+00002b80: 6f54 5720 4144 4946 2075 706c 6f61 6407  oTW ADIF upload.
+00002b90: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002ba0: 0000 1400 4c00 6f00 5400 5700 2000 6500  ....L.o.T.W. .e.
+00002bb0: 6d00 7000 6600 2e08 0000 0000 0600 0000  m.p.f...........
+00002bc0: 094c 6f54 5720 7263 7664 0700 0000 0944  .LoTW rcvd.....D
+00002bd0: 7261 676f 6e4c 6f67 0103 0000 0014 004c  ragonLog.......L
+00002be0: 006f 0054 0057 0020 0076 0065 0072 0073  .o.T.W. .v.e.r.s
+00002bf0: 002e 0800 0000 0006 0000 0009 4c6f 5457  ............LoTW
+00002c00: 2073 656e 7407 0000 0009 4472 6167 6f6e   sent.....Dragon
+00002c10: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+00002c20: 0000 074c 6f63 6174 6f72 0700 0000 0944  ...Locator.....D
+00002c30: 7261 676f 6e4c 6f67 0103 ffff ffff 0800  ragonLog........
+00002c40: 0000 0006 0000 000f 4c6f 6720 696d 706f  ........Log impo
+00002c50: 7274 2041 4449 4607 0000 0009 4472 6167  rt ADIF.....Drag
+00002c60: 6f6e 4c6f 6701 0300 0000 1c00 4c00 6f00  onLog.......L.o.
+00002c70: 6700 2000 4900 6d00 7000 6f00 7200 7400  g. .I.m.p.o.r.t.
+00002c80: 2000 4300 5300 5608 0000 0000 0600 0000   .C.S.V.........
+00002c90: 0e4c 6f67 2069 6d70 6f72 7420 4353 5607  .Log import CSV.
+00002ca0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002cb0: 0000 2000 4c00 6f00 6700 2000 4900 6d00  .. .L.o.g. .I.m.
+00002cc0: 7000 6f00 7200 7400 2000 4500 7800 6300  p.o.r.t. .E.x.c.
+00002cd0: 6500 6c08 0000 0000 0600 0000 104c 6f67  e.l..........Log
+00002ce0: 2069 6d70 6f72 7420 4578 6365 6c07 0000   import Excel...
+00002cf0: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00002d00: 1c00 4d00 6500 7400 6500 6f00 7200 2d00  ..M.e.t.e.o.r.-.
+00002d10: 5300 6300 6100 7400 7400 6500 7208 0000  S.c.a.t.t.e.r...
+00002d20: 0000 0600 0000 0e4d 6574 656f 7220 7363  .......Meteor sc
+00002d30: 6174 7465 7207 0000 0009 4472 6167 6f6e  atter.....Dragon
+00002d40: 4c6f 6701 0300 0000 5a00 4b00 6500 6900  Log.....Z.K.e.i.
+00002d50: 6e00 6500 2000 5300 7400 6100 7400 6900  n.e. .S.t.a.t.i.
+00002d60: 6f00 6e00 7300 6b00 6f00 6e00 6600 6900  o.n.s.k.o.n.f.i.
+00002d70: 6700 7500 7200 6100 7400 6900 6f00 6e00  g.u.r.a.t.i.o.n.
+00002d80: 2000 6900 6e00 2000 5400 5100 5300 4c00   .i.n. .T.Q.S.L.
+00002d90: 2000 7600 6500 7200 6600 fc00 6700 6200   .v.e.r.f...g.b.
+00002da0: 6100 7208 0000 0000 0600 0000 254d 6973  a.r.........%Mis
+00002db0: 7369 6e67 2073 7461 7469 6f6e 2063 6f6e  sing station con
+00002dc0: 6669 6775 7261 7469 6f6e 2069 6e20 5451  figuration in TQ
+00002dd0: 534c 0700 0000 0944 7261 676f 6e4c 6f67  SL.....DragonLog
+00002de0: 0103 ffff ffff 0800 0000 0006 0000 0004  ................
+00002df0: 4d6f 6465 0700 0000 0944 7261 676f 6e4c  Mode.....DragonL
+00002e00: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+00002e10: 0004 4e61 6d65 0700 0000 0944 7261 676f  ..Name.....Drago
+00002e20: 6e4c 6f67 0103 0000 0034 004b 0065 0069  nLog.....4.K.e.i
+00002e30: 006e 0065 0020 0051 0053 004f 0073 0020  .n.e. .Q.S.O.s. 
+00002e40: 0066 00fc 0072 0020 0064 0065 006e 0020  .f...r. .d.e.n. 
+00002e50: 004c 006f 0063 0061 0074 006f 0072 0800  .L.o.c.a.t.o.r..
+00002e60: 0000 0006 0000 0017 4e6f 2072 6563 6f72  ........No recor
+00002e70: 6473 2066 6f72 206c 6f63 6174 696f 6e07  ds for location.
+00002e80: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002e90: 0000 0e00 4e00 6f00 7400 6900 7a00 6500  ....N.o.t.i.z.e.
+00002ea0: 6e08 0000 0000 0600 0000 054e 6f74 6573  n..........Notes
+00002eb0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002ec0: ffff ffff 0800 0000 0006 0000 0002 4f6b  ..............Ok
+00002ed0: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002ee0: 0000 001e 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
+00002ef0: 0072 0020 004c 006f 0063 0061 0074 006f  .r. .L.o.c.a.t.o
+00002f00: 0072 0800 0000 0006 0000 000b 4f77 6e20  .r..........Own 
+00002f10: 4c6f 6361 746f 7207 0000 0009 4472 6167  Locator.....Drag
+00002f20: 6f6e 4c6f 6701 0300 0000 1800 4500 6900  onLog.......E.i.
+00002f30: 6700 6500 6e00 6500 7200 2000 4e00 6100  g.e.n.e.r. .N.a.
+00002f40: 6d00 6508 0000 0000 0600 0000 084f 776e  m.e..........Own
+00002f50: 204e 616d 6507 0000 0009 4472 6167 6f6e   Name.....Dragon
+00002f60: 4c6f 6701 0300 0000 1600 4500 6900 6700  Log.......E.i.g.
+00002f70: 6500 6e00 6500 7200 2000 5100 5400 4808  e.n.e.r. .Q.T.H.
+00002f80: 0000 0000 0600 0000 074f 776e 2051 5448  .........Own QTH
+00002f90: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00002fa0: 0000 0024 0045 0069 0067 0065 006e 0065  ...$.E.i.g.e.n.e
+00002fb0: 0073 0020 0052 0075 0066 007a 0065 0069  .s. .R.u.f.z.e.i
+00002fc0: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+00002fd0: 000d 4f77 6e20 6361 6c6c 2073 6967 6e07  ..Own call sign.
+00002fe0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+00002ff0: 0000 1000 4c00 6500 6900 7300 7400 7500  ....L.e.i.s.t.u.
+00003000: 6e00 6708 0000 0000 0600 0000 0550 6f77  n.g..........Pow
+00003010: 6572 0700 0000 0944 7261 676f 6e4c 6f67  er.....DragonLog
+00003020: 0103 0000 0016 0041 0075 0073 0062 0072  .......A.u.s.b.r
+00003030: 0065 0069 0074 0075 006e 0067 0800 0000  .e.i.t.u.n.g....
+00003040: 0006 0000 000b 5072 6f70 6167 6174 696f  ......Propagatio
+00003050: 6e07 0000 0009 4472 6167 6f6e 4c6f 6701  n.....DragonLog.
+00003060: 0300 0000 1a00 5100 5300 4c00 2d00 4e00  ......Q.S.L.-.N.
+00003070: 6100 6300 6800 7200 6900 6300 6800 7408  a.c.h.r.i.c.h.t.
+00003080: 0000 0000 0600 0000 0b51 534c 206d 6573  .........QSL mes
+00003090: 7361 6765 0700 0000 0944 7261 676f 6e4c  sage.....DragonL
+000030a0: 6f67 0103 0000 0010 0051 0053 004c 002d  og.......Q.S.L.-
+000030b0: 0050 0066 0061 0064 0800 0000 0006 0000  .P.f.a.d........
+000030c0: 0008 5153 4c20 7061 7468 0700 0000 0944  ..QSL path.....D
+000030d0: 7261 676f 6e4c 6f67 0103 0000 0012 0051  ragonLog.......Q
+000030e0: 0053 004c 0020 0065 006d 0070 0066 002e  .S.L. .e.m.p.f..
+000030f0: 0800 0000 0006 0000 0008 5153 4c20 7263  ..........QSL rc
+00003100: 7664 0700 0000 0944 7261 676f 6e4c 6f67  vd.....DragonLog
+00003110: 0103 0000 0012 0051 0053 004c 0020 0076  .......Q.S.L. .v
+00003120: 0065 0072 0073 002e 0800 0000 0006 0000  .e.r.s..........
+00003130: 0008 5153 4c20 7365 6e74 0700 0000 0944  ..QSL sent.....D
+00003140: 7261 676f 6e4c 6f67 0103 0000 000e 0051  ragonLog.......Q
+00003150: 0053 004c 002d 0056 0069 0061 0800 0000  .S.L.-.V.i.a....
+00003160: 0006 0000 0007 5153 4c20 7669 6107 0000  ......QSL via...
+00003170: 0009 4472 6167 6f6e 4c6f 6701 03ff ffff  ..DragonLog.....
+00003180: ff08 0000 0000 0600 0000 0351 534f 0700  ...........QSO..
+00003190: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+000031a0: 0048 0051 0053 004f 002d 004c 006f 0067  .H.Q.S.O.-.L.o.g
+000031b0: 0020 0028 002a 002e 0071 006c 006f 0067  . .(.*...q.l.o.g
+000031c0: 0029 003b 003b 0041 006c 006c 0065 0020  .).;.;.A.l.l.e. 
+000031d0: 0044 0061 0074 0065 0069 0065 006e 0020  .D.a.t.e.i.e.n. 
+000031e0: 0028 002a 002e 002a 0029 0800 0000 0006  .(.*...*.)......
+000031f0: 0000 0021 5153 4f2d 4c6f 6720 282a 2e71  ...!QSO-Log (*.q
+00003200: 6c6f 6729 3b3b 416c 6c20 4669 6c65 7320  log);;All Files 
+00003210: 282a 2e2a 2907 0000 0009 4472 6167 6f6e  (*.*).....Dragon
+00003220: 4c6f 6701 03ff ffff ff08 0000 0000 0600  Log.............
+00003230: 0000 0351 5448 0700 0000 0944 7261 676f  ...QTH.....Drago
+00003240: 6e4c 6f67 0103 0000 0012 0052 0053 0054  nLog.......R.S.T
+00003250: 0020 0065 006d 0070 0066 002e 0800 0000  . .e.m.p.f......
+00003260: 0006 0000 0008 5253 5420 7263 7664 0700  ......RST rcvd..
+00003270: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003280: 0010 0052 0053 0054 0020 0067 0065 0073  ...R.S.T. .g.e.s
+00003290: 002e 0800 0000 0006 0000 0008 5253 5420  ............RST 
+000032a0: 7365 6e74 0700 0000 0944 7261 676f 6e4c  sent.....DragonL
+000032b0: 6f67 0103 ffff ffff 0800 0000 0006 0000  og..............
+000032c0: 0005 5261 6469 6f07 0000 0009 4472 6167  ..Radio.....Drag
+000032d0: 6f6e 4c6f 6701 0300 0000 1800 5200 6100  onLog.......R.a.
+000032e0: 6900 6e00 2d00 5300 6300 6100 7400 7400  i.n.-.S.c.a.t.t.
+000032f0: 6500 7208 0000 0000 0600 0000 0c52 6169  e.r..........Rai
+00003300: 6e20 7363 6174 7465 7207 0000 0009 4472  n scatter.....Dr
+00003310: 6167 6f6e 4c6f 6701 0300 0000 3200 5200  agonLog.....2.R.
+00003320: 6500 7000 6500 6100 7400 6500 7200 2000  e.p.e.a.t.e.r. .
+00003330: 6f00 6400 6500 7200 2000 5400 7200 6100  o.d.e.r. .T.r.a.
+00003340: 6e00 7300 7000 6f00 6e00 6400 6500 7208  n.s.p.o.n.d.e.r.
+00003350: 0000 0000 0600 0000 1752 6570 6561 7465  .........Repeate
+00003360: 7220 6f72 2054 7261 6e73 706f 6e64 6572  r or Transponder
+00003370: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003380: 0000 0018 0045 006d 0070 0066 002e 0020  .....E.m.p.f... 
+00003390: 0051 0053 004f 0020 0049 0044 0800 0000  .Q.S.O. .I.D....
+000033a0: 0006 0000 0009 5278 2051 534f 2049 4407  ......Rx QSO ID.
+000033b0: 0000 0009 4472 6167 6f6e 4c6f 6701 0300  ....DragonLog...
+000033c0: 0000 1600 4500 6d00 7000 6600 2e00 2000  ....E.m.p.f... .
+000033d0: 4400 6100 7400 6500 6e08 0000 0000 0600  D.a.t.e.n.......
+000033e0: 0000 0752 7820 6461 7461 0700 0000 0944  ...Rx data.....D
+000033f0: 7261 676f 6e4c 6f67 0103 0000 0010 0053  ragonLog.......S
+00003400: 0061 0074 0065 006c 006c 0069 0074 0800  .a.t.e.l.l.i.t..
+00003410: 0000 0006 0000 0009 5361 7465 6c6c 6974  ........Satellit
+00003420: 6507 0000 0009 4472 6167 6f6e 4c6f 6701  e.....DragonLog.
+00003430: 0300 0000 2a00 4500 7800 7000 6f00 7200  ....*.E.x.p.o.r.
+00003440: 7400 6400 6100 7400 6500 6900 2000 7300  t.d.a.t.e.i. .s.
+00003450: 7000 6500 6900 6300 6800 6500 7200 6e08  p.e.i.c.h.e.r.n.
+00003460: 0000 0000 0600 0000 1253 656c 6563 7420  .........Select 
+00003470: 6578 706f 7274 2066 696c 6507 0000 0009  export file.....
+00003480: 4472 6167 6f6e 4c6f 6701 0300 0000 2000  DragonLog..... .
+00003490: 4400 6100 7400 6500 6e00 6200 6100 6e00  D.a.t.e.n.b.a.n.
+000034a0: 6b00 2000 f600 6600 6600 6e00 6500 6e08  k. ...f.f.n.e.n.
+000034b0: 0000 0000 0600 0000 0b53 656c 6563 7420  .........Select 
+000034c0: 6669 6c65 0700 0000 0944 7261 676f 6e4c  file.....DragonL
+000034d0: 6f67 0103 0000 0038 005a 0075 0020 00fc  og.....8.Z.u. ..
+000034e0: 0062 0065 0072 0077 0061 0063 0068 0065  .b.e.r.w.a.c.h.e
+000034f0: 006e 0064 0065 0020 0044 0061 0074 0065  .n.d.e. .D.a.t.e
+00003500: 0069 0020 0077 00e4 0068 006c 0065 006e  .i. .w...h.l.e.n
+00003510: 0800 0000 0006 0000 0014 5365 6c65 6374  ..........Select
+00003520: 2066 696c 6520 746f 2077 6174 6368 0700   file to watch..
+00003530: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003540: 0024 0049 006d 0070 006f 0072 0074 0064  .$.I.m.p.o.r.t.d
+00003550: 0061 0074 0065 0069 0020 00f6 0066 0066  .a.t.e.i. ...f.f
+00003560: 006e 0065 006e 0800 0000 0006 0000 0012  .n.e.n..........
+00003570: 5365 6c65 6374 2069 6d70 6f72 7420 6669  Select import fi
+00003580: 6c65 0700 0000 0944 7261 676f 6e4c 6f67  le.....DragonLog
+00003590: 0103 0000 001a 0057 00e4 0068 006c 0065  .......W...h.l.e
+000035a0: 0020 0053 0074 0061 0074 0069 006f 006e  . .S.t.a.t.i.o.n
+000035b0: 0800 0000 0006 0000 000e 5365 6c65 6374  ..........Select
+000035c0: 2073 7461 7469 6f6e 0700 0000 0944 7261   station.....Dra
+000035d0: 676f 6e4c 6f67 0103 0000 0044 004c 006f  gonLog.....D.L.o
+000035e0: 0054 0057 002d 0053 0065 0072 0076 0065  .T.W.-.S.e.r.v.e
+000035f0: 0072 0020 0068 0061 0074 0020 0064 0061  .r. .h.a.t. .d.a
+00003600: 0073 0020 004c 006f 0067 0020 0061 0062  .s. .L.o.g. .a.b
+00003610: 0067 0065 0077 0069 0065 0073 0065 006e  .g.e.w.i.e.s.e.n
+00003620: 0800 0000 0006 0000 0013 5365 7276 6572  ..........Server
+00003630: 2072 656a 6563 7465 6420 6c6f 6707 0000   rejected log...
+00003640: 0009 4472 6167 6f6e 4c6f 6701 0300 0000  ..DragonLog.....
+00003650: 1400 7a00 6500 6900 6700 6500 2000 6100  ..z.e.i.g.e. .a.
+00003660: 6c00 6c00 6508 0000 0000 0600 0000 0853  l.l.e..........S
+00003670: 686f 7720 616c 6c07 0000 0009 4472 6167  how all.....Drag
+00003680: 6f6e 4c6f 6701 0300 0000 1400 5300 7000  onLog.......S.p.
+00003690: 6f00 7200 6100 6400 6900 6300 2d00 4508  o.r.a.d.i.c.-.E.
+000036a0: 0000 0000 0600 0000 0a53 706f 7261 6469  .........Sporadi
+000036b0: 6320 4507 0000 0009 4472 6167 6f6e 4c6f  c E.....DragonLo
+000036c0: 6701 03ff ffff ff08 0000 0000 0600 0000  g...............
+000036d0: 0753 7562 6d6f 6465 0700 0000 0944 7261  .Submode.....Dra
+000036e0: 676f 6e4c 6f67 0103 0000 002a 0054 0051  gonLog.....*.T.Q
+000036f0: 0053 004c 002d 0053 0069 0067 006e 0061  .S.L.-.S.i.g.n.a
+00003700: 0074 0075 0072 0070 0061 0073 0073 0077  .t.u.r.p.a.s.s.w
+00003710: 006f 0072 0074 0800 0000 0006 0000 0017  .o.r.t..........
+00003720: 5451 534c 2073 6967 6e61 7475 7265 2070  TQSL signature p
+00003730: 6173 7377 6f72 6407 0000 0009 4472 6167  assword.....Drag
+00003740: 6f6e 4c6f 6701 0300 0000 b200 4400 6900  onLog.......D.i.
+00003750: 6500 2000 4400 6100 7400 6500 6e00 6200  e. .D.a.t.e.n.b.
+00003760: 6100 6e00 6b00 7300 7400 7200 7500 6b00  a.n.k.s.t.r.u.k.
+00003770: 7400 7500 7200 2000 6900 7300 7400 2000  t.u.r. .i.s.t. .
+00003780: 7600 6500 7200 6100 6c00 7400 6500 7400  v.e.r.a.l.t.e.t.
+00003790: 2000 7500 6e00 6400 2000 6d00 7500 7300   .u.n.d. .m.u.s.
+000037a0: 7300 2000 6b00 6f00 6e00 7600 6500 7200  s. .k.o.n.v.e.r.
+000037b0: 7400 6900 6500 7200 7400 2000 7700 6500  t.i.e.r.t. .w.e.
+000037c0: 7200 6400 6500 6e00 0a00 0a00 4500 6900  r.d.e.n.....E.i.
+000037d0: 6e00 2000 4200 6100 6300 6b00 7500 7000  n. .B.a.c.k.u.p.
+000037e0: 2000 7700 6900 7200 6400 2000 6500 7200   .w.i.r.d. .e.r.
+000037f0: 7300 7400 6500 6c00 6c00 7400 3a08 0000  s.t.e.l.l.t.:...
+00003800: 0000 0600 0000 5754 6865 2064 6174 6162  ......WThe datab
+00003810: 6173 6520 7374 7275 6374 7572 6520 6973  ase structure is
+00003820: 206f 7574 2d64 6174 6564 2061 6e64 206e   out-dated and n
+00003830: 6565 6473 2061 2063 6f6e 7665 7273 696f  eeds a conversio
+00003840: 6e0a 0a41 2062 6163 6b75 7020 7769 6c6c  n..A backup will
+00003850: 2062 6520 6765 6e65 7261 7465 643a 0700   be generated:..
+00003860: 0000 0944 7261 676f 6e4c 6f67 0103 0000  ...DragonLog....
+00003870: 001e 0054 0072 0061 006e 0073 0065 0071  ...T.r.a.n.s.e.q
+00003880: 0075 0061 0074 006f 0072 0069 0061 006c  .u.a.t.o.r.i.a.l
+00003890: 0800 0000 0006 0000 0010 5472 616e 732d  ..........Trans-
+000038a0: 6571 7561 746f 7269 616c 0700 0000 0944  equatorial.....D
+000038b0: 7261 676f 6e4c 6f67 0103 0000 0028 0054  ragonLog.....(.T
+000038c0: 0072 006f 0070 006f 0073 0070 0068 0065  .r.o.p.o.s.p.h.e
+000038d0: 0072 0069 0063 002d 0044 0075 0063 0074  .r.i.c.-.D.u.c.t
+000038e0: 0069 006e 0067 0800 0000 0006 0000 0014  .i.n.g..........
+000038f0: 5472 6f70 6f73 7068 6572 6963 2064 7563  Tropospheric duc
+00003900: 7469 6e67 0700 0000 0944 7261 676f 6e4c  ting.....DragonL
+00003910: 6f67 0103 0000 0016 0047 0065 0073 002e  og.......G.e.s..
+00003920: 0020 0051 0053 004f 0020 0049 0044 0800  . .Q.S.O. .I.D..
+00003930: 0000 0006 0000 0009 5478 2051 534f 2049  ........Tx QSO I
+00003940: 4407 0000 0009 4472 6167 6f6e 4c6f 6701  D.....DragonLog.
+00003950: 03ff ffff ff08 0000 0000 0600 0000 0756  ...............V
+00003960: 6572 7369 6f6e 0700 0000 0944 7261 676f  ersion.....Drago
+00003970: 6e4c 6f67 0103 0000 002c 0050 0072 006f  nLog.....,.P.r.o
+00003980: 0067 0072 0061 006d 006d 006c 006f 0067  .g.r.a.m.m.l.o.g
+00003990: 0020 00fc 0062 0065 0072 0077 0061 0063  . ...b.e.r.w.a.c
+000039a0: 0068 0065 006e 0800 0000 0006 0000 0015  .h.e.n..........
+000039b0: 5761 7463 6820 6170 706c 6963 6174 696f  Watch applicatio
+000039c0: 6e20 6c6f 6707 0000 0009 4472 6167 6f6e  n log.....Dragon
+000039d0: 4c6f 6701 0300 0000 2000 4400 6100 7400  Log..... .D.a.t.
+000039e0: 6500 6900 fc00 6200 6500 7200 7700 6100  e.i...b.e.r.w.a.
+000039f0: 6300 6800 7500 6e00 6708 0000 0000 0600  c.h.u.n.g.......
+00003a00: 0000 0d57 6174 6368 696e 6720 6669 6c65  ...Watching file
+00003a10: 0700 0000 0944 7261 676f 6e4c 6f67 0103  .....DragonLog..
+00003a20: 0000 0014 0065 0051 0053 004c 0020 0065  .....e.Q.S.L. .e
+00003a30: 006d 0070 0066 002e 0800 0000 0006 0000  .m.p.f..........
+00003a40: 0009 6551 534c 2072 6376 6407 0000 0009  ..eQSL rcvd.....
+00003a50: 4472 6167 6f6e 4c6f 6701 0300 0000 1400  DragonLog.......
+00003a60: 6500 5100 5300 4c00 2000 7600 6500 7200  e.Q.S.L. .v.e.r.
+00003a70: 7300 2e08 0000 0000 0600 0000 0965 5153  s............eQS
+00003a80: 4c20 7365 6e74 0700 0000 0944 7261 676f  L sent.....Drago
+00003a90: 6e4c 6f67 0103 0000 000e 0069 006e 0061  nLog.......i.n.a
+00003aa0: 006b 0074 0069 0076 0800 0000 0006 0000  .k.t.i.v........
+00003ab0: 0007 696e 6163 7469 7607 0000 0009 4472  ..inactiv.....Dr
+00003ac0: 6167 6f6e 4c6f 6701 0300 0000 0c00 2800  agonLog.......(.
+00003ad0: 6c00 6500 6500 7200 2908 0000 0000 0600  l.e.e.r.).......
+00003ae0: 0000 0728 656d 7074 7929 0700 0000 084c  ...(empty).....L
+00003af0: 6973 7445 6469 7401 03ff ffff ff08 0000  istEdit.........
+00003b00: 0000 0600 0000 0446 6f72 6d07 0000 000c  .......Form.....
+00003b10: 4c69 7374 4564 6974 466f 726d 0103 ffff  ListEditForm....
+00003b20: ffff 0800 0000 0006 0000 0005 4c61 6265  ............Labe
+00003b30: 6c07 0000 000c 4c69 7374 4564 6974 466f  l.....ListEditFo
+00003b40: 726d 0103 0000 0008 00dc 0062 0065 0072  rm.........b.e.r
+00003b50: 0800 0000 0006 0000 0005 4162 6f75 7407  ..........About.
+00003b60: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00003b70: 0000 000e 00dc 0062 0065 0072 0020 0051  .......b.e.r. .Q
+00003b80: 0074 0800 0000 0006 0000 0008 4162 6f75  .t..........Abou
+00003b90: 7420 5174 0700 0000 0a4d 6169 6e57 696e  t Qt.....MainWin
+00003ba0: 646f 7701 0300 0000 1a00 4100 6e00 7700  dow.......A.n.w.
+00003bb0: 6500 6e00 6400 7500 6e00 6700 7300 6c00  e.n.d.u.n.g.s.l.
+00003bc0: 6f00 6708 0000 0000 0600 0000 0f41 7070  o.g..........App
+00003bd0: 6c69 6361 7469 6f6e 204c 6f67 0700 0000  lication Log....
+00003be0: 0a4d 6169 6e57 696e 646f 7701 03ff ffff  .MainWindow.....
+00003bf0: ff08 0000 0000 0600 0000 0442 616e 6407  ...........Band.
+00003c00: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+00003c10: 0000 0014 0052 0075 0066 007a 0065 0069  .....R.u.f.z.e.i
+00003c20: 0063 0068 0065 006e 0800 0000 0006 0000  .c.h.e.n........
+00003c30: 0008 4361 6c6c 7369 676e 0700 0000 0a4d  ..Callsign.....M
+00003c40: 6169 6e57 696e 646f 7701 0300 0000 2200  ainWindow.....".
+00003c50: 4500 6900 6e00 7400 7200 6100 6700 2000  E.i.n.t.r.a.g. .
+00003c60: e400 6e00 6400 6500 7200 6e00 2e00 2e00  ..n.d.e.r.n.....
+00003c70: 2e08 0000 0000 0600 0000 1343 6861 6e67  ...........Chang
+00003c80: 6520 6c6f 6720 656e 7472 792e 2e2e 0700  e log entry.....
+00003c90: 0000 0a4d 6169 6e57 696e 646f 7701 03ff  ...MainWindow...
+00003ca0: ffff ff08 0000 0000 0600 0000 0643 7472  .............Ctr
+00003cb0: 6c2b 4507 0000 000a 4d61 696e 5769 6e64  l+E.....MainWind
+00003cc0: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003cd0: 0006 4374 726c 2b46 0700 0000 0a4d 6169  ..Ctrl+F.....Mai
+00003ce0: 6e57 696e 646f 7701 03ff ffff ff08 0000  nWindow.........
+00003cf0: 0000 0600 0000 0643 7472 6c2b 4c07 0000  .......Ctrl+L...
+00003d00: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00003d10: ffff 0800 0000 0006 0000 0006 4374 726c  ............Ctrl
+00003d20: 2b51 0700 0000 0a4d 6169 6e57 696e 646f  +Q.....MainWindo
+00003d30: 7701 03ff ffff ff08 0000 0000 0600 0000  w...............
+00003d40: 0643 7472 6c2b 5707 0000 000a 4d61 696e  .Ctrl+W.....Main
+00003d50: 5769 6e64 6f77 0103 ffff ffff 0800 0000  Window..........
+00003d60: 0006 0000 0006 4374 726c 2b58 0700 0000  ......Ctrl+X....
+00003d70: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
+00003d80: 1200 4400 6100 7400 7500 6d00 2000 7600  ..D.a.t.u.m. .v.
+00003d90: 6f00 6e08 0000 0000 0600 0000 0944 6174  o.n..........Dat
+00003da0: 6520 6672 6f6d 0700 0000 0a4d 6169 6e57  e from.....MainW
+00003db0: 696e 646f 7701 0300 0000 1200 4400 6100  indow.......D.a.
+00003dc0: 7400 7500 6d00 2000 6200 6900 7308 0000  t.u.m. .b.i.s...
+00003dd0: 0000 0600 0000 0744 6174 6520 746f 0700  .......Date to..
+00003de0: 0000 0a4d 6169 6e57 696e 646f 7701 0300  ...MainWindow...
+00003df0: 0000 1e00 4500 6900 6e00 7400 7200 6100  ....E.i.n.t.r.a.
+00003e00: 6700 2000 6c00 f600 7300 6300 6800 6500  g. .l...s.c.h.e.
+00003e10: 6e08 0000 0000 0600 0000 1044 656c 6574  n..........Delet
+00003e20: 6520 6c6f 6720 656e 7472 7907 0000 000a  e log entry.....
+00003e30: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
+00003e40: 0800 0000 0006 0000 0009 4472 6167 6f6e  ..........Dragon
+00003e50: 4c6f 6707 0000 000a 4d61 696e 5769 6e64  Log.....MainWind
+00003e60: 6f77 0103 0000 0014 0042 0065 0061 0072  ow.......B.e.a.r
+00003e70: 0062 0065 0069 0074 0065 006e 0800 0000  .b.e.i.t.e.n....
+00003e80: 0006 0000 0004 4564 6974 0700 0000 0a4d  ......Edit.....M
+00003e90: 6169 6e57 696e 646f 7701 0300 0000 0e00  ainWindow.......
+00003ea0: 4200 6500 6500 6e00 6400 6500 6e08 0000  B.e.e.n.d.e.n...
+00003eb0: 0000 0600 0000 0445 7869 7407 0000 000a  .......Exit.....
+00003ec0: 4d61 696e 5769 6e64 6f77 0103 ffff ffff  MainWindow......
+00003ed0: 0800 0000 0006 0000 0006 4578 706f 7274  ..........Export
+00003ee0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00003ef0: 0300 0000 1c00 4500 7800 7000 6f00 7200  ......E.x.p.o.r.
+00003f00: 7400 6900 6500 7200 6500 6e00 2e00 2e00  t.i.e.r.e.n.....
+00003f10: 2e08 0000 0000 0600 0000 0945 7870 6f72  ...........Expor
+00003f20: 742e 2e2e 0700 0000 0a4d 6169 6e57 696e  t........MainWin
+00003f30: 646f 7701 0300 0000 0a00 4400 6100 7400  dow.......D.a.t.
+00003f40: 6500 6908 0000 0000 0600 0000 0446 696c  e.i..........Fil
+00003f50: 6507 0000 000a 4d61 696e 5769 6e64 6f77  e.....MainWindow
+00003f60: 0103 ffff ffff 0800 0000 0006 0000 0006  ................
+00003f70: 4669 6c74 6572 0700 0000 0a4d 6169 6e57  Filter.....MainW
+00003f80: 696e 646f 7701 0300 0000 0a00 4800 6900  indow.......H.i.
+00003f90: 6c00 6600 6508 0000 0000 0600 0000 0448  l.f.e..........H
+00003fa0: 656c 7007 0000 000a 4d61 696e 5769 6e64  elp.....MainWind
+00003fb0: 6f77 0103 ffff ffff 0800 0000 0006 0000  ow..............
+00003fc0: 0006 496d 706f 7274 0700 0000 0a4d 6169  ..Import.....Mai
+00003fd0: 6e57 696e 646f 7701 0300 0000 1c00 4900  nWindow.......I.
+00003fe0: 6d00 7000 6f00 7200 7400 6900 6500 7200  m.p.o.r.t.i.e.r.
+00003ff0: 6500 6e00 2e00 2e00 2e08 0000 0000 0600  e.n.............
+00004000: 0000 0949 6d70 6f72 742e 2e2e 0700 0000  ...Import.......
+00004010: 0a4d 6169 6e57 696e 646f 7701 0300 0000  .MainWindow.....
+00004020: 1800 4c00 6f00 6700 6700 6500 2000 5100  ..L.o.g.g.e. .Q.
+00004030: 5300 4f00 2e00 2e00 2e08 0000 0000 0600  S.O.............
+00004040: 0000 0a4c 6f67 2051 534f 2e2e 2e07 0000  ...Log QSO......
+00004050: 000a 4d61 696e 5769 6e64 6f77 0103 ffff  ..MainWindow....
+00004060: ffff 0800 0000 0006 0000 0004 4d6f 6465  ............Mode
+00004070: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+00004080: 0300 0000 1800 5100 5300 4f00 2d00 4600  ......Q.S.O.-.F.
+00004090: 6f00 7200 6d00 7500 6c00 6100 7208 0000  o.r.m.u.l.a.r...
+000040a0: 0000 0600 0000 0851 534f 2046 6f72 6d07  .......QSO Form.
+000040b0: 0000 000a 4d61 696e 5769 6e64 6f77 0103  ....MainWindow..
+000040c0: 0000 0026 0044 0061 0074 0065 006e 0062  ...&.D.a.t.e.n.b
+000040d0: 0061 006e 006b 0020 0077 00e4 0068 006c  .a.n.k. .w...h.l
+000040e0: 0065 006e 002e 002e 002e 0800 0000 0006  .e.n............
+000040f0: 0000 0012 5365 6c65 6374 2064 6174 6162  ....Select datab
+00004100: 6173 652e 2e2e 0700 0000 0a4d 6169 6e57  ase........MainW
+00004110: 696e 646f 7701 0300 0000 1a00 4500 6900  indow.......E.i.
+00004120: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
+00004130: 6700 6500 6e08 0000 0000 0600 0000 0853  g.e.n..........S
+00004140: 6574 7469 6e67 7307 0000 000a 4d61 696e  ettings.....Main
+00004150: 5769 6e64 6f77 0103 0000 0024 005a 0065  Window.....$.Z.e
+00004160: 0069 0067 0065 0020 0046 0069 006c 0074  .i.g.e. .F.i.l.t
+00004170: 0065 0072 0064 0069 0061 006c 006f 0067  .e.r.d.i.a.l.o.g
+00004180: 0800 0000 0006 0000 000b 5368 6f77 2066  ..........Show f
+00004190: 696c 7465 7207 0000 000a 4d61 696e 5769  ilter.....MainWi
+000041a0: 6e64 6f77 0103 0000 0026 005a 0065 0069  ndow.....&.Z.e.i
+000041b0: 0067 0065 0020 0041 006e 0077 0065 006e  .g.e. .A.n.w.e.n
+000041c0: 0064 0075 006e 0067 0073 006c 006f 0067  .d.u.n.g.s.l.o.g
+000041d0: 0800 0000 0006 0000 0008 5368 6f77 206c  ..........Show l
+000041e0: 6f67 0700 0000 0a4d 6169 6e57 696e 646f  og.....MainWindo
+000041f0: 7701 0300 0000 1a00 5300 7400 6100 7200  w.......S.t.a.r.
+00004200: 7400 6500 2000 4800 6100 6d00 6c00 6900  t.e. .H.a.m.l.i.
+00004210: 6208 0000 0000 0600 0000 0c53 7461 7274  b..........Start
+00004220: 2068 616d 6c69 6207 0000 000a 4d61 696e   hamlib.....Main
+00004230: 5769 6e64 6f77 0103 0000 001c 0057 0065  Window.......W.e
+00004240: 0072 006b 007a 0065 0075 0067 006c 0065  .r.k.z.e.u.g.l.e
+00004250: 0069 0073 0074 0065 0800 0000 0006 0000  .i.s.t.e........
+00004260: 0007 546f 6f6c 6261 7207 0000 000a 4d61  ..Toolbar.....Ma
+00004270: 696e 5769 6e64 6f77 0103 0000 0032 004c  inWindow.....2.L
+00004280: 006f 0067 0073 0020 007a 0075 0020 004c  .o.g.s. .z.u. .L
+00004290: 006f 0054 0057 0020 0068 006f 0063 0068  .o.T.W. .h.o.c.h
+000042a0: 006c 0061 0064 0065 006e 002e 002e 002e  .l.a.d.e.n......
+000042b0: 0800 0000 0006 0000 0016 5570 6c6f 6164  ..........Upload
+000042c0: 206c 6f67 7320 746f 204c 6f54 572e 2e2e   logs to LoTW...
+000042d0: 0700 0000 0a4d 6169 6e57 696e 646f 7701  .....MainWindow.
+000042e0: 0300 0000 4200 4400 6100 7400 6500 6900  ....B.D.a.t.e.i.
+000042f0: 2000 6100 7500 6600 2000 6e00 6500 7500   .a.u.f. .n.e.u.
+00004300: 6500 2000 5100 5300 4f00 7300 2000 fc00  e. .Q.S.O.s. ...
+00004310: 6200 6500 7200 7700 6100 6300 6800 6500  b.e.r.w.a.c.h.e.
+00004320: 6e00 2e00 2e00 2e08 0000 0000 0600 0000  n...............
+00004330: 1657 6174 6368 2066 696c 6520 666f 7220  .Watch file for 
+00004340: 5153 4f73 2e2e 2e07 0000 000a 4d61 696e  QSOs........Main
+00004350: 5769 6e64 6f77 0103 0000 0014 004a 004a  Window.......J.J
+00004360: 004a 004a 002d 004d 004d 002d 0054 0054  .J.J.-.M.M.-.T.T
+00004370: 0800 0000 0006 0000 000a 5959 5959 2d4d  ..........YYYY-M
+00004380: 4d2d 4444 0700 0000 0a4d 6169 6e57 696e  M-DD.....MainWin
+00004390: 646f 7701 03ff ffff ff08 0000 0000 0600  dow.............
+000043a0: 0000 0220 5707 0000 0007 5153 4f46 6f72  ... W.....QSOFor
+000043b0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+000043c0: 0420 6b48 7a07 0000 0007 5153 4f46 6f72  . kHz.....QSOFor
+000043d0: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+000043e0: 0235 3907 0000 0007 5153 4f46 6f72 6d01  .59.....QSOForm.
+000043f0: 0300 0000 4800 4500 6900 6e00 2000 4600  ....H.E.i.n. .F.
+00004400: 6500 6c00 6400 2000 6600 6500 6800 6c00  e.l.d. .f.e.h.l.
+00004410: 7400 2000 6600 fc00 7200 2000 6400 6900  t. .f...r. .d.i.
+00004420: 6500 2000 4900 6e00 6200 6f00 7800 2d00  e. .I.n.b.o.x.-.
+00004430: 5000 7200 fc00 6600 7500 6e00 6708 0000  P.r...f.u.n.g...
+00004440: 0000 0600 0000 2241 2066 6965 6c64 2069  ......"A field i
+00004450: 7320 6d69 7373 696e 6720 666f 7220 696e  s missing for in
+00004460: 626f 7820 6368 6563 6b07 0000 0007 5153  box check.....QS
+00004470: 4f46 6f72 6d01 0300 0000 4200 4600 6500  OForm.....B.F.e.
+00004480: 6800 6c00 6500 6e00 6400 6500 7300 2000  h.l.e.n.d.e.s. .
+00004490: 4600 6500 6c00 6400 2000 6600 fc00 7200  F.e.l.d. .f...r.
+000044a0: 2000 6400 6500 6e00 2000 4c00 6f00 6700   .d.e.n. .L.o.g.
+000044b0: 2d00 5500 7000 6c00 6f00 6100 6408 0000  -.U.p.l.o.a.d...
+000044c0: 0000 0600 0000 2141 2066 6965 6c64 2069  ......!A field i
+000044d0: 7320 6d69 7373 696e 6720 666f 7220 6c6f  s missing for lo
+000044e0: 6720 7570 6c6f 6164 0700 0000 0751 534f  g upload.....QSO
+000044f0: 466f 726d 0103 0000 0056 0046 0065 0068  Form.....V.F.e.h
+00004500: 006c 0065 006e 0064 0065 0073 0020 0046  .l.e.n.d.e.s. .F
+00004510: 0065 006c 0064 0020 0066 00fc 0072 0020  .e.l.d. .f...r. 
+00004520: 0064 0065 006e 0020 004c 006f 0067 002d  .d.e.n. .L.o.g.-
+00004530: 0055 0070 006c 006f 0061 0064 0020 007a  .U.p.l.o.a.d. .z
+00004540: 0075 0020 0048 0061 006d 0051 0054 0048  .u. .H.a.m.Q.T.H
+00004550: 0800 0000 0006 0000 002b 4120 6669 656c  .........+A fiel
+00004560: 6420 6973 206d 6973 7369 6e67 2066 6f72  d is missing for
+00004570: 206c 6f67 2075 706c 6f61 6420 746f 2048   log upload to H
+00004580: 616d 5154 4807 0000 0007 5153 4f46 6f72  amQTH.....QSOFor
+00004590: 6d01 0300 0000 1600 4100 6b00 7a00 6500  m.......A.k.z.e.
+000045a0: 7000 7400 6900 6500 7200 7400 3a08 0000  p.t.i.e.r.t.:...
+000045b0: 0000 0600 0000 0841 6363 6570 7473 3a07  .......Accepts:.
+000045c0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+000045d0: 6a00 4500 6900 6e00 2000 4600 6500 6800  j.E.i.n. .F.e.h.
+000045e0: 6c00 6500 7200 2000 7400 7200 6100 7400  l.e.r. .t.r.a.t.
+000045f0: 2000 7700 e400 6800 7200 6500 6e00 6400   .w...h.r.e.n.d.
+00004600: 2000 6400 6500 7200 2000 dc00 6200 6500   .d.e.r. ...b.e.
+00004610: 7200 7400 7200 6100 6700 7500 6e00 6700  r.t.r.a.g.u.n.g.
+00004620: 2000 7a00 7500 2000 4800 6100 6d00 5100   .z.u. .H.a.m.Q.
+00004630: 5400 4800 2000 6100 7500 6608 0000 0000  T.H. .a.u.f.....
+00004640: 0600 0000 2741 6e20 6572 726f 7220 6f63  ....'An error oc
+00004650: 6375 7265 6420 6f6e 2075 706c 6f61 6469  cured on uploadi
+00004660: 6e67 2074 6f20 4861 6d51 5448 0700 0000  ng to HamQTH....
+00004670: 0751 534f 466f 726d 0103 0000 0016 0041  .QSOForm.......A
+00004680: 0075 0074 006f 006d 0061 0074 0069 0073  .u.t.o.m.a.t.i.s
+00004690: 0063 0068 0800 0000 0006 0000 000d 4175  .c.h..........Au
+000046a0: 746f 6d61 7469 6361 6c6c 7907 0000 0007  tomatically.....
+000046b0: 5153 4f46 6f72 6d01 0300 0000 3800 4600  QSOForm.....8.F.
+000046c0: 6500 6800 6c00 6500 7200 6800 6100 6600  e.h.l.e.r.h.a.f.
+000046d0: 7400 6500 7300 2000 4100 6200 6600 7200  t.e.s. .A.b.f.r.
+000046e0: 6100 6700 6500 6500 7200 6700 6500 6200  a.g.e.e.r.g.e.b.
+000046f0: 6e00 6900 7308 0000 0000 0600 0000 1242  n.i.s..........B
+00004700: 6164 2072 6571 7565 7374 2072 6573 756c  ad request resul
+00004710: 7407 0000 0007 5153 4f46 6f72 6d01 03ff  t.....QSOForm...
+00004720: ffff ff08 0000 0000 0600 0000 0442 616e  .............Ban
+00004730: 6407 0000 0007 5153 4f46 6f72 6d01 0300  d.....QSOForm...
+00004740: 0000 0800 4200 fc00 7200 6f08 0000 0000  ....B...r.o.....
+00004750: 0600 0000 0642 7572 6561 7507 0000 0007  .....Bureau.....
+00004760: 5153 4f46 6f72 6d01 0300 0000 1600 4200  QSOForm.......B.
+00004770: fc00 7200 6f00 2f00 4400 6900 7200 6500  ..r.o./.D.i.r.e.
+00004780: 6b00 7408 0000 0000 0600 0000 0d42 7572  k.t..........Bur
+00004790: 6561 752f 4469 7265 6374 0700 0000 0751  eau/Direct.....Q
+000047a0: 534f 466f 726d 0103 0000 0014 0052 0075  SOForm.......R.u
+000047b0: 0066 007a 0065 0069 0063 0068 0065 006e  .f.z.e.i.c.h.e.n
+000047c0: 0800 0000 0006 0000 0009 4361 6c6c 2073  ..........Call s
+000047d0: 6967 6e07 0000 0007 5153 4f46 6f72 6d01  ign.....QSOForm.
+000047e0: 0300 0000 3c00 4600 6500 6800 6c00 6500  ....<.F.e.h.l.e.
+000047f0: 7200 2000 6200 6500 6900 2000 6400 6500  r. .b.e.i. .d.e.
+00004800: 7200 2000 5200 7500 6600 7a00 6500 6900  r. .R.u.f.z.e.i.
+00004810: 6300 6800 6500 6e00 7300 7500 6300 6800  c.h.e.n.s.u.c.h.
+00004820: 6508 0000 0000 0600 0000 1543 616c 6c62  e..........Callb
+00004830: 6f6f 6b20 7365 6172 6368 2065 7272 6f72  ook search error
+00004840: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004850: 002a 0043 0061 006c 006c 0062 006f 006f  .*.C.a.l.l.b.o.o
+00004860: 006b 002d 0053 0075 0063 0068 0065 0072  .k.-.S.u.c.h.e.r
+00004870: 0067 0065 0062 006e 0069 0073 0800 0000  .g.e.b.n.i.s....
+00004880: 0006 0000 0016 4361 6c6c 626f 6f6b 2073  ......Callbook s
+00004890: 6561 7263 6820 7265 7375 6c74 0700 0000  earch result....
+000048a0: 0751 534f 466f 726d 0103 0000 0032 0052  .QSOForm.....2.R
+000048b0: 0075 0066 007a 0065 0069 0063 0068 0065  .u.f.z.e.i.c.h.e
+000048c0: 006e 0020 006e 0069 0063 0068 0074 0020  .n. .n.i.c.h.t. 
+000048d0: 0067 0065 0066 0075 006e 0064 0065 006e  .g.e.f.u.n.d.e.n
+000048e0: 0800 0000 0006 0000 0012 4361 6c6c 7369  ..........Callsi
+000048f0: 676e 206e 6f74 2066 6f75 6e64 0700 0000  gn not found....
+00004900: 0751 534f 466f 726d 0103 0000 000a 004b  .QSOForm.......K
+00004910: 0061 006e 0061 006c 0800 0000 0006 0000  .a.n.a.l........
+00004920: 0007 4368 616e 6e65 6c07 0000 0007 5153  ..Channel.....QS
+00004930: 4f46 6f72 6d01 0300 0000 1600 5000 7200  OForm.......P.r.
+00004940: fc00 6600 6500 2000 4900 6e00 6200 6f00  ..f.e. .I.n.b.o.
+00004950: 7808 0000 0000 0600 0000 0b43 6865 636b  x..........Check
+00004960: 2049 6e62 6f78 0700 0000 0751 534f 466f   Inbox.....QSOFo
+00004970: 726d 0103 0000 0042 0046 0065 0068 006c  rm.....B.F.e.h.l
+00004980: 0065 0072 0020 0062 0065 0069 006d 0020  .e.r. .b.e.i.m. 
+00004990: 0050 0072 00fc 0066 0065 006e 0020 0064  .P.r...f.e.n. .d
+000049a0: 0065 0072 0020 004c 006f 0054 0057 002d  .e.r. .L.o.T.W.-
+000049b0: 0049 006e 0062 006f 0078 0800 0000 0006  .I.n.b.o.x......
+000049c0: 0000 0016 4368 6563 6b20 4c6f 5457 2049  ....Check LoTW I
+000049d0: 6e62 6f78 2065 7272 6f72 0700 0000 0751  nbox error.....Q
+000049e0: 534f 466f 726d 0103 0000 001c 0050 0072  SOForm.......P.r
+000049f0: 00fc 0066 0065 0020 004c 006f 0054 0057  ...f.e. .L.o.T.W
+00004a00: 0020 0051 0053 004c 0800 0000 0006 0000  . .Q.S.L........
+00004a10: 000e 4368 6563 6b20 4c6f 5457 2051 534c  ..Check LoTW QSL
+00004a20: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004a30: 0038 0065 0051 0053 004c 002d 0046 0065  .8.e.Q.S.L.-.F.e
+00004a40: 0068 006c 0065 0072 0020 0070 0072 00fc  .h.l.e.r. .p.r..
+00004a50: 0066 0065 006e 0020 0064 0065 0072 0020  .f.e.n. .d.e.r. 
+00004a60: 0049 006e 0062 006f 0078 0800 0000 0006  .I.n.b.o.x......
+00004a70: 0000 0016 4368 6563 6b20 6551 534c 2049  ....Check eQSL I
+00004a80: 6e62 6f78 2065 7272 6f72 0700 0000 0751  nbox error.....Q
+00004a90: 534f 466f 726d 0103 0000 0018 005a 0075  SOForm.......Z.u
+00004aa0: 0072 00fc 0063 006b 0073 0065 0074 007a  .r...c.k.s.e.t.z
+00004ab0: 0065 006e 0800 0000 0006 0000 0005 436c  .e.n..........Cl
+00004ac0: 6561 7207 0000 0007 5153 4f46 6f72 6d01  ear.....QSOForm.
+00004ad0: 0300 0000 2000 4b00 6f00 6e00 6600 6900  .... .K.o.n.f.i.
+00004ae0: 6700 7500 7200 6900 6500 7200 7400 6500  g.u.r.i.e.r.t.e.
+00004af0: 2000 4900 4408 0000 0000 0600 0000 1343   .I.D..........C
+00004b00: 6f6e 6669 6775 7265 6420 6964 656e 7469  onfigured identi
+00004b10: 7479 0700 0000 0751 534f 466f 726d 0103  ty.....QSOForm..
+00004b20: 0000 002a 004b 006f 006e 0066 0069 0067  ...*.K.o.n.f.i.g
+00004b30: 0075 0072 0069 0065 0072 0074 0065 0020  .u.r.i.e.r.t.e. 
+00004b40: 0053 0074 0061 0074 0069 006f 006e 0800  .S.t.a.t.i.o.n..
+00004b50: 0000 0006 0000 0012 436f 6e66 6967 7572  ........Configur
+00004b60: 6564 2073 7461 7469 6f6e 0700 0000 0751  ed station.....Q
+00004b70: 534f 466f 726d 0103 ffff ffff 0800 0000  SOForm..........
+00004b80: 0006 0000 0007 436f 6e74 6573 7407 0000  ......Contest...
+00004b90: 0007 5153 4f46 6f72 6d01 03ff ffff ff08  ..QSOForm.......
+00004ba0: 0000 0000 0600 0000 0a43 6f6e 7465 7374  .........Contest
+00004bb0: 2049 4407 0000 0007 5153 4f46 6f72 6d01   ID.....QSOForm.
+00004bc0: 0300 0000 1600 4500 6d00 7000 6600 2e00  ......E.m.p.f...
+00004bd0: 2000 4400 6100 7400 6500 6e08 0000 0000   .D.a.t.e.n.....
+00004be0: 0600 0000 0444 6174 6107 0000 0007 5153  .....Data.....QS
+00004bf0: 4f46 6f72 6d01 0300 0000 0c00 6400 6900  OForm.......d.i.
+00004c00: 7200 6500 6b00 7408 0000 0000 0600 0000  r.e.k.t.........
+00004c10: 0644 6972 6563 7407 0000 0007 5153 4f46  .Direct.....QSOF
+00004c20: 6f72 6d01 0300 0000 1c00 6500 5100 5300  orm.......e.Q.S.
+00004c30: 4c00 2000 7300 7000 6500 6900 6300 6800  L. .s.p.e.i.c.h.
+00004c40: 6500 7200 6e08 0000 0000 0600 0000 0d44  e.r.n..........D
+00004c50: 6f77 6e6c 6f61 6420 6551 534c 0700 0000  ownload eQSL....
+00004c60: 0751 534f 466f 726d 0103 0000 006c 0057  .QSOForm.....l.W
+00004c70: 00e4 0068 0072 0065 006e 0064 0020 0064  ...h.r.e.n.d. .d
+00004c80: 0065 0072 0020 0052 0075 0066 007a 0065  .e.r. .R.u.f.z.e
+00004c90: 0069 0063 0068 0065 006e 0073 0075 0063  .i.c.h.e.n.s.u.c
+00004ca0: 0068 0065 0020 0069 0073 0074 0020 0065  .h.e. .i.s.t. .e
+00004cb0: 0069 006e 0020 0046 0065 0068 006c 0065  .i.n. .F.e.h.l.e
+00004cc0: 0072 0020 0061 0075 0066 0067 0065 0074  .r. .a.u.f.g.e.t
+00004cd0: 0072 0065 0074 0065 006e 0800 0000 0006  .r.e.t.e.n......
+00004ce0: 0000 0027 4475 7269 6e67 2063 616c 6c62  ...'During callb
+00004cf0: 6f6f 6b20 7365 6172 6368 2061 6e20 6572  ook search an er
+00004d00: 726f 7220 6f63 6375 7265 6407 0000 0007  ror occured.....
+00004d10: 5153 4f46 6f72 6d01 0300 0000 0800 4500  QSOForm.......E.
+00004d20: 6e00 6400 6508 0000 0000 0600 0000 0345  n.d.e..........E
+00004d30: 6e64 0700 0000 0751 534f 466f 726d 0103  nd.....QSOForm..
+00004d40: 0000 000c 0046 0065 0068 006c 0065 0072  .....F.e.h.l.e.r
+00004d50: 0800 0000 0006 0000 0005 4572 726f 7207  ..........Error.
+00004d60: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004d70: 2400 6500 5100 5300 4c00 2d00 5500 7000  $.e.Q.S.L.-.U.p.
+00004d80: 6c00 6f00 6100 6400 2d00 4600 6500 6800  l.o.a.d.-.F.e.h.
+00004d90: 6c00 6500 7208 0000 0000 0600 0000 0f45  l.e.r..........E
+00004da0: 7272 6f72 206f 6e20 7570 6c6f 6164 0700  rror on upload..
+00004db0: 0000 0751 534f 466f 726d 0103 0000 0010  ...QSOForm......
+00004dc0: 0046 0072 0065 0071 0075 0065 006e 007a  .F.r.e.q.u.e.n.z
+00004dd0: 0800 0000 0006 0000 0009 4672 6571 7565  ..........Freque
+00004de0: 6e63 7907 0000 0007 5153 4f46 6f72 6d01  ncy.....QSOForm.
+00004df0: 03ff ffff ff08 0000 0000 0600 0000 0648  ...............H
+00004e00: 616d 5154 4807 0000 0007 5153 4f46 6f72  amQTH.....QSOFor
+00004e10: 6d01 0300 0000 0400 4900 4408 0000 0000  m.......I.D.....
+00004e20: 0600 0000 0849 6465 6e74 6974 7907 0000  .....Identity...
+00004e30: 0007 5153 4f46 6f72 6d01 0300 0000 2600  ..QSOForm.....&.
+00004e40: 4c00 6900 6e00 6b00 2000 7a00 7500 7200  L.i.n.k. .z.u.r.
+00004e50: 2000 6500 5100 5300 4c00 2d00 4b00 6100   .e.Q.S.L.-.K.a.
+00004e60: 7200 7400 6508 0000 0000 0600 0000 114c  r.t.e..........L
+00004e70: 696e 6b20 746f 2065 5153 4c20 4361 7264  ink to eQSL Card
+00004e80: 0700 0000 0751 534f 466f 726d 0103 ffff  .....QSOForm....
+00004e90: ffff 0800 0000 0006 0000 0004 4c6f 5457  ............LoTW
+00004ea0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00004eb0: 001c 004c 006f 0054 0057 0020 0065 006d  ...L.o.T.W. .e.m
+00004ec0: 0070 0066 0061 006e 0067 0065 006e 0800  .p.f.a.n.g.e.n..
+00004ed0: 0000 0006 0000 000d 4c6f 5457 2072 6563  ........LoTW rec
+00004ee0: 6569 7665 6407 0000 0007 5153 4f46 6f72  eived.....QSOFor
+00004ef0: 6d01 0300 0000 1c00 4c00 6f00 5400 5700  m.......L.o.T.W.
+00004f00: 2000 7600 6500 7200 7300 6500 6e00 6400   .v.e.r.s.e.n.d.
+00004f10: 6500 7408 0000 0000 0600 0000 094c 6f54  e.t..........LoT
+00004f20: 5720 7365 6e74 0700 0000 0751 534f 466f  W sent.....QSOFo
+00004f30: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00004f40: 0007 4c6f 6361 746f 7207 0000 0007 5153  ..Locator.....QS
+00004f50: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00004f60: 0600 0000 074c 6f67 626f 6f6b 0700 0000  .....Logbook....
+00004f70: 0751 534f 466f 726d 0103 0000 0042 004c  .QSOForm.....B.L
+00004f80: 006f 0067 0069 006e 0020 0066 0065 0068  .o.g.i.n. .f.e.h
+00004f90: 006c 0067 0065 0073 0063 0068 006c 0061  .l.g.e.s.c.h.l.a
+00004fa0: 0067 0065 006e 0020 0066 00fc 0072 0020  .g.e.n. .f...r. 
+00004fb0: 0042 0065 006e 0075 0074 007a 0065 0072  .B.e.n.u.t.z.e.r
+00004fc0: 0800 0000 0006 0000 0015 4c6f 6769 6e20  ..........Login 
+00004fd0: 6661 696c 6564 2066 6f72 2075 7365 7207  failed for user.
+00004fe0: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00004ff0: 5800 4c00 6f00 6700 6900 6e00 2000 6200  X.L.o.g.i.n. .b.
+00005000: 6500 6900 2000 4800 6100 6d00 5100 5400  e.i. .H.a.m.Q.T.
+00005010: 4800 2000 6600 6500 6800 6c00 6700 6500  H. .f.e.h.l.g.e.
+00005020: 7300 6300 6800 6c00 6100 6700 6500 6e00  s.c.h.l.a.g.e.n.
+00005030: 2000 6600 fc00 7200 2000 4200 6500 6e00   .f...r. .B.e.n.
+00005040: 7500 7400 7a00 6500 7208 0000 0000 0600  u.t.z.e.r.......
+00005050: 0000 1f4c 6f67 696e 2074 6f20 4861 6d51  ...Login to HamQ
+00005060: 5448 2066 6169 6c65 6420 666f 7220 7573  TH failed for us
+00005070: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
+00005080: 0000 0014 0048 0061 0075 0070 0074 0064  .....H.a.u.p.t.d
+00005090: 0061 0074 0065 006e 0800 0000 0006 0000  .a.t.e.n........
+000050a0: 0009 4d61 696e 2064 6174 6107 0000 0007  ..Main data.....
+000050b0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+000050c0: 0000 0600 0000 044d 6f64 6507 0000 0007  .......Mode.....
+000050d0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+000050e0: 0000 0600 0000 044e 616d 6507 0000 0007  .......Name.....
+000050f0: 5153 4f46 6f72 6d01 0300 0000 2400 4b00  QSOForm.....$.K.
+00005100: 6500 6900 6e00 2000 5100 5300 4c00 2000  e.i.n. .Q.S.L. .
+00005110: 7600 6500 7200 6600 fc00 6700 6200 6100  v.e.r.f...g.b.a.
+00005120: 7208 0000 0000 0600 0000 104e 6f20 5153  r..........No QS
+00005130: 4c20 6176 6169 6c61 626c 6507 0000 0007  L available.....
+00005140: 5153 4f46 6f72 6d01 0300 0000 2600 4b00  QSOForm.....&.K.
+00005150: 6500 6900 6e00 2000 6500 5100 5300 4c00  e.i.n. .e.Q.S.L.
+00005160: 2000 7600 6500 7200 6600 fc00 6700 6200   .v.e.r.f...g.b.
+00005170: 6100 7208 0000 0000 0600 0000 114e 6f20  a.r..........No 
+00005180: 6551 534c 2061 7661 696c 6162 6c65 0700  eQSL available..
+00005190: 0000 0751 534f 466f 726d 0103 0000 000a  ...QSOForm......
+000051a0: 004a 0065 0074 007a 0074 0800 0000 0006  .J.e.t.z.t......
+000051b0: 0000 0003 4e6f 7707 0000 0007 5153 4f46  ....Now.....QSOF
+000051c0: 6f72 6d01 0300 0000 1600 4500 6900 6700  orm.......E.i.g.
+000051d0: 6500 6e00 6500 7200 2000 5100 5400 4808  e.n.e.r. .Q.T.H.
+000051e0: 0000 0000 0600 0000 074f 776e 2051 5448  .........Own QTH
+000051f0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005200: 0024 0045 0069 0067 0065 006e 0065 0073  .$.E.i.g.e.n.e.s
+00005210: 0020 0052 0075 0066 007a 0065 0069 0063  . .R.u.f.z.e.i.c
+00005220: 0068 0065 006e 0800 0000 0006 0000 000d  .h.e.n..........
+00005230: 4f77 6e20 6361 6c6c 2073 6967 6e07 0000  Own call sign...
+00005240: 0007 5153 4f46 6f72 6d01 0300 0000 1e00  ..QSOForm.......
+00005250: 4500 6900 6700 6500 6e00 6500 7200 2000  E.i.g.e.n.e.r. .
+00005260: 4c00 6f00 6300 6100 7400 6f00 7208 0000  L.o.c.a.t.o.r...
+00005270: 0000 0600 0000 0b4f 776e 206c 6f63 6174  .......Own locat
+00005280: 6f72 0700 0000 0751 534f 466f 726d 0103  or.....QSOForm..
+00005290: 0000 0018 0045 0069 0067 0065 006e 0065  .....E.i.g.e.n.e
+000052a0: 0072 0020 004e 0061 006d 0065 0800 0000  .r. .N.a.m.e....
+000052b0: 0006 0000 0008 4f77 6e20 6e61 6d65 0700  ......Own name..
+000052c0: 0000 0751 534f 466f 726d 0103 0000 001c  ...QSOForm......
+000052d0: 0045 0069 0067 0065 006e 0065 0020 004e  .E.i.g.e.n.e. .N
+000052e0: 006f 0074 0069 007a 0065 006e 0800 0000  .o.t.i.z.e.n....
+000052f0: 0006 0000 0009 4f77 6e20 6e6f 7465 7307  ......Own notes.
+00005300: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005310: 1000 4c00 6500 6900 7300 7400 7500 6e00  ..L.e.i.s.t.u.n.
+00005320: 6708 0000 0000 0600 0000 0550 6f77 6572  g..........Power
+00005330: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005340: 001e 0041 0075 0073 0062 0072 0065 0069  ...A.u.s.b.r.e.i
+00005350: 0074 0075 006e 0067 0073 0061 0072 0074  .t.u.n.g.s.a.r.t
+00005360: 0800 0000 0006 0000 000b 5072 6f70 6167  ..........Propag
+00005370: 6174 696f 6e07 0000 0007 5153 4f46 6f72  ation.....QSOFor
+00005380: 6d01 03ff ffff ff08 0000 0000 0600 0000  m...............
+00005390: 0551 525a 4351 0700 0000 0751 534f 466f  .QRZCQ.....QSOFo
+000053a0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+000053b0: 0003 5153 4c07 0000 0007 5153 4f46 6f72  ..QSL.....QSOFor
+000053c0: 6d01 0300 0000 2200 5100 5300 4c00 2000  m.....".Q.S.L. .
+000053d0: 2600 2600 2000 4c00 6f00 6700 2d00 5500  &.&. .L.o.g.-.U.
+000053e0: 7000 6c00 6f00 6100 6408 0000 0000 0600  p.l.o.a.d.......
+000053f0: 0000 1151 534c 2026 2620 4c6f 6720 7570  ...QSL && Log up
+00005400: 6c6f 6164 0700 0000 0751 534f 466f 726d  load.....QSOForm
+00005410: 0103 0000 001c 0051 0053 004c 002d 004b  .......Q.S.L.-.K
+00005420: 0061 0072 0074 0065 006e 0074 0065 0078  .a.r.t.e.n.t.e.x
+00005430: 0074 0800 0000 0006 0000 0010 5153 4c20  .t..........QSL 
+00005440: 6361 7264 206d 6573 7361 6765 0700 0000  card message....
+00005450: 0751 534f 466f 726d 0103 0000 001a 0051  .QSOForm.......Q
+00005460: 0053 004c 0020 0065 006d 0070 0066 0061  .S.L. .e.m.p.f.a
+00005470: 006e 0067 0065 006e 0800 0000 0006 0000  .n.g.e.n........
+00005480: 000c 5153 4c20 7265 6365 6976 6564 0700  ..QSL received..
+00005490: 0000 0751 534f 466f 726d 0103 0000 0018  ...QSOForm......
+000054a0: 0051 0053 004c 0020 0067 0065 0073 0065  .Q.S.L. .g.e.s.e
+000054b0: 006e 0064 0065 0074 0800 0000 0006 0000  .n.d.e.t........
+000054c0: 0008 5153 4c20 7365 6e74 0700 0000 0751  ..QSL sent.....Q
+000054d0: 534f 466f 726d 0103 0000 000e 0051 0053  SOForm.......Q.S
+000054e0: 004c 002d 0056 0069 0061 0800 0000 0006  .L.-.V.i.a......
+000054f0: 0000 0007 5153 4c20 7669 6107 0000 0007  ....QSL via.....
+00005500: 5153 4f46 6f72 6d01 0300 0000 1800 5100  QSOForm.......Q.
+00005510: 5300 4f00 2d00 4600 6f00 7200 6d00 7500  S.O.-.F.o.r.m.u.
+00005520: 6c00 6100 7208 0000 0000 0600 0000 0851  l.a.r..........Q
+00005530: 534f 2046 6f72 6d07 0000 0007 5153 4f46  SO Form.....QSOF
+00005540: 6f72 6d01 0300 0000 1a00 5100 5300 4f00  orm.......Q.S.O.
+00005550: 2d00 4b00 6f00 6d00 6d00 6500 6e00 7400  -.K.o.m.m.e.n.t.
+00005560: 6100 7208 0000 0000 0600 0000 0b51 534f  a.r..........QSO
+00005570: 2063 6f6d 6d65 6e74 0700 0000 0751 534f   comment.....QSO
+00005580: 466f 726d 0103 0000 003e 0051 0053 004f  Form.....>.Q.S.O
+00005590: 0020 0077 0075 0072 0064 0065 0020 0076  . .w.u.r.d.e. .v
+000055a0: 006f 006e 0020 0048 0061 006d 0051 0054  .o.n. .H.a.m.Q.T
+000055b0: 0048 0020 0061 0062 0067 0065 0077 0069  .H. .a.b.g.e.w.i
+000055c0: 0065 0073 0065 006e 0800 0000 0006 0000  .e.s.e.n........
+000055d0: 0016 5153 4f20 7265 6a65 6374 6564 206f  ..QSO rejected o
+000055e0: 6e20 4861 6d51 5448 0700 0000 0751 534f  n HamQTH.....QSO
+000055f0: 466f 726d 0103 ffff ffff 0800 0000 0006  Form............
+00005600: 0000 0003 5154 4807 0000 0007 5153 4f46  ....QTH.....QSOF
+00005610: 6f72 6d01 03ff ffff ff08 0000 0000 0600  orm.............
+00005620: 0000 0652 5354 2052 7807 0000 0007 5153  ...RST Rx.....QS
+00005630: 4f46 6f72 6d01 03ff ffff ff08 0000 0000  OForm...........
+00005640: 0600 0000 0652 5354 2054 7807 0000 0007  .....RST Tx.....
+00005650: 5153 4f46 6f72 6d01 0300 0000 1a00 5200  QSOForm.......R.
+00005660: 5300 5400 2000 6500 6d00 7000 6600 6100  S.T. .e.m.p.f.a.
+00005670: 6e00 6700 6500 6e08 0000 0000 0600 0000  n.g.e.n.........
+00005680: 0c52 5354 2072 6563 6569 7665 6407 0000  .RST received...
+00005690: 0007 5153 4f46 6f72 6d01 0300 0000 1800  ..QSOForm.......
+000056a0: 5200 5300 5400 2000 6700 6500 7300 6500  R.S.T. .g.e.s.e.
+000056b0: 6e00 6400 6500 7408 0000 0000 0600 0000  n.d.e.t.........
+000056c0: 0852 5354 2073 656e 7407 0000 0007 5153  .RST sent.....QS
+000056d0: 4f46 6f72 6d01 0300 0000 1800 4500 6d00  OForm.......E.m.
+000056e0: 7000 6600 2e00 2000 5100 5300 4f00 2000  p.f... .Q.S.O. .
+000056f0: 4900 4408 0000 0000 0600 0000 0b52 6376  I.D..........Rcv
+00005700: 6420 5153 4f20 4944 0700 0000 0751 534f  d QSO ID.....QSO
+00005710: 466f 726d 0103 0000 0012 0053 0070 0065  Form.......S.p.e
+00005720: 0069 0063 0068 0065 0072 006e 0800 0000  .i.c.h.e.r.n....
+00005730: 0006 0000 0004 5361 7665 0700 0000 0751  ......Save.....Q
+00005740: 534f 466f 726d 0103 0000 0026 0053 0070  SOForm.....&.S.p
+00005750: 0065 0069 0063 0068 0065 0072 006e 0020  .e.i.c.h.e.r.n. 
+00005760: 0026 0026 0020 0055 0070 006c 006f 0061  .&.&. .U.p.l.o.a
+00005770: 0064 0800 0000 0006 0000 000e 5361 7665  .d..........Save
+00005780: 2026 2620 5570 6c6f 6164 0700 0000 0751   && Upload.....Q
+00005790: 534f 466f 726d 0103 0000 002a 0065 0051  SOForm.....*.e.Q
+000057a0: 0053 004c 002d 004f 0072 0064 006e 0065  .S.L.-.O.r.d.n.e
+000057b0: 0072 0020 0061 0075 0073 0077 00e4 0068  .r. .a.u.s.w...h
+000057c0: 006c 0065 006e 0800 0000 0006 0000 0012  .l.e.n..........
+000057d0: 5365 6c65 6374 2065 5153 4c20 666f 6c64  Select eQSL fold
+000057e0: 6572 0700 0000 0751 534f 466f 726d 0103  er.....QSOForm..
+000057f0: 0000 0016 0047 0065 0073 002e 0020 0051  .....G.e.s... .Q
+00005800: 0053 004f 0020 0049 0044 0800 0000 0006  .S.O. .I.D......
+00005810: 0000 000b 5365 6e74 2051 534f 2049 4407  ....Sent QSO ID.
+00005820: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005830: 3600 5300 6500 7200 7600 6500 7200 6b00  6.S.e.r.v.e.r.k.
+00005840: 6f00 6d00 6d00 7500 6e00 6900 6b00 6100  o.m.m.u.n.i.k.a.
+00005850: 7400 6900 6f00 6e00 7300 2d00 4600 6500  t.i.o.n.s.-.F.e.
+00005860: 6800 6c00 6500 7208 0000 0000 0600 0000  h.l.e.r.........
+00005870: 1a53 6572 7665 7220 636f 6d6d 756e 6963  .Server communic
+00005880: 6174 696f 6e20 6572 726f 7207 0000 0007  ation error.....
+00005890: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+000058a0: 0000 0600 0000 0553 7461 7274 0700 0000  .......Start....
+000058b0: 0751 534f 466f 726d 0103 ffff ffff 0800  .QSOForm........
+000058c0: 0000 0006 0000 0007 5374 6174 696f 6e07  ........Station.
+000058d0: 0000 0007 5153 4f46 6f72 6d01 03ff ffff  ....QSOForm.....
+000058e0: ff08 0000 0000 0600 0000 0753 7562 6d6f  ...........Submo
+000058f0: 6465 0700 0000 0751 534f 466f 726d 0103  de.....QSOForm..
+00005900: 0000 0030 0044 0061 0073 0020 0051 0053  ...0.D.a.s. .Q.S
+00005910: 004f 0020 0069 0073 0074 0020 0065 0069  .O. .i.s.t. .e.i
+00005920: 006e 0020 0044 0075 0070 006c 0069 006b  .n. .D.u.p.l.i.k
+00005930: 0061 0074 0800 0000 0006 0000 0016 5468  .a.t..........Th
+00005940: 6520 5153 4f20 6973 2061 2064 7570 6c69  e QSO is a dupli
+00005950: 6361 7465 0700 0000 0751 534f 466f 726d  cate.....QSOForm
+00005960: 0103 0000 00b8 0044 0069 0065 0020 0051  .......D.i.e. .Q
+00005970: 0053 004c 002d 0052 006f 0075 0074 0065  .S.L.-.R.o.u.t.e
+00005980: 0020 0064 0065 0072 0020 006b 006f 006e  . .d.e.r. .k.o.n
+00005990: 0074 0061 006b 0074 0069 0065 0072 0074  .t.a.k.t.i.e.r.t
+000059a0: 0065 006e 0020 0053 0074 0061 0074 0069  .e.n. .S.t.a.t.i
+000059b0: 006f 006e 002e 000a 0044 0069 0065 0073  .o.n.....D.i.e.s
+000059c0: 0020 0069 0073 0074 0020 006e 0069 0063  . .i.s.t. .n.i.c
+000059d0: 0068 0074 0020 0064 0069 0065 0020 0041  .h.t. .d.i.e. .A
+000059e0: 0064 0072 0065 0073 0073 0065 0020 0064  .d.r.e.s.s.e. .d
+000059f0: 0065 0073 0020 0051 0053 004c 002d 004d  .e.s. .Q.S.L.-.M
+00005a00: 0061 006e 0061 0067 0065 0072 0073 002f  .a.n.a.g.e.r.s./
+00005a10: 002d 0042 00fc 0072 006f 0073 002e 0800  .-.B...r.o.s....
+00005a20: 0000 0006 0000 004c 5468 6520 636f 6e74  .......LThe cont
+00005a30: 6163 7465 6420 7374 6174 696f 6e20 5153  acted station QS
+00005a40: 4c20 726f 7574 652e 0a54 6869 7320 6973  L route..This is
+00005a50: 206e 6f74 2074 6865 2051 534c 206d 616e   not the QSL man
+00005a60: 6167 6572 2f62 7572 6561 7520 6164 6472  ager/bureau addr
+00005a70: 6573 732e 0700 0000 0751 534f 466f 726d  ess......QSOForm
+00005a80: 0103 0000 0010 0045 006e 0064 0065 007a  .......E.n.d.e.z
+00005a90: 0065 0069 0074 0800 0000 0006 0000 0008  .e.i.t..........
+00005aa0: 5469 6d65 2065 6e64 0700 0000 0751 534f  Time end.....QSO
+00005ab0: 466f 726d 0103 0000 0012 0053 0074 0061  Form.......S.t.a
+00005ac0: 0072 0074 007a 0065 0069 0074 0800 0000  .r.t.z.e.i.t....
+00005ad0: 0006 0000 000a 5469 6d65 2073 7461 7274  ......Time start
+00005ae0: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005af0: 0024 0065 0051 0053 004c 002d 0055 0070  .$.e.Q.S.L.-.U.p
+00005b00: 006c 006f 0061 0064 002d 0046 0065 0068  .l.o.a.d.-.F.e.h
+00005b10: 006c 0065 0072 0800 0000 0006 0000 0011  .l.e.r..........
+00005b20: 5570 6c6f 6164 2065 5153 4c20 6572 726f  Upload eQSL erro
+00005b30: 7207 0000 0007 5153 4f46 6f72 6d01 0300  r.....QSOForm...
+00005b40: 0000 1a00 5500 7000 6c00 6f00 6100 6400  ....U.p.l.o.a.d.
+00005b50: 2d00 4600 6500 6800 6c00 6500 7208 0000  -.F.e.h.l.e.r...
+00005b60: 0000 0600 0000 1055 706c 6f61 6420 6c6f  .......Upload lo
+00005b70: 6720 6572 726f 7207 0000 0007 5153 4f46  g error.....QSOF
+00005b80: 6f72 6d01 0300 0000 6800 5500 7000 6c00  orm.....h.U.p.l.
+00005b90: 6f00 6100 6400 2000 6500 7200 6600 6f00  o.a.d. .e.r.f.o.
+00005ba0: 6c00 6700 7400 2000 6e00 7500 7200 2000  l.g.t. .n.u.r. .
+00005bb0: 7700 6500 6e00 6e00 2000 6100 7500 6600  w.e.n.n. .a.u.f.
+00005bc0: 2000 6400 6500 7200 2000 5100 5300 4c00   .d.e.r. .Q.S.L.
+00005bd0: 2d00 5300 6500 6900 7400 6500 2000 6100  -.S.e.i.t.e. .a.
+00005be0: 7500 7300 6700 6500 7700 e400 6800 6c00  u.s.g.e.w...h.l.
+00005bf0: 7408 0000 0000 0600 0000 2455 706c 6f61  t.........$Uploa
+00005c00: 6473 206f 6e6c 7920 6966 2073 656c 6563  ds only if selec
+00005c10: 7465 6420 6f6e 2051 534c 2070 6167 6507  ted on QSL page.
+00005c20: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005c30: 4800 4400 6500 7200 2000 4e00 7500 7400  H.D.e.r. .N.u.t.
+00005c40: 7a00 6500 7200 2000 4300 6100 6c00 6c00  z.e.r. .C.a.l.l.
+00005c50: 2000 7300 7400 6900 6d00 6d00 7400 2000   .s.t.i.m.m.t. .
+00005c60: 6e00 6900 6300 6800 7400 2000 fc00 6200  n.i.c.h.t. ...b.
+00005c70: 6500 7200 6500 6900 6e08 0000 0000 0600  e.r.e.i.n.......
+00005c80: 0000 1855 7365 7220 6361 6c6c 2064 6f65  ...User call doe
+00005c90: 7320 6e6f 7420 6d61 7463 6807 0000 0007  s not match.....
+00005ca0: 5153 4f46 6f72 6d01 03ff ffff ff08 0000  QSOForm.........
+00005cb0: 0000 0600 0000 0465 5153 4c07 0000 0007  .......eQSL.....
+00005cc0: 5153 4f46 6f72 6d01 0300 0000 1c00 6500  QSOForm.......e.
+00005cd0: 5100 5300 4c00 2000 6500 6d00 7000 6600  Q.S.L. .e.m.p.f.
+00005ce0: 6100 6e00 6700 6500 6e08 0000 0000 0600  a.n.g.e.n.......
+00005cf0: 0000 0d65 5153 4c20 7265 6365 6976 6564  ...eQSL received
+00005d00: 0700 0000 0751 534f 466f 726d 0103 0000  .....QSOForm....
+00005d10: 001a 0065 0051 0053 004c 0020 0067 0065  ...e.Q.S.L. .g.e
+00005d20: 0073 0065 006e 0064 0065 0074 0800 0000  .s.e.n.d.e.t....
+00005d30: 0006 0000 0009 6551 534c 2073 656e 7407  ......eQSL sent.
+00005d40: 0000 0007 5153 4f46 6f72 6d01 0300 0000  ....QSOForm.....
+00005d50: 0800 6b00 2e00 4100 2e08 0000 0000 0600  ..k...A.........
+00005d60: 0000 046e 2e61 2e07 0000 0007 5153 4f46  ...n.a......QSOF
+00005d70: 6f72 6d01 0300 0000 3400 7200 6900 6700  orm.....4.r.i.g.
+00005d80: 6300 7400 6c00 6400 2000 5a00 6500 6900  c.t.l.d. .Z.e.i.
+00005d90: 7400 fc00 6200 6500 7200 7300 6300 6800  t...b.e.r.s.c.h.
+00005da0: 7200 6500 6900 7400 7500 6e00 6708 0000  r.e.i.t.u.n.g...
+00005db0: 0000 0600 0000 0f72 6967 6374 6c64 2074  .......rigctld t
+00005dc0: 696d 656f 7574 0700 0000 0751 534f 466f  imeout.....QSOFo
+00005dd0: 726d 0103 ffff ffff 0800 0000 0006 0000  rm..............
+00005de0: 000a 7979 7979 2d4d 4d2d 6464 0700 0000  ..yyyy-MM-dd....
+00005df0: 0751 534f 466f 726d 0103 0000 0010 0041  .QSOForm.......A
+00005e00: 006e 0074 0065 006e 006e 0065 006e 0800  .n.t.e.n.n.e.n..
+00005e10: 0000 0006 0000 0008 416e 7465 6e6e 6173  ........Antennas
+00005e20: 0700 0000 0853 6574 7469 6e67 7301 0300  .....Settings...
+00005e30: 0000 7a00 4300 4100 5400 2d00 4500 6900  ..z.C.A.T.-.E.i.
+00005e40: 6e00 7300 7400 6500 6c00 6c00 7500 6e00  n.s.t.e.l.l.u.n.
+00005e50: 6700 2000 7700 7500 7200 6400 2000 6e00  g. .w.u.r.d. .n.
+00005e60: 6f00 6300 6800 2000 6e00 6900 6500 2000  o.c.h. .n.i.e. .
+00005e70: 6700 6500 7300 7000 6500 6900 6300 6800  g.e.s.p.e.i.c.h.
+00005e80: 6500 7200 7400 2000 6f00 7200 2000 5000  e.r.t. .o.r. .P.
+00005e90: 6100 7200 6100 6d00 6500 7400 6500 7200  a.r.a.m.e.t.e.r.
+00005ea0: 2000 6600 6500 6800 6c00 6500 6e08 0000   .f.e.h.l.e.n...
+00005eb0: 0000 0600 0000 3b43 4154 2063 6f6e 6669  ......;CAT confi
+00005ec0: 6775 7261 7469 6f6e 2077 6173 206e 6576  guration was nev
+00005ed0: 6572 2073 6176 6564 206f 7220 6120 7061  er saved or a pa
+00005ee0: 7261 6d65 7465 7220 6973 206d 6973 7369  rameter is missi
+00005ef0: 6e67 0700 0000 0853 6574 7469 6e67 7301  ng.....Settings.
+00005f00: 0300 0000 3000 4300 4100 5400 2d00 4500  ....0.C.A.T.-.E.
+00005f10: 6900 6e00 7300 7400 6500 6c00 6c00 7500  i.n.s.t.e.l.l.u.
+00005f20: 6e00 6700 6500 6e00 2000 4600 6500 6800  n.g.e.n. .F.e.h.
+00005f30: 6c00 6500 7208 0000 0000 0600 0000 1243  l.e.r..........C
+00005f40: 4154 2073 6574 7469 6e67 7320 6572 726f  AT settings erro
+00005f50: 7207 0000 0008 5365 7474 696e 6773 0103  r.....Settings..
+00005f60: 0000 002a 0048 0061 006d 006c 0069 0062  ...*.H.a.m.l.i.b
+00005f70: 0020 0072 0069 0067 0063 0074 006c 0064  . .r.i.g.c.t.l.d
+00005f80: 0020 0077 00e4 0068 006c 0065 006e 0800  . .w...h.l.e.n..
+00005f90: 0000 0006 0000 0020 4368 6f6f 7365 2068  ....... Choose h
+00005fa0: 616d 6c69 6220 7269 6763 746c 6420 6578  amlib rigctld ex
+00005fb0: 6563 7574 6162 6c65 0700 0000 0853 6574  ecutable.....Set
+00005fc0: 7469 6e67 7301 0300 0000 2000 4400 6100  tings..... .D.a.
+00005fd0: 7400 7500 6d00 2f00 5a00 6500 6900 7400  t.u.m./.Z.e.i.t.
+00005fe0: 2000 5300 7400 6100 7200 7408 0000 0000   .S.t.a.r.t.....
+00005ff0: 0600 0000 0f44 6174 652f 5469 6d65 2073  .....Date/Time s
+00006000: 7461 7274 0700 0000 0853 6574 7469 6e67  tart.....Setting
+00006010: 7301 0300 0000 4200 4600 6500 6800 6c00  s.....B.F.e.h.l.
+00006020: 6500 7200 2000 6200 6500 6900 6d00 2000  e.r. .b.e.i.m. .
+00006030: 4100 7500 7300 6600 fc00 6800 7200 6500  A.u.s.f...h.r.e.
+00006040: 6e00 2000 7600 6f00 6e00 2000 7200 6900  n. .v.o.n. .r.i.
+00006050: 6700 6300 7400 6c00 6408 0000 0000 0600  g.c.t.l.d.......
+00006060: 0000 1745 7272 6f72 2065 7865 6375 7469  ...Error executi
+00006070: 6e67 2072 6967 6374 6c64 0700 0000 0853  ng rigctld.....S
+00006080: 6574 7469 6e67 7301 03ff ffff ff08 0000  ettings.........
+00006090: 0000 0600 0000 0648 616d 6c69 6207 0000  .......Hamlib...
+000060a0: 0008 5365 7474 696e 6773 0103 0000 0014  ..Settings......
+000060b0: 0046 0075 006e 006b 0067 0065 0072 00e4  .F.u.n.k.g.e.r..
+000060c0: 0074 0065 0800 0000 0006 0000 0006 5261  .t.e..........Ra
+000060d0: 6469 6f73 0700 0000 0853 6574 7469 6e67  dios.....Setting
+000060e0: 7301 0300 0000 4e00 4400 6900 6500 2000  s.....N.D.i.e. .
+000060f0: 6700 6500 7700 e400 6800 6c00 7400 6500  g.e.w...h.l.t.e.
+00006100: 2000 4400 6100 7400 6500 6900 2000 6900   .D.a.t.e.i. .i.
+00006110: 7300 7400 2000 6e00 6900 6300 6800 7400  s.t. .n.i.c.h.t.
+00006120: 2000 6100 7500 7300 6600 fc00 6800 7200   .a.u.s.f...h.r.
+00006130: 6200 6100 7208 0000 0000 0600 0000 2353  b.a.r.........#S
+00006140: 656c 6563 7465 6420 6669 6c65 2069 7320  elected file is 
+00006150: 6e6f 7420 7468 6520 6578 6563 7574 6162  not the executab
+00006160: 6c65 0700 0000 0853 6574 7469 6e67 7301  le.....Settings.
+00006170: 0300 0000 1400 7a00 6500 6900 6700 6500  ......z.e.i.g.e.
+00006180: 2000 6100 6c00 6c00 6508 0000 0000 0600   .a.l.l.e.......
+00006190: 0000 0853 686f 7720 616c 6c07 0000 0008  ...Show all.....
+000061a0: 5365 7474 696e 6773 0103 ffff ffff 0800  Settings........
+000061b0: 0000 0006 0000 0005 5374 6172 7407 0000  ........Start...
+000061c0: 0008 5365 7474 696e 6773 0103 0000 001a  ..Settings......
+000061d0: 0053 0074 0061 0072 0074 0065 0020 0048  .S.t.a.r.t.e. .H
+000061e0: 0061 006d 006c 0069 0062 0800 0000 0006  .a.m.l.i.b......
+000061f0: 0000 000c 5374 6172 7420 6861 6d6c 6962  ....Start hamlib
+00006200: 0700 0000 0853 6574 7469 6e67 7301 03ff  .....Settings...
+00006210: ffff ff08 0000 0000 0600 0000 0453 746f  .............Sto
+00006220: 7007 0000 0008 5365 7474 696e 6773 0103  p.....Settings..
+00006230: 0000 001a 0053 0074 006f 0070 0070 0065  .....S.t.o.p.p.e
+00006240: 0020 0048 0061 006d 006c 0069 0062 0800  . .H.a.m.l.i.b..
+00006250: 0000 0006 0000 000b 5374 6f70 2068 616d  ........Stop ham
+00006260: 6c69 6207 0000 0008 5365 7474 696e 6773  lib.....Settings
+00006270: 0103 0000 000a 0061 006b 0074 0069 0076  .......a.k.t.i.v
+00006280: 0800 0000 0006 0000 0005 6163 7469 7607  ..........activ.
+00006290: 0000 0008 5365 7474 696e 6773 0103 0000  ....Settings....
+000062a0: 000e 0069 006e 0061 006b 0074 0069 0076  ...i.n.a.k.t.i.v
+000062b0: 0800 0000 0006 0000 0007 696e 6163 7469  ..........inacti
+000062c0: 7607 0000 0008 5365 7474 696e 6773 0103  v.....Settings..
+000062d0: 0000 004a 0072 0069 0067 0063 0074 006c  ...J.r.i.g.c.t.l
+000062e0: 0064 0020 006b 006f 006e 006e 0074 0065  .d. .k.o.n.n.t.e
+000062f0: 0020 006e 0069 0063 0068 0074 0020 0067  . .n.i.c.h.t. .g
+00006300: 0065 0073 0074 0061 0072 0074 0065 0074  .e.s.t.a.r.t.e.t
+00006310: 0020 0077 0065 0072 0064 0065 006e 0800  . .w.e.r.d.e.n..
+00006320: 0000 0006 0000 001e 7269 6763 746c 6420  ........rigctld 
+00006330: 6469 6420 6e6f 7420 7374 6172 7420 7072  did not start pr
+00006340: 6f70 6572 6c79 0700 0000 0853 6574 7469  operly.....Setti
+00006350: 6e67 7301 0300 0000 3600 7200 6900 6700  ngs.....6.r.i.g.
+00006360: 6300 7400 6c00 6400 2000 6900 7300 7400  c.t.l.d. .i.s.t.
+00006370: 2000 6e00 6900 6300 6800 7400 2000 7600   .n.i.c.h.t. .v.
+00006380: 6500 7200 6600 fc00 6700 6200 6100 7208  e.r.f...g.b.a.r.
+00006390: 0000 0000 0600 0000 1872 6967 6374 6c64  .........rigctld
+000063a0: 2069 7320 6e6f 7420 6176 6169 6c61 626c   is not availabl
+000063b0: 6507 0000 0008 5365 7474 696e 6773 0103  e.....Settings..
+000063c0: 0000 0010 0067 0065 00e4 006e 0064 0065  .....g.e...n.d.e
+000063d0: 0072 0074 0800 0000 0006 0000 0001 4d07  .r.t..........M.
+000063e0: 0000 0014 5472 616e 736c 6174 6564 5461  ....TranslatedTa
+000063f0: 626c 654d 6f64 656c 0103 0000 0008 004e  bleModel.......N
+00006400: 0065 0069 006e 0800 0000 0006 0000 0001  .e.i.n..........
+00006410: 4e07 0000 0014 5472 616e 736c 6174 6564  N.....Translated
+00006420: 5461 626c 654d 6f64 656c 0103 0000 0012  TableModel......
+00006430: 0061 006e 0067 0065 0066 0072 0061 0067  .a.n.g.e.f.r.a.g
+00006440: 0074 0800 0000 0006 0000 0001 5207 0000  .t..........R...
+00006450: 0014 5472 616e 736c 6174 6564 5461 626c  ..TranslatedTabl
+00006460: 654d 6f64 656c 0103 0000 0004 004a 0061  eModel.......J.a
+00006470: 0800 0000 0006 0000 0001 5907 0000 0014  ..........Y.....
+00006480: 5472 616e 736c 6174 6564 5461 626c 654d  TranslatedTableM
+00006490: 6f64 656c 0103 ffff ffff 0800 0000 0006  odel............
+000064a0: 0000 0007 4a53 3843 616c 6c07 0000 000f  ....JS8Call.....
+000064b0: 6170 7053 656c 6563 7444 6961 6c6f 6701  appSelectDialog.
+000064c0: 03ff ffff ff08 0000 0000 0600 0000 054f  ...............O
+000064d0: 7468 6572 0700 0000 0f61 7070 5365 6c65  ther.....appSele
+000064e0: 6374 4469 616c 6f67 0103 0000 002a 0041  ctDialog.....*.A
+000064f0: 0075 0073 0077 0061 0068 006c 0020 0064  .u.s.w.a.h.l. .d
+00006500: 0065 0073 0020 0050 0072 006f 0067 0072  .e.s. .P.r.o.g.r
+00006510: 0061 006d 006d 0073 0800 0000 0006 0000  .a.m.m.s........
+00006520: 0016 5365 6c65 6374 2074 6865 2061 7070  ..Select the app
+00006530: 6c69 6361 7469 6f6e 0700 0000 0f61 7070  lication.....app
+00006540: 5365 6c65 6374 4469 616c 6f67 0103 ffff  SelectDialog....
+00006550: ffff 0800 0000 0006 0000 0006 5753 4a54  ............WSJT
+00006560: 2d58 0700 0000 0f61 7070 5365 6c65 6374  -X.....appSelect
+00006570: 4469 616c 6f67 0103 ffff ffff 0800 0000  Dialog..........
+00006580: 0006 0000 0006 666c 6469 6769 0700 0000  ......fldigi....
+00006590: 0f61 7070 5365 6c65 6374 4469 616c 6f67  .appSelectDialog
+000065a0: 0188 0000 0002 0101                      ........
```

### Comparing `dragonlog-1.1.3/dragonlog/data/modes.json` & `dragonlog-1.2/dragonlog/data/modes.json`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/eQSL.py` & `dragonlog-1.2/dragonlog/eQSL.py`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/Screenshot.png` & `dragonlog-1.2/dragonlog/icons/Screenshot.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/db.png` & `dragonlog-1.2/dragonlog/icons/db.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/edit.png` & `dragonlog-1.2/dragonlog/icons/edit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/edit_add.png` & `dragonlog-1.2/dragonlog/icons/edit_add.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/edit_addmulti.png` & `dragonlog-1.2/dragonlog/icons/edit_addmulti.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/edit_addmulti.xcf` & `dragonlog-1.2/dragonlog/icons/edit_addmulti.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/edit_remove.png` & `dragonlog-1.2/dragonlog/icons/edit_remove.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/exit.png` & `dragonlog-1.2/dragonlog/icons/exit.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/file_doc.png` & `dragonlog-1.2/dragonlog/icons/file_doc.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/fileexport.png` & `dragonlog-1.2/dragonlog/icons/fileexport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/fileimport.png` & `dragonlog-1.2/dragonlog/icons/fileimport.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/gear.png` & `dragonlog-1.2/dragonlog/icons/gear.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/help.png` & `dragonlog-1.2/dragonlog/icons/help.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.png` & `dragonlog-1.2/dragonlog/icons/icons8-dragon-96.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/icons8-dragon-96.xcf` & `dragonlog-1.2/dragonlog/icons/icons8-dragon-96.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/info.png` & `dragonlog-1.2/dragonlog/icons/info.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/logo.ico` & `dragonlog-1.2/dragonlog/icons/logo.ico`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/no.png` & `dragonlog-1.2/dragonlog/icons/no.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/ok.png` & `dragonlog-1.2/dragonlog/icons/ok.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/player_play.png` & `dragonlog-1.2/dragonlog/icons/player_play.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/player_stop.png` & `dragonlog-1.2/dragonlog/icons/player_stop.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/upload_lotw.png` & `dragonlog-1.2/dragonlog/icons/upload_lotw.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/upload_lotw.xcf` & `dragonlog-1.2/dragonlog/icons/upload_lotw.xcf`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/dragonlog/icons/watch.png` & `dragonlog-1.2/dragonlog/icons/watch.png`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/pyproject.toml` & `dragonlog-1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dragonlog-1.1.3/setup_msi.py` & `dragonlog-1.2/setup_msi.py`

 * *Files identical despite different names*

