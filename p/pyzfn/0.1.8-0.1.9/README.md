# Comparing `tmp/pyzfn-0.1.8.tar.gz` & `tmp/pyzfn-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzfn-0.1.8.tar", last modified: Fri Sep 22 14:34:54 2023, max compression
+gzip compressed data, was "pyzfn-0.1.9.tar", last modified: Sun Dec 10 20:05:28 2023, max compression
```

## Comparing `pyzfn-0.1.8.tar` & `pyzfn-0.1.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 14:34:54.936529 pyzfn-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-09-22 14:34:43.000000 pyzfn-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-09-22 14:34:54.936529 pyzfn-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-09-22 14:34:43.000000 pyzfn-0.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      631 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 14:34:54.936529 pyzfn-0.1.8/pyzfn/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyzfn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyzfn/equations.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyzfn/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    19427 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyzfn/pyzfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     9947 2023-09-22 14:34:43.000000 pyzfn-0.1.8/pyzfn/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 14:34:54.936529 pyzfn-0.1.8/pyzfn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      345 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      229 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2023-09-22 14:34:54.000000 pyzfn-0.1.8/pyzfn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-09-22 14:34:54.936529 pyzfn-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       69 2023-09-22 14:34:43.000000 pyzfn-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-22 14:34:54.936529 pyzfn-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      919 2023-09-22 14:34:43.000000 pyzfn-0.1.8/tests/test_pyzfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-09-22 14:34:43.000000 pyzfn-0.1.8/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:05:28.904636 pyzfn-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2023-12-10 20:05:19.000000 pyzfn-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-12-10 20:05:28.904636 pyzfn-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1597 2023-12-10 20:05:19.000000 pyzfn-0.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:05:28.900636 pyzfn-0.1.9/pyzfn/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyzfn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3658 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyzfn/equations.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyzfn/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    19427 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyzfn/pyzfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9947 2023-12-10 20:05:19.000000 pyzfn-0.1.9/pyzfn/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:05:28.904636 pyzfn-0.1.9/pyzfn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2023-12-10 20:05:28.000000 pyzfn-0.1.9/pyzfn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2023-12-10 20:05:28.904636 pyzfn-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2023-12-10 20:05:19.000000 pyzfn-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-10 20:05:28.904636 pyzfn-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      919 2023-12-10 20:05:19.000000 pyzfn-0.1.9/tests/test_pyzfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2023-12-10 20:05:19.000000 pyzfn-0.1.9/tests/test_utils.py
```

### Comparing `pyzfn-0.1.8/LICENSE` & `pyzfn-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/PKG-INFO` & `pyzfn-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzfn
-Version: 0.1.8
+Version: 0.1.9
 Summary: micromagnetic post processing library
 Author: Mathieu Moalic
 License: GPL-3.0
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pyzfn-0.1.8/README.md` & `pyzfn-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/pyproject.toml` & `pyzfn-0.1.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/pyzfn/equations.py` & `pyzfn-0.1.9/pyzfn/equations.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/pyzfn/pyzfn.py` & `pyzfn-0.1.9/pyzfn/pyzfn.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/pyzfn/utils.py` & `pyzfn-0.1.9/pyzfn/utils.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/pyzfn.egg-info/PKG-INFO` & `pyzfn-0.1.9/pyzfn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyzfn
-Version: 0.1.8
+Version: 0.1.9
 Summary: micromagnetic post processing library
 Author: Mathieu Moalic
 License: GPL-3.0
 Platform: unix
 Platform: linux
 Platform: osx
 Platform: cygwin
```

### Comparing `pyzfn-0.1.8/setup.cfg` & `pyzfn-0.1.9/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyzfn
-version = 0.1.8
+version = 0.1.9
 description = micromagnetic post processing library
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Mathieu Moalic
 license = GPL-3.0
 license_files = LICENSE
 platforms = unix, linux, osx, cygwin, win32
```

### Comparing `pyzfn-0.1.8/tests/test_pyzfn.py` & `pyzfn-0.1.9/tests/test_pyzfn.py`

 * *Files identical despite different names*

### Comparing `pyzfn-0.1.8/tests/test_utils.py` & `pyzfn-0.1.9/tests/test_utils.py`

 * *Files identical despite different names*

