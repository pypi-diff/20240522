# Comparing `tmp/dkist_service_configuration-2.0.0rc2.tar.gz` & `tmp/dkist_service_configuration-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dkist_service_configuration-2.0.0rc2.tar", last modified: Mon Apr 29 22:52:25 2024, max compression
+gzip compressed data, was "dkist_service_configuration-2.0.1.tar", last modified: Wed May 22 14:56:05 2024, max compression
```

## Comparing `dkist_service_configuration-2.0.0rc2.tar` & `dkist_service_configuration-2.0.1.tar`

### file list

```diff
@@ -1,30 +1,27 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      580 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)     1063 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      482 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1282 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1675 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/bitbucket-pipelines.yml
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/
--rw-rw-rw-   0 root         (0) root         (0)      145 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1688 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1987 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      279 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1701 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_settings.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2127 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      763 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/not-zip-safe
--rw-rw-rw-   0 root         (0) root         (0)      105 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-04-29 22:52:25.000000 dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/licenses/
--rw-rw-rw-   0 root         (0) root         (0)      372 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/licenses/README.rst
--rw-rw-rw-   0 root         (0) root         (0)     1482 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/licenses/license.rst
--rw-rw-rw-   0 root         (0) root         (0)     2184 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       38 2024-04-29 22:52:25.618972 dkist_service_configuration-2.0.0rc2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1250 2024-04-29 22:52:10.000000 dkist_service_configuration-2.0.0rc2/tox.ini
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      580 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     1063 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      482 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1282 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/README.rst
+-rw-rw-rw-   0 root         (0) root         (0)     1675 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/bitbucket-pipelines.yml
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.341018 dkist_service_configuration-2.0.1/dkist_service_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      411 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1688 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1987 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      279 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1701 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_settings.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2116 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      722 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2024-05-22 14:56:04.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/not-zip-safe
+-rw-rw-rw-   0 root         (0) root         (0)       97 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)       39 2024-05-22 14:56:05.000000 dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2115 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       38 2024-05-22 14:56:05.345018 dkist_service_configuration-2.0.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1250 2024-05-22 14:55:51.000000 dkist_service_configuration-2.0.1/tox.ini
```

### Comparing `dkist_service_configuration-2.0.0rc2/.gitignore` & `dkist_service_configuration-2.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/.pre-commit-config.yaml` & `dkist_service_configuration-2.0.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/LICENSE` & `dkist_service_configuration-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/PKG-INFO` & `dkist_service_configuration-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.0rc2
+Version: 2.0.1
 Summary: Library for retrieving configurations for DKIST services
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: loguru>0.7.0
 Requires-Dist: pydantic-settings>2.0
-Requires-Dist: pydantic[dotenv]>2.0
+Requires-Dist: pydantic>2.0
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist_service_configuration-2.0.0rc2/README.rst` & `dkist_service_configuration-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/bitbucket-pipelines.yml` & `dkist_service_configuration-2.0.1/bitbucket-pipelines.yml`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/logging.py` & `dkist_service_configuration-2.0.1/dkist_service_configuration/logging.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/settings.py` & `dkist_service_configuration-2.0.1/dkist_service_configuration/settings.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/dkist_service_configuration/tests/test_settings.py` & `dkist_service_configuration-2.0.1/dkist_service_configuration/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/PKG-INFO` & `dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: dkist-service-configuration
-Version: 2.0.0rc2
+Version: 2.0.1
 Summary: Library for retrieving configurations for DKIST services
 Author-email: NSO / AURA <dkistdc@nso.edu>
 License: BSD 3-Clause
 Project-URL: repository, https://bitbucket.org/dkistdc/dkist_service_configuration
-Classifier: License :: OSI Approved :: BSD License
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.11
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 Requires-Dist: loguru>0.7.0
 Requires-Dist: pydantic-settings>2.0
-Requires-Dist: pydantic[dotenv]>2.0
+Requires-Dist: pydantic>2.0
 Provides-Extra: test
 Requires-Dist: tox>=4; extra == "test"
 Requires-Dist: pytest; extra == "test"
 Requires-Dist: pytest-cov; extra == "test"
 Requires-Dist: Pygments; extra == "test"
 Requires-Dist: PyPDF4; extra == "test"
```

### Comparing `dkist_service_configuration-2.0.0rc2/dkist_service_configuration.egg-info/SOURCES.txt` & `dkist_service_configuration-2.0.1/dkist_service_configuration.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,10 +14,8 @@
 dkist_service_configuration.egg-info/SOURCES.txt
 dkist_service_configuration.egg-info/dependency_links.txt
 dkist_service_configuration.egg-info/not-zip-safe
 dkist_service_configuration.egg-info/requires.txt
 dkist_service_configuration.egg-info/top_level.txt
 dkist_service_configuration/tests/__init__.py
 dkist_service_configuration/tests/test_logging.py
-dkist_service_configuration/tests/test_settings.py
-licenses/README.rst
-licenses/license.rst
+dkist_service_configuration/tests/test_settings.py
```

### Comparing `dkist_service_configuration-2.0.0rc2/pyproject.toml` & `dkist_service_configuration-2.0.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 
 [project]
 name = "dkist-service-configuration"
 description = "Library for retrieving configurations for DKIST services"
 readme = "README.rst"
 requires-python = ">=3.11"
 classifiers = [
-    "License :: OSI Approved :: BSD License",
+    "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.11",
 ]
 license = { text = "BSD 3-Clause" }
 authors = [
   { name = "NSO / AURA", email = "dkistdc@nso.edu" },
 ]
-# the current version of Airflow does not support pydantic v2
+
 dependencies = [
     "loguru>0.7.0",
     "pydantic-settings>2.0",
-    "pydantic[dotenv]>2.0",
+    "pydantic>2.0",
 ]
 dynamic = ["version"]
 
 # tox is not required to run the tests, but simplifies IDE integration
 # Pygments is solely to support README.rst rendering
 [project.optional-dependencies]
 test = [
```

### Comparing `dkist_service_configuration-2.0.0rc2/tox.ini` & `dkist_service_configuration-2.0.1/tox.ini`

 * *Files identical despite different names*

