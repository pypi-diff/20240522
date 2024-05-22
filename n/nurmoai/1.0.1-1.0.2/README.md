# Comparing `tmp/nurmoai-1.0.1.tar.gz` & `tmp/nurmoai-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nurmoai-1.0.1.tar", last modified: Tue May 21 14:41:55 2024, max compression
+gzip compressed data, was "nurmoai-1.0.2.tar", last modified: Wed May 22 14:13:58 2024, max compression
```

## Comparing `nurmoai-1.0.1.tar` & `nurmoai-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:41:55.620899 nurmoai-1.0.1/
--rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-05-21 14:41:55.620899 nurmoai-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-05-21 14:39:00.000000 nurmoai-1.0.1/README.md
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:41:55.616899 nurmoai-1.0.1/nurmoai/
--rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-05-21 14:40:55.000000 nurmoai-1.0.1/nurmoai/__init__.py
--rw-r--r--   0 runner    (1000) runner    (1000)     1022 2024-05-21 14:40:41.000000 nurmoai-1.0.1/nurmoai/nurmoai.py
-drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-21 14:41:55.620899 nurmoai-1.0.1/nurmoai.egg-info/
--rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-05-21 14:41:55.000000 nurmoai-1.0.1/nurmoai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1000) runner    (1000)      226 2024-05-21 14:41:55.000000 nurmoai-1.0.1/nurmoai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-21 14:41:55.000000 nurmoai-1.0.1/nurmoai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-05-21 14:41:55.000000 nurmoai-1.0.1/nurmoai.egg-info/requires.txt
--rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-05-21 14:41:55.000000 nurmoai-1.0.1/nurmoai.egg-info/top_level.txt
--rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmoai-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-21 14:41:55.620899 nurmoai-1.0.1/setup.cfg
--rw-------   0 runner    (1000) runner    (1000)      425 2024-05-21 14:41:19.000000 nurmoai-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-22 14:13:58.927363 nurmoai-1.0.2/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-05-22 14:13:58.923363 nurmoai-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)     1487 2024-05-21 14:39:00.000000 nurmoai-1.0.2/README.md
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-22 14:13:58.923363 nurmoai-1.0.2/nurmoai/
+-rw-r--r--   0 runner    (1000) runner    (1000)       28 2024-05-21 14:40:55.000000 nurmoai-1.0.2/nurmoai/__init__.py
+-rw-r--r--   0 runner    (1000) runner    (1000)     1022 2024-05-21 14:40:41.000000 nurmoai-1.0.2/nurmoai/nurmoai.py
+drwxr-xr-x   0 runner    (1000) runner    (1000)        0 2024-05-22 14:13:58.923363 nurmoai-1.0.2/nurmoai.egg-info/
+-rw-r--r--   0 runner    (1000) runner    (1000)     1735 2024-05-22 14:13:58.000000 nurmoai-1.0.2/nurmoai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1000) runner    (1000)      226 2024-05-22 14:13:58.000000 nurmoai-1.0.2/nurmoai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        1 2024-05-22 14:13:58.000000 nurmoai-1.0.2/nurmoai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)       17 2024-05-22 14:13:58.000000 nurmoai-1.0.2/nurmoai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1000) runner    (1000)        8 2024-05-22 14:13:58.000000 nurmoai-1.0.2/nurmoai.egg-info/top_level.txt
+-rw-------   0 runner    (1000) runner    (1000)      544 2024-02-27 23:10:40.000000 nurmoai-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1000) runner    (1000)       38 2024-05-22 14:13:58.927363 nurmoai-1.0.2/setup.cfg
+-rw-------   0 runner    (1000) runner    (1000)      425 2024-05-22 14:11:42.000000 nurmoai-1.0.2/setup.py
```

### Comparing `nurmoai-1.0.1/PKG-INFO` & `nurmoai-1.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmoai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python client for the NurmoAI API.
 Home-page: https://nurmo.app
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmoai-1.0.1/README.md` & `nurmoai-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `nurmoai-1.0.1/nurmoai/nurmoai.py` & `nurmoai-1.0.2/nurmoai/nurmoai.py`

 * *Files identical despite different names*

### Comparing `nurmoai-1.0.1/nurmoai.egg-info/PKG-INFO` & `nurmoai-1.0.2/nurmoai.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nurmoai
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python client for the NurmoAI API.
 Home-page: https://nurmo.app
 Author: Reksely
 Author-email: reksely@gmail.com
 Description-Content-Type: text/markdown
 Requires-Dist: requests>=2.25.1
```

### Comparing `nurmoai-1.0.1/pyproject.toml` & `nurmoai-1.0.2/pyproject.toml`

 * *Files identical despite different names*

