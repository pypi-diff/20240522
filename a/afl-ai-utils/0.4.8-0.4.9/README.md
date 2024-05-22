# Comparing `tmp/afl-ai-utils-0.4.8.tar.gz` & `tmp/afl-ai-utils-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "afl-ai-utils-0.4.8.tar", last modified: Wed May 15 07:16:57 2024, max compression
+gzip compressed data, was "afl-ai-utils-0.4.9.tar", last modified: Wed May 22 06:05:04 2024, max compression
```

## Comparing `afl-ai-utils-0.4.8.tar` & `afl-ai-utils-0.4.9.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.373898 afl-ai-utils-0.4.8/
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.8/LICENSE
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-15 07:16:57.373628 afl-ai-utils-0.4.8/PKG-INFO
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2407 2023-11-10 08:42:51.000000 afl-ai-utils-0.4.8/README.md
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.371581 afl-ai-utils-0.4.8/afl_ai_utils/
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-20 08:02:33.000000 afl-ai-utils-0.4.8/afl_ai_utils/__init__.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     7308 2024-05-15 07:16:24.000000 afl-ai-utils-0.4.8/afl_ai_utils/bigquery_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)       36 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.8/afl_ai_utils/consts.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     4991 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.8/afl_ai_utils/drive_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     4996 2023-11-29 16:38:37.000000 afl-ai-utils-0.4.8/afl_ai_utils/email_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     1132 2024-03-28 12:10:06.000000 afl-ai-utils-0.4.8/afl_ai_utils/microsoft_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-04-01 09:52:23.000000 afl-ai-utils-0.4.8/afl_ai_utils/ms_api.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-03-28 14:25:52.000000 afl-ai-utils-0.4.8/afl_ai_utils/office365_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)    11871 2024-04-01 08:50:54.000000 afl-ai-utils-0.4.8/afl_ai_utils/outlook_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     3357 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.8/afl_ai_utils/selenium_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     1375 2024-04-08 08:08:34.000000 afl-ai-utils-0.4.8/afl_ai_utils/sftp_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2063 2023-11-10 08:39:25.000000 afl-ai-utils-0.4.8/afl_ai_utils/slack_utils.py
--rw-r--r--   0 abhaykumar   (502) staff       (20)    16225 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.8/afl_ai_utils/text_utils.py
-drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-15 07:16:57.373197 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/
--rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/PKG-INFO
--rw-r--r--   0 abhaykumar   (502) staff       (20)      570 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/SOURCES.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)        1 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/dependency_links.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       88 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/requires.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       13 2024-05-15 07:16:57.000000 afl-ai-utils-0.4.8/afl_ai_utils.egg-info/top_level.txt
--rw-r--r--   0 abhaykumar   (502) staff       (20)       38 2024-05-15 07:16:57.373954 afl-ai-utils-0.4.8/setup.cfg
--rw-r--r--   0 abhaykumar   (502) staff       (20)      612 2024-05-15 07:16:45.000000 afl-ai-utils-0.4.8/setup.py
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-22 06:05:04.138920 afl-ai-utils-0.4.9/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.9/LICENSE
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-22 06:05:04.138590 afl-ai-utils-0.4.9/PKG-INFO
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2407 2023-11-10 08:42:51.000000 afl-ai-utils-0.4.9/README.md
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-22 06:05:04.135809 afl-ai-utils-0.4.9/afl_ai_utils/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2023-10-20 08:02:33.000000 afl-ai-utils-0.4.9/afl_ai_utils/__init__.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     7308 2024-05-15 07:16:24.000000 afl-ai-utils-0.4.9/afl_ai_utils/bigquery_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       36 2023-10-19 13:42:39.000000 afl-ai-utils-0.4.9/afl_ai_utils/consts.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     4991 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.9/afl_ai_utils/drive_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     4996 2023-11-29 16:38:37.000000 afl-ai-utils-0.4.9/afl_ai_utils/email_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     1132 2024-03-28 12:10:06.000000 afl-ai-utils-0.4.9/afl_ai_utils/microsoft_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-04-01 09:52:23.000000 afl-ai-utils-0.4.9/afl_ai_utils/ms_api.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        0 2024-03-28 14:25:52.000000 afl-ai-utils-0.4.9/afl_ai_utils/office365_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)    11871 2024-04-01 08:50:54.000000 afl-ai-utils-0.4.9/afl_ai_utils/outlook_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)      882 2024-05-22 05:34:55.000000 afl-ai-utils-0.4.9/afl_ai_utils/secrets_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     3357 2024-03-04 10:23:21.000000 afl-ai-utils-0.4.9/afl_ai_utils/selenium_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     1375 2024-04-08 08:08:34.000000 afl-ai-utils-0.4.9/afl_ai_utils/sftp_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2063 2023-11-10 08:39:25.000000 afl-ai-utils-0.4.9/afl_ai_utils/slack_utils.py
+-rw-r--r--   0 abhaykumar   (502) staff       (20)    16225 2023-12-22 11:43:29.000000 afl-ai-utils-0.4.9/afl_ai_utils/text_utils.py
+drwxr-xr-x   0 abhaykumar   (502) staff       (20)        0 2024-05-22 06:05:04.138155 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/
+-rw-r--r--   0 abhaykumar   (502) staff       (20)     2729 2024-05-22 06:05:04.000000 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/PKG-INFO
+-rw-r--r--   0 abhaykumar   (502) staff       (20)      600 2024-05-22 06:05:04.000000 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)        1 2024-05-22 06:05:04.000000 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       88 2024-05-22 06:05:04.000000 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/requires.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       13 2024-05-22 06:05:04.000000 afl-ai-utils-0.4.9/afl_ai_utils.egg-info/top_level.txt
+-rw-r--r--   0 abhaykumar   (502) staff       (20)       38 2024-05-22 06:05:04.138995 afl-ai-utils-0.4.9/setup.cfg
+-rw-r--r--   0 abhaykumar   (502) staff       (20)      612 2024-05-22 06:04:44.000000 afl-ai-utils-0.4.9/setup.py
```

### Comparing `afl-ai-utils-0.4.8/PKG-INFO` & `afl-ai-utils-0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afl-ai-utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: A sample test package
 Home-page: https://github.com/gituser/test-tackage
 Author: Abhay Kumar
 Author-email: abhay.kumar@arvindbrands.co.in
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `afl-ai-utils-0.4.8/README.md` & `afl-ai-utils-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/bigquery_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/bigquery_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/drive_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/drive_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/email_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/email_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/microsoft_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/microsoft_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/outlook_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/outlook_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/selenium_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/selenium_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/sftp_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/sftp_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/slack_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/slack_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils/text_utils.py` & `afl-ai-utils-0.4.9/afl_ai_utils/text_utils.py`

 * *Files identical despite different names*

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils.egg-info/PKG-INFO` & `afl-ai-utils-0.4.9/afl_ai_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: afl-ai-utils
-Version: 0.4.8
+Version: 0.4.9
 Summary: A sample test package
 Home-page: https://github.com/gituser/test-tackage
 Author: Abhay Kumar
 Author-email: abhay.kumar@arvindbrands.co.in
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `afl-ai-utils-0.4.8/afl_ai_utils.egg-info/SOURCES.txt` & `afl-ai-utils-0.4.9/afl_ai_utils.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 afl_ai_utils/consts.py
 afl_ai_utils/drive_utils.py
 afl_ai_utils/email_utils.py
 afl_ai_utils/microsoft_utils.py
 afl_ai_utils/ms_api.py
 afl_ai_utils/office365_utils.py
 afl_ai_utils/outlook_utils.py
+afl_ai_utils/secrets_utils.py
 afl_ai_utils/selenium_utils.py
 afl_ai_utils/sftp_utils.py
 afl_ai_utils/slack_utils.py
 afl_ai_utils/text_utils.py
 afl_ai_utils.egg-info/PKG-INFO
 afl_ai_utils.egg-info/SOURCES.txt
 afl_ai_utils.egg-info/dependency_links.txt
```

### Comparing `afl-ai-utils-0.4.8/setup.py` & `afl-ai-utils-0.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     description = fh.read()
 
 setuptools.setup(
     name="afl-ai-utils",
-    version="0.4.8",
+    version="0.4.9",
     author="Abhay Kumar",
     author_email="abhay.kumar@arvindbrands.co.in",
     packages=["afl_ai_utils"],
     description="A sample test package",
     long_description=description,
     long_description_content_type="text/markdown",
     url="https://github.com/gituser/test-tackage",
```

