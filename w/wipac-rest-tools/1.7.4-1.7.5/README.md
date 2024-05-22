# Comparing `tmp/wipac-rest-tools-1.7.4.tar.gz` & `tmp/wipac-rest-tools-1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wipac-rest-tools-1.7.4.tar", last modified: Fri May  3 21:43:28 2024, max compression
+gzip compressed data, was "wipac-rest-tools-1.7.5.tar", last modified: Wed May 22 21:58:15 2024, max compression
```

## Comparing `wipac-rest-tools-1.7.4.tar` & `wipac-rest-tools-1.7.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/
--rw-r--r--   0 root         (0) root         (0)     1070 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6052 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4958 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.354988 wipac-rest-tools-1.7.4/rest_tools/
--rw-r--r--   0 root         (0) root         (0)      513 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.354988 wipac-rest-tools-1.7.4/rest_tools/client/
--rw-r--r--   0 root         (0) root         (0)      638 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    15182 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/client.py
--rw-r--r--   0 root         (0) root         (0)     2008 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/client_credentials.py
--rw-r--r--   0 root         (0) root         (0)     7641 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/device_client.py
--rw-r--r--   0 root         (0) root         (0)     3118 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/openid_client.py
--rw-r--r--   0 root         (0) root         (0)     2523 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/session.py
--rw-r--r--   0 root         (0) root         (0)     2545 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/client/utils.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/rest_tools/server/
--rw-r--r--   0 root         (0) root         (0)      843 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8514 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/arghandler.py
--rw-r--r--   0 root         (0) root         (0)    17104 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/decorators.py
--rw-r--r--   0 root         (0) root         (0)    18812 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/handler.py
--rw-r--r--   0 root         (0) root         (0)     2251 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/server.py
--rw-r--r--   0 root         (0) root         (0)     2348 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/server/stats.py
--rw-r--r--   0 root         (0) root         (0)     1781 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/telemetry.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/rest_tools/utils/
--rw-r--r--   0 root         (0) root         (0)      252 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5579 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/auth.py
--rw-r--r--   0 root         (0) root         (0)      136 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/config.py
--rw-r--r--   0 root         (0) root         (0)     6123 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/daemon.py
--rw-r--r--   0 root         (0) root         (0)     4832 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/rest_tools/utils/json_util.py
--rw-r--r--   0 root         (0) root         (0)     2311 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      104 2024-05-03 21:43:26.000000 wipac-rest-tools-1.7.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-03 21:43:28.358988 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6052 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      842 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      583 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-05-03 21:43:28.000000 wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4958 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.913997 wipac-rest-tools-1.7.5/rest_tools/
+-rw-r--r--   0 root         (0) root         (0)      513 2024-05-22 21:58:14.000000 wipac-rest-tools-1.7.5/rest_tools/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.913997 wipac-rest-tools-1.7.5/rest_tools/client/
+-rw-r--r--   0 root         (0) root         (0)      638 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    15182 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/client.py
+-rw-r--r--   0 root         (0) root         (0)     2008 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/client_credentials.py
+-rw-r--r--   0 root         (0) root         (0)     7641 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/device_client.py
+-rw-r--r--   0 root         (0) root         (0)     3118 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/openid_client.py
+-rw-r--r--   0 root         (0) root         (0)     2523 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/session.py
+-rw-r--r--   0 root         (0) root         (0)     1937 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/client/utils.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/rest_tools/server/
+-rw-r--r--   0 root         (0) root         (0)      843 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8514 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/arghandler.py
+-rw-r--r--   0 root         (0) root         (0)    17104 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/decorators.py
+-rw-r--r--   0 root         (0) root         (0)    18812 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/handler.py
+-rw-r--r--   0 root         (0) root         (0)     2251 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/server.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/server/stats.py
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/telemetry.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/rest_tools/utils/
+-rw-r--r--   0 root         (0) root         (0)      252 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/utils/auth.py
+-rw-r--r--   0 root         (0) root         (0)      136 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/utils/config.py
+-rw-r--r--   0 root         (0) root         (0)     6123 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/utils/daemon.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/rest_tools/utils/json_util.py
+-rw-r--r--   0 root         (0) root         (0)     2311 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      104 2024-05-22 21:58:13.000000 wipac-rest-tools-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-22 21:58:15.917997 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6052 2024-05-22 21:58:15.000000 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      842 2024-05-22 21:58:15.000000 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-22 21:58:15.000000 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      583 2024-05-22 21:58:15.000000 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-05-22 21:58:15.000000 wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/top_level.txt
```

### Comparing `wipac-rest-tools-1.7.4/LICENSE` & `wipac-rest-tools-1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/PKG-INFO` & `wipac-rest-tools-1.7.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.4
+Version: 1.7.5
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.4/README.md` & `wipac-rest-tools-1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/__init__.py` & `wipac-rest-tools-1.7.5/rest_tools/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # version is a human-readable version number.
 
 # version_info is a four-tuple for programmatic comparison. The first
 # three numbers are the components of the version number. The fourth
 # is zero for an official release, positive for a development branch,
 # or negative for a release candidate or beta (after the base version
 # number has been incremented)
-__version__ = "1.7.4"
+__version__ = "1.7.5"
 version_info = (
     int(__version__.split(".")[0]),
     int(__version__.split(".")[1]),
     int(__version__.split(".")[2]),
     0,
 )
```

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/__init__.py` & `wipac-rest-tools-1.7.5/rest_tools/client/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/client.py` & `wipac-rest-tools-1.7.5/rest_tools/client/client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/client_credentials.py` & `wipac-rest-tools-1.7.5/rest_tools/client/client_credentials.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/device_client.py` & `wipac-rest-tools-1.7.5/rest_tools/client/device_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/openid_client.py` & `wipac-rest-tools-1.7.5/rest_tools/client/openid_client.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/client/session.py` & `wipac-rest-tools-1.7.5/rest_tools/client/session.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/__init__.py` & `wipac-rest-tools-1.7.5/rest_tools/server/__init__.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/arghandler.py` & `wipac-rest-tools-1.7.5/rest_tools/server/arghandler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/decorators.py` & `wipac-rest-tools-1.7.5/rest_tools/server/decorators.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/handler.py` & `wipac-rest-tools-1.7.5/rest_tools/server/handler.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/server.py` & `wipac-rest-tools-1.7.5/rest_tools/server/server.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/server/stats.py` & `wipac-rest-tools-1.7.5/rest_tools/server/stats.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/telemetry.py` & `wipac-rest-tools-1.7.5/rest_tools/telemetry.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/utils/auth.py` & `wipac-rest-tools-1.7.5/rest_tools/utils/auth.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/utils/daemon.py` & `wipac-rest-tools-1.7.5/rest_tools/utils/daemon.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/rest_tools/utils/json_util.py` & `wipac-rest-tools-1.7.5/rest_tools/utils/json_util.py`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/setup.cfg` & `wipac-rest-tools-1.7.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/PKG-INFO` & `wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wipac-rest-tools
-Version: 1.7.4
+Version: 1.7.5
 Summary: REST tools in python - common code for client and server
 Home-page: https://github.com/WIPACrepo/rest-tools
 Download-URL: https://pypi.org/project/wipac-rest-tools/
 Author: WIPAC Developers
 Author-email: developers@icecube.wisc.edu
 License: MIT
 Project-URL: Tracker, https://github.com/WIPACrepo/rest-tools/issues
```

### Comparing `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/SOURCES.txt` & `wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wipac-rest-tools-1.7.4/wipac_rest_tools.egg-info/requires.txt` & `wipac-rest-tools-1.7.5/wipac_rest_tools.egg-info/requires.txt`

 * *Files identical despite different names*

