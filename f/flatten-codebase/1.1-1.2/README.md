# Comparing `tmp/flatten-codebase-1.1.tar.gz` & `tmp/flatten-codebase-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatten-codebase-1.1.tar", last modified: Tue May 21 20:00:12 2024, max compression
+gzip compressed data, was "flatten-codebase-1.2.tar", last modified: Tue May 21 20:03:21 2024, max compression
```

## Comparing `flatten-codebase-1.1.tar` & `flatten-codebase-1.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:00:12.816369 flatten-codebase-1.1/
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     3314 2024-05-21 20:00:12.816369 flatten-codebase-1.1/PKG-INFO
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     2739 2024-05-21 19:40:45.000000 flatten-codebase-1.1/README.md
-drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:00:12.816369 flatten-codebase-1.1/flatten_codebase/
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 19:57:33.000000 flatten-codebase-1.1/flatten_codebase/__init__.py
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     1801 2024-05-21 13:46:41.000000 flatten-codebase-1.1/flatten_codebase/main.py
-drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:00:12.816369 flatten-codebase-1.1/flatten_codebase.egg-info/
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     3314 2024-05-21 20:00:12.000000 flatten-codebase-1.1/flatten_codebase.egg-info/PKG-INFO
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)      275 2024-05-21 20:00:12.000000 flatten-codebase-1.1/flatten_codebase.egg-info/SOURCES.txt
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)        1 2024-05-21 20:00:12.000000 flatten-codebase-1.1/flatten_codebase.egg-info/dependency_links.txt
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       65 2024-05-21 20:00:12.000000 flatten-codebase-1.1/flatten_codebase.egg-info/entry_points.txt
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       17 2024-05-21 20:00:12.000000 flatten-codebase-1.1/flatten_codebase.egg-info/top_level.txt
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       38 2024-05-21 20:00:12.816369 flatten-codebase-1.1/setup.cfg
--rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)      887 2024-05-21 20:00:04.000000 flatten-codebase-1.1/setup.py
+drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:03:21.704370 flatten-codebase-1.2/
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     3314 2024-05-21 20:03:21.704370 flatten-codebase-1.2/PKG-INFO
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     2739 2024-05-21 19:40:45.000000 flatten-codebase-1.2/README.md
+drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:03:21.704370 flatten-codebase-1.2/flatten_codebase/
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       30 2024-05-21 20:03:10.000000 flatten-codebase-1.2/flatten_codebase/__init__.py
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     1801 2024-05-21 13:46:41.000000 flatten-codebase-1.2/flatten_codebase/main.py
+drwxrwxr-x   0 victor.henrique  (7374) victor.henrique (11376)        0 2024-05-21 20:03:21.704370 flatten-codebase-1.2/flatten_codebase.egg-info/
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)     3314 2024-05-21 20:03:21.000000 flatten-codebase-1.2/flatten_codebase.egg-info/PKG-INFO
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)      275 2024-05-21 20:03:21.000000 flatten-codebase-1.2/flatten_codebase.egg-info/SOURCES.txt
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)        1 2024-05-21 20:03:21.000000 flatten-codebase-1.2/flatten_codebase.egg-info/dependency_links.txt
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       65 2024-05-21 20:03:21.000000 flatten-codebase-1.2/flatten_codebase.egg-info/entry_points.txt
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       17 2024-05-21 20:03:21.000000 flatten-codebase-1.2/flatten_codebase.egg-info/top_level.txt
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)       38 2024-05-21 20:03:21.704370 flatten-codebase-1.2/setup.cfg
+-rw-rw-r--   0 victor.henrique  (7374) victor.henrique (11376)      887 2024-05-21 20:03:18.000000 flatten-codebase-1.2/setup.py
```

### Comparing `flatten-codebase-1.1/PKG-INFO` & `flatten-codebase-1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatten-codebase
-Version: 1.1
+Version: 1.2
 Summary: Flatten Codebase simplifies codebase preparation for Language Models by converting it into a single Markdown file, making it easier for the developer to provide the codebase to the LM
 Home-page: https://github.com/VictorHenrique317/flatten-codebase
 Author: Victor Henrique Silva Ribeiro
 Author-email: victor.henrique5800@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flatten-codebase-1.1/README.md` & `flatten-codebase-1.2/README.md`

 * *Files identical despite different names*

### Comparing `flatten-codebase-1.1/flatten_codebase/main.py` & `flatten-codebase-1.2/flatten_codebase/main.py`

 * *Files identical despite different names*

### Comparing `flatten-codebase-1.1/flatten_codebase.egg-info/PKG-INFO` & `flatten-codebase-1.2/flatten_codebase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatten-codebase
-Version: 1.1
+Version: 1.2
 Summary: Flatten Codebase simplifies codebase preparation for Language Models by converting it into a single Markdown file, making it easier for the developer to provide the codebase to the LM
 Home-page: https://github.com/VictorHenrique317/flatten-codebase
 Author: Victor Henrique Silva Ribeiro
 Author-email: victor.henrique5800@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `flatten-codebase-1.1/setup.py` & `flatten-codebase-1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='flatten-codebase',
-    version='1.1',
+    version='1.2',
     packages=find_packages(),
     description="Flatten Codebase simplifies codebase preparation for Language Models by converting it into a single Markdown file, making it easier for the developer to provide the codebase to the LM",
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     author='Victor Henrique Silva Ribeiro',
     author_email='victor.henrique5800@gmail.com',
     url='https://github.com/VictorHenrique317/flatten-codebase',
```

