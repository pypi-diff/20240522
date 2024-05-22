# Comparing `tmp/openbb_econometrics-1.2.0.tar.gz` & `tmp/openbb_econometrics-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_econometrics-1.2.0.tar", max compression
+gzip compressed data, was "openbb_econometrics-1.2.1.tar", max compression
```

## Comparing `openbb_econometrics-1.2.0.tar` & `openbb_econometrics-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      321 2024-05-15 14:27:44.668244 openbb_econometrics-1.2.0/README.md
--rw-r--r--   0        0        0       37 2024-04-23 10:22:39.598318 openbb_econometrics-1.2.0/openbb_econometrics/__init__.py
--rw-r--r--   0        0        0    28152 2024-04-23 10:22:39.598476 openbb_econometrics-1.2.0/openbb_econometrics/econometrics_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.733411 openbb_econometrics-1.2.0/openbb_econometrics/py.typed
--rw-r--r--   0        0        0     4117 2024-04-23 10:22:39.598600 openbb_econometrics-1.2.0/openbb_econometrics/utils.py
--rw-r--r--   0        0        0      715 2024-05-15 16:04:15.823322 openbb_econometrics-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 openbb_econometrics-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      321 2024-05-22 11:48:40.403330 openbb_econometrics-1.2.1/README.md
+-rw-r--r--   0        0        0       37 2024-05-14 16:56:41.561863 openbb_econometrics-1.2.1/openbb_econometrics/__init__.py
+-rw-r--r--   0        0        0    28152 2024-05-14 16:56:41.561863 openbb_econometrics-1.2.1/openbb_econometrics/econometrics_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.561863 openbb_econometrics-1.2.1/openbb_econometrics/py.typed
+-rw-r--r--   0        0        0     4117 2024-05-14 16:56:41.561863 openbb_econometrics-1.2.1/openbb_econometrics/utils.py
+-rw-r--r--   0        0        0      715 2024-05-22 13:54:36.451296 openbb_econometrics-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1098 1970-01-01 00:00:00.000000 openbb_econometrics-1.2.1/PKG-INFO
```

### Comparing `openbb_econometrics-1.2.0/openbb_econometrics/econometrics_router.py` & `openbb_econometrics-1.2.1/openbb_econometrics/econometrics_router.py`

 * *Files identical despite different names*

### Comparing `openbb_econometrics-1.2.0/openbb_econometrics/utils.py` & `openbb_econometrics-1.2.1/openbb_econometrics/utils.py`

 * *Files identical despite different names*

### Comparing `openbb_econometrics-1.2.0/pyproject.toml` & `openbb_econometrics-1.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "openbb-econometrics"
-version = "1.2.0"
+version = "1.2.1"
 description = "Econometrics Toolkit for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_econometrics" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"                 # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 arch = "^5.5.0"
 linearmodels = "<=4.25"                # ^4.26 has setuptools-scm in setup_requires
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 econometrics = "openbb_econometrics.econometrics_router:router"
```

### Comparing `openbb_econometrics-1.2.0/PKG-INFO` & `openbb_econometrics-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-econometrics
-Version: 1.2.0
+Version: 1.2.1
 Summary: Econometrics Toolkit for OpenBB
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
 Requires-Dist: arch (>=5.5.0,<6.0.0)
 Requires-Dist: linearmodels (<=4.25)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # Econometrics extension for OpenBB Platform
 
 This extension provides a set of econometrics tools.
```

