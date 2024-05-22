# Comparing `tmp/flytekitplugins_wandb-1.12.1b1.tar.gz` & `tmp/flytekitplugins_wandb-1.12.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins_wandb-1.12.1b1.tar", last modified: Thu May 16 22:53:20 2024, max compression
+gzip compressed data, was "flytekitplugins_wandb-1.12.1b2.tar", last modified: Wed May 22 13:27:18 2024, max compression
```

## Comparing `flytekitplugins_wandb-1.12.1b1.tar` & `flytekitplugins_wandb-1.12.1b2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-16 22:52:45.000000 flytekitplugins_wandb-1.12.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/flytekitplugins/wandb/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 22:52:45.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins/wandb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-16 22:52:45.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins/wandb/tracking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 22:53:20.000000 flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-16 22:53:09.000000 flytekitplugins_wandb-1.12.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 22:53:20.227286 flytekitplugins_wandb-1.12.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-16 22:52:45.000000 flytekitplugins_wandb-1.12.1b1/tests/test_wandb_init.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-05-22 13:26:34.000000 flytekitplugins_wandb-1.12.1b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:18.178367 flytekitplugins_wandb-1.12.1b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/flytekitplugins/wandb/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-22 13:26:34.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins/wandb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 13:26:34.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins/wandb/tracking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 13:27:18.000000 flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-05-22 13:27:07.000000 flytekitplugins_wandb-1.12.1b2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:27:18.182367 flytekitplugins_wandb-1.12.1b2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2879 2024-05-22 13:26:34.000000 flytekitplugins_wandb-1.12.1b2/tests/test_wandb_init.py
```

### Comparing `flytekitplugins_wandb-1.12.1b1/PKG-INFO` & `flytekitplugins_wandb-1.12.1b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-wandb
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: This package enables seamless use of Weights & Biases within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_wandb-1.12.1b1/README.md` & `flytekitplugins_wandb-1.12.1b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins_wandb-1.12.1b1/flytekitplugins/wandb/tracking.py` & `flytekitplugins_wandb-1.12.1b2/flytekitplugins/wandb/tracking.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins_wandb-1.12.1b1/flytekitplugins_wandb.egg-info/PKG-INFO` & `flytekitplugins_wandb-1.12.1b2/flytekitplugins_wandb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-wandb
-Version: 1.12.1b1
+Version: 1.12.1b2
 Summary: This package enables seamless use of Weights & Biases within Flyte
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins_wandb-1.12.1b1/setup.py` & `flytekitplugins_wandb-1.12.1b2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "wandb"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit>=1.12.0,<2.0.0", "wandb>=0.17.0"]
 
-__version__ = "1.12.1b1"
+__version__ = "1.12.1b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables seamless use of Weights & Biases within Flyte",
```

### Comparing `flytekitplugins_wandb-1.12.1b1/tests/test_wandb_init.py` & `flytekitplugins_wandb-1.12.1b2/tests/test_wandb_init.py`

 * *Files identical despite different names*

