# Comparing `tmp/lensIQ-1.3.0.tar.gz` & `tmp/lensiq-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lensIQ-1.3.0.tar", last modified: Wed Apr 10 22:24:05 2024, max compression
+gzip compressed data, was "lensiq-1.3.1.tar", last modified: Wed May 22 18:25:31 2024, max compression
```

## Comparing `lensIQ-1.3.0.tar` & `lensiq-1.3.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.377166 lensIQ-1.3.0/
--rw-rw-rw-   0        0        0     3758 2024-01-12 23:13:24.000000 lensIQ-1.3.0/LICENSE
--rw-rw-rw-   0        0        0     6131 2024-04-10 22:24:05.373395 lensIQ-1.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     5344 2024-04-10 22:16:28.000000 lensIQ-1.3.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.296223 lensIQ-1.3.0/lensIQ/
--rw-rw-rw-   0        0        0      254 2024-01-09 19:31:09.000000 lensIQ-1.3.0/lensIQ/__init__.py
--rw-rw-rw-   0        0        0    22102 2024-01-25 19:50:47.000000 lensIQ-1.3.0/lensIQ/defaultCalData.py
--rw-rw-rw-   0        0        0    49490 2024-04-10 22:15:50.000000 lensIQ-1.3.0/lensIQ/lensIQ.py
-drwxrwxrwx   0        0        0        0 2024-04-10 22:24:05.371400 lensIQ-1.3.0/lensIQ.egg-info/
--rw-rw-rw-   0        0        0     6131 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      242 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2024-04-10 22:24:05.000000 lensIQ-1.3.0/lensIQ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      877 2024-04-10 22:16:18.000000 lensIQ-1.3.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-10 22:24:05.378169 lensIQ-1.3.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 18:25:31.533842 lensiq-1.3.1/
+-rw-rw-rw-   0        0        0     3758 2024-01-12 23:13:24.000000 lensiq-1.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6131 2024-05-22 18:25:31.528847 lensiq-1.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     5344 2024-05-22 18:21:05.000000 lensiq-1.3.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 18:25:31.449040 lensiq-1.3.1/lensIQ/
+-rw-rw-rw-   0        0        0      254 2024-01-09 19:31:09.000000 lensiq-1.3.1/lensIQ/__init__.py
+-rw-rw-rw-   0        0        0    22102 2024-01-25 19:50:47.000000 lensiq-1.3.1/lensIQ/defaultCalData.py
+-rw-rw-rw-   0        0        0    49485 2024-05-22 18:21:13.000000 lensiq-1.3.1/lensIQ/lensIQ.py
+drwxrwxrwx   0        0        0        0 2024-05-22 18:25:31.526853 lensiq-1.3.1/lensIQ.egg-info/
+-rw-rw-rw-   0        0        0     6131 2024-05-22 18:25:31.000000 lensiq-1.3.1/lensIQ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      242 2024-05-22 18:25:31.000000 lensiq-1.3.1/lensIQ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 18:25:31.000000 lensiq-1.3.1/lensIQ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2024-05-22 18:25:31.000000 lensiq-1.3.1/lensIQ.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-05-22 18:25:31.000000 lensiq-1.3.1/lensIQ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      877 2024-05-22 18:20:59.000000 lensiq-1.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 18:25:31.533842 lensiq-1.3.1/setup.cfg
```

### Comparing `lensIQ-1.3.0/LICENSE` & `lensiq-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lensIQ-1.3.0/PKG-INFO` & `lensiq-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensIQ
-Version: 1.3.0
+Version: 1.3.1
 Summary: Theia MCR motor control conversions and calculations
 Author-email: Mark Peterson <mpeterson@theiatech.com>
 Project-URL: Homepage, https://github.com/cliquot22/lensIQ
 Project-URL: Bug Tracker, https://github.com/cliquot22/lensIQ/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
@@ -90,8 +90,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.3.0
+v.1.3.1
```

### Comparing `lensIQ-1.3.0/README.md` & `lensiq-1.3.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -70,8 +70,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.3.0
+v.1.3.1
```

### Comparing `lensIQ-1.3.0/lensIQ/defaultCalData.py` & `lensiq-1.3.1/lensIQ/defaultCalData.py`

 * *Files identical despite different names*

### Comparing `lensIQ-1.3.0/lensIQ/lensIQ.py` & `lensiq-1.3.1/lensIQ/lensIQ.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
         - ERR_OD_VALUE = 'OD value'           # OD not specified
         - ERR_NA_MIN = 'NA min'               # minimum numerical aperture exceeded
         - ERR_NA_MAX = 'NA max'               # maximum numerical aperture exceeded
         - ERR_RANGE_MIN = 'out of range-min'  # out of allowable range
         - ERR_RANGE_MAX = 'out of range-max'  # out of allowable range
         - ERR_CALC = 'calculation error'      # calculation error (infinity or divide by zero or other)
         - WARN_VALUE = 'value warning'        # warning if value seems extreme, possible unit conversion issue
-        - STRING_VALUE = 'string value'       # string value returned when number value is expected
+        - ERR_NAN = 'string value'       # string value returned when number value is expected
 
         (c)2023 Theia Technologies
         www.TheiaTech.com
         '''
         self.calData = {}
         self.COC = lensIQ.COC
         self.sensorWd = 0
```

### Comparing `lensIQ-1.3.0/lensIQ.egg-info/PKG-INFO` & `lensiq-1.3.1/lensIQ.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lensIQ
-Version: 1.3.0
+Version: 1.3.1
 Summary: Theia MCR motor control conversions and calculations
 Author-email: Mark Peterson <mpeterson@theiatech.com>
 Project-URL: Homepage, https://github.com/cliquot22/lensIQ
 Project-URL: Bug Tracker, https://github.com/cliquot22/lensIQ/issues
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Manufacturing
@@ -90,8 +90,8 @@
 
 # Contact information
 For more information contact: 
 Mark Peterson at Theia Technologies
 [mpeterson@theiatech.com](mailto://mpeterson@theiatech.com)
 
 # Revision
-v.1.3.0
+v.1.3.1
```

### Comparing `lensIQ-1.3.0/pyproject.toml` & `lensiq-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "lensIQ"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="Mark Peterson", email="mpeterson@theiatech.com" },
 ]
 description = "Theia MCR motor control conversions and calculations"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

