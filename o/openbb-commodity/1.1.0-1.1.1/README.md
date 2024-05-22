# Comparing `tmp/openbb_commodity-1.1.0.tar.gz` & `tmp/openbb_commodity-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_commodity-1.1.0.tar", max compression
+gzip compressed data, was "openbb_commodity-1.1.1.tar", max compression
```

## Comparing `openbb_commodity-1.1.0.tar` & `openbb_commodity-1.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0      332 2024-05-15 14:27:23.324681 openbb_commodity-1.1.0/README.md
--rw-r--r--   0        0        0       34 2024-04-23 10:22:39.591940 openbb_commodity-1.1.0/openbb_commodity/__init__.py
--rw-r--r--   0        0        0     1298 2024-04-23 10:22:39.592095 openbb_commodity-1.1.0/openbb_commodity/commodity_router.py
--rw-r--r--   0        0        0      496 2024-05-15 16:04:09.706991 openbb_commodity-1.1.0/pyproject.toml
--rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 openbb_commodity-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      332 2024-05-22 11:48:40.395330 openbb_commodity-1.1.1/README.md
+-rw-r--r--   0        0        0       34 2024-05-14 16:56:41.553863 openbb_commodity-1.1.1/openbb_commodity/__init__.py
+-rw-r--r--   0        0        0     1298 2024-05-14 16:56:41.553863 openbb_commodity-1.1.1/openbb_commodity/commodity_router.py
+-rw-r--r--   0        0        0      496 2024-05-22 13:54:47.071331 openbb_commodity-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0      996 1970-01-01 00:00:00.000000 openbb_commodity-1.1.1/PKG-INFO
```

### Comparing `openbb_commodity-1.1.0/openbb_commodity/commodity_router.py` & `openbb_commodity-1.1.1/openbb_commodity/commodity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_commodity-1.1.0/PKG-INFO` & `openbb_commodity-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-commodity
-Version: 1.1.0
+Version: 1.1.1
 Summary: Commodity extension for OpenBB
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
 
 # Commodity Extension for OpenBB Platform
 
 This extension provides a set of commands for commodity-related data.
 
 ## Installation
```

