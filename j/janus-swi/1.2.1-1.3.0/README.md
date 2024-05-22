# Comparing `tmp/janus_swi-1.2.1.tar.gz` & `tmp/janus_swi-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_swi-1.2.1.tar", last modified: Fri May 17 08:02:45 2024, max compression
+gzip compressed data, was "janus_swi-1.3.0.tar", last modified: Wed May 22 09:53:54 2024, max compression
```

## Comparing `janus_swi-1.2.1.tar` & `janus_swi-1.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.861220 janus_swi-1.2.1/
--rw-r--r--   0 jan       (1000) jan       (1000)       83 2023-09-03 11:56:51.000000 janus_swi-1.2.1/.gitignore
--rw-r--r--   0 jan       (1000) jan       (1000)     2180 2024-04-23 15:19:04.000000 janus_swi-1.2.1/CMakeLists.txt
--rw-r--r--   0 jan       (1000) jan       (1000)     6657 2024-05-17 08:02:45.861220 janus_swi-1.2.1/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)     6125 2023-12-08 12:29:10.000000 janus_swi-1.2.1/README.md
--rw-r--r--   0 jan       (1000) jan       (1000)        6 2024-05-17 07:56:51.000000 janus_swi-1.2.1/VERSION
--rw-r--r--   0 jan       (1000) jan       (1000)       82 2024-02-02 10:15:19.000000 janus_swi-1.2.1/config.h.cmake
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.858219 janus_swi-1.2.1/examples/
--rw-r--r--   0 jan       (1000) jan       (1000)      443 2023-08-03 15:55:23.000000 janus_swi-1.2.1/examples/SpaCY.md
--rw-r--r--   0 jan       (1000) jan       (1000)      394 2023-08-03 15:55:23.000000 janus_swi-1.2.1/examples/spacy.pl
--rw-r--r--   0 jan       (1000) jan       (1000)      200 2023-10-16 09:41:10.000000 janus_swi-1.2.1/examples/trains.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.858219 janus_swi-1.2.1/gen/
--rw-r--r--   0 jan       (1000) jan       (1000)      726 2023-09-07 10:01:02.000000 janus_swi-1.2.1/gen/janus.bbl
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.858219 janus_swi-1.2.1/janus/
--rw-r--r--   0 jan       (1000) jan       (1000)      925 2023-09-03 12:39:21.000000 janus_swi-1.2.1/janus/__init__.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1261 2023-11-09 16:44:28.000000 janus_swi-1.2.1/janus/_find_swipl.py
--rw-r--r--   0 jan       (1000) jan       (1000)     4634 2023-11-08 13:09:52.000000 janus_swi-1.2.1/janus/hash.c
--rw-r--r--   0 jan       (1000) jan       (1000)    58165 2024-05-17 07:55:49.000000 janus_swi-1.2.1/janus/janus.c
--rw-r--r--   0 jan       (1000) jan       (1000)    45100 2024-03-24 17:26:38.000000 janus_swi-1.2.1/janus/janus.pl
--rw-r--r--   0 jan       (1000) jan       (1000)    19808 2024-05-17 07:59:51.000000 janus_swi-1.2.1/janus/janus.py
--rw-r--r--   0 jan       (1000) jan       (1000)      113 2023-09-03 11:56:51.000000 janus_swi-1.2.1/janus/janus_swi.py
--rw-r--r--   0 jan       (1000) jan       (1000)    16902 2024-05-17 07:55:49.000000 janus_swi-1.2.1/janus/mod_swipl.c
--rw-r--r--   0 jan       (1000) jan       (1000)    56534 2024-04-23 15:27:36.000000 janus_swi-1.2.1/janus.doc
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.861220 janus_swi-1.2.1/janus_swi.egg-info/
--rw-r--r--   0 jan       (1000) jan       (1000)     6657 2024-05-17 08:02:45.000000 janus_swi-1.2.1/janus_swi.egg-info/PKG-INFO
--rw-r--r--   0 jan       (1000) jan       (1000)      915 2024-05-17 08:02:45.000000 janus_swi-1.2.1/janus_swi.egg-info/SOURCES.txt
--rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-17 08:02:45.000000 janus_swi-1.2.1/janus_swi.egg-info/dependency_links.txt
--rw-r--r--   0 jan       (1000) jan       (1000)       10 2024-05-17 08:02:45.000000 janus_swi-1.2.1/janus_swi.egg-info/top_level.txt
--rw-r--r--   0 jan       (1000) jan       (1000)      589 2023-09-19 08:05:44.000000 janus_swi-1.2.1/pyproject.toml
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.859219 janus_swi-1.2.1/scripts/
--rwxr-xr-x   0 jan       (1000) jan       (1000)     1582 2023-12-15 13:16:39.000000 janus_swi-1.2.1/scripts/newversion
--rwxrwxr-x   0 jan       (1000) jan       (1000)      310 2023-12-17 16:29:23.000000 janus_swi-1.2.1/scripts/pypi-upload
--rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-17 08:02:45.861220 janus_swi-1.2.1/setup.cfg
--rw-r--r--   0 jan       (1000) jan       (1000)     1651 2024-05-17 07:59:51.000000 janus_swi-1.2.1/setup.py
--rw-r--r--   0 jan       (1000) jan       (1000)    14985 2024-05-17 07:55:49.000000 janus_swi-1.2.1/test_janus.pl
--rw-r--r--   0 jan       (1000) jan       (1000)     8218 2024-01-16 08:48:38.000000 janus_swi-1.2.1/test_xsb_janus.pl
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.860220 janus_swi-1.2.1/tests/
--rw-r--r--   0 jan       (1000) jan       (1000)       28 2023-09-07 07:25:25.000000 janus_swi-1.2.1/tests/baseclasses.py
--rw-r--r--   0 jan       (1000) jan       (1000)     5706 2023-11-01 16:45:15.000000 janus_swi-1.2.1/tests/bench.pl
--rw-r--r--   0 jan       (1000) jan       (1000)     4023 2024-05-17 07:55:49.000000 janus_swi-1.2.1/tests/demo.py
--rw-r--r--   0 jan       (1000) jan       (1000)      275 2023-12-20 20:35:11.000000 janus_swi-1.2.1/tests/dog.py
--rw-rw-r--   0 jan       (1000) jan       (1000)      170 2023-07-28 09:08:08.000000 janus_swi-1.2.1/tests/russel.pl
--rw-r--r--   0 jan       (1000) jan       (1000)      586 2023-10-16 09:28:16.000000 janus_swi-1.2.1/tests/threads.py
--rw-r--r--   0 jan       (1000) jan       (1000)      188 2023-10-16 09:41:10.000000 janus_swi-1.2.1/tests/while.py
-drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-17 08:02:45.861220 janus_swi-1.2.1/xsb_tests/
--rw-r--r--   0 jan       (1000) jan       (1000)     2101 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/Person.py
--rw-r--r--   0 jan       (1000) jan       (1000)     2256 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/jintf.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1322 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/kwargs.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1286 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/numpexamp.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1946 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/returnVal.py
--rw-r--r--   0 jan       (1000) jan       (1000)      568 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/sample.json
--rw-r--r--   0 jan       (1000) jan       (1000)     1824 2023-09-07 07:29:42.000000 janus_swi-1.2.1/xsb_tests/stressTest.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1338 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/sumlist3.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1320 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/test_err.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1685 2023-09-07 07:30:23.000000 janus_swi-1.2.1/xsb_tests/test_stress.pl
--rw-r--r--   0 jan       (1000) jan       (1000)     1289 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/testc.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1400 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/tupInList.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1260 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/tupletest.py
--rw-r--r--   0 jan       (1000) jan       (1000)     1392 2023-09-03 11:56:51.000000 janus_swi-1.2.1/xsb_tests/variadic.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.319128 janus_swi-1.3.0/
+-rw-r--r--   0 jan       (1000) jan       (1000)       83 2023-09-03 11:56:51.000000 janus_swi-1.3.0/.gitignore
+-rw-r--r--   0 jan       (1000) jan       (1000)     2180 2024-04-23 15:19:04.000000 janus_swi-1.3.0/CMakeLists.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)     6657 2024-05-22 09:53:54.319128 janus_swi-1.3.0/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)     6125 2023-12-08 12:29:10.000000 janus_swi-1.3.0/README.md
+-rw-r--r--   0 jan       (1000) jan       (1000)        6 2024-05-22 09:53:05.000000 janus_swi-1.3.0/VERSION
+-rw-r--r--   0 jan       (1000) jan       (1000)       82 2024-02-02 10:15:19.000000 janus_swi-1.3.0/config.h.cmake
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.315128 janus_swi-1.3.0/examples/
+-rw-r--r--   0 jan       (1000) jan       (1000)      443 2023-08-03 15:55:23.000000 janus_swi-1.3.0/examples/SpaCY.md
+-rw-r--r--   0 jan       (1000) jan       (1000)      394 2023-08-03 15:55:23.000000 janus_swi-1.3.0/examples/spacy.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)      200 2023-10-16 09:41:10.000000 janus_swi-1.3.0/examples/trains.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.315128 janus_swi-1.3.0/gen/
+-rw-r--r--   0 jan       (1000) jan       (1000)      726 2023-09-07 10:01:02.000000 janus_swi-1.3.0/gen/janus.bbl
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.316128 janus_swi-1.3.0/janus/
+-rw-r--r--   0 jan       (1000) jan       (1000)      925 2023-09-03 12:39:21.000000 janus_swi-1.3.0/janus/__init__.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1261 2023-11-09 16:44:28.000000 janus_swi-1.3.0/janus/_find_swipl.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     4634 2023-11-08 13:09:52.000000 janus_swi-1.3.0/janus/hash.c
+-rw-r--r--   0 jan       (1000) jan       (1000)    58174 2024-05-22 08:22:25.000000 janus_swi-1.3.0/janus/janus.c
+-rw-r--r--   0 jan       (1000) jan       (1000)    45100 2024-03-24 17:26:38.000000 janus_swi-1.3.0/janus/janus.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)    19882 2024-05-22 09:53:13.000000 janus_swi-1.3.0/janus/janus.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      113 2023-09-03 11:56:51.000000 janus_swi-1.3.0/janus/janus_swi.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    16902 2024-05-17 07:55:49.000000 janus_swi-1.3.0/janus/mod_swipl.c
+-rw-r--r--   0 jan       (1000) jan       (1000)    58561 2024-05-22 08:22:25.000000 janus_swi-1.3.0/janus.doc
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.319128 janus_swi-1.3.0/janus_swi.egg-info/
+-rw-r--r--   0 jan       (1000) jan       (1000)     6657 2024-05-22 09:53:54.000000 janus_swi-1.3.0/janus_swi.egg-info/PKG-INFO
+-rw-r--r--   0 jan       (1000) jan       (1000)      915 2024-05-22 09:53:54.000000 janus_swi-1.3.0/janus_swi.egg-info/SOURCES.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)        1 2024-05-22 09:53:54.000000 janus_swi-1.3.0/janus_swi.egg-info/dependency_links.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)       10 2024-05-22 09:53:54.000000 janus_swi-1.3.0/janus_swi.egg-info/top_level.txt
+-rw-r--r--   0 jan       (1000) jan       (1000)      589 2023-09-19 08:05:44.000000 janus_swi-1.3.0/pyproject.toml
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.317128 janus_swi-1.3.0/scripts/
+-rwxr-xr-x   0 jan       (1000) jan       (1000)     1582 2023-12-15 13:16:39.000000 janus_swi-1.3.0/scripts/newversion
+-rwxrwxr-x   0 jan       (1000) jan       (1000)      310 2023-12-17 16:29:23.000000 janus_swi-1.3.0/scripts/pypi-upload
+-rw-r--r--   0 jan       (1000) jan       (1000)       38 2024-05-22 09:53:54.319128 janus_swi-1.3.0/setup.cfg
+-rw-r--r--   0 jan       (1000) jan       (1000)     1651 2024-05-22 09:53:13.000000 janus_swi-1.3.0/setup.py
+-rw-r--r--   0 jan       (1000) jan       (1000)    16665 2024-05-22 08:22:25.000000 janus_swi-1.3.0/test_janus.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)     8218 2024-01-16 08:48:38.000000 janus_swi-1.3.0/test_xsb_janus.pl
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.317128 janus_swi-1.3.0/tests/
+-rw-r--r--   0 jan       (1000) jan       (1000)       28 2023-09-07 07:25:25.000000 janus_swi-1.3.0/tests/baseclasses.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     5706 2023-11-01 16:45:15.000000 janus_swi-1.3.0/tests/bench.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)     7578 2024-05-22 08:22:25.000000 janus_swi-1.3.0/tests/demo.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      275 2023-12-20 20:35:11.000000 janus_swi-1.3.0/tests/dog.py
+-rw-rw-r--   0 jan       (1000) jan       (1000)      170 2023-07-28 09:08:08.000000 janus_swi-1.3.0/tests/russel.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)      582 2024-05-22 08:22:25.000000 janus_swi-1.3.0/tests/threads.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      193 2024-05-22 08:22:25.000000 janus_swi-1.3.0/tests/while.py
+drwxr-xr-x   0 jan       (1000) jan       (1000)        0 2024-05-22 09:53:54.319128 janus_swi-1.3.0/xsb_tests/
+-rw-r--r--   0 jan       (1000) jan       (1000)     2101 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/Person.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     2256 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/jintf.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1322 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/kwargs.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1286 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/numpexamp.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1946 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/returnVal.py
+-rw-r--r--   0 jan       (1000) jan       (1000)      568 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/sample.json
+-rw-r--r--   0 jan       (1000) jan       (1000)     1824 2023-09-07 07:29:42.000000 janus_swi-1.3.0/xsb_tests/stressTest.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1338 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/sumlist3.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1320 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/test_err.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1685 2023-09-07 07:30:23.000000 janus_swi-1.3.0/xsb_tests/test_stress.pl
+-rw-r--r--   0 jan       (1000) jan       (1000)     1289 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/testc.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1400 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/tupInList.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1260 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/tupletest.py
+-rw-r--r--   0 jan       (1000) jan       (1000)     1392 2023-09-03 11:56:51.000000 janus_swi-1.3.0/xsb_tests/variadic.py
```

### Comparing `janus_swi-1.2.1/CMakeLists.txt` & `janus_swi-1.3.0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/PKG-INFO` & `janus_swi-1.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus_swi
-Version: 1.2.1
+Version: 1.3.0
 Summary: Janus library to call SWI-Prolog
 Home-page: https://github.com/SWI-Prolog/packages-swipy
 Author: Jan Wielemaker
 Author-email: Jan Wielemaker <jan@swi-prolog.org>
 License: BSD-2-Clause
 Project-URL: Homepage, https://www.swi-prolog.org
 Project-URL: Documentation, https://www.swi-prolog.org/pldoc/package/janus
```

### Comparing `janus_swi-1.2.1/README.md` & `janus_swi-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/gen/janus.bbl` & `janus_swi-1.3.0/gen/janus.bbl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus/__init__.py` & `janus_swi-1.3.0/janus/__init__.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus/_find_swipl.py` & `janus_swi-1.3.0/janus/_find_swipl.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus/hash.c` & `janus_swi-1.3.0/janus/hash.c`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus/janus.c` & `janus_swi-1.3.0/janus/janus.c`

 * *Files 0% similar despite different names*

```diff
@@ -2344,15 +2344,15 @@
   if ( !py_gil_ensure(&state) )
     return FALSE;
   if ( (rc=py_from_prolog(t, &obj)) )
   { PyObject *s = check_error(PyObject_Str(obj));
     Py_DECREF(obj);
 
     if ( s )
-    { rc = py_unify(str, s, 0);
+    { rc = py_unify(str, s, PYU_STRING);
       Py_DECREF(s);
     } else
       rc = FALSE;
   }
   py_gil_release(state);
 
   return rc;
```

### Comparing `janus_swi-1.2.1/janus/janus.pl` & `janus_swi-1.3.0/janus/janus.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus/janus.py` & `janus_swi-1.3.0/janus/janus.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 if not hasattr(_swipl, 'call'):
     raise RuntimeError(f"Loaded wrong module '_swipl' from {_swipl.__file__}")
 
 ################################################################
 # Versions
 
 # 10000*major + 100*minor + patch
-version_num=10201
+version_num=10300
 
 def version_str(num=version_num):
     """
     Return Janus version as major.minor.patch
     """
     return f"{num//10000}.{num%10000//100}.{num%100}"
 
@@ -198,29 +198,31 @@
         inputs['truth'] = truth_vals
         self.state = _swipl.open_query(query, inputs)
     def __iter__(self):
         """Implement iter protocol"""
         return self
     def __next__(self):
         """Implement iter protocol.  Returns a dict as janus.query_once()"""
-        rc = _swipl.next_solution(self.state)
-        if rc == False or rc["truth"] == False:
+        rc = self.next()
+        if rc is None:
             raise StopIteration()
-        else:
-            return rc
+        return rc
+    def __enter__(self):
+        """Implement context manager protocol"""
+        return self
+    def __exit__(self, type, value, tb):
+        """Implement context manager protocol"""
+        self.close()
     def __del__(self):
         """Close the Prolog query"""
-        _swipl.close_query(self.state)
+        self.close()
     def next(self):
         """Allow for explicit enumeration,  Returns None or a dict"""
         rc = _swipl.next_solution(self.state)
-        if rc == False or rc["truth"] == False:
-            return None
-        else:
-            return rc
+        return None if rc == False or rc["truth"] == False else rc
     def close(self):
         """Explicitly close the query."""
         _swipl.close_query(self.state)
 
 def query_once(query, inputs={}, keep=False, truth_vals=TruthVal.PLAIN_TRUTHVALS):
     """
     Call a Prolog predicate as `query_once/1`
@@ -249,15 +251,15 @@
     pass
 
 def once(query, inputs={}, keep=False, truth_vals=TruthVal.PLAIN_TRUTHVALS):
     """
     Deprecated.  Renamed to query_once().
     """
     return query_once(query, inputs, keep, truth)
-    
+
 ################################################################
 # Functional style interface
 
 # Ideally, we'd define apply_once() and pass on the arguments.  This
 # however is considerably slower and in C we can detect the absence
 # of `fail=`, which we seems impossible in Python.
 
@@ -460,15 +462,15 @@
     """Represent any Prolog term
 
     Class `Term` is much like the Python object reference that we have
     in Prolog: it represents an arbitrary Prolog term we cannot represent
     in Python.  Instances are created if data is passed to Python as
     `prolog(Term)`.  Upon transforming the data back to Prolog, the
     interface recovers a copy of the original Prolog terms.
-    
+
     The user should never create instances of this explicitly.
     """
 
     def __init__(self, record):
         """Create from a Prolog record pointer. DO NOT USE!"""
         self._record = record;
     def __str__(self):
```

### Comparing `janus_swi-1.2.1/janus/mod_swipl.c` & `janus_swi-1.3.0/janus/mod_swipl.c`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/janus.doc` & `janus_swi-1.3.0/janus.doc`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
   Prolog predicates using the calling conventions of
   \cfuncref{janus.query_once}{} and \cfuncref{janus.apply_once}{}.
 \end{itemize}
 
 The API of Janus is the result of discussions between the SWI-Prolog,
 XSB and Ciao lang teams.  It will be reflected in a PIP
 (\jargon{Prolog Improvement Proposal}).  Considering the large
-differences in design an opinions in Prolog implementation, the PIP
+differences in designs and opinions in Prolog implementation, the PIP
 does not cover all aspects of the API.  Many of the predicates and
 functions have a \jargon{Compatibility} note that explains the
 relation of the SWI-Prolog API and the PIP.  We summarize the
 differences in \secref{janus-vs-xsb}.
 
 
 \section{Data conversion}
@@ -190,15 +190,15 @@
 Using Prolog \jargon{comma lists}, e.g., \verb$(a,b,c)$ does not
 implement array semantics, cannot represent empty tuples and cannot
 disambiguate tuples with one element from the element itself.  We
 settled with compound terms using the \const{-} as functor to make
 the common binary tuple map to a Prolog \jargon{pair}.
 
 
-\section{Janus by example}
+\section{Janus by example - Prolog calling Python}
 \label{sec:janus-examples}
 
 This section introduces Janus calling Python from Prolog with examples.
 
 \subsection{Janus calling spaCy}
 \label{sec:janus-spacy}
 
@@ -347,15 +347,15 @@
   The value for a \term{py_string_as}{As} option is invalid.  For
   example, \exam{py_call(m:f(), R, [py_string_as(codes)])}
   \termitem{py_dict_as}{}
   The value for a \term{py_dict_as}{As} option is invalid.  For
   example, \exam{py_call(m:f(), R, [py_dict_as(list)])}
   \termitem{py_term}{}
   A term being translated to Python is unsupported.  For example,
-  \exam{py_call(m:f(point(1,2), R)}.
+  \exam{py_call(m:f(point(1,2)), R)}.
 \end{description}
 
 Defined \textbf{types} are:
 
 \begin{description}
   \termitem{py_object}{}
   A Python object reference was expected.  For example,
@@ -367,15 +367,15 @@
   and the \const{__str__()} method does not produce a correct string.
   \termitem{py_key_value}{}
   Inside a \exam{\{k:v, \ldots\}} representation for a dictionary we
   find a term that is not a key-value pair.  For example,
   \exam{py_call(m:f(\{a:1, x\}), R)}
   \termitem{py_set}{}
   Inside a \term{py_set}{Elements}, \arg{Elements} is not a list.
-  For example, \exam{py_call(m:f(py_set(42), R)}.
+  For example, \exam{py_call(m:f(py_set(42)), R)}.
   \termitem{py_target}{}
   In \term{py_call}{Target:FuncOrAttrOrMethod}, \arg{Target} is not
   a module (atom) or Python object reference.
   For example, \exam{py_call(7:f(), R)}.
   \termitem{py_callable}{}
   In \term{py_call}{Target:FuncOrAttrOrMethod}, \arg{FuncOrAttrOrMethod}
   is not an atom or compound.
@@ -427,15 +427,15 @@
 between Python and Prolog are supported.  They should be handled with
 some care as it is easy to crash the process due to a stack overflow.
 
 Loading janus into Python is realized using the Python package
 \const{janus-swi}, which defines the module \const{janus_swi}.  We do
 not call this simply \const{janus} to allow coexistence of Janus for
 multiple Prolog implementations.  Unless you plan to interact with
-multiple Prolog systems in the same session, we advice to import janus
+multiple Prolog systems in the same session, we advise importing janus
 for SWI-Prolog as below.
 
 \begin{code}
 import janus_swi as janus
 \end{code}
 
 If Python is embedded into SWI-Prolog, the Python module may be
@@ -560,31 +560,60 @@
 contains a \const{truth} field.  This field cannot be \const{False}
 though and thus is either \const{True} or an instance of the class
 \cfuncref{janus.Undefined}{}
 
 \begin{code}
 import janus_swi as janus
 
-def printRange(from, to):
-    for d in janus.query("between(F,T,X)", {"F":from, "T":to})
+def printRange(fr, to):
+    for d in janus.query("between(F,T,X)", {"F":fr, "T":to}):
         print(d["X"])
 \end{code}
 
+The call to janus.query() returns an object that implements
+both the iterator protocol and the context manager protocol. A
+context manager ensures that the query is cleaned up as soon as it
+goes out of scope - Python typically does this with for loops, but
+there is no guarantee of when cleanup happens, especially if there
+is an error. (You can think of a \const{with} statement as similar
+to Prolog's setup_call_cleanup/3.)
+Using a context manager, we can write
+
+\begin{code}
+def printRange(fr, to):
+    with janus.query("between(F,T,X)", {"F":fr, "T":to}) as d_q:
+        for d in d_q:
+            print(d["X"])
+\end{code}
+
 Iterators may be nested.  For example,  we can create a list of tuples
 like below.
 
 \begin{code}
 def double_iter(w,h):
     tuples=[]
     for yd in janus.query("between(1,M,Y)", {"M":h}):
         for xd in janus.query("between(1,M,X)", {"M":w}):
             tuples.append((xd['X'],yd['Y']))
     return tuples
 \end{code}
 
+or, using context managers:
+
+\begin{code}
+def doc_double_iter(w,h):
+    tuples=[]
+    with janus.query("between(1,M,Y)", {"M":h}) as yd_q:
+        for yd in yd_q:
+            with janus.query("between(1,M,X)", {"M":w}) as xd_q:
+                for xd in xd_q:
+                    tuples.append((xd['X'],yd['Y']))
+    return tuples
+\end{code}
+
 After this, we may run
 
 \begin{code}
 >>> demo.double_iter(2,3)
 [(1, 1), (2, 1), (1, 2), (2, 2), (1, 3), (2, 3)]
 \end{code}
 
@@ -596,14 +625,34 @@
 \begin{code}
     q = query("between(1,3,X)")
     while ( s := q.next() ):
         print(s['X'])
     q.close()
 \end{code}
 
+or
+
+\begin{code}
+  try:
+      q = query("between(1,3,X)")
+      while ( s := q.next() ):
+          print(s['X'])
+  finally:
+      q.close()
+\end{code}
+
+The close() is called by the context manager, so the following
+is equivalent:
+
+\begin{code}
+    with query("between(1,3,X)") as q:
+        while ( s := q.next() ):
+            print(s['X'])
+\end{code}
+
 
 But, \textbf{iterators based on Prolog goals are fragile}.  This
 is because, while it is possible to open and run a new query while
 there is an open query, the inner query must be closed before we
 can ask for the next solution of the outer query.  We illustrate
 this using the sequence below.
 
@@ -621,14 +670,17 @@
 {'truth': True, 'X': 1}
 >>> q1.close()
 \end{code}
 
 \textbf{Failure to close a query typically leaves SWI-Prolog in an
 inconsistent state and further interaction with Prolog is likely to
 crash the process}.  Future versions may improve on that.
+To avoid this, it is recommended that you use the query
+with a context manager, that is using the Python const{with}
+statement.
 
 
 \begin{description}
   \cfunction{dict}{janus.query_once}{query, inputs=\{{}\}, keep=False,
 			            truth_vals=TruthVals.PLAIN_TRUTHVALS}
 Call \arg{query} using \arg{bindings} as once/1, returning a dict with
 the resulting bindings. If \arg{bindings} is omitted, no variables are
@@ -767,14 +819,17 @@
 \label{sec:janus-class-query}
 
 Class \cfuncref{janus.query}{} is similar to the
 \cfuncref{janus.query_once}{} function, but it returns a Python
 \jargon{iterator} that allows for iterating over the answers to a
 non-deterministic Prolog predicate.
 
+The iterator also implements the Python context manaager protocol
+(for the Python \const{with} statement).
+
 \begin{description}
    \cfunction{query}{janus.query}{query, inputs=\{{}\}, keep=False}
    As \cfuncref{janus.query_once}{}, returning an \jargon{iterator} that
    provides an answer dict as \cfuncref{janus.query_once}{} for each answer
    to \arg{query}.  Answers never have \const{truth} \const{False}.
    See discussion above.
 
@@ -784,20 +839,26 @@
 
    \cfunction{Query}{janus.Query}{query, inputs=\{{}\}, keep=False}
    \jargon{Deprecated}.  This class was renamed to \cfuncref{janus.query}.
 
    \cfunction{dict{|}None}{janus.query.next}{}
    Explicitly ask for the next solution of the iterator.  Normally,
    using the \ctype{query} as an iterator is to be preferred.  See
-   discussion above.
+   discussion above. \exam{q.next()} is equivalent to \exam{next(q)}
+   except it returns \const{None} if there are no more values instead
+   of raising the \const{StopIteration} exception.
 
    \cfunction{None}{janus.query.close}{}
    Close the query.  Closing a query is obligatory.  When used as
    an iterator, the Python destructor (\cfuncref{__del__}{}) takes
-   care of closing the query.
+   care of closing the query. However, Python does not guarantee
+   when the destructor will be called, so it is recommended that
+   the context manager protocol is used (with the Python \const{with}
+   statement), which closes the query when the query goes out of scope
+   or when an error happens.
 
 \begin{tags}
 \tag{Compatibility} PIP.
 \end{tags}
 \end{description}
 
 \subsection{Janus iterator apply}
@@ -811,15 +872,15 @@
   \cfunction{apply}{janus.apply}{module, predicate, *input}
   As \cfuncref{janus.apply_once}{}, returning an \jargon{iterator}
   that returns individual answers.  The example below uses Python
   \jargon{list comprehension} to create a list of integers from
   the Prolog built-in between/3.
 
 \begin{code}
->>> [*janus.apply("user", "between", 1, 6)]
+>>> list(janus.apply("user", "between", 1, 6))
 [1, 2, 3, 4, 5, 6]
 \end{code}
 
 \begin{tags}
 \tag{Compatibility} PIP.
 \end{tags}
 
@@ -1128,17 +1189,17 @@
 such issues.
 
 \subsection{Janus versions}
 \label{sec:janus-version}
 
 The current version as an integer can be accessed as
 \exam{janus.version}.  The integer uses the same conventions as the
-SWI-Prolog flag \const{version} and is defined as $10,000*Major +
-100*Minor + Patch$.  In addition, the module defines the following
-functions:
+SWI-Prolog flag \const{version} and is defined as
+$10,000*Major + 100*Minor + Patch$.
+In addition, the module defines the following functions:
 
 \begin{description}
   \cfunction{str}{janus.version_str}{}
   Return the Janus version as a string \arg{Major.Minor.Patch}.
   \cfunction{None}{janus.version}{}
   Print information about Janus and SWI-Prolog version.
 \end{description}
@@ -1357,15 +1418,15 @@
   XSB uses a term.  The predicate py_is_object/1 may be used to test
   that a Prolog term refers to a Python object.   In XSB, the user
   \emph{must} call py_free/1 when done with some object.  In SWI-Prolog,
   either py_free/1 may be used or the object may be left to the Prolog
   (atom) garbage collector.
 \item Prolog exceptions passed to Python are represented differently.
 \item When calling Prolog from Python and relying on well founded
-  semantics, only \jargon{plain truth values} (i.e., \const{janus.undefined}
+  semantics, only \jargon{plain truth values} (i.e., \const{janus.undefined})
   are supported in a portable way.  \jargon{Delay lists}, providing
   details on why the result is undefined, are represented differently.
 \end{itemize}
 
 \subsection{Writing portable Janus modules}
 \label{sec:janus-portable-code}
```

### Comparing `janus_swi-1.2.1/janus_swi.egg-info/PKG-INFO` & `janus_swi-1.3.0/janus_swi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus_swi
-Version: 1.2.1
+Version: 1.3.0
 Summary: Janus library to call SWI-Prolog
 Home-page: https://github.com/SWI-Prolog/packages-swipy
 Author: Jan Wielemaker
 Author-email: Jan Wielemaker <jan@swi-prolog.org>
 License: BSD-2-Clause
 Project-URL: Homepage, https://www.swi-prolog.org
 Project-URL: Documentation, https://www.swi-prolog.org/pldoc/package/janus
```

### Comparing `janus_swi-1.2.1/janus_swi.egg-info/SOURCES.txt` & `janus_swi-1.3.0/janus_swi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/pyproject.toml` & `janus_swi-1.3.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/scripts/newversion` & `janus_swi-1.3.0/scripts/newversion`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/setup.py` & `janus_swi-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     link_args.append(f'-Wl,-rpath={props["PLLIBDIR"]},--enable-new-dtags')
 elif ( sys.platform == 'darwin' ):
     link_args.append(f'-Wl,-rpath,{props["PLLIBDIR"]}')
 elif ( sys.platform == 'win32' ):
     PLLIB="libswipl"
 
 setup(name='janus_swi',
-      version='1.2.1',
+      version='1.3.0',
       description="Janus library to call SWI-Prolog",
       author="Jan Wielemaker",
       author_email="jan@swi-prolog.org",
       url="https://github.com/SWI-Prolog/packages-swipy",
       license="BSD-2",
       packages=['janus_swi'],
       package_dir={"janus_swi":"janus"},
```

### Comparing `janus_swi-1.2.1/test_janus.pl` & `janus_swi-1.3.0/test_janus.pl`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,16 @@
                 janus_reflect,
                 janus_gc,
 		python_call_prolog,
 		janus_iter,
 		janus_errors,
 		janus_unicode,
                 janus_load,
-		xsb_call
+		xsb_call,
+                demo
               ]).
 
 :- py_add_lib_dir(tests).
 
 :- begin_tests(janus_data).
 
 test(noarg, Z == 42) :-
@@ -343,17 +344,25 @@
     sort('Y', @=<, List0, List),
     py_call(janus:undefined, Undef).
 test(py_double, Tuples == [1-1,2-1,3-1,
                            1-2,2-2,3-2,
                            1-3,2-3,3-3,
                            1-4,2-4,3-4]) :-
     py_call(demo:double_iter(3,4), Tuples).
-test(invalid_nesting, X == @true) :-
+test(invalid_nesting, X == @false) :-
     py_call(demo:test_invalid_nesting(), X).
 :- if((py_call(sys:hexversion, V), V >= 0x03080000)).
+test(invalid_nesting2, [BlobType, BlobStr] ==
+                       ['PyObject',               % PrologError is tested for in demo.py
+                        "swipl.next_solution(): not inner query"]) :-
+    py_call(demo:test_invalid_nesting2(), Blob),
+    janus:py_str(Blob, BlobStr), % TODO: re-export py_str from module janus?
+    blob(Blob, BlobType).
+test(invalid_nesting3, error(python_error('PrologError',_))) :-
+    py_call(demo:test_invalid_nesting3(), _).
 test(while, X == [1,2,3]) :-
     py_call(while:test_while(), X).
 :- endif.
 test(apply, X == 3) :-
     py_call(janus:apply_once(user, plus, 1, 2), X).
 test(apply, X == 1) :-
     py_call(janus:apply_once(user, between, 1, 2), X).
@@ -457,14 +466,53 @@
 test(cmd, error(python_error('PrologError', _))) :-
     py_call(janus:cmd(test_janus, no_such_pred), _).
 
 test_janus:p(42).
 
 :- end_tests(xsb_call).
 
+:- begin_tests(demo).
+
+test(doc_sqrt, R == py{'truth': @(true), 'Y': 1.4142135623730951}) :-
+    py_call(demo:doc_sqrt(), R).
+
+test(doc_user_plus, R == 3) :-
+    py_call(demo:doc_user_plus(), R).
+
+test(doc_findall_parent, [blocked('need to define parent/2 predicate'), R == [ 'Kees', 'Jan' ]]) :-
+    py_call(demo:doc_findall_parent(), R).
+
+test(doc_has_big_integers, R == @(TrueFalse)) :-
+    py_call(demo:doc_has_big_integers(), R),
+    (   current_prolog_flag(bounded,false)
+    ->  TrueFalse = true
+    ;   TrueFalse = false
+    ).
+
+test(doc_getRange, R == [3,4,5]) :-
+    py_call(demo:doc_getRange(3,5), R).
+test(doc_getRange, R == [3,4,5]) :-
+    py_call(demo:doc_getRange2(3,5), R).
+
+test(doc_double_iter, R == [1-1, 2-1, 1-2, 2-2, 1-3, 2-3]) :-
+    py_call(demo:doc_double_iter(2,3), R).
+test(doc_double_iter, R == [1-1, 2-1, 1-2, 2-2, 1-3, 2-3]) :-
+    py_call(demo:doc_double_iter2(2,3), R).
+
+test(doc_get_between, R == [1,2,3]) :-
+    py_call(demo:doc_get_between(), R).
+
+test(doc_apply_between, R == [1, 2, 3, 4, 5, 6]) :-
+    py_call(demo:doc_apply_between(), R).
+
+test(doc_between_1_6, R == [1, 2, 3, 4, 5, 6]) :-
+    py_call(demo:doc_between_1_6(), R).
+
+:- end_tests(demo).
+
 bench_janus :-
     bench_python(concat_list(100 000)).
 
 bench_python(concat_list(N)) :-
     numlist(1, N, List),
     time(py_call(demo:concat(List, List), Concat)),
     length(Concat, N2),
```

### Comparing `janus_swi-1.2.1/test_xsb_janus.pl` & `janus_swi-1.3.0/test_xsb_janus.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/tests/bench.pl` & `janus_swi-1.3.0/tests/bench.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/tests/threads.py` & `janus_swi-1.3.0/tests/threads.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import janus_swi as janus
 import threading
 
 def one():
     print("Starting one")
     plone()
 
-def plone():    
+def plone():
     x = janus.query_once("""
     thread_self(_Me),
     thread_property(_Me, id(Me)),
     writeln(start(Me)),
     forall(between(1,20,_X),
            (between(1, 1 000 000, _), writeln(_X)))
     """)
```

### Comparing `janus_swi-1.2.1/xsb_tests/Person.py` & `janus_swi-1.3.0/xsb_tests/Person.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/jintf.py` & `janus_swi-1.3.0/xsb_tests/jintf.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/kwargs.py` & `janus_swi-1.3.0/xsb_tests/kwargs.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/numpexamp.py` & `janus_swi-1.3.0/xsb_tests/numpexamp.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/returnVal.py` & `janus_swi-1.3.0/xsb_tests/returnVal.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/sample.json` & `janus_swi-1.3.0/xsb_tests/sample.json`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/stressTest.py` & `janus_swi-1.3.0/xsb_tests/stressTest.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/sumlist3.py` & `janus_swi-1.3.0/xsb_tests/sumlist3.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/test_err.py` & `janus_swi-1.3.0/xsb_tests/test_err.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/test_stress.pl` & `janus_swi-1.3.0/xsb_tests/test_stress.pl`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/testc.py` & `janus_swi-1.3.0/xsb_tests/testc.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/tupInList.py` & `janus_swi-1.3.0/xsb_tests/tupInList.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/tupletest.py` & `janus_swi-1.3.0/xsb_tests/tupletest.py`

 * *Files identical despite different names*

### Comparing `janus_swi-1.2.1/xsb_tests/variadic.py` & `janus_swi-1.3.0/xsb_tests/variadic.py`

 * *Files identical despite different names*

