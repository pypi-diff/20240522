# Comparing `tmp/AAVT-0.0.3.tar.gz` & `tmp/AAVT-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAVT-0.0.3.tar", last modified: Wed May 22 11:18:13 2024, max compression
+gzip compressed data, was "AAVT-0.0.4.tar", last modified: Wed May 22 11:24:50 2024, max compression
```

## Comparing `AAVT-0.0.3.tar` & `AAVT-0.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 11:18:13.530226 AAVT-0.0.3/
-drwxrwxrwx   0        0        0        0 2024-05-22 11:18:13.518646 AAVT-0.0.3/AAVT/
--rw-rw-rw-   0        0        0      172 2024-05-22 11:15:57.000000 AAVT-0.0.3/AAVT/__init__.py
--rw-rw-rw-   0        0        0     6222 2024-05-21 15:55:35.000000 AAVT-0.0.3/AAVT/blog.py
--rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.0.3/AAVT/merge.py
--rw-rw-rw-   0        0        0     4424 2024-05-21 11:37:39.000000 AAVT-0.0.3/AAVT/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:18:13.527647 AAVT-0.0.3/AAVT/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.0.3/AAVT/utils/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.0.3/AAVT/utils/srt.py
--rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.0.3/AAVT/whisper_faster.py
--rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.0.3/AAVT/whisper_openai.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:18:13.525646 AAVT-0.0.3/AAVT.egg-info/
--rw-rw-rw-   0        0        0     1339 2024-05-22 11:18:13.000000 AAVT-0.0.3/AAVT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-05-22 11:18:13.000000 AAVT-0.0.3/AAVT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:18:13.000000 AAVT-0.0.3/AAVT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-22 11:18:13.000000 AAVT-0.0.3/AAVT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        5 2024-05-22 11:18:13.000000 AAVT-0.0.3/AAVT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1339 2024-05-22 11:18:13.529645 AAVT-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      764 2024-05-21 16:12:14.000000 AAVT-0.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 11:18:13.530226 AAVT-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      754 2024-05-22 11:18:11.000000 AAVT-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:50.056268 AAVT-0.0.4/
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:50.044271 AAVT-0.0.4/AAVT/
+-rw-rw-rw-   0        0        0      172 2024-05-22 11:23:11.000000 AAVT-0.0.4/AAVT/__init__.py
+-rw-rw-rw-   0        0        0     6220 2024-05-22 11:24:21.000000 AAVT-0.0.4/AAVT/blog.py
+-rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.0.4/AAVT/merge.py
+-rw-rw-rw-   0        0        0     4424 2024-05-21 11:37:39.000000 AAVT-0.0.4/AAVT/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:50.054268 AAVT-0.0.4/AAVT/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.0.4/AAVT/utils/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.0.4/AAVT/utils/srt.py
+-rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.0.4/AAVT/whisper_faster.py
+-rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.0.4/AAVT/whisper_openai.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:50.051268 AAVT-0.0.4/AAVT.egg-info/
+-rw-rw-rw-   0        0        0     1339 2024-05-22 11:24:49.000000 AAVT-0.0.4/AAVT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-22 11:24:49.000000 AAVT-0.0.4/AAVT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:24:49.000000 AAVT-0.0.4/AAVT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-22 11:24:49.000000 AAVT-0.0.4/AAVT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 11:24:49.000000 AAVT-0.0.4/AAVT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2024-05-22 11:24:50.056268 AAVT-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2024-05-21 16:12:14.000000 AAVT-0.0.4/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:24:50.056268 AAVT-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      754 2024-05-22 11:24:41.000000 AAVT-0.0.4/setup.py
```

### Comparing `AAVT-0.0.3/AAVT/blog.py` & `AAVT-0.0.4/AAVT/blog.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import cv2
 import base64
 from openai import OpenAI
-from w.whisper_openai import whisper_openai
-from w.whisper_faster import whisper_faster
+from .whisper_openai import whisper_openai
+from .whisper_faster import whisper_faster
 from .utils.srt import generate_srt_from_result
 
 
 def blog(video_path: str, api_key: str, base_url: str = "https://api.openai.com/v1", vision: str = "视频作者",
          whisper_model: str = "api", local_model: str = None, temperature: float = 0.8, output_path: str = None) -> str:
     file_name = os.path.basename(video_path)
     if file_name.split('.')[-1] != "mp4":
```

### Comparing `AAVT-0.0.3/AAVT/merge.py` & `AAVT-0.0.4/AAVT/merge.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/AAVT/translate.py` & `AAVT-0.0.4/AAVT/translate.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/AAVT/utils/srt.py` & `AAVT-0.0.4/AAVT/utils/srt.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/AAVT/whisper_faster.py` & `AAVT-0.0.4/AAVT/whisper_faster.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/AAVT/whisper_openai.py` & `AAVT-0.0.4/AAVT/whisper_openai.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/AAVT.egg-info/PKG-INFO` & `AAVT-0.0.4/AAVT.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
 License: UNKNOWN
 Description: # Chenyme-AAVT 
         > AI Auto Video(Audio) Translation
```

### Comparing `AAVT-0.0.3/PKG-INFO` & `AAVT-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.0.3
+Version: 0.0.4
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
 License: UNKNOWN
 Description: # Chenyme-AAVT 
         > AI Auto Video(Audio) Translation
```

### Comparing `AAVT-0.0.3/README.md` & `AAVT-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.3/setup.py` & `AAVT-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='AAVT',
-    version='0.0.3',
+    version='0.0.4',
     packages=find_packages(),
     install_requires=[
         'faster-whisper',
         'openai',
         'opencv-python',
     ],
     description='A Python package for Video Translate and Some Tools for Video',
```

