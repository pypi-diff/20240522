# Comparing `tmp/sklearntools-0.3.0.tar.gz` & `tmp/sklearntools-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sklearntools-0.3.0.tar", last modified: Tue May 21 10:55:39 2024, max compression
+gzip compressed data, was "sklearntools-0.4.0.tar", last modified: Tue May 21 15:34:04 2024, max compression
```

## Comparing `sklearntools-0.3.0.tar` & `sklearntools-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.964308 sklearntools-0.3.0/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:55:39.963662 sklearntools-0.3.0/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.3.0/README.rst
--rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 10:55:39.964582 sklearntools-0.3.0/setup.cfg
--rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 10:55:30.000000 sklearntools-0.3.0/setup.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.958923 sklearntools-0.3.0/sklearntools/
--rw-r--r--   0 summy      (501) staff       (20)     5089 2024-05-21 10:52:41.000000 sklearntools-0.3.0/sklearntools/__init__.py
-drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 10:55:39.962786 sklearntools-0.3.0/sklearntools.egg-info/
--rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/PKG-INFO
--rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/SOURCES.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/dependency_links.txt
--rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/not-zip-safe
--rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/requires.txt
--rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 10:55:39.000000 sklearntools-0.3.0/sklearntools.egg-info/top_level.txt
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.042734 sklearntools-0.4.0/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 15:34:04.041021 sklearntools-0.4.0/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      761 2024-05-21 10:29:01.000000 sklearntools-0.4.0/README.rst
+-rw-r--r--   0 summy      (501) staff       (20)       38 2024-05-21 15:34:04.042925 sklearntools-0.4.0/setup.cfg
+-rw-r--r--   0 summy      (501) staff       (20)      882 2024-05-21 15:33:58.000000 sklearntools-0.4.0/setup.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.030913 sklearntools-0.4.0/sklearntools/
+-rw-r--r--   0 summy      (501) staff       (20)     6978 2024-05-21 15:31:57.000000 sklearntools-0.4.0/sklearntools/__init__.py
+drwxr-xr-x   0 summy      (501) staff       (20)        0 2024-05-21 15:34:04.039939 sklearntools-0.4.0/sklearntools.egg-info/
+-rw-r--r--   0 summy      (501) staff       (20)     1061 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/PKG-INFO
+-rw-r--r--   0 summy      (501) staff       (20)      258 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/SOURCES.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/dependency_links.txt
+-rw-r--r--   0 summy      (501) staff       (20)        1 2024-05-21 10:55:39.000000 sklearntools-0.4.0/sklearntools.egg-info/not-zip-safe
+-rw-r--r--   0 summy      (501) staff       (20)       32 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/requires.txt
+-rw-r--r--   0 summy      (501) staff       (20)       13 2024-05-21 15:34:03.000000 sklearntools-0.4.0/sklearntools.egg-info/top_level.txt
```

### Comparing `sklearntools-0.3.0/PKG-INFO` & `sklearntools-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

### Comparing `sklearntools-0.3.0/README.rst` & `sklearntools-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `sklearntools-0.3.0/setup.py` & `sklearntools-0.4.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 setup(
     name='sklearntools',
     packages=['sklearntools'],
     description="Tools of sklearn.",
     long_description=long_description,
     long_description_content_type='text/markdown',
-    version='0.3.0',
+    version='0.4.0',
     install_requires=[
         'joblib>=1.1.0',
         'scikit-learn>=1.0',
     ],
     url='https://gitee.com/summry/sklearntools',
     author='summy',
     author_email='xiazhongbiao@126.com',
```

### Comparing `sklearntools-0.3.0/sklearntools.egg-info/PKG-INFO` & `sklearntools-0.4.0/sklearntools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sklearntools
-Version: 0.3.0
+Version: 0.4.0
 Summary: Tools of sklearn.
 Home-page: https://gitee.com/summry/sklearntools
 Author: summy
 Author-email: xiazhongbiao@126.com
 License: UNKNOWN
 Keywords: sklearn
 Platform: UNKNOWN
```

