# Comparing `tmp/pyremotechrome-0.0.1.tar.gz` & `tmp/pyremotechrome-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.1.tar", last modified: Wed May 22 14:41:29 2024, max compression
+gzip compressed data, was "pyremotechrome-0.0.2.tar", last modified: Wed May 22 14:16:55 2024, max compression
```

## Comparing `pyremotechrome-0.0.1.tar` & `pyremotechrome-0.0.2.tar`

### file list

```diff
@@ -1,52 +1,50 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.582276 pyremotechrome-0.0.1/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.1/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 14:41:29.578276 pyremotechrome-0.0.1/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.1/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.562276 pyremotechrome-0.0.1/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)   191192 2024-05-22 14:40:24.000000 pyremotechrome-0.0.1/dist/pyremotechrome-0.0.1-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)   188376 2024-05-22 14:40:21.000000 pyremotechrome-0.0.1/dist/pyremotechrome-0.0.1.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)    68667 2024-05-22 14:16:57.000000 pyremotechrome-0.0.1/dist/pyremotechrome-0.0.2-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    65106 2024-05-22 14:16:55.000000 pyremotechrome-0.0.1/dist/pyremotechrome-0.0.2.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 14:41:05.000000 pyremotechrome-0.0.1/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.566276 pyremotechrome-0.0.1/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.1/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      607 2024-05-22 14:00:24.000000 pyremotechrome-0.0.1/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.570276 pyremotechrome-0.0.1/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       57 2024-05-22 14:00:29.000000 pyremotechrome-0.0.1/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1535 2024-05-22 12:03:24.000000 pyremotechrome-0.0.1/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.1/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.570276 pyremotechrome-0.0.1/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.1/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.1/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6310 2024-05-22 14:00:32.000000 pyremotechrome-0.0.1/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4149 2024-05-22 14:00:41.000000 pyremotechrome-0.0.1/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.574276 pyremotechrome-0.0.1/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.1/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15574 2024-05-22 14:00:40.000000 pyremotechrome-0.0.1/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2002 2024-05-22 14:00:39.000000 pyremotechrome-0.0.1/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.574276 pyremotechrome-0.0.1/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.1/pyremotechrome/session/monitor/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.1/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 14:00:38.000000 pyremotechrome-0.0.1/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.554276 pyremotechrome-0.0.1/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.574276 pyremotechrome-0.0.1/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.578276 pyremotechrome-0.0.1/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.1/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.1/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.578276 pyremotechrome-0.0.1/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.1/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.1/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.1/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:41:29.578276 pyremotechrome-0.0.1/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 14:41:29.000000 pyremotechrome-0.0.1/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1340 2024-05-22 14:41:29.000000 pyremotechrome-0.0.1/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 14:41:29.000000 pyremotechrome-0.0.1/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 14:41:29.000000 pyremotechrome-0.0.1/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       26 2024-05-22 14:41:29.000000 pyremotechrome-0.0.1/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 14:41:29.582276 pyremotechrome-0.0.1/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.170021 pyremotechrome-0.0.2/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.2/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      501 2024-05-22 14:16:55.170021 pyremotechrome-0.0.2/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.2/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.158021 pyremotechrome-0.0.2/dist/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    27983 2024-05-22 14:05:17.000000 pyremotechrome-0.0.2/dist/pyremotechrome-0.0.1-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    24407 2024-05-22 14:04:42.000000 pyremotechrome-0.0.2/dist/pyremotechrome-0.0.1.tar.gz
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      636 2024-05-22 14:16:26.000000 pyremotechrome-0.0.2/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.158021 pyremotechrome-0.0.2/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.2/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      607 2024-05-22 14:00:24.000000 pyremotechrome-0.0.2/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.162021 pyremotechrome-0.0.2/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       57 2024-05-22 14:00:29.000000 pyremotechrome-0.0.2/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1535 2024-05-22 12:03:24.000000 pyremotechrome-0.0.2/pyremotechrome/config/config.json
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.2/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.162021 pyremotechrome-0.0.2/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.2/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.2/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6310 2024-05-22 14:00:32.000000 pyremotechrome-0.0.2/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4149 2024-05-22 14:00:41.000000 pyremotechrome-0.0.2/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.162021 pyremotechrome-0.0.2/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.2/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    15574 2024-05-22 14:00:40.000000 pyremotechrome-0.0.2/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2002 2024-05-22 14:00:39.000000 pyremotechrome-0.0.2/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.166021 pyremotechrome-0.0.2/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.2/pyremotechrome/session/monitor/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.2/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 14:00:38.000000 pyremotechrome-0.0.2/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.154021 pyremotechrome-0.0.2/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.166021 pyremotechrome-0.0.2/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.166021 pyremotechrome-0.0.2/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.2/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.2/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.170021 pyremotechrome-0.0.2/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.2/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.2/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.2/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:16:55.170021 pyremotechrome-0.0.2/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      501 2024-05-22 14:16:55.000000 pyremotechrome-0.0.2/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1264 2024-05-22 14:16:55.000000 pyremotechrome-0.0.2/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 14:16:55.000000 pyremotechrome-0.0.2/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 14:16:55.000000 pyremotechrome-0.0.2/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       26 2024-05-22 14:16:55.000000 pyremotechrome-0.0.2/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 14:16:55.170021 pyremotechrome-0.0.2/setup.cfg
```

### Comparing `pyremotechrome-0.0.1/LICENSE` & `pyremotechrome-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/__main__.py` & `pyremotechrome-0.0.2/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/config/config.json` & `pyremotechrome-0.0.2/pyremotechrome/config/config.json`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/config/config.py` & `pyremotechrome-0.0.2/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.0.2/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/server/manager.py` & `pyremotechrome-0.0.2/pyremotechrome/server/manager.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/server/server.py` & `pyremotechrome-0.0.2/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/base.py` & `pyremotechrome-0.0.2/pyremotechrome/session/base.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/mega.py` & `pyremotechrome-0.0.2/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.0.2/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.0.2/pyremotechrome/session/monitor/display.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.0.2/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.0.2/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.0.2/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/util.py` & `pyremotechrome-0.0.2/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.0.2/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.1/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.0.2/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 LICENSE
 README.md
 pyproject.toml
 dist/pyremotechrome-0.0.1-py3-none-any.whl
 dist/pyremotechrome-0.0.1.tar.gz
-dist/pyremotechrome-0.0.2-py3-none-any.whl
-dist/pyremotechrome-0.0.2.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
```

