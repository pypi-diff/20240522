# Comparing `tmp/mayatk-0.9.8.tar.gz` & `tmp/mayatk-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mayatk-0.9.8.tar", last modified: Sun Dec 17 21:07:08 2023, max compression
+gzip compressed data, was "mayatk-0.9.9.tar", last modified: Wed Dec 20 15:35:28 2023, max compression
```

## Comparing `mayatk-0.9.8.tar` & `mayatk-0.9.9.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.904800 mayatk-0.9.8/
--rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.9.8/LICENSE
--rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.9.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2331 2023-12-17 21:07:08.903799 mayatk-0.9.8/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.864473 mayatk-0.9.8/mayatk/
--rw-rw-rw-   0        0        0     3681 2023-12-17 21:07:04.000000 mayatk-0.9.8/mayatk/__init__.py
--rw-rw-rw-   0        0        0     9777 2023-12-10 18:21:24.000000 mayatk-0.9.8/mayatk/anim_utils.py
--rw-rw-rw-   0        0        0     7373 2023-09-28 12:44:03.000000 mayatk-0.9.8/mayatk/cam_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.878840 mayatk-0.9.8/mayatk/core_utils/
--rw-rw-rw-   0        0        0      622 2023-10-05 14:58:53.000000 mayatk-0.9.8/mayatk/core_utils/__init__.py
--rw-rw-rw-   0        0        0    24274 2023-12-10 12:13:38.000000 mayatk-0.9.8/mayatk/core_utils/_core_utils.py
--rw-rw-rw-   0        0        0    70573 2023-12-14 21:09:17.000000 mayatk-0.9.8/mayatk/core_utils/components.py
--rw-rw-rw-   0        0        0    11637 2023-12-17 13:52:51.000000 mayatk-0.9.8/mayatk/core_utils/macro.py
--rw-rw-rw-   0        0        0    13446 2023-09-06 12:44:32.000000 mayatk-0.9.8/mayatk/core_utils/mash.py
--rw-rw-rw-   0        0        0     7254 2023-11-08 16:58:30.000000 mayatk-0.9.8/mayatk/core_utils/preview.py
--rw-rw-rw-   0        0        0    12138 2023-11-07 03:38:12.000000 mayatk-0.9.8/mayatk/core_utils/project.py
--rw-rw-rw-   0        0        0    12342 2023-10-31 11:50:37.000000 mayatk-0.9.8/mayatk/core_utils/reference_manager.py
--rw-rw-rw-   0        0        0     6428 2023-10-23 14:26:30.000000 mayatk-0.9.8/mayatk/core_utils/reference_manager.ui
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.880841 mayatk-0.9.8/mayatk/display_utils/
--rw-rw-rw-   0        0        0      341 2023-09-06 12:44:32.000000 mayatk-0.9.8/mayatk/display_utils/__init__.py
--rw-rw-rw-   0        0        0     4009 2023-11-09 02:25:51.000000 mayatk-0.9.8/mayatk/display_utils/_display_utils.py
--rw-rw-rw-   0        0        0     6014 2023-12-11 15:47:31.000000 mayatk-0.9.8/mayatk/display_utils/exploded_view.py
--rw-rw-rw-   0        0        0     8630 2023-12-11 15:08:13.000000 mayatk-0.9.8/mayatk/display_utils/exploded_view.ui
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.891518 mayatk-0.9.8/mayatk/edit_utils/
--rw-rw-rw-   0        0        0      394 2023-09-06 12:44:32.000000 mayatk-0.9.8/mayatk/edit_utils/__init__.py
--rw-rw-rw-   0        0        0    40012 2023-12-01 19:24:02.000000 mayatk-0.9.8/mayatk/edit_utils/_edit_utils.py
--rw-rw-rw-   0        0        0     4093 2023-10-05 14:38:13.000000 mayatk-0.9.8/mayatk/edit_utils/bevel_edges.py
--rw-rw-rw-   0        0        0     8555 2023-12-01 19:41:02.000000 mayatk-0.9.8/mayatk/edit_utils/bevel_edges.ui
--rw-rw-rw-   0        0        0     3576 2023-12-01 21:04:54.000000 mayatk-0.9.8/mayatk/edit_utils/cut_on_axis.py
--rw-rw-rw-   0        0        0     9950 2023-12-17 17:08:38.000000 mayatk-0.9.8/mayatk/edit_utils/cut_on_axis.ui
--rw-rw-rw-   0        0        0     4502 2023-09-20 18:32:00.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_grid.py
--rw-rw-rw-   0        0        0    13102 2023-10-04 16:40:31.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_grid.ui
--rw-rw-rw-   0        0        0     7045 2023-09-27 13:23:23.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_linear.py
--rw-rw-rw-   0        0        0    23445 2023-10-04 16:40:54.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_linear.ui
--rw-rw-rw-   0        0        0     7471 2023-10-01 15:04:51.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_radial.py
--rw-rw-rw-   0        0        0    34535 2023-10-04 16:40:39.000000 mayatk-0.9.8/mayatk/edit_utils/duplicate_radial.ui
--rw-rw-rw-   0        0        0     3536 2023-12-01 17:06:42.000000 mayatk-0.9.8/mayatk/edit_utils/mirror.py
--rw-rw-rw-   0        0        0     9664 2023-10-23 14:26:30.000000 mayatk-0.9.8/mayatk/edit_utils/mirror.ui
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.895791 mayatk-0.9.8/mayatk/mat_utils/
--rw-rw-rw-   0        0        0      344 2023-09-12 13:56:55.000000 mayatk-0.9.8/mayatk/mat_utils/__init__.py
--rw-rw-rw-   0        0        0    13781 2023-10-01 16:06:02.000000 mayatk-0.9.8/mayatk/mat_utils/_mat_utils.py
--rw-rw-rw-   0        0        0     6068 2023-10-02 12:53:33.000000 mayatk-0.9.8/mayatk/mat_utils/hdr_manager.py
--rw-rw-rw-   0        0        0    11211 2023-10-25 13:11:20.000000 mayatk-0.9.8/mayatk/mat_utils/hdr_manager.ui
--rw-rw-rw-   0        0        0    18022 2023-11-06 01:11:52.000000 mayatk-0.9.8/mayatk/mat_utils/stingray_arnold_shader.py
--rw-rw-rw-   0        0        0    13370 2023-10-03 16:10:32.000000 mayatk-0.9.8/mayatk/mat_utils/stingray_arnold_shader.ui
--rw-rw-rw-   0        0        0    31815 2023-10-24 01:44:30.000000 mayatk-0.9.8/mayatk/node_utils.py
--rw-rw-rw-   0        0        0    18104 2023-12-10 12:09:45.000000 mayatk-0.9.8/mayatk/rig_utils.py
--rw-rw-rw-   0        0        0    30106 2023-12-01 19:44:33.000000 mayatk-0.9.8/mayatk/xform_utils.py
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.902835 mayatk-0.9.8/mayatk.egg-info/
--rw-rw-rw-   0        0        0     2331 2023-12-17 21:07:08.000000 mayatk-0.9.8/mayatk.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1619 2023-12-17 21:07:08.000000 mayatk-0.9.8/mayatk.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-12-17 21:07:08.000000 mayatk-0.9.8/mayatk.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       43 2023-12-17 21:07:08.000000 mayatk-0.9.8/mayatk.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-12-17 21:07:08.000000 mayatk-0.9.8/mayatk.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-12-17 21:07:08.904800 mayatk-0.9.8/setup.cfg
--rw-rw-rw-   0        0        0     1465 2023-12-17 13:21:52.000000 mayatk-0.9.8/setup.py
-drwxrwxrwx   0        0        0        0 2023-12-17 21:07:08.902835 mayatk-0.9.8/test/
--rw-rw-rw-   0        0        0     1289 2023-09-18 17:28:10.000000 mayatk-0.9.8/test/__init__.py
--rw-rw-rw-   0        0        0    26254 2023-11-08 11:36:43.000000 mayatk-0.9.8/test/components_test.py
--rw-rw-rw-   0        0        0     4594 2023-10-06 00:03:03.000000 mayatk-0.9.8/test/core_utils_test.py
--rw-rw-rw-   0        0        0     6651 2023-11-07 11:53:59.000000 mayatk-0.9.8/test/edit_utils_test.py
--rw-rw-rw-   0        0        0     2179 2023-10-06 00:08:07.000000 mayatk-0.9.8/test/mat_utils_test.py
--rw-rw-rw-   0        0        0     4774 2023-10-06 00:04:10.000000 mayatk-0.9.8/test/node_utils_test.py
--rw-rw-rw-   0        0        0     2754 2023-10-23 14:26:30.000000 mayatk-0.9.8/test/rig_utils_test.py
--rw-rw-rw-   0        0        0      470 2023-11-07 11:30:14.000000 mayatk-0.9.8/test/run_tests.py
--rw-rw-rw-   0        0        0     3669 2023-10-06 00:02:48.000000 mayatk-0.9.8/test/xform_utils_test.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.808808 mayatk-0.9.9/
+-rw-rw-rw-   0        0        0     1093 2023-03-28 23:39:14.000000 mayatk-0.9.9/LICENSE
+-rw-rw-rw-   0        0        0       27 2023-03-28 23:39:14.000000 mayatk-0.9.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2331 2023-12-20 15:35:28.807786 mayatk-0.9.9/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.301825 mayatk-0.9.9/mayatk/
+-rw-rw-rw-   0        0        0     3681 2023-12-20 15:35:23.000000 mayatk-0.9.9/mayatk/__init__.py
+-rw-rw-rw-   0        0        0     9777 2023-12-10 18:21:24.000000 mayatk-0.9.9/mayatk/anim_utils.py
+-rw-rw-rw-   0        0        0     7373 2023-09-28 12:44:03.000000 mayatk-0.9.9/mayatk/cam_utils.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.465596 mayatk-0.9.9/mayatk/core_utils/
+-rw-rw-rw-   0        0        0      622 2023-10-05 14:58:53.000000 mayatk-0.9.9/mayatk/core_utils/__init__.py
+-rw-rw-rw-   0        0        0    24274 2023-12-10 12:13:38.000000 mayatk-0.9.9/mayatk/core_utils/_core_utils.py
+-rw-rw-rw-   0        0        0    70573 2023-12-14 21:09:17.000000 mayatk-0.9.9/mayatk/core_utils/components.py
+-rw-rw-rw-   0        0        0    11637 2023-12-17 13:52:51.000000 mayatk-0.9.9/mayatk/core_utils/macro.py
+-rw-rw-rw-   0        0        0    13446 2023-09-06 12:44:32.000000 mayatk-0.9.9/mayatk/core_utils/mash.py
+-rw-rw-rw-   0        0        0     7254 2023-11-08 16:58:30.000000 mayatk-0.9.9/mayatk/core_utils/preview.py
+-rw-rw-rw-   0        0        0    12138 2023-11-07 03:38:12.000000 mayatk-0.9.9/mayatk/core_utils/project.py
+-rw-rw-rw-   0        0        0    12342 2023-10-31 11:50:37.000000 mayatk-0.9.9/mayatk/core_utils/reference_manager.py
+-rw-rw-rw-   0        0        0     6428 2023-10-23 14:26:30.000000 mayatk-0.9.9/mayatk/core_utils/reference_manager.ui
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.508723 mayatk-0.9.9/mayatk/display_utils/
+-rw-rw-rw-   0        0        0      341 2023-09-06 12:44:32.000000 mayatk-0.9.9/mayatk/display_utils/__init__.py
+-rw-rw-rw-   0        0        0     4009 2023-11-09 02:25:51.000000 mayatk-0.9.9/mayatk/display_utils/_display_utils.py
+-rw-rw-rw-   0        0        0     6014 2023-12-11 15:47:31.000000 mayatk-0.9.9/mayatk/display_utils/exploded_view.py
+-rw-rw-rw-   0        0        0     8630 2023-12-11 15:08:13.000000 mayatk-0.9.9/mayatk/display_utils/exploded_view.ui
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.676495 mayatk-0.9.9/mayatk/edit_utils/
+-rw-rw-rw-   0        0        0      394 2023-09-06 12:44:32.000000 mayatk-0.9.9/mayatk/edit_utils/__init__.py
+-rw-rw-rw-   0        0        0    40469 2023-12-20 14:19:21.000000 mayatk-0.9.9/mayatk/edit_utils/_edit_utils.py
+-rw-rw-rw-   0        0        0     4093 2023-10-05 14:38:13.000000 mayatk-0.9.9/mayatk/edit_utils/bevel_edges.py
+-rw-rw-rw-   0        0        0     8555 2023-12-01 19:41:02.000000 mayatk-0.9.9/mayatk/edit_utils/bevel_edges.ui
+-rw-rw-rw-   0        0        0     3576 2023-12-01 21:04:54.000000 mayatk-0.9.9/mayatk/edit_utils/cut_on_axis.py
+-rw-rw-rw-   0        0        0     9950 2023-12-17 17:08:38.000000 mayatk-0.9.9/mayatk/edit_utils/cut_on_axis.ui
+-rw-rw-rw-   0        0        0     4502 2023-09-20 18:32:00.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_grid.py
+-rw-rw-rw-   0        0        0    13102 2023-10-04 16:40:31.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_grid.ui
+-rw-rw-rw-   0        0        0     7045 2023-09-27 13:23:23.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_linear.py
+-rw-rw-rw-   0        0        0    23445 2023-10-04 16:40:54.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_linear.ui
+-rw-rw-rw-   0        0        0     7471 2023-10-01 15:04:51.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_radial.py
+-rw-rw-rw-   0        0        0    34535 2023-10-04 16:40:39.000000 mayatk-0.9.9/mayatk/edit_utils/duplicate_radial.ui
+-rw-rw-rw-   0        0        0     3536 2023-12-01 17:06:42.000000 mayatk-0.9.9/mayatk/edit_utils/mirror.py
+-rw-rw-rw-   0        0        0     9664 2023-10-23 14:26:30.000000 mayatk-0.9.9/mayatk/edit_utils/mirror.ui
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.735607 mayatk-0.9.9/mayatk/mat_utils/
+-rw-rw-rw-   0        0        0      344 2023-09-12 13:56:55.000000 mayatk-0.9.9/mayatk/mat_utils/__init__.py
+-rw-rw-rw-   0        0        0    13781 2023-10-01 16:06:02.000000 mayatk-0.9.9/mayatk/mat_utils/_mat_utils.py
+-rw-rw-rw-   0        0        0     6068 2023-10-02 12:53:33.000000 mayatk-0.9.9/mayatk/mat_utils/hdr_manager.py
+-rw-rw-rw-   0        0        0    11211 2023-10-25 13:11:20.000000 mayatk-0.9.9/mayatk/mat_utils/hdr_manager.ui
+-rw-rw-rw-   0        0        0    18022 2023-11-06 01:11:52.000000 mayatk-0.9.9/mayatk/mat_utils/stingray_arnold_shader.py
+-rw-rw-rw-   0        0        0    13370 2023-10-03 16:10:32.000000 mayatk-0.9.9/mayatk/mat_utils/stingray_arnold_shader.ui
+-rw-rw-rw-   0        0        0    31815 2023-10-24 01:44:30.000000 mayatk-0.9.9/mayatk/node_utils.py
+-rw-rw-rw-   0        0        0    18104 2023-12-10 12:09:45.000000 mayatk-0.9.9/mayatk/rig_utils.py
+-rw-rw-rw-   0        0        0    30106 2023-12-01 19:44:33.000000 mayatk-0.9.9/mayatk/xform_utils.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.807786 mayatk-0.9.9/mayatk.egg-info/
+-rw-rw-rw-   0        0        0     2331 2023-12-20 15:35:28.000000 mayatk-0.9.9/mayatk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1619 2023-12-20 15:35:28.000000 mayatk-0.9.9/mayatk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-12-20 15:35:28.000000 mayatk-0.9.9/mayatk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       43 2023-12-20 15:35:28.000000 mayatk-0.9.9/mayatk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-12-20 15:35:28.000000 mayatk-0.9.9/mayatk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-12-20 15:35:28.808808 mayatk-0.9.9/setup.cfg
+-rw-rw-rw-   0        0        0     1465 2023-12-17 13:21:52.000000 mayatk-0.9.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-12-20 15:35:28.805804 mayatk-0.9.9/test/
+-rw-rw-rw-   0        0        0     1289 2023-09-18 17:28:10.000000 mayatk-0.9.9/test/__init__.py
+-rw-rw-rw-   0        0        0    26254 2023-11-08 11:36:43.000000 mayatk-0.9.9/test/components_test.py
+-rw-rw-rw-   0        0        0     4594 2023-10-06 00:03:03.000000 mayatk-0.9.9/test/core_utils_test.py
+-rw-rw-rw-   0        0        0     6651 2023-11-07 11:53:59.000000 mayatk-0.9.9/test/edit_utils_test.py
+-rw-rw-rw-   0        0        0     2179 2023-10-06 00:08:07.000000 mayatk-0.9.9/test/mat_utils_test.py
+-rw-rw-rw-   0        0        0     4774 2023-10-06 00:04:10.000000 mayatk-0.9.9/test/node_utils_test.py
+-rw-rw-rw-   0        0        0     2754 2023-10-23 14:26:30.000000 mayatk-0.9.9/test/rig_utils_test.py
+-rw-rw-rw-   0        0        0      470 2023-11-07 11:30:14.000000 mayatk-0.9.9/test/run_tests.py
+-rw-rw-rw-   0        0        0     3669 2023-10-06 00:02:48.000000 mayatk-0.9.9/test/xform_utils_test.py
```

### Comparing `mayatk-0.9.8/LICENSE` & `mayatk-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/PKG-INFO` & `mayatk-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.9.8
+Version: 0.9.9
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 Requires-Dist: PySide2
 Requires-Dist: pythontk==0.7.10
 Requires-Dist: uitk==1.0.7
 Requires-Dist: pymel
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/Version-0.9.8-blue.svg)](https://pypi.org/project/mayatk/)
+[![Version](https://img.shields.io/badge/Version-0.9.9-blue.svg)](https://pypi.org/project/mayatk/)
 [![CoreUtils Tests](https://img.shields.io/badge/CoreUtils-Passing-brightgreen.svg)](../test/core_utils_test.py#CoreUtilsTest)
 [![XformUtils Tests](https://img.shields.io/badge/XformUtils-Passing-brightgreen.svg)](../test/xform_utils_test.py#XformUtilsTest)
 [![EditUtils Tests](https://img.shields.io/badge/EditUtils-Passing-brightgreen.svg)](../test/edit_utils_test.py#EditUtilsTest)
 [![NodeUtils Tests](https://img.shields.io/badge/NodeUtils-Passing-brightgreen.svg)](../test/edit_utils_test.py#NodeUtilsTest)
 [![CamUtils Tests](https://img.shields.io/badge/CamUtils-Passing-brightgreen.svg)](../test/cam_utils_test.py#CamUtilsTest)
 [![MatUtils Tests](https://img.shields.io/badge/MatUtils-Passing-brightgreen.svg)](../test/mat_utils_test.py#MatUtilsTest)
 [![RigUtils Tests](https://img.shields.io/badge/RigUtils-Passing-brightgreen.svg)](../test/rig_utils_test.py#RigUtilsTest)
```

### Comparing `mayatk-0.9.8/mayatk/__init__.py` & `mayatk-0.9.9/mayatk/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # coding=utf-8
 import inspect
 import importlib
 import pkgutil
 
 
 __package__ = "mayatk"
-__version__ = "0.9.8"
+__version__ = "0.9.9"
 
 """Dynamic Attribute Resolver for Module-based Packages
 
 This module implements a dynamic attribute resolver that allows accessing attributes
 (classes, methods, and class methods) from a package's modules using the pattern
 '<package>.<attribute>'. The resolver builds dictionaries that map attribute names to
 their respective module names, enabling efficient and maintainable access to these
```

### Comparing `mayatk-0.9.8/mayatk/anim_utils.py` & `mayatk-0.9.9/mayatk/anim_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/cam_utils.py` & `mayatk-0.9.9/mayatk/cam_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/__init__.py` & `mayatk-0.9.9/mayatk/core_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/_core_utils.py` & `mayatk-0.9.9/mayatk/core_utils/_core_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/components.py` & `mayatk-0.9.9/mayatk/core_utils/components.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/macro.py` & `mayatk-0.9.9/mayatk/core_utils/macro.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/mash.py` & `mayatk-0.9.9/mayatk/core_utils/mash.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/preview.py` & `mayatk-0.9.9/mayatk/core_utils/preview.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/project.py` & `mayatk-0.9.9/mayatk/core_utils/project.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/reference_manager.py` & `mayatk-0.9.9/mayatk/core_utils/reference_manager.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/core_utils/reference_manager.ui` & `mayatk-0.9.9/mayatk/core_utils/reference_manager.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/display_utils/_display_utils.py` & `mayatk-0.9.9/mayatk/display_utils/_display_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/display_utils/exploded_view.py` & `mayatk-0.9.9/mayatk/display_utils/exploded_view.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/display_utils/exploded_view.ui` & `mayatk-0.9.9/mayatk/display_utils/exploded_view.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/_edit_utils.py` & `mayatk-0.9.9/mayatk/edit_utils/_edit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,91 +9,106 @@
 # from this package:
 from mayatk import core_utils, node_utils, xform_utils
 
 
 class EditUtils:
     """ """
 
-    @staticmethod
+    @classmethod
     @core_utils.CoreUtils.undo
-    def rename(objects, to, fltr="", regex=False, ignore_case=False):
-        """Rename scene objects.
+    def rename(cls, objects, to, fltr="", regex=False, ignore_case=False):
+        """Rename scene objects based on specified patterns and filters, ensuring compliance with Maya's naming conventions.
 
         Parameters:
-            objects (str/obj/list): The object(s to rename. If nothing is given, all scene objects will be renamed.
-            to (str): Desired name: An optional asterisk modifier can be used for formatting
+            objects (str/obj/list): The object(s) to rename. If empty, all scene objects will be renamed.
+            to (str): Desired name pattern. Asterisk (*) can be used for formatting:
                     chars - replace all.
                     *chars* - replace only.
                     *chars - replace suffix.
                     **chars - append suffix.
                     chars* - replace prefix.
                     chars** - append prefix.
-            fltr (str): Optionally, filter which the given objects to rename using the following:
-                    An asterisk denotes startswith*, *endswith, *contains*, and multiple search strings can be separated by pipe ('|') chars.
-                    chars - Search exact.
-                    *chars* - Search contains chars.
-                    *chars - Search endswith chars.
-                    chars* - Search startswith chars.
-                    chars|chars - Search any of.  can be used in conjuction with other modifiers.
-            regex (bool): If True, regular expression syntax is used instead of the default '*' and '|' modifiers.
-            ignore_case (bool): Ignore case when searching. Applies only to the 'fltr' parameter's search.
+            fltr (str): Filter to apply on object names using wildcards or regular expressions:
+                    chars - exact match.
+                    *chars* - contains chars.
+                    *chars - ends with chars.
+                    chars* - starts with chars.
+                    chars|chars - matches any of the specified patterns.
+            regex (bool): Use regular expressions if True, else use default '*' and '|' modifiers for pattern matching.
+            ignore_case (bool): Ignore case when filtering. Applies only to the 'fltr' parameter.
+
+        Returns:
+            None: Objects are renamed in the scene directly.
 
         Example:
-            rename(r'Cube', '*001', regex=True) #replace chars after 'fltr' on any object with a name that contains 'Cube'. ie. 'polyCube001' from 'polyCube'
-            rename(r'Cube', '**001', regex=True) #append chars on any object with a name that contains 'Cube'. ie. 'polyCube1001' from 'polyCube1'
+            rename('Cube', '*001', regex=True) # Replace suffix on objects containing 'Cube' in their name, e.g., 'polyCube' becomes 'polyCube001'.
+            rename('Cube', '**001', regex=True) # Append '001' to names of objects containing 'Cube', e.g., 'polyCube1' becomes 'polyCube1001'.
         """
-        # pm.undoInfo (openChunk=1)
         objects = pm.ls(objectsOnly=1) if not objects else pm.ls(objects)
-
-        # get the short names from the long in order to correctly format. ex. 'NUT_' from: 'CENTER_HINGE_FEMALE_GRP|NUT_'
         long_names = [obj.name() for obj in objects]
-        short_names = [
-            ii if ii else i for i, ii in ptk.split_at_chars(long_names)
-        ]  # split the long names at the last '|' to get the short name.
+        short_names = [ii if ii else i for i, ii in ptk.split_at_chars(long_names)]
 
         names = ptk.find_str_and_format(
             short_names,
             to,
             fltr,
             regex=regex,
             ignore_case=ignore_case,
             return_orig_strings=True,
         )
+
         print("# Rename: Found {} matches. #".format(len(names)))
 
         for i, (oldName, newName) in enumerate(names):
-            oldName = long_names[
-                i
-            ]  # use the long name to reference the object instead.
+            # Strip illegal characters from newName
+            newName = cls.strip_illegal_chars(newName)
+
+            oldName = long_names[i]  # Use the long name to reference the object
             try:
                 if pm.objExists(oldName):
-                    n = pm.rename(
-                        oldName, newName
-                    )  # Rename the object with the new name
+                    n = pm.rename(oldName, newName)  # Rename the object
                     if not n == newName:
                         print(
-                            '# Warning: Attempt to rename "{}" to "{}" failed. Renamed instead to "{}". #'.format(
-                                oldName, newName, n
-                            )
-                        )
-                    else:
-                        print(
-                            '# Result: Successfully renamed "{}" to "{}". #'.format(
-                                oldName, newName
+                            '# Warning: "{}" renamed to "{}" instead of "{}". #'.format(
+                                oldName, n, newName
                             )
                         )
-
             except Exception as e:
-                if not pm.ls(oldName, readOnly=True) == []:  # ignore read-only errors.
+                if not pm.ls(oldName, readOnly=True) == []:  # Ignore read-only errors
                     print(
-                        '# Error: Attempt to rename "{}" to "{}" failed. {} #'.format(
+                        '# Error renaming "{}" to "{}": {} #'.format(
                             oldName, newName, str(e).rstrip()
                         )
                     )
-        # pm.undoInfo (closeChunk=1)
+
+    @staticmethod
+    def strip_illegal_chars(input_data, replace_with="_"):
+        """Strips illegal characters from a string or a list of strings, replacing them with a specified character, conforming to Maya naming conventions.
+
+        Parameters:
+            input_data (str/list): A single string or a list of strings to be sanitized.
+            replace_with (str): The character to replace illegal characters with. Default is underscore (_).
+
+        Returns:
+            str/list: Sanitized string or list of strings, with illegal characters replaced.
+        """
+        import re
+
+        def clean_string(s):
+            pattern = re.compile(r"[^a-zA-Z0-9_]")
+            return pattern.sub(replace_with, s)
+
+        if isinstance(input_data, (list, tuple, set)):
+            return [clean_string(s) for s in input_data]
+        elif isinstance(input_data, str):
+            return clean_string(input_data)
+        else:
+            raise TypeError(
+                "Input data must be a string or a list, tuple, set of strings."
+            )
 
     @staticmethod
     @core_utils.CoreUtils.undo
     def set_case(objects=[], case="caplitalize"):
         """Rename objects following the given case.
 
         Parameters:
```

### Comparing `mayatk-0.9.8/mayatk/edit_utils/bevel_edges.py` & `mayatk-0.9.9/mayatk/edit_utils/bevel_edges.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/bevel_edges.ui` & `mayatk-0.9.9/mayatk/edit_utils/bevel_edges.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/cut_on_axis.py` & `mayatk-0.9.9/mayatk/edit_utils/cut_on_axis.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/cut_on_axis.ui` & `mayatk-0.9.9/mayatk/edit_utils/cut_on_axis.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_grid.py` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_grid.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_grid.ui` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_grid.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_linear.py` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_linear.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_linear.ui` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_linear.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_radial.py` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_radial.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/duplicate_radial.ui` & `mayatk-0.9.9/mayatk/edit_utils/duplicate_radial.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/mirror.py` & `mayatk-0.9.9/mayatk/edit_utils/mirror.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/edit_utils/mirror.ui` & `mayatk-0.9.9/mayatk/edit_utils/mirror.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/mat_utils/_mat_utils.py` & `mayatk-0.9.9/mayatk/mat_utils/_mat_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/mat_utils/hdr_manager.py` & `mayatk-0.9.9/mayatk/mat_utils/hdr_manager.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/mat_utils/hdr_manager.ui` & `mayatk-0.9.9/mayatk/mat_utils/hdr_manager.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/mat_utils/stingray_arnold_shader.py` & `mayatk-0.9.9/mayatk/mat_utils/stingray_arnold_shader.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/mat_utils/stingray_arnold_shader.ui` & `mayatk-0.9.9/mayatk/mat_utils/stingray_arnold_shader.ui`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/node_utils.py` & `mayatk-0.9.9/mayatk/node_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/rig_utils.py` & `mayatk-0.9.9/mayatk/rig_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk/xform_utils.py` & `mayatk-0.9.9/mayatk/xform_utils.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/mayatk.egg-info/PKG-INFO` & `mayatk-0.9.9/mayatk.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mayatk
-Version: 0.9.8
+Version: 0.9.9
 Summary: *mayattk is a collection of backend utilities for Autodesk Maya.*
 Home-page: https://github.com/m3trik/mayatk
 Author: Ryan Simpson
 Author-email: m3trik@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -12,15 +12,15 @@
 License-File: LICENSE
 Requires-Dist: PySide2
 Requires-Dist: pythontk==0.7.10
 Requires-Dist: uitk==1.0.7
 Requires-Dist: pymel
 
 [![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](https://opensource.org/licenses/MIT)
-[![Version](https://img.shields.io/badge/Version-0.9.8-blue.svg)](https://pypi.org/project/mayatk/)
+[![Version](https://img.shields.io/badge/Version-0.9.9-blue.svg)](https://pypi.org/project/mayatk/)
 [![CoreUtils Tests](https://img.shields.io/badge/CoreUtils-Passing-brightgreen.svg)](../test/core_utils_test.py#CoreUtilsTest)
 [![XformUtils Tests](https://img.shields.io/badge/XformUtils-Passing-brightgreen.svg)](../test/xform_utils_test.py#XformUtilsTest)
 [![EditUtils Tests](https://img.shields.io/badge/EditUtils-Passing-brightgreen.svg)](../test/edit_utils_test.py#EditUtilsTest)
 [![NodeUtils Tests](https://img.shields.io/badge/NodeUtils-Passing-brightgreen.svg)](../test/edit_utils_test.py#NodeUtilsTest)
 [![CamUtils Tests](https://img.shields.io/badge/CamUtils-Passing-brightgreen.svg)](../test/cam_utils_test.py#CamUtilsTest)
 [![MatUtils Tests](https://img.shields.io/badge/MatUtils-Passing-brightgreen.svg)](../test/mat_utils_test.py#MatUtilsTest)
 [![RigUtils Tests](https://img.shields.io/badge/RigUtils-Passing-brightgreen.svg)](../test/rig_utils_test.py#RigUtilsTest)
```

### Comparing `mayatk-0.9.8/mayatk.egg-info/SOURCES.txt` & `mayatk-0.9.9/mayatk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/setup.py` & `mayatk-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/__init__.py` & `mayatk-0.9.9/test/__init__.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/components_test.py` & `mayatk-0.9.9/test/components_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/core_utils_test.py` & `mayatk-0.9.9/test/core_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/edit_utils_test.py` & `mayatk-0.9.9/test/edit_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/mat_utils_test.py` & `mayatk-0.9.9/test/mat_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/node_utils_test.py` & `mayatk-0.9.9/test/node_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/rig_utils_test.py` & `mayatk-0.9.9/test/rig_utils_test.py`

 * *Files identical despite different names*

### Comparing `mayatk-0.9.8/test/xform_utils_test.py` & `mayatk-0.9.9/test/xform_utils_test.py`

 * *Files identical despite different names*

