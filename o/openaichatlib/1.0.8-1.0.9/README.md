# Comparing `tmp/openaichatlib-1.0.8.tar.gz` & `tmp/openaichatlib-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openaichatlib-1.0.8.tar", last modified: Sun Apr 28 02:33:22 2024, max compression
+gzip compressed data, was "openaichatlib-1.0.9.tar", last modified: Wed May 22 08:33:03 2024, max compression
```

## Comparing `openaichatlib-1.0.8.tar` & `openaichatlib-1.0.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:33:22.180790 openaichatlib-1.0.8/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.8/LICENSE
--rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 02:33:22.180079 openaichatlib-1.0.8/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.8/README.md
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:33:22.176055 openaichatlib-1.0.8/openaichatlib/
--rw-r--r--   0 chenshuai   (501) staff       (20)    18691 2024-04-28 02:33:18.000000 openaichatlib-1.0.8/openaichatlib/V3.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.8/openaichatlib/__init__.py
--rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.8/openaichatlib/typings.py
--rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.8/openaichatlib/utils.py
--rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.8/openaichatlib/version.py
-drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-04-28 02:33:22.179309 openaichatlib-1.0.8/openaichatlib.egg-info/
--rw-r--r--   0 chenshuai   (501) staff       (20)     1314 2024-04-28 02:33:22.000000 openaichatlib-1.0.8/openaichatlib.egg-info/PKG-INFO
--rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-04-28 02:33:22.000000 openaichatlib-1.0.8/openaichatlib.egg-info/SOURCES.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-04-28 02:33:22.000000 openaichatlib-1.0.8/openaichatlib.egg-info/dependency_links.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       45 2024-04-28 02:33:22.000000 openaichatlib-1.0.8/openaichatlib.egg-info/requires.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-04-28 02:33:22.000000 openaichatlib-1.0.8/openaichatlib.egg-info/top_level.txt
--rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-04-28 02:33:22.180995 openaichatlib-1.0.8/setup.cfg
--rw-r--r--   0 chenshuai   (501) staff       (20)     1164 2024-04-28 02:33:18.000000 openaichatlib-1.0.8/setup.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.680343 openaichatlib-1.0.9/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1063 2024-03-01 02:06:24.000000 openaichatlib-1.0.9/LICENSE
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 08:33:03.679817 openaichatlib-1.0.9/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      558 2024-03-06 07:58:11.000000 openaichatlib-1.0.9/README.md
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.676477 openaichatlib-1.0.9/openaichatlib/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     8147 2024-05-22 08:32:14.000000 openaichatlib-1.0.9/openaichatlib/V3.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      894 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/__init__.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)     2047 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/typings.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)      825 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/utils.py
+-rw-r--r--   0 chenshuai   (501) staff       (20)       18 2024-04-28 00:54:42.000000 openaichatlib-1.0.9/openaichatlib/version.py
+drwxr-xr-x   0 chenshuai   (501) staff       (20)        0 2024-05-22 08:33:03.679233 openaichatlib-1.0.9/openaichatlib.egg-info/
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1255 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/PKG-INFO
+-rw-r--r--   0 chenshuai   (501) staff       (20)      329 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/SOURCES.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)        1 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/dependency_links.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       16 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/requires.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       14 2024-05-22 08:33:03.000000 openaichatlib-1.0.9/openaichatlib.egg-info/top_level.txt
+-rw-r--r--   0 chenshuai   (501) staff       (20)       38 2024-05-22 08:33:03.680451 openaichatlib-1.0.9/setup.cfg
+-rw-r--r--   0 chenshuai   (501) staff       (20)     1121 2024-05-22 08:32:14.000000 openaichatlib-1.0.9/setup.py
```

### Comparing `openaichatlib-1.0.8/LICENSE` & `openaichatlib-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.8/PKG-INFO` & `openaichatlib-1.0.9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,17 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx[socks]
 Requires-Dist: requests[socks]
-Requires-Dist: tiktoken>=0.3.0
 
 # OpenAI Chat Python Lib
 
 ## Requirements
 ```
 python: >=3.9
 ```
```

### Comparing `openaichatlib-1.0.8/README.md` & `openaichatlib-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.8/openaichatlib/__init__.py` & `openaichatlib-1.0.9/openaichatlib/__init__.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.8/openaichatlib/typings.py` & `openaichatlib-1.0.9/openaichatlib/typings.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.8/openaichatlib/utils.py` & `openaichatlib-1.0.9/openaichatlib/utils.py`

 * *Files identical despite different names*

### Comparing `openaichatlib-1.0.8/openaichatlib.egg-info/PKG-INFO` & `openaichatlib-1.0.9/openaichatlib.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openaichatlib
-Version: 1.0.8
+Version: 1.0.9
 Summary: OpenAI Chat API
 Home-page: https://github.com/IAn2018cs/OpenAIChatLib
 Author: IAn2018
 Author-email: ian2018cs@gmail.com
 Keywords: openai,ChatGPT,api,chat
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
@@ -12,17 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.9, <3.13
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: httpx[socks]
 Requires-Dist: requests[socks]
-Requires-Dist: tiktoken>=0.3.0
 
 # OpenAI Chat Python Lib
 
 ## Requirements
 ```
 python: >=3.9
 ```
```

### Comparing `openaichatlib-1.0.8/setup.py` & `openaichatlib-1.0.9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,22 +8,20 @@
 from setuptools import find_packages, setup
 
 here = pathlib.Path(__file__).parent.resolve()
 
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 install_requires = [
-    "httpx[socks]",
     "requests[socks]",
-    "tiktoken>=0.3.0",
 ]
 
 setup(
     name="openaichatlib",
-    version="1.0.8",
+    version="1.0.9",
     description="OpenAI Chat API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/IAn2018cs/OpenAIChatLib",
     author="IAn2018",
     author_email="ian2018cs@gmail.com",
     classifiers=[
```

