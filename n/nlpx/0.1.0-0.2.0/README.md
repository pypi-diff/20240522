# Comparing `tmp/nlpx-0.1.0.tar.gz` & `tmp/nlpx-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpx-0.1.0.tar", last modified: Tue May 21 12:04:38 2024, max compression
+gzip compressed data, was "nlpx-0.2.0.tar", last modified: Wed May 22 02:11:06 2024, max compression
```

## Comparing `nlpx-0.1.0.tar` & `nlpx-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 12:04:38.285051 nlpx-0.1.0/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-21 12:04:38.284054 nlpx-0.1.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.1.0/README.rst
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 12:04:38.277312 nlpx-0.1.0/nlpx/
--rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.1.0/nlpx/__init__.py
--rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.1.0/nlpx/text_token.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 12:04:38.282737 nlpx-0.1.0/nlpx.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-21 12:04:38.000000 nlpx-0.1.0/nlpx.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      194 2024-05-21 12:04:38.000000 nlpx-0.1.0/nlpx.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 12:04:38.000000 nlpx-0.1.0/nlpx.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 12:04:38.000000 nlpx-0.1.0/nlpx.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-21 12:04:38.000000 nlpx-0.1.0/nlpx.egg-info/top_level.txt
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 12:04:38.285406 nlpx-0.1.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-21 12:04:30.000000 nlpx-0.1.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.590511 nlpx-0.2.0/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-22 02:11:06.589764 nlpx-0.2.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      448 2024-04-07 01:09:43.000000 nlpx-0.2.0/README.rst
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.582520 nlpx-0.2.0/nlpx/
+-rw-r--r--   0 summy      (501) staff       (20)        0 2024-05-21 11:15:55.000000 nlpx-0.2.0/nlpx/__init__.py
+-rw-r--r--   0 summy      (501) staff       (20)    41701 2024-04-07 00:53:15.000000 nlpx-0.2.0/nlpx/text_token.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-22 02:11:06.587431 nlpx-0.2.0/nlpx.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)      730 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      194 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)        5 2024-05-22 02:11:06.000000 nlpx-0.2.0/nlpx.egg-info/top_level.txt
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-22 02:11:06.590764 nlpx-0.2.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      998 2024-05-22 02:11:00.000000 nlpx-0.2.0/setup.py
```

### Comparing `nlpx-0.1.0/PKG-INFO` & `nlpx-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.1.0/nlpx/text_token.py` & `nlpx-0.2.0/nlpx/text_token.py`

 * *Files identical despite different names*

### Comparing `nlpx-0.1.0/nlpx.egg-info/PKG-INFO` & `nlpx-0.2.0/nlpx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpx
-Version: 0.1.0
+Version: 0.2.0
 Summary: A tool set for NLP.
 Home-page: https://gitee.com/summry/nlpx
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: NLP
 Platform: UNKNOWN
```

### Comparing `nlpx-0.1.0/setup.py` & `nlpx-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 setup(
     name='nlpx',
     packages=['nlpx'],
     description="A tool set for NLP.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.1.0',
+    version='0.2.0',
     url='https://gitee.com/summry/nlpx',
     author='summy',
     author_email='xiazhongbiao@126.com',
     keywords=['NLP'],
     package_data={
         # include json and txt files
         '': ['*.rst', '*.dtd', '*.tpl'],
```

