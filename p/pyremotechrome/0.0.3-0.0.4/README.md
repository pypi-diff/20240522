# Comparing `tmp/pyremotechrome-0.0.3.tar.gz` & `tmp/pyremotechrome-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyremotechrome-0.0.3.tar", last modified: Wed May 22 14:43:31 2024, max compression
+gzip compressed data, was "pyremotechrome-0.0.4.tar", last modified: Wed May 22 15:04:21 2024, max compression
```

## Comparing `pyremotechrome-0.0.3.tar` & `pyremotechrome-0.0.4.tar`

### file list

```diff
@@ -1,52 +1,47 @@
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.286751 pyremotechrome-0.0.3/
--rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.3/LICENSE
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 14:43:31.286751 pyremotechrome-0.0.3/PKG-INFO
--rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.3/README.md
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.274751 pyremotechrome-0.0.3/dist/
--rw-rw-r--   0 wes       (1000) wes       (1000)   518338 2024-05-22 14:41:42.000000 pyremotechrome-0.0.3/dist/pyremotechrome-0.0.1-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)   515650 2024-05-22 14:41:29.000000 pyremotechrome-0.0.3/dist/pyremotechrome-0.0.1.tar.gz
--rw-rw-r--   0 wes       (1000) wes       (1000)    68667 2024-05-22 14:16:57.000000 pyremotechrome-0.0.3/dist/pyremotechrome-0.0.2-py3-none-any.whl
--rw-rw-r--   0 wes       (1000) wes       (1000)    65106 2024-05-22 14:16:55.000000 pyremotechrome-0.0.3/dist/pyremotechrome-0.0.2.tar.gz
--rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 14:43:07.000000 pyremotechrome-0.0.3/pyproject.toml
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.278751 pyremotechrome-0.0.3/pyremotechrome/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.3/pyremotechrome/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      607 2024-05-22 14:00:24.000000 pyremotechrome-0.0.3/pyremotechrome/__main__.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.278751 pyremotechrome-0.0.3/pyremotechrome/config/
--rw-rw-r--   0 wes       (1000) wes       (1000)       57 2024-05-22 14:00:29.000000 pyremotechrome-0.0.3/pyremotechrome/config/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     1535 2024-05-22 12:03:24.000000 pyremotechrome-0.0.3/pyremotechrome/config/config.json
--rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.3/pyremotechrome/config/config.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/server/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.3/pyremotechrome/server/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.3/pyremotechrome/server/favicon.ico
--rw-rw-r--   0 wes       (1000) wes       (1000)     6310 2024-05-22 14:00:32.000000 pyremotechrome-0.0.3/pyremotechrome/server/manager.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4149 2024-05-22 14:00:41.000000 pyremotechrome-0.0.3/pyremotechrome/server/server.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/session/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.3/pyremotechrome/session/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)    15574 2024-05-22 14:00:40.000000 pyremotechrome-0.0.3/pyremotechrome/session/base.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     2002 2024-05-22 14:00:39.000000 pyremotechrome-0.0.3/pyremotechrome/session/mega.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/session/monitor/
--rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.3/pyremotechrome/session/monitor/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.3/pyremotechrome/session/monitor/audio.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 14:00:38.000000 pyremotechrome-0.0.3/pyremotechrome/session/monitor/display.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.266751 pyremotechrome-0.0.3/pyremotechrome/session/support/
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/session/support/common/
--rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/common/__init__.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/common/directory.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/common/info.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/common/result.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/common/vector.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/session/support/options/
--rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/options/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.3/pyremotechrome/session/support/options/ffmpeg.py
--rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.3/pyremotechrome/util.py
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.282751 pyremotechrome-0.0.3/pyremotechrome/wave/
--rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.3/pyremotechrome/wave/__init__.py
--rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.3/pyremotechrome/wave/index.html
--rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.3/pyremotechrome/wave/loop.wav
-drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 14:43:31.286751 pyremotechrome-0.0.3/pyremotechrome.egg-info/
--rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 14:43:31.000000 pyremotechrome-0.0.3/pyremotechrome.egg-info/PKG-INFO
--rw-rw-r--   0 wes       (1000) wes       (1000)     1340 2024-05-22 14:43:31.000000 pyremotechrome-0.0.3/pyremotechrome.egg-info/SOURCES.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 14:43:31.000000 pyremotechrome-0.0.3/pyremotechrome.egg-info/dependency_links.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 14:43:31.000000 pyremotechrome-0.0.3/pyremotechrome.egg-info/requires.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       26 2024-05-22 14:43:31.000000 pyremotechrome-0.0.3/pyremotechrome.egg-info/top_level.txt
--rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 14:43:31.286751 pyremotechrome-0.0.3/setup.cfg
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1063 2024-05-22 13:27:37.000000 pyremotechrome-0.0.4/LICENSE
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/PKG-INFO
+-rwxrwxr-x   0 wes       (1000) wes       (1000)      114 2024-05-22 14:14:51.000000 pyremotechrome-0.0.4/README.md
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      914 2024-05-22 15:04:07.000000 pyremotechrome-0.0.4/pyproject.toml
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.923891 pyremotechrome-0.0.4/pyremotechrome/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-22 04:06:17.000000 pyremotechrome-0.0.4/pyremotechrome/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      599 2024-05-22 14:58:48.000000 pyremotechrome-0.0.4/pyremotechrome/__main__.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.931892 pyremotechrome-0.0.4/pyremotechrome/config/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       45 2024-05-22 14:58:40.000000 pyremotechrome-0.0.4/pyremotechrome/config/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1535 2024-05-22 12:03:24.000000 pyremotechrome-0.0.4/pyremotechrome/config/config.json
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1021 2024-05-22 03:53:35.000000 pyremotechrome-0.0.4/pyremotechrome/config/config.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.935892 pyremotechrome-0.0.4/pyremotechrome/server/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-21 12:28:42.000000 pyremotechrome-0.0.4/pyremotechrome/server/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)     4286 2024-05-21 12:36:41.000000 pyremotechrome-0.0.4/pyremotechrome/server/favicon.ico
+-rw-rw-r--   0 wes       (1000) wes       (1000)     6317 2024-05-22 15:02:41.000000 pyremotechrome-0.0.4/pyremotechrome/server/manager.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4143 2024-05-22 14:59:39.000000 pyremotechrome-0.0.4/pyremotechrome/server/server.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.939892 pyremotechrome-0.0.4/pyremotechrome/session/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)       93 2024-05-22 15:01:48.000000 pyremotechrome-0.0.4/pyremotechrome/session/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)    15584 2024-05-22 15:00:20.000000 pyremotechrome-0.0.4/pyremotechrome/session/base.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     2001 2024-05-22 15:02:00.000000 pyremotechrome-0.0.4/pyremotechrome/session/mega.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/pyremotechrome/session/monitor/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)        0 2024-05-21 07:44:37.000000 pyremotechrome-0.0.4/pyremotechrome/session/monitor/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4691 2024-05-21 10:45:01.000000 pyremotechrome-0.0.4/pyremotechrome/session/monitor/audio.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     4073 2024-05-22 14:00:38.000000 pyremotechrome-0.0.4/pyremotechrome/session/monitor/display.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.919891 pyremotechrome-0.0.4/pyremotechrome/session/support/
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/pyremotechrome/session/support/common/
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      258 2024-05-22 14:00:34.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/common/__init__.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1349 2024-05-21 08:22:01.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/common/directory.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      666 2024-05-21 07:44:37.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/common/info.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      365 2024-05-21 10:45:18.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/common/result.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)      627 2024-05-21 10:45:20.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/common/vector.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/pyremotechrome/session/support/options/
+-rw-rw-r--   0 wes       (1000) wes       (1000)       81 2024-05-22 14:00:37.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/options/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      484 2024-05-22 14:00:33.000000 pyremotechrome-0.0.4/pyremotechrome/session/support/options/ffmpeg.py
+-rwxrwxrwx   0 wes       (1000) wes       (1000)     1999 2024-05-22 08:50:35.000000 pyremotechrome-0.0.4/pyremotechrome/util.py
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/pyremotechrome/wave/
+-rw-rw-r--   0 wes       (1000) wes       (1000)        0 2024-05-22 09:17:54.000000 pyremotechrome-0.0.4/pyremotechrome/wave/__init__.py
+-rw-rw-r--   0 wes       (1000) wes       (1000)      396 2024-05-22 11:11:18.000000 pyremotechrome-0.0.4/pyremotechrome/wave/index.html
+-rw-rw-r--   0 wes       (1000) wes       (1000)   882078 2024-05-21 11:12:02.000000 pyremotechrome-0.0.4/pyremotechrome/wave/loop.wav
+drwxrwxr-x   0 wes       (1000) wes       (1000)        0 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/pyremotechrome.egg-info/
+-rw-r--r--   0 wes       (1000) wes       (1000)      780 2024-05-22 15:04:21.000000 pyremotechrome-0.0.4/pyremotechrome.egg-info/PKG-INFO
+-rw-rw-r--   0 wes       (1000) wes       (1000)     1188 2024-05-22 15:04:21.000000 pyremotechrome-0.0.4/pyremotechrome.egg-info/SOURCES.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)        1 2024-05-22 15:04:21.000000 pyremotechrome-0.0.4/pyremotechrome.egg-info/dependency_links.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       83 2024-05-22 15:04:21.000000 pyremotechrome-0.0.4/pyremotechrome.egg-info/requires.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       20 2024-05-22 15:04:21.000000 pyremotechrome-0.0.4/pyremotechrome.egg-info/top_level.txt
+-rw-rw-r--   0 wes       (1000) wes       (1000)       38 2024-05-22 15:04:21.943892 pyremotechrome-0.0.4/setup.cfg
```

### Comparing `pyremotechrome-0.0.3/LICENSE` & `pyremotechrome-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/PKG-INFO` & `pyremotechrome-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.3/pyproject.toml` & `pyremotechrome-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [metadata]
 name = "pyremotechrome"
-version = "0.0.3"
+version = "0.0.4"
 
 [tool.setuptools.packages]
 find = {}  # Scan the project directory with the default parameters
 
 [tool.setuptools.package-data]
 "*" = ["*.*"] # Include resources
 
 [project]
 name = "pyremotechrome"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Wes Wei", email="lockingonapple@outlook.com" },
 ]
 dependencies = [
   "selenium>=4.19.0",
   "psutil>=5.9.8",
   "PyVirtualDisplay>=3.0",
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/__main__.py` & `pyremotechrome-0.0.4/pyremotechrome/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """
 Use this module to start the server
 """
 
 from sys import argv
 from os.path import dirname, realpath
 from subprocess import Popen, PIPE, STDOUT
-from pyremotechrome.config import MegaConf
+from pyremotechrome.config import Conf
 
 
-c = MegaConf()
+c = Conf()
 __ROOT__ = f"{dirname(realpath(__file__))}"
 __PYTHON_EXEC__ = c.server.python_executable_path
 
 
 def start() -> None:
     """Start the server"""
     proc_args = [__PYTHON_EXEC__, f"{__ROOT__}/server/server.py"]
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/config/config.json` & `pyremotechrome-0.0.4/pyremotechrome/config/config.json`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/config/config.py` & `pyremotechrome-0.0.4/pyremotechrome/config/config.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/server/favicon.ico` & `pyremotechrome-0.0.4/pyremotechrome/server/favicon.ico`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/server/manager.py` & `pyremotechrome-0.0.4/pyremotechrome/server/manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from re import search
 from inspect import signature
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
+from pyremotechrome.config import Conf
+from pyremotechrome.session import MegaBase
 from pyremotechrome.session.support.common import Directory
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.session.support.common import Result
 from pyremotechrome.session.support.options import FFMpegOptions
-from pyremotechrome.session.mega import Mega
-from pyremotechrome.config import MegaConf
 from pyremotechrome.util import print_exception
 from pyremotechrome.util import get_value_in_dict
 
 # load the following from config.json
-c = MegaConf()
+c = Conf()
 
 # Session
 session = c.session
 size = session.size
 __DEFAULT_WIDTH__ = size.window.width
 __DEFAULT_HEIGHT__ = size.window.height
 __SCREEN_WIDTH__ = size.screen.width
@@ -39,15 +39,15 @@
 # Server
 server = c.server
 url = server.url
 __WAVE_URL__ = f"{url.scheme}://{url.name}:{url.port}/wave/"
 __DEBUG__ = server.debug
 
 
-class MegaSession(Mega):
+class RemoteSession(MegaBase):
 
     def __init__(self, id: str) -> None:
 
         super().__init__(
             id=id,
             scale=__DEFAULT_SCALE__,
             data_dir=f"{__DATA_DIR__}/{id}",
@@ -63,33 +63,33 @@
                 fps=__FRAME_PER_SEC__,
                 queue_size_multiplier=__QUEUE_SIZE_MULTIPLIER__
             ),
             url_rules=__URL_RULES__
         )
 
 class Manager:
-    """Manage Mega Sessions"""
+    """Manage Remote Sessions"""
 
-    _sessions: dict[str, MegaSession]
+    _sessions: dict[str, RemoteSession]
     _data_dir: dict[str, str]
 
     def __init__(self) -> None:
         """DOCTSTRING"""
         self._sessions = {}
         self._data_dir = Directory(__DATA_DIR__)
 
     def create_session(self, session_id: str) -> Result:
         """
-        If the Mega Session is not created, create a Mega Session and
+        If the Remote Session is not created, create a Remote Session and
         store it in an array. Then return a Result object with
         the first window_handle.
         """
 
         if session_id not in self._sessions:
-            self._sessions[session_id] = MegaSession(session_id)
+            self._sessions[session_id] = RemoteSession(session_id)
             window_handle = self._sessions[session_id].get_current_window_handle()
             return Result(True, "", {"window_handle": window_handle})
         else:
             return Result(False, f"session `{session_id}` already exists.")
 
     def get_session_info(self, session_id: str) -> Result:
         """Return Session Result containing window_handles, _title and _icon"""
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/server/server.py` & `pyremotechrome-0.0.4/pyremotechrome/server/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 """
-This is an api server to control MegaSession
+This is an api server to control RemoteSession
 
 // Use this as url_obj for debugging:
 // url_obj = {"method": "GET", "url": url, "response": response}
 
 TODO: Try using a json file for configuration
 TODO: Try using a log file to log errors, and actions
 """
@@ -14,24 +14,24 @@
 from json import dumps as json_dumps
 from http.server import BaseHTTPRequestHandler
 from http.server import HTTPServer
 from urllib.parse import urlparse
 from urllib.parse import parse_qs
 from pyremotechrome.session.support.common import Result
 from pyremotechrome.server.manager import Manager
-from pyremotechrome.config import MegaConf
+from pyremotechrome.config import Conf
 from pyremotechrome.util import get_value_in_dict
 
 
 __ROOT__ = dirname(dirname(realpath(__file__)))
 __ICON_PATH__ = f"{__ROOT__}/server/favicon.ico"
 __WAVE_DIR__ = f"{__ROOT__}/wave/"
 
 # load the following from config.json
-c = MegaConf()
+c = Conf()
 
 # Server
 server = c.server
 url = server.url
 __SERVER_SCHEME__ = url.scheme
 __SERVER_NAME__ = url.name
 __SERVER_PORT__ = url.port
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/base.py` & `pyremotechrome-0.0.4/pyremotechrome/session/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,15 +311,15 @@
         """Emulate pressing a sequence of keys"""
         for keys in key_seqs:
             self.key(keys)
 
     # Copy and Paste
     def _create_clipboard(self) -> WebElement:
         """Create an invisble text_area"""
-        textarea_id = f"mega-clipboard-{self._id}-{self.get_current_window_handle()}"
+        textarea_id = f"pyremotechrome-clipboard-{self._id}-{self.get_current_window_handle()}"
         css_selector = f"textarea#{textarea_id}"
         try:
             self.select(css_selector)
         except NoSuchElementException:
             self.execute_script(f"""
                 input = document.createElement('textarea');
                 input.style.width = '0px';
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/mega.py` & `pyremotechrome-0.0.4/pyremotechrome/session/mega.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from selenium.webdriver.support.events import EventFiringWebDriver
 from selenium.webdriver.support.events import AbstractEventListener
-from pyremotechrome.session.base import Base
+from pyremotechrome.session import Base
 from pyremotechrome.session.support.options import FFMpegOptions
 from pyremotechrome.session.support.common import Vector
 from pyremotechrome.util import Numbers
 
 
 class CustomEventListeners(AbstractEventListener):
     """DOCSTRING"""
@@ -25,15 +25,15 @@
     def after_navigate_back(self, driver: Base) -> None:
         driver.hide_scrollbar(driver)
 
     def after_navigate_forward(self, driver: Base) -> None:
         driver.hide_scrollbar()
 
 
-class Mega(EventFiringWebDriver):
+class MegaBase(EventFiringWebDriver):
 
     url_rules: list[str]
 
     def __init__(
         self,
         id: str,
         scale: Numbers,
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/monitor/audio.py` & `pyremotechrome-0.0.4/pyremotechrome/session/monitor/audio.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/monitor/display.py` & `pyremotechrome-0.0.4/pyremotechrome/session/monitor/display.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/support/common/directory.py` & `pyremotechrome-0.0.4/pyremotechrome/session/support/common/directory.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/support/common/info.py` & `pyremotechrome-0.0.4/pyremotechrome/session/support/common/info.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/session/support/common/vector.py` & `pyremotechrome-0.0.4/pyremotechrome/session/support/common/vector.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/util.py` & `pyremotechrome-0.0.4/pyremotechrome/util.py`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome/wave/loop.wav` & `pyremotechrome-0.0.4/pyremotechrome/wave/loop.wav`

 * *Files identical despite different names*

### Comparing `pyremotechrome-0.0.3/pyremotechrome.egg-info/PKG-INFO` & `pyremotechrome-0.0.4/pyremotechrome.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyremotechrome
-Version: 0.0.3
+Version: 0.0.4
 Summary: PyRemoteChrome Beta
 Author-email: Wes Wei <lockingonapple@outlook.com>
 Project-URL: Homepage, https://github.com/Wes-KW/PyRemoteChrome
 Project-URL: Issues, https://github.com/Wes-KW/PyRemoteChrome/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `pyremotechrome-0.0.3/pyremotechrome.egg-info/SOURCES.txt` & `pyremotechrome-0.0.4/pyremotechrome.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,10 @@
 LICENSE
 README.md
 pyproject.toml
-dist/pyremotechrome-0.0.1-py3-none-any.whl
-dist/pyremotechrome-0.0.1.tar.gz
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

