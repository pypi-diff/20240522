# Comparing `tmp/pyright-1.1.362.tar.gz` & `tmp/pyright-1.1.363.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyright-1.1.362.tar", last modified: Wed May  8 10:05:18 2024, max compression
+gzip compressed data, was "pyright-1.1.363.tar", last modified: Wed May 15 07:34:11 2024, max compression
```

## Comparing `pyright-1.1.362.tar` & `pyright-1.1.363.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:05:18.875471 pyright-1.1.362/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-08 10:05:09.000000 pyright-1.1.362/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-08 10:05:09.000000 pyright-1.1.362/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-08 10:05:18.875471 pyright-1.1.362/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-08 10:05:09.000000 pyright-1.1.362/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-08 10:05:09.000000 pyright-1.1.362/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:05:18.875471 pyright-1.1.362/pyright/
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/_mureq.py
--rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/langserver.py
--rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/node.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-08 10:05:09.000000 pyright-1.1.362/pyright/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 10:05:18.875471 pyright-1.1.362/pyright.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-08 10:05:18.000000 pyright-1.1.362/pyright.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-08 10:05:09.000000 pyright-1.1.362/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 10:05:18.875471 pyright-1.1.362/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     2199 2024-05-08 10:05:09.000000 pyright-1.1.362/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:34:11.369715 pyright-1.1.363/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-05-15 07:34:03.000000 pyright-1.1.363/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-15 07:34:03.000000 pyright-1.1.363/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-15 07:34:11.369715 pyright-1.1.363/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-05-15 07:34:03.000000 pyright-1.1.363/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-15 07:34:03.000000 pyright-1.1.363/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:34:11.365715 pyright-1.1.363/pyright/
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14622 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/_mureq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4911 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/langserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7305 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/node.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-15 07:34:03.000000 pyright-1.1.363/pyright/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 07:34:11.369715 pyright-1.1.363/pyright.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6041 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 07:34:11.000000 pyright-1.1.363/pyright.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 07:34:03.000000 pyright-1.1.363/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 07:34:11.369715 pyright-1.1.363/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2199 2024-05-15 07:34:03.000000 pyright-1.1.363/setup.py
```

### Comparing `pyright-1.1.362/LICENSE` & `pyright-1.1.363/LICENSE`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/PKG-INFO` & `pyright-1.1.363/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.362
+Version: 1.1.363
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -62,15 +62,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.362
+    rev: v1.1.363
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.362/README.md` & `pyright-1.1.363/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.362
+    rev: v1.1.363
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.362/pyright/__init__.py` & `pyright-1.1.363/pyright/__init__.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/_mureq.py` & `pyright-1.1.363/pyright/_mureq.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/_utils.py` & `pyright-1.1.363/pyright/_utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/cli.py` & `pyright-1.1.363/pyright/cli.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/errors.py` & `pyright-1.1.363/pyright/errors.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/langserver.py` & `pyright-1.1.363/pyright/langserver.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/node.py` & `pyright-1.1.363/pyright/node.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/types.py` & `pyright-1.1.363/pyright/types.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright/utils.py` & `pyright-1.1.363/pyright/utils.py`

 * *Files identical despite different names*

### Comparing `pyright-1.1.362/pyright.egg-info/PKG-INFO` & `pyright-1.1.363/pyright.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyright
-Version: 1.1.362
+Version: 1.1.363
 Summary: Command line wrapper for pyright
 Home-page: https://github.com/RobertCraigie/pyright-python
 Author: Robert Craigie
 Maintainer: Robert Craigie
 License: MIT
 Project-URL: Source, https://github.com/RobertCraigie/pyright-python
 Project-URL: Tracker, https://github.com/RobertCraigie/pyright-python/issues
@@ -62,15 +62,15 @@
 ### Pre-commit
 
 You can also setup pyright to run automatically before each commit by setting up [pre-commit](https://pre-commit.com) and registering pyright in your `.pre-commit-config.yaml` file
 
 ```yaml
 repos:
   - repo: https://github.com/RobertCraigie/pyright-python
-    rev: v1.1.362
+    rev: v1.1.363
     hooks:
     - id: pyright
 ```
 
 Pre-commit will install pyright-python in its own virtual environment which can cause pyright to not be able to detect your installed dependencies.
 
 To fix this you can either [tell pre-commit](https://pre-commit.com/#config-additional_dependencies) to also install those dependencies or explicitly tell pyright which virtual environment to use by updating your [pyright configuration file](https://github.com/microsoft/pyright/blob/main/docs/configuration.md):
```

### Comparing `pyright-1.1.362/setup.py` & `pyright-1.1.363/setup.py`

 * *Files identical despite different names*

