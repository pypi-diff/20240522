# Comparing `tmp/openbb_biztoc-1.2.0.tar.gz` & `tmp/openbb_biztoc-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_biztoc-1.2.0.tar", max compression
+gzip compressed data, was "openbb_biztoc-1.2.1.tar", max compression
```

## Comparing `openbb_biztoc-1.2.0.tar` & `openbb_biztoc-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      319 2024-05-15 14:26:14.052690 openbb_biztoc-1.2.0/README.md
--rw-r--r--   0        0        0     1559 2024-05-14 15:30:05.610553 openbb_biztoc-1.2.0/openbb_biztoc/__init__.py
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.653849 openbb_biztoc-1.2.0/openbb_biztoc/models/__init__.py
--rw-r--r--   0        0        0     4199 2024-04-08 12:02:16.580761 openbb_biztoc-1.2.0/openbb_biztoc/models/world_news.py
--rw-r--r--   0        0        0       20 2024-04-23 10:22:39.653933 openbb_biztoc-1.2.0/openbb_biztoc/utils/__init__.py
--rw-r--r--   0        0        0     3916 2024-04-23 10:22:39.654037 openbb_biztoc-1.2.0/openbb_biztoc/utils/helpers.py
--rw-r--r--   0        0        0      476 2024-05-15 16:06:31.748997 openbb_biztoc-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 openbb_biztoc-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      319 2024-05-22 11:48:40.467330 openbb_biztoc-1.2.1/README.md
+-rw-r--r--   0        0        0     1559 2024-05-15 09:21:56.057885 openbb_biztoc-1.2.1/openbb_biztoc/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:41.677864 openbb_biztoc-1.2.1/openbb_biztoc/models/__init__.py
+-rw-r--r--   0        0        0     4199 2024-05-14 16:56:41.677864 openbb_biztoc-1.2.1/openbb_biztoc/models/world_news.py
+-rw-r--r--   0        0        0       20 2024-05-14 16:56:41.677864 openbb_biztoc-1.2.1/openbb_biztoc/utils/__init__.py
+-rw-r--r--   0        0        0     3916 2024-05-14 16:56:41.677864 openbb_biztoc-1.2.1/openbb_biztoc/utils/helpers.py
+-rw-r--r--   0        0        0      476 2024-05-22 13:56:47.459731 openbb_biztoc-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      997 1970-01-01 00:00:00.000000 openbb_biztoc-1.2.1/PKG-INFO
```

### Comparing `openbb_biztoc-1.2.0/openbb_biztoc/__init__.py` & `openbb_biztoc-1.2.1/openbb_biztoc/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.2.0/openbb_biztoc/models/world_news.py` & `openbb_biztoc-1.2.1/openbb_biztoc/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.2.0/openbb_biztoc/utils/helpers.py` & `openbb_biztoc-1.2.1/openbb_biztoc/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_biztoc-1.2.0/PKG-INFO` & `openbb_biztoc-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-biztoc
-Version: 1.2.0
+Version: 1.2.1
 Summary: 
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
 Requires-Dist: requests-cache (>=1.1.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Biztoc Provider
 
 This extension integrates the Biztoc data provider
 into the OpenBB Platform.
```

