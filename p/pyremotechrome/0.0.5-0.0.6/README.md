# Comparing `tmp/pyremotechrome-0.0.5.tar.gz` & `tmp/pyremotechrome-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.5.tar", last modified: Wed May 22 15:12:02 2024, max compression
+gzip compressed data, was "pyremotechrome-0.0.6.tar", last modified: Wed May 22 17:28:02 2024, max compression
```

## Comparing `pyremotechrome-0.0.5.tar` & `pyremotechrome-0.0.6.tar`

### file list

```diff
@@ -1,50 +1,52 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.5/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.5/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.880861 pyremotechrome-0.0.5/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)    28214 2024-05-22 15:04:26.000000 pyremotechrome-0.0.5/dist/pyremotechrome-0.0.4-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    24906 2024-05-22 15:04:21.000000 pyremotechrome-0.0.5/dist/pyremotechrome-0.0.4.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 15:11:59.000000 pyremotechrome-0.0.5/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.880861 pyremotechrome-0.0.5/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.5/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      501 2024-05-22 15:11:43.000000 pyremotechrome-0.0.5/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.884861 pyremotechrome-0.0.5/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.5/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 15:11:18.000000 pyremotechrome-0.0.5/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.5/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.888862 pyremotechrome-0.0.5/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.5/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.5/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.5/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.5/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.888862 pyremotechrome-0.0.5/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.5/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15584 2024-05-22 15:00:20.000000 pyremotechrome-0.0.5/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.5/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.888862 pyremotechrome-0.0.5/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.5/pyremotechrome/session/monitor/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.5/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 14:00:38.000000 pyremotechrome-0.0.5/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.880861 pyremotechrome-0.0.5/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.5/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.5/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.5/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.5/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.5/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 15:12:02.000000 pyremotechrome-0.0.5/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1264 2024-05-22 15:12:02.000000 pyremotechrome-0.0.5/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 15:12:02.000000 pyremotechrome-0.0.5/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 15:12:02.000000 pyremotechrome-0.0.5/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 15:12:02.000000 pyremotechrome-0.0.5/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 15:12:02.892861 pyremotechrome-0.0.5/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.493886 pyremotechrome-0.0.6/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.6/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 17:28:02.493886 pyremotechrome-0.0.6/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.6/README.md
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.469897 pyremotechrome-0.0.6/dist/
+-rw-rw-r--   0 wes       (1000) wes       (1000)    28214 2024-05-22 15:04:26.000000 pyremotechrome-0.0.6/dist/pyremotechrome-0.0.4-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    24906 2024-05-22 15:04:21.000000 pyremotechrome-0.0.6/dist/pyremotechrome-0.0.4.tar.gz
+-rw-rw-r--   0 wes       (1000) wes       (1000)    69473 2024-05-22 15:12:15.000000 pyremotechrome-0.0.6/dist/pyremotechrome-0.0.5-py3-none-any.whl
+-rw-rw-r--   0 wes       (1000) wes       (1000)    66317 2024-05-22 15:12:02.000000 pyremotechrome-0.0.6/dist/pyremotechrome-0.0.5.tar.gz
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 17:27:52.000000 pyremotechrome-0.0.6/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.469897 pyremotechrome-0.0.6/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.6/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      501 2024-05-22 15:11:43.000000 pyremotechrome-0.0.6/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.477893 pyremotechrome-0.0.6/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.6/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1552 2024-05-22 16:19:13.000000 pyremotechrome-0.0.6/pyremotechrome/config/config.json
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.6/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.481891 pyremotechrome-0.0.6/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.6/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.6/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.6/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.6/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.481891 pyremotechrome-0.0.6/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.6/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    15678 2024-05-22 17:26:55.000000 pyremotechrome-0.0.6/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.6/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.485890 pyremotechrome-0.0.6/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.6/pyremotechrome/session/monitor/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.6/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 16:19:07.000000 pyremotechrome-0.0.6/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.461901 pyremotechrome-0.0.6/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.485890 pyremotechrome-0.0.6/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.489888 pyremotechrome-0.0.6/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.6/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.6/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.489888 pyremotechrome-0.0.6/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.6/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.6/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.6/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 17:28:02.493886 pyremotechrome-0.0.6/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 17:28:02.000000 pyremotechrome-0.0.6/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1340 2024-05-22 17:28:02.000000 pyremotechrome-0.0.6/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 17:28:02.000000 pyremotechrome-0.0.6/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 17:28:02.000000 pyremotechrome-0.0.6/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 17:28:02.000000 pyremotechrome-0.0.6/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 17:28:02.493886 pyremotechrome-0.0.6/setup.cfg
```

### Comparing `pyremotechrome-0.0.5/LICENSE` & `pyremotechrome-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/PKG-INFO` & `pyremotechrome-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.5/dist/pyremotechrome-0.0.4-py3-none-any.whl` & `pyremotechrome-0.0.6/dist/pyremotechrome-0.0.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/dist/pyremotechrome-0.0.4.tar.gz` & `pyremotechrome-0.0.6/dist/pyremotechrome-0.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyproject.toml` & `pyremotechrome-0.0.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.0.5"
+version = "0.0.6"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.0.5"
+version = "0.0.6"
 authors = [
   { name="Wes Wei", email="lockingonapple@outlook.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.0.5/pyremotechrome/config/config.json` & `pyremotechrome-0.0.6/pyremotechrome/config/config.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9791666666666666%*

 * *Differences: {"'ffmpeg'": "{'queue_size_multiplier': 2}"}*

```diff
@@ -1,12 +1,12 @@
 {
     "ffmpeg": {
         "ffmpeg_exec": "/usr/bin/ffmpeg",
         "fps": 30,
-        "queue_size_multiplier": 8,
+        "queue_size_multiplier": 2,
         "segment_time": 1
     },
     "server": {
         "debug": false,
         "python_executable_path": "/usr/bin/python3.11",
         "url": {
             "ips": [
```

### Comparing `pyremotechrome-0.0.5/pyremotechrome/config/config.py` & `pyremotechrome-0.0.6/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.0.6/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/server/manager.py` & `pyremotechrome-0.0.6/pyremotechrome/server/manager.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/server/server.py` & `pyremotechrome-0.0.6/pyremotechrome/server/server.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/base.py` & `pyremotechrome-0.0.6/pyremotechrome/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from pyremotechrome.session.support.options import FFMpegOptions
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Info
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.util import get_absolute_path
 from pyremotechrome.util import Numbers
 
+__CHROME_AUTOMATION_LABEL_HEIGHT__ = 6
 
 class Base(webdriver.Chrome):
 
     _id: str
     _cursor: Vector
     _position: Vector
     _border_width: Vector
@@ -103,14 +104,15 @@
         bw, bh = self.execute_script("""
             var w=window;
             return [
                 w.outerWidth - w.innerWidth,
                 w.outerHeight - w.innerHeight
             ];
         """)
+        bh += __CHROME_AUTOMATION_LABEL_EXTRA_HEIGHT__
         self._border_width = Vector(bw, bh)
         
         width, height = size()
         self.set_window_size(width, height)
         self.set_window_position(0, 0)
         self.set_page_load_timeout(60)
         self.zoom()
```

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/mega.py` & `pyremotechrome-0.0.6/pyremotechrome/session/mega.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.0.6/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.0.6/pyremotechrome/session/monitor/display.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.0.6/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.0.6/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.0.6/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/util.py` & `pyremotechrome-0.0.6/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.0.6/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.5/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.0.6/pyremotechrome.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.5
+Version: 0.0.6
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.5/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.0.6/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 README.md
 pyproject.toml
 dist/pyremotechrome-0.0.4-py3-none-any.whl
 dist/pyremotechrome-0.0.4.tar.gz
+dist/pyremotechrome-0.0.5-py3-none-any.whl
+dist/pyremotechrome-0.0.5.tar.gz
 pyremotechrome/__init__.py
 pyremotechrome/__main__.py
 pyremotechrome/util.py
 pyremotechrome.egg-info/PKG-INFO
 pyremotechrome.egg-info/SOURCES.txt
 pyremotechrome.egg-info/dependency_links.txt
 pyremotechrome.egg-info/requires.txt
```

