# Comparing `tmp/udi_interface-3.3.5.tar.gz` & `tmp/udi_interface-3.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udi_interface-3.3.5.tar", last modified: Mon Apr 29 12:43:15 2024, max compression
+gzip compressed data, was "udi_interface-3.3.6.tar", last modified: Wed May 22 12:30:26 2024, max compression
```

## Comparing `udi_interface-3.3.5.tar` & `udi_interface-3.3.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.318079 udi_interface-3.3.5/
--rwxrwxrwx   0 admin     (1001) admin     (1001)     1068 2023-07-05 13:05:47.000000 udi_interface-3.3.5/LICENSE
--rw-r--r--   0 admin     (1001) admin     (1001)     2418 2024-04-29 12:43:15.318219 udi_interface-3.3.5/PKG-INFO
--rwxrwxrwx   0 admin     (1001) admin     (1001)     1769 2023-07-05 13:05:47.000000 udi_interface-3.3.5/README.md
--rwxrwxrwx   0 admin     (1001) admin     (1001)      224 2024-04-29 12:43:15.318754 udi_interface-3.3.5/setup.cfg
--rwxrw-r--   0 admin     (1001) admin     (1001)     1514 2024-02-27 13:56:52.000000 udi_interface-3.3.5/setup.py
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.316623 udi_interface-3.3.5/udi_interface/
--rwxrw-r--   0 admin     (1001) admin     (1001)     1630 2024-04-29 12:41:59.000000 udi_interface-3.3.5/udi_interface/__init__.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     6362 2024-03-19 20:20:13.000000 udi_interface-3.3.5/udi_interface/custom.py
--rwxrw-r--   0 admin     (1001) admin     (1001)    65274 2024-03-20 20:32:06.000000 udi_interface-3.3.5/udi_interface/interface.py
--rw-r--r--   0 admin     (1001) admin     (1001)     2964 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/isy.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     7126 2024-03-20 20:09:23.000000 udi_interface-3.3.5/udi_interface/node.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     6804 2024-04-29 12:38:02.000000 udi_interface-3.3.5/udi_interface/oauth.py
--rwxr-xr-x   0 admin     (1001) admin     (1001)     3276 2023-12-22 20:03:53.000000 udi_interface-3.3.5/udi_interface/polylogger.py
--rw-r--r--   0 admin     (1001) admin     (1001)      873 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/startupdiag.py
--rwxrw-r--   0 admin     (1001) admin     (1001)     2345 2024-01-05 14:26:37.000000 udi_interface-3.3.5/udi_interface/test.py
--rwxr-xr-x   0 admin     (1001) admin     (1001)     4004 2024-01-25 19:13:19.000000 udi_interface-3.3.5/udi_interface/udi_interface.py
-drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-04-29 12:43:15.317916 udi_interface-3.3.5/udi_interface.egg-info/
--rwxrwxrwx   0 admin     (1001) admin     (1001)     2418 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/PKG-INFO
--rwxrwxrwx   0 admin     (1001) admin     (1001)      509 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/SOURCES.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/dependency_links.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-05 20:51:23.000000 udi_interface-3.3.5/udi_interface.egg-info/not-zip-safe
--rwxrwxrwx   0 admin     (1001) admin     (1001)       92 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/requires.txt
--rwxrwxrwx   0 admin     (1001) admin     (1001)       14 2024-04-29 12:43:15.000000 udi_interface-3.3.5/udi_interface.egg-info/top_level.txt
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-05-22 12:30:26.447572 udi_interface-3.3.6/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1068 2023-07-05 13:05:47.000000 udi_interface-3.3.6/LICENSE
+-rw-r--r--   0 admin     (1001) admin     (1001)     2418 2024-05-22 12:30:26.447709 udi_interface-3.3.6/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     1769 2023-07-05 13:05:47.000000 udi_interface-3.3.6/README.md
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      224 2024-05-22 12:30:26.448320 udi_interface-3.3.6/setup.cfg
+-rwxrw-r--   0 admin     (1001) admin     (1001)     1514 2024-02-27 13:56:52.000000 udi_interface-3.3.6/setup.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-05-22 12:30:26.445804 udi_interface-3.3.6/udi_interface/
+-rwxrw-r--   0 admin     (1001) admin     (1001)     1630 2024-05-22 12:24:36.000000 udi_interface-3.3.6/udi_interface/__init__.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     6362 2024-03-19 20:20:13.000000 udi_interface-3.3.6/udi_interface/custom.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)    65274 2024-05-22 12:24:36.000000 udi_interface-3.3.6/udi_interface/interface.py
+-rw-r--r--   0 admin     (1001) admin     (1001)     2964 2024-01-25 19:13:19.000000 udi_interface-3.3.6/udi_interface/isy.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     7126 2024-03-20 20:09:23.000000 udi_interface-3.3.6/udi_interface/node.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     6804 2024-04-29 12:38:02.000000 udi_interface-3.3.6/udi_interface/oauth.py
+-rwxr-xr-x   0 admin     (1001) admin     (1001)     3276 2023-12-22 20:03:53.000000 udi_interface-3.3.6/udi_interface/polylogger.py
+-rw-r--r--   0 admin     (1001) admin     (1001)      873 2024-01-25 19:13:19.000000 udi_interface-3.3.6/udi_interface/startupdiag.py
+-rwxrw-r--   0 admin     (1001) admin     (1001)     2345 2024-01-05 14:26:37.000000 udi_interface-3.3.6/udi_interface/test.py
+-rwxr-xr-x   0 admin     (1001) admin     (1001)     4004 2024-01-25 19:13:19.000000 udi_interface-3.3.6/udi_interface/udi_interface.py
+drwxr-xr-x   0 admin     (1001) admin     (1001)        0 2024-05-22 12:30:26.447407 udi_interface-3.3.6/udi_interface.egg-info/
+-rwxrwxrwx   0 admin     (1001) admin     (1001)     2418 2024-05-22 12:30:26.000000 udi_interface-3.3.6/udi_interface.egg-info/PKG-INFO
+-rwxrwxrwx   0 admin     (1001) admin     (1001)      509 2024-05-22 12:30:26.000000 udi_interface-3.3.6/udi_interface.egg-info/SOURCES.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2024-05-22 12:30:26.000000 udi_interface-3.3.6/udi_interface.egg-info/dependency_links.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)        1 2023-07-05 20:51:23.000000 udi_interface-3.3.6/udi_interface.egg-info/not-zip-safe
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       92 2024-05-22 12:30:26.000000 udi_interface-3.3.6/udi_interface.egg-info/requires.txt
+-rwxrwxrwx   0 admin     (1001) admin     (1001)       14 2024-05-22 12:30:26.000000 udi_interface-3.3.6/udi_interface.egg-info/top_level.txt
```

### Comparing `udi_interface-3.3.5/LICENSE` & `udi_interface-3.3.6/LICENSE`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/PKG-INFO` & `udi_interface-3.3.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi_interface
-Version: 3.3.5
+Version: 3.3.6
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `udi_interface-3.3.5/README.md` & `udi_interface-3.3.6/README.md`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/setup.py` & `udi_interface-3.3.6/setup.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/__init__.py` & `udi_interface-3.3.6/udi_interface/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.3.5'
+__version__ = '3.3.6'
 __description__ = 'UDI Python Interface for Polyglot version 3'
 __url__ = 'https://github.com/UniversalDevicesInc/udi_python_interface'
 __author__ = 'Universal Devices Inc.'
 __authoremail__ = 'bpaauwe@yahoo.com'
 __license__ = 'MIT'
 
 import traceback
```

### Comparing `udi_interface-3.3.5/udi_interface/custom.py` & `udi_interface-3.3.6/udi_interface/custom.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/interface.py` & `udi_interface-3.3.6/udi_interface/interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -3280,15 +3280,15 @@
 0000ccf0: 7328 6e61 6d65 2c20 2775 7466 2d38 2729  s(name, 'utf-8')
 0000cd00: 2e64 6563 6f64 6528 2775 7466 2d38 272c  .decode('utf-8',
 0000cd10: 2769 676e 6f72 6527 290d 0a20 2020 2020  'ignore')..     
 0000cd20: 2020 2072 6574 7572 6e20 7265 2e73 7562     return re.sub
 0000cd30: 2872 225b 3c3e 607e 2140 2324 255e 262a  (r"[<>`~!@#$%^&*
 0000cd40: 2829 7b7d 5b5c 5d3f 2f5c 5c3b 3a5c 2227  (){}[\]?/\\;:\"'
 0000cd50: 5c2d 5d2b 222c 2022 222c 206e 616d 652e  \-]+", "", name.
-0000cd60: 6c6f 7765 7228 295b 3a31 345d 290d 0a20  lower()[:14]).. 
+0000cd60: 6c6f 7765 7228 2929 5b3a 3134 5d0d 0a20  lower())[:14].. 
 0000cd70: 2020 2064 6566 2069 734e 616d 6556 616c     def isNameVal
 0000cd80: 6964 2873 656c 662c 206e 616d 6529 3a0d  id(self, name):.
 0000cd90: 0a20 2020 2020 2020 2072 6e61 6d65 203d  .        rname =
 0000cda0: 2062 7974 6573 286e 616d 652c 2027 7574   bytes(name, 'ut
 0000cdb0: 662d 3827 292e 6465 636f 6465 2827 7574  f-8').decode('ut
 0000cdc0: 662d 3827 2c27 6967 6e6f 7265 2729 0d0a  f-8','ignore')..
 0000cdd0: 2020 2020 2020 2020 2320 5265 6d6f 7665          # Remove
```

### Comparing `udi_interface-3.3.5/udi_interface/isy.py` & `udi_interface-3.3.6/udi_interface/isy.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/node.py` & `udi_interface-3.3.6/udi_interface/node.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/oauth.py` & `udi_interface-3.3.6/udi_interface/oauth.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/polylogger.py` & `udi_interface-3.3.6/udi_interface/polylogger.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/startupdiag.py` & `udi_interface-3.3.6/udi_interface/startupdiag.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/test.py` & `udi_interface-3.3.6/udi_interface/test.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface/udi_interface.py` & `udi_interface-3.3.6/udi_interface/udi_interface.py`

 * *Files identical despite different names*

### Comparing `udi_interface-3.3.5/udi_interface.egg-info/PKG-INFO` & `udi_interface-3.3.6/udi_interface.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udi-interface
-Version: 3.3.5
+Version: 3.3.6
 Summary: UDI Python Interface for Polyglot version 3
 Home-page: https://github.com/UniversalDevicesInc/udi_python_interface
 Author: Universal Devices Inc.
 Author-email: bpaauwe@yahoo.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

