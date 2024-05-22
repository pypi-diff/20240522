# Comparing `tmp/composio_openai-0.2.61.tar.gz` & `tmp/composio_openai-0.2.62.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_openai-0.2.61.tar", last modified: Tue May 21 20:13:27 2024, max compression
+gzip compressed data, was "composio_openai-0.2.62.tar", last modified: Wed May 22 10:40:42 2024, max compression
```

## Comparing `composio_openai-0.2.61.tar` & `composio_openai-0.2.62.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.728754 composio_openai-0.2.61/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-21 20:13:27.728551 composio_openai-0.2.61/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)     2107 2024-05-02 07:57:45.000000 composio_openai-0.2.61/README.md
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.727485 composio_openai-0.2.61/composio_openai/
--rw-r--r--   0 sawradip   (501) staff       (20)      213 2024-05-20 14:09:13.000000 composio_openai-0.2.61/composio_openai/__init__.py
--rw-r--r--   0 sawradip   (501) staff       (20)     5403 2024-05-21 20:07:08.000000 composio_openai-0.2.61/composio_openai/openai_toolspec.py
-drwxr-xr-x   0 sawradip   (501) staff       (20)        0 2024-05-21 20:13:27.728309 composio_openai-0.2.61/composio_openai.egg-info/
--rw-r--r--   0 sawradip   (501) staff       (20)     2615 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/PKG-INFO
--rw-r--r--   0 sawradip   (501) staff       (20)      275 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/SOURCES.txt
--rw-r--r--   0 sawradip   (501) staff       (20)        1 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/dependency_links.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       23 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/requires.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       16 2024-05-21 20:13:27.000000 composio_openai-0.2.61/composio_openai.egg-info/top_level.txt
--rw-r--r--   0 sawradip   (501) staff       (20)       38 2024-05-21 20:13:27.728793 composio_openai-0.2.61/setup.cfg
--rw-r--r--   0 sawradip   (501) staff       (20)      811 2024-05-21 20:12:30.000000 composio_openai-0.2.61/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:42.929775 composio_openai-0.2.62/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-22 10:40:42.929590 composio_openai-0.2.62/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2107 2024-05-05 16:54:48.000000 composio_openai-0.2.62/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:42.928628 composio_openai-0.2.62/composio_openai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      213 2024-05-20 14:51:26.000000 composio_openai-0.2.62/composio_openai/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5403 2024-05-22 10:40:02.000000 composio_openai-0.2.62/composio_openai/openai_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-05-22 10:40:42.929370 composio_openai-0.2.62/composio_openai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2615 2024-05-22 10:40:42.000000 composio_openai-0.2.62/composio_openai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      275 2024-05-22 10:40:42.000000 composio_openai-0.2.62/composio_openai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-05-22 10:40:42.000000 composio_openai-0.2.62/composio_openai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       23 2024-05-22 10:40:42.000000 composio_openai-0.2.62/composio_openai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-05-22 10:40:42.000000 composio_openai-0.2.62/composio_openai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-05-22 10:40:42.929811 composio_openai-0.2.62/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      811 2024-05-22 10:40:15.000000 composio_openai-0.2.62/setup.py
```

### Comparing `composio_openai-0.2.61/PKG-INFO` & `composio_openai-0.2.62/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.61
+Version: 0.2.62
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.61
+Requires-Dist: composio_core===0.2.62
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

### Comparing `composio_openai-0.2.61/README.md` & `composio_openai-0.2.62/README.md`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.61/composio_openai/openai_toolspec.py` & `composio_openai-0.2.62/composio_openai/openai_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_openai-0.2.61/composio_openai.egg-info/PKG-INFO` & `composio_openai-0.2.62/composio_openai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_openai
-Version: 0.2.61
+Version: 0.2.62
 Summary: Use Composio to get an array of tools with your OpenAI Function Call.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9,<4
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.61
+Requires-Dist: composio_core===0.2.62
 
 ## 🚀🔗 Leveraging OpenAI with Composio
 
 Facilitate the integration of OpenAI with Composio to empower OpenAI models to directly interact with external applications, broadening their capabilities and application scope.
 
 ### Objective
```

