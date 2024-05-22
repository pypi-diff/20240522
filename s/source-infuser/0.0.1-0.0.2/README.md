# Comparing `tmp/source_infuser-0.0.1.tar.gz` & `tmp/source_infuser-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "source_infuser-0.0.1.tar", last modified: Wed May 22 20:14:51 2024, max compression
+gzip compressed data, was "source_infuser-0.0.2.tar", last modified: Wed May 22 20:28:42 2024, max compression
```

## Comparing `source_infuser-0.0.1.tar` & `source_infuser-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,22 @@
-drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:14:51.348538 source_infuser-0.0.1/
--rw-r--r--   0 Administrator   (501) staff       (20)     2501 2024-05-22 20:14:51.347805 source_infuser-0.0.1/PKG-INFO
--rw-r--r--   0 Administrator   (501) staff       (20)     2001 2024-05-22 19:37:45.000000 source_infuser-0.0.1/README.md
--rw-r--r--   0 Administrator   (501) staff       (20)       38 2024-05-22 20:14:51.348759 source_infuser-0.0.1/setup.cfg
--rw-r--r--   0 Administrator   (501) staff       (20)     1131 2024-05-22 20:14:27.000000 source_infuser-0.0.1/setup.py
-drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:14:51.341962 source_infuser-0.0.1/source_infuser/
--rw-r--r--   0 Administrator   (501) staff       (20)      110 2024-05-22 19:53:20.000000 source_infuser-0.0.1/source_infuser/__init__.py
--rw-r--r--   0 Administrator   (501) staff       (20)      910 2024-05-21 13:55:28.000000 source_infuser-0.0.1/source_infuser/ignore.py
--rw-r--r--   0 Administrator   (501) staff       (20)     1895 2024-05-21 13:55:48.000000 source_infuser-0.0.1/source_infuser/logic.py
--rw-r--r--   0 Administrator   (501) staff       (20)      581 2024-05-21 13:47:14.000000 source_infuser-0.0.1/source_infuser/logs.py
-drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:14:51.346894 source_infuser-0.0.1/source_infuser.egg-info/
--rw-r--r--   0 Administrator   (501) staff       (20)     2501 2024-05-22 20:14:51.000000 source_infuser-0.0.1/source_infuser.egg-info/PKG-INFO
--rw-r--r--   0 Administrator   (501) staff       (20)      349 2024-05-22 20:14:51.000000 source_infuser-0.0.1/source_infuser.egg-info/SOURCES.txt
--rw-r--r--   0 Administrator   (501) staff       (20)        1 2024-05-22 20:14:51.000000 source_infuser-0.0.1/source_infuser.egg-info/dependency_links.txt
--rw-r--r--   0 Administrator   (501) staff       (20)       83 2024-05-22 20:14:51.000000 source_infuser-0.0.1/source_infuser.egg-info/entry_points.txt
--rw-r--r--   0 Administrator   (501) staff       (20)       15 2024-05-22 20:14:51.000000 source_infuser-0.0.1/source_infuser.egg-info/top_level.txt
-drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:14:51.346108 source_infuser-0.0.1/test/
--rw-r--r--   0 Administrator   (501) staff       (20)      540 2024-05-22 18:57:26.000000 source_infuser-0.0.1/test/test_ignore.py
--rw-r--r--   0 Administrator   (501) staff       (20)      347 2024-05-22 18:05:44.000000 source_infuser-0.0.1/test/test_logic.py
+drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:28:42.706369 source_infuser-0.0.2/
+-rw-r--r--   0 Administrator   (501) staff       (20)     2501 2024-05-22 20:28:42.705587 source_infuser-0.0.2/PKG-INFO
+-rw-r--r--   0 Administrator   (501) staff       (20)     2001 2024-05-22 19:37:45.000000 source_infuser-0.0.2/README.md
+-rw-r--r--   0 Administrator   (501) staff       (20)       38 2024-05-22 20:28:42.706505 source_infuser-0.0.2/setup.cfg
+-rw-r--r--   0 Administrator   (501) staff       (20)     1161 2024-05-22 20:24:47.000000 source_infuser-0.0.2/setup.py
+drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:28:42.699620 source_infuser-0.0.2/source_infuser/
+-rw-r--r--   0 Administrator   (501) staff       (20)      110 2024-05-22 20:28:23.000000 source_infuser-0.0.2/source_infuser/__init__.py
+-rw-r--r--   0 Administrator   (501) staff       (20)      910 2024-05-21 13:55:28.000000 source_infuser-0.0.2/source_infuser/ignore.py
+-rw-r--r--   0 Administrator   (501) staff       (20)     1895 2024-05-21 13:55:48.000000 source_infuser-0.0.2/source_infuser/logic.py
+-rw-r--r--   0 Administrator   (501) staff       (20)      581 2024-05-21 13:47:14.000000 source_infuser-0.0.2/source_infuser/logs.py
+drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:28:42.702874 source_infuser-0.0.2/source_infuser/scripts/
+-rw-r--r--   0 Administrator   (501) staff       (20)        0 2024-05-22 20:22:20.000000 source_infuser-0.0.2/source_infuser/scripts/__init__.py
+-rw-r--r--   0 Administrator   (501) staff       (20)      871 2024-05-21 13:57:23.000000 source_infuser-0.0.2/source_infuser/scripts/infuser.py
+drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:28:42.704801 source_infuser-0.0.2/source_infuser.egg-info/
+-rw-r--r--   0 Administrator   (501) staff       (20)     2501 2024-05-22 20:28:42.000000 source_infuser-0.0.2/source_infuser.egg-info/PKG-INFO
+-rw-r--r--   0 Administrator   (501) staff       (20)      418 2024-05-22 20:28:42.000000 source_infuser-0.0.2/source_infuser.egg-info/SOURCES.txt
+-rw-r--r--   0 Administrator   (501) staff       (20)        1 2024-05-22 20:28:42.000000 source_infuser-0.0.2/source_infuser.egg-info/dependency_links.txt
+-rw-r--r--   0 Administrator   (501) staff       (20)      113 2024-05-22 20:28:42.000000 source_infuser-0.0.2/source_infuser.egg-info/entry_points.txt
+-rw-r--r--   0 Administrator   (501) staff       (20)       15 2024-05-22 20:28:42.000000 source_infuser-0.0.2/source_infuser.egg-info/top_level.txt
+drwxr-xr-x   0 Administrator   (501) staff       (20)        0 2024-05-22 20:28:42.704097 source_infuser-0.0.2/test/
+-rw-r--r--   0 Administrator   (501) staff       (20)      540 2024-05-22 18:57:26.000000 source_infuser-0.0.2/test/test_ignore.py
+-rw-r--r--   0 Administrator   (501) staff       (20)      347 2024-05-22 18:05:44.000000 source_infuser-0.0.2/test/test_logic.py
```

### Comparing `source_infuser-0.0.1/PKG-INFO` & `source_infuser-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: source_infuser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to prepare your software project for continuous infusion into your AI assistant
 Home-page: https://github.com/ivanzhovannik/source-infuser
 Author: Ivan Zhovannik
 Author-email: i.zhovannik@maastrichtuniversity.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `source_infuser-0.0.1/README.md` & `source_infuser-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `source_infuser-0.0.1/setup.py` & `source_infuser-0.0.2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,12 +26,12 @@
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
     python_requires='>=3.9',
     entry_points={
         'console_scripts': [
-            'source_infuser=scripts.infuser:main',
-            'psi=scripts.infuser:main'
+            'source_infuser=source_infuser.scripts.infuser:main',
+            'psi=source_infuser.scripts.infuser:main'
         ],
     },
 )
```

### Comparing `source_infuser-0.0.1/source_infuser/ignore.py` & `source_infuser-0.0.2/source_infuser/ignore.py`

 * *Files identical despite different names*

### Comparing `source_infuser-0.0.1/source_infuser/logic.py` & `source_infuser-0.0.2/source_infuser/logic.py`

 * *Files identical despite different names*

### Comparing `source_infuser-0.0.1/source_infuser/logs.py` & `source_infuser-0.0.2/source_infuser/logs.py`

 * *Files identical despite different names*

### Comparing `source_infuser-0.0.1/source_infuser.egg-info/PKG-INFO` & `source_infuser-0.0.2/source_infuser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: source_infuser
-Version: 0.0.1
+Version: 0.0.2
 Summary: A package to prepare your software project for continuous infusion into your AI assistant
 Home-page: https://github.com/ivanzhovannik/source-infuser
 Author: Ivan Zhovannik
 Author-email: i.zhovannik@maastrichtuniversity.nl
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `source_infuser-0.0.1/test/test_ignore.py` & `source_infuser-0.0.2/test/test_ignore.py`

 * *Files identical despite different names*

