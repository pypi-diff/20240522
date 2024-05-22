# Comparing `tmp/flytekitplugins_mmcloud-1.12.1b1.tar.gz` & `tmp/flytekitplugins_mmcloud-1.12.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_mmcloud-1.12.1b1.tar", last modified: Thu May 16 22:53:16 2024, max compression
+gzip compressed data, was "flytekitplugins_mmcloud-1.12.1b2.tar", last modified: Wed May 22 13:27:14 2024, max compression
```

## Comparing `flytekitplugins_mmcloud-1.12.1b1.tar` & `flytekitplugins_mmcloud-1.12.1b2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:16.087230 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/task.py
--rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:16.000000 flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 22:53:09.000000 flytekitplugins_mmcloud-1.12.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:16.091230 flytekitplugins_mmcloud-1.12.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-16 22:52:45.000000 flytekitplugins_mmcloud-1.12.1b1/tests/test_mmcloud.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3528 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:14.000000 flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-22 13:27:07.000000 flytekitplugins_mmcloud-1.12.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:14.198363 flytekitplugins_mmcloud-1.12.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8026 2024-05-22 13:26:34.000000 flytekitplugins_mmcloud-1.12.1b2/tests/test_mmcloud.py
```

### Comparing `flytekitplugins_mmcloud-1.12.1b1/PKG-INFO` & `flytekitplugins_mmcloud-1.12.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_mmcloud-1.12.1b1/README.md` & `flytekitplugins_mmcloud-1.12.1b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/agent.py` & `flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/agent.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/task.py` & `flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b1/flytekitplugins/mmcloud/utils.py` & `flytekitplugins_mmcloud-1.12.1b2/flytekitplugins/mmcloud/utils.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/PKG-INFO` & `flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-mmcloud
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: MemVerge Flyte plugin
 Author: Edwin Yu, Helen Zhang
 Author-email: helen.zhang@memverge.com
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_mmcloud-1.12.1b1/flytekitplugins_mmcloud.egg-info/SOURCES.txt` & `flytekitplugins_mmcloud-1.12.1b2/flytekitplugins_mmcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flytekitplugins_mmcloud-1.12.1b1/setup.py` & `flytekitplugins_mmcloud-1.12.1b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "mmcloud"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.9.1,<2.0.0", "kubernetes"]
 
-__version__ = "1.12.1b1"
+__version__ = "1.12.1b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Edwin Yu, Helen Zhang",
     author_email="helen.zhang@memverge.com",
     description="MemVerge Flyte plugin",
```

### Comparing `flytekitplugins_mmcloud-1.12.1b1/tests/test_mmcloud.py` & `flytekitplugins_mmcloud-1.12.1b2/tests/test_mmcloud.py`

 * *Files identical despite different names*

