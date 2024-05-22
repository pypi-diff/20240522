# Comparing `tmp/openbb_wsj-1.2.0.tar.gz` & `tmp/openbb_wsj-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_wsj-1.2.0.tar", max compression
+gzip compressed data, was "openbb_wsj-1.2.1.tar", max compression
```

## Comparing `openbb_wsj-1.2.0.tar` & `openbb_wsj-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      300 2024-05-15 14:24:28.442108 openbb_wsj-1.2.0/README.md
--rw-r--r--   0        0        0     1071 2024-05-14 15:30:05.621595 openbb_wsj-1.2.0/openbb_wsj/__init__.py
--rw-r--r--   0        0        0     3077 2024-02-29 11:03:36.977934 openbb_wsj-1.2.0/openbb_wsj/models/active.py
--rw-r--r--   0        0        0     3277 2024-04-08 12:02:16.764578 openbb_wsj-1.2.0/openbb_wsj/models/gainers.py
--rw-r--r--   0        0        0     3266 2024-04-08 12:02:16.764674 openbb_wsj-1.2.0/openbb_wsj/models/losers.py
--rw-r--r--   0        0        0      459 2024-05-15 16:05:29.883147 openbb_wsj-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 openbb_wsj-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-05-22 11:48:40.551330 openbb_wsj-1.2.1/README.md
+-rw-r--r--   0        0        0     1071 2024-05-15 09:21:56.109886 openbb_wsj-1.2.1/openbb_wsj/__init__.py
+-rw-r--r--   0        0        0     3077 2024-05-14 16:56:42.341866 openbb_wsj-1.2.1/openbb_wsj/models/active.py
+-rw-r--r--   0        0        0     3277 2024-05-14 16:56:42.341866 openbb_wsj-1.2.1/openbb_wsj/models/gainers.py
+-rw-r--r--   0        0        0     3266 2024-05-14 16:56:42.341866 openbb_wsj-1.2.1/openbb_wsj/models/losers.py
+-rw-r--r--   0        0        0      459 2024-05-22 13:57:32.739881 openbb_wsj-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 openbb_wsj-1.2.1/PKG-INFO
```

### Comparing `openbb_wsj-1.2.0/openbb_wsj/__init__.py` & `openbb_wsj-1.2.1/openbb_wsj/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.2.0/openbb_wsj/models/active.py` & `openbb_wsj-1.2.1/openbb_wsj/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.2.0/openbb_wsj/models/gainers.py` & `openbb_wsj-1.2.1/openbb_wsj/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.2.0/openbb_wsj/models/losers.py` & `openbb_wsj-1.2.1/openbb_wsj/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_wsj-1.2.0/PKG-INFO` & `openbb_wsj-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-wsj
-Version: 1.2.0
+Version: 1.2.1
 Summary: wsj extension for OpenBB
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
 
 # OpenBB Wall St Journal Provider
 
 This extension integrates the [WSJ](https://wsj.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

