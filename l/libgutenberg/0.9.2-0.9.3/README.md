# Comparing `tmp/libgutenberg-0.9.2.tar.gz` & `tmp/libgutenberg-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/libgutenberg-0.9.2.tar", last modified: Fri Jun 17 18:21:55 2022, max compression
+gzip compressed data, was "dist/libgutenberg-0.9.3.tar", last modified: Fri Jun 17 18:24:38 2022, max compression
```

## Comparing `libgutenberg-0.9.2.tar` & `libgutenberg-0.9.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/
--rw-r--r--   0 eric       (501) staff       (20)    35141 2017-04-21 20:50:26.000000 libgutenberg-0.9.2/LICENSE
--rw-r--r--   0 eric       (501) staff       (20)      965 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      231 2022-03-29 20:39:05.000000 libgutenberg-0.9.2/README.md
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/libgutenberg/
--rw-r--r--   0 eric       (501) staff       (20)      273 2019-10-22 17:18:47.000000 libgutenberg-0.9.2/libgutenberg/CommonOptions.py
--rwxr-xr-x   0 eric       (501) staff       (20)    28526 2020-10-17 21:52:39.000000 libgutenberg-0.9.2/libgutenberg/Cover.py
--rw-r--r--   0 eric       (501) staff       (20)     3148 2021-09-03 21:52:12.000000 libgutenberg-0.9.2/libgutenberg/DBUtils.py
--rw-r--r--   0 eric       (501) staff       (20)    29774 2022-06-08 15:40:11.000000 libgutenberg-0.9.2/libgutenberg/DublinCore.py
--rw-r--r--   0 eric       (501) staff       (20)    15201 2022-04-06 22:10:31.000000 libgutenberg-0.9.2/libgutenberg/DublinCoreMapping.py
--rw-r--r--   0 eric       (501) staff       (20)      491 2020-11-23 16:43:55.000000 libgutenberg-0.9.2/libgutenberg/DummyConnectionPool.py
--rw-r--r--   0 eric       (501) staff       (20)     4253 2022-03-29 20:40:20.000000 libgutenberg-0.9.2/libgutenberg/GutenbergDatabase.py
--rw-r--r--   0 eric       (501) staff       (20)    13626 2022-04-06 22:11:53.000000 libgutenberg-0.9.2/libgutenberg/GutenbergDatabaseDublinCore.py
--rw-r--r--   0 eric       (501) staff       (20)     6457 2021-11-17 03:50:57.000000 libgutenberg-0.9.2/libgutenberg/GutenbergFiles.py
--rw-r--r--   0 eric       (501) staff       (20)    12946 2022-02-04 19:14:21.000000 libgutenberg-0.9.2/libgutenberg/GutenbergGlobals.py
--rw-r--r--   0 eric       (501) staff       (20)     2311 2022-06-17 17:18:38.000000 libgutenberg-0.9.2/libgutenberg/Logger.py
--rw-r--r--   0 eric       (501) staff       (20)     2925 2022-01-19 15:28:34.000000 libgutenberg-0.9.2/libgutenberg/MediaTypes.py
--rw-r--r--   0 eric       (501) staff       (20)    21972 2021-08-26 16:29:41.000000 libgutenberg-0.9.2/libgutenberg/Models.py
--rw-r--r--   0 eric       (501) staff       (20)      212 2019-10-22 17:18:47.000000 libgutenberg-0.9.2/libgutenberg/__init__.py
-drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/libgutenberg.egg-info/
--rw-r--r--   0 eric       (501) staff       (20)      965 2022-06-17 18:21:54.000000 libgutenberg-0.9.2/libgutenberg.egg-info/PKG-INFO
--rw-r--r--   0 eric       (501) staff       (20)      618 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/libgutenberg.egg-info/SOURCES.txt
--rw-r--r--   0 eric       (501) staff       (20)        1 2022-06-17 18:21:54.000000 libgutenberg-0.9.2/libgutenberg.egg-info/dependency_links.txt
--rw-r--r--   0 eric       (501) staff       (20)       99 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/libgutenberg.egg-info/requires.txt
--rw-r--r--   0 eric       (501) staff       (20)       13 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/libgutenberg.egg-info/top_level.txt
--rw-r--r--   0 eric       (501) staff       (20)       38 2022-06-17 18:21:55.000000 libgutenberg-0.9.2/setup.cfg
--rw-r--r--   0 eric       (501) staff       (20)     1513 2022-06-17 18:21:20.000000 libgutenberg-0.9.2/setup.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/
+-rw-r--r--   0 eric       (501) staff       (20)    35141 2017-04-21 20:50:26.000000 libgutenberg-0.9.3/LICENSE
+-rw-r--r--   0 eric       (501) staff       (20)      965 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      231 2022-03-29 20:39:05.000000 libgutenberg-0.9.3/README.md
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/libgutenberg/
+-rw-r--r--   0 eric       (501) staff       (20)      273 2019-10-22 17:18:47.000000 libgutenberg-0.9.3/libgutenberg/CommonOptions.py
+-rwxr-xr-x   0 eric       (501) staff       (20)    28526 2020-10-17 21:52:39.000000 libgutenberg-0.9.3/libgutenberg/Cover.py
+-rw-r--r--   0 eric       (501) staff       (20)     3148 2021-09-03 21:52:12.000000 libgutenberg-0.9.3/libgutenberg/DBUtils.py
+-rw-r--r--   0 eric       (501) staff       (20)    29774 2022-06-08 15:40:11.000000 libgutenberg-0.9.3/libgutenberg/DublinCore.py
+-rw-r--r--   0 eric       (501) staff       (20)    15201 2022-04-06 22:10:31.000000 libgutenberg-0.9.3/libgutenberg/DublinCoreMapping.py
+-rw-r--r--   0 eric       (501) staff       (20)      491 2020-11-23 16:43:55.000000 libgutenberg-0.9.3/libgutenberg/DummyConnectionPool.py
+-rw-r--r--   0 eric       (501) staff       (20)     4253 2022-03-29 20:40:20.000000 libgutenberg-0.9.3/libgutenberg/GutenbergDatabase.py
+-rw-r--r--   0 eric       (501) staff       (20)    13626 2022-04-06 22:11:53.000000 libgutenberg-0.9.3/libgutenberg/GutenbergDatabaseDublinCore.py
+-rw-r--r--   0 eric       (501) staff       (20)     6457 2021-11-17 03:50:57.000000 libgutenberg-0.9.3/libgutenberg/GutenbergFiles.py
+-rw-r--r--   0 eric       (501) staff       (20)    12946 2022-02-04 19:14:21.000000 libgutenberg-0.9.3/libgutenberg/GutenbergGlobals.py
+-rw-r--r--   0 eric       (501) staff       (20)     2311 2022-06-17 18:22:38.000000 libgutenberg-0.9.3/libgutenberg/Logger.py
+-rw-r--r--   0 eric       (501) staff       (20)     2925 2022-01-19 15:28:34.000000 libgutenberg-0.9.3/libgutenberg/MediaTypes.py
+-rw-r--r--   0 eric       (501) staff       (20)    21972 2021-08-26 16:29:41.000000 libgutenberg-0.9.3/libgutenberg/Models.py
+-rw-r--r--   0 eric       (501) staff       (20)      212 2019-10-22 17:18:47.000000 libgutenberg-0.9.3/libgutenberg/__init__.py
+drwxr-xr-x   0 eric       (501) staff       (20)        0 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/libgutenberg.egg-info/
+-rw-r--r--   0 eric       (501) staff       (20)      965 2022-06-17 18:24:37.000000 libgutenberg-0.9.3/libgutenberg.egg-info/PKG-INFO
+-rw-r--r--   0 eric       (501) staff       (20)      618 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/libgutenberg.egg-info/SOURCES.txt
+-rw-r--r--   0 eric       (501) staff       (20)        1 2022-06-17 18:24:37.000000 libgutenberg-0.9.3/libgutenberg.egg-info/dependency_links.txt
+-rw-r--r--   0 eric       (501) staff       (20)       99 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/libgutenberg.egg-info/requires.txt
+-rw-r--r--   0 eric       (501) staff       (20)       13 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/libgutenberg.egg-info/top_level.txt
+-rw-r--r--   0 eric       (501) staff       (20)       38 2022-06-17 18:24:38.000000 libgutenberg-0.9.3/setup.cfg
+-rw-r--r--   0 eric       (501) staff       (20)     1513 2022-06-17 18:23:19.000000 libgutenberg-0.9.3/setup.py
```

### Comparing `libgutenberg-0.9.2/LICENSE` & `libgutenberg-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/PKG-INFO` & `libgutenberg-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgutenberg
-Version: 0.9.2
+Version: 0.9.3
 Summary: Common files used by Project Gutenberg python projects.
 Home-page: https://github.com/gutenbergtools/libgutenberg/
 Author: Marcello Perathoner
 Maintainer: Eric Hellman
 Maintainer-email: eric@hellman.net
 License: GPL v3
 Keywords: project gutenberg
```

### Comparing `libgutenberg-0.9.2/libgutenberg/Cover.py` & `libgutenberg-0.9.3/libgutenberg/Cover.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/DBUtils.py` & `libgutenberg-0.9.3/libgutenberg/DBUtils.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/DublinCore.py` & `libgutenberg-0.9.3/libgutenberg/DublinCore.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/DublinCoreMapping.py` & `libgutenberg-0.9.3/libgutenberg/DublinCoreMapping.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/GutenbergDatabase.py` & `libgutenberg-0.9.3/libgutenberg/GutenbergDatabase.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/GutenbergDatabaseDublinCore.py` & `libgutenberg-0.9.3/libgutenberg/GutenbergDatabaseDublinCore.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/GutenbergFiles.py` & `libgutenberg-0.9.3/libgutenberg/GutenbergFiles.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/GutenbergGlobals.py` & `libgutenberg-0.9.3/libgutenberg/GutenbergGlobals.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/Logger.py` & `libgutenberg-0.9.3/libgutenberg/Logger.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -52,22 +52,22 @@
 
 
 
 def setup(logformat, logfile=None, loglevel=logging.INFO, notifier=None):
     """ Setup logger. """
 
     # StreamHandler defaults to sys.stderr
+    logger = logging.getLogger()
     if logfile: 
         file_handler = logging.FileHandler(logfile) 
     else: 
         if logger.hasHandlers():
             logger.handlers.clear()        
         file_handler = logging.StreamHandler()
     file_handler.setFormatter(CustomFormatter(logformat))
-    logger = logging.getLogger()
     logger.addHandler(file_handler)
     if notifier:
         notify_handler = NotificationHandler(notifier=notifier)
         logger.addHandler(notify_handler)
     logger.setLevel(loglevel)
     return file_handler
```

### Comparing `libgutenberg-0.9.2/libgutenberg/MediaTypes.py` & `libgutenberg-0.9.3/libgutenberg/MediaTypes.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg/Models.py` & `libgutenberg-0.9.3/libgutenberg/Models.py`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/libgutenberg.egg-info/PKG-INFO` & `libgutenberg-0.9.3/libgutenberg.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libgutenberg
-Version: 0.9.2
+Version: 0.9.3
 Summary: Common files used by Project Gutenberg python projects.
 Home-page: https://github.com/gutenbergtools/libgutenberg/
 Author: Marcello Perathoner
 Maintainer: Eric Hellman
 Maintainer-email: eric@hellman.net
 License: GPL v3
 Keywords: project gutenberg
```

### Comparing `libgutenberg-0.9.2/libgutenberg.egg-info/SOURCES.txt` & `libgutenberg-0.9.3/libgutenberg.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libgutenberg-0.9.2/setup.py` & `libgutenberg-0.9.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 #
 # libgutenberg setup.py
 #
 
-__version__ = '0.9.2'
+__version__ = '0.9.3'
 
 from setuptools import setup
 
 setup (
     name         = 'libgutenberg',
     version      = __version__,
```

