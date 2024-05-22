# Comparing `tmp/openbb_tradier-1.1.0.tar.gz` & `tmp/openbb_tradier-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradier-1.1.0.tar", max compression
+gzip compressed data, was "openbb_tradier-1.1.1.tar", max compression
```

## Comparing `openbb_tradier-1.1.0.tar` & `openbb_tradier-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      558 2024-05-15 14:32:56.427613 openbb_tradier-1.1.0/README.md
--rw-r--r--   0        0        0     1740 2024-05-14 15:30:05.620279 openbb_tradier-1.1.0/openbb_tradier/__init__.py
--rw-r--r--   0        0        0       31 2024-04-23 10:22:39.796948 openbb_tradier-1.1.0/openbb_tradier/models/__init__.py
--rw-r--r--   0        0        0     6588 2024-05-10 10:40:27.303718 openbb_tradier-1.1.0/openbb_tradier/models/equity_historical.py
--rw-r--r--   0        0        0     9228 2024-05-10 10:40:27.304076 openbb_tradier-1.1.0/openbb_tradier/models/equity_quote.py
--rw-r--r--   0        0        0     4124 2024-04-08 12:02:16.760537 openbb_tradier-1.1.0/openbb_tradier/models/equity_search.py
--rw-r--r--   0        0        0    10325 2024-04-23 10:22:39.797971 openbb_tradier-1.1.0/openbb_tradier/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-04-08 12:02:16.760617 openbb_tradier-1.1.0/openbb_tradier/py.typed
--rw-r--r--   0        0        0       30 2024-04-23 10:22:39.798100 openbb_tradier-1.1.0/openbb_tradier/utils/__init__.py
--rw-r--r--   0        0        0     1341 2024-04-08 12:02:16.760718 openbb_tradier-1.1.0/openbb_tradier/utils/constants.py
--rw-r--r--   0        0        0      500 2024-05-15 16:05:23.906169 openbb_tradier-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 openbb_tradier-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      558 2024-05-22 11:48:40.547330 openbb_tradier-1.1.1/README.md
+-rw-r--r--   0        0        0     1740 2024-05-15 09:21:56.105885 openbb_tradier-1.1.1/openbb_tradier/__init__.py
+-rw-r--r--   0        0        0       31 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/models/__init__.py
+-rw-r--r--   0        0        0     6588 2024-05-15 09:21:56.105885 openbb_tradier-1.1.1/openbb_tradier/models/equity_historical.py
+-rw-r--r--   0        0        0     9228 2024-05-15 09:21:56.105885 openbb_tradier-1.1.1/openbb_tradier/models/equity_quote.py
+-rw-r--r--   0        0        0     4124 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/models/equity_search.py
+-rw-r--r--   0        0        0    10325 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/py.typed
+-rw-r--r--   0        0        0       30 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/utils/__init__.py
+-rw-r--r--   0        0        0     1341 2024-05-14 16:56:42.333866 openbb_tradier-1.1.1/openbb_tradier/utils/constants.py
+-rw-r--r--   0        0        0      500 2024-05-22 13:57:43.051915 openbb_tradier-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1235 1970-01-01 00:00:00.000000 openbb_tradier-1.1.1/PKG-INFO
```

### Comparing `openbb_tradier-1.1.0/README.md` & `openbb_tradier-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/__init__.py` & `openbb_tradier-1.1.1/openbb_tradier/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/models/equity_historical.py` & `openbb_tradier-1.1.1/openbb_tradier/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/models/equity_quote.py` & `openbb_tradier-1.1.1/openbb_tradier/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/models/equity_search.py` & `openbb_tradier-1.1.1/openbb_tradier/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/models/options_chains.py` & `openbb_tradier-1.1.1/openbb_tradier/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/openbb_tradier/utils/constants.py` & `openbb_tradier-1.1.1/openbb_tradier/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_tradier-1.1.0/PKG-INFO` & `openbb_tradier-1.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-tradier
-Version: 1.1.0
+Version: 1.1.1
 Summary: Tradier Provider Extension for the OpenBB Platform
 License: AGPL-3.0-only
 Author: OpenBB
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
 
 # OpenBB Tradier Provider
 
 This extension integrates the [Tradier](https://tradier.com) data provider into the OpenBB Platform.
 
 ## Installation
```

