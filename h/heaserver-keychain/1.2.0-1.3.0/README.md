# Comparing `tmp/heaserver_keychain-1.2.0.tar.gz` & `tmp/heaserver_keychain-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_keychain-1.2.0.tar", last modified: Sat May  4 04:33:32 2024, max compression
+gzip compressed data, was "heaserver_keychain-1.3.0.tar", last modified: Wed May 22 00:05:37 2024, max compression
```

## Comparing `heaserver_keychain-1.2.0.tar` & `heaserver_keychain-1.3.0.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.570361 heaserver_keychain-1.2.0/
--rw-rw-rw-   0        0        0      325 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/.gitignore
--rw-rw-rw-   0        0        0     1579 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/Dockerfile
--rw-rw-rw-   0        0        0    11625 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     5289 2024-05-04 04:33:32.569362 heaserver_keychain-1.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     3963 2024-05-04 04:32:29.000000 heaserver_keychain-1.2.0/README.md
--rw-rw-rw-   0        0        0     2654 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/RELEASING.md
--rw-rw-rw-   0        0        0      588 2024-03-21 23:50:19.000000 heaserver_keychain-1.2.0/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.268010 heaserver_keychain-1.2.0/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.268010 heaserver_keychain-1.2.0/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.413968 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.437647 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952
--rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752
--rw-rw-rw-   0        0        0     4145 2024-03-21 23:50:19.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6650 2024-05-04 04:28:23.000000 heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/testcase.py
--rw-rw-rw-   0        0        0      109 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/requirements_dev.txt
--rw-rw-rw-   0        0        0     1048 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-05-04 04:33:32.570361 heaserver_keychain-1.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1830 2024-05-04 04:32:49.000000 heaserver_keychain-1.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.271010 heaserver_keychain-1.2.0/src/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.270009 heaserver_keychain-1.2.0/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.454678 heaserver_keychain-1.2.0/src/heaserver/keychain/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/src/heaserver/keychain/__init__.py
--rw-rw-rw-   0        0        0    17020 2024-03-21 23:50:19.000000 heaserver_keychain-1.2.0/src/heaserver/keychain/service.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.463663 heaserver_keychain-1.2.0/src/heaserver/keychain/wstl/
--rw-rw-rw-   0        0        0    18071 2024-04-26 16:56:20.000000 heaserver_keychain-1.2.0/src/heaserver/keychain/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.567364 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/
--rw-rw-rw-   0        0        0     5289 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2045 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-05-04 04:33:32.000000 heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.271010 heaserver_keychain-1.2.0/tests/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.272011 heaserver_keychain-1.2.0/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.535693 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/
--rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-04 04:33:32.565361 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348
--rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848
--rw-rw-rw-   0        0        0     2205 2024-01-04 18:07:50.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296
--rw-rw-rw-   0        0        0     3778 2024-03-21 23:50:19.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/permissionstestcase.py
--rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/test_all.py
--rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0     6554 2024-05-04 04:28:06.000000 heaserver_keychain-1.2.0/tests/heaserver/keychaintest/testcase.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.707608 heaserver_keychain-1.3.0/
+-rw-rw-rw-   0        0        0      325 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/.gitignore
+-rw-rw-rw-   0        0        0     1579 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     5416 2024-05-22 00:05:37.706608 heaserver_keychain-1.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     4090 2024-05-22 00:04:34.000000 heaserver_keychain-1.3.0/README.md
+-rw-rw-rw-   0        0        0     2654 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/RELEASING.md
+-rw-rw-rw-   0        0        0      588 2024-03-21 23:50:19.000000 heaserver_keychain-1.3.0/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.427909 heaserver_keychain-1.3.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.427909 heaserver_keychain-1.3.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.559549 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.578360 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952
+-rw-rw-rw-   0        0        0     2227 2024-01-04 18:16:21.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752
+-rw-rw-rw-   0        0        0     4195 2024-05-17 22:48:39.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     6736 2024-05-17 23:10:18.000000 heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/testcase.py
+-rw-rw-rw-   0        0        0      109 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0     1048 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 00:05:37.707608 heaserver_keychain-1.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1830 2024-05-22 00:04:56.000000 heaserver_keychain-1.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.431077 heaserver_keychain-1.3.0/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.430029 heaserver_keychain-1.3.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.592906 heaserver_keychain-1.3.0/src/heaserver/keychain/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/__init__.py
+-rw-rw-rw-   0        0        0    17020 2024-03-21 23:50:19.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.604575 heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/
+-rw-rw-rw-   0        0        0    18063 2024-05-21 23:29:36.000000 heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.703225 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/
+-rw-rw-rw-   0        0        0     5416 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2045 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 00:05:37.000000 heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.432131 heaserver_keychain-1.3.0/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.432729 heaserver_keychain-1.3.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.677196 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/
+-rw-rw-rw-   0        0        0        0 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 00:05:37.703199 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348
+-rw-rw-rw-   0        0        0     2205 2023-11-10 05:51:07.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848
+-rw-rw-rw-   0        0        0     2205 2024-01-04 18:07:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296
+-rw-rw-rw-   0        0        0     3828 2024-05-17 22:49:36.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/permissionstestcase.py
+-rw-rw-rw-   0        0        0      404 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all.py
+-rw-rw-rw-   0        0        0     1083 2023-12-18 04:32:50.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     6604 2024-05-17 22:49:23.000000 heaserver_keychain-1.3.0/tests/heaserver/keychaintest/testcase.py
```

### Comparing `heaserver_keychain-1.2.0/Dockerfile` & `heaserver_keychain-1.3.0/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/LICENSE` & `heaserver_keychain-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/PKG-INFO` & `heaserver_keychain-1.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.2.0
+Version: 1.3.0
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.2
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.3.0
+* Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
+
 ## Version 1.2.0
 * Display type display name in properties card.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 * Return type_display_name attribute from GET calls.
```

### Comparing `heaserver_keychain-1.2.0/README.md` & `heaserver_keychain-1.3.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.3.0
+* Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
+
 ## Version 1.2.0
 * Display type display name in properties card.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 * Return type_display_name attribute from GET calls.
```

### Comparing `heaserver_keychain-1.2.0/RELEASING.md` & `heaserver_keychain-1.3.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/docker-entrypoint.sh` & `heaserver_keychain-1.3.0/docker-entrypoint.sh`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.2384`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.29448`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.35952`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.36752`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/permissionstestcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.keychain.Credentials',
         'version': None,
         'created': None,
         'account': None,
         'where': None,
-        'password': None
+        'password': None,
+        'role': None
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -51,15 +52,16 @@
             'source': None,
             'source_detail': None,
             'type': 'heaobject.keychain.Credentials',
             'version': None,
             'created': None,
             'account': None,
             'where': None,
-            'password': None
+            'password': None,
+            'role': None
         }]}
 
 PermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_CREDENTIALS_COLLECTION,
                               wstl_package=service.__package__,
                               href='http://localhost:8080/credentials/',
                               db_manager_cls=MockDockerMongoManager,
```

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.0/integrationtests/heaserver/keychainintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/integrationtests/heaserver/keychainintegrationtest/testcase.py` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/testcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
 
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
-from heaserver.service.testcase.dockermongo import MockDockerMongoManager
 from heaserver.keychain import service
 from heaobject.user import NONE_USER
 from heaserver.service.testcase.expectedvalues import Action
 
 db_store = {
     service.MONGODB_CREDENTIALS_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
@@ -24,15 +23,16 @@
         'source': None,
         'source_detail': None,
         'type': 'heaobject.keychain.Credentials',
         'created': None,
         'account': None,
         'where': None,
         'password': None,
-        'type_display_name': 'Credentials'
+        'type_display_name': 'Credentials',
+        'role': None
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -41,38 +41,38 @@
             'modified': None,
             'name': 'luximus',
             'owner': NONE_USER,
             'shares': [],
             'source': None,
             'source_detail': None,
             'type': 'heaobject.keychain.Credentials',
-            'created': None,
             'account': None,
+            'created': None,
             'where': None,
             'password': None,
-            'type_display_name': 'Credentials'
+            'type_display_name': 'Credentials',
+            'role': None
         }]}
 
 TestCase = get_test_case_cls_default(coll=service.MONGODB_CREDENTIALS_COLLECTION,
-                                     href='http://localhost:8080/credentials',
                                      wstl_package=service.__package__,
-                                     db_manager_cls=MockDockerMongoManager,
+                                     href='http://localhost:8080/credentials',
                                      fixtures=db_store,
                                      get_actions=[Action(name='heaserver-keychain-credentials-get-properties',
-                                                         rel=['hea-context-menu', 'hea-properties'],
-                                                         itemif='type=="heaobject.keychain.Credentials"'),
+                                                             rel=['hea-context-menu', 'hea-properties'],
+                                                             itemif='type=="heaobject.keychain.Credentials"'),
                                                   Action(name='heaserver-keychain-awscredentials-get-properties',
-                                                         rel=['hea-context-menu', 'hea-properties'],
-                                                         itemif='type=="heaobject.keychain.AWSCredentials"'),
+                                                             rel=['hea-context-menu', 'hea-properties'],
+                                                             itemif='type=="heaobject.keychain.AWSCredentials"'),
                                                   # Action(name='heaserver-keychain-credentials-open-choices',
-                                                  #        url='http://localhost:8080/credentials/{id}/opener',
-                                                  #        rel=['hea-context-menu', 'hea-opener-choices']),
+                                                  #            url='http://localhost:8080/credentials/{id}/opener',
+                                                  #            rel=['hea-context-menu', 'hea-opener-choices']),
                                                   # Action(name='heaserver-keychain-credentials-duplicate',
-                                                  #        url='http://localhost:8080/credentials/{id}/duplicator',
-                                                  #        rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
+                                                  #            url='http://localhost:8080/credentials/{id}/duplicator',
+                                                  #            rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                   Action(name='heaserver-keychain-credentials-get-self',
                                                              url='http://localhost:8080/credentials/{id}',
                                                              rel=['self']),
                                                   Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"')
@@ -80,21 +80,21 @@
                                      get_all_actions=[Action(name='heaserver-keychain-credentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.Credentials"'),
                                                       Action(name='heaserver-keychain-awscredentials-get-properties',
                                                              rel=['hea-context-menu', 'hea-properties'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"'),
                                                       # Action(name='heaserver-keychain-credentials-open-choices',
-                                                      #        url='http://localhost:8080/credentials/{id}/opener',
-                                                      #        rel=['hea-context-menu', 'hea-opener-choices']),
+                                                      #            url='http://localhost:8080/credentials/{id}/opener',
+                                                      #            rel=['hea-context-menu', 'hea-opener-choices']),
                                                       # Action(name='heaserver-keychain-credentials-duplicate',
-                                                      #        url='http://localhost:8080/credentials/{id}/duplicator',
-                                                      #        rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
+                                                      #            url='http://localhost:8080/credentials/{id}/duplicator',
+                                                      #            rel=['hea-context-menu', 'hea-dynamic-standard', 'hea-icon-duplicator']),
                                                       Action(name='heaserver-keychain-credentials-get-self',
-                                                             url='http://localhost:8080/credentials/{id}',
-                                                             rel=['self']),
+                                                                 url='http://localhost:8080/credentials/{id}',
+                                                                 rel=['self']),
                                                       Action(name='heaserver-keychain-awscredentials-get-cli-credentials-file',
                                                              url='http://localhost:8080/credentials/{id}/awsclicredentialsfile',
                                                              rel=['hea-dynamic-clipboard', 'hea-icon-for-clipboard', 'hea-context-menu'],
                                                              itemif='type=="heaobject.keychain.AWSCredentials"')],
                                      #duplicate_action_name='heaserver-keychain-credentials-duplicate-form'
                                      )
```

### Comparing `heaserver_keychain-1.2.0/run-swaggerui.py` & `heaserver_keychain-1.3.0/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/setup.py` & `heaserver_keychain-1.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 from setuptools import setup
 
 with open('README.md', encoding='utf-8') as readme_file:
     readme = readme_file.read()
 
 setup(
     name='heaserver-keychain',
-    version='1.2.0',
+    version='1.3.0',
     description="a service for managing laboratory credentials",
     long_description=readme,
     long_description_content_type='text/markdown',
     url='https://risr.hci.utah.edu',
     author="Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT",
     author_email='Andrew.Post@hci.utah.edu',
     python_requires='>=3.10',
     package_dir={'': 'src'},
     packages=['heaserver.keychain'],
     package_data={'heaserver.keychain': ['wstl/*.json']},
-    install_requires=['heaserver~=1.5.2'],
+    install_requires=['heaserver~=1.6.0'],
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: Apache Software License',
         'Framework :: AsyncIO',
         'Environment :: Web Environment',
```

### Comparing `heaserver_keychain-1.2.0/src/heaserver/keychain/service.py` & `heaserver_keychain-1.3.0/src/heaserver/keychain/service.py`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/src/heaserver/keychain/wstl/all.json` & `heaserver_keychain-1.3.0/src/heaserver/keychain/wstl/all.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999979332010582%*

 * *Differences: {"'wstl'": "{'actions': {5: {'inputs': {9: {'name': 'role', 'prompt': 'Role'}}}}}"}*

```diff
@@ -331,16 +331,16 @@
                         ],
                         "type": "select"
                     },
                     {
                         "hea": {
                             "display": false
                         },
-                        "name": "role_arn",
-                        "prompt": "Role ARN"
+                        "name": "role",
+                        "prompt": "Role"
                     },
                     {
                         "hea": {
                             "type": "datetime"
                         },
                         "name": "expiration",
                         "prompt": "Expiration",
```

### Comparing `heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/PKG-INFO` & `heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-keychain
-Version: 1.2.0
+Version: 1.3.0
 Summary: a service for managing laboratory credentials
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Keywords: heaserver-keychain,microservice,healthcare,cancer,research,informatics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -21,22 +21,25 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.5.2
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Keychain
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://hci.utah.edu),
 Salt Lake City, UT
 
 The HEA server Keychain is a service for managing laboratory and user credentials.
 
+## Version 1.3.0
+* Now all Credentials objects have a role attribute, replacing the old AWSCredentials role_arn attribute.
+
 ## Version 1.2.0
 * Display type display name in properties card.
 
 ## Version 1.1.0
 * Pass desktop object permissions back to clients.
 * Return type_display_name attribute from GET calls.
```

### Comparing `heaserver_keychain-1.2.0/src/heaserver_keychain.egg-info/SOURCES.txt` & `heaserver_keychain-1.3.0/src/heaserver_keychain.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.14948`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.28348`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.32848`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.9296`

 * *Files identical despite different names*

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/permissionstestcase.py` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/permissionstestcase.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         'modified': None,
         'name': 'reximus',
         'owner': NONE_USER,
         'shares': [],
         'source': None,
         'source_detail': None,
         'type': 'heaobject.keychain.Credentials',
-        'version': None
+        'version': None,
+        'role': None
     },
         {
             'id': '0123456789ab0123456789ab',
             'created': None,
             'derived_by': None,
             'derived_from': [],
             'description': None,
@@ -42,15 +43,16 @@
                 'invite': None,
                 'user': TEST_USER,
                 'permissions': [Permission.VIEWER.name]
             }],
             'source': None,
             'source_detail': None,
             'type': 'heaobject.keychain.Credentials',
-            'version': None
+            'version': None,
+            'role': None
         }]}
 
 PermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_CREDENTIALS_COLLECTION,
                               wstl_package=service.__package__,
                               href='http://localhost:8080/credentials/',
                               fixtures=db_store,
```

### Comparing `heaserver_keychain-1.2.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py` & `heaserver_keychain-1.3.0/tests/heaserver/keychaintest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

