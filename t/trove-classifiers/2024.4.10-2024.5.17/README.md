# Comparing `tmp/trove-classifiers-2024.4.10.tar.gz` & `tmp/trove_classifiers-2024.5.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trove-classifiers-2024.4.10.tar", last modified: Wed Apr 10 13:15:43 2024, max compression
+gzip compressed data, was "trove_classifiers-2024.5.17.tar", last modified: Fri May 17 05:54:11 2024, max compression
```

## Comparing `trove-classifiers-2024.4.10.tar` & `trove_classifiers-2024.5.17.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/bin/
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/bin/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.221619 trove-classifiers-2024.4.10/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/src/trove_classifiers/
--rw-r--r--   0 runner    (1001) docker     (127)    41353 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/src/trove_classifiers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/src/trove_classifiers/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/src/trove_classifiers/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-04-10 13:15:43.000000 trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-10 13:15:43.000000 trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:15:43.000000 trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-10 13:15:43.000000 trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:15:43.225619 trove-classifiers-2024.4.10/tests/lib/
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/tests/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/tests/lib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-04-10 13:15:18.000000 trove-classifiers-2024.4.10/tests/test_classifiers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.917073 trove_classifiers-2024.5.17/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/bin/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.917073 trove_classifiers-2024.5.17/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.917073 trove_classifiers-2024.5.17/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/src/trove_classifiers/
+-rw-r--r--   0 runner    (1001) docker     (127)    41399 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/src/trove_classifiers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/src/trove_classifiers/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/src/trove_classifiers/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2158 2024-05-17 05:54:11.000000 trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-17 05:54:11.000000 trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 05:54:11.000000 trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-17 05:54:11.000000 trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 05:54:11.921073 trove_classifiers-2024.5.17/tests/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/tests/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/tests/lib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2332 2024-05-17 05:53:51.000000 trove_classifiers-2024.5.17/tests/test_classifiers.py
```

### Comparing `trove-classifiers-2024.4.10/CONTRIBUTING.md` & `trove_classifiers-2024.5.17/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/LICENSE` & `trove_classifiers-2024.5.17/LICENSE`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/Makefile` & `trove_classifiers-2024.5.17/Makefile`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/PKG-INFO` & `trove_classifiers-2024.5.17/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2024.4.10
+Version: 2024.5.17
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2024.4.10/README.md` & `trove_classifiers-2024.5.17/README.md`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/bin/sort.py` & `trove_classifiers-2024.5.17/bin/sort.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/setup.py` & `trove_classifiers-2024.5.17/setup.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/src/trove_classifiers/__init__.py` & `trove_classifiers-2024.5.17/src/trove_classifiers/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -512,14 +512,15 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: 3.13",
+    "Programming Language :: Python :: 3.14",
     "Programming Language :: Python :: Implementation",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: IronPython",
     "Programming Language :: Python :: Implementation :: Jython",
     "Programming Language :: Python :: Implementation :: MicroPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Programming Language :: Python :: Implementation :: Stackless",
```

### Comparing `trove-classifiers-2024.4.10/src/trove_classifiers.egg-info/PKG-INFO` & `trove_classifiers-2024.5.17/src/trove_classifiers.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trove-classifiers
-Version: 2024.4.10
+Version: 2024.5.17
 Summary: Canonical source for classifiers on PyPI (pypi.org).
 Home-page: https://github.com/pypa/trove-classifiers
 Author: The PyPI Admins
 Author-email: admin@pypi.org
 Keywords: classifiers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `trove-classifiers-2024.4.10/tests/lib/__init__.py` & `trove_classifiers-2024.5.17/tests/lib/__init__.py`

 * *Files identical despite different names*

### Comparing `trove-classifiers-2024.4.10/tests/test_classifiers.py` & `trove_classifiers-2024.5.17/tests/test_classifiers.py`

 * *Files identical despite different names*

