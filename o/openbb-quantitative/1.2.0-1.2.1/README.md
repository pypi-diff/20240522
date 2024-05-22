# Comparing `tmp/openbb_quantitative-1.2.0.tar.gz` & `tmp/openbb_quantitative-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_quantitative-1.2.0.tar", max compression
+gzip compressed data, was "openbb_quantitative-1.2.1.tar", max compression
```

## Comparing `openbb_quantitative-1.2.0.tar` & `openbb_quantitative-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      477 2024-05-15 14:26:38.357393 openbb_quantitative-1.2.0/README.md
--rw-r--r--   0        0        0       59 2024-02-29 11:03:36.741757 openbb_quantitative-1.2.0/openbb_quantitative/__init__.py
--rw-r--r--   0        0        0     2443 2024-04-08 12:02:16.532009 openbb_quantitative-1.2.0/openbb_quantitative/helpers.py
--rw-r--r--   0        0        0     1158 2024-04-08 12:02:16.532109 openbb_quantitative-1.2.0/openbb_quantitative/models.py
--rw-r--r--   0        0        0     8654 2024-04-23 10:22:39.607204 openbb_quantitative-1.2.0/openbb_quantitative/performance/performance_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.741954 openbb_quantitative-1.2.0/openbb_quantitative/py.typed
--rw-r--r--   0        0        0    10131 2024-04-23 10:22:39.607339 openbb_quantitative-1.2.0/openbb_quantitative/quantitative_router.py
--rw-r--r--   0        0        0    14268 2024-04-23 10:22:39.607491 openbb_quantitative-1.2.0/openbb_quantitative/rolling/rolling_router.py
--rw-r--r--   0        0        0     1378 2024-04-23 10:22:39.607598 openbb_quantitative-1.2.0/openbb_quantitative/statistics.py
--rw-r--r--   0        0        0    10942 2024-04-23 10:22:39.607745 openbb_quantitative-1.2.0/openbb_quantitative/stats/stats_router.py
--rw-r--r--   0        0        0      635 2024-05-15 16:03:44.878012 openbb_quantitative-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 openbb_quantitative-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      477 2024-05-22 11:48:40.407330 openbb_quantitative-1.2.1/README.md
+-rw-r--r--   0        0        0       59 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/__init__.py
+-rw-r--r--   0        0        0     2443 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/helpers.py
+-rw-r--r--   0        0        0     1158 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/models.py
+-rw-r--r--   0        0        0     8654 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/performance/performance_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/py.typed
+-rw-r--r--   0        0        0    10131 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/quantitative_router.py
+-rw-r--r--   0        0        0    14268 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/rolling/rolling_router.py
+-rw-r--r--   0        0        0     1378 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/statistics.py
+-rw-r--r--   0        0        0    10942 2024-05-14 16:56:41.569863 openbb_quantitative-1.2.1/openbb_quantitative/stats/stats_router.py
+-rw-r--r--   0        0        0      635 2024-05-22 13:54:41.875314 openbb_quantitative-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 openbb_quantitative-1.2.1/PKG-INFO
```

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/helpers.py` & `openbb_quantitative-1.2.1/openbb_quantitative/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/models.py` & `openbb_quantitative-1.2.1/openbb_quantitative/models.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/performance/performance_router.py` & `openbb_quantitative-1.2.1/openbb_quantitative/performance/performance_router.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/quantitative_router.py` & `openbb_quantitative-1.2.1/openbb_quantitative/quantitative_router.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/rolling/rolling_router.py` & `openbb_quantitative-1.2.1/openbb_quantitative/rolling/rolling_router.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/statistics.py` & `openbb_quantitative-1.2.1/openbb_quantitative/statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/openbb_quantitative/stats/stats_router.py` & `openbb_quantitative-1.2.1/openbb_quantitative/stats/stats_router.py`

 * *Files identical despite different names*

### Comparing `openbb_quantitative-1.2.0/pyproject.toml` & `openbb_quantitative-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "openbb-quantitative"
-version = "1.2.0"
+version = "1.2.1"
 description = "Quantitative Analysis extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_quantitative" }]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"   # scipy forces python <4.0 explicitly
 scipy = "^1.10.1"
 statsmodels = "^0.14.0"
 pandas-ta = "^0.3.14b"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_core_extension"]
 quantitative = "openbb_quantitative.quantitative_router:router"
```

### Comparing `openbb_quantitative-1.2.0/PKG-INFO` & `openbb_quantitative-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-quantitative
-Version: 1.2.0
+Version: 1.2.1
 Summary: Quantitative Analysis extension for OpenBB
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
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Description-Content-Type: text/markdown
 
 # OpenBB QA Extension
```

