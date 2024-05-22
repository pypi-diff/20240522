# Comparing `tmp/engi1020-5.1.2.tar.gz` & `tmp/engi1020-5.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "engi1020-5.1.2.tar", last modified: Tue Mar 29 11:40:27 2022, max compression
+gzip compressed data, was "engi1020-5.1.3.tar", last modified: Wed May 22 17:38:16 2024, max compression
```

## Comparing `engi1020-5.1.2.tar` & `engi1020-5.1.3.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-03-29 11:40:27.165689 engi1020-5.1.2/
--rw-r--r--   0 jon        (501) staff       (20)     1146 2022-03-29 11:40:27.165397 engi1020-5.1.2/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      609 2022-01-04 13:56:31.000000 engi1020-5.1.2/README.rst
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-03-29 11:40:27.147207 engi1020-5.1.2/engi1020/
--rw-r--r--   0 jon        (501) staff       (20)        0 2022-01-04 13:56:31.000000 engi1020-5.1.2/engi1020/__init__.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-03-29 11:40:27.164545 engi1020-5.1.2/engi1020/arduino/
--rw-r--r--   0 jon        (501) staff       (20)      669 2022-01-18 12:52:07.000000 engi1020-5.1.2/engi1020/arduino/__init__.py
--rw-r--r--   0 jon        (501) staff       (20)     1624 2022-03-29 11:39:22.000000 engi1020-5.1.2/engi1020/arduino/api.py
--rw-r--r--   0 jon        (501) staff       (20)     3522 2022-01-18 13:17:16.000000 engi1020-5.1.2/engi1020/arduino/cli.py
--rw-r--r--   0 jon        (501) staff       (20)      300 2022-03-08 19:43:21.000000 engi1020-5.1.2/engi1020/arduino/dht11.py
--rw-r--r--   0 jon        (501) staff       (20)      337 2022-03-29 11:39:22.000000 engi1020-5.1.2/engi1020/arduino/heart_rate.py
--rw-r--r--   0 jon        (501) staff       (20)     2521 2022-03-08 19:43:21.000000 engi1020-5.1.2/engi1020/arduino/io.py
--rw-r--r--   0 jon        (501) staff       (20)     1032 2022-03-29 11:39:22.000000 engi1020-5.1.2/engi1020/arduino/joystick.py
--rw-r--r--   0 jon        (501) staff       (20)      939 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/oled.py
--rw-r--r--   0 jon        (501) staff       (20)      412 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/pressure.py
--rw-r--r--   0 jon        (501) staff       (20)      948 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/rgb_lcd.py
--rw-r--r--   0 jon        (501) staff       (20)      938 2022-03-29 11:39:22.000000 engi1020-5.1.2/engi1020/arduino/rgb_led.py
--rw-r--r--   0 jon        (501) staff       (20)     5518 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/serial.py
--rw-r--r--   0 jon        (501) staff       (20)      282 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/servo.py
--rw-r--r--   0 jon        (501) staff       (20)     2231 2022-01-21 17:30:49.000000 engi1020-5.1.2/engi1020/arduino/shell.py
--rw-r--r--   0 jon        (501) staff       (20)      840 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/testing.py
--rw-r--r--   0 jon        (501) staff       (20)      741 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/three_axis_accel.py
--rw-r--r--   0 jon        (501) staff       (20)     1054 2022-01-18 12:52:07.000000 engi1020-5.1.2/engi1020/arduino/tlv.py
--rw-r--r--   0 jon        (501) staff       (20)     1303 2022-01-18 12:52:07.000000 engi1020-5.1.2/engi1020/arduino/tracing.py
--rw-r--r--   0 jon        (501) staff       (20)      325 2022-03-14 22:29:58.000000 engi1020-5.1.2/engi1020/arduino/ultra_distance.py
--rw-r--r--   0 jon        (501) staff       (20)       32 2022-01-04 13:56:31.000000 engi1020-5.1.2/engi1020/plotting.py
-drwxr-xr-x   0 jon        (501) staff       (20)        0 2022-03-29 11:40:27.150367 engi1020-5.1.2/engi1020.egg-info/
--rw-r--r--   0 jon        (501) staff       (20)     1146 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/PKG-INFO
--rw-r--r--   0 jon        (501) staff       (20)      782 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/SOURCES.txt
--rw-r--r--   0 jon        (501) staff       (20)        1 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/dependency_links.txt
--rw-r--r--   0 jon        (501) staff       (20)       72 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/entry_points.txt
--rw-r--r--   0 jon        (501) staff       (20)       48 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/requires.txt
--rw-r--r--   0 jon        (501) staff       (20)        9 2022-03-29 11:40:26.000000 engi1020-5.1.2/engi1020.egg-info/top_level.txt
--rw-r--r--   0 jon        (501) staff       (20)       38 2022-03-29 11:40:27.165874 engi1020-5.1.2/setup.cfg
--rw-r--r--   0 jon        (501) staff       (20)      913 2022-03-29 11:39:59.000000 engi1020-5.1.2/setup.py
+drwxr-xr-x   0 jon        (504) staff       (20)        0 2024-05-22 17:38:16.803757 engi1020-5.1.3/
+-rw-r--r--   0 jon        (504) staff       (20)     1230 2024-05-22 17:38:16.803544 engi1020-5.1.3/PKG-INFO
+-rw-r--r--   0 jon        (504) staff       (20)      609 2022-01-04 13:56:31.000000 engi1020-5.1.3/README.rst
+drwxr-xr-x   0 jon        (504) staff       (20)        0 2024-05-22 17:38:16.797681 engi1020-5.1.3/engi1020/
+-rw-r--r--   0 jon        (504) staff       (20)        0 2022-01-04 13:56:31.000000 engi1020-5.1.3/engi1020/__init__.py
+drwxr-xr-x   0 jon        (504) staff       (20)        0 2024-05-22 17:38:16.803017 engi1020-5.1.3/engi1020/arduino/
+-rw-r--r--   0 jon        (504) staff       (20)      669 2022-01-18 12:52:07.000000 engi1020-5.1.3/engi1020/arduino/__init__.py
+-rw-r--r--   0 jon        (504) staff       (20)     1624 2022-03-29 11:39:22.000000 engi1020-5.1.3/engi1020/arduino/api.py
+-rw-r--r--   0 jon        (504) staff       (20)     3522 2022-01-18 13:17:16.000000 engi1020-5.1.3/engi1020/arduino/cli.py
+-rw-r--r--   0 jon        (504) staff       (20)      300 2022-03-08 19:43:21.000000 engi1020-5.1.3/engi1020/arduino/dht11.py
+-rw-r--r--   0 jon        (504) staff       (20)      337 2022-03-29 11:39:22.000000 engi1020-5.1.3/engi1020/arduino/heart_rate.py
+-rw-r--r--   0 jon        (504) staff       (20)     2521 2022-03-08 19:43:21.000000 engi1020-5.1.3/engi1020/arduino/io.py
+-rw-r--r--   0 jon        (504) staff       (20)     1032 2022-03-29 11:39:22.000000 engi1020-5.1.3/engi1020/arduino/joystick.py
+-rw-r--r--   0 jon        (504) staff       (20)      939 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/oled.py
+-rw-r--r--   0 jon        (504) staff       (20)      412 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/pressure.py
+-rw-r--r--   0 jon        (504) staff       (20)      948 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/rgb_lcd.py
+-rw-r--r--   0 jon        (504) staff       (20)      938 2022-03-29 11:39:22.000000 engi1020-5.1.3/engi1020/arduino/rgb_led.py
+-rw-r--r--   0 jon        (504) staff       (20)     5521 2024-05-22 17:12:08.000000 engi1020-5.1.3/engi1020/arduino/serial.py
+-rw-r--r--   0 jon        (504) staff       (20)      282 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/servo.py
+-rw-r--r--   0 jon        (504) staff       (20)     2231 2022-01-21 17:30:49.000000 engi1020-5.1.3/engi1020/arduino/shell.py
+-rw-r--r--   0 jon        (504) staff       (20)      840 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/testing.py
+-rw-r--r--   0 jon        (504) staff       (20)      741 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/three_axis_accel.py
+-rw-r--r--   0 jon        (504) staff       (20)     1054 2022-01-18 12:52:07.000000 engi1020-5.1.3/engi1020/arduino/tlv.py
+-rw-r--r--   0 jon        (504) staff       (20)     1303 2022-01-18 12:52:07.000000 engi1020-5.1.3/engi1020/arduino/tracing.py
+-rw-r--r--   0 jon        (504) staff       (20)      325 2022-03-14 22:29:58.000000 engi1020-5.1.3/engi1020/arduino/ultra_distance.py
+-rw-r--r--   0 jon        (504) staff       (20)       32 2022-01-04 13:56:31.000000 engi1020-5.1.3/engi1020/plotting.py
+drwxr-xr-x   0 jon        (504) staff       (20)        0 2024-05-22 17:38:16.803301 engi1020-5.1.3/engi1020.egg-info/
+-rw-r--r--   0 jon        (504) staff       (20)     1230 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/PKG-INFO
+-rw-r--r--   0 jon        (504) staff       (20)      782 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/SOURCES.txt
+-rw-r--r--   0 jon        (504) staff       (20)        1 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/dependency_links.txt
+-rw-r--r--   0 jon        (504) staff       (20)       53 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/entry_points.txt
+-rw-r--r--   0 jon        (504) staff       (20)       48 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/requires.txt
+-rw-r--r--   0 jon        (504) staff       (20)        9 2024-05-22 17:38:16.000000 engi1020-5.1.3/engi1020.egg-info/top_level.txt
+-rw-r--r--   0 jon        (504) staff       (20)       38 2024-05-22 17:38:16.803861 engi1020-5.1.3/setup.cfg
+-rw-r--r--   0 jon        (504) staff       (20)      913 2024-05-22 17:14:05.000000 engi1020-5.1.3/setup.py
```

### Comparing `engi1020-5.1.2/PKG-INFO` & `engi1020-5.1.3/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: engi1020
-Version: 5.1.2
+Version: 5.1.3
 Summary: Software library for Engineering 1020: Introduction to Programming at Memorial University.
-Home-page: UNKNOWN
 Author: Jonathan Anderson, Lori Hogan
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: click
+Requires-Dist: hexdump
+Requires-Dist: matplotlib
+Requires-Dist: pyserial
+Requires-Dist: python-dotenv
 
 =======================================
 engi1020: Engineering 1020 library
 =======================================
 
 This library wraps several other libraries and re-exports them.
 This makes for a messy namespace, but that simplifies the business of importing
@@ -27,9 +30,7 @@
 The libraries (re-)imported by this library are:
 
 https://matplotlib.org/api/pyplot_api.html[`matplotlib.pyplot`]
   A plotting library using a MATLAB-like API
 
 https://pypi.org/project/nanpy[`nanpy`]
   A Python library for interacting with an Arduino board
-
-
```

### Comparing `engi1020-5.1.2/README.rst` & `engi1020-5.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/__init__.py` & `engi1020-5.1.3/engi1020/arduino/__init__.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/api.py` & `engi1020-5.1.3/engi1020/arduino/api.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/cli.py` & `engi1020-5.1.3/engi1020/arduino/cli.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/io.py` & `engi1020-5.1.3/engi1020/arduino/io.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/joystick.py` & `engi1020-5.1.3/engi1020/arduino/joystick.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/oled.py` & `engi1020-5.1.3/engi1020/arduino/oled.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/rgb_lcd.py` & `engi1020-5.1.3/engi1020/arduino/rgb_lcd.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/rgb_led.py` & `engi1020-5.1.3/engi1020/arduino/rgb_led.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/serial.py` & `engi1020-5.1.3/engi1020/arduino/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -160,15 +160,15 @@
     elif sys.platform == "win32":
         ports = list(serial.tools.list_ports.comports())
 
         if len(ports) != 1:
             print("Check Windows Device Manager for COM port number")
 
     else:
-        ports = list(serial.tools.list_ports.grep("ttyUSB[0-9]+"))
+        ports = list(serial.tools.list_ports.grep("ttyU(SB)?[0-9]+"))
 
         if len(ports) == 0:
             ports = list(serial.tools.list_ports.grep("ttyACM[0-9]+"))
 
     if len(ports) == 0:
         sys.stderr.write("No Arduino device detected (none plugged in?)\n")
         return None
```

### Comparing `engi1020-5.1.2/engi1020/arduino/shell.py` & `engi1020-5.1.3/engi1020/arduino/shell.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/testing.py` & `engi1020-5.1.3/engi1020/arduino/testing.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/three_axis_accel.py` & `engi1020-5.1.3/engi1020/arduino/three_axis_accel.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/tlv.py` & `engi1020-5.1.3/engi1020/arduino/tlv.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020/arduino/tracing.py` & `engi1020-5.1.3/engi1020/arduino/tracing.py`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/engi1020.egg-info/PKG-INFO` & `engi1020-5.1.3/engi1020.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: engi1020
-Version: 5.1.2
+Version: 5.1.3
 Summary: Software library for Engineering 1020: Introduction to Programming at Memorial University.
-Home-page: UNKNOWN
 Author: Jonathan Anderson, Lori Hogan
 License: MIT
-Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: click
+Requires-Dist: hexdump
+Requires-Dist: matplotlib
+Requires-Dist: pyserial
+Requires-Dist: python-dotenv
 
 =======================================
 engi1020: Engineering 1020 library
 =======================================
 
 This library wraps several other libraries and re-exports them.
 This makes for a messy namespace, but that simplifies the business of importing
@@ -27,9 +30,7 @@
 The libraries (re-)imported by this library are:
 
 https://matplotlib.org/api/pyplot_api.html[`matplotlib.pyplot`]
   A plotting library using a MATLAB-like API
 
 https://pypi.org/project/nanpy[`nanpy`]
   A Python library for interacting with an Arduino board
-
-
```

### Comparing `engi1020-5.1.2/engi1020.egg-info/SOURCES.txt` & `engi1020-5.1.3/engi1020.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `engi1020-5.1.2/setup.py` & `engi1020-5.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup, find_packages
 
 setup(
     name="engi1020",
-    version="5.1.2",
+    version="5.1.3",
     description="Software library for Engineering 1020: Introduction to Programming at Memorial University.",
     license="MIT",
     author="Jonathan Anderson, Lori Hogan",
     packages=find_packages(),
     entry_points='''
         [console_scripts]
         arduino=engi1020.arduino.cli:cli
```

