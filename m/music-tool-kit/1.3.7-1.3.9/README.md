# Comparing `tmp/music-tool-kit-1.3.7.tar.gz` & `tmp/music-tool-kit-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "music-tool-kit-1.3.7.tar", last modified: Wed May 22 07:59:35 2024, max compression
+gzip compressed data, was "music-tool-kit-1.3.9.tar", last modified: Wed May 22 12:10:33 2024, max compression
```

## Comparing `music-tool-kit-1.3.7.tar` & `music-tool-kit-1.3.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:59:35.916125 music-tool-kit-1.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 07:59:15.000000 music-tool-kit-1.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 07:59:35.916125 music-tool-kit-1.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-22 07:59:15.000000 music-tool-kit-1.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:59:35.916125 music-tool-kit-1.3.7/mk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 07:59:15.000000 music-tool-kit-1.3.7/mk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-22 07:59:15.000000 music-tool-kit-1.3.7/mk/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:59:35.916125 music-tool-kit-1.3.7/music_tool_kit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-22 07:59:35.000000 music-tool-kit-1.3.7/music_tool_kit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 07:59:35.916125 music-tool-kit-1.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1681 2024-05-22 07:59:15.000000 music-tool-kit-1.3.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:10:33.741112 music-tool-kit-1.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-22 12:10:15.000000 music-tool-kit-1.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 12:10:33.741112 music-tool-kit-1.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-22 12:10:15.000000 music-tool-kit-1.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:10:33.737112 music-tool-kit-1.3.9/mk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 12:10:15.000000 music-tool-kit-1.3.9/mk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15372 2024-05-22 12:10:15.000000 music-tool-kit-1.3.9/mk/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 12:10:33.741112 music-tool-kit-1.3.9/music_tool_kit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5856 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-05-22 12:10:33.000000 music-tool-kit-1.3.9/music_tool_kit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 12:10:33.741112 music-tool-kit-1.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-22 12:10:26.000000 music-tool-kit-1.3.9/setup.py
```

### Comparing `music-tool-kit-1.3.7/LICENSE` & `music-tool-kit-1.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.7/PKG-INFO` & `music-tool-kit-1.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-tool-kit
-Version: 1.3.7
+Version: 1.3.9
 Summary: A tool kit for music download and clip
 Home-page: https://github.com/nichuanfang/music-tool-kit
 Author: Nichuan Fang
 Author-email: f18326186224@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nichuanfang/music-tool-kit
 Project-URL: Bug Tracker, https://github.com/nichuanfang/music-tool-kit/issues
```

### Comparing `music-tool-kit-1.3.7/README.md` & `music-tool-kit-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.7/mk/__main__.py` & `music-tool-kit-1.3.9/mk/__main__.py`

 * *Files identical despite different names*

### Comparing `music-tool-kit-1.3.7/music_tool_kit.egg-info/PKG-INFO` & `music-tool-kit-1.3.9/music_tool_kit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: music-tool-kit
-Version: 1.3.7
+Version: 1.3.9
 Summary: A tool kit for music download and clip
 Home-page: https://github.com/nichuanfang/music-tool-kit
 Author: Nichuan Fang
 Author-email: f18326186224@gmail.com
 License: MIT
 Project-URL: Source Code, https://github.com/nichuanfang/music-tool-kit
 Project-URL: Bug Tracker, https://github.com/nichuanfang/music-tool-kit/issues
```

### Comparing `music-tool-kit-1.3.7/setup.py` & `music-tool-kit-1.3.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
     readme = f.read()
 
 with open('requirements.txt', 'r', encoding='utf-8') as f:
     requirements = f.read()
 
 setup(
     name='music-tool-kit',
-    version='1.3.7',
+    version='v1.3.9',
     description='A tool kit for music download and clip',
     long_description_content_type='text/markdown',
     long_description=readme,
     url='https://github.com/nichuanfang/music-tool-kit',
 
     project_urls={
         'Source Code': 'https://github.com/nichuanfang/music-tool-kit',
```

