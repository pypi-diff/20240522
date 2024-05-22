# Comparing `tmp/fastclip-0.0.8.tar.gz` & `tmp/fastclip-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastclip-0.0.8.tar", last modified: Sun Apr  7 21:11:14 2024, max compression
+gzip compressed data, was "fastclip-0.0.9.tar", last modified: Mon Apr  8 22:35:38 2024, max compression
```

## Comparing `fastclip-0.0.8.tar` & `fastclip-0.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:11:14.667587 fastclip-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-07 21:11:01.000000 fastclip-0.0.8/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 21:11:14.667587 fastclip-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-07 21:11:01.000000 fastclip-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:11:14.663587 fastclip-0.0.8/fastclip/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:11:14.667587 fastclip-0.0.8/fastclip/enums/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/enums/ClipFormat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:11:14.667587 fastclip-0.0.8/fastclip/schemas/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/schemas/AbstractTranscriptComponent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/schemas/ClipPreviewPayload.py
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/schemas/SubtitleSettings.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-07 21:11:01.000000 fastclip-0.0.8/fastclip/schemas/Word.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 21:11:14.667587 fastclip-0.0.8/fastclip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-07 21:11:14.000000 fastclip-0.0.8/fastclip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      398 2024-04-07 21:11:14.000000 fastclip-0.0.8/fastclip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 21:11:14.000000 fastclip-0.0.8/fastclip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 21:11:14.000000 fastclip-0.0.8/fastclip.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 21:11:14.000000 fastclip-0.0.8/fastclip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-07 21:11:14.667587 fastclip-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-07 21:11:01.000000 fastclip-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:35:38.510504 fastclip-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 22:35:27.000000 fastclip-0.0.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 22:35:38.510504 fastclip-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-04-08 22:35:27.000000 fastclip-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:35:38.510504 fastclip-0.0.9/fastclip/
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:35:38.510504 fastclip-0.0.9/fastclip/enums/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/enums/ClipFormat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:35:38.510504 fastclip-0.0.9/fastclip/schemas/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/schemas/AbstractTranscriptComponent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/schemas/ClipPreviewPayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/schemas/ClipSavePayload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/schemas/SubtitleSettings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 22:35:27.000000 fastclip-0.0.9/fastclip/schemas/Word.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 22:35:38.510504 fastclip-0.0.9/fastclip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 22:35:38.000000 fastclip-0.0.9/fastclip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 22:35:38.000000 fastclip-0.0.9/fastclip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 22:35:38.000000 fastclip-0.0.9/fastclip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-08 22:35:38.000000 fastclip-0.0.9/fastclip.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 22:35:38.000000 fastclip-0.0.9/fastclip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-04-08 22:35:38.510504 fastclip-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-08 22:35:27.000000 fastclip-0.0.9/setup.py
```

### Comparing `fastclip-0.0.8/LICENSE.txt` & `fastclip-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fastclip-0.0.8/fastclip/schemas/AbstractTranscriptComponent.py` & `fastclip-0.0.9/fastclip/schemas/AbstractTranscriptComponent.py`

 * *Files identical despite different names*

### Comparing `fastclip-0.0.8/fastclip/schemas/ClipPreviewPayload.py` & `fastclip-0.0.9/fastclip/schemas/ClipPreviewPayload.py`

 * *Files identical despite different names*

### Comparing `fastclip-0.0.8/fastclip/schemas/Word.py` & `fastclip-0.0.9/fastclip/schemas/Word.py`

 * *Files identical despite different names*

### Comparing `fastclip-0.0.8/setup.py` & `fastclip-0.0.9/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from distutils.core import setup
 
 # Edit this to update the package version
-VERSION = "0.0.8"
+VERSION = "0.0.9"
 
 FULL_VERSION = VERSION.replace(".", "")
 
 setup(
     name="fastclip",
     version=VERSION,
     license="MIT",
```

