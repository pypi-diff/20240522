# Comparing `tmp/openbb_finra-1.2.0.tar.gz` & `tmp/openbb_finra-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finra-1.2.0.tar", max compression
+gzip compressed data, was "openbb_finra-1.2.1.tar", max compression
```

## Comparing `openbb_finra-1.2.0.tar` & `openbb_finra-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      296 2024-05-15 14:25:50.021203 openbb_finra-1.2.0/README.md
--rw-r--r--   0        0        0      719 2024-05-14 15:30:05.612451 openbb_finra-1.2.0/openbb_finra/__init__.py
--rw-r--r--   0        0        0     2891 2024-04-08 12:02:16.629529 openbb_finra-1.2.0/openbb_finra/models/equity_short_interest.py
--rw-r--r--   0        0        0     2079 2024-04-08 12:02:16.629624 openbb_finra-1.2.0/openbb_finra/models/otc_aggregate.py
--rw-r--r--   0        0        0     2270 2024-04-08 12:02:16.629733 openbb_finra-1.2.0/openbb_finra/utils/data_storage.py
--rw-r--r--   0        0        0     5553 2024-04-23 10:22:39.664081 openbb_finra-1.2.0/openbb_finra/utils/helpers.py
--rw-r--r--   0        0        0      471 2024-05-15 16:06:09.380712 openbb_finra-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 openbb_finra-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      296 2024-05-22 11:48:40.527330 openbb_finra-1.2.1/README.md
+-rw-r--r--   0        0        0      719 2024-05-15 09:21:56.065885 openbb_finra-1.2.1/openbb_finra/__init__.py
+-rw-r--r--   0        0        0     2891 2024-05-14 16:56:41.777864 openbb_finra-1.2.1/openbb_finra/models/equity_short_interest.py
+-rw-r--r--   0        0        0     2079 2024-05-14 16:56:41.777864 openbb_finra-1.2.1/openbb_finra/models/otc_aggregate.py
+-rw-r--r--   0        0        0     2270 2024-05-14 16:56:41.777864 openbb_finra-1.2.1/openbb_finra/utils/data_storage.py
+-rw-r--r--   0        0        0     5553 2024-05-14 16:56:41.777864 openbb_finra-1.2.1/openbb_finra/utils/helpers.py
+-rw-r--r--   0        0        0      471 2024-05-22 13:57:47.691930 openbb_finra-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 openbb_finra-1.2.1/PKG-INFO
```

### Comparing `openbb_finra-1.2.0/openbb_finra/__init__.py` & `openbb_finra-1.2.1/openbb_finra/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.2.0/openbb_finra/models/equity_short_interest.py` & `openbb_finra-1.2.1/openbb_finra/models/equity_short_interest.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.2.0/openbb_finra/models/otc_aggregate.py` & `openbb_finra-1.2.1/openbb_finra/models/otc_aggregate.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.2.0/openbb_finra/utils/data_storage.py` & `openbb_finra-1.2.1/openbb_finra/utils/data_storage.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.2.0/openbb_finra/utils/helpers.py` & `openbb_finra-1.2.1/openbb_finra/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_finra-1.2.0/PKG-INFO` & `openbb_finra-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-finra
-Version: 1.2.0
+Version: 1.2.1
 Summary: FINRA extension for OpenBB
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
 
 # OpenBB FINRA Provider
 
 This extension integrates the [FINRA](https://finra.org/) data provider into the OpenBB Platform.
 
 ## Installation
```

