# Comparing `tmp/pynenv-0.1.2.tar.gz` & `tmp/pynenv-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynenv-0.1.2.tar", max compression
+gzip compressed data, was "pynenv-0.2.1.tar", max compression
```

## Comparing `pynenv-0.1.2.tar` & `pynenv-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.1.2/LICENSE
--rw-r--r--   0        0        0      345 2024-05-21 06:56:32.953388 pynenv-0.1.2/README.md
--rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.1.2/pynenv/__init__.py
--rw-r--r--   0        0        0      542 2024-05-21 06:49:05.377202 pynenv-0.1.2/pynenv/environment.py
--rw-r--r--   0        0        0      285 2024-05-21 06:57:31.385891 pynenv-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 pynenv-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.1/LICENSE
+-rw-r--r--   0        0        0      345 2024-05-21 06:58:06.909590 pynenv-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.1/pynenv/__init__.py
+-rw-r--r--   0        0        0      911 2024-05-22 17:37:47.347698 pynenv-0.2.1/pynenv/environment.py
+-rw-r--r--   0        0        0      326 2024-05-22 17:38:46.358270 pynenv-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      711 1970-01-01 00:00:00.000000 pynenv-0.2.1/PKG-INFO
```

### Comparing `pynenv-0.1.2/LICENSE` & `pynenv-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynenv-0.1.2/PKG-INFO` & `pynenv-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: pynenv
-Version: 0.1.2
-Summary: 
+Version: 0.2.1
+Summary: General helper functions for environments
 Author: Nik Sheridan
 Author-email: niksheridan@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Description-Content-Type: text/markdown
@@ -27,10 +27,10 @@
 
 my_env_var = get_environment_variable('SOME_VAR')
 ```
 
 ## Build
 
 * Adjust version in ```pyproject.toml```
-* Run ```poerty build```
+* Run ```poetry build```
 * Run ```poetry publish```
```

