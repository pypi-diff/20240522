# Comparing `tmp/AAVT-0.0.1.tar.gz` & `tmp/AAVT-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AAVT-0.0.1.tar", last modified: Wed May 22 10:43:31 2024, max compression
+gzip compressed data, was "AAVT-0.0.2.tar", last modified: Wed May 22 11:08:38 2024, max compression
```

## Comparing `AAVT-0.0.1.tar` & `AAVT-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 10:43:31.661076 AAVT-0.0.1/
-drwxrwxrwx   0        0        0        0 2024-05-22 10:43:31.645451 AAVT-0.0.1/AAVT.egg-info/
--rw-rw-rw-   0        0        0     1309 2024-05-22 10:43:31.000000 AAVT-0.0.1/AAVT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2024-05-22 10:43:31.000000 AAVT-0.0.1/AAVT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 10:43:31.000000 AAVT-0.0.1/AAVT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-22 10:43:31.000000 AAVT-0.0.1/AAVT.egg-info/requires.txt
--rw-rw-rw-   0        0        0        2 2024-05-22 10:43:31.000000 AAVT-0.0.1/AAVT.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1309 2024-05-22 10:43:31.661076 AAVT-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-22 10:43:31.661076 AAVT-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-22 10:43:31.645451 AAVT-0.0.1/test/
--rw-rw-rw-   0        0        0      894 2024-05-21 15:55:55.000000 AAVT-0.0.1/test/test.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:43:31.661076 AAVT-0.0.1/w/
--rw-rw-rw-   0        0        0      172 2024-05-21 15:28:59.000000 AAVT-0.0.1/w/__init__.py
--rw-rw-rw-   0        0        0     6222 2024-05-21 15:55:35.000000 AAVT-0.0.1/w/blog.py
--rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.0.1/w/merge.py
--rw-rw-rw-   0        0        0     4424 2024-05-21 11:37:39.000000 AAVT-0.0.1/w/translate.py
-drwxrwxrwx   0        0        0        0 2024-05-22 10:43:31.661076 AAVT-0.0.1/w/utils/
--rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.0.1/w/utils/__init__.py
--rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.0.1/w/utils/srt.py
--rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.0.1/w/whisper_faster.py
--rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.0.1/w/whisper_openai.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:38.907388 AAVT-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:38.896389 AAVT-0.0.2/AAVT/
+-rw-rw-rw-   0        0        0        0 2024-05-21 15:55:26.000000 AAVT-0.0.2/AAVT/__init__.py
+-rw-rw-rw-   0        0        0     6222 2024-05-21 15:55:35.000000 AAVT-0.0.2/AAVT/blog.py
+-rw-rw-rw-   0        0        0     3825 2024-05-21 15:41:40.000000 AAVT-0.0.2/AAVT/merge.py
+-rw-rw-rw-   0        0        0     4424 2024-05-21 11:37:39.000000 AAVT-0.0.2/AAVT/translate.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:38.905388 AAVT-0.0.2/AAVT/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-20 03:44:38.000000 AAVT-0.0.2/AAVT/utils/__init__.py
+-rw-rw-rw-   0        0        0     2708 2024-05-20 03:33:29.000000 AAVT-0.0.2/AAVT/utils/srt.py
+-rw-rw-rw-   0        0        0     4202 2024-05-21 11:35:31.000000 AAVT-0.0.2/AAVT/whisper_faster.py
+-rw-rw-rw-   0        0        0     2799 2024-05-21 15:41:40.000000 AAVT-0.0.2/AAVT/whisper_openai.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:08:38.903389 AAVT-0.0.2/AAVT.egg-info/
+-rw-rw-rw-   0        0        0     1339 2024-05-22 11:08:38.000000 AAVT-0.0.2/AAVT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-05-22 11:08:38.000000 AAVT-0.0.2/AAVT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:08:38.000000 AAVT-0.0.2/AAVT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-22 11:08:38.000000 AAVT-0.0.2/AAVT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        5 2024-05-22 11:08:38.000000 AAVT-0.0.2/AAVT.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1339 2024-05-22 11:08:38.907388 AAVT-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      764 2024-05-21 16:12:14.000000 AAVT-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:08:38.907388 AAVT-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      754 2024-05-22 11:08:32.000000 AAVT-0.0.2/setup.py
```

### Comparing `AAVT-0.0.1/AAVT.egg-info/PKG-INFO` & `AAVT-0.0.2/AAVT.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
+License: UNKNOWN
+Description: # Chenyme-AAVT 
+        > AI Auto Video(Audio) Translation
+        
+        Thank you very much for visiting my AI Auto Video-Audio Translation project! This project aims to provide an easy-to-use, fully automatic video translation tool to help you quickly recognize voices and translate subtitles, then merge the translated subtitles with the original video, allowing you to achieve video translation more efficiently.
+        
+        It is recommended to use the Faster-whisper and Large models to obtain the best sentence segmentation and recognition experience.
+        
+        Attention: Before enabling GPU acceleration, you need to download CUDA and PyTorch, and ensure that the PyTorch version matches CUDA. Otherwise, if the program identification fails, GPU acceleration will be disabled by default.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: faster-whisper
-Requires-Dist: openai
-Requires-Dist: opencv-python
-
-# Chenyme-AAVT 
-> AI Auto Video(Audio) Translation
-
-Thank you very much for visiting my AI Auto Video-Audio Translation project! This project aims to provide an easy-to-use, fully automatic video translation tool to help you quickly recognize voices and translate subtitles, then merge the translated subtitles with the original video, allowing you to achieve video translation more efficiently.
-
-It is recommended to use the Faster-whisper and Large models to obtain the best sentence segmentation and recognition experience.
-
-Attention: Before enabling GPU acceleration, you need to download CUDA and PyTorch, and ensure that the PyTorch version matches CUDA. Otherwise, if the program identification fails, GPU acceleration will be disabled by default.
```

### Comparing `AAVT-0.0.1/PKG-INFO` & `AAVT-0.0.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: AAVT
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package for Video Translate and Some Tools for Video
 Home-page: https://github.com/Chenyme/Chenyme-AAVT
 Author: chenyme（Orange橙子）
 Author-email: chenyme03@gmail.com
+License: UNKNOWN
+Description: # Chenyme-AAVT 
+        > AI Auto Video(Audio) Translation
+        
+        Thank you very much for visiting my AI Auto Video-Audio Translation project! This project aims to provide an easy-to-use, fully automatic video translation tool to help you quickly recognize voices and translate subtitles, then merge the translated subtitles with the original video, allowing you to achieve video translation more efficiently.
+        
+        It is recommended to use the Faster-whisper and Large models to obtain the best sentence segmentation and recognition experience.
+        
+        Attention: Before enabling GPU acceleration, you need to download CUDA and PyTorch, and ensure that the PyTorch version matches CUDA. Otherwise, if the program identification fails, GPU acceleration will be disabled by default.
+        
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: faster-whisper
-Requires-Dist: openai
-Requires-Dist: opencv-python
-
-# Chenyme-AAVT 
-> AI Auto Video(Audio) Translation
-
-Thank you very much for visiting my AI Auto Video-Audio Translation project! This project aims to provide an easy-to-use, fully automatic video translation tool to help you quickly recognize voices and translate subtitles, then merge the translated subtitles with the original video, allowing you to achieve video translation more efficiently.
-
-It is recommended to use the Faster-whisper and Large models to obtain the best sentence segmentation and recognition experience.
-
-Attention: Before enabling GPU acceleration, you need to download CUDA and PyTorch, and ensure that the PyTorch version matches CUDA. Otherwise, if the program identification fails, GPU acceleration will be disabled by default.
```

### Comparing `AAVT-0.0.1/w/blog.py` & `AAVT-0.0.2/AAVT/blog.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.1/w/merge.py` & `AAVT-0.0.2/AAVT/merge.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.1/w/translate.py` & `AAVT-0.0.2/AAVT/translate.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.1/w/utils/srt.py` & `AAVT-0.0.2/AAVT/utils/srt.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.1/w/whisper_faster.py` & `AAVT-0.0.2/AAVT/whisper_faster.py`

 * *Files identical despite different names*

### Comparing `AAVT-0.0.1/w/whisper_openai.py` & `AAVT-0.0.2/AAVT/whisper_openai.py`

 * *Files identical despite different names*

