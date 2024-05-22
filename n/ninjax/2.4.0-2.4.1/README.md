# Comparing `tmp/ninjax-2.4.0.tar.gz` & `tmp/ninjax-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ninjax-2.4.0.tar", last modified: Fri May  3 01:12:06 2024, max compression
+gzip compressed data, was "ninjax-2.4.1.tar", last modified: Wed May 22 00:58:47 2024, max compression
```

## Comparing `ninjax-2.4.0.tar` & `ninjax-2.4.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.420701 ninjax-2.4.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2023-11-19 22:35:43.000000 ninjax-2.4.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-03 01:12:06.420701 ninjax-2.4.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)     8749 2024-05-03 01:12:04.000000 ninjax-2.4.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.408701 ninjax-2.4.0/ninjax/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      493 2023-12-04 20:45:03.000000 ninjax-2.4.0/ninjax/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    22614 2024-05-03 01:12:04.000000 ninjax-2.4.0/ninjax/ninjax.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.408701 ninjax-2.4.0/ninjax.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      394 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        4 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2024-05-03 01:12:06.000000 ninjax-2.4.0/ninjax.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-03 01:12:06.420701 ninjax-2.4.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)      800 2024-02-05 01:40:52.000000 ninjax-2.4.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-03 01:12:06.420701 ninjax-2.4.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1959 2023-11-26 03:13:56.000000 ninjax-2.4.0/tests/test_attrs.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1020 2023-12-05 21:38:21.000000 ninjax-2.4.0/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1138 2023-11-29 00:10:03.000000 ninjax-2.4.0/tests/test_cond.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3608 2023-12-05 21:36:48.000000 ninjax-2.4.0/tests/test_grad.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2428 2023-11-29 00:16:02.000000 ninjax-2.4.0/tests/test_init.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2528 2023-12-04 20:45:06.000000 ninjax-2.4.0/tests/test_jit.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1751 2023-11-29 00:28:06.000000 ninjax-2.4.0/tests/test_module.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1435 2023-12-05 21:04:09.000000 ninjax-2.4.0/tests/test_scan.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1278 2023-11-29 00:14:22.000000 ninjax-2.4.0/tests/test_variable.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 00:58:47.206099 ninjax-2.4.1/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1071 2023-11-19 22:35:43.000000 ninjax-2.4.1/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-22 00:58:47.206099 ninjax-2.4.1/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     8749 2024-05-03 01:12:04.000000 ninjax-2.4.1/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 00:58:47.202099 ninjax-2.4.1/ninjax/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 00:58:02.000000 ninjax-2.4.1/ninjax/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    22614 2024-05-22 00:58:38.000000 ninjax-2.4.1/ninjax/ninjax.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 00:58:47.202099 ninjax-2.4.1/ninjax.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     9160 2024-05-22 00:58:47.000000 ninjax-2.4.1/ninjax.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      394 2024-05-22 00:58:47.000000 ninjax-2.4.1/ninjax.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 00:58:47.000000 ninjax-2.4.1/ninjax.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        4 2024-05-22 00:58:47.000000 ninjax-2.4.1/ninjax.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        7 2024-05-22 00:58:47.000000 ninjax-2.4.1/ninjax.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 00:58:47.206099 ninjax-2.4.1/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      800 2024-02-05 01:40:52.000000 ninjax-2.4.1/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 00:58:47.202099 ninjax-2.4.1/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1959 2023-11-26 03:13:56.000000 ninjax-2.4.1/tests/test_attrs.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1020 2023-12-05 21:38:21.000000 ninjax-2.4.1/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1138 2023-11-29 00:10:03.000000 ninjax-2.4.1/tests/test_cond.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3608 2023-12-05 21:36:48.000000 ninjax-2.4.1/tests/test_grad.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2428 2023-11-29 00:16:02.000000 ninjax-2.4.1/tests/test_init.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2528 2023-12-04 20:45:06.000000 ninjax-2.4.1/tests/test_jit.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1751 2023-11-29 00:28:06.000000 ninjax-2.4.1/tests/test_module.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1435 2023-12-05 21:04:09.000000 ninjax-2.4.1/tests/test_scan.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1278 2023-11-29 00:14:22.000000 ninjax-2.4.1/tests/test_variable.py
```

### Comparing `ninjax-2.4.0/LICENSE` & `ninjax-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/PKG-INFO` & `ninjax-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 2.4.0
+Version: 2.4.1
 Summary: Flexible Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-2.4.0/README.md` & `ninjax-2.4.1/README.md`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/ninjax/ninjax.py` & `ninjax-2.4.1/ninjax/ninjax.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 import re
 import threading
 
 import jax
 import jax.numpy as jnp
 
-__version__ = '2.4.0'
+__version__ = '2.4.1'
 
 
 ###############################################################################
 # State
 ###############################################################################
```

### Comparing `ninjax-2.4.0/ninjax.egg-info/PKG-INFO` & `ninjax-2.4.1/ninjax.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ninjax
-Version: 2.4.0
+Version: 2.4.1
 Summary: Flexible Modules for JAX
 Home-page: http://github.com/danijar/ninjax
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
```

### Comparing `ninjax-2.4.0/setup.py` & `ninjax-2.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_attrs.py` & `ninjax-2.4.1/tests/test_attrs.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_checkpoint.py` & `ninjax-2.4.1/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_cond.py` & `ninjax-2.4.1/tests/test_cond.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_grad.py` & `ninjax-2.4.1/tests/test_grad.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_init.py` & `ninjax-2.4.1/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_jit.py` & `ninjax-2.4.1/tests/test_jit.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_module.py` & `ninjax-2.4.1/tests/test_module.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_scan.py` & `ninjax-2.4.1/tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `ninjax-2.4.0/tests/test_variable.py` & `ninjax-2.4.1/tests/test_variable.py`

 * *Files identical despite different names*

