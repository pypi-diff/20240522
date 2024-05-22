# Comparing `tmp/heaserver-volumes-1.1.0.tar.gz` & `tmp/heaserver_volumes-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-volumes-1.1.0.tar", last modified: Fri Apr  5 20:01:11 2024, max compression
+gzip compressed data, was "heaserver_volumes-1.2.0.tar", last modified: Wed May 22 15:58:10 2024, max compression
```

## Comparing `heaserver-volumes-1.1.0.tar` & `heaserver_volumes-1.2.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.543153 heaserver-volumes-1.1.0/
--rw-rw-rw-   0        0        0      261 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/.gitignore
--rw-rw-rw-   0        0        0     1689 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4933 2024-04-05 20:01:11.542115 heaserver-volumes-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3631 2024-03-21 23:46:04.000000 heaserver-volumes-1.1.0/README.md
--rw-rw-rw-   0        0        0     1737 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/RELEASING.md
--rw-rw-rw-   0        0        0      408 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.358392 heaserver-volumes-1.1.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.358392 heaserver-volumes-1.1.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.455568 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     6953 2024-04-04 20:56:23.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0     8935 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     3703 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0    10728 2024-04-04 20:56:14.000000 heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     4637 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-05 20:01:11.543153 heaserver-volumes-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1799 2024-04-05 20:00:40.000000 heaserver-volumes-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.360478 heaserver-volumes-1.1.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.359455 heaserver-volumes-1.1.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.468851 heaserver-volumes-1.1.0/src/heaserver/volume/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/src/heaserver/volume/__init__.py
--rw-rw-rw-   0        0        0    35524 2024-04-05 05:05:11.000000 heaserver-volumes-1.1.0/src/heaserver/volume/service.py
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.476743 heaserver-volumes-1.1.0/src/heaserver/volume/wstl/
--rw-rw-rw-   0        0        0    14506 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/src/heaserver/volume/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.541060 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/
--rw-rw-rw-   0        0        0     4933 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1093 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       68 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-05 20:01:11.000000 heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.361508 heaserver-volumes-1.1.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.361508 heaserver-volumes-1.1.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-05 20:01:11.538950 heaserver-volumes-1.1.0/tests/heaserver/volumetest/
--rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/__init__.py
--rw-rw-rw-   0        0        0     6760 2024-04-04 20:56:06.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/permissionstestcase.py
--rw-rw-rw-   0        0        0     8648 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all.py
--rw-rw-rw-   0        0        0     3681 2023-12-18 23:36:40.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     7601 2024-04-04 20:55:52.000000 heaserver-volumes-1.1.0/tests/heaserver/volumetest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:10.059313 heaserver_volumes-1.2.0/
+-rw-rw-rw-   0        0        0      261 2022-03-20 02:03:35.000000 heaserver_volumes-1.2.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1689 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-20 02:03:35.000000 heaserver_volumes-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5310 2024-05-22 15:58:10.057716 heaserver_volumes-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4008 2024-05-22 15:29:26.000000 heaserver_volumes-1.2.0/README.md
+-rw-rw-rw-   0        0        0     1737 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/RELEASING.md
+-rw-rw-rw-   0        0        0      408 2024-05-16 17:34:18.000000 heaserver_volumes-1.2.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.847352 heaserver_volumes-1.2.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.847352 heaserver_volumes-1.2.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.954683 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     6953 2024-04-05 20:02:36.000000 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     8935 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     3703 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0    11722 2024-05-17 22:55:13.000000 heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     4637 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:58:10.059817 heaserver_volumes-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1799 2024-05-22 15:57:13.000000 heaserver_volumes-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.849352 heaserver_volumes-1.2.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.848349 heaserver_volumes-1.2.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.974215 heaserver_volumes-1.2.0/src/heaserver/volume/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver_volumes-1.2.0/src/heaserver/volume/__init__.py
+-rw-rw-rw-   0        0        0    34480 2024-05-16 17:38:26.000000 heaserver_volumes-1.2.0/src/heaserver/volume/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.976219 heaserver_volumes-1.2.0/src/heaserver/volume/wstl/
+-rw-rw-rw-   0        0        0    15494 2024-05-14 00:26:15.000000 heaserver_volumes-1.2.0/src/heaserver/volume/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:10.056678 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/
+-rw-rw-rw-   0        0        0     5310 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1093 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       68 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 15:58:09.000000 heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.850349 heaserver_volumes-1.2.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:09.850349 heaserver_volumes-1.2.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:58:10.054411 heaserver_volumes-1.2.0/tests/heaserver/volumetest/
+-rw-rw-rw-   0        0        0        0 2022-03-20 02:03:35.000000 heaserver_volumes-1.2.0/tests/heaserver/volumetest/__init__.py
+-rw-rw-rw-   0        0        0     6760 2024-04-05 20:02:36.000000 heaserver_volumes-1.2.0/tests/heaserver/volumetest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     8648 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/tests/heaserver/volumetest/test_all.py
+-rw-rw-rw-   0        0        0     3681 2023-12-18 23:36:40.000000 heaserver_volumes-1.2.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     8407 2024-05-17 22:39:45.000000 heaserver_volumes-1.2.0/tests/heaserver/volumetest/testcase.py
```

### Comparing `heaserver-volumes-1.1.0/Dockerfile` & `heaserver_volumes-1.2.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/LICENSE` & `heaserver_volumes-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/PKG-INFO` & `heaserver_volumes-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.1.0
+Version: 1.2.0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,32 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Volumes Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Volumes Microservice The HEA volumes service.
 
+## Version 1.2.0
+* Hid some attributes from the heaobject.volume.Volume properties card.
+* Added account_id attribute to the heaobject.volume.Volume properties card.
+* Removed the type name filter from volume queries. We now use heaobject.account.AccountView ids for the account id
+filter.
+
+## Version 1.1.0
+* Support filtering volumes by account id and type name.
+
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-volumes-1.1.0/README.md` & `heaserver_volumes-1.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # HEA Volumes Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Volumes Microservice The HEA volumes service.
 
+## Version 1.2.0
+* Hid some attributes from the heaobject.volume.Volume properties card.
+* Added account_id attribute to the heaobject.volume.Volume properties card.
+* Removed the type name filter from volume queries. We now use heaobject.account.AccountView ids for the account id
+filter.
+
+## Version 1.1.0
+* Support filtering volumes by account id and type name.
+
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-volumes-1.1.0/RELEASING.md` & `heaserver_volumes-1.2.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py` & `heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all.py` & `heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py` & `heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/integrationtests/heaserver/volumeintegrationtest/testcase.py` & `heaserver_volumes-1.2.0/integrationtests/heaserver/volumeintegrationtest/testcase.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,89 +8,95 @@
 from heaobject.user import NONE_USER
 from heaserver.service.testcase.expectedvalues import Action, Link
 from heaserver.service.testcase.dockermongo import RealRegistryContainerConfig
 
 db_store = {
     service.MONGODB_VOLUME_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus',
         'invites': [],
         'shares': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'heaobject.volume.MongoDBFileSystem^DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': '666f6f2d6261722d71757578',
         'mime_type': 'application/x.volume',
         'credential_id': None,
-        'account': None
+        'credential_type_name': None,
+        'account_id': None,
+        'type_display_name': 'Volume'
     },
     {
         'id': '0123456789ab0123456789ab',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Luximus',
         'invites': [],
         'shares': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'heaobject.volume.AWSFileSystem^DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': '0123456789ab0123456789ab',
         'mime_type': 'application/x.volume',
         'credential_id': None,
-        'account': None
+        'credential_type_name': None,
+        'account_id': None,
+        'type_display_name': 'Volume'
     }],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': 'Access to Amazon Web Services (AWS)',
         'display_name': 'Amazon Web Services',
         'invites': [],
         'shares': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
-        'type': 'heaobject.volume.AWSFileSystem'
+        'type': 'heaobject.volume.AWSFileSystem',
+        'type_display_name': 'AWS File System'
     },
         {
             'id': '0123456789ab0123456789ab',
-            'created': None,
+            'created': '2022-05-17T00:00:00+00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Local MongoDB instance',
             'invites': [],
             'shares': [],
-            'modified': None,
+            'modified': '2022-05-17T00:00:00+00:00',
             'name': 'DEFAULT_FILE_SYSTEM',
             'owner': NONE_USER,
             'source': None,
             'source_detail': None,
             'type': 'heaobject.volume.MongoDBFileSystem',
             'database_name': 'hea',
-            'connection_string': 'mongodb://heauser:heauser@localhost:27017/hea'
+            'connection_string': 'mongodb://heauser:heauser@localhost:27017/hea',
+            'type_display_name': 'MongoDB File System'
         }],
     'folders': [{
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus',
@@ -192,24 +198,30 @@
                                    get_actions=[Action(name='heaserver-volumes-volume-get-properties',
                                                        rel=['hea-properties']),
                                                 Action(name='heaserver-volumes-volume-get-open-choices',
                                                        url='http://localhost:8080/volumes/{id}/opener',
                                                        rel=['hea-opener-choices']),
                                                 Action(name='heaserver-volumes-volume-duplicate',
                                                        url='http://localhost:8080/volumes/{id}/duplicator',
-                                                       rel=['hea-duplicator'])
+                                                       rel=['hea-duplicator']),
+                                                Action(name='heaserver-volumes-volume-get-self',
+                                                       url='http://localhost:8080/volumes/{id}',
+                                                       rel=['self'])
                                                 ],
                                    get_all_actions=[Action(name='heaserver-volumes-volume-get-properties',
                                                            rel=['hea-properties']),
                                                     Action(name='heaserver-volumes-volume-get-open-choices',
                                                            url='http://localhost:8080/volumes/{id}/opener',
                                                            rel=['hea-opener-choices']),
                                                     Action(name='heaserver-volumes-volume-duplicate',
                                                            url='http://localhost:8080/volumes/{id}/duplicator',
-                                                           rel=['hea-duplicator'])],
+                                                           rel=['hea-duplicator']),
+                                                    Action(name='heaserver-volumes-volume-get-self',
+                                                        url='http://localhost:8080/volumes/{id}',
+                                                        rel=['self'])],
                                    expected_opener=Link(
                                        url=f'http://localhost:8080/volumes/{db_store[service.MONGODB_VOLUME_COLLECTION][0]["id"]}/content',
                                        rel=['hea-opener', 'hea-default', 'application/x.folder']),
                                    duplicate_action_name='heaserver-volumes-volume-duplicate-form',
                                    registry_docker_image=RealRegistryContainerConfig(HEASERVER_REGISTRY_IMAGE),
                                    put_content_status=405)
```

### Comparing `heaserver-volumes-1.1.0/run-swaggerui.py` & `heaserver_volumes-1.2.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/setup.py` & `heaserver_volumes-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-volumes',
-    version='1.1.0',
+    version='1.2.0',
     description="The HEA volumes service",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.volume'],
     package_data={'heaserver.volume': ['wstl/*.json']},
-    install_requires=['heaserver~=1.2.0'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver-volumes-1.1.0/src/heaserver/volume/service.py` & `heaserver_volumes-1.2.0/src/heaserver/volume/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 """
 The HEA Volumes Microservice provides ...
 """
-import logging
 
 from heaobject.folder import Folder, Item
 from heaserver.service import client, response, appproperty
 from heaserver.service.appproperty import HEA_DB, HEA_CACHE
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.db import mongo, mongoservicelib
 from heaserver.service.wstl import builder_factory, action
@@ -33,14 +32,15 @@
     return await mongoservicelib.ping(request)
 
 
 @routes.get('/volumes/{id}')
 @action('heaserver-volumes-volume-get-properties', rel='hea-properties')
 @action('heaserver-volumes-volume-get-open-choices', rel='hea-opener-choices', path='volumes/{id}/opener')
 @action('heaserver-volumes-volume-duplicate', rel='hea-duplicator', path='volumes/{id}/duplicator')
+@action('heaserver-volumes-volume-get-self', rel='self', path='volumes/{id}')
 async def get_volume(request: web.Request) -> web.Response:
     """
     Gets the volume with the specified id.
     :param request: the HTTP request.
     :return: the requested volume or Not Found.
     ---
     summary: A specific volume.
@@ -78,17 +78,17 @@
     """
     volume_dict = await request.app[HEA_DB].get(request, MONGODB_VOLUME_COLLECTION, var_parts='id')
     if volume_dict is None:
         return response.status_not_found()
     volume = Volume()
     volume.from_dict(volume_dict)
     for trash_subclass in InVolumeTrashItem.get_subclasses():
-        component = await client.get_component(request.app, trash_subclass, volume.file_system_type, volume.file_system_name)
+        component = await client.get_component(request.app, trash_subclass)
         if component is not None:
-            resource = component.get_external_resource_url(trash_subclass.get_type_name(), volume.file_system_name)
+            resource = component.get_external_resource_url(trash_subclass.get_type_name())
             return response.status_moved(location=resource)
     return response.status_not_found()
 
 
 @routes.get('/volumes/{id}/content')
 async def get_volume_content(request: web.Request) -> web.Response:
     """
@@ -111,17 +111,17 @@
     if volume_dict is None:
         return response.status_not_found()
     volume = Volume()
     volume.from_dict(volume_dict)
     if volume.folder_id is None:
         return response.status_not_found()
     headers = {SUB: request.headers[SUB]} if SUB in request.headers else None
-    url = await type_to_resource_url(request, Folder, volume.file_system_type, volume.file_system_name)
+    url = await type_to_resource_url(request, Folder)
     if url is None:
-        raise ValueError(f'No folder service registered for file system type {volume.file_system_type} and file system name {volume.file_system_name}')
+        raise ValueError(f'No folder service registered')
     items = [i.to_dict() async for i in client.get_all(request.app, URL(url) / volume.folder_id / 'items', Item, headers=headers)]
     return await response.get_all(request, items)
 
 
 @routes.get('/volumes/byname/{name}')
 async def get_volume_by_name(request: web.Request) -> web.Response:
     """
@@ -154,35 +154,30 @@
 
 
 @routes.get('/volumes')
 @routes.get('/volumes/')
 @action('heaserver-volumes-volume-get-properties', rel='hea-properties')
 @action('heaserver-volumes-volume-get-open-choices', rel='hea-opener-choices', path='volumes/{id}/opener')
 @action('heaserver-volumes-volume-duplicate', rel='hea-duplicator', path='volumes/{id}/duplicator')
+@action('heaserver-volumes-volume-get-self', rel='self', path='volumes/{id}')
 async def get_all_volumes(request: web.Request) -> web.Response:
     """
     Gets all volumes.
     :param request: the HTTP request.
     :return: all volumes.
     ---
     summary: All volumes.
     tags:
         - heaserver-volumes-get-all-volumes
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    account_ids = request.query.getall('account_id', None)
-    account_type_names = request.query.getall('account_type_name', None)
-    if account_ids is not None and len(account_ids) != len(account_type_names):
-        return response.status_bad_request('Every account_id must have a corresponding account_type_name')
-    if account_ids:
-        mongoattributes = {'$or': [{'$and': [{'account.actual_object_id': account_id,
-                                              'account.actual_object_type_name': account_type_names[i]
-                                              }]} for i, account_id in enumerate(account_ids)]}
+    if account_ids := request.query.getall('account_id', None):
+        mongoattributes = {'$or': [{'account_id': account_id} for account_id in account_ids]}
     else:
         mongoattributes = None
     return await mongoservicelib.get_all(request, MONGODB_VOLUME_COLLECTION, mongoattributes=mongoattributes)
 
 
 @routes.get('/volumes/{id}/duplicator')
 @action(name='heaserver-volumes-volume-duplicate-form', path='volumes/{id}')
@@ -581,21 +576,16 @@
     """
     type_ = request.match_info['type']
     sub = request.headers.get(SUB, NONE_USER)
     account_ids = request.query.getall('account_id', None)
     cache_key = (sub, MONGODB_VOLUME_COLLECTION, None, f'file_system_type^{type_}', f'file_system_name^DEFAULT_FILE_SYSTEM')
     objs = request.app[HEA_CACHE].get(cache_key) if account_ids is None else None
     if objs is None:
-        account_type_names = request.query.getall('account_type_name', None)
-        if account_ids is not None and len(account_ids) != len(account_type_names):
-            return response.status_bad_request('Every account_id must have a corresponding account_type_name')
         if account_ids:
-            mongoattributes = {'$or': [{'$and': [{'account.actual_object_id': account_id,
-                                                  'account.actual_object_type_name': account_type_names[i]
-                                                  }]} for i, account_id in enumerate(account_ids)]}
+            mongoattributes = {'$or': [{'account_id': account_id} for account_id in account_ids]}
         else:
             mongoattributes = {}
         mongoattributes.update({'file_system_type': {'$eq': request.match_info['type']},
                                 'file_system_name': {'$eq': 'DEFAULT_FILE_SYSTEM'}})
         objs = []
         async for obj in request.app[appproperty.HEA_DB].get_all(request, MONGODB_VOLUME_COLLECTION,
                                                                  mongoattributes=mongoattributes, sub=sub):
@@ -973,12 +963,11 @@
       '204':
         $ref: '#/components/responses/204'
       '404':
         $ref: '#/components/responses/404'
     """
     return await mongoservicelib.delete(request, MONGODB_FILE_SYSTEM_COLLECTION)
 
-
 def main() -> None:
-    config = init_cmd_line(description='The HEA volumes service',
-                           default_port=8080)
-    start(package_name='heaserver-volumes', db=mongo.MongoManager, wstl_builder_factory=builder_factory(__package__), config=config)
+    config = init_cmd_line(description='The HEA volumes service', default_port=8080)
+    start(package_name='heaserver-volumes',
+          db=mongo.MongoManager, wstl_builder_factory=builder_factory(__package__), config=config)
```

### Comparing `heaserver-volumes-1.1.0/src/heaserver/volume/wstl/all.json` & `heaserver_volumes-1.2.0/src/heaserver/volume/wstl/all.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9874043367346939%*

 * *Differences: {"'wstl'": "{'actions': {4: {'inputs': {0: {'hea': OrderedDict([('display', False)])}, 1: {'hea': "*

 * *           "OrderedDict([('display', False)])}, insert: [(6, OrderedDict([('name', 'account_id'), "*

 * *           "('prompt', 'Account'), ('type', 'select'), ('hea', OrderedDict([('optionsFromUrl', "*

 * *           "OrderedDict([('path', 'accounts/'), ('value', 'id'), ('text', "*

 * *           "'display_name')]))]))]))]}}, insert: [(5, OrderedDict([('name', "*

 * *           "'heaserver-volumes-volume-get-self'), ('descripti […]*

```diff
@@ -30,19 +30,25 @@
                 "type": "safe"
             },
             {
                 "action": "update",
                 "description": "View and edit this volume's properties",
                 "inputs": [
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "id",
                         "prompt": "Id",
                         "readOnly": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "name",
                         "prompt": "Name",
                         "readOnly": true
                     },
                     {
                         "name": "display_name",
                         "prompt": "Name",
@@ -62,14 +68,26 @@
                         "name": "file_system_name",
                         "prompt": "File System Name",
                         "required": true
                     },
                     {
                         "hea": {
                             "optionsFromUrl": {
+                                "path": "accounts/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "account_id",
+                        "prompt": "Account",
+                        "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "optionsFromUrl": {
                                 "path": "credentials/",
                                 "text": "display_name",
                                 "value": "id"
                             }
                         },
                         "name": "credential_id",
                         "prompt": "Credentials",
@@ -161,14 +179,22 @@
                 ],
                 "name": "heaserver-volumes-volume-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
             {
+                "action": "read",
+                "description": "View this person",
+                "name": "heaserver-volumes-volume-get-self",
+                "prompt": "View",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
                 "action": "update",
                 "description": "Duplicate this volume",
                 "inputs": [
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "required": true
```

### Comparing `heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/PKG-INFO` & `heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-volumes
-Version: 1.1.0
+Version: 1.2.0
 Summary: The HEA volumes service
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-volumes,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,32 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.2.0
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Volumes Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Volumes Microservice The HEA volumes service.
 
+## Version 1.2.0
+* Hid some attributes from the heaobject.volume.Volume properties card.
+* Added account_id attribute to the heaobject.volume.Volume properties card.
+* Removed the type name filter from volume queries. We now use heaobject.account.AccountView ids for the account id
+filter.
+
+## Version 1.1.0
+* Support filtering volumes by account id and type name.
+
+
 ## Version 1.0.2
 * Improved performance.
 
 ## Version 1.0.1
 * Improved performance.
 
 ## Version 1
```

### Comparing `heaserver-volumes-1.1.0/src/heaserver_volumes.egg-info/SOURCES.txt` & `heaserver_volumes-1.2.0/src/heaserver_volumes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/tests/heaserver/volumetest/permissionstestcase.py` & `heaserver_volumes-1.2.0/tests/heaserver/volumetest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all.py` & `heaserver_volumes-1.2.0/tests/heaserver/volumetest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py` & `heaserver_volumes-1.2.0/tests/heaserver/volumetest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-volumes-1.1.0/tests/heaserver/volumetest/testcase.py` & `heaserver_volumes-1.2.0/tests/heaserver/volumetest/testcase.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,15 +25,17 @@
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.MongoDBFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': None,
         'mime_type': 'application/x.volume',
         'credential_id': None,
-        'account': None
+        'credential_type_name': None,
+        'type_display_name': 'Volume',
+        'account_id': None
     },
     {
         'id': '0123456789ab0123456789ab',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -47,15 +49,17 @@
         'source_detail': None,
         'type': 'heaobject.volume.Volume',
         'file_system_type': 'heaobject.volume.AWSFileSystem',
         'file_system_name': 'DEFAULT_FILE_SYSTEM',
         'folder_id': None,
         'mime_type': 'application/x.volume',
         'credential_id': None,
-        'account': None
+        'credential_type_name': None,
+        'type_display_name': 'Volume',
+        'account_id': None
     }],
     service.MONGODB_FILE_SYSTEM_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': 'Access to Amazon Web Services (AWS)',
@@ -63,15 +67,16 @@
         'invites': [],
         'modified': None,
         'name': 'DEFAULT_FILE_SYSTEM',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.AWSFileSystem',
-        'shares': []
+        'shares': [],
+        'type_display_name': 'AWS File System'
     },
     {
         'id': '0123456789ab0123456789ab',
         'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
@@ -81,15 +86,16 @@
         'name': 'local_mongodb_file_system',
         'owner': NONE_USER,
         'source': None,
         'source_detail': None,
         'type': 'heaobject.volume.MongoDBFileSystem',
         'database_name': 'hea',
         'connection_string': 'mongodb://heauser:heauser@localhost:27017/hea',
-        'shares': []
+        'shares': [],
+        'type_display_name': 'MongoDB File System'
     }]
 }
 
 
 def get_test_case_cls(*args, **kwargs):
     """Get a test case class specifically for this microservice."""
     class MyTestCase(get_test_case_cls_default(*args, **kwargs)):
@@ -111,24 +117,30 @@
                                    get_actions=[Action(name='heaserver-volumes-volume-get-properties',
                                                        rel=['hea-properties']),
                                                 Action(name='heaserver-volumes-volume-get-open-choices',
                                                        url='http://localhost:8080/volumes/{id}/opener',
                                                        rel=['hea-opener-choices']),
                                                 Action(name='heaserver-volumes-volume-duplicate',
                                                        url='http://localhost:8080/volumes/{id}/duplicator',
-                                                       rel=['hea-duplicator'])
+                                                       rel=['hea-duplicator']),
+                                                Action(name='heaserver-volumes-volume-get-self',
+                                                       url='http://localhost:8080/volumes/{id}',
+                                                       rel=['self'])
                                                 ],
                                    get_all_actions=[Action(name='heaserver-volumes-volume-get-properties',
                                                            rel=['hea-properties']),
                                                     Action(name='heaserver-volumes-volume-get-open-choices',
                                                            url='http://localhost:8080/volumes/{id}/opener',
                                                            rel=['hea-opener-choices']),
                                                     Action(name='heaserver-volumes-volume-duplicate',
                                                            url='http://localhost:8080/volumes/{id}/duplicator',
-                                                           rel=['hea-duplicator'])],
+                                                           rel=['hea-duplicator']),
+                                                    Action(name='heaserver-volumes-volume-get-self',
+                                                        url='http://localhost:8080/volumes/{id}',
+                                                        rel=['self'])],
                                    expected_opener=expectedvalues.Link(
                                        url=f'http://localhost:8080/volumes/{db_store[service.MONGODB_VOLUME_COLLECTION][0]["id"]}/content',
                                        rel=['hea-opener', 'hea-default', 'application/x.folder']),
                                    duplicate_action_name='heaserver-volumes-volume-duplicate-form',
                                    put_content_status=405)
 
 FileSystemTestCase = get_test_case_cls(coll=service.MONGODB_FILE_SYSTEM_COLLECTION,
```

