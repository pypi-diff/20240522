# Comparing `tmp/prusa.connect.sdk.printer-0.7.1.tar.gz` & `tmp/prusa_connect_sdk_printer-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prusa.connect.sdk.printer-0.7.1.tar", last modified: Mon Oct  9 15:43:57 2023, max compression
+gzip compressed data, was "prusa_connect_sdk_printer-0.8.0.tar", last modified: Wed May 22 12:41:02 2024, max compression
```

## Comparing `prusa.connect.sdk.printer-0.7.1.tar` & `prusa_connect_sdk_printer-0.8.0.tar`

### file list

```diff
@@ -1,49 +1,50 @@
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.615256 prusa.connect.sdk.printer-0.7.1/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     5170 2023-10-09 15:18:32.000000 prusa.connect.sdk.printer-0.7.1/ChangeLog
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      128 2023-10-09 15:43:29.000000 prusa.connect.sdk.printer-0.7.1/MANIFEST.in
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7610 2023-10-09 15:43:57.611256 prusa.connect.sdk.printer-0.7.1/PKG-INFO
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6459 2023-02-13 11:09:16.000000 prusa.connect.sdk.printer-0.7.1/README.rst
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.607256 prusa.connect.sdk.printer-0.7.1/prusa/
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.607256 prusa.connect.sdk.printer-0.7.1/prusa/connect/
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.611256 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    30881 2023-10-09 15:18:32.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/__init__.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    19879 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    14921 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_configurator.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7291 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_controller.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    11803 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_driver.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      996 2022-03-17 11:43:55.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/clock.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6877 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/command.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    10144 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/conditions.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6717 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/const.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    15845 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/download.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     3377 2023-01-05 07:37:50.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/errors.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    32830 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/files.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6580 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/models.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2022-03-17 11:43:55.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/py.typed
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     2061 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/util.py
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.611256 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7610 2023-10-09 15:43:57.000000 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/PKG-INFO
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1147 2023-10-09 15:43:57.000000 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/SOURCES.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        1 2023-10-09 15:43:57.000000 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/dependency_links.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       80 2023-10-09 15:43:57.000000 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/requires.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)        6 2023-10-09 15:43:57.000000 prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/top_level.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6374 2023-10-09 15:43:44.000000 prusa.connect.sdk.printer-0.7.1/pyproject.toml
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       80 2023-10-09 15:18:32.000000 prusa.connect.sdk.printer-0.7.1/requirements.txt
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)       38 2023-10-09 15:43:57.615256 prusa.connect.sdk.printer-0.7.1/setup.cfg
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     2029 2023-05-24 10:58:11.000000 prusa.connect.sdk.printer-0.7.1/setup.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      781 2023-02-15 09:33:59.000000 prusa.connect.sdk.printer-0.7.1/sl.py
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.611256 prusa.connect.sdk.printer-0.7.1/tests/
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.607256 prusa.connect.sdk.printer-0.7.1/tests/gcodes/
-drwxr-xr-x   0 mcbig     (1000) mcbig     (1000)        0 2023-10-09 15:43:57.611256 prusa.connect.sdk.printer-0.7.1/tests/gcodes/metadata/
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2022-03-17 11:43:55.000000 prusa.connect.sdk.printer-0.7.1/tests/gcodes/metadata/.hidden_fdn_filename.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2022-03-17 11:43:55.000000 prusa.connect.sdk.printer-0.7.1/tests/gcodes/metadata/fdn_filename.gcode
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    22860 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/tests/test_cameras.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1130 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/tests/test_clock.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     5260 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/tests/test_command.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6860 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/tests/test_conditions.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    10228 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/tests/test_download.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1152 2023-05-24 08:47:29.000000 prusa.connect.sdk.printer-0.7.1/tests/test_errors.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1159 2022-03-17 11:43:55.000000 prusa.connect.sdk.printer-0.7.1/tests/test_events.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    23077 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/tests/test_files.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)    45445 2023-10-09 12:40:14.000000 prusa.connect.sdk.printer-0.7.1/tests/test_printer.py
--rw-r--r--   0 mcbig     (1000) mcbig     (1000)      560 2022-04-25 10:31:32.000000 prusa.connect.sdk.printer-0.7.1/tests/test_telemetry.py
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     5465 2024-05-22 12:38:00.000000 prusa_connect_sdk_printer-0.8.0/ChangeLog
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      128 2023-10-09 15:43:29.000000 prusa_connect_sdk_printer-0.8.0/MANIFEST.in
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7651 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/PKG-INFO
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6459 2023-02-13 11:09:16.000000 prusa_connect_sdk_printer-0.8.0/README.rst
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.787010 prusa_connect_sdk_printer-0.8.0/prusa/
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.787010 prusa_connect_sdk_printer-0.8.0/prusa/connect/
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.791010 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)    33024 2024-05-22 12:38:00.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/__init__.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    19879 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    14921 2023-05-24 08:47:29.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_configurator.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7291 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_controller.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    11803 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_driver.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      996 2022-03-17 11:43:55.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/clock.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6877 2023-05-24 08:47:29.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/command.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    10105 2024-03-13 14:33:11.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/conditions.py
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     6978 2024-05-22 12:16:34.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/const.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    16039 2024-03-13 14:28:17.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/download.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     3377 2023-01-05 07:37:50.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/errors.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    32830 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/files.py
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     6762 2024-05-15 08:39:53.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/models.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)        0 2022-03-17 11:43:55.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/py.typed
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     2061 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/util.py
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     7651 2024-05-22 12:41:02.000000 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/PKG-INFO
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     1165 2024-05-22 12:41:02.000000 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/SOURCES.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)        1 2024-05-22 12:41:02.000000 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/dependency_links.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)      106 2024-05-22 12:41:02.000000 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/requires.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)        6 2024-05-22 12:41:02.000000 prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/top_level.txt
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6374 2024-02-02 11:29:15.000000 prusa_connect_sdk_printer-0.8.0/pyproject.toml
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)      106 2024-05-22 12:38:00.000000 prusa_connect_sdk_printer-0.8.0/requirements.txt
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)       38 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/setup.cfg
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     2029 2023-05-24 10:58:11.000000 prusa_connect_sdk_printer-0.8.0/setup.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      781 2023-02-15 09:33:59.000000 prusa_connect_sdk_printer-0.8.0/sl.py
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/tests/
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.787010 prusa_connect_sdk_printer-0.8.0/tests/gcodes/
+drwxrwxr-x   0 mcbig     (1000) mcbig     (1000)        0 2024-05-22 12:41:02.795010 prusa_connect_sdk_printer-0.8.0/tests/gcodes/metadata/
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2022-03-17 11:43:55.000000 prusa_connect_sdk_printer-0.8.0/tests/gcodes/metadata/.hidden_fdn_filename.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    21829 2022-03-17 11:43:55.000000 prusa_connect_sdk_printer-0.8.0/tests/gcodes/metadata/fdn_filename.gcode
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    22784 2024-01-31 09:55:26.000000 prusa_connect_sdk_printer-0.8.0/tests/test_cameras.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1071 2024-01-31 09:55:26.000000 prusa_connect_sdk_printer-0.8.0/tests/test_clock.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     5260 2023-05-24 08:47:29.000000 prusa_connect_sdk_printer-0.8.0/tests/test_command.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     6860 2023-05-24 08:47:29.000000 prusa_connect_sdk_printer-0.8.0/tests/test_conditions.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    10161 2024-03-13 14:28:17.000000 prusa_connect_sdk_printer-0.8.0/tests/test_download.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1152 2023-05-24 08:47:29.000000 prusa_connect_sdk_printer-0.8.0/tests/test_errors.py
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)     1229 2024-05-15 08:39:53.000000 prusa_connect_sdk_printer-0.8.0/tests/test_events.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)    23077 2023-10-09 12:40:14.000000 prusa_connect_sdk_printer-0.8.0/tests/test_files.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)     1368 2024-03-06 13:27:28.000000 prusa_connect_sdk_printer-0.8.0/tests/test_mmu.py
+-rw-rw-r--   0 mcbig     (1000) mcbig     (1000)    46369 2024-05-15 08:39:53.000000 prusa_connect_sdk_printer-0.8.0/tests/test_printer.py
+-rw-r--r--   0 mcbig     (1000) mcbig     (1000)      560 2024-05-14 12:03:30.000000 prusa_connect_sdk_printer-0.8.0/tests/test_telemetry.py
```

### Comparing `prusa.connect.sdk.printer-0.7.1/ChangeLog` & `prusa_connect_sdk_printer-0.8.0/ChangeLog`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 ChangeLog
 =========
+0.8.0 (2024-05-22)
+    * Send additional version headers
+    * Add printer dialog handling
+    * Stop transfers on application exit
+    * Report read timeouts differently
+    * Initial support for the new connect MMU API
+    * Add new SL types
+    * Download manager abort transter on stop_loop
 
 0.7.1 (2023-10-09)
     * Attribute ro renamed to read_only
     * Inotify using improvement
 
 0.7.0 (2023-05-02)
     * Added new flat struct for filesystem, old one is renamed to legacy
```

### Comparing `prusa.connect.sdk.printer-0.7.1/PKG-INFO` & `prusa_connect_sdk_printer-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusa.connect.sdk.printer
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python printer library for PrusaConnect
 Home-page: https://github.com/prusa3d/Prusa-Connect-SDK-Printer
 Author: Prusa Link Developers
 Author-email: Prusa Link Developers <link@prusa3d.cz>
 Maintainer: Prusa Link Developers
 Maintainer-email: Ondřej Tůma <mcbig@zeropage.cz>, Michal Zoubek <michal.zoubek@prusa3d.cz>, Tomáš Jozífek <jozifektomas@gmail.com>
 License: Freeware
@@ -15,18 +15,19 @@
 Classifier: Natural Language :: English
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Requires-Dist: py-gcode-metadata
+Requires-Dist: py-gcode-metadata>=0.2.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: inotify_simple~=1.3.5
 Requires-Dist: mypy-extensions~=1.0.0
+Requires-Dist: urllib3<3,>=1.21.1
 
 PrusaConnect SDK for Printer
 =============================
 
 :Requirements: basic knowledge of `PrusaConnect API docs <https://connect.prusa3d.com/docs/>`_.
 
 Printer instance
```

### Comparing `prusa.connect.sdk.printer-0.7.1/README.rst` & `prusa_connect_sdk_printer-0.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/__init__.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 """Python printer library for PrusaConnect.
 
-    Copyright (C) 2023 PrusaResearch
+    Copyright (C) 2024 PrusaResearch
 """
 import configparser
 import os
 import re
 from logging import getLogger
 from queue import Empty, Queue
 from time import sleep, time
 from typing import Any, Callable, Dict, List, Optional
 
 from gcode_metadata import get_metadata
 from requests import RequestException, Response, Session  # type: ignore
 
 # pylint: disable=redefined-builtin
 from requests.exceptions import ConnectionError  # type: ignore
+from urllib3.exceptions import ReadTimeoutError  # type: ignore
 
 from . import const, errors
 from .camera_controller import CameraController
 from .clock import ClockWatcher
 from .command import Command, CommandFailed
 from .conditions import API, HTTP, INTERNET, TOKEN, CondState
+from .const import MMU_SLOT_COUNTS
 from .download import DownloadMgr, Transfer
 from .files import Filesystem, InotifyHandler, delete
 from .models import (
     CameraRegister,
     Event,
     LoopObject,
     Register,
     Sheet,
     Telemetry,
 )
 from .util import RetryingSession, get_timestamp
 
-__version__ = "0.7.1"
-__date__ = "9 Oct 2023"  # version date
-__copyright__ = "(c) 2023 Prusa 3D"
+__version__ = "0.8.0"
+__date__ = "22 May 2024"  # version date
+__copyright__ = "(c) 2024 Prusa 3D"
 __author_name__ = "Prusa Link Developers"
 __author_email__ = "link@prusa3d.cz"
 __author__ = f"{__author_name__} <{__author_email__}>"
 __description__ = "Python printer library for PrusaConnect"
 
 __credits__ = "Ondřej Tůma, Martin Užák, Michal Zoubek, Tomáš Jozífek"
 __url__ = "https://github.com/prusa3d/Prusa-Connect-SDK-Printer"
@@ -76,25 +78,30 @@
     # pylint: disable=too-many-public-methods
 
     queue: "Queue[LoopObject]"
     server: Optional[str] = None
     token: Optional[str] = None
     conn: Session
 
+    # Printer firmware version
+    firmware: Optional[str] = None
+    # Software version if is different to printer version
+    software: Optional[str] = None
+
     NOT_INITIALISED_MSG = "Printer has not been initialized properly"
 
     def __init__(self,
                  type_: Optional[const.PrinterType] = None,
                  sn: Optional[str] = None,
                  fingerprint: Optional[str] = None,
-                 max_retries: int = 1):
+                 max_retries: int = 1,
+                 mmu_supported: bool = True):
         self.__type = type_
         self.__sn = sn
         self.__fingerprint = fingerprint
-        self.firmware = None
         self.network_info = {
             "lan_mac": None,
             "lan_ipv4": None,
             "lan_ipv6": None,
             "wifi_mac": None,
             "wifi_ipv4": None,
             "wifi_ipv6": None,
@@ -108,25 +115,30 @@
 
         self.__ready: bool = False
         self.__state: const.State = const.State.BUSY
         self.job_id: Optional[int] = None
         self.mbl: Optional[List[float]] = None
         self.sheet_settings: Optional[List[Sheet]] = None
         self.active_sheet: Optional[int] = None  # index
+        self.mmu_supported: bool = mmu_supported
+        self.mmu_enabled: bool = False
+        self.mmu_fw: Optional[str] = None
+        self.mmu_type: Optional[const.MMUType] = None
 
         if max_retries > 1:
             self.conn = RetryingSession(max_retries=max_retries)
         else:
             self.conn = Session()
 
         self.queue = Queue()
 
         self.command = Command(self.event_cb)
         self.set_handler(const.Command.SEND_INFO, self.send_info)
         self.set_handler(const.Command.SEND_FILE_INFO, self.get_file_info)
+        self.set_handler(const.Command.SEND_STATE_INFO, self.get_state_info)
         self.set_handler(const.Command.CREATE_FOLDER, self.create_folder)
         self.set_handler(const.Command.CREATE_DIRECTORY, self.create_folder)
         self.set_handler(const.Command.DELETE_FILE, self.delete_file)
         self.set_handler(const.Command.DELETE_FOLDER, self.delete_folder)
         self.set_handler(const.Command.DELETE_DIRECTORY, self.delete_folder)
         self.set_handler(const.Command.START_URL_DOWNLOAD,
                          self.start_url_download)
@@ -134,14 +146,15 @@
                          self.start_connect_download)
         self.set_handler(const.Command.STOP_TRANSFER, self.transfer_stop)
         self.set_handler(const.Command.SEND_TRANSFER_INFO, self.transfer_info)
         self.set_handler(const.Command.SET_PRINTER_READY,
                          self.set_printer_ready)
         self.set_handler(const.Command.CANCEL_PRINTER_READY,
                          self.cancel_printer_ready)
+        self.set_handler(const.Command.DIALOG_ACTION, self.dialog_action)
 
         self.fs = Filesystem(sep=os.sep, event_cb=self.event_cb)
         self.inotify_handler = InotifyHandler(self.fs)
         # Handler blocks communication with Connect in loop method!
         self.register_handler = default_register_handler
         self.__printed_file_cb = lambda: None
         self.download_finished_cb = lambda transfer: None  # noaq: ARG005
@@ -173,14 +186,19 @@
         """
         protocol = 'https' if tls else 'http'
         if port:
             return f"{protocol}://{host}:{port}"
         return f"{protocol}://{host}"
 
     @property
+    def running_loop(self):
+        """Return if loop is running (if was started but not stopped)."""
+        return self.__running_loop
+
+    @property
     def printed_file_cb(self):
         """Returns path of currently printed file"""
         return self.__printed_file_cb
 
     @printed_file_cb.setter
     def printed_file_cb(self, value):
         """Sets path of currently printed file"""
@@ -250,14 +268,17 @@
     def make_headers(self, timestamp: Optional[float] = None) -> dict:
         """Returns request headers from connection variables."""
         timestamp = get_timestamp(timestamp)
 
         headers = {
             "Fingerprint": self.fingerprint,
             "Timestamp": str(timestamp),
+            "User-Agent": f"Prusa-Connect-SDK-Printer/{__version__}",
+            "User-Agent-Printer": str(self.__type),
+            "User-Agent-Version": str(self.software or self.firmware),
         }
         if self.token:
             headers['Token'] = self.token
 
         if self.clock_watcher.clock_adjusted():
             log.debug("Clock adjustment detected. Resetting watcher")
             headers['Clock-Adjusted'] = "1"
@@ -368,15 +389,16 @@
         """Returns kwargs for Command.finish method as reaction
          to SEND_INFO."""
         # pylint: disable=unused-argument
         if self.__type is not None:
             type_, ver, sub = self.__type.value
         else:
             type_, ver, sub = (None, None, None)
-        return {
+
+        data = {
             "source": const.Source.CONNECT,
             "event": const.Event.INFO,
             "state": self.__state,
             "type": type_,
             "version": ver,
             "subversion": sub,
             "firmware": self.firmware,
@@ -387,14 +409,24 @@
             "sn": self.sn,
             "fingerprint": self.fingerprint,
             "mbl": self.mbl,
             "sheet_settings": self.sheet_settings,
             "active_sheet": self.active_sheet,
         }
 
+        if self.mmu_supported:
+            mmu: Dict[str, Any] = {"enabled": self.mmu_enabled}
+            if self.mmu_fw is not None:
+                mmu["version"] = self.mmu_fw
+            data["mmu"] = mmu
+
+            if self.mmu_type is not None and self.mmu_enabled:
+                data["slots"] = MMU_SLOT_COUNTS.get(self.mmu_type)
+        return data
+
     def send_info(self, caller: Command) -> Dict[str, Any]:
         """Accept command arguments and adapt the call for the getter"""
         # pylint: disable=unused-argument
         return self.get_info()
 
     def start_url_download(self, caller: Command) -> Dict[str, Any]:
         """Download an URL specified by url, to_select and to_print flags
@@ -475,14 +507,21 @@
         """Cancel READY state and switch printer back to IDLE"""
         # pylint: disable=unused-argument
         if self.ready:
             self.set_state(const.State.IDLE, const.Source.CONNECT, ready=False)
             return {'source': const.Source.CONNECT}
         raise ValueError("Can't cancel, printer isn't ready")
 
+    def dialog_action(self, caller: Command) -> Dict[str, Any]:
+        """Process dialog action"""
+        # pylint: disable=unused-argument
+        if not caller.kwargs:
+            raise ValueError(f"{const.Command.DIALOG_ACTION} requires kwargs")
+        return {'source': const.Source.CONNECT}
+
     def get_file_info(self, caller: Command) -> Dict[str, Any]:
         """Returns file info for a given file, if it exists."""
         # pylint: disable=unused-argument
         if not caller.kwargs or "path" not in caller.kwargs:
             raise ValueError("SEND_FILE_INFO requires kwargs")
 
         path = caller.kwargs["path"]
@@ -514,14 +553,24 @@
                             biggest = data
                     info['preview'] = biggest.decode()
         except FileNotFoundError:
             log.debug("File not found: %s", path)
 
         return info
 
+    def get_state_info(self, caller: Command) -> Dict[str, Any]:
+        """Returns state info for a given file, if it exists."""
+        # pylint: disable=unused-argument
+
+        return {
+            "source": const.Source.CONNECT,
+            "event": const.Event.STATE_CHANGED,
+            "state": self.__state,
+        }
+
     def delete_file(self, caller: Command) -> Dict[str, Any]:
         """Handler for delete a file."""
         if not caller.kwargs or "path" not in caller.kwargs:
             raise ValueError(f"{caller.command_name} requires kwargs")
 
         if self.fs.get(caller.kwargs["path"]).to_dict()["read_only"]:
             raise ValueError("File is read only")
@@ -583,14 +632,15 @@
 
         .. code:: python
 
             @printer.command(const.GCODE)
             def gcode(prn, gcode):
                 ...
         """
+
         def wrapper(handler: Callable[[Command], Dict[str, Any]]):
             self.set_handler(command, handler)
             return handler
 
         return wrapper
 
     def parse_command(self, res: Response):
@@ -675,15 +725,15 @@
             API.state = CondState.NOK
             if res.status_code >= 500:
                 errors.HTTP.ok = False
                 HTTP.state = CondState.NOK
             else:
                 errors.HTTP.ok = True
                 HTTP.state = CondState.OK
-            log.debug("Status code: {res.status_code}")
+            log.debug("Status code: %d", res.status_code)
             raise RuntimeError(res.text)
 
         self.code = res.headers["Code"]
         self.queue.put(Register(self.code))
         errors.API.ok = True
         API.state = CondState.OK
         return self.code
@@ -734,14 +784,18 @@
             log.warning("No token, skipping item: %s", item)
             return
 
         # Send it
         headers = self.make_headers(item.timestamp)
         try:
             res = item.send(self.conn, self.server, headers)
+        except ReadTimeoutError as err:
+            errors.HTTP.ok = False
+            HTTP.state = CondState.NOK
+            log.error("Experiencing connect communication problems - %s", err)
         except ConnectionError as err:
             errors.HTTP.ok = False
             HTTP.state = CondState.NOK
             log.error(err)
         except RequestException as err:
             errors.INTERNET.ok = False
             INTERNET.state = CondState.NOK
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_configurator.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_configurator.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_controller.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_controller.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/camera_driver.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/camera_driver.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/clock.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/clock.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/command.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/command.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/conditions.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/conditions.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     OK = True
     NOK = False
 
 
 # pylint: disable=too-many-arguments
 class Condition:
     """A more detailed condition for state tracking"""
+
     def __init__(self,
                  name: str,
                  long_msg: str,
                  parent: Optional[Condition] = None,
                  short_msg: Optional[str] = None,
                  priority: int = 0):
         self.name: str = name
@@ -155,26 +156,26 @@
         return self._state is CondState.OK
 
     def __str__(self):
         return f"{self.name}: {self._state.name}"
 
     def __iter__(self):
         for child in self._children:
-            for child_iter in child:
-                yield child_iter
+            yield from child
         yield self
 
 
 class ConditionTracker:
     """
     Tracks the NOK conditions and their priorities
 
     The time complexity is O(n), but the number of
     items is expected to be low
     """
+
     def __init__(self) -> None:
         self._nok_conditions: Set[Condition] = set()
         self._tracked_conditions: Set[Condition] = set()
         self._cached_worst = None
 
     def add_tracked_condition_tree(self, root_condition: Condition):
         """Add a tree of conditions to be tracked"""
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/const.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/const.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,23 +47,33 @@
 class PrinterType(Enum):
     """Printer Type"""
     I3MK25 = (1, 2, 5)
     I3MK25S = (1, 2, 6)
     I3MK3 = (1, 3, 0)
     I3MK3S = (1, 3, 1)
     SL1 = (5, 1, 0)
-    TRILAB_DQ2 = (6, 2, 0)
-    TRILAB_DQ2P = (6, 2, 1)
-    TRILAB_AQI = (7, 2, 0)
+    SL1S = (5, 1, 1)
+    M1 = (5, 2, 0)
+    HT90 = (6, 1, 0)
 
     def __str__(self):
         # pylint: disable=not-an-iterable
         return '.'.join(str(i) for i in self.value)
 
 
+class MMUType(Enum):
+    """MMU Type"""
+    MMU3 = "MMU3"
+
+
+MMU_SLOT_COUNTS: Dict[MMUType, int] = {
+    MMUType.MMU3: 5,
+}
+
+
 class StorageType(Enum):
     """Storage Type"""
     LOCAL = 'LOCAL'
     SDCARD = 'SDCARD'
     USB = 'USB'
 
 
@@ -85,26 +95,29 @@
     TRANSFER_INFO = "TRANSFER_INFO"
     MESH_BED_DATA = "MESH_BED_DATA"
 
     TRANSFER_ABORTED = "TRANSFER_ABORTED"
     TRANSFER_STOPPED = "TRANSFER_STOPPED"
     TRANSFER_FINISHED = "TRANSFER_FINISHED"
 
+    SLOT_EVENT = "SLOT_EVENT"
+
 
 class Source(Enum):
     """Printer event source."""
     CONNECT = "CONNECT"
     GUI = "GUI"
     WUI = "WUI"
     SERIAL = "SERIAL"
     GCODE = "GCODE"
     MARLIN = "MARLIN"
     FIRMWARE = "FIRMWARE"
     HW = "HW"
     USER = "USER"
+    SLOT = "SLOT"
 
 
 class Command(Enum):
     """Commands which could be sent by Connect."""
     SEND_INFO = "SEND_INFO"
     GCODE = "GCODE"
 
@@ -116,28 +129,31 @@
     SEND_FILE_INFO = "SEND_FILE_INFO"
     DELETE_FILE = "DELETE_FILE"
     DELETE_FOLDER = "DELETE_FOLDER"
     DELETE_DIRECTORY = "DELETE_DIRECTORY"
     CREATE_FOLDER = "CREATE_FOLDER"
     CREATE_DIRECTORY = "CREATE_DIRECTORY"
     SEND_JOB_INFO = "SEND_JOB_INFO"
+    SEND_STATE_INFO = "SEND_STATE_INFO"
 
     UPGRADE = "UPGRADE"
     RESET_PRINTER = "RESET_PRINTER"
 
     START_URL_DOWNLOAD = "START_URL_DOWNLOAD"
     START_CONNECT_DOWNLOAD = "START_CONNECT_DOWNLOAD"
     SEND_TRANSFER_INFO = "SEND_TRANSFER_INFO"
     STOP_TRANSFER = "STOP_TRANSFER"
 
     SET_PRINTER_READY = "SET_PRINTER_READY"
     CANCEL_PRINTER_READY = "CANCEL_PRINTER_READY"
 
     LOAD_FILAMENT = "LOAD_FILAMENT"
     UNLOAD_FILAMENT = "UNLOAD_FILAMENT"
+    SLOT_ACTION = "SLOT_ACTION"
+    DIALOG_ACTION = "DIALOG_ACTION"
 
 
 class TransferType(Enum):
     """File transfer types"""
     NO_TRANSFER = "NO_TRANSFER"
     FROM_WEB = "FROM_WEB"  # from URL
     FROM_CONNECT = "FROM_CONNECT"  # from URL using Connect
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/download.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/download.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,15 +395,16 @@
         """Execute the download and store the file in `self.tmp_filename()`"""
         self.transfer.start_ts = time.time()
         server, self.headers = self.conn_details_cb()
 
         # server is not connect server, set token to None
         if not server or \
                 not self.transfer.url.lower().startswith(server.lower()):
-            self.headers = {}
+            user_agent = self.headers.get("User-Agent")
+            self.headers = {"User-Agent": user_agent}
 
         res = requests.get(self.transfer.url,
                            stream=True,
                            headers=self.headers,
                            timeout=CONNECTION_TIMEOUT)
 
         if res.status_code != 200:
@@ -423,14 +424,16 @@
                   self.transfer.url)
 
         with open(self.tmp_filename(), 'wb') as f:
             self.event_cb(Event.TRANSFER_INFO, Source.WUI, **self.info())
             for data in res.iter_content(chunk_size=self.buffer_size):
                 if self.transfer.stop_ts > 0:
                     raise TransferStoppedError("Transfer was stopped")
+                if not self._running_loop:
+                    raise TransferAbortedError("Transfer was aborted")
                 f.write(data)
                 if self.throttle:
                     time.sleep(self.throttle)
                 self.transfer.transferred += len(data)
 
         if not self.transfer.transferred:
             raise TransferAbortedError("Empty response")
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/errors.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/errors.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/files.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/files.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/models.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -122,33 +122,39 @@
                  source: const.Source,
                  timestamp: Optional[float] = None,
                  command_id: Optional[int] = None,
                  job_id: Optional[int] = None,
                  transfer_id: Optional[int] = None,
                  reason: Optional[str] = None,
                  state: Optional[const.State] = None,
+                 dialog_id: Optional[int] = None,
                  **kwargs):
         super().__init__(timestamp=timestamp)
         self.event = event
         self.source = source
         self.command_id = command_id
         self.job_id = job_id
         self.transfer_id = transfer_id
         self.reason = reason
         self.state = state
+        self.dialog_id = dialog_id
         self.data = kwargs
 
     def to_payload(self):
         """Send event to connect."""
         data = {
             "event": self.event.value,
             "source": self.source.value,
             "data": filter_null(self.data),
         }
-        for attr in ('command_id', 'job_id', 'transfer_id', 'reason'):
+        for attr in ('command_id',
+                     'job_id',
+                     'transfer_id',
+                     'reason',
+                     'dialog_id'):
             value = getattr(self, attr)
             if value:
                 data[attr] = value
         if self.state:
             data["state"] = self.state.value
 
         return data
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa/connect/printer/util.py` & `prusa_connect_sdk_printer-0.8.0/prusa/connect/printer/util.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/PKG-INFO` & `prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prusa.connect.sdk.printer
-Version: 0.7.1
+Version: 0.8.0
 Summary: Python printer library for PrusaConnect
 Home-page: https://github.com/prusa3d/Prusa-Connect-SDK-Printer
 Author: Prusa Link Developers
 Author-email: Prusa Link Developers <link@prusa3d.cz>
 Maintainer: Prusa Link Developers
 Maintainer-email: Ondřej Tůma <mcbig@zeropage.cz>, Michal Zoubek <michal.zoubek@prusa3d.cz>, Tomáš Jozífek <jozifektomas@gmail.com>
 License: Freeware
@@ -15,18 +15,19 @@
 Classifier: Natural Language :: English
 Classifier: License :: Freeware
 Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst
-Requires-Dist: py-gcode-metadata
+Requires-Dist: py-gcode-metadata>=0.2.0
 Requires-Dist: requests>=2.31.0
 Requires-Dist: inotify_simple~=1.3.5
 Requires-Dist: mypy-extensions~=1.0.0
+Requires-Dist: urllib3<3,>=1.21.1
 
 PrusaConnect SDK for Printer
 =============================
 
 :Requirements: basic knowledge of `PrusaConnect API docs <https://connect.prusa3d.com/docs/>`_.
 
 Printer instance
```

### Comparing `prusa.connect.sdk.printer-0.7.1/prusa.connect.sdk.printer.egg-info/SOURCES.txt` & `prusa_connect_sdk_printer-0.8.0/prusa.connect.sdk.printer.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -29,11 +29,12 @@
 tests/test_clock.py
 tests/test_command.py
 tests/test_conditions.py
 tests/test_download.py
 tests/test_errors.py
 tests/test_events.py
 tests/test_files.py
+tests/test_mmu.py
 tests/test_printer.py
 tests/test_telemetry.py
 tests/gcodes/metadata/.hidden_fdn_filename.gcode
 tests/gcodes/metadata/fdn_filename.gcode
```

### Comparing `prusa.connect.sdk.printer-0.7.1/pyproject.toml` & `prusa_connect_sdk_printer-0.8.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/setup.py` & `prusa_connect_sdk_printer-0.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/sl.py` & `prusa_connect_sdk_printer-0.8.0/sl.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/gcodes/metadata/.hidden_fdn_filename.gcode` & `prusa_connect_sdk_printer-0.8.0/tests/gcodes/metadata/.hidden_fdn_filename.gcode`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/gcodes/metadata/fdn_filename.gcode` & `prusa_connect_sdk_printer-0.8.0/tests/gcodes/metadata/fdn_filename.gcode`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_cameras.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_cameras.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,26 +16,24 @@
 from prusa.connect.printer.const import (
     CapabilityType,
     DriverError,
     NotSupported,
     TriggerScheme,
 )
 from prusa.connect.printer.models import CameraRegister
-from tests.util import SERVER, printer, run_loop
-
-# Shut up flake8, I'm importing a fixture!
-assert printer  # type: ignore
+from tests.util import SERVER, run_loop
 
 
 class DummyDriver(CameraDriver):
     """It's a dummy driver for testing"""
 
     name = "Humpty Dumpty"
     REQUIRES_SETTINGS = MappingProxyType({
-        "parameter": "A placeholder parameter for testing",
+        "parameter":
+        "A placeholder parameter for testing",
     })
 
     # Allows changes for tests with newly detected cameras
     scanned_cameras: ClassVar[dict] = {
         "id1": {
             "name": "Bad Camera 1",
             "parameter": "very parametric",
```

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_clock.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_clock.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,12 @@
 from func_timeout import FunctionTimedOut, func_timeout  # type: ignore
 
 from prusa.connect.printer import const
 from prusa.connect.printer.clock import ClockWatcher
 
-from .util import printer
-
-assert printer  # type: ignore
-
 
 def adjust_clock(clock_watcher):
     """Helper to mock adjusting the clock in `clock_watcher`"""
     clock_watcher.delta += (ClockWatcher.TOLERANCE + 1)
 
 
 def test_clock_adjusted():
```

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_command.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_conditions.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_download.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_download.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,24 +7,19 @@
 import time
 
 import pytest
 import responses
 
 from prusa.connect.printer import Telemetry, const
 
-from .util import printer
-
-assert printer  # type: ignore
-
 # pylint: disable=missing-function-docstring
-# pylint: disable=redefined-outer-name
 
-GCODE_URL = "https://media.prusaprinters.org/media/prints/27216/gcodes/" + \
-            "272161_a9977cd4-cc70-4fb3-8d09-276a023b132d/" + \
-            "cam_clip_3_015mm_pla_mk3s_2h13m.gcode"
+GCODE_URL = ("https://files.printables.com/media/prints/27216/gcodes/"
+             "272161_a9977cd4-cc70-4fb3-8d09-276a023b132d/"
+             "cam_clip_3_015mm_pla_mk3s_2h13m.gcode")
 DST = '/sdcard/my_example.gcode'
 
 
 @responses.activate
 @pytest.fixture
 def gcode(printer):
     # pylint: disable=unused-argument
@@ -42,17 +37,18 @@
     printer.fs.from_dir(tmp_dir.name, 'sdcard')
     yield printer.download_mgr
 
     shutil.rmtree(tmp_dir.name)
 
 
 def run_test_loop(download_mgr, timeout=.1, unset_stop=False):
+
     def fullstop():
-        download_mgr.transfer.stop()
         if unset_stop:
+            download_mgr.transfer.stop()
             download_mgr.transfer.stop_ts = 0
         download_mgr._running_loop = False
 
     t = threading.Timer(timeout, fullstop)
     t.start()
 
     download_mgr.loop()
@@ -116,14 +112,15 @@
                        DST,
                        GCODE_URL,
                        to_print=False,
                        to_select=False)
     transfer = download_mgr.transfer
     download_mgr.buffer_size = 1
     run_test_loop(download_mgr)
+    download_mgr.transfer.stop()
 
     assert transfer.time_remaining() == 0
 
 
 def test_download_info(gcode, download_mgr):
     info = download_mgr.start(const.TransferType.FROM_WEB,
                               DST,
```

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_errors.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_events.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_events.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,13 +26,15 @@
 
 def test_kwargs():
     event = Event(const.Event.STATE_CHANGED,
                   const.Source.WUI,
                   command_id=42,
                   job_id=12,
                   reason="Chuck Norris",
-                  state=const.State.FINISHED)
+                  state=const.State.FINISHED,
+                  dialog_id=33)
     payload = event.to_payload()
     assert payload['command_id'] == 42
     assert payload['job_id'] == 12
     assert payload['reason'] == "Chuck Norris"
     assert payload['state'] == "FINISHED"
+    assert payload['dialog_id'] == 33
```

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_files.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_printer.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_printer.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,25 +17,20 @@
 from tests.util import (
     CONNECT_HOST,
     CONNECT_PORT,
     FINGERPRINT,
     SERVER,
     SN,
     TOKEN,
-    printer,
     run_loop,
 )
 
 # pylint: disable=missing-function-docstring
-# pylint: disable=redefined-outer-name
 # pylint: disable=too-many-lines
 
-# Shut up flake8, I'm importing a fixture!
-assert printer  # type: ignore
-
 MAC = "00:01:02:03:04:05"
 FIRMWARE = "3.9.0rc2"
 IP = "192.168.1.101"
 TYPE = const.TransferType.FROM_WEB
 
 
 @pytest.fixture(scope="session")
@@ -99,14 +94,15 @@
     printer.attach(tmp_dir.name, "sdcard")
     printer.queue.get_nowait()  # consume MEDIUM_INSERTED event
     yield printer
 
 
 class TestPrinter:
     """Tests for Printer class."""
+
     def test_init(self, printer):
         assert printer
 
         assert printer.is_initialised()
         with pytest.raises(RuntimeError):
             printer.fingerprint = "foo"
 
@@ -127,14 +123,36 @@
     def test_telemetry(self, printer):
         printer.telemetry()
         item = printer.queue.get_nowait()
 
         assert isinstance(item, Telemetry)
         assert item.to_payload() == {'state': 'BUSY'}
 
+    def test_telemetry_headers(self, requests_mock, printer):
+        requests_mock.post(SERVER + "/p/telemetry", status_code=204)
+        printer.telemetry()
+
+        headers = printer.make_headers()
+        assert headers["Fingerprint"] == printer.fingerprint
+        assert headers["User-Agent"].startswith("Prusa-Connect-SDK-Printer/")
+        assert headers["User-Agent-Printer"] == str(printer.type)
+        assert headers["User-Agent-Version"] == printer.software
+        assert headers["Token"] == printer.token
+
+        item = printer.queue.get_nowait()
+        item.send(printer.conn, printer.server, headers)
+
+        req = requests_mock.request_history[0]
+        assert str(req) == f"POST {SERVER}/p/telemetry"
+        assert req.headers["Fingerprint"] == printer.fingerprint
+        assert req.headers["User-Agent"] == headers["User-Agent"]
+        assert req.headers["User-Agent-Printer"] == str(printer.type)
+        assert req.headers["User-Agent-Version"] == printer.software
+        assert req.headers["Token"] == printer.token
+
     def test_telemetry_no_fingerprint(self, printer_no_fp):
         printer_no_fp.telemetry(temp_bed=1, temp_nozzle=2)
         item = printer_no_fp.queue.get_nowait()
         assert isinstance(item, Telemetry)
         assert item.to_payload() == {'state': 'BUSY'}
 
     def test_parse_command_no_fingerprint(self, printer_no_fp):
@@ -219,22 +237,24 @@
 
         assert errors.INTERNET.ok is True
         assert INTERNET.state is CondState.OK
         assert errors.HTTP.ok is False
         assert HTTP.state is CondState.NOK
 
     def test_set_handler(self, printer):
+
         def send_info(caller: Command) -> Any:
             assert caller.args
 
         printer.set_handler(const.Command.SEND_INFO, send_info)
         # pylint: disable=comparison-with-callable
         assert printer.command.handlers[const.Command.SEND_INFO] == send_info
 
     def test_decorator(self, printer):
+
         @printer.handler(const.Command.GCODE)
         def gcode(caller: Command) -> None:
             assert caller.args
 
         # pylint: disable=comparison-with-callable
         assert printer.command.handlers[const.Command.GCODE] == gcode
```

### Comparing `prusa.connect.sdk.printer-0.7.1/tests/test_telemetry.py` & `prusa_connect_sdk_printer-0.8.0/tests/test_telemetry.py`

 * *Files identical despite different names*

