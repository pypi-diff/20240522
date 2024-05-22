# Comparing `tmp/openbb_index-1.2.0.tar.gz` & `tmp/openbb_index-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_index-1.2.0.tar", max compression
+gzip compressed data, was "openbb_index-1.2.1.tar", max compression
```

## Comparing `openbb_index-1.2.0.tar` & `openbb_index-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      333 2024-05-15 14:26:49.501757 openbb_index-1.2.0/README.md
--rw-r--r--   0        0        0       23 2024-02-29 11:03:36.740144 openbb_index-1.2.0/openbb_index/__init__.py
--rw-r--r--   0        0        0     4097 2024-04-23 10:22:39.605412 openbb_index-1.2.0/openbb_index/index_router.py
--rw-r--r--   0        0        0       19 2024-04-08 12:02:10.402459 openbb_index-1.2.0/openbb_index/price/__init__.py
--rw-r--r--   0        0        0      999 2024-04-08 12:02:16.530616 openbb_index-1.2.0/openbb_index/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.740242 openbb_index-1.2.0/openbb_index/py.typed
--rw-r--r--   0        0        0      472 2024-05-15 16:04:44.792679 openbb_index-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 openbb_index-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      333 2024-05-22 11:48:40.407330 openbb_index-1.2.1/README.md
+-rw-r--r--   0        0        0       23 2024-05-14 16:56:41.569863 openbb_index-1.2.1/openbb_index/__init__.py
+-rw-r--r--   0        0        0     4097 2024-05-14 16:56:41.569863 openbb_index-1.2.1/openbb_index/index_router.py
+-rw-r--r--   0        0        0       19 2024-05-14 16:56:41.569863 openbb_index-1.2.1/openbb_index/price/__init__.py
+-rw-r--r--   0        0        0      999 2024-05-14 16:56:41.569863 openbb_index-1.2.1/openbb_index/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.569863 openbb_index-1.2.1/openbb_index/py.typed
+-rw-r--r--   0        0        0      472 2024-05-22 13:55:02.435382 openbb_index-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      989 1970-01-01 00:00:00.000000 openbb_index-1.2.1/PKG-INFO
```

### Comparing `openbb_index-1.2.0/openbb_index/index_router.py` & `openbb_index-1.2.1/openbb_index/index_router.py`

 * *Files identical despite different names*

### Comparing `openbb_index-1.2.0/openbb_index/price/price_router.py` & `openbb_index-1.2.1/openbb_index/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_index-1.2.0/PKG-INFO` & `openbb_index-1.2.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-index
-Version: 1.2.0
+Version: 1.2.1
 Summary: Index extension for OpenBB
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
 Description-Content-Type: text/markdown
 
 # OpenBB Index Extension
 
 The Index extension provides global and european index data access for the OpenBB Platform.
 
 ## Installation
```

