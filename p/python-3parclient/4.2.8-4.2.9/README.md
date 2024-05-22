# Comparing `tmp/python-3parclient-4.2.8.tar.gz` & `tmp/python-3parclient-4.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/python-3parclient-4.2.8.tar", last modified: Tue Dec  4 08:27:25 2018, max compression
+gzip compressed data, was "dist/python-3parclient-4.2.9.tar", last modified: Thu Mar  7 12:01:41 2019, max compression
```

## Comparing `python-3parclient-4.2.8.tar` & `python-3parclient-4.2.9.tar`

### file list

```diff
@@ -1,38 +1,40 @@
-drwxrwxr-x   0 sneha     (1000) sneha     (1000)        0 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/
-drwxrwxr-x   0 sneha     (1000) sneha     (1000)        0 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/
--rw-rw-r--   0 sneha     (1000) sneha     (1000)      991 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/SOURCES.txt
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     9104 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/PKG-INFO
--rw-rw-r--   0 sneha     (1000) sneha     (1000)       27 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/requires.txt
--rw-rw-r--   0 sneha     (1000) sneha     (1000)        1 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/dependency_links.txt
--rw-rw-r--   0 sneha     (1000) sneha     (1000)       19 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/python_3parclient.egg-info/top_level.txt
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     9104 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/PKG-INFO
--rw-rw-r--   0 sneha     (1000) sneha     (1000)       38 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/setup.cfg
-drwxrwxr-x   0 sneha     (1000) sneha     (1000)        0 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/hpe3parclient/
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    14535 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/hpe3parclient/ssh.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     1132 2018-12-04 08:25:50.000000 python-3parclient-4.2.8/hpe3parclient/__init__.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    14843 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/hpe3parclient/http.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)   207589 2018-12-04 08:25:50.000000 python-3parclient-4.2.8/hpe3parclient/client.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    71164 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/hpe3parclient/file_client.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    12347 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/hpe3parclient/exceptions.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     2393 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/hpe3parclient/tcl_parser.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     6169 2018-12-04 08:25:50.000000 python-3parclient-4.2.8/README.rst
-drwxrwxr-x   0 sneha     (1000) sneha     (1000)        0 2018-12-04 08:27:25.000000 python-3parclient-4.2.8/test/
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    79863 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/HPE3ParMockServer_flask.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)        0 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/__init__.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    10176 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_MockSSH.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    14651 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_FilePersona_Mock.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    30242 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/HPE3ParMockServer_ssh.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     6489 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_CPG.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    16690 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_HostSet.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     2526 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_ports.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     4837 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HTTPJSONRESTClient.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     2765 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_Stats.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    20775 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_host.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    41919 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_FilePersona.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    14884 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_VLUN.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     2267 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_Exception.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     9153 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/HPE3ParClient_base.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     4895 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_system.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)    89646 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_volume.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     3426 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/test/test_HPE3ParClient_retry.py
--rw-rw-r--   0 sneha     (1000) sneha     (1000)     1244 2018-11-27 12:51:04.000000 python-3parclient-4.2.8/setup.py
+drwxrwxr-x   0 docker    (1000) docker    (1000)        0 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/
+-rw-rw-r--   0 docker    (1000) docker    (1000)     9072 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/PKG-INFO
+drwxrwxr-x   0 docker    (1000) docker    (1000)        0 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/
+-rw-rw-r--   0 docker    (1000) docker    (1000)       19 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/top_level.txt
+-rw-rw-r--   0 docker    (1000) docker    (1000)     9072 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/PKG-INFO
+-rw-rw-r--   0 docker    (1000) docker    (1000)       27 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/requires.txt
+-rw-rw-r--   0 docker    (1000) docker    (1000)        1 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 docker    (1000) docker    (1000)     1066 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/python_3parclient.egg-info/SOURCES.txt
+drwxrwxr-x   0 docker    (1000) docker    (1000)        0 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/hpe3parclient/
+-rw-rw-r--   0 docker    (1000) docker    (1000)    14535 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/ssh.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     2393 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/tcl_parser.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)   210091 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/client.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    71164 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/file_client.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     5273 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/showport_parser.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     1132 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/__init__.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    14843 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/http.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    12347 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/hpe3parclient/exceptions.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     6169 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/README.rst
+-rw-rw-r--   0 docker    (1000) docker    (1000)       59 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/setup.cfg
+-rw-rw-r--   0 docker    (1000) docker    (1000)     1244 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/setup.py
+drwxrwxr-x   0 docker    (1000) docker    (1000)        0 2019-03-07 12:01:41.000000 python-3parclient-4.2.9/test/
+-rw-rw-r--   0 docker    (1000) docker    (1000)     5374 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_ports.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    14884 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_VLUN.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     4837 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HTTPJSONRESTClient.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     3426 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_retry.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    14651 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_FilePersona_Mock.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     9153 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/HPE3ParClient_base.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    10176 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_MockSSH.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    30242 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/HPE3ParMockServer_ssh.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    79863 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/HPE3ParMockServer_flask.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     4895 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_system.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     2765 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_Stats.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    16690 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_HostSet.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)        0 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/__init__.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     6489 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_CPG.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)     2267 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_Exception.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    41919 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_FilePersona.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    89646 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_volume.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    20775 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_host.py
+-rw-rw-r--   0 docker    (1000) docker    (1000)    19923 2019-03-07 12:01:09.000000 python-3parclient-4.2.9/test/test_HPE3ParClient_ShowportParser.py
```

### Comparing `python-3parclient-4.2.8/python_3parclient.egg-info/SOURCES.txt` & `python-3parclient-4.2.9/python_3parclient.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 README.rst
 setup.py
 hpe3parclient/__init__.py
 hpe3parclient/client.py
 hpe3parclient/exceptions.py
 hpe3parclient/file_client.py
 hpe3parclient/http.py
+hpe3parclient/showport_parser.py
 hpe3parclient/ssh.py
 hpe3parclient/tcl_parser.py
 python_3parclient.egg-info/PKG-INFO
 python_3parclient.egg-info/SOURCES.txt
 python_3parclient.egg-info/dependency_links.txt
 python_3parclient.egg-info/requires.txt
 python_3parclient.egg-info/top_level.txt
@@ -18,14 +19,15 @@
 test/__init__.py
 test/test_HPE3ParClient_CPG.py
 test/test_HPE3ParClient_Exception.py
 test/test_HPE3ParClient_FilePersona.py
 test/test_HPE3ParClient_FilePersona_Mock.py
 test/test_HPE3ParClient_HostSet.py
 test/test_HPE3ParClient_MockSSH.py
+test/test_HPE3ParClient_ShowportParser.py
 test/test_HPE3ParClient_Stats.py
 test/test_HPE3ParClient_VLUN.py
 test/test_HPE3ParClient_host.py
 test/test_HPE3ParClient_ports.py
 test/test_HPE3ParClient_retry.py
 test/test_HPE3ParClient_system.py
 test/test_HPE3ParClient_volume.py
```

### Comparing `python-3parclient-4.2.8/python_3parclient.egg-info/PKG-INFO` & `python-3parclient-4.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: python-3parclient
-Version: 4.2.8
+Version: 4.2.9
 Summary: HPE 3PAR HTTP REST Client
 Home-page: http://packages.python.org/python-3parclient
 Author: Walter A. Boring IV
 Author-email: walter.boring@hpe.com
-Maintainer: Walter A. Boring IV
 License: Apache License, Version 2.0
 Description: .. image:: https://img.shields.io/pypi/v/python-3parclient.svg
             :target: https://pypi.python.org/pypi/python-3parclient
             :alt: Latest Version
         
         .. image:: https://img.shields.io/pypi/dm/python-3parclient.svg
             :target: https://pypi.python.org/pypi/python-3parclient
```

### Comparing `python-3parclient-4.2.8/PKG-INFO` & `python-3parclient-4.2.9/python_3parclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 1.2
+Metadata-Version: 1.1
 Name: python-3parclient
-Version: 4.2.8
+Version: 4.2.9
 Summary: HPE 3PAR HTTP REST Client
 Home-page: http://packages.python.org/python-3parclient
 Author: Walter A. Boring IV
 Author-email: walter.boring@hpe.com
-Maintainer: Walter A. Boring IV
 License: Apache License, Version 2.0
 Description: .. image:: https://img.shields.io/pypi/v/python-3parclient.svg
             :target: https://pypi.python.org/pypi/python-3parclient
             :alt: Latest Version
         
         .. image:: https://img.shields.io/pypi/dm/python-3parclient.svg
             :target: https://pypi.python.org/pypi/python-3parclient
```

### Comparing `python-3parclient-4.2.8/hpe3parclient/ssh.py` & `python-3parclient-4.2.9/hpe3parclient/ssh.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/hpe3parclient/__init__.py` & `python-3parclient-4.2.9/hpe3parclient/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 :Author: Walter A. Boring IV
 :Author: Kurt Martin
 :Copyright: Copyright 2012-2016 Hewlett Packard Enterprise Development LP
 :License: Apache v2.0
 
 """
 
-version_tuple = (4, 2, 8)
+version_tuple = (4, 2, 9)
 
 
 def get_version_string():
     """Current version of HPE3PARClient."""
     if isinstance(version_tuple[-1], str):
         return '.'.join(map(str, version_tuple[:-1])) + version_tuple[-1]
     return '.'.join(map(str, version_tuple))
```

### Comparing `python-3parclient-4.2.8/hpe3parclient/http.py` & `python-3parclient-4.2.9/hpe3parclient/http.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/hpe3parclient/client.py` & `python-3parclient-4.2.9/hpe3parclient/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,30 +22,31 @@
 :Description: This is the 3PAR Client that talks to 3PAR's REST WSAPI Service.
 It provides the ability to provision 3PAR volumes, VLUNs, CPGs.  This version
 also supports running actions on the 3PAR that use SSH.
 
 This client requires and works with 3PAR InForm 3.1.3 MU1 firmware
 
 """
+import copy
 import re
 import time
 import uuid
 
 try:
     # For Python 3.0 and later
     from urllib.parse import quote
 except ImportError:
     # Fall back to Python 2's urllib2
     from urllib2 import quote
 
 from hpe3parclient import exceptions, http, ssh
+from hpe3parclient import showport_parser
 
 
 class HPE3ParClient(object):
-
     """ The 3PAR REST API Client.
 
     :param api_url: The url to the WSAPI service on 3PAR
                     ie. http://<3par server>:8080/api/v1
     :type api_url: str
 
     """
@@ -136,31 +137,31 @@
     VLUN_TYPE_MATCHED_SET = 4
     VLUN_TYPE_HOST_SET = 5
 
     VLUN_MULTIPATH_UNKNOWN = 1
     VLUN_MULTIPATH_ROUND_ROBIN = 2
     VLUN_MULTIPATH_FAILOVER = 3
 
-    CPG_RAID_R0 = 1     # RAID 0
-    CPG_RAID_R1 = 2     # RAID 1
-    CPG_RAID_R5 = 3     # RAID 5
-    CPG_RAID_R6 = 4     # RAID 6
-
-    CPG_HA_PORT = 1     # Support failure of a port.
-    CPG_HA_CAGE = 2     # Support failure of a drive cage.
-    CPG_HA_MAG = 3      # Support failure of a drive magazine.
+    CPG_RAID_R0 = 1  # RAID 0
+    CPG_RAID_R1 = 2  # RAID 1
+    CPG_RAID_R5 = 3  # RAID 5
+    CPG_RAID_R6 = 4  # RAID 6
+
+    CPG_HA_PORT = 1  # Support failure of a port.
+    CPG_HA_CAGE = 2  # Support failure of a drive cage.
+    CPG_HA_MAG = 3  # Support failure of a drive magazine.
 
     # Lowest numbered available chunklets, where transfer rate is the fastest.
     CPG_CHUNKLET_POS_PREF_FIRST = 1
     # Highest numbered available chunklets, where transfer rate is the slowest.
     CPG_CHUNKLET_POS_PREF_LAST = 2
 
-    CPG_DISK_TYPE_FC = 1        # Fibre Channel
-    CPG_DISK_TYPE_NL = 2        # Near Line
-    CPG_DISK_TYPE_SSD = 3       # SSD
+    CPG_DISK_TYPE_FC = 1  # Fibre Channel
+    CPG_DISK_TYPE_NL = 2  # Near Line
+    CPG_DISK_TYPE_SSD = 3  # SSD
 
     HOST_EDIT_ADD = 1
     HOST_EDIT_REMOVE = 2
 
     HOST_PERSONA_GENERIC = 1
     HOST_PERSONA_GENERIC_ALUA = 2
     HOST_PERSONA_GENERIC_LEGACY = 3
@@ -215,22 +216,22 @@
                        'not supported.') % ex_desc
                 raise exceptions.UnsupportedVersion(msg)
 
         # Note the build contains major, minor, maintenance and build
         # e.g. 30102422 is 3 01 02 422
         # therefore all we need to compare is the build
         if (api_version is None or
-           api_version['build'] < self.HPE3PAR_WS_MIN_BUILD_VERSION):
+                api_version['build'] < self.HPE3PAR_WS_MIN_BUILD_VERSION):
             raise exceptions.UnsupportedVersion(
                 'Invalid 3PAR WS API, requires version, %s' %
                 self.HPE3PAR_WS_MIN_BUILD_VERSION_DESC)
 
         # Check for VLUN query support.
         if (api_version['build'] >=
-           self.HPE3PAR_WS_MIN_BUILD_VERSION_VLUN_QUERY):
+                self.HPE3PAR_WS_MIN_BUILD_VERSION_VLUN_QUERY):
             self.vlun_query_supported = True
 
     def setSSHOptions(self, ip, login, password, port=22,
                       conn_timeout=None, privatekey=None,
                       **kwargs):
         """Set SSH Options for ssh calls.
 
@@ -1744,14 +1745,15 @@
 
         :param iqn: lookup based on iSCSI initiator
         :type iqn: str
         :param wwn: lookup based on WWN
         :type wwn: str
 
         """
+
         # for now there is no search in the REST API
         # so we can do a create looking for a specific
         # error.  If we don't get that error, we nuke the
         # fake host.
 
         def _hostname():
             # create a safe, random hostname that won't
@@ -1876,14 +1878,38 @@
     def getPorts(self):
         """Get the list of ports on the 3PAR.
 
         :returns: list of Ports
 
         """
         response, body = self.http.get('/ports')
+        # if any of the ports are iSCSI ports and
+        # are vlan tagged (as shown by showport -iscsivlans), then
+        # the port information is merged with the WSAPI
+        # returned port information.
+        if self.ssh is not None:
+            if any([port['protocol'] == self.PORT_PROTO_ISCSI and
+                    'iSCSIPortInfo' in port and
+                    port['iSCSIPortInfo']['vlan'] == 1
+                    for port in body['members']]):
+                iscsi_vlan_data = self._run(['showport', '-iscsivlans'])
+                port_parser = showport_parser.ShowportParser()
+                iscsi_ports = port_parser.parseShowport(iscsi_vlan_data)
+                expanded_ports = self._cloneISCSIPorts(body, iscsi_ports)
+                for cli_port in expanded_ports:
+                    for wsapi_port in body[u'members']:
+                        if wsapi_port['portPos']['node'] == \
+                                cli_port['portPos']['node']  \
+                           and wsapi_port['portPos']['slot'] == \
+                                cli_port['portPos']['slot'] \
+                           and wsapi_port['portPos']['cardPort'] == \
+                                cli_port['portPos']['cardPort']:
+                            port_parser._merge_dict(wsapi_port, cli_port)
+                body['total'] = len(body['members'])
+
         return body
 
     def _getProtocolPorts(self, protocol, state=None):
         return_ports = []
         ports = self.getPorts()
         if ports:
             for port in ports['members']:
@@ -1891,14 +1917,38 @@
                     if state is None:
                         return_ports.append(port)
                     elif port['linkState'] == state:
                         return_ports.append(port)
 
         return return_ports
 
+    def _cloneISCSIPorts(self, real_ports, vlan_ports):
+        cloned_ports = []
+        for port in vlan_ports:
+            matching_ports = [
+                x for x in real_ports['members']
+                if (x['protocol'] == self.PORT_PROTO_ISCSI and
+                    x['iSCSIPortInfo']['vlan'] == 1 and
+                    x['portPos'] == port['portPos'])
+            ]
+
+            # should only be one
+            if len(matching_ports) > 1:
+                err = ("Found {} matching ports for vlan tagged iSCSI port "
+                       "{}.  There should only be one.")
+                raise exceptions.\
+                    NoUniqueMatch(err.format(len(matching_ports), port))
+
+            if len(matching_ports) == 1:
+                new_port = copy.deepcopy(matching_ports[0])
+                new_port.update(port)
+                cloned_ports.append(new_port)
+
+        return cloned_ports
+
     def getFCPorts(self, state=None):
         """Get a list of Fibre Channel Ports.
 
         :returns: list of Fibre Channel Ports
 
         """
         return self._getProtocolPorts(1, state)
@@ -2083,15 +2133,15 @@
             if vluns:
                 for vlun in vluns['members']:
                     if vlun['volumeName'] == volumeName:
                         return vlun
 
         raise exceptions.HTTPNotFound({'code': 'NON_EXISTENT_VLUN',
                                        'desc': "VLUN '%s' was not found" %
-                                       volumeName})
+                                               volumeName})
 
     def createVLUN(self, volumeName, lun=None, hostname=None, portPos=None,
                    noVcn=None, overrideLowerPriority=None, auto=False):
         """Create a new VLUN.
 
         When creating a VLUN, the volumeName is required. The lun member is
         not required if auto is set to True.
@@ -3728,28 +3778,29 @@
                 parameters = {'action': 2,
                               'volumeName': volumeName}
                 if optional:
                     parameters = self._mergeDict(parameters, optional)
 
                 response, body = self.http.put('/remotecopygroups/%s' % name,
                                                body=parameters)
+                return body
         else:
             option = None
             if optional and optional.get('keepSnap') and removeFromTarget:
                 raise Exception("keepSnap and removeFromTarget cannot be both\
                     true while removing the volume from remote copy group")
             elif optional and optional.get('keepSnap'):
                 option = 'keepSnap'
             elif removeFromTarget:
                 option = 'removeSecondaryVolume'
             delete_url = '/remotecopygroups/%s/volumes/%s' % (name, volumeName)
             if option:
                 delete_url += '?%s=true' % option
             response, body = self.http.delete(delete_url)
-        return body
+            return body
 
     def startRemoteCopy(self, name, optional=None):
         """
         Starts a remote copy
 
         :param name: Name of the remote copy group
         :type name: string
@@ -4193,16 +4244,16 @@
 
         """
         uri = '/volumes?query="snapCPG EQ %s"' % (snapcpgName)
         response, body = self.http.get(uri)
         snapshots = []
         for volume in body['members']:
             if 'copyOf' in volume:
-                if(volume['copyOf'] == volName and
-                   volume['copyType'] == self.VIRTUAL_COPY):
+                if (volume['copyOf'] == volName and
+                        volume['copyType'] == self.VIRTUAL_COPY):
                     snapshots.append(volume['name'])
         return snapshots
 
     def getFlashCache(self):
         """Get information about flash cache on the 3Par array.
         :returns: list of Hosts
         """
@@ -4344,16 +4395,16 @@
         """
         cmd = ['showrcopy', 'links']
         response = self._run(cmd)
         for item in response:
             if item.startswith(targetName):
                 link_info = item.split(',')
                 if link_info[0] == targetName and \
-                   link_info[1] == local_port and \
-                   link_info[2] == target_system_peer_port:
+                        link_info[1] == local_port and \
+                        link_info[2] == target_system_peer_port:
                     return True
         return False
 
     def admitRemoteCopyTarget(self, targetName, mode, remote_copy_group_name,
                               optional=None):
         """Adding target to remote copy group
         :param targetName - The name of target system
@@ -4381,16 +4432,17 @@
 
         cmd = ['admitrcopytarget', targetName,
                mode, remote_copy_group_name]
         if optional:
             volumePairs = optional.get('volumePairs')
             if volumePairs is not None:
                 for volumePair in volumePairs:
-                    source_target_pair = volumePair['sourceVolumeName'] + \
-                        ':' + volumePair['targetVolumeName']
+                    source_target_pair = \
+                        volumePair['sourceVolumeName'] + ':' + \
+                        volumePair['targetVolumeName']
                     cmd.append(source_target_pair)
         response = self._run(cmd)
         err_resp = self.check_response_for_admittarget(response, targetName)
         if err_resp:
             err = (("Admit remote copy target failed Error is\
  '%(err_resp)s' ") % {'err_resp': err_resp})
             raise exceptions.SSHException(err)
@@ -4457,28 +4509,30 @@
     def check_response_for_admittarget(self, resp, targetName):
         """
         Checks whether command response having valid output
         or not if output is invalid then return that response.
         """
         for r in resp:
             if 'error' in str.lower(r) or 'invalid' in str.lower(r) \
-               or 'must specify a mapping' in str.lower(r) \
-               or 'not exist' in str.lower(r) or 'no target' in str.lower(r) \
-               or 'group contains' in str.lower(r) \
-               or 'Target is already in this group.' in str(r) \
-               or 'could not locate an indicated volume.' in str(r) \
-               or 'Target system %s could not be contacted' % targetName \
-               in str(r) \
-               or 'Target %s could not get info on secondary target' \
-               % targetName in str(r) \
-               or 'Target %s is not up and ready' % targetName in str(r) \
-               or 'A group may have only a single synchronous target.' \
-               in str(r) or \
-               'cannot have groups with more than one synchronization mode' \
-               in str.lower(r):
+                    or 'must specify a mapping' in str.lower(r) \
+                    or 'not exist' in str.lower(r) \
+                    or 'no target' in str.lower(r) \
+                    or 'group contains' in str.lower(r) \
+                    or 'Target is already in this group.' in str(r) \
+                    or 'could not locate an indicated volume.' in str(r) \
+                    or 'Target system %s could not be contacted' % targetName \
+                    in str(r) \
+                    or 'Target %s could not get info on secondary target' \
+                    % targetName in str(r) \
+                    or 'Target %s is not up and ready' % targetName in str(r) \
+                    or 'A group may have only a single synchronous target.' \
+                    in str(r) or \
+                    'cannot have groups with more than one ' \
+                    'synchronization mode' \
+                    in str.lower(r):
                 return r
 
     def check_response(self, resp):
         for r in resp:
             if 'error' in str.lower(r) or 'invalid' in str.lower(r):
                 err_resp = r.strip()
                 return err_resp
```

### Comparing `python-3parclient-4.2.8/hpe3parclient/file_client.py` & `python-3parclient-4.2.9/hpe3parclient/file_client.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/hpe3parclient/exceptions.py` & `python-3parclient-4.2.9/hpe3parclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/hpe3parclient/tcl_parser.py` & `python-3parclient-4.2.9/hpe3parclient/tcl_parser.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/README.rst` & `python-3parclient-4.2.9/README.rst`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/HPE3ParMockServer_flask.py` & `python-3parclient-4.2.9/test/HPE3ParMockServer_flask.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_MockSSH.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_MockSSH.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_FilePersona_Mock.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_FilePersona_Mock.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/HPE3ParMockServer_ssh.py` & `python-3parclient-4.2.9/test/HPE3ParMockServer_ssh.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_CPG.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_CPG.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_HostSet.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_HostSet.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HTTPJSONRESTClient.py` & `python-3parclient-4.2.9/test/test_HTTPJSONRESTClient.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_Stats.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_Stats.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_host.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_host.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_FilePersona.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_FilePersona.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_VLUN.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_VLUN.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_Exception.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_Exception.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/HPE3ParClient_base.py` & `python-3parclient-4.2.9/test/HPE3ParClient_base.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_system.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_system.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_volume.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_volume.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/test/test_HPE3ParClient_retry.py` & `python-3parclient-4.2.9/test/test_HPE3ParClient_retry.py`

 * *Files identical despite different names*

### Comparing `python-3parclient-4.2.8/setup.py` & `python-3parclient-4.2.9/setup.py`

 * *Files identical despite different names*

