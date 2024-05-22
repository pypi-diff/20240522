# Comparing `tmp/robotframework-zoomba-4.0.0.tar.gz` & `tmp/robotframework_zoomba-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robotframework-zoomba-4.0.0.tar", last modified: Tue Mar 26 14:31:18 2024, max compression
+gzip compressed data, was "robotframework_zoomba-4.0.1.tar", last modified: Mon Apr 29 16:04:14 2024, max compression
```

## Comparing `robotframework-zoomba-4.0.0.tar` & `robotframework_zoomba-4.0.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.705246 robotframework-zoomba-4.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/docs/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.705246 robotframework-zoomba-4.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/src/Zoomba/
--rw-r--r--   0 runner    (1001) docker     (127)    31523 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/APILibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)      224 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/DesktopLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/GUILibrary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/src/Zoomba/Helpers/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/Helpers/ReactSelect.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/Helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/MobileLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/SOAPLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/ZoombaError.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/src/Zoomba/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-03-26 14:31:18.000000 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-03-26 14:31:18.000000 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 14:31:18.000000 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-03-26 14:31:18.000000 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-26 14:31:18.000000 robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 14:31:18.709246 robotframework-zoomba-4.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/test/test_zoomba_error.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-03-26 14:31:11.000000 robotframework-zoomba-4.0.0/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.438434 robotframework_zoomba-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 16:04:14.438434 robotframework_zoomba-4.0.1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.434434 robotframework_zoomba-4.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     7132 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/docs/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 16:04:14.438434 robotframework_zoomba-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.430434 robotframework_zoomba-4.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.434434 robotframework_zoomba-4.0.1/src/Zoomba/
+-rw-r--r--   0 runner    (1001) docker     (127)    31523 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/APILibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)      224 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/DesktopLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22847 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/GUILibrary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.434434 robotframework_zoomba-4.0.1/src/Zoomba/Helpers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/Helpers/ReactSelect.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/Helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/MobileLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/SOAPLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/ZoombaError.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/src/Zoomba/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.434434 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8443 2024-04-29 16:04:14.000000 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-29 16:04:14.000000 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 16:04:14.000000 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-29 16:04:14.000000 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-29 16:04:14.000000 robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 16:04:14.434434 robotframework_zoomba-4.0.1/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/test/test_zoomba_error.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-29 16:04:10.000000 robotframework_zoomba-4.0.1/version.py
```

### Comparing `robotframework-zoomba-4.0.0/LICENSE` & `robotframework_zoomba-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/PKG-INFO` & `robotframework_zoomba-4.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-zoomba
-Version: 4.0.0
+Version: 4.0.1
 Summary: Robot Framework mini-framework.
 Home-page: https://github.com/Accruent/zoomba
 Maintainer: Alex Calandra, Michael Hintz, Keith Smoland, Matthew Giardina, Brandon Wolfe, Neil Howell, Tommy Hoang
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium requests appium soap winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibrary api-rest api soap-api appium-mobile mobile
 Platform: any
@@ -12,19 +12,19 @@
 Classifier:         Operating System :: OS Independent
 Classifier:         Programming Language :: Python :: 3
 Classifier:         Topic :: Software Development :: Testing
 Classifier:         Framework :: Robot Framework :: Library
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: robotframework==7.0
-Requires-Dist: robotframework-requests==0.9.6
-Requires-Dist: robotframework-seleniumlibrary==6.2.0
+Requires-Dist: robotframework-requests==0.9.7
+Requires-Dist: robotframework-seleniumlibrary==6.3.0
 Requires-Dist: robotframework-sudslibrary-aljcalandra==1.1.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: selenium==4.18.1
+Requires-Dist: selenium==4.20.0
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pandas>=1.3.5
 Provides-Extra: testing
 Requires-Dist: mock; extra == "testing"
 
 RobotFramework-Zoomba
 ===========
```

### Comparing `robotframework-zoomba-4.0.0/docs/README.md` & `robotframework_zoomba-4.0.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/setup.py` & `robotframework_zoomba-4.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/Zoomba/APILibrary.py` & `robotframework_zoomba-4.0.1/src/Zoomba/APILibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/Zoomba/GUILibrary.py` & `robotframework_zoomba-4.0.1/src/Zoomba/GUILibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/Zoomba/Helpers/ReactSelect.py` & `robotframework_zoomba-4.0.1/src/Zoomba/Helpers/ReactSelect.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/Zoomba/SOAPLibrary.py` & `robotframework_zoomba-4.0.1/src/Zoomba/SOAPLibrary.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/Zoomba/ZoombaError.py` & `robotframework_zoomba-4.0.1/src/Zoomba/ZoombaError.py`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/PKG-INFO` & `robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotframework-zoomba
-Version: 4.0.0
+Version: 4.0.1
 Summary: Robot Framework mini-framework.
 Home-page: https://github.com/Accruent/zoomba
 Maintainer: Alex Calandra, Michael Hintz, Keith Smoland, Matthew Giardina, Brandon Wolfe, Neil Howell, Tommy Hoang
 Maintainer-email: robosquad@accruent.com
 License: GPL-3.0
 Keywords: Robot Framework robot-framework selenium requests appium soap winappdriver appium robotframeworkdesktop windows zoomba python robotframework-library appium-windows appiumlibrary api-rest api soap-api appium-mobile mobile
 Platform: any
@@ -12,19 +12,19 @@
 Classifier:         Operating System :: OS Independent
 Classifier:         Programming Language :: Python :: 3
 Classifier:         Topic :: Software Development :: Testing
 Classifier:         Framework :: Robot Framework :: Library
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: robotframework==7.0
-Requires-Dist: robotframework-requests==0.9.6
-Requires-Dist: robotframework-seleniumlibrary==6.2.0
+Requires-Dist: robotframework-requests==0.9.7
+Requires-Dist: robotframework-seleniumlibrary==6.3.0
 Requires-Dist: robotframework-sudslibrary-aljcalandra==1.1.4
 Requires-Dist: requests==2.31.0
-Requires-Dist: selenium==4.18.1
+Requires-Dist: selenium==4.20.0
 Requires-Dist: python-dateutil>=2.8.2
 Requires-Dist: pandas>=1.3.5
 Provides-Extra: testing
 Requires-Dist: mock; extra == "testing"
 
 RobotFramework-Zoomba
 ===========
```

### Comparing `robotframework-zoomba-4.0.0/src/robotframework_zoomba.egg-info/SOURCES.txt` & `robotframework_zoomba-4.0.1/src/robotframework_zoomba.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `robotframework-zoomba-4.0.0/test/test_zoomba_error.py` & `robotframework_zoomba-4.0.1/test/test_zoomba_error.py`

 * *Files identical despite different names*

