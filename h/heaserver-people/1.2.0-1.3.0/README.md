# Comparing `tmp/heaserver_people-1.2.0.tar.gz` & `tmp/heaserver_people-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_people-1.2.0.tar", last modified: Thu Apr 18 03:45:58 2024, max compression
+gzip compressed data, was "heaserver_people-1.3.0.tar", last modified: Tue May 21 23:18:55 2024, max compression
```

## Comparing `heaserver_people-1.2.0.tar` & `heaserver_people-1.3.0.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.826035 heaserver_people-1.2.0/
--rw-rw-rw-   0        0        0      261 2023-12-18 20:25:25.000000 heaserver_people-1.2.0/.editorconfig
--rw-rw-rw-   0        0        0      353 2023-12-18 20:25:25.000000 heaserver_people-1.2.0/.gitignore
--rw-rw-rw-   0        0        0    11625 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5270 2024-04-18 03:45:58.824036 heaserver_people-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3912 2024-04-18 03:44:27.000000 heaserver_people-1.2.0/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.760036 heaserver_people-1.2.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.781083 heaserver_people-1.2.0/integrationtests/.pytest_cache/
--rw-rw-rw-   0        0        0       39 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/.gitignore
--rw-rw-rw-   0        0        0      194 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/CACHEDIR.TAG
--rw-rw-rw-   0        0        0      303 2023-02-23 16:41:17.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/README.md
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.759065 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.784036 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/nodeids
--rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.2.0/integrationtests/.pytest_cache/v/cache/stepwise
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.760036 heaserver_people-1.2.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.789035 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     4674 2024-04-11 18:14:29.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      547 2024-02-25 02:42:01.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     7893 2024-04-11 18:14:17.000000 heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      111 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 03:45:58.826035 heaserver_people-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1854 2024-04-18 03:45:10.000000 heaserver_people-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.762034 heaserver_people-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.761068 heaserver_people-1.2.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.798035 heaserver_people-1.2.0/src/heaserver/person/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/src/heaserver/person/__init__.py
--rw-rw-rw-   0        0        0     4121 2024-02-25 02:42:01.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmockmongotestcase.py
--rw-rw-rw-   0        0        0    27189 2024-04-17 03:50:10.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmongo.py
--rw-rw-rw-   0        0        0    10027 2024-03-26 23:05:06.000000 heaserver_people-1.2.0/src/heaserver/person/keycloakmongotestcase.py
--rw-rw-rw-   0        0        0    16645 2024-04-11 22:04:52.000000 heaserver_people-1.2.0/src/heaserver/person/service.py
--rw-rw-rw-   0        0        0     1772 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/src/heaserver/person/testcasedata.py
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.799080 heaserver_people-1.2.0/src/heaserver/person/wstl/
--rw-rw-rw-   0        0        0    14175 2024-04-11 22:04:18.000000 heaserver_people-1.2.0/src/heaserver/person/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.823037 heaserver_people-1.2.0/src/heaserver_people.egg-info/
--rw-rw-rw-   0        0        0     5270 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1289 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       67 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 03:45:58.000000 heaserver_people-1.2.0/src/heaserver_people.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.763038 heaserver_people-1.2.0/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.763038 heaserver_people-1.2.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 03:45:58.821041 heaserver_people-1.2.0/tests/heaserver/persontest/
--rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/tests/heaserver/persontest/__init__.py
--rw-rw-rw-   0        0        0     4010 2024-04-11 18:14:03.000000 heaserver_people-1.2.0/tests/heaserver/persontest/permissionstestcase.py
--rw-rw-rw-   0        0        0     1343 2023-12-18 20:25:26.000000 heaserver_people-1.2.0/tests/heaserver/persontest/test_all.py
--rw-rw-rw-   0        0        0     7195 2024-04-11 18:13:51.000000 heaserver_people-1.2.0/tests/heaserver/persontest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.266333 heaserver_people-1.3.0/
+-rw-rw-rw-   0        0        0      261 2023-12-18 20:25:25.000000 heaserver_people-1.3.0/.editorconfig
+-rw-rw-rw-   0        0        0      353 2023-12-18 20:25:25.000000 heaserver_people-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0    11625 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5966 2024-05-21 23:18:55.264332 heaserver_people-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4608 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.206668 heaserver_people-1.3.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.229771 heaserver_people-1.3.0/integrationtests/.pytest_cache/
+-rw-rw-rw-   0        0        0       39 2023-02-23 16:41:17.000000 heaserver_people-1.3.0/integrationtests/.pytest_cache/.gitignore
+-rw-rw-rw-   0        0        0      194 2023-02-23 16:41:17.000000 heaserver_people-1.3.0/integrationtests/.pytest_cache/CACHEDIR.TAG
+-rw-rw-rw-   0        0        0      303 2023-02-23 16:41:17.000000 heaserver_people-1.3.0/integrationtests/.pytest_cache/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.205675 heaserver_people-1.3.0/integrationtests/.pytest_cache/v/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.231774 heaserver_people-1.3.0/integrationtests/.pytest_cache/v/cache/
+-rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.3.0/integrationtests/.pytest_cache/v/cache/nodeids
+-rw-rw-rw-   0        0        0        2 2023-02-23 16:42:55.000000 heaserver_people-1.3.0/integrationtests/.pytest_cache/v/cache/stepwise
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.206668 heaserver_people-1.3.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.237774 heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     4674 2024-04-18 03:47:11.000000 heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      547 2024-02-25 02:42:01.000000 heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     9139 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-05-21 23:18:55.266333 heaserver_people-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1854 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.209669 heaserver_people-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.208669 heaserver_people-1.3.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.246775 heaserver_people-1.3.0/src/heaserver/person/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/src/heaserver/person/__init__.py
+-rw-rw-rw-   0        0        0     4121 2024-02-25 02:42:01.000000 heaserver_people-1.3.0/src/heaserver/person/keycloakmockmongotestcase.py
+-rw-rw-rw-   0        0        0    40214 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/src/heaserver/person/keycloakmongo.py
+-rw-rw-rw-   0        0        0    10027 2024-03-26 23:05:06.000000 heaserver_people-1.3.0/src/heaserver/person/keycloakmongotestcase.py
+-rw-rw-rw-   0        0        0    19534 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/src/heaserver/person/service.py
+-rw-rw-rw-   0        0        0     2114 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/src/heaserver/person/testcasedata.py
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.247773 heaserver_people-1.3.0/src/heaserver/person/wstl/
+-rw-rw-rw-   0        0        0    16523 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/src/heaserver/person/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.263330 heaserver_people-1.3.0/src/heaserver_people.egg-info/
+-rw-rw-rw-   0        0        0     5966 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1289 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       67 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-21 23:18:55.000000 heaserver_people-1.3.0/src/heaserver_people.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.210670 heaserver_people-1.3.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.210670 heaserver_people-1.3.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-21 23:18:55.261331 heaserver_people-1.3.0/tests/heaserver/persontest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/tests/heaserver/persontest/__init__.py
+-rw-rw-rw-   0        0        0     4010 2024-04-18 03:47:11.000000 heaserver_people-1.3.0/tests/heaserver/persontest/permissionstestcase.py
+-rw-rw-rw-   0        0        0     1343 2023-12-18 20:25:26.000000 heaserver_people-1.3.0/tests/heaserver/persontest/test_all.py
+-rw-rw-rw-   0        0        0     8461 2024-05-21 23:18:19.000000 heaserver_people-1.3.0/tests/heaserver/persontest/testcase.py
```

### Comparing `heaserver_people-1.2.0/LICENSE` & `heaserver_people-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/PKG-INFO` & `heaserver_people-1.3.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.2.0
+Version: 1.3.0
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,35 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.4.0
+* Changed /groups and /roles to get all groups and roles.
+* New API for modifying a person's groups.
+* Fixed caching issue.
+* Include system users in /people calls by default, but permit omitting them with the excludesystem query parameter.
+* Group objects now have a group_type attribute to differentiate between ADMIN groups (starting with /*) and
+ORGANIZATION groups (everything else, currently).
+* Don't allow access to data modifying admin APIs unless you're the system|credentialsmanager, or the affected person
+(for calls to add/remove groups to/from a person).
+
+## Version 1.3.0
+* Display type display name in properties card, and return it from GET calls.
+
 ## Version 1.2.0
 * Added /groups endpoint.
 * Corrected 500 error with /roles endpoint in some circumstances.
 
 ## Version 1.1.0
 * System users are now included in the people API calls.
```

### Comparing `heaserver_people-1.2.0/README.md` & `heaserver_people-1.3.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.4.0
+* Changed /groups and /roles to get all groups and roles.
+* New API for modifying a person's groups.
+* Fixed caching issue.
+* Include system users in /people calls by default, but permit omitting them with the excludesystem query parameter.
+* Group objects now have a group_type attribute to differentiate between ADMIN groups (starting with /*) and
+ORGANIZATION groups (everything else, currently).
+* Don't allow access to data modifying admin APIs unless you're the system|credentialsmanager, or the affected person
+(for calls to add/remove groups to/from a person).
+
+## Version 1.3.0
+* Display type display name in properties card, and return it from GET calls.
+
 ## Version 1.2.0
 * Added /groups endpoint.
 * Corrected 500 error with /roles endpoint in some circumstances.
 
 ## Version 1.1.0
 * System users are now included in the people API calls.
```

### Comparing `heaserver_people-1.2.0/RELEASING.md` & `heaserver_people-1.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py` & `heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/test_all.py` & `heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/integrationtests/heaserver/personintegrationtest/testcase.py` & `heaserver_people-1.3.0/tests/heaserver/persontest/testcase.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,98 +1,109 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
 
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
 from heaserver.person import service
-from heaserver.service.testcase.dockermongo import RealRegistryContainerConfig
-from heaserver.person.keycloakmongotestcase import KeycloakMongoManagerForPyTest
-from heaobject.user import NONE_USER, ALL_USERS
-from heaobject.person import Person, get_system_people
+from heaobject.user import NONE_USER, ALL_USERS, CREDENTIALS_MANAGER_USER
 from heaserver.service.testcase.expectedvalues import Action
-from heaserver.service.testcase.collection import CollectionKey
-
+from heaserver.person.keycloakmockmongotestcase import KeycloakMockMongoManager
 
 db_store = {
-    CollectionKey(name=service.MONGODB_PERSON_COLLECTION, db_manager_cls=KeycloakMongoManagerForPyTest): [{
-        'id': '666f6f2d6261722d71757578',
-        'created': None,
+    service.MONGODB_PERSON_COLLECTION: [{
+        'id': 'system|none',
+        'created': '2022-01-01T00:00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus Max',
         'invites': [],
         'modified': None,
-        'name': 'reximus',
+        'name': 'reximusmax',
         'owner': NONE_USER,
         'shares': [{
-            'invite': None,
-            'permissions': ['VIEWER'],
-            'type': 'heaobject.root.ShareImpl',
-            'user': ALL_USERS
-        }],
-        'source': 'Keycloak',
+                'invite': None,
+                'permissions': ['VIEWER'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': ALL_USERS
+            }, {
+                'invite': None,
+                'permissions': ['EDITOR'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': CREDENTIALS_MANAGER_USER
+            }],
+        'source': None,
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Max',
-        'type': Person.get_type_name(),
+        'full_name': 'Reximus Max',
+        'type': 'heaobject.person.Person',
+        'title': None,
         'phone_number': None,
         'preferred_name': None,
-        'email': 'reximus.max@example.com',
-        'title': None,
-        'type_display_name': 'Person'
+        'email': None,
+        'type_display_name': 'Person',
+        'group_ids': []
     },
         {
-            'id': '0123456789ab0123456789ab',
-            'created': None,
+            'id': 'system|test',
+            'created': '2022-01-01T00:00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Luximus Max',
             'invites': [],
             'modified': None,
-            'name': 'luximus',
+            'name': 'luximusmax',
             'owner': NONE_USER,
             'shares': [{
                 'invite': None,
                 'permissions': ['VIEWER'],
                 'type': 'heaobject.root.ShareImpl',
                 'user': ALL_USERS
+            }, {
+                'invite': None,
+                'permissions': ['EDITOR'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': CREDENTIALS_MANAGER_USER
             }],
-            'source': 'Keycloak',
+            'source': None,
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Max',
-            'type': Person.get_type_name(),
+            'full_name': 'Luximus Max',
+            'type': 'heaobject.person.Person',
+            'title': None,
             'phone_number': None,
             'preferred_name': None,
-            'email': 'luximus.max@example.com',
-            'title': None,
-            'type_display_name': 'Person'
-        }] + [system_person.to_dict() for system_person in get_system_people()]}
-
-HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
+            'email': None,
+            'type_display_name': 'Person',
+            'group_ids': []
+        }]}
 
 
 TestCase = get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
-                                     href='http://localhost:8080/people',
                                      wstl_package=service.__package__,
-                                     db_manager_cls=KeycloakMongoManagerForPyTest,
+                                     db_manager_cls=KeycloakMockMongoManager,
+                                     href='http://localhost:8080/people',
                                      fixtures=db_store,
                                      get_actions=[Action(name='heaserver-people-person-get-properties',
                                                          rel=['hea-properties']),
                                                   Action(name='heaserver-people-person-get-self',
                                                          url='http://localhost:8080/people/{id}',
                                                          rel=['self']),
                                                   Action(name='heaserver-people-person-get-settings',
-                                                         url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
-                                                         rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
+                                                             url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
+                                                             rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
                                                   # Action(name='heaserver-people-person-get-organization-collection',
                                                   #        url='http://localhost:8080/collections/heaobject.organization.Organization',
                                                   #        rel=['hea-system-menu-item', 'application/x.collection']),
+                                                  Action(name='heaserver-people-person-get-volumes-collection',
+                                                         url='http://localhost:8080/collections/heaobject.volume.Volume',
+                                                         rel=['hea-system-menu-item', 'application/x.collection']),
                                                   Action(name='heaserver-people-person-get-organizations',
                                                          url='http://localhost:8080/organizations/',
                                                          rel=['application/x.organization']),
                                                   Action(name='heaserver-people-person-get-volumes',
                                                          url='http://localhost:8080/volumes/',
                                                          rel=['application/x.volume']),
                                                   Action(name='heaserver-people-person-get-desktop-object-actions',
@@ -106,20 +117,21 @@
                                                              rel=['self']),
                                                       Action(name='heaserver-people-person-get-settings',
                                                              url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
                                                              rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
                                                       # Action(name='heaserver-people-person-get-organization-collection',
                                                       #        url='http://localhost:8080/collections/heaobject.organization.Organization',
                                                       #        rel=['hea-system-menu-item', 'application/x.collection']),
+                                                      Action(name='heaserver-people-person-get-volumes-collection',
+                                                         url='http://localhost:8080/collections/heaobject.volume.Volume',
+                                                         rel=['hea-system-menu-item', 'application/x.collection']),
                                                       Action(name='heaserver-people-person-get-organizations',
                                                              url='http://localhost:8080/organizations/',
                                                              rel=['application/x.organization']),
                                                       Action(name='heaserver-people-person-get-volumes',
                                                              url='http://localhost:8080/volumes/',
                                                              rel=['application/x.volume']),
                                                       Action(name='heaserver-people-person-get-desktop-object-actions',
                                                              url='http://localhost:8080/desktopobjectactions/',
-                                                             rel=['application/x.desktopobjectaction'])
-                                                      ],
-                                     registry_docker_image=RealRegistryContainerConfig(HEASERVER_REGISTRY_IMAGE),
-                                     duplicate_action_name='heaserver-people-person-duplicate-form',
-                                     exclude=['body_put', 'body_post'])
+                                                             rel=['application/x.desktopobjectaction'])],
+                                     duplicate_action_name=None,
+        exclude=['body_put', 'body_post'])
```

### Comparing `heaserver_people-1.2.0/setup.py` & `heaserver_people-1.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-people',
-    version='1.2.0',
+    version='1.3.0',
     description="A microservice designed to provide CRUD operations for the Person HEA object type",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.person'],
     package_data={'heaserver.person': ['wstl/*.json']},
-    install_requires=['heaserver~=1.4.1'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_people-1.2.0/src/heaserver/person/keycloakmockmongotestcase.py` & `heaserver_people-1.3.0/src/heaserver/person/keycloakmockmongotestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/src/heaserver/person/keycloakmongotestcase.py` & `heaserver_people-1.3.0/src/heaserver/person/keycloakmongotestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/src/heaserver/person/service.py` & `heaserver_people-1.3.0/src/heaserver/person/service.py`

 * *Files 16% similar despite different names*

```diff
@@ -17,15 +17,18 @@
 """
 import logging
 
 from heaserver.service import response
 from heaserver.service.runner import init_cmd_line, routes, start, web
 from heaserver.service.wstl import action, builder_factory
 from heaserver.service import appproperty
+from heaserver.service.heaobjectsupport import new_heaobject_from_type
 from heaserver.service.oidcclaimhdrs import SUB
+from heaobject.error import DeserializeException
+from heaobject.person import Group
 from .keycloakmongo import KeycloakMongoManager
 from heaobject.user import NONE_USER
 from aiohttp import ClientResponseError
 from base64 import urlsafe_b64decode
 from binascii import Error as B64DecodeError
 
 
@@ -43,14 +46,15 @@
 
 
 @routes.get('/people/me')
 @action(name='heaserver-people-person-get-properties', rel='hea-properties')
 @action(name='heaserver-people-person-get-self', rel='self', path='people/{id}')
 @action(name='heaserver-people-person-get-settings', rel='hea-system-menu-item hea-user-menu-item application/x.settingsobject application/x.collection', path='collections/heaobject.settings.SettingsObject')
 #@action(name='heaserver-people-person-get-organization-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.organization.Organization')
+@action(name='heaserver-people-person-get-volumes-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.volume.Volume')
 @action(name='heaserver-people-person-get-organizations', rel='application/x.organization', path='organizations/')
 @action(name='heaserver-people-person-get-volumes', rel='application/x.volume', path='volumes/')
 @action(name='heaserver-people-person-get-desktop-object-actions', rel='application/x.desktopobjectaction', path='desktopobjectactions/')
 async def get_me(request: web.Request) -> web.Response:
     """
     Gets the currently logged in person.
 
@@ -82,14 +86,15 @@
 
 
 @routes.get('/people/{id}')
 @action(name='heaserver-people-person-get-properties', rel='hea-properties')
 @action(name='heaserver-people-person-get-self', rel='self', path='people/{id}')
 @action(name='heaserver-people-person-get-settings', rel='hea-system-menu-item hea-user-menu-item application/x.settingsobject application/x.collection', path='collections/heaobject.settings.SettingsObject')
 #@action(name='heaserver-people-person-get-organization-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.organization.Organization')
+@action(name='heaserver-people-person-get-volumes-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.volume.Volume')
 @action(name='heaserver-people-person-get-organizations', rel='application/x.organization', path='organizations/')
 @action(name='heaserver-people-person-get-volumes', rel='application/x.volume', path='volumes/')
 @action(name='heaserver-people-person-get-desktop-object-actions', rel='application/x.desktopobjectaction', path='desktopobjectactions/')
 async def get_person(request: web.Request) -> web.Response:
     """
     Gets the person with the specified id.
     :param request: the HTTP request.
@@ -154,14 +159,15 @@
 
 @routes.get('/people')
 @routes.get('/people/')
 @action(name='heaserver-people-person-get-properties', rel='hea-properties')
 @action(name='heaserver-people-person-get-self', rel='self', path='people/{id}')
 @action(name='heaserver-people-person-get-settings', rel='hea-system-menu-item hea-user-menu-item application/x.settingsobject application/x.collection', path='collections/heaobject.settings.SettingsObject')
 #@action(name='heaserver-people-person-get-organization-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.organization.Organization')
+@action(name='heaserver-people-person-get-volumes-collection', rel='hea-system-menu-item application/x.collection', path='collections/heaobject.volume.Volume')
 @action(name='heaserver-people-person-get-organizations', rel='application/x.organization', path='organizations/')
 @action(name='heaserver-people-person-get-volumes', rel='application/x.volume', path='volumes/')
 @action(name='heaserver-people-person-get-desktop-object-actions', rel='application/x.desktopobjectaction', path='desktopobjectactions/')
 async def get_all_persons(request: web.Request) -> web.Response:
     """
     Gets all persons.
     :param request: the HTTP request.
@@ -178,35 +184,34 @@
     try:
         persons = await request.app[appproperty.HEA_DB].get_users(request)
         return await response.get_all(request, [person.to_dict() for person in persons],
                                       permissions=[person.get_permissions(sub) for person in persons])
     except ClientResponseError as e:
         return response.status_generic(e.status, body=e.message)
 
-
 @routes.get('/roles')
 @routes.get('/roles/')
 @action(name='heaserver-people-role-get-properties', rel='hea-properties')
 @action(name='heaserver-people-role-get-self', rel='self', path='roles/{id}')
 async def get_all_roles(request: web.Request) -> web.Response:
     """
-    Gets all roles for the current user.
+    Gets all roles that are known to Keycloak.
     :param request: the HTTP request.
     :return: all roles.
     ---
     summary: All roles.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
     sub = request.headers.get(SUB, NONE_USER)
     try:
-        roles = await request.app[appproperty.HEA_DB].get_current_user_roles(request)
+        roles = await request.app[appproperty.HEA_DB].get_all_roles(request)
         return await response.get_all(request, [role.to_dict() for role in roles],
                                       permissions=[role.get_permissions(sub) for role in roles])
     except ClientResponseError as e:
         if e.status == 404:
             return await response.get_all(request, [])
         else:
             return response.status_generic(e.status, body=e.message)
@@ -227,15 +232,15 @@
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
     sub = request.headers.get(SUB, NONE_USER)
     id_ = request.match_info['id']
     try:
-        roles = await request.app[appproperty.HEA_DB].get_current_user_roles(request)
+        roles = await request.app[appproperty.HEA_DB].get_all_roles(request)
         role = next((role for role in roles if role.id == id_), None)
         if role is not None:
             return await response.get(request, role.to_dict(), permissions=role.get_permissions(sub))
         else:
             return await response.get(request, None)
     except ClientResponseError as e:
         if e.status == 404:
@@ -256,60 +261,51 @@
     summary: All roles.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    logger = logging.getLogger(__name__)
-    name_encoded = request.match_info['name']
+    sub = request.headers.get(SUB, NONE_USER)
+    name = request.match_info['name']
     try:
-        name = urlsafe_b64decode(name_encoded).decode('utf-8')
-        if logger.getEffectiveLevel() == logging.DEBUG:
-            logger.debug('match_info %s', request.match_info)
-            logger.debug('headers %s', request.headers)
-            logger.debug('checking role %s', name)
-        has_role = await request.app[appproperty.HEA_DB].has_role_current_user(request, name)
-        if request.method == 'GET':
-            return has_role
-        else:
-            if has_role:
-                return response.status_ok()
-            else:
-                return response.status_not_found()
+        roles = await request.app[appproperty.HEA_DB].get_all_roles(request)
+        role = next((role for role in roles if role.name == name), None)
+        if role is not None:
+            return await response.get(request, role.to_dict(), permissions=role.get_permissions(sub))
+        else:
+            return await response.get(request, None)
     except ClientResponseError as e:
-        logger.exception('Got client response error')
         if e.status == 404:
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
-    except B64DecodeError as e:
-        return response.status_not_found()
-
 
 @routes.get('/groups')
 @routes.get('/groups/')
 @action(name='heaserver-people-group-get-properties', rel='hea-properties')
 @action(name='heaserver-people-group-get-self', rel='self', path='groups/{id}')
 async def get_all_groups(request: web.Request) -> web.Response:
     """
-    Gets all groups for the current user.
+    Gets all groups that are known to Keycloak.
     :param request: the HTTP request.
     :return: all groups.
     ---
     summary: All groups.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
+    logger = logging.getLogger(__name__)
     sub = request.headers.get(SUB, NONE_USER)
     try:
-        groups = await request.app[appproperty.HEA_DB].get_current_user_groups(request)
+        groups = await request.app[appproperty.HEA_DB].get_all_groups(request)
+        logger.debug('groups: %s', groups)
         return await response.get_all(request, [group.to_dict() for group in groups],
                                       permissions=[group.get_permissions(sub) for group in groups])
     except ClientResponseError as e:
         if e.status == 404:
             return await response.get_all(request, [])
         else:
             return response.status_generic(e.status, body=e.message)
@@ -330,27 +326,26 @@
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
     sub = request.headers.get(SUB, NONE_USER)
     id_ = request.match_info['id']
     try:
-        groups = await request.app[appproperty.HEA_DB].get_current_user_groups(request)
+        groups = await request.app[appproperty.HEA_DB].get_all_groups(request)
         group = next((group for group in groups if group.id == id_), None)
         if group is not None:
             return await response.get(request, group.to_dict(), permissions=group.get_permissions(sub))
         else:
             return await response.get(request, None)
     except ClientResponseError as e:
         if e.status == 404:
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
 
-
 @routes.get('/groups/byname/{name}')
 async def get_group_by_name(request: web.Request) -> web.Response:
     """
     Gets the requested group for the current user. Requires an Authorization header with a valid Bearer token, in
     addition to the usual OIDC_CLAIM_sub header.
 
     :param request: the HTTP request.
@@ -359,38 +354,96 @@
     summary: All groups.
     tags:
         - heaserver-people
     responses:
       '200':
         $ref: '#/components/responses/200'
     """
-    logger = logging.getLogger(__name__)
-    name_encoded = request.match_info['name']
+    sub = request.headers.get(SUB, NONE_USER)
+    name = request.match_info['name']
     try:
-        name = urlsafe_b64decode(name_encoded).decode('utf-8')
-        if logger.getEffectiveLevel() == logging.DEBUG:
-            logger.debug('match_info %s', request.match_info)
-            logger.debug('headers %s', request.headers)
-            logger.debug('checking role %s', name)
-        has_group = await request.app[appproperty.HEA_DB].has_group_current_user(request, name)
-        if request.method == 'GET':
-            return has_group
-        else:
-            if has_group:
-                return response.status_ok()
-            else:
-                return response.status_not_found()
+        groups = await request.app[appproperty.HEA_DB].get_all_groups(request)
+        group = next((group for group in groups if group.name == name), None)
+        if group is not None:
+            return await response.get(request, group.to_dict(), permissions=group.get_permissions(sub))
+        else:
+            return await response.get(request, None)
     except ClientResponseError as e:
-        logger.exception('Got client response error')
         if e.status == 404:
             return response.status_not_found()
         else:
             return response.status_generic(e.status, body=e.message)
-    except B64DecodeError as e:
+
+@routes.post('/people/{person_id}/groups')
+@routes.post('/people/{person_id}/groups/')
+async def post_user_group(request: web.Request) -> web.Response:
+    logger = logging.getLogger(__name__)
+    person_id = request.match_info['person_id']
+    try:
+        obj = await new_heaobject_from_type(request, Group)
+    except DeserializeException as e:
+        return response.status_bad_request(str(e))
+    if person_id == 'me':
+        coro = request.app[appproperty.HEA_DB].add_current_user_to_group(request, obj.id)
+    else:
+        coro = request.app[appproperty.HEA_DB].add_user_to_group(request, person_id, obj.id)
+    if result := await coro:
+        return await response.post(request, obj.id if result else None, 'groups')
+    else:
         return response.status_not_found()
 
+@routes.get('/people/{person_id}/groups')
+@routes.get('/people/{person_id}/groups/')
+async def get_user_group(request: web.Request) -> web.Response:
+    """
+    Gets all groups for the current user.
+    :param request: the HTTP request.
+    :return: all groups.
+    ---
+    summary: All groups.
+    tags:
+        - heaserver-people
+    responses:
+      '200':
+        $ref: '#/components/responses/200'
+    """
+    person_id = request.match_info['person_id']
+    sub = request.headers.get(SUB, NONE_USER)
+    try:
+        if person_id == 'me':
+            groups = await request.app[appproperty.HEA_DB].get_current_user_groups(request)
+        else:
+            groups = await request.app[appproperty.HEA_DB].get_user_groups(request, person_id)
+        return await response.get_all(request, [group.to_dict() for group in groups],
+                                      permissions=[group.get_permissions(sub) for group in groups])
+    except ClientResponseError as e:
+        if e.status == 404:
+            return await response.get_all(request, [])
+        else:
+            return response.status_generic(e.status, body=e.message)
+
+@routes.delete('/people/{person_id}/groups/{id}')
+async def delete_user_group(request: web.Request) -> web.Response:
+    id_ = request.match_info['id']
+    person_id = request.match_info['person_id']
+    if person_id == 'me':
+        result = await request.app[appproperty.HEA_DB].remove_current_user_group(request, id_)
+    else:
+        result = await request.app[appproperty.HEA_DB].remove_user_group(request, person_id, id_)
+    return await response.delete(result)
+
+@routes.delete('/people/{person_id}/groups/bygroup/{group}')
+async def delete_group_by_group(request: web.Request) -> web.Response:
+    group = request.match_info['group']
+    person_id = request.match_info['person_id']
+    if person_id == 'me':
+        result = await request.app[appproperty.HEA_DB].remove_current_user_group_by_group(request, group)
+    else:
+        result = await request.app[appproperty.HEA_DB].remove_user_group_by_group(request, person_id, group)
+    return await response.delete(result)
+
 def main() -> None:
     config = init_cmd_line(description='Read-only wrapper around Keycloak for accessing user information.',
                            default_port=8080)
     start(package_name='heaserver-people', db=KeycloakMongoManager, config=config, wstl_builder_factory=builder_factory(__package__))
```

### Comparing `heaserver_people-1.2.0/src/heaserver/person/testcasedata.py` & `heaserver_people-1.3.0/src/heaserver/person/testcasedata.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from heaobject.person import Person
-from heaobject.user import NONE_USER, ALL_USERS
+from heaobject.user import NONE_USER, ALL_USERS, CREDENTIALS_MANAGER_USER
 
 person1 = Person()
 person2 = Person()
 person1.from_dict({
     'id': 'system|none',
     'created': '2022-01-01T00:00:00',
     'derived_by': None,
@@ -15,14 +15,19 @@
     'name': 'reximusmax',
     'owner': NONE_USER,
     'shares': [{
         'invite': None,
         'permissions': ['VIEWER'],
         'type': 'heaobject.root.ShareImpl',
         'user': ALL_USERS
+    }, {
+        'invite': None,
+        'permissions': ['EDITOR'],
+        'type': 'heaobject.root.ShareImpl',
+        'user': CREDENTIALS_MANAGER_USER
     }],
     'source': None,
     'first_name': 'Reximus',
     'last_name': 'Max',
     'type': 'heaobject.person.Person',
     'version': None,
     'title': None,
@@ -46,14 +51,19 @@
     'name': 'luximusmax',
     'owner': NONE_USER,
     'shares': [{
         'invite': None,
         'permissions': ['VIEWER'],
         'type': 'heaobject.root.ShareImpl',
         'user': ALL_USERS
+    }, {
+        'invite': None,
+        'permissions': ['EDITOR'],
+        'type': 'heaobject.root.ShareImpl',
+        'user': CREDENTIALS_MANAGER_USER
     }],
     'source': None,
     'first_name': 'Luximus',
     'last_name': 'Max',
     'type': 'heaobject.person.Person',
     'version': None,
     'title': None,
```

### Comparing `heaserver_people-1.2.0/src/heaserver/person/wstl/all.json` & `heaserver_people-1.3.0/src/heaserver/person/wstl/all.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9904912367724867%*

 * *Differences: {"'wstl'": "{'actions': {6: {'description': 'View and edit organizations'}, 11: {'inputs': {3: "*

 * *           "{'name': 'type_display_name'}, insert: [(2, OrderedDict([('name', 'type'), "*

 * *           "('readOnly', True), ('required', True), ('hea', OrderedDict([('display', False)]))])), "*

 * *           "(17, OrderedDict([('name', 'group_ids'), ('prompt', 'Groups'), ('readOnly', True), "*

 * *           "('type', 'select'), ('hea', OrderedDict([('optionsFromUrl', OrderedDict([('path', "*

 * *           "'groups/'), ('value' […]*

```diff
@@ -43,22 +43,30 @@
                 "name": "heaserver-people-person-get-settings",
                 "prompt": "Settings",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
-                "description": "View and edit this person's organizations",
+                "description": "View and edit organizations",
                 "name": "heaserver-people-person-get-organization-collection",
                 "prompt": "Organizations",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
                 "action": "read",
+                "description": "View and edit volumes",
+                "name": "heaserver-people-person-get-volumes-collection",
+                "prompt": "Volumes",
+                "target": "item read cj",
+                "type": "safe"
+            },
+            {
+                "action": "read",
                 "description": "View and edit this person's organizations",
                 "name": "heaserver-people-person-get-organizations",
                 "prompt": "Organizations",
                 "target": "item read cj",
                 "type": "safe"
             },
             {
@@ -89,15 +97,23 @@
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "readOnly": true,
                         "required": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
                         "name": "type",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
+                        "name": "type_display_name",
                         "prompt": "Type",
                         "readOnly": true,
                         "required": true
                     },
                     {
                         "hea": {
                             "display": false
@@ -231,14 +247,28 @@
                             },
                             {
                                 "text": "Viewer",
                                 "value": "VIEWER"
                             }
                         ],
                         "type": "select"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "optionsFromUrl": {
+                                "path": "groups/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "group_ids",
+                        "prompt": "Groups",
+                        "readOnly": true,
+                        "type": "select"
                     }
                 ],
                 "name": "heaserver-people-person-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
@@ -257,14 +287,22 @@
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "readOnly": true,
                         "required": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "type",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
                         "name": "type_display_name",
                         "prompt": "Type",
                         "readOnly": true,
                         "required": true
                     }
                 ],
                 "name": "heaserver-people-role-get-properties",
@@ -287,18 +325,41 @@
                     {
                         "name": "display_name",
                         "prompt": "Name",
                         "readOnly": true,
                         "required": true
                     },
                     {
+                        "hea": {
+                            "display": false
+                        },
+                        "name": "type",
+                        "readOnly": true,
+                        "required": true
+                    },
+                    {
                         "name": "type_display_name",
                         "prompt": "Type",
                         "readOnly": true,
-                        "required": true
+                        "required": true,
+                        "value": "Person"
+                    },
+                    {
+                        "hea": {
+                            "cardinality": "multiple",
+                            "optionsFromUrl": {
+                                "path": "roles/",
+                                "text": "display_name",
+                                "value": "id"
+                            }
+                        },
+                        "name": "role_ids",
+                        "prompt": "Roles",
+                        "readOnly": true,
+                        "type": "select"
                     }
                 ],
                 "name": "heaserver-people-group-get-properties",
                 "prompt": "Properties",
                 "target": "item cj-template",
                 "type": "unsafe"
             },
```

### Comparing `heaserver_people-1.2.0/src/heaserver_people.egg-info/PKG-INFO` & `heaserver_people-1.3.0/src/heaserver_people.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-people
-Version: 1.2.0
+Version: 1.3.0
 Summary: A microservice designed to provide CRUD operations for the Person HEA object type
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-people,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,35 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Person Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA Person Microservice is A microservice designed to provide CRUD operations for the Person HEA object type.
 
+## Version 1.4.0
+* Changed /groups and /roles to get all groups and roles.
+* New API for modifying a person's groups.
+* Fixed caching issue.
+* Include system users in /people calls by default, but permit omitting them with the excludesystem query parameter.
+* Group objects now have a group_type attribute to differentiate between ADMIN groups (starting with /*) and
+ORGANIZATION groups (everything else, currently).
+* Don't allow access to data modifying admin APIs unless you're the system|credentialsmanager, or the affected person
+(for calls to add/remove groups to/from a person).
+
+## Version 1.3.0
+* Display type display name in properties card, and return it from GET calls.
+
 ## Version 1.2.0
 * Added /groups endpoint.
 * Corrected 500 error with /roles endpoint in some circumstances.
 
 ## Version 1.1.0
 * System users are now included in the people API calls.
```

### Comparing `heaserver_people-1.2.0/src/heaserver_people.egg-info/SOURCES.txt` & `heaserver_people-1.3.0/src/heaserver_people.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/tests/heaserver/persontest/permissionstestcase.py` & `heaserver_people-1.3.0/tests/heaserver/persontest/permissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/tests/heaserver/persontest/test_all.py` & `heaserver_people-1.3.0/tests/heaserver/persontest/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver_people-1.2.0/tests/heaserver/persontest/testcase.py` & `heaserver_people-1.3.0/integrationtests/heaserver/personintegrationtest/testcase.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,115 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
 
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
 from heaserver.person import service
-from heaobject.user import NONE_USER, ALL_USERS
+from heaserver.service.testcase.dockermongo import RealRegistryContainerConfig
+from heaserver.person.keycloakmongotestcase import KeycloakMongoManagerForPyTest
+from heaobject.user import NONE_USER, ALL_USERS, CREDENTIALS_MANAGER_USER
+from heaobject.person import Person, get_system_people
 from heaserver.service.testcase.expectedvalues import Action
-from heaserver.person.keycloakmockmongotestcase import KeycloakMockMongoManager
+from heaserver.service.testcase.collection import CollectionKey
+
 
 db_store = {
-    service.MONGODB_PERSON_COLLECTION: [{
-        'id': 'system|none',
-        'created': '2022-01-01T00:00:00',
+    CollectionKey(name=service.MONGODB_PERSON_COLLECTION, db_manager_cls=KeycloakMongoManagerForPyTest): [{
+        'id': '666f6f2d6261722d71757578',
+        'created': None,
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus Max',
         'invites': [],
         'modified': None,
-        'name': 'reximusmax',
+        'name': 'reximus',
         'owner': NONE_USER,
         'shares': [{
-                'invite': None,
-                'permissions': ['VIEWER'],
-                'type': 'heaobject.root.ShareImpl',
-                'user': ALL_USERS
-            }],
-        'source': None,
+            'invite': None,
+            'permissions': ['VIEWER'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': ALL_USERS
+        }, {
+            'invite': None,
+            'permissions': ['EDITOR'],
+            'type': 'heaobject.root.ShareImpl',
+            'user': CREDENTIALS_MANAGER_USER
+        }],
+        'source': 'Keycloak',
         'source_detail': None,
         'first_name': 'Reximus',
         'last_name': 'Max',
-        'type': 'heaobject.person.Person',
-        'title': None,
+        'full_name': 'Reximus Max',
+        'type': Person.get_type_name(),
         'phone_number': None,
         'preferred_name': None,
-        'email': None,
-        'type_display_name': 'Person'
+        'email': 'reximus.max@example.com',
+        'title': None,
+        'type_display_name': 'Person',
+        'group_ids': []
     },
         {
-            'id': 'system|test',
-            'created': '2022-01-01T00:00:00',
+            'id': '0123456789ab0123456789ab',
+            'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Luximus Max',
             'invites': [],
             'modified': None,
-            'name': 'luximusmax',
+            'name': 'luximus',
             'owner': NONE_USER,
             'shares': [{
                 'invite': None,
                 'permissions': ['VIEWER'],
                 'type': 'heaobject.root.ShareImpl',
                 'user': ALL_USERS
+            }, {
+                'invite': None,
+                'permissions': ['EDITOR'],
+                'type': 'heaobject.root.ShareImpl',
+                'user': CREDENTIALS_MANAGER_USER
             }],
-            'source': None,
+            'source': 'Keycloak',
             'source_detail': None,
             'first_name': 'Luximus',
             'last_name': 'Max',
-            'type': 'heaobject.person.Person',
-            'title': None,
+            'full_name': 'Luximus Max',
+            'type': Person.get_type_name(),
             'phone_number': None,
             'preferred_name': None,
-            'email': None,
-            'type_display_name': 'Person'
-        }]}
+            'email': 'luximus.max@example.com',
+            'title': None,
+            'type_display_name': 'Person',
+            'group_ids': []
+        }] + [system_person.to_dict() for system_person in get_system_people()]}
+
+HEASERVER_REGISTRY_IMAGE = 'registry.gitlab.com/huntsman-cancer-institute/risr/hea/heaserver-registry:1.0.0'
 
 
 TestCase = get_test_case_cls_default(coll=service.MONGODB_PERSON_COLLECTION,
-                                     wstl_package=service.__package__,
-                                     db_manager_cls=KeycloakMockMongoManager,
                                      href='http://localhost:8080/people',
+                                     wstl_package=service.__package__,
+                                     db_manager_cls=KeycloakMongoManagerForPyTest,
                                      fixtures=db_store,
                                      get_actions=[Action(name='heaserver-people-person-get-properties',
                                                          rel=['hea-properties']),
                                                   Action(name='heaserver-people-person-get-self',
                                                          url='http://localhost:8080/people/{id}',
                                                          rel=['self']),
                                                   Action(name='heaserver-people-person-get-settings',
-                                                             url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
-                                                             rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
+                                                         url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
+                                                         rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
                                                   # Action(name='heaserver-people-person-get-organization-collection',
                                                   #        url='http://localhost:8080/collections/heaobject.organization.Organization',
                                                   #        rel=['hea-system-menu-item', 'application/x.collection']),
+                                                  Action(name='heaserver-people-person-get-volumes-collection',
+                                                         url='http://localhost:8080/collections/heaobject.volume.Volume',
+                                                         rel=['hea-system-menu-item', 'application/x.collection']),
                                                   Action(name='heaserver-people-person-get-organizations',
                                                          url='http://localhost:8080/organizations/',
                                                          rel=['application/x.organization']),
                                                   Action(name='heaserver-people-person-get-volumes',
                                                          url='http://localhost:8080/volumes/',
                                                          rel=['application/x.volume']),
                                                   Action(name='heaserver-people-person-get-desktop-object-actions',
@@ -100,18 +123,23 @@
                                                              rel=['self']),
                                                       Action(name='heaserver-people-person-get-settings',
                                                              url='http://localhost:8080/collections/heaobject.settings.SettingsObject',
                                                              rel=['hea-system-menu-item', 'hea-user-menu-item', 'application/x.settingsobject', 'application/x.collection']),
                                                       # Action(name='heaserver-people-person-get-organization-collection',
                                                       #        url='http://localhost:8080/collections/heaobject.organization.Organization',
                                                       #        rel=['hea-system-menu-item', 'application/x.collection']),
+                                                      Action(name='heaserver-people-person-get-volumes-collection',
+                                                         url='http://localhost:8080/collections/heaobject.volume.Volume',
+                                                         rel=['hea-system-menu-item', 'application/x.collection']),
                                                       Action(name='heaserver-people-person-get-organizations',
                                                              url='http://localhost:8080/organizations/',
                                                              rel=['application/x.organization']),
                                                       Action(name='heaserver-people-person-get-volumes',
                                                              url='http://localhost:8080/volumes/',
                                                              rel=['application/x.volume']),
                                                       Action(name='heaserver-people-person-get-desktop-object-actions',
                                                              url='http://localhost:8080/desktopobjectactions/',
-                                                             rel=['application/x.desktopobjectaction'])],
-                                     duplicate_action_name=None,
-        exclude=['body_put', 'body_post'])
+                                                             rel=['application/x.desktopobjectaction'])
+                                                      ],
+                                     registry_docker_image=RealRegistryContainerConfig(HEASERVER_REGISTRY_IMAGE),
+                                     duplicate_action_name='heaserver-people-person-duplicate-form',
+                                     exclude=['body_put', 'body_post'])
```

