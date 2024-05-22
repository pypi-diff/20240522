# Comparing `tmp/snowflake_native_apps_permission_stub-0.1.7.tar.gz` & `tmp/snowflake-native-apps-permission-stub-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake_native_apps_permission_stub-0.1.7.tar", last modified: Thu Apr 25 16:59:34 2024, max compression
+gzip compressed data, was "/mnt/jenkins/home/jenkins/workspace/NA_Permissions_Sdk_Stub_To_PyPI/dist/tmp0a9u_c7c/snowflake-native-apps-permission-stub-0.1.", last modified: Wed May 22 21:35:07 2024, max compression
```

## Comparing `snowflake_native_apps_permission_stub-0.1.7.tar` & `snowflake-native-apps-permission-stub-0.1.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 melnacouzi   (501) staff       (20)        0 2024-04-25 16:59:34.919494 snowflake_native_apps_permission_stub-0.1.7/
--rw-r--r--   0 melnacouzi   (501) staff       (20)    11366 2024-04-09 19:04:09.000000 snowflake_native_apps_permission_stub-0.1.7/LICENSE.txt
--rw-r--r--   0 melnacouzi   (501) staff       (20)     1383 2024-04-25 16:59:34.919202 snowflake_native_apps_permission_stub-0.1.7/PKG-INFO
--rw-r--r--   0 melnacouzi   (501) staff       (20)      206 2024-04-08 13:19:03.000000 snowflake_native_apps_permission_stub-0.1.7/README.md
--rw-r--r--   0 melnacouzi   (501) staff       (20)       59 2024-04-09 19:04:09.000000 snowflake_native_apps_permission_stub-0.1.7/pyproject.toml
--rw-r--r--   0 melnacouzi   (501) staff       (20)       38 2024-04-25 16:59:34.919555 snowflake_native_apps_permission_stub-0.1.7/setup.cfg
--rw-r--r--   0 melnacouzi   (501) staff       (20)     1935 2024-04-18 18:29:13.000000 snowflake_native_apps_permission_stub-0.1.7/setup.py
-drwxr-xr-x   0 melnacouzi   (501) staff       (20)        0 2024-04-25 16:59:34.914620 snowflake_native_apps_permission_stub-0.1.7/src/
-drwxr-xr-x   0 melnacouzi   (501) staff       (20)        0 2024-04-25 16:59:34.916860 snowflake_native_apps_permission_stub-0.1.7/src/snowflake/
--rw-r--r--   0 melnacouzi   (501) staff       (20)       25 2024-04-09 19:04:09.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake/__init__.py
--rw-r--r--   0 melnacouzi   (501) staff       (20)     1645 2024-04-18 18:29:13.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake/permissions.py
--rw-r--r--   0 melnacouzi   (501) staff       (20)       23 2024-04-18 18:29:13.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake/version.py
-drwxr-xr-x   0 melnacouzi   (501) staff       (20)        0 2024-04-25 16:59:34.918860 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/
--rw-r--r--   0 melnacouzi   (501) staff       (20)     1383 2024-04-25 16:59:34.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/PKG-INFO
--rw-r--r--   0 melnacouzi   (501) staff       (20)      509 2024-04-25 16:59:34.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/SOURCES.txt
--rw-r--r--   0 melnacouzi   (501) staff       (20)        1 2024-04-25 16:59:34.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/dependency_links.txt
--rw-r--r--   0 melnacouzi   (501) staff       (20)       19 2024-04-25 16:59:34.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/requires.txt
--rw-r--r--   0 melnacouzi   (501) staff       (20)       10 2024-04-25 16:59:34.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/top_level.txt
--rw-r--r--   0 melnacouzi   (501) staff       (20)        1 2024-04-08 13:34:02.000000 snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/zip-safe
+drwxr-xr-x   0 jenkins   (1006) jenkins   (1007)        0 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/
+drwxr-xr-x   0 jenkins   (1006) jenkins   (1007)        0 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/
+drwxr-xr-x   0 jenkins   (1006) jenkins   (1007)        0 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake/
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       25 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake/__init__.py
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)     1830 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake/permissions.py
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       23 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake/version.py
+drwxr-xr-x   0 jenkins   (1006) jenkins   (1007)        0 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)     1404 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)      509 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)        1 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       19 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       10 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)        1 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/zip-safe
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)    11366 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/LICENSE.txt
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)      206 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/README.md
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       59 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/pyproject.toml
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)     1935 2024-05-22 21:34:43.000000 snowflake-native-apps-permission-stub-0.1.9/setup.py
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)     1404 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/PKG-INFO
+-rw-r--r--   0 jenkins   (1006) jenkins   (1007)       38 2024-05-22 21:35:07.000000 snowflake-native-apps-permission-stub-0.1.9/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `snowflake_native_apps_permission_stub-0.1.7/LICENSE.txt` & `snowflake-native-apps-permission-stub-0.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake_native_apps_permission_stub-0.1.7/PKG-INFO` & `snowflake-native-apps-permission-stub-0.1.9/src/snowflake_native_apps_permission_stub.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: snowflake-native-apps-permission-stub
-Version: 0.1.7
+Version: 0.1.9
 Summary: Snowflake Native App Permission SDK Stub
+Home-page: UNKNOWN
 Author: Snowflake, Inc
 Author-email: support@snowflake.com
+License: UNKNOWN
 Keywords: Snowflake db database cloud warehouse permissions sdk native apps
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -21,10 +24,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
-Requires-Dist: setuptools>=40.0.0
 
 This package provides a set of stub functions that replaces the permissions SDK for local testing
+
```

### Comparing `snowflake_native_apps_permission_stub-0.1.7/setup.py` & `snowflake-native-apps-permission-stub-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `snowflake_native_apps_permission_stub-0.1.7/src/snowflake/permissions.py` & `snowflake-native-apps-permission-stub-0.1.9/src/snowflake/permissions.py`

 * *Files 18% similar despite different names*

```diff
@@ -44,12 +44,18 @@
 
 def is_event_sharing_enabled() -> bool:
     return False
 
 def is_application_local_to_package() -> bool:
     return False
 
+def is_application_authorized_for_telemetry_event_sharing() -> bool:
+    return False
+
+def is_application_all_mandatory_telemetry_event_definitions_enabled() -> bool:
+    return False
+
 def request_external_data() -> None:
     pass
 
 def is_external_data_enabled() -> bool:
     return False
```

### Comparing `snowflake_native_apps_permission_stub-0.1.7/src/snowflake_native_apps_permission_stub.egg-info/PKG-INFO` & `snowflake-native-apps-permission-stub-0.1.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 Metadata-Version: 2.1
 Name: snowflake-native-apps-permission-stub
-Version: 0.1.7
+Version: 0.1.9
 Summary: Snowflake Native App Permission SDK Stub
+Home-page: UNKNOWN
 Author: Snowflake, Inc
 Author-email: support@snowflake.com
+License: UNKNOWN
 Keywords: Snowflake db database cloud warehouse permissions sdk native apps
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Environment :: Console
 Classifier: Environment :: Other Environment
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
@@ -21,10 +24,10 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: LICENSE.txt
-Requires-Dist: setuptools>=40.0.0
 
 This package provides a set of stub functions that replaces the permissions SDK for local testing
+
```

