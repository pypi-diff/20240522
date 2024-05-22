# Comparing `tmp/heaserver_registry-1.0.2.tar.gz` & `tmp/heaserver_registry-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver_registry-1.0.2.tar", last modified: Thu Apr 18 02:22:07 2024, max compression
+gzip compressed data, was "heaserver_registry-1.0.3.tar", last modified: Wed May 22 15:16:00 2024, max compression
```

## Comparing `heaserver_registry-1.0.2.tar` & `heaserver_registry-1.0.3.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.414178 heaserver_registry-1.0.2/
--rw-rw-rw-   0        0        0      261 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/.gitignore
--rw-rw-rw-   0        0        0     1658 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/Dockerfile
--rw-rw-rw-   0        0        0    11625 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/LICENSE
--rw-rw-rw-   0        0        0      272 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     4790 2024-04-18 02:22:07.413179 heaserver_registry-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     3566 2024-04-18 02:20:30.000000 heaserver_registry-1.0.2/README.md
--rw-rw-rw-   0        0        0     1878 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/RELEASING.md
--rw-rw-rw-   0        0        0      329 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/docker-entrypoint.sh
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.349180 heaserver_registry-1.0.2/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.350177 heaserver_registry-1.0.2/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.379177 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/__init__.py
--rw-rw-rw-   0        0        0     7887 2024-04-17 00:22:00.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py
--rw-rw-rw-   0        0        0     3991 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     9262 2024-04-17 02:40:54.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0    23391 2024-04-17 02:54:48.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all.py
--rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py
--rw-rw-rw-   0        0        0      111 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/pytest.ini
--rw-rw-rw-   0        0        0      248 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/requirements_dev.txt
--rw-rw-rw-   0        0        0     3014 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/run-swaggerui.py
--rw-rw-rw-   0        0        0       42 2024-04-18 02:22:07.415177 heaserver_registry-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2439 2024-04-18 02:21:19.000000 heaserver_registry-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.352177 heaserver_registry-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.351177 heaserver_registry-1.0.2/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.381178 heaserver_registry-1.0.2/src/heaserver/registry/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/src/heaserver/registry/__init__.py
--rw-rw-rw-   0        0        0    38098 2024-04-17 03:30:21.000000 heaserver_registry-1.0.2/src/heaserver/registry/service.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.382179 heaserver_registry-1.0.2/src/heaserver/registry/wstl/
--rw-rw-rw-   0        0        0    13493 2024-03-07 16:45:28.000000 heaserver_registry-1.0.2/src/heaserver/registry/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.412178 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/
--rw-rw-rw-   0        0        0     4790 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1920 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       71 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 02:22:07.000000 heaserver_registry-1.0.2/src/heaserver_registry.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.353179 heaserver_registry-1.0.2/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.353179 heaserver_registry-1.0.2/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.398182 heaserver_registry-1.0.2/tests/heaserver/registrytest/
--rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:22:07.410178 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260
--rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268
--rw-rw-rw-   0        0        0     2921 2023-11-10 05:23:52.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740
--rw-rw-rw-   0        0        0     7528 2024-04-17 00:19:45.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/collectiontestcase.py
--rw-rw-rw-   0        0        0     3850 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     8623 2024-04-17 00:31:26.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/componenttestcase.py
--rw-rw-rw-   0        0        0    23342 2024-04-17 00:39:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all.py
--rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all_with_bad_permissions.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.817045 heaserver_registry-1.0.3/
+-rw-rw-rw-   0        0        0      261 2022-03-11 23:00:39.000000 heaserver_registry-1.0.3/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/.gitignore
+-rw-rw-rw-   0        0        0     1658 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/Dockerfile
+-rw-rw-rw-   0        0        0    11625 2022-03-11 23:00:39.000000 heaserver_registry-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0      272 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     4992 2024-05-22 15:16:00.816045 heaserver_registry-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3768 2024-05-22 15:14:25.000000 heaserver_registry-1.0.3/README.md
+-rw-rw-rw-   0        0        0     1878 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/RELEASING.md
+-rw-rw-rw-   0        0        0      329 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/docker-entrypoint.sh
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.752890 heaserver_registry-1.0.3/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.752890 heaserver_registry-1.0.3/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.781655 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/__init__.py
+-rw-rw-rw-   0        0        0     7887 2024-04-18 02:23:11.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py
+-rw-rw-rw-   0        0        0     3991 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     9354 2024-05-22 15:09:39.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0    20801 2024-05-22 15:12:38.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/test_all.py
+-rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      111 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/pytest.ini
+-rw-rw-rw-   0        0        0      248 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/requirements_dev.txt
+-rw-rw-rw-   0        0        0     3014 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/run-swaggerui.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 15:16:00.818220 heaserver_registry-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2439 2024-05-22 15:15:18.000000 heaserver_registry-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.754899 heaserver_registry-1.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.753915 heaserver_registry-1.0.3/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.784655 heaserver_registry-1.0.3/src/heaserver/registry/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.3/src/heaserver/registry/__init__.py
+-rw-rw-rw-   0        0        0    36170 2024-05-16 15:21:23.000000 heaserver_registry-1.0.3/src/heaserver/registry/service.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.785990 heaserver_registry-1.0.3/src/heaserver/registry/wstl/
+-rw-rw-rw-   0        0        0    14324 2024-05-13 22:36:07.000000 heaserver_registry-1.0.3/src/heaserver/registry/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.815047 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/
+-rw-rw-rw-   0        0        0     4992 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1920 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       71 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 15:16:00.000000 heaserver_registry-1.0.3/src/heaserver_registry.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.755890 heaserver_registry-1.0.3/tests/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.755890 heaserver_registry-1.0.3/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.803169 heaserver_registry-1.0.3/tests/heaserver/registrytest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 23:00:39.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 15:16:00.813045 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260
+-rw-rw-rw-   0        0        0     2208 2023-07-03 21:35:26.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268
+-rw-rw-rw-   0        0        0     2921 2023-11-10 05:23:52.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740
+-rw-rw-rw-   0        0        0     7528 2024-04-18 02:23:11.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/collectiontestcase.py
+-rw-rw-rw-   0        0        0     3850 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     8623 2024-04-18 02:23:11.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/componenttestcase.py
+-rw-rw-rw-   0        0        0    20734 2024-05-16 15:23:06.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/test_all.py
+-rw-rw-rw-   0        0        0     1418 2023-12-18 23:38:46.000000 heaserver_registry-1.0.3/tests/heaserver/registrytest/test_all_with_bad_permissions.py
```

### Comparing `heaserver_registry-1.0.2/Dockerfile` & `heaserver_registry-1.0.3/Dockerfile`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/LICENSE` & `heaserver_registry-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/PKG-INFO` & `heaserver_registry-1.0.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-registry
-Version: 1.0.2
+Version: 1.0.3
 Summary: The HEA registry service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,25 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.3
+* Use the type display name in the properties card.
+* Hide some other heaobject.registry.Collection attributes in the properties card.
+
+
 ## Version 1.0.2
 * When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+* Return the type_display_name attribute.
 
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver_registry-1.0.2/README.md` & `heaserver_registry-1.0.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.3
+* Use the type display name in the properties card.
+* Hide some other heaobject.registry.Collection attributes in the properties card.
+
+
 ## Version 1.0.2
 * When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+* Return the type_display_name attribute.
 
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver_registry-1.0.2/RELEASING.md` & `heaserver_registry-1.0.3/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py` & `heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/collectiontestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py` & `heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/componenttestcase.py` & `heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/componenttestcase.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from heaobject.user import NONE_USER, TEST_USER, ALL_USERS
 from heaobject.root import Permission
 from heaserver.service.testcase.expectedvalues import Action
 
 db_store = {
     service.MONGODB_COMPONENT_COLLECTION: [{
         'id': '666f6f2d6261722d71757578',
-        'created': None,
+        'created': '2022-05-17T00:00:00+00:00',
         'derived_by': None,
         'derived_from': [],
         'description': None,
         'display_name': 'Reximus',
         'invites': [],
-        'modified': None,
+        'modified': '2022-05-17T00:00:00+00:00',
         'name': 'reximus',
         'owner': NONE_USER,
         'shares': [],
         'source': None,
         'source_detail': None,
         'type': 'heaobject.registry.Component',
         'base_url': 'http://localhost/foo',
@@ -39,21 +39,21 @@
             'default_shares': [],
             'type_display_name': 'Resource'
         }],
         'type_display_name': 'Registry Component'
     },
         {
             'id': '0123456789ab0123456789ab',
-            'created': None,
+            'created': '2022-05-17T00:00:00+00:00',
             'derived_by': None,
             'derived_from': [],
             'description': None,
             'display_name': 'Luximus',
             'invites': [],
-            'modified': None,
+            'modified': '2022-05-17T00:00:00+00:00',
             'name': 'luximus',
             'owner': NONE_USER,
             'shares': [],
             'source': None,
             'source_detail': None,
             'type': 'heaobject.registry.Component',
             'base_url': 'http://localhost/foo',
```

### Comparing `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all.py` & `heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/test_all.py`

 * *Files 17% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                     {
                         "name": "id",
                         "value": "666f6f2d6261722d71757578",
                         "prompt": "id",
                         "display": False},
                     {
                         "name": "created",
-                        "value": None,
+                        "value": '2022-05-17T00:00:00+00:00',
                         "prompt": "created",
                         "display": True},
                     {
                         "name": "derived_by",
                         "value": None,
                         "prompt": "derived_by",
                         "display": True},
@@ -101,15 +101,15 @@
                         "name": "shares",
                         "prompt": "shares",
                         "value": [],
                         "display": True
                     },
                     {
                         "name": "modified",
-                        "value": None,
+                        "value": '2022-05-17T00:00:00+00:00',
                         "prompt": "modified",
                         "display": True},
                     {
                         "name": "name",
                         "value": "reximus",
                         "prompt": "name",
                         "display": True},
@@ -239,28 +239,14 @@
 
     async def test_no_file_system_2_status(self):
         obj = await self.client.request('GET',
                                         (self._href / 'bytype' / 'heaobject.folder.Item').path,
                                         headers=self._headers)
         self.assertEquals(200, obj.status)
 
-    async def test_right_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name()).path,
-                                        headers=self._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / 'heaobject.volume.WrongFileSystem').path,
-                                        headers=self._headers)
-        self.assertEquals(404, obj.status)
-
 
 class TestGetResource2(ComponentTestCase2):
     _headers = {SUB: NONE_USER, hdrs.X_FORWARDED_HOST: 'localhost:8080'}
 
     async def test_no_file_system(self):
         expected = [{"collection": {"version": "1.0",
                                     "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
@@ -465,42 +451,14 @@
 
     async def test_no_file_system_status(self):
         obj = await self.client.request('GET',
                                         (self._href / 'bytype' / 'heaobject.folder.Folder').path,
                                         headers=TestGetResource2._headers)
         self.assertEquals(200, obj.status)
 
-    async def test_right_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name()).path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / 'heaobject.volume.WrongFileSystem').path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(404, obj.status)
-
-    async def test_right_file_system_type_and_name_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name() / 'byfilesystemname' / DEFAULT_FILE_SYSTEM).path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_type_and_name_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name() / 'byfilesystemname' / 'WRONG_FILE_SYSTEM').path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(404, obj.status)
-
 
 class TestGetCollection(CollectionTestCase, GetOneMixin):
     pass
 
 
 class TestGetAllCollections(CollectionTestCase, GetAllMixin):
     pass
```

### Comparing `heaserver_registry-1.0.2/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py` & `heaserver_registry-1.0.3/integrationtests/heaserver/registryintegrationtest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/run-swaggerui.py` & `heaserver_registry-1.0.3/run-swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/setup.py` & `heaserver_registry-1.0.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setuptools.setup(name='heaserver-registry',
-                 version='1.0.2',
+                 version='1.0.3',
                  description='The HEA registry service.',
                  long_description=long_description,
                  long_description_content_type='text/markdown',
                  url='https://risr.hci.utah.edu',
                  author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
                  author_email='Andrew.Post@hci.utah.edu',
                  python_requires='>=3.10',
                  package_dir={'': 'src'},
                  packages=['heaserver.registry'],
                  package_data={'heaserver.registry': ['wstl/*.json']},
                  install_requires=[
-                     'heaserver~=1.4.1'
+                     'heaserver~=1.6.0'
                  ],
                  classifiers=[
                      'Development Status :: 5 - Production/Stable',
                      'Intended Audience :: Developers',
                      'Intended Audience :: Science/Research',
                      'License :: OSI Approved :: Apache Software License',
                      'Framework :: AsyncIO',
```

### Comparing `heaserver_registry-1.0.2/src/heaserver/registry/service.py` & `heaserver_registry-1.0.3/src/heaserver/registry/service.py`

 * *Files 8% similar despite different names*

```diff
@@ -73,21 +73,17 @@
       '404':
         $ref: '#/components/responses/404'
     """
     return await mongoservicelib.get_by_name(request, MONGODB_COMPONENT_COLLECTION)
 
 
 @routes.get('/components/bytype/{type}')
-@routes.get('/components/bytype/{type}/byfilesystemtype/{filesystemtype}')
-@routes.get('/components/bytype/{type}/byfilesystemtype/{filesystemtype}/byfilesystemname/{filesystemname}')
 async def get_component_by_type(request: web.Request) -> web.Response:
     """
-    Gets the component that serves resources of the specified HEA object type and file system. If no file system name
-    is passed in, DEFAULT_FILE_SYSTEM is assumed. If not file system type is passed in,
-    heaobject.volume.MongoDBFileSystem is assumed.
+    Gets the component that serves resources of the specified HEA object type.
 
     :param request: the HTTP request.
     :return: the requested component or Not Found.
     ---
     summary: A specific component, by type and file system.
     tags:
         - heaserver-registry-component
@@ -98,59 +94,28 @@
           description: The type of the component to retrieve.
           schema:
             type: string
           examples:
             example:
               summary: A component type
               value: heaobject.folder.Folder
-        - name: filesystemtype
-          in: path
-          required: true
-          description: The type of the component's file system.
-          schema:
-            type: string
-          examples:
-            example:
-              summary: A component type
-              value: heaobject.volume.MongoDBFileSystem
-        - name: filesystemname
-          in: path
-          required: true
-          description: The name of the component's file system.
-          schema:
-            type: string
-          examples:
-            example:
-              summary: A component name
-              value: DEFAULT_FILE_SYSTEM
     responses:
       '200':
         $ref: '#/components/responses/200'
       '404':
         $ref: '#/components/responses/404'
     """
     sub = request.headers.get(SUB, NONE_USER)
     type_ = request.match_info['type']
-    file_system_name = request.match_info.get('filesystemname', DEFAULT_FILE_SYSTEM)
-    file_system_type = request.match_info.get('filesystemtype', MongoDBFileSystem.get_type_name())
-    cache_key = (request.headers.get(SUB, NONE_USER), MONGODB_COMPONENT_COLLECTION, f'type^{type_}', f'file_system_type^{file_system_type}', f'file_system_name^{file_system_name}')
+    cache_key = (sub, MONGODB_COMPONENT_COLLECTION, f'type^{type_}')
     result = request.app[appproperty.HEA_CACHE].get(cache_key)
     if result is None:
-        if file_system_name == DEFAULT_FILE_SYSTEM:
-            query_clause = {'$or': [{'file_system_name': {'$exists': False}}, {'file_system_name': {'$in': [file_system_name, None]}}]}
-        else:
-            query_clause = {'file_system_name': {'$eq': file_system_name}}
-        if file_system_type == MongoDBFileSystem.get_type_name():
-            query_clause.update({'$or': [{'file_system_type': {'$exists': False}}, {'file_system_type': {'$in': [file_system_type, None]}}]})
-        else:
-            query_clause.update({'file_system_type': {'$eq': file_system_type}})
         mongo_attributes = {'resources': {
             '$elemMatch': {
-                'resource_type_name': {'$eq': type_},
-                **query_clause
+                'resource_type_name': {'$eq': type_}
             }}}
 
         result_dict = await request.app[appproperty.HEA_DB].get(request,
                                                         MONGODB_COMPONENT_COLLECTION,
                                                         mongoattributes=mongo_attributes)
         if result_dict is None:
             return await response.get(request, None)
```

### Comparing `heaserver_registry-1.0.2/src/heaserver_registry.egg-info/PKG-INFO` & `heaserver_registry-1.0.3/src/heaserver_registry.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver-registry
-Version: 1.0.2
+Version: 1.0.3
 Summary: The HEA registry service.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
@@ -20,25 +20,31 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaserver~=1.4.1
+Requires-Dist: heaserver~=1.6.0
 
 # HEA Server Registry Microservice
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/),
 Salt Lake City, UT
 
 The HEA Server Registry Microservice manages mappings of HEA Object types to the microservices for storing and
 retrieving them.
 
+## Version 1.0.3
+* Use the type display name in the properties card.
+* Hide some other heaobject.registry.Collection attributes in the properties card.
+
+
 ## Version 1.0.2
 * When requesting desktop objects as a Collection+JSON document, add the permissions property to the document.
+* Return the type_display_name attribute.
 
 ## Version 1.0.1
 * Made the collection object form template fields read-only, and added the type field.
 
 ## Version 1
 Initial release.
```

### Comparing `heaserver_registry-1.0.2/src/heaserver_registry.egg-info/SOURCES.txt` & `heaserver_registry-1.0.3/src/heaserver_registry.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.14464`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.1528`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23164`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.23260`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-310-pytest-7.3.2.pyc.31268`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/__pycache__/test_all_with_bad_permissions.cpython-311-pytest-7.4.3.pyc.20740`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/collectiontestcase.py` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/collectiontestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/componentpermissionstestcase.py` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/componenttestcase.py` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all.py` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/test_all.py`

 * *Files 16% similar despite different names*

```diff
@@ -243,29 +243,14 @@
 
     async def test_no_file_system_status(self):
         obj = await self.client.request("GET",
                                         (self._href / "bytype" / "heaobject.folder.Folder").path,
                                         headers=self._headers)
         self.assertEquals(200, obj.status)
 
-    async def test_right_file_system_status(self):
-        obj = await self.client.request("GET",
-                                        (
-                                            self._href / "bytype" / "heaobject.folder.Folder" / "byfilesystemtype" / MongoDBFileSystem.get_type_name()).path,
-                                        headers=self._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_status(self):
-        obj = await self.client.request("GET",
-                                        (
-                                            self._href / "bytype" / "heaobject.folder.Folder" / "byfilesystemtype" / "WRONG_FILE_SYSTEM").path,
-                                        headers=self._headers)
-        self.assertEquals(404, obj.status)
-
-
 class TestGetResource2(ComponentTestCase2):
     _headers = {SUB: NONE_USER, hdrs.X_FORWARDED_HOST: "localhost:8080"}
 
     async def test_no_file_system(self):
         expected = [{"collection": {
             "version": "1.0",
             "href": "http://localhost:8080/components/bytype/heaobject.folder.Folder",
@@ -476,42 +461,14 @@
 
     async def test_no_file_system_status(self):
         obj = await self.client.request('GET',
                                         (self._href / 'bytype' / 'heaobject.folder.Folder').path,
                                         headers=TestGetResource2._headers)
         self.assertEquals(200, obj.status)
 
-    async def test_right_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name()).path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / 'WRONG_FILE_SYSTEM').path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(404, obj.status)
-
-    async def test_right_file_system_type_and_name_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name() / 'byfilesystemname' / DEFAULT_FILE_SYSTEM).path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(200, obj.status)
-
-    async def test_wrong_file_system_type_and_name_status(self):
-        obj = await self.client.request('GET',
-                                        (
-                                            self._href / 'bytype' / 'heaobject.folder.Folder' / 'byfilesystemtype' / MongoDBFileSystem.get_type_name() / 'byfilesystemname' / 'WRONG_FILE_SYSTEM').path,
-                                        headers=TestGetResource2._headers)
-        self.assertEquals(404, obj.status)
-
 
 class TestGetCollection(CollectionTestCase, GetOneMixin):
     pass
 
 
 class TestGetAllCollections(CollectionTestCase, GetAllMixin):
     pass
```

### Comparing `heaserver_registry-1.0.2/tests/heaserver/registrytest/test_all_with_bad_permissions.py` & `heaserver_registry-1.0.3/tests/heaserver/registrytest/test_all_with_bad_permissions.py`

 * *Files identical despite different names*

