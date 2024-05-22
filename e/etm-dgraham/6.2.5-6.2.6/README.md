# Comparing `tmp/etm-dgraham-6.2.5.tar.gz` & `tmp/etm-dgraham-6.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "etm-dgraham-6.2.5.tar", last modified: Sat May 18 17:38:14 2024, max compression
+gzip compressed data, was "etm-dgraham-6.2.6.tar", last modified: Wed May 22 19:11:35 2024, max compression
```

## Comparing `etm-dgraham-6.2.5.tar` & `etm-dgraham-6.2.6.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.946382 etm-dgraham-6.2.5/
--rw-r--r--   0 dag        (501) staff       (20)     5532 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/CHANGES.txt
--rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/MANIFEST.in
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-18 17:38:14.946169 etm-dgraham-6.2.5/PKG-INFO
--rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.5/README.md
--rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.5/_config.yml
--rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/bump.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.939442 etm-dgraham-6.2.5/docs/
--rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/index_konnections.md
--rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/index_usedtime.md
--rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/docs/multiple_timers.md
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.942321 etm-dgraham-6.2.5/etm/
--rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/etm/__init__.py
--rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.5/etm/__main__.py
--rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/__version__.py
--rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-18 16:18:38.000000 etm-dgraham-6.2.5/etm/common.py
--rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/etm/data.py
--rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.5/etm/make_examples.py
--rwxr-xr-x   0 dag        (501) staff       (20)   330183 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/model.py
--rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.5/etm/options.py
--rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.5/etm/report.py
--rwxr-xr-x   0 dag        (501) staff       (20)   126487 2024-05-18 17:38:09.000000 etm-dgraham-6.2.5/etm/view.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.944588 etm-dgraham-6.2.5/etm_dgraham.egg-info/
--rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO
--rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO [conflicted]
--rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/dependency_links.txt
--rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/entry_points.txt
--rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/requires [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/requires.txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/top_level [conflicted].txt
--rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-18 17:38:14.000000 etm-dgraham-6.2.5/etm_dgraham.egg-info/top_level.txt
--rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.5/etmlogo.png
--rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/etmlogo_small.png
--rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.5/etmview_agenda.png
--rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/namedcolors.py
--rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.5/new.png
--rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.5/requirements.txt
--rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-18 17:38:14.946418 etm-dgraham-6.2.5/setup.cfg
--rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.5/setup.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.944725 etm-dgraham-6.2.5/test/
--rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.5/test/test_parser.py
-drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-18 17:38:14.945647 etm-dgraham-6.2.5/utilities/
--rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.5/utilities/colons_to_slashes.py
--rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.5/utilities/etm_in
--rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.5/utilities/inbasket
--rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.5/utilities/open_in_mutt
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.363712 etm-dgraham-6.2.6/
+-rw-r--r--   0 dag        (501) staff       (20)     5306 2024-05-22 19:11:28.000000 etm-dgraham-6.2.6/CHANGES.txt
+-rw-rw-rw-   0 dag        (501) staff       (20)       37 2020-06-03 13:02:08.000000 etm-dgraham-6.2.6/MANIFEST.in
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-22 19:11:35.363421 etm-dgraham-6.2.6/PKG-INFO
+-rw-r--r--   0 dag        (501) staff       (20)   144578 2024-05-07 12:58:43.000000 etm-dgraham-6.2.6/README.md
+-rw-r--r--   0 dag        (501) staff       (20)       25 2023-04-24 16:44:33.000000 etm-dgraham-6.2.6/_config.yml
+-rwxr-xr-x   0 dag        (501) staff       (20)     4516 2024-04-24 18:26:45.000000 etm-dgraham-6.2.6/bump.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.355513 etm-dgraham-6.2.6/docs/
+-rwxr-xr-x   0 dag        (501) staff       (20)     7571 2021-12-29 14:26:10.000000 etm-dgraham-6.2.6/docs/index_konnections.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     8246 2021-12-29 14:26:10.000000 etm-dgraham-6.2.6/docs/index_usedtime.md
+-rwxr-xr-x   0 dag        (501) staff       (20)     4732 2021-12-29 14:26:10.000000 etm-dgraham-6.2.6/docs/multiple_timers.md
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.359375 etm-dgraham-6.2.6/etm/
+-rwxr-xr-x   0 dag        (501) staff       (20)        0 2021-12-29 14:26:10.000000 etm-dgraham-6.2.6/etm/__init__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    15262 2024-05-04 14:12:33.000000 etm-dgraham-6.2.6/etm/__main__.py
+-rwxr-xr-x   0 dag        (501) staff       (20)       17 2024-05-22 19:11:28.000000 etm-dgraham-6.2.6/etm/__version__.py
+-rw-r--r--   0 dag        (501) staff       (20)    26965 2024-05-18 16:18:38.000000 etm-dgraham-6.2.6/etm/common.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    29368 2024-04-24 18:26:45.000000 etm-dgraham-6.2.6/etm/data.py
+-rwxr-xr-x   0 dag        (501) staff       (20)     9528 2024-04-24 18:26:45.000000 etm-dgraham-6.2.6/etm/make_examples.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   326594 2024-05-22 19:11:28.000000 etm-dgraham-6.2.6/etm/model.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    38924 2024-05-06 14:19:59.000000 etm-dgraham-6.2.6/etm/options.py
+-rwxr-xr-x   0 dag        (501) staff       (20)    27887 2024-05-04 14:12:33.000000 etm-dgraham-6.2.6/etm/report.py
+-rwxr-xr-x   0 dag        (501) staff       (20)   126420 2024-05-22 19:11:28.000000 etm-dgraham-6.2.6/etm/view.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.361556 etm-dgraham-6.2.6/etm_dgraham.egg-info/
+-rw-r--r--   0 dag        (501) staff       (20)   146147 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/PKG-INFO
+-rwxrwxrwx   0 dag        (501) staff       (20)   102652 2020-06-03 14:25:34.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/PKG-INFO [conflicted]
+-rwxrwxrwx   0 dag        (501) staff       (20)      504 2020-06-03 14:25:34.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/SOURCES [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      882 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/SOURCES.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        1 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/dependency_links.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)       71 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/entry_points.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      316 2020-06-03 14:25:34.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/requires [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)      300 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/requires.txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2020-06-03 14:25:34.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/top_level [conflicted].txt
+-rwxrwxrwx   0 dag        (501) staff       (20)        4 2024-05-22 19:11:35.000000 etm-dgraham-6.2.6/etm_dgraham.egg-info/top_level.txt
+-rw-r--r--   0 dag        (501) staff       (20)    28934 2023-04-27 18:21:07.000000 etm-dgraham-6.2.6/etmlogo.png
+-rw-rw-rw-   0 dag        (501) staff       (20)     7047 2020-06-03 13:02:08.000000 etm-dgraham-6.2.6/etmlogo_small.png
+-rw-rw-rw-   0 dag        (501) staff       (20)    36594 2020-07-27 15:42:26.000000 etm-dgraham-6.2.6/etmview_agenda.png
+-rwxrwxrwx   0 dag        (501) staff       (20)     1005 2020-06-03 13:02:08.000000 etm-dgraham-6.2.6/namedcolors.py
+-rw-r--r--   0 dag        (501) staff       (20)   448972 2024-05-06 20:30:20.000000 etm-dgraham-6.2.6/new.png
+-rw-rw-rw-   0 dag        (501) staff       (20)      326 2020-06-03 13:02:08.000000 etm-dgraham-6.2.6/requirements.txt
+-rw-r--r--   0 dag        (501) staff       (20)       38 2024-05-22 19:11:35.363760 etm-dgraham-6.2.6/setup.cfg
+-rwxr-xr-x   0 dag        (501) staff       (20)     4952 2024-01-10 16:01:12.000000 etm-dgraham-6.2.6/setup.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.361703 etm-dgraham-6.2.6/test/
+-rw-r--r--   0 dag        (501) staff       (20)     1155 2022-03-22 15:05:47.000000 etm-dgraham-6.2.6/test/test_parser.py
+drwxr-xr-x   0 dag        (501) staff       (20)        0 2024-05-22 19:11:35.362904 etm-dgraham-6.2.6/utilities/
+-rwxr-xr-x   0 dag        (501) staff       (20)     1078 2021-12-29 14:26:10.000000 etm-dgraham-6.2.6/utilities/colons_to_slashes.py
+-rwxrwxrwx   0 dag        (501) staff       (20)     2089 2024-04-28 16:49:51.000000 etm-dgraham-6.2.6/utilities/etm_in
+-rwxrwxrwx   0 dag        (501) staff       (20)     4834 2020-10-30 02:00:48.000000 etm-dgraham-6.2.6/utilities/inbasket
+-rwxrwxrwx   0 dag        (501) staff       (20)      643 2020-10-20 14:57:04.000000 etm-dgraham-6.2.6/utilities/open_in_mutt
```

### Comparing `etm-dgraham-6.2.5/CHANGES.txt` & `etm-dgraham-6.2.6/CHANGES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,28 @@
-2024-05-18 6376025 Daniel Graham
+2024-05-22 ef18e3f Daniel Graham
+    Tagged version 6.2.6.
+
+2024-05-22 3c75e39 Daniel Graham
+    Removed more logging.debug statements
+
+2024-05-22 3ed355b Daniel Graham
+    Finishing repeating tasks now seems correct. Cleaned up
+    logging.debug statements.
+
+2024-05-22 fa11ab4 Daniel Graham
+    Next pass at finishing repeated tasks correctly
+
+2024-05-19 94b7683 Daniel Graham
+    Fixed bug in completing repeating task when @s doesn't fit the
+    recurrence rule
+
+2024-05-19 b8e0c42 Daniel Graham
+    @s inclusion fix for past due repeating tasks
+
+2024-05-18 34730e7 Daniel Graham
     Tagged version 6.2.5.
 
 2024-05-18 b2713d0 Daniel Graham
     Fixed bug in which pressing 'E' without an item selected, would
     open the last item
 
 2024-05-18 4b525cd Daniel Graham
@@ -173,30 +193,7 @@
     Tagged version 6.1.24.
 
 2024-04-24 10b8c3a Daniel Graham
     Fixed import bug
 
 2024-04-24 e7af668 Daniel Graham
     Tagged version 6.1.23.
-
-2024-04-24 b421570 Daniel Graham
-    Avoid unnecessary import of view in bump.py
-
-2024-04-24 25a596e Daniel Graham
-    Added 'doghouse' example of task with jobs to lorem examples.
-
-2024-04-24 24e900c Daniel Graham
-    More work on common.py. Added # pyright:
-    reportUndefinedVariable=false to suppress pyright warnings. Fixed
-    jobs format start/extend and summary format. Updated discussion of
-    tasks and jobs in README.
-
-2024-04-21 3d71359 Daniel Graham
-    Expanded imports from common to fix pylance problem reports. First
-    pass at making tasks with @s and @e entries due at @s + @e and
-    only past due after that.
-
-2024-03-19 0f628dc Daniel Graham
-    setup_logging __main__ -> common
-
-2024-03-18 2285c8f Daniel Graham
-    ETMQuery class view.py -> data.py
```

### Comparing `etm-dgraham-6.2.5/PKG-INFO` & `etm-dgraham-6.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.5
+Version: 6.2.6
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.2.5/README.md` & `etm-dgraham-6.2.6/README.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/bump.py` & `etm-dgraham-6.2.6/bump.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/docs/index_konnections.md` & `etm-dgraham-6.2.6/docs/index_konnections.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/docs/index_usedtime.md` & `etm-dgraham-6.2.6/docs/index_usedtime.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/docs/multiple_timers.md` & `etm-dgraham-6.2.6/docs/multiple_timers.md`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/__main__.py` & `etm-dgraham-6.2.6/etm/__main__.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/common.py` & `etm-dgraham-6.2.6/etm/common.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/data.py` & `etm-dgraham-6.2.6/etm/data.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/make_examples.py` & `etm-dgraham-6.2.6/etm/make_examples.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/model.py` & `etm-dgraham-6.2.6/etm/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # pyright: reportUndefinedVariable=false
 #  standard sort order for usable ASCII characters
 # usable = ['!', '"', '#', '$', '%', '&', "'", '(', ')', '*', '+', ',', '-', '.', '/', '0', '1', '2', '3', '4', '5', '6', '7', '8', '9', ':', ';', '<', '=', '>', '?', '@', 'A', 'B', 'C', 'D', 'E', 'F', 'G', 'H', 'I', 'J', 'K', 'L', 'M', 'N', 'O', 'P', 'Q', 'R', 'S', 'T', 'U', 'V', 'W', 'X', 'Y', 'Z', '[', '\\', ']', '^', '_', '`', 'a', 'b', 'c', 'd', 'e', 'f', 'g', 'h', 'i', 'j', 'k', 'l', 'm', 'n', 'o', 'p', 'q', 'r', 's', 't', 'u', 'v', 'w', 'x', 'y', 'z', '{', '|', '}', '~']
 # len(usable): 94
 
-from typing import Union
+from typing import Union, Tuple, Optional
+
 from etm.common import ( 
     VERSION_INFO,
     parse,
     WKDAYS_DECODE,
     WKDAYS_ENCODE,
     # ETM_CHAR,
     EtmChar,
@@ -828,30 +829,28 @@
             self.dbitem = DBITEM
             self.dbquery = DBITEM
 
         else:
             if not os.path.exists(dbfile):
                 logger.error(f'{dbfile} does not exist')
                 return
-            logger.debug(f"dbfile is {dbfile}, initializing tinydb")
             self.db = data.initialize_tinydb(dbfile)
             self.dbarch = self.db.table('archive', cache_size=30)
             self.dbquery = self.db.table('items', cache_size=0)
 
     def use_archive(self):
         self.query_mode = 'archive table'
         self.db = DBARCH
 
     def use_items(self):
         self.query_mode = 'items table'
         self.db = DBITEM
 
     def check_goto_link(self, num=5):
         """ """
-        logger.debug("calling update_item_hsh from check_goto_link")
         self.update_item_hsh()
         if goto := self.item_hsh.get('g'):
             return True, goto
         else:
             return False, 'does not have an @g goto entry'
 
     def get_repetitions(self):
@@ -869,18 +868,19 @@
         if 's' not in item and ('r' not in item or '+' not in item):
             return showing, 'not a repeating item'
         relevant = date_to_datetime(item['s'])
         at_plus = item.get('+', [])
         if at_plus:
             at_plus.sort()
             relevant = min(relevant, date_to_datetime(at_plus[0]))
-        logger.debug(f'relevant: {relevant}')
 
-        instances = item_instances(item, relevant, num + 1, False)
+        # instances = item_instances(item, relevant, num + 1, False)
+        instances = item_instances(item, None, num + 1, False)
         instances.sort()
+        relevant = instances[0][0]
         pairs = [format_datetime(x[0])[1] for x in instances]
         starting = format_datetime(relevant.date())[1]
         if len(pairs) > num:
             showing = f'Next {num} repetitions'
             pairs = pairs[:num]
         elif pairs:
             showing = 'All repetitions'
@@ -889,15 +889,15 @@
         return showing, f'from {starting}:\n  ' + '\n  '.join(pairs)
 
     def do_update(self):
         try:
             self.db.remove(doc_ids=[self.doc_id])
             self.db.insert(Document(self.item_hsh, doc_id=self.doc_id))
         except Exception as e:
-            logger.debug(f"exception: {e}")
+            logger.warning(f"exception: {e}")
         return True
 
     def do_insert(self):
         timer_insert = TimeIt('***INSERT***')
         if 'created' not in self.item_hsh:
             self.item_hsh['created'] = datetime.now().astimezone()
         doc_id = self.db.insert(self.item_hsh)
@@ -1145,27 +1145,22 @@
         self.doc_id = item_id
         # self.created = self.item_hsh['created']
         q = self.item_hsh.get('q', [])
         if not len(q) > 0:
             return False
         quota = q[0]
         now = datetime.now().astimezone()
-        logger.debug(f"{now = }") 
         this_week = tuple([int(x) for x in now.strftime("%Y,%W").split(',')])
-        logger.debug(f"{this_week = }")
         self.item_hsh.setdefault('h', {})
         hist = self.item_hsh.get('h', {})
-        logger.debug(f"{hist = }")
         this_week_str = f"{this_week[0]}:{this_week[1]:02}"
         done = hist.get(this_week_str, 0)
         hist[this_week_str] = done + 1
-        logger.debug(f"{done = }; {quota = }; {hist = }")
         self.item_hsh['h'] = hist
         self.item_hsh['modified'] = now
-        logger.debug(f"{self.item_hsh = }")
         self.do_update()
         return True
 
     def toggle_goal_active(
             self,
             item_id: int,
             ) -> bool:
@@ -1178,15 +1173,14 @@
         q = self.item_hsh.get('q', [])
         if not len(q) > 0 or q[0] == 0:
             return False
         q[0] = -q[0]
         self.item_hsh['q'] = q 
         now = datetime.now().astimezone()
         self.item_hsh['modified'] = now
-        logger.debug(f"{self.item_hsh = }")
         self.do_update()
         return True
 
     def end_goal(
             self,
             item_id: int,
             ) -> bool:
@@ -1199,15 +1193,14 @@
         q = self.item_hsh.get('q', [])
         if not len(q) > 0 or q[0] == 0:
             return False
         q[0] = 0
         self.item_hsh['q'] = q 
         now = datetime.now().astimezone()
         self.item_hsh['modified'] = now
-        logger.debug(f"{self.item_hsh = }")
         self.do_update()
         return True
 
     def finish_item(
         self,
         item_id: int,
         job_id: any,
@@ -1292,14 +1285,15 @@
             if '+' in self.item_hsh and due_datetime in self.item_hsh['+']:
                 self.item_hsh['+'].remove(due_datetime)
                 if not self.item_hsh['+']:
                     del self.item_hsh['+']
                 self.item_hsh.setdefault('h', []).append(completion_entry)
                 save_item = True
             elif 'r' in self.item_hsh:
+                self.item_hsh.setdefault('-', []).append(due_datetime)
                 from_rrule = self.item_hsh.get('o', 'k') == 's'
                 nxt = get_next_due(
                     self.item_hsh, completed_datetime, completion_entry.end, from_rrule
                 )
                 if nxt:
                     for i in range(len(self.item_hsh['r'])):
                         if (
@@ -1343,15 +1337,14 @@
                 if ok:
                     sh = self.item_hsh['h']
                     sh.sort(key=sortprd)
                     self.item_hsh['h'] = sh[-num_finished:]
 
             self.item_hsh['created'] = self.created
             self.item_hsh['modified'] = datetime.now().astimezone()
-            # self.db.update(db_replace(self.item_hsh), doc_ids=[self.doc_id])
             self.do_update()
             return True
         return False
 
     def record_timer(
         self, item_id, job_id=None, completed_datetime=None, elapsed_time=None
     ):
@@ -1388,20 +1381,17 @@
         # ((17, 24), ('e', '90m'))
         self.interval, self.active = active_from_pos(self.pos_hsh, pos)
 
 
     def text_changed(self, s, pos, modified=True):
         """ """
         # self.is_modified = modified
-        # logger.debug(f"\n### starting text_changed with s: {s} and self.keyvals: {self.keyvals}")
         self.entry = s
         self.pos_hsh, keyvals = process_entry(s, self.settings)
         removed, changed = listdiff(self.keyvals, keyvals)
-        # logger.debug(f"{self.pos_hsh = };\n{keyvals = }\n{removed = };\n{changed = }")
-        # if removed + changed != []:
         if self.init_entry != self.entry:
             self.is_modified = True
         # only process changes for kv entries
         update_timezone = False
         for kv in removed + changed:
             if kv[0] == 'z':
                 update_timezone = True
@@ -1417,62 +1407,49 @@
             if kv in self.askreply:
                 del self.askreply[kv]
             if kv in keyvals:
                 keyvals.remove(kv)
         self.keyvals = []
         # for kv in [x for x in changed if x not in removed]:
         for kv in [x for x in keyvals if x not in removed]:
-            # logger.debug(f"updating kv: {kv}")
             self.update_keyval(kv)
             self.keyvals.append(kv)
-        # logger.debug(f"### leaving text_changed with self.keyvals: {self.keyvals}\n")
 
     def update_keyval(self, kv):
         """
         TODO: add return status
         """
         key, val = kv
-        # logger.debug(f"starting update_keyval with self.keyvals: {self.keyvals}")
 
         condition = 'f' in key
 
-        # logger.debug(f"checking kv: {kv}")
         if key in self.keys:
-            # logger.debug(f"found kv: {kv}")
             a, r, do = self.keys[key]
             ask = a
             msg = self.check_allowed(key)
-            # logger.debug(f"got {msg = } when checking {kv = } allowed")
             if msg:
                 obj = None
                 ask = 'error'
                 reply = msg
                 self.object_hsh[kv] = None
             else:   # only do this for allowed keys
                 msg = self.check_requires(key)
-                # logger.debug(f"got msg: {msg} checking required for {key}")
                 if msg:
-                    # logger.debug(f"failed required, self: {self}")
                     obj = None
                     reply = msg
                 else:
                     # call the appropriate do for the key
                     obj, rep = do(val)
                     reply = rep if rep else r
-                    # logger.debug(f"got obj: {obj}, rep: {rep} from {val}")
                     if obj is not None:
                         self.object_hsh[kv] = obj
-                        # logger.debug(f"added {kv[0]}: {obj} to obj_hsh: {self.object_hsh}")
-                        # self.item_hsh[kv[0]] = obj
                     else:
                         if kv in self.object_hsh:
                             del self.object_hsh[kv]
-            # logger.debug(f"{kv = }; {ask = }; {reply = }")
             self.askreply[kv] = (ask, reply)
-            # logger.debug(f"{self.askreply = }")
         else:
             display_key = f'@{key}' if len(key) == 1 else f'&{key[-1]}'
             self.askreply[kv] = (
                 'unrecognized key',
                 f'{display_key} is invalid',
             )
 
@@ -1482,15 +1459,14 @@
         self.item_hsh = {'created': created}
         cur_hsh = {}
         cur_key = None
         msg = []
         for pos, (k, v) in self.pos_hsh.items():
             obj = self.object_hsh.get((k, v))
             if obj is None:
-                # logger.debug(f"{self.askreply.get((k,v), '')}")
                 msg.append(f'bad entry for {k}: {v}\n{self.askreply.get((k,v), ["", ""])[-1]}')
                 return msg
                 # continue
             elif k in ['a', 'u', 'n', 't', 'k', 'K']:
                 self.item_hsh.setdefault(k, []).append(obj)
             elif k in ['rr', 'jj']:
                 if cur_hsh:
@@ -1576,19 +1552,17 @@
                 self.do_update()
 
     def check_requires(self, key):
         """
         Check that key has the prerequisite entries.
         if key in requires, check that each key in requires[k] has a corresponding key, val in keyvals: [(k, v), (k, v), ...]
         """
-        # logger.debug(f"self.keyvals: {self.keyvals}")
         missing = []
         if key in requires:
             cur_keys = [k for (k, v) in self.keyvals]
-            # logger.debug(f"checking cur_keys {cur_keys} for required key {key}")
             missing = [f'@{k[0]}' for k in requires[key] if k not in cur_keys]
 
         if missing:
             display_key = (
                 f'@{key[0]}'
                 if len(key) == 1 or key in ['rr', 'jj']
                 else f'&{key[-1]}'
@@ -1621,20 +1595,18 @@
 
 
             numuses = {}
             duplicates = []
             for k, v in self.keyvals:
                 numuses.setdefault(k, 0)
                 numuses[k] += 1
-            # logger.debug(f"{numuses = }")
             duplicates = [
                 k for (k, v) in numuses.items() if v > 0 and k not in [
                     'a', 'u', 't', 'k', 'K', 'jj', 'rr', 'ji', 'js', 'jb', 'jp', 'ja', 'jd', 'je', 'jf', 'jl', 'jm', 'ju']
                 ]
-            # logger.debug(f"{key = }; {duplicates = }")
 
             if key in duplicates:
                 display_key = f'@{key}' if len(key) == 1 else f'&{key[-1]}'
                 return f'{display_key} has already been entered'
             else:
                 return ''
         else:
@@ -1810,15 +1782,14 @@
         obj = None
         m = quota_regex.match(arg)
         if m:
             obj = [int(x) for x in arg.split(',') if x.strip()]
             weeks = f"for {obj[1]} weeks" if len(obj) > 1 else "indefinitely" 
             rep = f'{obj[0]} times/week {weeks}'
             self.item_hsh['q'] = obj                
-            # logger.debug(f"{self.item_hsh = }")
         else:
             rep = "goal: instances per week optionally followed by a comma and the number of weeks"
         return obj, rep
         
 
     def do_datetime(self, arg):
         """
@@ -3172,15 +3143,15 @@
             if ' | ' not in x:
                 continue
             parts = x.split(' | ')
             if len(parts) == 2:
                 k, v = parts
                 self.kompletions[k.strip()[3:]] = f"@k {v.strip()}"
             else:
-                logger.debug(f"bad parts: {parts}")
+                logger.warning(f"bad parts: {parts}")
 
 
     def show_occurrences(self):
         width = shutil.get_terminal_size()[0]
         tmp = []
         newline = False
         for k in self.completion_keys:
@@ -3410,19 +3381,17 @@
             n- -> r-   n- -> p-
             n+ -> i+   n+ -> i+
             i- -> r-   i- -> r-
             i+ -> r-   i+ -> r-
             r- -> p-   r- -> p-
             p- -> r-   p- -> r-
         """
-        logger.debug("next_timer_state")
         if not doc_id:
             return
         other_timers = deepcopy(self.timers)
-        logger.debug(f"{other_timers = }")
         if doc_id in other_timers:
             del other_timers[doc_id]
         active = [x for x, v in other_timers.items() if v[0] in ['r', 'p']]
         if len(active) > 1:
             logger.warning(f'more than one active timer: {active}')
         now = datetime.now().astimezone()
         if doc_id in self.timers:
@@ -4066,15 +4035,14 @@
         item_id = res[0]
         item = self.db.get(doc_id=item_id)
         if 'doc_id' in item:
             return item['doc_id']
 
     def get_details(self, row=None, edit=False):
         res = self.get_row_details(row)
-        logger.debug(f"{res = }")
         if not (res and res[0]):
             return None, ''
         
         item_id = res[0]
 
         if not edit and item_id in self.itemcache:
             return item_id, self.itemcache[item_id]
@@ -4083,24 +4051,22 @@
             item_hsh = item_details(item, edit)
             return item_id, item_hsh
         return None, ''
 
     def toggle_pinned(self, row=None):
         res = self.get_row_details(row)
         if not (res and res[0]):
-            logger.debug(f'toggle_pinned no details for {row}')
             return None, ''
         item_id = res[0]
         if item_id in self.pinned_list:
             self.pinned_list.remove(item_id)
             act = 'unpinned'
         else:
             self.pinned_list.append(item_id)
             act = 'pinned'
-        logger.debug(f'pinned_list: {self.pinned_list}')
         return f'{act} {item_id}'
 
     def get_pinned(self):
         return [self.db.get(doc_id=x) for x in self.pinned_list if x]
 
     def get_goto(self, row=None):
         res = self.get_row_details(row)
@@ -4126,15 +4092,14 @@
         res = self.get_row_details(row)
         if not res:
             return None, ''
         item_id = res[0]
         instance = res[1]
 
         if not (item_id and item_id in self.id2relevant):
-            logger.debug(f'{item_id} not in id2relevant')
             return ''
         showing = 'Repetitions'
         item = DBITEM.get(doc_id=item_id)
         details = f"{item['itemtype']} {item['summary']}"
 
         if not ('s' in item and ('r' in item or '+' in item)):
             return showing, 'not a repeating item'
@@ -4682,15 +4647,14 @@
         message = smtp_body.format(
             start=start,
             when=when,
             summary=summary,
             location=location,
             description=description,
         )
-        logger.debug(f"message: {message}")
         # All the necessary ingredients are in place
         import smtplib
         from email.mime.multipart import MIMEMultipart
         from email.mime.text import MIMEText
         from email.utils import COMMASPACE, formatdate
 
         assert type(email_addresses) == list
@@ -5743,15 +5707,15 @@
             if x in WKDAYS_DECODE:
                 good.append(eval('dr.{}'.format(WKDAYS_DECODE[x])))
                 rep.append(x)
             elif x in WKDAYS_ENCODE:
                 try:
                     good.append(eval(x))
                 except Exception as e:
-                    logger.debug(f"exception: {e} when evaluating '{x}'")
+                    logger.warning(f"exception: {e} when evaluating '{x}'")
 
                 rep.append(WKDAYS_ENCODE[x].lstrip('+'))
             else:
                 bad.append(x)
         if bad:
             obj = None
             rep = f"incomplete or invalid weekdays: {', '.join(bad)}. {weekdaysstr}"
@@ -6036,37 +6000,34 @@
         logger.warning(
             f"Warning: using both 'c' and 'u' is depreciated in {r_hsh}"
         )
     freq = rrule_freq[r_hsh['r']]
     kwd = {rrule_name[k]: r_hsh[k] for k in r_hsh if k != 'r'}
     return freq, kwd
 
-
 def get_next_due(item, done, due, from_rrule=False):
     """
     return the next due datetime for an @r and @+ / @- repetition
     """
+    def f(dt: datetime)->str:
+        return(dt.astimezone().strftime("%Y-%m-%d %H:%M:%S"))
+
+    instances = [f(x[0]) for x in item_instances(item, item['s'], 2, False)]
     lofh = item.get('r')
     if not lofh:
         return ''
     rset = dr.rruleset()
     overdue = item.get('o', 'k')   # make 'k' the default for 'o'
     start = item['s']
     dtstart = date_to_datetime(item['s'])
-    if due > dtstart:
-        # we've finished a between instance
-        return dtstart
-    # we're finishing the oldest instance
-    h = [x.end for x in item.get('h', [])]
-    h.sort()
 
     due = dtstart if not due else due
 
     if overdue == 'k':
-        aft = due
+        aft = dtstart
         inc = False
     elif overdue == 'r':
         aft = done
         dtstart = done
         inc = False
     else:  # 's' skip
         today = date_to_datetime(date.today())
@@ -6097,17 +6058,23 @@
     plus_not_minus = list(set(plus) - set(minus_hist))
     minus_not_plus = list(set(minus_hist) - set(plus))
     if from_rrule:
         for dt in minus_not_plus:
             rset.exdate(date_to_datetime(dt))
         nxt = rset.after(date_to_datetime(aft), inc)
     else:
-        for dt in plus_not_minus:
-            rset.rdate(date_to_datetime(dt))
+        logger.debug(f"before {f(aft) = }")
+
+        if plus_not_minus:
+            plus_not_minus.sort()
+            aft = min(aft, plus_not_minus[0])
+            for dt in plus_not_minus:
+                rset.rdate(date_to_datetime(dt))
         nxt = rset.after(date_to_datetime(aft), inc)
+        after = rset.after(date_to_datetime(dtstart), False)
     if nxt:
         if using_dates:
             nxt = nxt.date()
     else:
         nxt = None
     return nxt
 
@@ -6122,16 +6089,15 @@
             minute=minute,
             second=0,
             microsecond=0,
         ).astimezone()
         dt = new_dt
     return dt
 
-
-def item_instances(item, aft_dt, bef_dt=1, honor_skip=True):
+def item_instances(item, aft_dt, bef_dt=1, honor_skip=True)-> Tuple[Optional[datetime], Optional[datetime]]:
     """
     Dates and datetimes decoded from the data store will all be aware and in the local timezone. aft_dt and bef_dt must therefore also be aware and in the local timezone.
     In dateutil, the starting datetime (dtstart) is not the first recurrence instance, unless it does fit in the specified rules.  Notice that you can easily get the original behavior by using a rruleset and adding the dtstart as an rdate recurrence.
     Each instance is a tuple (beginning datetime, ending datetime) where ending datetime is None unless the item is an event.
 
     Get instances from item falling on or after aft_dt and on or before bef_dt or, if bef_dt is an integer, n, get the first n instances after aft_dt. All datetimes will be returned with zero offsets.
     >>> item_eg = { "s": parse('2018-03-07 8am', tz="US/Eastern"), "e": timedelta(days=1, hours=5), "r": [ { "r": "w", "i": 2, "u": parse('2018-04-01 8am', tz="US/Eastern")}], "z": "US/Eastern", "itemtype": "*" }
@@ -6172,14 +6138,20 @@
         else:
             return []
     instances = []
     dtstart = item['s']
     if not (isinstance(dtstart, datetime) or isinstance(dtstart, date)):
         return []
     # This should not be necessary since the data store decodes dates as datetimes
+    if aft_dt is None:
+        if '+' in item:
+            tmp = min(item['+'])
+            aft_dt = min(tmp, dtstart)
+        else:
+            aft_dt = dtstart
     if isinstance(dtstart, date) and not isinstance(dtstart, datetime):
         dtstart = datetime(
             year=dtstart.year,
             month=dtstart.month,
             day=dtstart.day,
             hour=0,
             minute=0,
@@ -6864,15 +6836,14 @@
     >>> end_dt = parse('2018-03-07 2pm')
     >>> fmt_extent(beg_dt, end_dt)
     '10am-2pm'
     """
     beg_suffix = end_suffix = ''
     ampm = settings['ampm']
     if not (isinstance(beg_dt, datetime) and isinstance(end_dt, datetime)):
-        logger.debug(f"{beg_dt = }; {end_dt = }")
         return 'xxx y'
 
     if ampm:
         diff = beg_dt.hour < 12 and end_dt.hour >= 12
         end_suffix = end_dt.strftime('%p').lower().rstrip('m')
         if diff:
             beg_suffix = beg_dt.strftime('%p').lower().rstrip('m')
@@ -7068,40 +7039,14 @@
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         if item['itemtype'] == '!':
             inbox.append([0, summary, item.doc_id, None, None])
             relevant = today
         
-        # elif item['itemtype'] == '~':
-        #     s = item.get('s', None)
-        #     q = item.get('q', [])
-        #     h = item.get('h', {})
-        #     quota = q[0] if q and len(q) > 0 else None
-        #     if not s or not q or not quota:
-        #         logger.error(f"bad goal: {item = }")
-        #         continue
-        #     weeks = q[1] if len(q) > 1 else None
-        #     if weeks and (now.date() - s.date()).days > weeks*7:
-        #         goal_counts['Ended'] += 1
-        #         continue
-        #     else:
-        #         this_week = now.isocalendar()[:2] 
-        #         this_week_str = f"{this_week[0]}:{this_week[1]:02}"
-        #         done = h.get(this_week_str, 0)
-        #         if int(quota) < 0:
-        #             goal_counts['Inactive'] += 1
-        #         else:
-        #             goal_counts['Active'] += 1
-
-        #     # omit days remaining:
-        #     goals.append([f"{done}/{abs(quota)}", summary, item.doc_id, None, None])
-        #     # show days remaining:
-        #     # goals.append([f"{done[0]}/{done[1]}-{weekdays_remaining}d", summary, item.doc_id, None, None])
-
         elif 'f' in item:
             if not isinstance(item['f'], Period):
                 logger.error(f"{item['f'] = } in {item = }")
                 raise ValueError(f"{item['f']} is not an instance of type Period")
             relevant = item['f'].end
             if isinstance(relevant, date) and not isinstance(
                 relevant, datetime
@@ -7171,21 +7116,21 @@
                 if '+' in item:
                     for dt in item['+']:
                         dt = date_to_datetime(dt)
                         rset.rdate(dt)
 
                 if item['itemtype'] == '-':
                     switch = item.get('o', 'k')
+                    plus_dates = item.get('+', [])
                     if switch == 's':
                         cur = date_to_datetime(item['s'])
                         # make 'all day' tasks not pastdue until one minute before midnight
                         delta = (
                             timedelta(hours=23, minutes=59) if (cur.hour == 0 and cur.minute == 0) else ZERO
                         )
-                        plus_dates = item.get('+', [])
                         if cur + delta < now:
                             # we need to update @s
                             relevant = rset.after(now, inc=True)
                             while relevant in plus_dates:
                                 relevant = rset.after(relevant, inc=False)
                             item['s'] = relevant
                             item.setdefault('h', []).append(
@@ -7221,15 +7166,22 @@
                             if changed:
                                 update_db(db, item.doc_id, item)
                         else:
                             relevant = cur
 
                     else:   # k or r
                         try:
-                            relevant = rset.after(today, inc=True)
+                            # relevant = rset.after(today, inc=True)
+                            instances = item_instances(item, None)
+                            instances.sort()
+                            relevant = instances[0][0] if instances else None
+                            # relevant = rset.after(dtstart, inc=True)
+                            # if plus_dates:
+                            #     plus_dates.sort()
+                            #     relevant = min(relevant, plus_dates[0])
                         except Exception as e:
                             logger.debug(f"Exception: {e}\nissue with today: {today} ({type(today)}) or rset: {rset}\nskipping {item}")
                             continue
 
                         already_done = [x.end for x in item.get('h', [])]
                         # relevant will be the first instance after 12am today
                         # it will be the @s entry for the updated repeating item
@@ -7245,24 +7197,26 @@
                         # the current date falls after item['s'] and relevant is reset
                         num_remaining = (
                             f'({len(remaining)})' if remaining else ''
                         )
                         sum_abbr = item['summary'][:summary_width]
                         summary = f'{sum_abbr} {num_remaining}'
                         extent = item.get('e', ZERO)
-                        if dtstart.date() + extent < today.date() and 'j' not in item and 'r' not in item:
-                            pastdue.append(
-                                [
-                                    (dtstart.date() - today.date()).days,
+                        # if dtstart.date() + extent < today.date() and 'j' not in item:
+                        # if dtstart.date() + extent < today.date() and 'j' not in item and 'r' not in item:
+                        if relevant.date() + extent < today.date() and 'j' not in item:
+                            candidate = [
+                                    (relevant.date() - today.date()).days,
                                     summary,
                                     item.doc_id,
                                     None,
                                     None,
                                 ]
-                            )
+                            if candidate not in pastdue:
+                                pastdue.append(candidate)
                 else:
                     # get the first instance after today
                     try:
                         relevant = rset.after(today, inc=True)
                     except Exception as e:
                         logger.error(f'error processing {item}; {repr(e)}')
                     if not relevant:
@@ -7469,23 +7423,23 @@
         if (
             item['itemtype'] == '-'
             and 'f' not in item
             and 'j' not in item
             and relevant.date() < today.date()
         ):
             extent = item.get('e', ZERO)
-            pastdue.append(
-                [
+            candidate = [
                     ((relevant + extent).date() - today.date()).days,
                     summary,
                     item.doc_id,
                     None,
                     None,
                 ]
-            )
+            if candidate not in pastdue:
+                pastdue.append(candidate)
 
     inbox.sort()
     pastdue.sort()
     beginbys.sort()
     alerts.sort()
     # alerts: alert datetime, start datetime, commands, summary, doc_id
     week = today.isocalendar()[:2]
@@ -7681,18 +7635,14 @@
         rows.append(
             {
                 'sort': dt,
                 'path': year,
                 'values': [itemtype, summary, flags, rhc, doc_id],
             }
         )
-    # if len(rows) == 1:
-    #     logger.debug(f"rows[0]: {rows[0]}")
-    #     res = rows[0]
-    #     return item_details(res), {}
 
     rdict = NDict()
     path = f'query: {text[:summary_width]}{item_count}'
     for row in rows:
         values = row['values']
         rdict.add(path, values)
     tree, row2id = rdict.as_tree(rdict)
@@ -7974,15 +7924,14 @@
                         summary,
                         flags,
                         rhc,
                         (doc_id, None, None),
                     ],
                 }
             )
-    # logger.debug(f"{[x['sort'] for x in rows] = }")
     rows.sort(key=itemgetter('sort'))
     rdict = NDict()
     for row in rows:
         if using_groups:
             groups = location2groups.get(row['location'], ['OTHER'])
             for group in groups:
                 path = f"{group}/{row['location']}"
@@ -8121,15 +8070,14 @@
         s = item.get('s', None)
         q = item.get('q', [])
         h = item.get('h', {})
         for k, v in h.items():
             count += 1
             total += int(v)
         average = f"{total/count:.2}" if count and total else 0
-        logger.debug(f"{summary = }; {total = }; {count = }; {average = }")
         path = None
         # status: current, paused, ended, bad
         
         quota = q[0] if len(q) > 0 else None
         if not s or q is None:
             logger.error(f"bad goal: {item = }")
             continue
@@ -8155,29 +8103,27 @@
                 itemtype='~'
 
         if path == 'Active' and current_weekday >= 0:
             fraction_done = done/abs(quota)
             min_used = (current_weekday)/7 #  0, 1/7, ..., 6/7
             max_used = (current_weekday+1)/7 # 1/7, 2/7, ..., 1
             need = math.ceil(max_used*abs(quota) - done)
-            # logger.debug(f"{max_used*abs(quota) = }; {done = }")
             goal = f"{done}/{abs(quota)}+{need} ({average})" if need > 0 else f"{done}/{abs(quota)} ({average})"
             if current_weekday == 0:
                 # Monday - don't warn about 0 completions
                 itemtype = '~'
             elif fraction_done >= max_used:
                 # on target
                 itemtype = '~'
             elif fraction_done >= min_used:
                 # borderline
                 itemtype = EtmChar.SLOW_CHAR
             else:
                 # behind
                 itemtype = EtmChar.LATE_CHAR
-            logger.debug(f"{fraction_done = }; {max_used = }; {min_used = }; {current_weekday = }")
 
         sort = (path2sort[path], ss, summary)
 
         flags = get_flags(
             doc_id, repeat_list, link_list, konnected, pinned_list, timers
         )
         rows.append(
@@ -8376,15 +8322,14 @@
     konnected=[],
     timers={},
 ):
     width = shutil.get_terminal_size()[0] - 3
     rows = []
     rhc_width = 8
     md_fmt = '%-d %b' if settings['dayfirst'] else '%b %-d'
-    logger.debug(f'repeat_list: {repeat_list}; pinned_list: {pinned_list}')
 
     for item in items:
         mt = item.get('modified', None)
         if mt is not None:
             dt, label = mt, 'm'
         else:
             dt, label = item.get('created', None), 'c'
@@ -8697,23 +8642,14 @@
     tomorrowYMD = (now + 1 * DAY).strftime('%Y%m%d')
 
     for item in db:
         completed = []
         if item.get('itemtype', None) == None:
             logger.error(f'itemtype missing from {item}')
             continue
-        # if item['itemtype'] == '~':
-        #     # add completions from history to goal_hsh
-        #     g_s = item.get('summary', '')
-        #     g_c = item.get('h', {}) # 'yyyy:ww' -> done
-        #     for k, v in g_c.items():
-        #         g_yw = [int(x) for x in k.split(':')]
-        #         g_r = f"~ {g_s}: {str(v)}"
-        #         goal_hsh.setdefault(tuple(g_yw), []).append(g_r)
-        #     continue
 
         if item['itemtype'] in '!?~':
             continue
 
         doc_id = item.doc_id
 
         itemtype = item['itemtype']
@@ -8852,15 +8788,16 @@
                                 '',
                                 (row[2], None, row[3]),
                             ],
                         }
                     )
 
         startdt = date_to_datetime(start)
-        if not start or finished is not None or startdt in completed:
+        # if not start or finished is not None or startdt in completed:
+        if not start or finished is not None:
             continue
 
         # XXX INSTANCES
 
         # keep these for reference for this item
         end_dt = None
 
@@ -8926,15 +8863,14 @@
                     if 'f' in job:
                         continue
                     job_summary = job.get('summary', '')
                     jobstart = dt + job.get('s', ZERO)
                     sort_dt = jobstart.strftime('%Y%m%d%H%M')
                     if sort_dt.endswith('0000'):
                         sort_dt = sort_dt[:-4] + '2359'
-                    # logger.debug(f"{job = }; {sort_dt = }")
                     job_id = job.get('i', None)
                     job_sort = str(job_id)
 
                     # rhc = fmt_time(dt).center(rhc_width, ' ')
                     et = job.get('e', ZERO)
                     if et:
                         if omit and 'c' in item and item['c'] in omit:
@@ -9147,32 +9083,16 @@
     
 
     if yw == getWeekNum(now):
         rows.extend(current)
     rows.sort(key=itemgetter('sort'))
     done.sort(key=itemgetter('sort'))
     effort.sort(key=itemgetter('sort'))
-    # if goal_hsh:
-    #     tmp = {}
-    #     wks = []
-    #     for k, v in goal_hsh.items():
-    #         wks.append(k)
-    #         v.sort()
-    #         tmp[k] = v
-    #     wks.sort()
-    #     out = "Goals\n"
-    #     for k in wks:
-    #         out += f"  {k[0]}:{k[1]}\n"
-    #         for row in tmp[k]:
-    #             out += f"    {row}\n"
-    #     logger.debug(f"{out}")
-
     busy_details = {}
     allday_details = {}
-    # TODO
     dent = int((width - 69) / 2) * ' '
 
     ### item/agenda loop 2
     today = format_wkday(now)
     tomorrow = format_wkday(now + 1 * DAY)
 
     for week in week2day2allday:
```

### Comparing `etm-dgraham-6.2.5/etm/options.py` & `etm-dgraham-6.2.6/etm/options.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/report.py` & `etm-dgraham-6.2.6/etm/report.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm/view.py` & `etm-dgraham-6.2.6/etm/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -2854,19 +2854,21 @@
         show_message('Finish', 'Only an unfinished task can be finished.')
         return
 
     # has_timer = doc_id in dataview.timers
     # timer_warning = " and\nits associated timer" if has_timer else ""
     repeating = 's' in hsh and ('r' in hsh or '+' in hsh)
     if repeating:
-        due = hsh['s']
-        at_plus = hsh.get('+', [])
-        if at_plus:
-            at_plus.sort()
-            due = min(due, model.date_to_datetime(at_plus[0]))
+        instances = model.item_instances(hsh, None, )
+        instances.sort()
+        due = instances[0][0] if instances else None
+        # at_plus = hsh.get('+', [])
+        # if at_plus:
+        #     at_plus.sort()
+        #     due = min(due, model.date_to_datetime(at_plus[0]))
     else:
         due = hsh.get('s', None)
 
     between = []
 
     title = 'Finish'
 
@@ -2940,14 +2942,15 @@
                 datetime.now().replace(
                     hour=0, minute=0, second=0, microsecond=0
                 ),
             )
             if x[0] not in already_done
         ]
         if between:
+            phrase = "More than one" if len(between) > 1 else "One"
             # show_message('Finish', "There is nothing to complete.")
             need = 2
             values_list = []
             # values.append( (0, format_datetime(between[0][0])[1]) )
             count = -1
             for x in between:
                 count += 1
@@ -2955,15 +2958,15 @@
                 # values_list.append(f"   {format_datetime(x)[1]}")
 
             values_str = '\n'.join(values_list)
 
             text = f"""\
 {hsh['itemtype']} {hsh['summary']}
 
-More than one instance of this task is past due:
+{phrase} instance of this task is past due:
 {values_str}
 The default entered below is to use the current moment and the number of the oldest instance. Edit this "completion datetime : instance number" entry if you wish\
             """
 
             default = f'{now} : 0'
             due = ''
         else:
@@ -3196,15 +3199,14 @@
 """
 
     get_choice(title, text, options)
 
     def coroutine():
         keypress = dataview.details_key_press
         done = keypress in (['escape', '0'] + [x for x in values.keys()])
-        logger.debug(f"{keypress = }; {done = }")
         if done:
             if keypress == '0':
                 ok, msg = import_file('lorem')
                 if ok:
                     dataview.refreshRelevant()
                     dataview.refreshAgenda()
                     if dataview.mk_current:
@@ -3372,15 +3374,14 @@
         show_message('copy', 'selection copied to system clipboard', 2)
     else:
         pyperclip.copy(edit_buffer.text)
         show_message('copy', 'entry text copied to system clipboard', 2)
 
 @bindings.add('c-c', filter=is_details)
 def copy_details(*event):
-    logger.debug(f"{is_editing() = }")
     selection = details_area.buffer.copy_selection().text
     if selection:
         pyperclip.copy(selection)
         show_message('copy', 'selection copied to system clipboard', 2)
     else:
         # get_app().clipboard.set_data(data)
         details = details_area.text
@@ -3934,15 +3935,14 @@
     application.layout.focus(text_area)
     set_text(dataview.show_active_view())
     restore_row_col(row, col)
 
 
 # @edit_bindings.add('c-s', filter=is_editing, eager=True)
 def save_changes(*event):
-    logger.debug(f"{dataview.is_editing = }")
     if edit_buffer_changed():
         try:
             timer_save = TimeIt('***SAVE***')
             maybe_save(item)
             timer_save.stop()
         except Exception as e:
             logger.error(f'exception: {e}')
@@ -4174,16 +4174,14 @@
         EtmChar.BUSY: type_colors['event'],
         EtmChar.CONF: type_colors['inbox'],
         EtmChar.ADAY: type_colors['wrap'],
         EtmChar.FREE: type_colors['wrap'],
     }
     # query = ETMQuery()
     style = get_style(window_colors)
-    logger.debug(f"{text_pattern = }; {etmhome = }")
-    logger.debug(f"calling agenda_view; {busy_colors = }")
     agenda_view()
     logger.debug(f"setting application: {bindings = }; {style = }; {event_handler = }")
     application = pta.Application(
         layout=Layout(
             root_container,
             focused_element=text_area,
         ),
```

### Comparing `etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO` & `etm-dgraham-6.2.6/etm_dgraham.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: etm-dgraham
-Version: 6.2.5
+Version: 6.2.6
 Summary: event and task manager
 Home-page: https://dagraham.github.io/etm-dgraham/
 Author: Daniel A Graham
 Author-email: dnlgrhm@gmail.com
 License: GPL
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `etm-dgraham-6.2.5/etm_dgraham.egg-info/PKG-INFO [conflicted]` & `etm-dgraham-6.2.6/etm_dgraham.egg-info/PKG-INFO [conflicted]`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etm_dgraham.egg-info/SOURCES.txt` & `etm-dgraham-6.2.6/etm_dgraham.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etmlogo.png` & `etm-dgraham-6.2.6/etmlogo.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etmlogo_small.png` & `etm-dgraham-6.2.6/etmlogo_small.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/etmview_agenda.png` & `etm-dgraham-6.2.6/etmview_agenda.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/namedcolors.py` & `etm-dgraham-6.2.6/namedcolors.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/new.png` & `etm-dgraham-6.2.6/new.png`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/setup.py` & `etm-dgraham-6.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/test/test_parser.py` & `etm-dgraham-6.2.6/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/utilities/colons_to_slashes.py` & `etm-dgraham-6.2.6/utilities/colons_to_slashes.py`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/utilities/etm_in` & `etm-dgraham-6.2.6/utilities/etm_in`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/utilities/inbasket` & `etm-dgraham-6.2.6/utilities/inbasket`

 * *Files identical despite different names*

### Comparing `etm-dgraham-6.2.5/utilities/open_in_mutt` & `etm-dgraham-6.2.6/utilities/open_in_mutt`

 * *Files identical despite different names*

