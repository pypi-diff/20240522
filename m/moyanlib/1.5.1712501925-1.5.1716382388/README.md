# Comparing `tmp/moyanlib-1.5.1712501925.tar.gz` & `tmp/moyanlib-1.5.1716382388.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moyanlib-1.5.1712501925.tar", last modified: Sun Apr  7 14:58:46 2024, max compression
+gzip compressed data, was "moyanlib-1.5.1716382388.tar", last modified: Wed May 22 12:53:08 2024, max compression
```

## Comparing `moyanlib-1.5.1712501925.tar` & `moyanlib-1.5.1716382388.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/Error.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/cache.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/jsons.py
--rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/moyanlib/system.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.051429 moyanlib-1.5.1712501925/moyanlib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 14:58:46.000000 moyanlib-1.5.1712501925/moyanlib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:46.055429 moyanlib-1.5.1712501925/test/
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_dec.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-07 14:58:32.000000 moyanlib-1.5.1712501925/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:53:08.552605 moyanlib-1.5.1716382388/moyanlib/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/Error.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/cache.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/moyanlib/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1980 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2070 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/jsons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1384 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/moyanlib/system.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/moyanlib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 12:53:08.000000 moyanlib-1.5.1716382388/moyanlib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:53:08.556606 moyanlib-1.5.1716382388/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/test/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/test/test_dec.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/test/test_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-22 12:52:50.000000 moyanlib-1.5.1716382388/test/test_utils.py
```

### Comparing `moyanlib-1.5.1712501925/moyanlib/__init__.py` & `moyanlib-1.5.1716382388/moyanlib/__init__.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/cache.py` & `moyanlib-1.5.1716382388/moyanlib/cache.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/cli/__init__.py` & `moyanlib-1.5.1716382388/moyanlib/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/decorators.py` & `moyanlib-1.5.1716382388/moyanlib/decorators.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/jsons.py` & `moyanlib-1.5.1716382388/moyanlib/jsons.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/logger.py` & `moyanlib-1.5.1716382388/moyanlib/logger.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/moyanlib/system.py` & `moyanlib-1.5.1716382388/moyanlib/system.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/setup.py` & `moyanlib-1.5.1716382388/setup.py`

 * *Files identical despite different names*

### Comparing `moyanlib-1.5.1712501925/test/test_cache.py` & `moyanlib-1.5.1716382388/test/test_cache.py`

 * *Files identical despite different names*

