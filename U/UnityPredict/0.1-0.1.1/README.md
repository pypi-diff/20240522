# Comparing `tmp/UnityPredict-0.1.tar.gz` & `tmp/UnityPredict-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UnityPredict-0.1.tar", last modified: Tue May 21 16:10:21 2024, max compression
+gzip compressed data, was "UnityPredict-0.1.1.tar", last modified: Wed May 22 06:42:54 2024, max compression
```

## Comparing `UnityPredict-0.1.tar` & `UnityPredict-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-05-21 16:10:21.839105 UnityPredict-0.1/
--rw-rw-rw-   0        0        0       57 2024-05-21 16:10:21.838091 UnityPredict-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      485 2024-05-19 18:00:59.000000 UnityPredict-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-21 16:10:21.832102 UnityPredict-0.1/UnityPredict/
--rw-rw-rw-   0        0        0     3306 2024-05-19 13:56:42.000000 UnityPredict-0.1/UnityPredict/Models.py
--rw-rw-rw-   0        0        0     2383 2024-05-11 17:05:18.000000 UnityPredict-0.1/UnityPredict/Platform.py
--rw-rw-rw-   0        0        0    18322 2024-05-21 16:10:04.000000 UnityPredict-0.1/UnityPredict/UnityPredictLocalHost.py
--rw-rw-rw-   0        0        0       53 2024-05-12 18:12:20.000000 UnityPredict-0.1/UnityPredict/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-21 16:10:21.836092 UnityPredict-0.1/UnityPredict.egg-info/
--rw-rw-rw-   0        0        0       57 2024-05-21 16:10:21.000000 UnityPredict-0.1/UnityPredict.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      273 2024-05-21 16:10:21.000000 UnityPredict-0.1/UnityPredict.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-21 16:10:21.000000 UnityPredict-0.1/UnityPredict.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-21 16:10:21.000000 UnityPredict-0.1/UnityPredict.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-21 16:10:21.839105 UnityPredict-0.1/setup.cfg
--rw-rw-rw-   0        0        0      262 2024-05-18 08:43:01.000000 UnityPredict-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 06:42:54.782687 UnityPredict-0.1.1/
+-rw-rw-rw-   0        0        0     6879 2024-05-22 06:42:54.781689 UnityPredict-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6775 2024-05-22 04:27:19.000000 UnityPredict-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 06:42:54.777691 UnityPredict-0.1.1/UnityPredict/
+-rw-rw-rw-   0        0        0     3306 2024-05-19 13:56:42.000000 UnityPredict-0.1.1/UnityPredict/Models.py
+-rw-rw-rw-   0        0        0     2383 2024-05-11 17:05:18.000000 UnityPredict-0.1.1/UnityPredict/Platform.py
+-rw-rw-rw-   0        0        0    18322 2024-05-21 16:10:04.000000 UnityPredict-0.1.1/UnityPredict/UnityPredictLocalHost.py
+-rw-rw-rw-   0        0        0       53 2024-05-12 18:12:20.000000 UnityPredict-0.1.1/UnityPredict/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 06:42:54.780688 UnityPredict-0.1.1/UnityPredict.egg-info/
+-rw-rw-rw-   0        0        0     6879 2024-05-22 06:42:54.000000 UnityPredict-0.1.1/UnityPredict.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-22 06:42:54.000000 UnityPredict-0.1.1/UnityPredict.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 06:42:54.000000 UnityPredict-0.1.1/UnityPredict.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-22 06:42:54.000000 UnityPredict-0.1.1/UnityPredict.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 06:42:54.783688 UnityPredict-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      439 2024-05-22 06:42:49.000000 UnityPredict-0.1.1/setup.py
```

### Comparing `UnityPredict-0.1/UnityPredict/Models.py` & `UnityPredict-0.1.1/UnityPredict/Models.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1/UnityPredict/Platform.py` & `UnityPredict-0.1.1/UnityPredict/Platform.py`

 * *Files identical despite different names*

### Comparing `UnityPredict-0.1/UnityPredict/UnityPredictLocalHost.py` & `UnityPredict-0.1.1/UnityPredict/UnityPredictLocalHost.py`

 * *Files identical despite different names*

