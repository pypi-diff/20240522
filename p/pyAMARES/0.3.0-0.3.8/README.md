# Comparing `tmp/pyAMARES-0.3.0.tar.gz` & `tmp/pyAMARES-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyAMARES-0.3.0.tar", last modified: Sun May  5 04:41:36 2024, max compression
+gzip compressed data, was "pyAMARES-0.3.8.tar", last modified: Wed May 22 20:32:15 2024, max compression
```

## Comparing `pyAMARES-0.3.0.tar` & `pyAMARES-0.3.8.tar`

### file list

```diff
@@ -1,51 +1,54 @@
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:36.098226 pyAMARES-0.3.0/
--rw-r--r--   0 xujia     (1000) xujia     (1000)     1603 2024-05-01 20:09:46.000000 pyAMARES-0.3.0/LICENSE.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)      124 2024-05-04 22:32:09.000000 pyAMARES-0.3.0/MANIFEST.in
--rw-r--r--   0 xujia     (1000) xujia     (1000)     4378 2024-05-05 04:41:36.062708 pyAMARES-0.3.0/PKG-INFO
--rw-r--r--   0 xujia     (1000) xujia     (1000)     3416 2024-05-05 04:41:29.000000 pyAMARES-0.3.0/README.rst
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.817327 pyAMARES-0.3.0/pyAMARES/
--rw-r--r--   0 xujia     (1000) xujia     (1000)      259 2024-05-05 02:34:14.000000 pyAMARES-0.3.0/pyAMARES/__init__.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.912461 pyAMARES-0.3.0/pyAMARES/examples/
--rw-r--r--   0 xujia     (1000) xujia     (1000)     1776 2024-05-01 22:49:48.000000 pyAMARES-0.3.0/pyAMARES/examples/example_human_brain_31P_7T.csv
--rw-r--r--   0 xujia     (1000) xujia     (1000)    19146 2024-05-01 22:48:59.000000 pyAMARES-0.3.0/pyAMARES/examples/fid.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)     1743 2024-04-30 03:23:42.000000 pyAMARES-0.3.0/pyAMARES/examples/human_brain_31P_7T.csv
--rw-r--r--   0 xujia     (1000) xujia     (1000)     3033 2024-05-01 22:45:46.000000 pyAMARES-0.3.0/pyAMARES/examples/simple_example.csv
--rw-r--r--   0 xujia     (1000) xujia     (1000)    19490 2024-05-01 22:45:46.000000 pyAMARES-0.3.0/pyAMARES/examples/simple_example.html
--rw-r--r--   0 xujia     (1000) xujia     (1000)    89009 2024-05-01 22:45:46.000000 pyAMARES-0.3.0/pyAMARES/examples/simple_example.svg
--rw-r--r--   0 xujia     (1000) xujia     (1000)   241861 2024-05-01 22:45:46.000000 pyAMARES-0.3.0/pyAMARES/examples/simple_example_html.jpeg
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.932464 pyAMARES-0.3.0/pyAMARES/fileio/
--rw-r--r--   0 xujia     (1000) xujia     (1000)       28 2024-04-30 16:45:43.000000 pyAMARES-0.3.0/pyAMARES/fileio/__init__.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     2414 2024-04-30 16:42:05.000000 pyAMARES-0.3.0/pyAMARES/fileio/readmat.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.962631 pyAMARES-0.3.0/pyAMARES/kernel/
--rw-r--r--   0 xujia     (1000) xujia     (1000)    21183 2024-05-05 02:49:31.000000 pyAMARES-0.3.0/pyAMARES/kernel/PriorKnowledge.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)      510 2024-04-30 16:47:19.000000 pyAMARES-0.3.0/pyAMARES/kernel/__init__.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)    14449 2024-05-05 02:38:14.000000 pyAMARES-0.3.0/pyAMARES/kernel/fid.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)    17145 2024-05-05 02:39:10.000000 pyAMARES-0.3.0/pyAMARES/kernel/lmfit.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)      896 2024-04-30 16:47:58.000000 pyAMARES-0.3.0/pyAMARES/kernel/objective_func.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.981742 pyAMARES-0.3.0/pyAMARES/libs/
--rw-r--r--   0 xujia     (1000) xujia     (1000)     8890 2024-05-05 02:54:50.000000 pyAMARES-0.3.0/pyAMARES/libs/MPFIR.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)       43 2024-05-05 03:17:39.000000 pyAMARES-0.3.0/pyAMARES/libs/__init__.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)    37054 2024-02-29 20:15:22.000000 pyAMARES-0.3.0/pyAMARES/libs/hlsvd.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.994127 pyAMARES-0.3.0/pyAMARES/script/
--rw-r--r--   0 xujia     (1000) xujia     (1000)        0 2024-04-30 17:44:35.000000 pyAMARES-0.3.0/pyAMARES/script/__init__.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     5613 2024-05-05 03:17:39.000000 pyAMARES-0.3.0/pyAMARES/script/amaresfit.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:36.040923 pyAMARES-0.3.0/pyAMARES/util/
--rw-r--r--   0 xujia     (1000) xujia     (1000)      171 2024-04-30 16:55:19.000000 pyAMARES-0.3.0/pyAMARES/util/__init__.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     9024 2024-05-05 02:56:32.000000 pyAMARES-0.3.0/pyAMARES/util/crlb.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)    11168 2024-05-05 02:58:05.000000 pyAMARES-0.3.0/pyAMARES/util/hsvd.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)      397 2024-04-30 16:53:45.000000 pyAMARES-0.3.0/pyAMARES/util/misc.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     5241 2024-05-05 02:58:28.000000 pyAMARES-0.3.0/pyAMARES/util/multiprocessing.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     9320 2024-05-05 03:00:06.000000 pyAMARES-0.3.0/pyAMARES/util/report.py
--rw-r--r--   0 xujia     (1000) xujia     (1000)     6941 2024-05-03 16:58:37.000000 pyAMARES-0.3.0/pyAMARES/util/visualization.py
-drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-05 04:41:35.866108 pyAMARES-0.3.0/pyAMARES.egg-info/
--rw-r--r--   0 xujia     (1000) xujia     (1000)     4378 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/PKG-INFO
--rw-r--r--   0 xujia     (1000) xujia     (1000)     1103 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/SOURCES.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)        1 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/dependency_links.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)       61 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/entry_points.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)        1 2024-05-05 04:32:02.000000 pyAMARES-0.3.0/pyAMARES.egg-info/not-zip-safe
--rw-r--r--   0 xujia     (1000) xujia     (1000)      239 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/requires.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)        9 2024-05-05 04:41:35.000000 pyAMARES-0.3.0/pyAMARES.egg-info/top_level.txt
--rwxr-xr-x   0 xujia     (1000) xujia     (1000)   888010 2024-05-01 22:45:59.000000 pyAMARES-0.3.0/pyAMARES_logo.svg
--rw-r--r--   0 xujia     (1000) xujia     (1000)       97 2024-04-25 17:50:47.000000 pyAMARES-0.3.0/requirements.txt
--rw-r--r--   0 xujia     (1000) xujia     (1000)       38 2024-05-05 04:41:36.099225 pyAMARES-0.3.0/setup.cfg
--rw-r--r--   0 xujia     (1000) xujia     (1000)     3638 2024-05-05 03:36:29.000000 pyAMARES-0.3.0/setup.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.202408 pyAMARES-0.3.8/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     1570 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/CHANGELOG.rst
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     1603 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/LICENSE.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      124 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/MANIFEST.in
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     5635 2024-05-22 20:32:15.203412 pyAMARES-0.3.8/PKG-INFO
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     4673 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/README.rst
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.062358 pyAMARES-0.3.8/pyAMARES/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      259 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/__init__.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.124568 pyAMARES-0.3.8/pyAMARES/examples/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     1776 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/example_human_brain_31P_7T.csv
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    19146 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/fid.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     1743 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/human_brain_31P_7T.csv
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     3033 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/simple_example.csv
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    19490 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/simple_example.html
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    89009 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/simple_example.svg
+-rw-r--r--   0 xujia     (1000) xujia     (1000)   241861 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/examples/simple_example_html.jpeg
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.138600 pyAMARES-0.3.8/pyAMARES/fileio/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      116 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/fileio/__init__.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     5190 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/fileio/readfidall.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     3240 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/fileio/readmat.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     2538 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/fileio/readnifti.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.156836 pyAMARES-0.3.8/pyAMARES/kernel/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    22277 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/kernel/PriorKnowledge.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      510 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/kernel/__init__.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    14449 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/kernel/fid.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    17145 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/kernel/lmfit.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      896 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/kernel/objective_func.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.168371 pyAMARES-0.3.8/pyAMARES/libs/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     8890 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/libs/MPFIR.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)       43 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/libs/__init__.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    37054 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/libs/hlsvd.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.173570 pyAMARES-0.3.8/pyAMARES/script/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)        0 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/script/__init__.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     5613 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/script/amaresfit.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.201126 pyAMARES-0.3.8/pyAMARES/util/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      171 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/__init__.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     9989 2024-05-22 20:27:36.000000 pyAMARES-0.3.8/pyAMARES/util/crlb.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)    11168 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/hsvd.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      397 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/misc.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     5241 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/multiprocessing.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     9320 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/report.py
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     6941 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES/util/visualization.py
+drwxr-xr-x   0 xujia     (1000) xujia     (1000)        0 2024-05-22 20:32:15.081359 pyAMARES-0.3.8/pyAMARES.egg-info/
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     5635 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/PKG-INFO
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     1186 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/SOURCES.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)        1 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/dependency_links.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)       61 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/entry_points.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)        1 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/not-zip-safe
+-rw-r--r--   0 xujia     (1000) xujia     (1000)      239 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/requires.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)        9 2024-05-22 20:32:14.000000 pyAMARES-0.3.8/pyAMARES.egg-info/top_level.txt
+-rwxr-xr-x   0 xujia     (1000) xujia     (1000)   888010 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/pyAMARES_logo.svg
+-rw-r--r--   0 xujia     (1000) xujia     (1000)       97 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/requirements.txt
+-rw-r--r--   0 xujia     (1000) xujia     (1000)       38 2024-05-22 20:32:15.206844 pyAMARES-0.3.8/setup.cfg
+-rw-r--r--   0 xujia     (1000) xujia     (1000)     3638 2024-05-22 19:59:38.000000 pyAMARES-0.3.8/setup.py
```

### Comparing `pyAMARES-0.3.0/LICENSE.txt` & `pyAMARES-0.3.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/PKG-INFO` & `pyAMARES-0.3.8/README.rst`

 * *Files 22% similar despite different names*

```diff
@@ -1,79 +1,76 @@
-Metadata-Version: 2.1
-Name: pyAMARES
-Version: 0.3.0
-Summary: pyAMARES, an Open-Source Python Library for Fitting Magnetic Resonance Spectroscopy Data
-Home-page: https://github.com/hawkMRS/pyAMARES
-Author: Jia Xu, MR Research Facility, University of Iowa
-Author-email: jia-xu-1@uiowa.edu
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/x-rst
-Provides-Extra: docs
-Provides-Extra: jupyter
-License-File: LICENSE.txt
-
 **pyAMARES**, an Open-Source Python Library for Fitting Magnetic Resonance Spectroscopy Data
 ********************************************************************************************
 
-.. image:: pyAMARES_logo.svg
+.. image:: https://raw.githubusercontent.com/HawkMRS/pyAMARES/main/pyAMARES_logo.svg
    :width: 400
 
+The full documentation for pyAMARES can be found at `pyAMARES Documentation <https://pyamares.readthedocs.io/en/latest/index.html>`_.
+
 What is pyAMARES?
 =================
 
-PyAMARES package to provide the MRS community with open-source, easy-to-use MRS fitting method in Python.  
-It imports prior knowledge from Excel or CSV spreadsheets as initial values and constraints for fitting MRS data according to the AMARES model function. 
+The pyAMARES package provides the MRS community with an open-source, easy-to-use MRS fitting method in Python. 
+It imports prior knowledge from Excel or CSV spreadsheets as initial values and constraints for fitting MRS data 
+according to the AMARES model function.
+
+
 
 Getting Started
 ===============
 
+Requirements
+------------
+
+.. image:: https://img.shields.io/badge/Python->%3D3.6%2C%203.8+-blue.svg
+   :target: https://python.org
+   :alt: Python Version
+
+.. note::
+   PyAMARES requires Python 3.6 or newer. We recommend using Python 3.8 or newer. If you are using an older version of Python, you will need to upgrade to use pyAMARES.
+
 Installation
 ------------
+
 .. code-block:: bash
 
    pip install pyAMARES
 
+See the `Installation Guide <https://pyamares.readthedocs.io/en/latest/install.html>`_ for detailed information.
+
 Run pyAMARES as standard-alone script
 -------------------------------------
 
 
 .. code-block:: bash
 
    amaresFit -f ./pyAMARES/examples/fid.txt -p  ./pyAMARES/examples/example_human_brain_31P_7T.csv --MHz 120.0 --sw 10000 --deadtime 300e-6 --ifplot --xlim 10 -20 -o simple_example 
 
 Run pyAMARES in a Jupyter Notebook
 ----------------------------------
+**Try Jupyter Notebook on Google Colab** `here <https://colab.research.google.com/drive/184_7MJ6O1BgGYyqNvnXXqtri4_0N4ySw?usp=sharing>`_
 
 .. code-block:: python
 
    import pyAMARES
    # Load FID from a 2-column ASCII file, and set the MR parameters
    MHz = 120.0 # 31P nuclei at 7T
    sw = 10000 # spectrum width in Hz
    deadtime = 300e-6 # 300 us begin time for the FID signal acquisition
 
    fid = pyAMARES.readmrs('./pyAMARES/examples/fid.txt')
    # Load Prior Knowledge
    FIDobj = pyAMARES.initialize_FID(fid=fid, 
-                                    priorknowledge='./pyAMARES/examples/example_human_brain_31P_7T.csv',
+                                    priorknowledgefile='./pyAMARES/examples/example_human_brain_31P_7T.csv',
                                     MHz=MHz, 
                                     sw=sw,
                                     deadtime=deadtime, 
-                                    preview=False)
+                                    preview=False, 
+                                    normalize_fid=False,
+                                    xlim=(10, -20))# Region of Interest for visualization, -20 to 10 ppm
 
    # Initialize the parameter using Levenberg-Marquard method
    out1 = pyAMARES.fitAMARES(fid_parameters=FIDobj,
                               fitting_parameters=FIDobj.initialParams,
                               method='leastsq',
                               ifplot=False)
 
@@ -82,26 +79,27 @@
    out2 = pyAMARES.fitAMARES(fid_parameters=out1,
                              fitting_parameters=out1.fittedParams, # optimized parameter for last step
                              method='least_squares',
                              ifplot=False)
    
    # Save the data
    out2.styled_df.to_html('simple_example.html') # Save highlighted table to an HTML page
-   out2.result_sum.to_cscv('simple_example.csv') # Save table to CSV spreadsheet
-   out2.plotParameters.lb = 2.0 # Line Braodening
+                                                 # Python 3.6 does not support to_html. 
+   out2.result_sum.to_csv('simple_example.csv') # Save table to CSV spreadsheet
+   out2.plotParameters.lb = 2.0 # Line Broadening factor for visualization
    out2.plotParameters.ifphase = True # Phase the spectrum for visualization
    pyAMARES.plotAMARES(fid_parameters=out1, filename='simple_example.svg') # Save plot to SVG 
 
-Fitting Result
---------------
+Fitting Result for Example 31P MRS data
+------------------------------------------
 
-.. image:: pyAMARES/examples/simple_example.svg
+.. image:: https://raw.githubusercontent.com/HawkMRS/pyAMARES/main/pyAMARES/examples/simple_example.svg
    :width: 400
 
-.. image:: pyAMARES/examples/simple_example_html.jpeg
+.. image:: https://github.com/HawkMRS/pyAMARES/blob/4f9ca4431c0d72e1b41fb2b434f72e53feb1657f/pyAMARES/examples/simple_example_html.jpeg
    :width: 400
 
 How to cite
 ===========
 
 If you use pyAMARES in your research, please consider citing the following ISMRM proceeding:
```

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/example_human_brain_31P_7T.csv` & `pyAMARES-0.3.8/pyAMARES/examples/example_human_brain_31P_7T.csv`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/fid.txt` & `pyAMARES-0.3.8/pyAMARES/examples/fid.txt`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/human_brain_31P_7T.csv` & `pyAMARES-0.3.8/pyAMARES/examples/human_brain_31P_7T.csv`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/simple_example.csv` & `pyAMARES-0.3.8/pyAMARES/examples/simple_example.csv`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/simple_example.html` & `pyAMARES-0.3.8/pyAMARES/examples/simple_example.html`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/simple_example.svg` & `pyAMARES-0.3.8/pyAMARES/examples/simple_example.svg`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/examples/simple_example_html.jpeg` & `pyAMARES-0.3.8/pyAMARES/examples/simple_example_html.jpeg`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/fileio/readmat.py` & `pyAMARES-0.3.8/pyAMARES/fileio/readmat.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,56 +1,79 @@
 import numpy as np
 from scipy import io
+import warnings
+import mat73
+from .readfidall import is_mat_file_v7_3
 
 
 def readmrs(filename):
     """
     Reads MRS data from a file, supporting multiple file formats including ASCII, CSV, NPY, and MATLAB files.
 
-    This function detects the file format based on the file extension and loads the MRS data accordingly. For ASCII files, it expects two columns representing the real and imaginary parts. NPY files should contain a NumPy array, and MATLAB files should contain a variable named 'fid'.
+    This function detects the file format based on the file extension and loads the MRS data accordingly.
+    For ASCII files, it expects two columns representing the real and imaginary parts. 
+    NPY files should contain a NumPy array, and MATLAB files should contain a variable named ``fid`` and/or ``data``, 
+    when both ``fid`` and ``data`` present, only ``fid`` will be used. 
 
     Args:
         filename (str): The path and name of the file from which to load the MRS data.
 
     Returns:
         numpy.ndarray: A complex numpy array containing the MRS data from the file.
 
     Raises:
-        AssertionError: If the data loaded does not have a one-dimensional shape.
         FileNotFoundError: If the specified file does not exist or cannot be opened.
         ValueError: If the file format is unsupported or the required data cannot be found in the file.
+        KeyError:
 
     Example:
         >>> data = readmrs('fid.txt')
         >>> print(data.shape)
         >>> print(data.dtype)
 
     Note:
         - For ASCII files, data is expected to be in two columns with the first column as the real part and the second as the imaginary part.
         - For NPY files, it directly loads the NumPy array.
-        - For MATLAB files, both traditional (.mat) and V7.3 (.mat) files are supported, but the variable must be named 'fid'.
+        - For MATLAB files, both traditional (.mat) and V7.3 (.mat) files are supported, but the variable must be named ``fid`` or ``data``.
     """
     if filename.endswith("csv"):
         print("Try to load 2-column CSV")
         data = np.loadtxt(filename, delimiter=",")
         data = data[:, 0] + 1j * data[:, 1]
     elif filename.endswith("txt"):
         print("Try to load 2-column ASCII data")
         data = np.loadtxt(filename, delimiter=" ")
         data = data[:, 0] + 1j * data[:, 1]
     elif filename.endswith("npy"):
         print("Try to load python NPY file")
         data = np.load(filename)
     elif filename.endswith("mat"):
-        try:
-            print("Try to load Matlab mat file with the var saved as `fid`")
+        if is_mat_file_v7_3(filename):
+            print(
+                "Try to load Matlab V7.3 mat file with the var saved as `fid` or `data`"
+            )
+            matdic = mat73.loadmat(filename)
+        else:
+            print("Try to load Matlab mat file with the var saved as `fid` or `data`")
             matdic = io.loadmat(filename)
+        if "fid" in matdic.keys() and "data" in matdic.keys():
             data = matdic["fid"].squeeze().astype("complex")
-        except:
-            import mat73
-
-            print("Try to load Matlab V7.3 mat file with the var saved as `fid`")
-            matdic = mat73.loadmat(filename)
+        elif "fid" in matdic.keys():
             data = matdic["fid"].squeeze().astype("complex")
+        elif "data" in matdic.keys():
+            data = matdic["data"].squeeze().astype("complex")
+        else:
+            raise KeyError("Neither 'fid' nor 'data' found in the loaded .mat file")
+    else:
+        raise NotImplementedError(
+            "PyAMARES only supports 2-column data in TXT, CSV, MAT-files!"
+        )
+    # assert len(data.shape) == 1
+    if len(data.shape) != 1:
+        warnings.warn(
+            "Note pyAMARES.fitAMARES only fits 1D MRS data, however, your data shape is {data.shape}. Is it MRSI or raw MRS data that needs to be coil-combined?"
+        )
+
     print("data.shape=", data.shape)
-    assert len(data.shape) == 1
     return data
+
+
```

### Comparing `pyAMARES-0.3.0/pyAMARES/kernel/PriorKnowledge.py` & `pyAMARES-0.3.8/pyAMARES/kernel/PriorKnowledge.py`

 * *Files 3% similar despite different names*

```diff
@@ -320,29 +320,36 @@
             if np.isnan(lval):
                 lval = -np.inf
             if np.isnan(uval):
                 uval = np.inf
             name = para + "_" + peak
             if para == "freq":
                 pass
-            if para == "dk":
+            if para == "dk" and (lval != uval):
                 lval = 0
             if para == "g":
                 if g_global is False:
                     vary = True
                 else:
                     val = g_global
                     vary = False
             if para == "phi":
                 pass
             # Add parameter to lmfit Parameters object
             try:
-                allpara.add(
-                    name=name, value=val, min=lval, max=uval, vary=vary, expr=expr
-                )
+                if lval == uval:
+                    # When lval == uval, set the val to lval and fix it
+                    allpara.add(
+                        name=name, value=lval, vary=False,
+                    )
+                else:
+                    allpara.add(
+                        name=name, value=val, min=lval, max=uval, vary=vary, expr=expr
+                    )
+                    
             except NameError as e:
                 e2 = (
                     "This error may be caused by the expr {} being constrained "
                     "to a peak that is not defined yet. Define it in a column "
                     "to the left of the {} column."
                 ).format(expr, peak)
                 raise UnboundLocalError(e2)
@@ -366,14 +373,15 @@
     preview=False,
     xlim=None,
     truncate_initial_points=0,
     g_global=0.0,
     carrier=0.0,
     lb=2.0,
     ppm_offset=0,
+    noise_var='OXSA',
 ):
     """
     Initialize fitting parameters from prior knowledge (`priorknowledgefile`) or HSVD initialized result if there is
     not a prior knowledge file.
 
     Args:
         fid (numpy.ndarray): The input FID data.
@@ -383,18 +391,24 @@
         deadtime (float): The dead time or begin time in seconds before the FID signal starts.
         normalize_fid (bool): If True, normalize the FID data.
         flip_axis (bool): If True, flip the FID axis by taking the complex conjugate. Useful in some GE scanners where the MNS axis needs to be flipped.
         preview (bool): If True, display a preview plot of the original and initialized FID spectra.
         xlim (tuple): The x-axis limits for the preview plot in ppm.
         truncate_initial_points (int): Truncate initial points from FID to remove fast decaying components (e.g. macromolecule).
                                        This usually makes baseline more flat.
-        g_global (float, optional): Global value for the 'g' parameter. Defaults to 0.0. If set to False,
+        g_global (float, optional): Global value for the ``g`` parameter. Defaults to 0.0. If set to False,
         the g values specified in the prior knowledge will be used.
         carrier (float, optional): The carrier frequency in ppm, often used for water (4.7 ppm) or other reference metabolite such as Phosphocreatine (0 ppm).
         ppm_offset (float, optional): Adjust the ppm in priorknowledgefile. Default 0 ppm
+        noise_var (str or float): Method or value used to estimate the noise variance in the data. Options include:
+
+            - ``OXSA``: Uses the default noise variance estimation method employed by OXSA. See ``pyAMARES.util.crlb.evaluateCRB`` for details. 
+            - ``jMRUI``: Employs the default noise variance estimation method used by jMRUI. 
+            - A float value: Directly specifies the noise variance calculated externally.
+
     Returns:
         argparse.Namespace: An object containing FID fitting parameters.
     """
     if fid is None:
         print("Warning, fid is None!")
         fid = np.ones(1024, dtype=complex)
 
@@ -426,37 +440,43 @@
     # print(f"{-sw/2=}")
 
     opts = argparse.Namespace()
     opts.deadtime = deadtime
     opts.timeaxis = np.arange(0, dwelltime * fidpt, dwelltime) + deadtime
     # opts.timeaxis = np.linspace(deadtime, at, fidpt)
     opts.carrier = carrier  # 4.7 for water, 0 for PCr
-
+    if flip_axis:
+        # This must be done before the shifting FID for carrier. 
+        fid = np.conj(fid)
+    if carrier != 0:
+        print("Shift FID so that center frequency is at %s ppm!" % carrier)
+        fid = fid * np.exp(1j * 2 * np.pi * carrier * MHz * opts.timeaxis)
+        # ppm = ppm + carrier
+        # Hz = Hz + carrier / np.abs(MHz)
     # xlim is always ppm
     if xlim is None:
         opts.xlim = np.array((sw / 2, -sw / 2)) / np.abs(MHz)  # xlim should be Hz
     else:
         opts.xlim = np.array(xlim)
     opts.xlim_Hz = opts.xlim * MHz
 
     if normalize_fid:
         opts.fid = fid / np.max(fid)
     else:
         opts.fid = fid.copy()
-    if flip_axis:
-        opts.fid = np.conj(opts.fid)
     opts.spec = np.fft.fftshift(np.fft.fft(opts.fid))
 
     opts.MHz = MHz
     opts.ppm = ppm
     opts.Hz = Hz
     opts.dwelltime = dwelltime
     opts.deadpts = int(deadtime // dwelltime)
     opts.g_global = g_global  # for HSVD initialization
     opts.ppm_offset = ppm_offset
+    opts.noise_var = noise_var
 
     plotParameters = argparse.Namespace()
     plotParameters.deadtime = deadtime
     plotParameters.lb = lb  # linebroadening, Hz
     plotParameters.sw = sw  # spectrum widt, Hz
     plotParameters.xlim = xlim  # xlim, in ppm, such as (10, -20)
     plotParameters.ifphase = (
```

### Comparing `pyAMARES-0.3.0/pyAMARES/kernel/fid.py` & `pyAMARES-0.3.8/pyAMARES/kernel/fid.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/kernel/lmfit.py` & `pyAMARES-0.3.8/pyAMARES/kernel/lmfit.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/kernel/objective_func.py` & `pyAMARES-0.3.8/pyAMARES/kernel/objective_func.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/libs/MPFIR.py` & `pyAMARES-0.3.8/pyAMARES/libs/MPFIR.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/libs/hlsvd.py` & `pyAMARES-0.3.8/pyAMARES/libs/hlsvd.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/script/amaresfit.py` & `pyAMARES-0.3.8/pyAMARES/script/amaresfit.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/util/crlb.py` & `pyAMARES-0.3.8/pyAMARES/util/crlb.py`

 * *Files 6% similar despite different names*

```diff
@@ -106,15 +106,31 @@
 
     Returns:
         numpy.ndarray: The Cramer-Rao Bound (CRB) values calculated for the given parameters.
         Note: `opts` will be modified in place.
     """
     opts.D = Jacfunc(outparams, opts.timeaxis)
     opts.residual = uninterleave(multieq6(outparams, opts.timeaxis)) - opts.fid
-    opts.variance = np.var(opts.residual.real)
+    if opts.noise_var.startswith("OXSA"):
+        print("Estimated CRLBs are calculated using the default noise variance estimation used by OXSA.")
+        opts.variance = np.var(
+            opts.residual.real
+        )  # OXSA style, the "noise as SD in TD from TD residue" option selected in the Result Window of jMRUI V7. 
+    elif opts.noise_var.lower().startswith("jmrui"):
+        print("Estimated CRLBs are calculated using the default noise variance estimation used by jMRUI.")
+        opts.variance = np.var(
+            opts.fid[-len(opts.fid)//10 :].real
+        )  # jMRUI style, "noise as SD in TD from TD FID tall option selected in the Result Window of jMRUI V7" (I hard-coded last 10% points)
+    else:
+        try:
+            opts.variance = float(opts.noise_var)
+            print("The CRLB estimation will be divided by the input variance %s" % opts.variance)
+        except ValueError:
+            print("Error: noise_var %s is not a recognized string or a valid number." % opts.variance)
+
     if verbose:
         print("opts.D.shape=%s" % str(opts.D.shape))
         plt.plot(opts.residual.real)
         plt.title("residual")
         plt.show()
     opts.crlb = calculateCRB(opts.D, opts.variance, P=P, verbose=verbose)
     opts.resultpd = report_crlb(outparams=outparams, crlb=opts.crlb, Jacfunc=Jacfunc)
```

### Comparing `pyAMARES-0.3.0/pyAMARES/util/hsvd.py` & `pyAMARES-0.3.8/pyAMARES/util/hsvd.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/util/multiprocessing.py` & `pyAMARES-0.3.8/pyAMARES/util/multiprocessing.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/util/report.py` & `pyAMARES-0.3.8/pyAMARES/util/report.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES/util/visualization.py` & `pyAMARES-0.3.8/pyAMARES/util/visualization.py`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/pyAMARES.egg-info/PKG-INFO` & `pyAMARES-0.3.8/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyAMARES
-Version: 0.3.0
+Version: 0.3.8
 Summary: pyAMARES, an Open-Source Python Library for Fitting Magnetic Resonance Spectroscopy Data
 Home-page: https://github.com/hawkMRS/pyAMARES
 Author: Jia Xu, MR Research Facility, University of Iowa
 Author-email: jia-xu-1@uiowa.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -21,59 +21,80 @@
 Provides-Extra: docs
 Provides-Extra: jupyter
 License-File: LICENSE.txt
 
 **pyAMARES**, an Open-Source Python Library for Fitting Magnetic Resonance Spectroscopy Data
 ********************************************************************************************
 
-.. image:: pyAMARES_logo.svg
+.. image:: https://raw.githubusercontent.com/HawkMRS/pyAMARES/main/pyAMARES_logo.svg
    :width: 400
 
+The full documentation for pyAMARES can be found at `pyAMARES Documentation <https://pyamares.readthedocs.io/en/latest/index.html>`_.
+
 What is pyAMARES?
 =================
 
-PyAMARES package to provide the MRS community with open-source, easy-to-use MRS fitting method in Python.  
-It imports prior knowledge from Excel or CSV spreadsheets as initial values and constraints for fitting MRS data according to the AMARES model function. 
+The pyAMARES package provides the MRS community with an open-source, easy-to-use MRS fitting method in Python. 
+It imports prior knowledge from Excel or CSV spreadsheets as initial values and constraints for fitting MRS data 
+according to the AMARES model function.
+
+
 
 Getting Started
 ===============
 
+Requirements
+------------
+
+.. image:: https://img.shields.io/badge/Python->%3D3.6%2C%203.8+-blue.svg
+   :target: https://python.org
+   :alt: Python Version
+
+.. note::
+   PyAMARES requires Python 3.6 or newer. We recommend using Python 3.8 or newer. If you are using an older version of Python, you will need to upgrade to use pyAMARES.
+
 Installation
 ------------
+
 .. code-block:: bash
 
    pip install pyAMARES
 
+See the `Installation Guide <https://pyamares.readthedocs.io/en/latest/install.html>`_ for detailed information.
+
 Run pyAMARES as standard-alone script
 -------------------------------------
 
 
 .. code-block:: bash
 
    amaresFit -f ./pyAMARES/examples/fid.txt -p  ./pyAMARES/examples/example_human_brain_31P_7T.csv --MHz 120.0 --sw 10000 --deadtime 300e-6 --ifplot --xlim 10 -20 -o simple_example 
 
 Run pyAMARES in a Jupyter Notebook
 ----------------------------------
+**Try Jupyter Notebook on Google Colab** `here <https://colab.research.google.com/drive/184_7MJ6O1BgGYyqNvnXXqtri4_0N4ySw?usp=sharing>`_
 
 .. code-block:: python
 
    import pyAMARES
    # Load FID from a 2-column ASCII file, and set the MR parameters
    MHz = 120.0 # 31P nuclei at 7T
    sw = 10000 # spectrum width in Hz
    deadtime = 300e-6 # 300 us begin time for the FID signal acquisition
 
    fid = pyAMARES.readmrs('./pyAMARES/examples/fid.txt')
    # Load Prior Knowledge
    FIDobj = pyAMARES.initialize_FID(fid=fid, 
-                                    priorknowledge='./pyAMARES/examples/example_human_brain_31P_7T.csv',
+                                    priorknowledgefile='./pyAMARES/examples/example_human_brain_31P_7T.csv',
                                     MHz=MHz, 
                                     sw=sw,
                                     deadtime=deadtime, 
-                                    preview=False)
+                                    preview=False, 
+                                    normalize_fid=False,
+                                    xlim=(10, -20))# Region of Interest for visualization, -20 to 10 ppm
 
    # Initialize the parameter using Levenberg-Marquard method
    out1 = pyAMARES.fitAMARES(fid_parameters=FIDobj,
                               fitting_parameters=FIDobj.initialParams,
                               method='leastsq',
                               ifplot=False)
 
@@ -82,26 +103,27 @@
    out2 = pyAMARES.fitAMARES(fid_parameters=out1,
                              fitting_parameters=out1.fittedParams, # optimized parameter for last step
                              method='least_squares',
                              ifplot=False)
    
    # Save the data
    out2.styled_df.to_html('simple_example.html') # Save highlighted table to an HTML page
-   out2.result_sum.to_cscv('simple_example.csv') # Save table to CSV spreadsheet
-   out2.plotParameters.lb = 2.0 # Line Braodening
+                                                 # Python 3.6 does not support to_html. 
+   out2.result_sum.to_csv('simple_example.csv') # Save table to CSV spreadsheet
+   out2.plotParameters.lb = 2.0 # Line Broadening factor for visualization
    out2.plotParameters.ifphase = True # Phase the spectrum for visualization
    pyAMARES.plotAMARES(fid_parameters=out1, filename='simple_example.svg') # Save plot to SVG 
 
-Fitting Result
---------------
+Fitting Result for Example 31P MRS data
+------------------------------------------
 
-.. image:: pyAMARES/examples/simple_example.svg
+.. image:: https://raw.githubusercontent.com/HawkMRS/pyAMARES/main/pyAMARES/examples/simple_example.svg
    :width: 400
 
-.. image:: pyAMARES/examples/simple_example_html.jpeg
+.. image:: https://github.com/HawkMRS/pyAMARES/blob/4f9ca4431c0d72e1b41fb2b434f72e53feb1657f/pyAMARES/examples/simple_example_html.jpeg
    :width: 400
 
 How to cite
 ===========
 
 If you use pyAMARES in your research, please consider citing the following ISMRM proceeding:
```

### Comparing `pyAMARES-0.3.0/pyAMARES.egg-info/SOURCES.txt` & `pyAMARES-0.3.8/pyAMARES.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,14 @@
+CHANGELOG.rst
 LICENSE.txt
 MANIFEST.in
 README.rst
 pyAMARES_logo.svg
 requirements.txt
+setup.cfg
 setup.py
 pyAMARES/__init__.py
 pyAMARES.egg-info/PKG-INFO
 pyAMARES.egg-info/SOURCES.txt
 pyAMARES.egg-info/dependency_links.txt
 pyAMARES.egg-info/entry_points.txt
 pyAMARES.egg-info/not-zip-safe
@@ -16,15 +18,17 @@
 pyAMARES/examples/fid.txt
 pyAMARES/examples/human_brain_31P_7T.csv
 pyAMARES/examples/simple_example.csv
 pyAMARES/examples/simple_example.html
 pyAMARES/examples/simple_example.svg
 pyAMARES/examples/simple_example_html.jpeg
 pyAMARES/fileio/__init__.py
+pyAMARES/fileio/readfidall.py
 pyAMARES/fileio/readmat.py
+pyAMARES/fileio/readnifti.py
 pyAMARES/kernel/PriorKnowledge.py
 pyAMARES/kernel/__init__.py
 pyAMARES/kernel/fid.py
 pyAMARES/kernel/lmfit.py
 pyAMARES/kernel/objective_func.py
 pyAMARES/libs/MPFIR.py
 pyAMARES/libs/__init__.py
```

### Comparing `pyAMARES-0.3.0/pyAMARES_logo.svg` & `pyAMARES-0.3.8/pyAMARES_logo.svg`

 * *Files identical despite different names*

### Comparing `pyAMARES-0.3.0/setup.py` & `pyAMARES-0.3.8/setup.py`

 * *Files identical despite different names*

