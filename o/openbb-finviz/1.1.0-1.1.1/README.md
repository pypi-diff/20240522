# Comparing `tmp/openbb_finviz-1.1.0.tar.gz` & `tmp/openbb_finviz-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_finviz-1.1.0.tar", max compression
+gzip compressed data, was "openbb_finviz-1.1.1.tar", max compression
```

## Comparing `openbb_finviz-1.1.0.tar` & `openbb_finviz-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      315 2024-05-15 14:25:46.006898 openbb_finviz-1.1.0/README.md
--rw-r--r--   0        0        0     1029 2024-05-14 15:30:05.612881 openbb_finviz-1.1.0/openbb_finviz/__init__.py
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.665328 openbb_finviz-1.1.0/openbb_finviz/models/__init__.py
--rw-r--r--   0        0        0     9621 2024-05-09 15:04:29.070455 openbb_finviz-1.1.0/openbb_finviz/models/compare_groups.py
--rw-r--r--   0        0        0     8254 2024-05-10 10:40:27.291294 openbb_finviz-1.1.0/openbb_finviz/models/equity_profile.py
--rw-r--r--   0        0        0    11039 2024-05-10 10:40:27.291399 openbb_finviz-1.1.0/openbb_finviz/models/key_metrics.py
--rw-r--r--   0        0        0     4395 2024-05-15 11:17:30.040928 openbb_finviz-1.1.0/openbb_finviz/models/price_performance.py
--rw-r--r--   0        0        0     3932 2024-05-10 10:40:27.291736 openbb_finviz-1.1.0/openbb_finviz/models/price_target.py
--rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630717 openbb_finviz-1.1.0/openbb_finviz/models/py.typed
--rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630748 openbb_finviz-1.1.0/openbb_finviz/py.typed
--rw-r--r--   0        0        0       29 2024-04-23 10:22:39.665571 openbb_finviz-1.1.0/openbb_finviz/utils/__init__.py
--rw-r--r--   0        0        0     1122 2024-04-08 12:02:16.630850 openbb_finviz-1.1.0/openbb_finviz/utils/definitions.py
--rw-r--r--   0        0        0        0 2024-04-08 12:02:16.630874 openbb_finviz-1.1.0/openbb_finviz/utils/py.typed
--rw-r--r--   0        0        0      503 2024-05-15 16:05:18.824210 openbb_finviz-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 openbb_finviz-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      315 2024-05-22 11:48:40.527330 openbb_finviz-1.1.1/README.md
+-rw-r--r--   0        0        0     1029 2024-05-15 09:21:56.069885 openbb_finviz-1.1.1/openbb_finviz/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/models/__init__.py
+-rw-r--r--   0        0        0     9621 2024-05-15 09:21:56.069885 openbb_finviz-1.1.1/openbb_finviz/models/compare_groups.py
+-rw-r--r--   0        0        0     8254 2024-05-15 09:21:56.069885 openbb_finviz-1.1.1/openbb_finviz/models/equity_profile.py
+-rw-r--r--   0        0        0    11039 2024-05-15 09:21:56.069885 openbb_finviz-1.1.1/openbb_finviz/models/key_metrics.py
+-rw-r--r--   0        0        0     4395 2024-05-15 11:30:49.639743 openbb_finviz-1.1.1/openbb_finviz/models/price_performance.py
+-rw-r--r--   0        0        0     3932 2024-05-15 09:21:56.069885 openbb_finviz-1.1.1/openbb_finviz/models/price_target.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/models/py.typed
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/py.typed
+-rw-r--r--   0        0        0       29 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/utils/__init__.py
+-rw-r--r--   0        0        0     1122 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/utils/definitions.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.853864 openbb_finviz-1.1.1/openbb_finviz/utils/py.typed
+-rw-r--r--   0        0        0      503 2024-05-22 13:56:20.483641 openbb_finviz-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 openbb_finviz-1.1.1/PKG-INFO
```

### Comparing `openbb_finviz-1.1.0/openbb_finviz/__init__.py` & `openbb_finviz-1.1.1/openbb_finviz/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/models/compare_groups.py` & `openbb_finviz-1.1.1/openbb_finviz/models/compare_groups.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/models/equity_profile.py` & `openbb_finviz-1.1.1/openbb_finviz/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/models/key_metrics.py` & `openbb_finviz-1.1.1/openbb_finviz/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/models/price_performance.py` & `openbb_finviz-1.1.1/openbb_finviz/models/price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/models/price_target.py` & `openbb_finviz-1.1.1/openbb_finviz/models/price_target.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/openbb_finviz/utils/definitions.py` & `openbb_finviz-1.1.1/openbb_finviz/utils/definitions.py`

 * *Files identical despite different names*

### Comparing `openbb_finviz-1.1.0/PKG-INFO` & `openbb_finviz-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-finviz
-Version: 1.1.0
+Version: 1.1.1
 Summary: Finviz extension for OpenBB
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
 Requires-Dist: finvizfinance (==0.14.7)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Finviz Data Provider Extension
 
 This extension integrates the [Finviz](https://finviz.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

