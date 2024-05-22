# Comparing `tmp/openbb_regulators-1.2.0.tar.gz` & `tmp/openbb_regulators-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_regulators-1.2.0.tar", max compression
+gzip compressed data, was "openbb_regulators-1.2.1.tar", max compression
```

## Comparing `openbb_regulators-1.2.0.tar` & `openbb_regulators-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      343 2024-05-15 14:26:33.043720 openbb_regulators-1.2.0/README.md
--rw-r--r--   0        0        0       35 2024-04-23 10:22:39.608891 openbb_regulators-1.2.0/openbb_regulators/__init__.py
--rw-r--r--   0        0        0       51 2024-02-29 11:03:36.742976 openbb_regulators-1.2.0/openbb_regulators/cftc/__init__.py
--rw-r--r--   0        0        0     1889 2024-04-23 10:22:39.609012 openbb_regulators-1.2.0/openbb_regulators/cftc/cftc_router.py
--rw-r--r--   0        0        0      419 2024-04-23 10:22:39.609108 openbb_regulators-1.2.0/openbb_regulators/regulators_router.py
--rw-r--r--   0        0        0       35 2024-04-23 10:22:39.609201 openbb_regulators-1.2.0/openbb_regulators/sec/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-23 10:22:39.609308 openbb_regulators-1.2.0/openbb_regulators/sec/sec_router.py
--rw-r--r--   0        0        0      528 2024-05-15 16:05:00.871422 openbb_regulators-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openbb_regulators-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      343 2024-05-22 11:48:40.411330 openbb_regulators-1.2.1/README.md
+-rw-r--r--   0        0        0       35 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/__init__.py
+-rw-r--r--   0        0        0       51 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/cftc/__init__.py
+-rw-r--r--   0        0        0     1889 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/cftc/cftc_router.py
+-rw-r--r--   0        0        0      419 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/regulators_router.py
+-rw-r--r--   0        0        0       35 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/sec/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-14 16:56:41.573863 openbb_regulators-1.2.1/openbb_regulators/sec/sec_router.py
+-rw-r--r--   0        0        0      528 2024-05-22 13:55:42.375515 openbb_regulators-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 openbb_regulators-1.2.1/PKG-INFO
```

### Comparing `openbb_regulators-1.2.0/openbb_regulators/cftc/cftc_router.py` & `openbb_regulators-1.2.1/openbb_regulators/cftc/cftc_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.2.0/openbb_regulators/sec/sec_router.py` & `openbb_regulators-1.2.1/openbb_regulators/sec/sec_router.py`

 * *Files identical despite different names*

### Comparing `openbb_regulators-1.2.0/pyproject.toml` & `openbb_regulators-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-regulators"
-version = "1.2.0"
+version = "1.2.1"
 description = "Markets and Agency Regulators extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_regulators" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 regulators = "openbb_regulators.regulators_router:router"
```

### Comparing `openbb_regulators-1.2.0/PKG-INFO` & `openbb_regulators-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-regulators
-Version: 1.2.0
+Version: 1.2.1
 Summary: Markets and Agency Regulators extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Regulators Extension
 
 This extension provides a structure for data sourced from various global market regulators.
 
 ## Installation
```

