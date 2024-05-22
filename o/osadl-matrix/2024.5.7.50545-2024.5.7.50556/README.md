# Comparing `tmp/osadl_matrix-2024.5.7.50545.tar.gz` & `tmp/osadl_matrix-2024.5.7.50556.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osadl_matrix-2024.5.7.50545.tar", last modified: Tue May  7 05:25:50 2024, max compression
+gzip compressed data, was "osadl_matrix-2024.5.7.50556.tar", last modified: Tue May  7 05:26:00 2024, max compression
```

## Comparing `osadl_matrix-2024.5.7.50545.tar` & `osadl_matrix-2024.5.7.50556.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:50.173879 osadl_matrix-2024.5.7.50545/
--rw-r--r--   0 runner    (1001) docker     (127)    42371 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/DATALOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/LICENSE.Unlicensed
--rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/LICENSE.ccby40
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-07 05:25:50.173879 osadl_matrix-2024.5.7.50545/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:50.165878 osadl_matrix-2024.5.7.50545/osadl_matrix/
--rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/osadl_matrix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    55576 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/osadl_matrix/osadl-matrix.csv
--rw-r--r--   0 runner    (1001) docker     (127)   314715 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/osadl_matrix/osadl-matrix.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:50.169878 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-07 05:25:50.000000 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 05:25:50.000000 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:25:50.000000 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 05:25:50.000000 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 05:25:50.000000 osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-07 05:25:50.173879 osadl_matrix-2024.5.7.50545/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:50.169878 osadl_matrix-2024.5.7.50545/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1727 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/tests/test_compat_matrix.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2418 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/tests/test_customdb.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      881 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/tests/test_input.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50545/tests/test_licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:00.953993 osadl_matrix-2024.5.7.50556/
+-rw-r--r--   0 runner    (1001) docker     (127)    42371 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/DATALOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/LICENSE.Unlicensed
+-rw-r--r--   0 runner    (1001) docker     (127)    18656 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/LICENSE.ccby40
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-07 05:26:00.953993 osadl_matrix-2024.5.7.50556/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2477 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-07 05:25:56.000000 osadl_matrix-2024.5.7.50556/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:00.945993 osadl_matrix-2024.5.7.50556/osadl_matrix/
+-rw-r--r--   0 runner    (1001) docker     (127)     3903 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/osadl_matrix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55576 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/osadl_matrix/osadl-matrix.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   314715 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/osadl_matrix/osadl-matrix.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:00.949993 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5086 2024-05-07 05:26:00.000000 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-05-07 05:26:00.000000 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 05:26:00.000000 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-07 05:26:00.000000 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 05:26:00.000000 osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      866 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-05-07 05:26:00.953993 osadl_matrix-2024.5.7.50556/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 05:26:00.945993 osadl_matrix-2024.5.7.50556/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1727 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/tests/test_compat_matrix.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2418 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/tests/test_customdb.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      881 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/tests/test_input.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      504 2024-05-07 05:25:34.000000 osadl_matrix-2024.5.7.50556/tests/test_licensing.py
```

### Comparing `osadl_matrix-2024.5.7.50545/DATALOG.md` & `osadl_matrix-2024.5.7.50556/DATALOG.md`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/LICENSE.Unlicensed` & `osadl_matrix-2024.5.7.50556/LICENSE.Unlicensed`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/LICENSE.ccby40` & `osadl_matrix-2024.5.7.50556/LICENSE.ccby40`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/PKG-INFO` & `osadl_matrix-2024.5.7.50556/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2024.5.7.50545
+Version: 2024.5.7.50556
 Summary: OSADL license compatibility matrix
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Natural Language :: English
```

### Comparing `osadl_matrix-2024.5.7.50545/README.md` & `osadl_matrix-2024.5.7.50556/README.md`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/osadl_matrix/__init__.py` & `osadl_matrix-2024.5.7.50556/osadl_matrix/__init__.py`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/osadl_matrix/osadl-matrix.csv` & `osadl_matrix-2024.5.7.50556/osadl_matrix/osadl-matrix.csv`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/osadl_matrix/osadl-matrix.json` & `osadl_matrix-2024.5.7.50556/osadl_matrix/osadl-matrix.json`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/PKG-INFO` & `osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: osadl-matrix
-Version: 2024.5.7.50545
+Version: 2024.5.7.50556
 Summary: OSADL license compatibility matrix
 Author: Konrad Weihmann
 Author-email: kweihmann@outlook.com
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Legal Industry
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Natural Language :: English
```

### Comparing `osadl_matrix-2024.5.7.50545/osadl_matrix.egg-info/requires.txt` & `osadl_matrix-2024.5.7.50556/osadl_matrix.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/requirements-dev.txt` & `osadl_matrix-2024.5.7.50556/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/setup.py` & `osadl_matrix-2024.5.7.50556/setup.py`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/tests/test_compat_matrix.py` & `osadl_matrix-2024.5.7.50556/tests/test_compat_matrix.py`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/tests/test_customdb.py` & `osadl_matrix-2024.5.7.50556/tests/test_customdb.py`

 * *Files identical despite different names*

### Comparing `osadl_matrix-2024.5.7.50545/tests/test_input.py` & `osadl_matrix-2024.5.7.50556/tests/test_input.py`

 * *Files identical despite different names*

