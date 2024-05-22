# Comparing `tmp/pyrympro-0.0.7.tar.gz` & `tmp/pyrympro-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrympro-0.0.7.tar", last modified: Sat Feb  4 14:22:01 2023, max compression
+gzip compressed data, was "pyrympro-0.0.8.tar", last modified: Wed May 22 09:46:41 2024, max compression
```

## Comparing `pyrympro-0.0.7.tar` & `pyrympro-0.0.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2023-02-04 14:22:01.234538 pyrympro-0.0.7/
--rw-r--r--   0 onfreund   (501) staff       (20)     1065 2022-12-25 17:08:57.000000 pyrympro-0.0.7/LICENSE
--rw-r--r--   0 onfreund   (501) staff       (20)       25 2022-12-25 07:47:36.000000 pyrympro-0.0.7/MANIFEST.in
--rw-r--r--   0 onfreund   (501) staff       (20)     1235 2023-02-04 14:22:01.233962 pyrympro-0.0.7/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)      556 2022-12-25 16:34:49.000000 pyrympro-0.0.7/README.md
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2023-02-04 14:22:01.230348 pyrympro-0.0.7/pyrympro/
--rw-r--r--   0 onfreund   (501) staff       (20)       82 2022-12-25 08:31:25.000000 pyrympro-0.0.7/pyrympro/__init__.py
--rw-r--r--   0 onfreund   (501) staff       (20)      672 2023-02-04 14:18:55.000000 pyrympro-0.0.7/pyrympro/const.py
--rw-r--r--   0 onfreund   (501) staff       (20)     4592 2023-02-04 14:17:41.000000 pyrympro-0.0.7/pyrympro/rympro.py
-drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2023-02-04 14:22:01.233234 pyrympro-0.0.7/pyrympro.egg-info/
--rw-r--r--   0 onfreund   (501) staff       (20)     1235 2023-02-04 14:22:01.000000 pyrympro-0.0.7/pyrympro.egg-info/PKG-INFO
--rw-r--r--   0 onfreund   (501) staff       (20)      255 2023-02-04 14:22:01.000000 pyrympro-0.0.7/pyrympro.egg-info/SOURCES.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        1 2023-02-04 14:22:01.000000 pyrympro-0.0.7/pyrympro.egg-info/dependency_links.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        8 2023-02-04 14:22:01.000000 pyrympro-0.0.7/pyrympro.egg-info/requires.txt
--rw-r--r--   0 onfreund   (501) staff       (20)        9 2023-02-04 14:22:01.000000 pyrympro-0.0.7/pyrympro.egg-info/top_level.txt
--rw-r--r--   0 onfreund   (501) staff       (20)       38 2023-02-04 14:22:01.234871 pyrympro-0.0.7/setup.cfg
--rw-r--r--   0 onfreund   (501) staff       (20)     3414 2023-02-04 14:21:35.000000 pyrympro-0.0.7/setup.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-22 09:46:41.015303 pyrympro-0.0.8/
+-rw-r--r--   0 onfreund   (501) staff       (20)     1065 2022-12-25 17:08:57.000000 pyrympro-0.0.8/LICENSE
+-rw-r--r--   0 onfreund   (501) staff       (20)       25 2022-12-25 07:47:36.000000 pyrympro-0.0.8/MANIFEST.in
+-rw-r--r--   0 onfreund   (501) staff       (20)     1258 2024-05-22 09:46:41.009052 pyrympro-0.0.8/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)      556 2022-12-25 16:34:49.000000 pyrympro-0.0.8/README.md
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-22 09:46:40.881419 pyrympro-0.0.8/pyrympro/
+-rw-r--r--   0 onfreund   (501) staff       (20)       82 2022-12-25 08:31:25.000000 pyrympro-0.0.8/pyrympro/__init__.py
+-rw-r--r--   0 onfreund   (501) staff       (20)      580 2024-05-22 09:43:05.000000 pyrympro-0.0.8/pyrympro/const.py
+-rw-r--r--   0 onfreund   (501) staff       (20)     4592 2023-02-04 14:17:41.000000 pyrympro-0.0.8/pyrympro/rympro.py
+drwxr-xr-x   0 onfreund   (501) staff       (20)        0 2024-05-22 09:46:41.008012 pyrympro-0.0.8/pyrympro.egg-info/
+-rw-r--r--   0 onfreund   (501) staff       (20)     1258 2024-05-22 09:46:40.000000 pyrympro-0.0.8/pyrympro.egg-info/PKG-INFO
+-rw-r--r--   0 onfreund   (501) staff       (20)      255 2024-05-22 09:46:40.000000 pyrympro-0.0.8/pyrympro.egg-info/SOURCES.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        1 2024-05-22 09:46:40.000000 pyrympro-0.0.8/pyrympro.egg-info/dependency_links.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        8 2024-05-22 09:46:40.000000 pyrympro-0.0.8/pyrympro.egg-info/requires.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)        9 2024-05-22 09:46:40.000000 pyrympro-0.0.8/pyrympro.egg-info/top_level.txt
+-rw-r--r--   0 onfreund   (501) staff       (20)       38 2024-05-22 09:46:41.015544 pyrympro-0.0.8/setup.cfg
+-rw-r--r--   0 onfreund   (501) staff       (20)     3414 2024-05-22 09:46:18.000000 pyrympro-0.0.8/setup.py
```

### Comparing `pyrympro-0.0.7/LICENSE` & `pyrympro-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrympro-0.0.7/PKG-INFO` & `pyrympro-0.0.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrympro
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library to communitcate with Read Your Meter Pro (https://rym-pro.com/).
 Home-page: https://github.com/OnFreund/pyrympro
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 
 # pyrympro
 
 A python library to communitcate with [Read Your Meter Pro](https://rym-pro.com/).
 
 ## Installation
```

### Comparing `pyrympro-0.0.7/README.md` & `pyrympro-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `pyrympro-0.0.7/pyrympro/rympro.py` & `pyrympro-0.0.8/pyrympro/rympro.py`

 * *Files identical despite different names*

### Comparing `pyrympro-0.0.7/pyrympro.egg-info/PKG-INFO` & `pyrympro-0.0.8/pyrympro.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: pyrympro
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python library to communitcate with Read Your Meter Pro (https://rym-pro.com/).
 Home-page: https://github.com/OnFreund/pyrympro
 Author: On Freund
 Author-email: onfreund@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp
 
 
 # pyrympro
 
 A python library to communitcate with [Read Your Meter Pro](https://rym-pro.com/).
 
 ## Installation
```

### Comparing `pyrympro-0.0.7/setup.py` & `pyrympro-0.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 # Package meta-data.
 NAME = 'pyrympro'
 DESCRIPTION = 'A python library to communitcate with Read Your Meter Pro (https://rym-pro.com/).'
 URL = 'https://github.com/OnFreund/pyrympro'
 EMAIL = 'onfreund@gmail.com'
 AUTHOR = 'On Freund'
 REQUIRES_PYTHON = '>=3.10.0'
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 
 REQUIRED = ['aiohttp']
 
 EXTRAS = {}
 
 
 here = os.path.abspath(os.path.dirname(__file__))
```

