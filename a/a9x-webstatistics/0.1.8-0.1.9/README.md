# Comparing `tmp/a9x_webstatistics-0.1.8.tar.gz` & `tmp/a9x_webstatistics-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics-0.1.8.tar", last modified: Sat May 11 19:02:02 2024, max compression
+gzip compressed data, was "a9x_webstatistics-0.1.9.tar", last modified: Sun May 12 12:56:45 2024, max compression
```

## Comparing `a9x_webstatistics-0.1.8.tar` & `a9x_webstatistics-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/dist_del
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.481813 a9x_webstatistics-0.1.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.481813 a9x_webstatistics-0.1.8/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/module1.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics/updatestatistics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-11 19:02:02.000000 a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-11 19:02:02.485813 a9x_webstatistics-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_main001.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_main010.py
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-11 19:01:52.000000 a9x_webstatistics-0.1.8/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15480 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/dist_del
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6091 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/module1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2358 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics/updatestatistics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.625467 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16544 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-12 12:56:45.000000 a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 12:56:45.621467 a9x_webstatistics-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      858 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_main001.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_main010.py
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-05-12 12:56:29.000000 a9x_webstatistics-0.1.9/tests/test_module1.py
```

### Comparing `a9x_webstatistics-0.1.8/LICENSE` & `a9x_webstatistics-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.8/PKG-INFO` & `a9x_webstatistics-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.8
+Version: 0.1.9
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.8/README.md` & `a9x_webstatistics-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.8/setup.py` & `a9x_webstatistics-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.8/src/a9x_webstatistics/main.py` & `a9x_webstatistics-0.1.9/src/a9x_webstatistics/main.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.8/src/a9x_webstatistics/updatestatistics.py` & `a9x_webstatistics-0.1.9/src/a9x_webstatistics/updatestatistics.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     else:
         d['days'][dt]['serverResponseCode'][i['status']] = 1
 
     # process country if available:
     if 'country' in i:
         if 'countries' not in d['days'][dt]:
             d['days'][dt]['countries'] = {}
+        if i['country'] not in d['days'][dt]['countries']:
             d['days'][dt]['countries'][i['country']] = 0;
         d['days'][dt]['countries'][i['country']] = d['days'][dt]['countries'][i['country']] + 1;
 
     # update hits for device types:
     devCla = detectDeviceClass(i['user_agent']) 
     if devCla not in d['days'][dt]['device_hits']:
         d['days'][dt]['device_hits'][devCla] = 0
```

### Comparing `a9x_webstatistics-0.1.8/src/a9x_webstatistics.egg-info/PKG-INFO` & `a9x_webstatistics-0.1.9/src/a9x_webstatistics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics
-Version: 0.1.8
+Version: 0.1.9
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
```

### Comparing `a9x_webstatistics-0.1.8/tests/test_main001.py` & `a9x_webstatistics-0.1.9/tests/test_main001.py`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics-0.1.8/tests/test_main010.py` & `a9x_webstatistics-0.1.9/tests/test_main010.py`

 * *Files identical despite different names*

