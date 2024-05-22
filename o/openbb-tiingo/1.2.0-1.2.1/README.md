# Comparing `tmp/openbb_tiingo-1.2.0.tar.gz` & `tmp/openbb_tiingo-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tiingo-1.2.0.tar", max compression
+gzip compressed data, was "openbb_tiingo-1.2.1.tar", max compression
```

## Comparing `openbb_tiingo-1.2.0.tar` & `openbb_tiingo-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      304 2024-05-15 14:29:35.406731 openbb_tiingo-1.2.0/README.md
--rw-r--r--   0        0        0     1260 2024-05-14 15:30:05.619556 openbb_tiingo-1.2.0/openbb_tiingo/__init__.py
--rw-r--r--   0        0        0       21 2024-02-29 11:03:36.971894 openbb_tiingo-1.2.0/openbb_tiingo/models/__init__.py
--rw-r--r--   0        0        0     3657 2024-05-10 10:40:27.301343 openbb_tiingo-1.2.0/openbb_tiingo/models/company_news.py
--rw-r--r--   0        0        0     5313 2024-05-10 10:40:27.301906 openbb_tiingo-1.2.0/openbb_tiingo/models/crypto_historical.py
--rw-r--r--   0        0        0     4680 2024-05-10 10:40:27.302091 openbb_tiingo-1.2.0/openbb_tiingo/models/currency_historical.py
--rw-r--r--   0        0        0     5341 2024-05-10 10:40:27.302261 openbb_tiingo-1.2.0/openbb_tiingo/models/equity_historical.py
--rw-r--r--   0        0        0     2131 2024-04-02 11:35:59.532576 openbb_tiingo-1.2.0/openbb_tiingo/models/trailing_dividend_yield.py
--rw-r--r--   0        0        0     3657 2024-04-08 12:02:16.680377 openbb_tiingo-1.2.0/openbb_tiingo/models/world_news.py
--rw-r--r--   0        0        0       22 2024-02-29 11:03:36.972367 openbb_tiingo-1.2.0/openbb_tiingo/utils/__init__.py
--rw-r--r--   0        0        0     2909 2024-02-29 11:03:36.972440 openbb_tiingo-1.2.0/openbb_tiingo/utils/helpers.py
--rw-r--r--   0        0        0      477 2024-05-15 16:06:54.282954 openbb_tiingo-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 openbb_tiingo-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      304 2024-05-22 11:48:40.547330 openbb_tiingo-1.2.1/README.md
+-rw-r--r--   0        0        0     1260 2024-05-15 09:21:56.101885 openbb_tiingo-1.2.1/openbb_tiingo/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-14 16:56:42.113865 openbb_tiingo-1.2.1/openbb_tiingo/models/__init__.py
+-rw-r--r--   0        0        0     3657 2024-05-15 09:21:56.101885 openbb_tiingo-1.2.1/openbb_tiingo/models/company_news.py
+-rw-r--r--   0        0        0     5313 2024-05-15 09:21:56.101885 openbb_tiingo-1.2.1/openbb_tiingo/models/crypto_historical.py
+-rw-r--r--   0        0        0     4680 2024-05-15 09:21:56.101885 openbb_tiingo-1.2.1/openbb_tiingo/models/currency_historical.py
+-rw-r--r--   0        0        0     5341 2024-05-15 09:21:56.101885 openbb_tiingo-1.2.1/openbb_tiingo/models/equity_historical.py
+-rw-r--r--   0        0        0     2131 2024-05-14 16:56:42.113865 openbb_tiingo-1.2.1/openbb_tiingo/models/trailing_dividend_yield.py
+-rw-r--r--   0        0        0     3657 2024-05-14 16:56:42.113865 openbb_tiingo-1.2.1/openbb_tiingo/models/world_news.py
+-rw-r--r--   0        0        0       22 2024-05-14 16:56:42.113865 openbb_tiingo-1.2.1/openbb_tiingo/utils/__init__.py
+-rw-r--r--   0        0        0     2909 2024-05-14 16:56:42.113865 openbb_tiingo-1.2.1/openbb_tiingo/utils/helpers.py
+-rw-r--r--   0        0        0      477 2024-05-22 13:58:16.676026 openbb_tiingo-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      962 1970-01-01 00:00:00.000000 openbb_tiingo-1.2.1/PKG-INFO
```

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/__init__.py` & `openbb_tiingo-1.2.1/openbb_tiingo/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/company_news.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/crypto_historical.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/currency_historical.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/equity_historical.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/trailing_dividend_yield.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/trailing_dividend_yield.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/models/world_news.py` & `openbb_tiingo-1.2.1/openbb_tiingo/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/openbb_tiingo/utils/helpers.py` & `openbb_tiingo-1.2.1/openbb_tiingo/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_tiingo-1.2.0/PKG-INFO` & `openbb_tiingo-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-tiingo
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tiingo extension for OpenBB
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
 
 # OpenBB Tiingo Provider
 
 This extension integrates the [Tiingo](https://www.tiingo.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

