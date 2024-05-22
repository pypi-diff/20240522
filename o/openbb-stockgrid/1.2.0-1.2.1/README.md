# Comparing `tmp/openbb_stockgrid-1.2.0.tar.gz` & `tmp/openbb_stockgrid-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_stockgrid-1.2.0.tar", max compression
+gzip compressed data, was "openbb_stockgrid-1.2.1.tar", max compression
```

## Comparing `openbb_stockgrid-1.2.0.tar` & `openbb_stockgrid-1.2.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      311 2024-05-15 14:27:06.790677 openbb_stockgrid-1.2.0/README.md
--rw-r--r--   0        0        0      667 2024-05-14 15:30:05.619253 openbb_stockgrid-1.2.0/openbb_stockgrid/__init__.py
--rw-r--r--   0        0        0     2392 2024-04-08 12:02:16.679141 openbb_stockgrid-1.2.0/openbb_stockgrid/models/short_volume.py
--rw-r--r--   0        0        0      523 2024-05-15 16:07:15.537820 openbb_stockgrid-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_stockgrid-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      311 2024-05-22 11:48:40.547330 openbb_stockgrid-1.2.1/README.md
+-rw-r--r--   0        0        0      667 2024-05-15 09:21:56.097885 openbb_stockgrid-1.2.1/openbb_stockgrid/__init__.py
+-rw-r--r--   0        0        0     2392 2024-05-14 16:56:42.109866 openbb_stockgrid-1.2.1/openbb_stockgrid/models/short_volume.py
+-rw-r--r--   0        0        0      523 2024-05-22 13:56:57.327764 openbb_stockgrid-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1024 1970-01-01 00:00:00.000000 openbb_stockgrid-1.2.1/PKG-INFO
```

### Comparing `openbb_stockgrid-1.2.0/openbb_stockgrid/__init__.py` & `openbb_stockgrid-1.2.1/openbb_stockgrid/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_stockgrid-1.2.0/openbb_stockgrid/models/short_volume.py` & `openbb_stockgrid-1.2.1/openbb_stockgrid/models/short_volume.py`

 * *Files identical despite different names*

### Comparing `openbb_stockgrid-1.2.0/pyproject.toml` & `openbb_stockgrid-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-stockgrid"
-version = "1.2.0"
+version = "1.2.1"
 description = "stockgrid extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_stockgrid" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 pytest-freezegun = "^0.4.2"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_stockgrid-1.2.0/PKG-INFO` & `openbb_stockgrid-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-stockgrid
-Version: 1.2.0
+Version: 1.2.1
 Summary: stockgrid extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: pytest-freezegun (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Stockgrid Provider
 
 This extension integrates the [Stockgrid](https://Stockgrid.io/) data provider into the OpenBB Platform.
```

