# Comparing `tmp/pyremotechrome-0.0.7.tar.gz` & `tmp/pyremotechrome-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.7.tar", last modified: Wed May 22 18:27:46 2024, max compression
+gzip compressed data, was "pyremotechrome-0.0.8.tar", last modified: Wed May 22 18:31:02 2024, max compression
```

## Comparing `pyremotechrome-0.0.7.tar` & `pyremotechrome-0.0.8.tar`

### file list

```diff
@@ -1,54 +1,56 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.013859 pyremotechrome-0.0.7/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.7/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:27:46.013859 pyremotechrome-0.0.7/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.7/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:45.993859 pyremotechrome-0.0.7/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)    28214 2024-05-22 15:04:26.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.4-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    24906 2024-05-22 15:04:21.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.4.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)    69473 2024-05-22 15:12:15.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.5-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    66317 2024-05-22 15:12:02.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.5.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)   193965 2024-05-22 17:28:05.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.6-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)   190899 2024-05-22 17:28:02.000000 pyremotechrome-0.0.7/dist/pyremotechrome-0.0.6.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 18:27:42.000000 pyremotechrome-0.0.7/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:45.997859 pyremotechrome-0.0.7/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.7/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      806 2024-05-22 18:24:20.000000 pyremotechrome-0.0.7/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.001859 pyremotechrome-0.0.7/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.7/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 18:26:18.000000 pyremotechrome-0.0.7/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.7/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.005859 pyremotechrome-0.0.7/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.7/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.7/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.7/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.7/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.005859 pyremotechrome-0.0.7/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.7/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15678 2024-05-22 17:26:55.000000 pyremotechrome-0.0.7/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.7/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.005859 pyremotechrome-0.0.7/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.7/pyremotechrome/session/monitor/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.7/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 16:19:07.000000 pyremotechrome-0.0.7/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:45.981859 pyremotechrome-0.0.7/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.005859 pyremotechrome-0.0.7/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.005859 pyremotechrome-0.0.7/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.7/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.7/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.009859 pyremotechrome-0.0.7/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.7/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.7/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.7/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:27:46.013859 pyremotechrome-0.0.7/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:27:45.000000 pyremotechrome-0.0.7/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1416 2024-05-22 18:27:45.000000 pyremotechrome-0.0.7/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 18:27:45.000000 pyremotechrome-0.0.7/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 18:27:45.000000 pyremotechrome-0.0.7/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 18:27:45.000000 pyremotechrome-0.0.7/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 18:27:46.013859 pyremotechrome-0.0.7/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.8/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.8/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/dist/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    28214 2024-05-22 15:04:26.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    24906 2024-05-22 15:04:21.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4.tar.gz
+-rw-rw-r--   0 wes       (1000) wes       (1000)    69473 2024-05-22 15:12:15.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    66317 2024-05-22 15:12:02.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5.tar.gz
+-rw-rw-r--   0 wes       (1000) wes       (1000)   193965 2024-05-22 17:28:05.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)   190899 2024-05-22 17:28:02.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6.tar.gz
+-rw-rw-r--   0 wes       (1000) wes       (1000)   567115 2024-05-22 18:27:48.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.7-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)   563892 2024-05-22 18:27:46.000000 pyremotechrome-0.0.8/dist/pyremotechrome-0.0.7.tar.gz
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 18:30:57.000000 pyremotechrome-0.0.8/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.8/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      806 2024-05-22 18:24:20.000000 pyremotechrome-0.0.8/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.826416 pyremotechrome-0.0.8/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.8/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 18:26:18.000000 pyremotechrome-0.0.8/pyremotechrome/config/config.json
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.8/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.8/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.8/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.8/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.8/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.8/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    15672 2024-05-22 18:30:48.000000 pyremotechrome-0.0.8/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.8/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 16:19:07.000000 pyremotechrome-0.0.8/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.814416 pyremotechrome-0.0.8/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.830416 pyremotechrome-0.0.8/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.8/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.8/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.8/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.8/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.8/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1492 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 18:31:02.000000 pyremotechrome-0.0.8/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 18:31:02.834416 pyremotechrome-0.0.8/setup.cfg
```

### Comparing `pyremotechrome-0.0.7/LICENSE` & `pyremotechrome-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/PKG-INFO` & `pyremotechrome-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.4-py3-none-any.whl` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.4.tar.gz` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.5-py3-none-any.whl` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.5.tar.gz` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.5.tar.gz`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.6-py3-none-any.whl` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/dist/pyremotechrome-0.0.6.tar.gz` & `pyremotechrome-0.0.8/dist/pyremotechrome-0.0.6.tar.gz`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyproject.toml` & `pyremotechrome-0.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.0.7"
+version = "0.0.8"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Wes Wei", email="lockingonapple@outlook.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.0.7/pyremotechrome/__main__.py` & `pyremotechrome-0.0.8/pyremotechrome/__main__.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/config/config.json` & `pyremotechrome-0.0.8/pyremotechrome/config/config.json`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/config/config.py` & `pyremotechrome-0.0.8/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.0.8/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/server/manager.py` & `pyremotechrome-0.0.8/pyremotechrome/server/manager.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/server/server.py` & `pyremotechrome-0.0.8/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/base.py` & `pyremotechrome-0.0.8/pyremotechrome/session/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         bw, bh = self.execute_script("""
             var w=window;
             return [
                 w.outerWidth - w.innerWidth,
                 w.outerHeight - w.innerHeight
             ];
         """)
-        bh += __CHROME_AUTOMATION_LABEL_EXTRA_HEIGHT__
+        bh += __CHROME_AUTOMATION_LABEL_HEIGHT__
         self._border_width = Vector(bw, bh)
         
         width, height = size()
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
```

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/mega.py` & `pyremotechrome-0.0.8/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.0.8/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.0.8/pyremotechrome/session/monitor/display.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.0.8/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.0.8/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.0.8/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/util.py` & `pyremotechrome-0.0.8/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.0.8/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.7/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.0.8/pyremotechrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.7
+Version: 0.0.8
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.7/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.0.8/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 pyproject.toml
 dist/pyremotechrome-0.0.4-py3-none-any.whl
 dist/pyremotechrome-0.0.4.tar.gz
 dist/pyremotechrome-0.0.5-py3-none-any.whl
 dist/pyremotechrome-0.0.5.tar.gz
 dist/pyremotechrome-0.0.6-py3-none-any.whl
 dist/pyremotechrome-0.0.6.tar.gz
+dist/pyremotechrome-0.0.7-py3-none-any.whl
+dist/pyremotechrome-0.0.7.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
```

