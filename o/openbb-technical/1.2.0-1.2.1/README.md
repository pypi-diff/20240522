# Comparing `tmp/openbb_technical-1.2.0.tar.gz` & `tmp/openbb_technical-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_technical-1.2.0.tar", max compression
+gzip compressed data, was "openbb_technical-1.2.1.tar", max compression
```

## Comparing `openbb_technical-1.2.0.tar` & `openbb_technical-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      478 2024-05-15 14:26:27.342633 openbb_technical-1.2.0/README.md
--rw-r--r--   0        0        0       43 2024-02-29 11:03:36.744125 openbb_technical-1.2.0/openbb_technical/__init__.py
--rw-r--r--   0        0        0    16738 2024-04-23 10:22:39.610514 openbb_technical-1.2.0/openbb_technical/helpers.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.744320 openbb_technical-1.2.0/openbb_technical/py.typed
--rw-r--r--   0        0        0    19706 2024-04-23 10:22:39.610659 openbb_technical-1.2.0/openbb_technical/relative_rotation.py
--rw-r--r--   0        0        0    63911 2024-05-15 11:31:42.982565 openbb_technical-1.2.0/openbb_technical/technical_router.py
--rw-r--r--   0        0        0      640 2024-05-15 16:05:06.756816 openbb_technical-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 openbb_technical-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      478 2024-05-22 11:48:40.411330 openbb_technical-1.2.1/README.md
+-rw-r--r--   0        0        0       43 2024-05-14 16:56:41.573863 openbb_technical-1.2.1/openbb_technical/__init__.py
+-rw-r--r--   0        0        0    16738 2024-05-14 16:56:41.573863 openbb_technical-1.2.1/openbb_technical/helpers.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.573863 openbb_technical-1.2.1/openbb_technical/py.typed
+-rw-r--r--   0        0        0    19706 2024-05-14 16:56:41.573863 openbb_technical-1.2.1/openbb_technical/relative_rotation.py
+-rw-r--r--   0        0        0    63911 2024-05-22 11:48:40.411330 openbb_technical-1.2.1/openbb_technical/technical_router.py
+-rw-r--r--   0        0        0      640 2024-05-22 13:55:31.087478 openbb_technical-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 openbb_technical-1.2.1/PKG-INFO
```

### Comparing `openbb_technical-1.2.0/openbb_technical/helpers.py` & `openbb_technical-1.2.1/openbb_technical/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.2.0/openbb_technical/relative_rotation.py` & `openbb_technical-1.2.1/openbb_technical/relative_rotation.py`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.2.0/openbb_technical/technical_router.py` & `openbb_technical-1.2.1/openbb_technical/technical_router.py`

 * *Files identical despite different names*

### Comparing `openbb_technical-1.2.0/pyproject.toml` & `openbb_technical-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "openbb-technical"
-version = "1.2.0"
+version = "1.2.1"
 description = "Technical Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_technical" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"  # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 scikit-learn = "^1.3.1"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 technical = "openbb_technical.technical_router:router"
```

### Comparing `openbb_technical-1.2.0/PKG-INFO` & `openbb_technical-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-technical
-Version: 1.2.0
+Version: 1.2.1
 Summary: Technical Analysis extension for OpenBB
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
 Requires-Dist: pandas-ta (>=0.3.14b,<0.4.0)
 Requires-Dist: scikit-learn (>=1.3.1,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Technical Analysis Extension
```

