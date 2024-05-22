# Comparing `tmp/openbb_polygon-1.2.0.tar.gz` & `tmp/openbb_polygon-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_polygon-1.2.0.tar", max compression
+gzip compressed data, was "openbb_polygon-1.2.1.tar", max compression
```

## Comparing `openbb_polygon-1.2.0.tar` & `openbb_polygon-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      303 2024-05-15 14:25:08.997475 openbb_polygon-1.2.0/README.md
--rw-r--r--   0        0        0     2871 2024-05-14 15:30:05.617960 openbb_polygon-1.2.0/openbb_polygon/__init__.py
--rw-r--r--   0        0        0       43 2024-04-23 10:22:39.678191 openbb_polygon-1.2.0/openbb_polygon/models/__init__.py
--rw-r--r--   0        0        0     9313 2024-04-02 11:35:59.508406 openbb_polygon-1.2.0/openbb_polygon/models/balance_sheet.py
--rw-r--r--   0        0        0     7039 2024-05-09 13:34:29.229455 openbb_polygon-1.2.0/openbb_polygon/models/cash_flow.py
--rw-r--r--   0        0        0     4606 2024-05-10 10:40:27.300299 openbb_polygon-1.2.0/openbb_polygon/models/company_news.py
--rw-r--r--   0        0        0     6289 2024-05-10 10:40:27.300493 openbb_polygon-1.2.0/openbb_polygon/models/crypto_historical.py
--rw-r--r--   0        0        0     6261 2024-05-10 10:40:27.300668 openbb_polygon-1.2.0/openbb_polygon/models/currency_historical.py
--rw-r--r--   0        0        0     5135 2024-05-09 15:04:29.071926 openbb_polygon-1.2.0/openbb_polygon/models/currency_pairs.py
--rw-r--r--   0        0        0     9871 2024-05-10 10:40:27.300830 openbb_polygon-1.2.0/openbb_polygon/models/currency_snapshots.py
--rw-r--r--   0        0        0     7156 2024-05-10 10:40:27.301011 openbb_polygon-1.2.0/openbb_polygon/models/equity_historical.py
--rw-r--r--   0        0        0     8240 2024-04-08 12:02:16.668848 openbb_polygon-1.2.0/openbb_polygon/models/equity_nbbo.py
--rw-r--r--   0        0        0    13663 2024-04-08 12:02:16.668984 openbb_polygon-1.2.0/openbb_polygon/models/income_statement.py
--rw-r--r--   0        0        0     6148 2024-05-10 10:40:27.301163 openbb_polygon-1.2.0/openbb_polygon/models/index_historical.py
--rw-r--r--   0        0        0     3734 2024-04-23 10:22:39.678939 openbb_polygon-1.2.0/openbb_polygon/models/market_indices.py
--rw-r--r--   0        0        0     6126 2024-04-08 12:02:16.669327 openbb_polygon-1.2.0/openbb_polygon/models/market_snapshots.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.887235 openbb_polygon-1.2.0/openbb_polygon/py.typed
--rw-r--r--   0        0        0       28 2024-04-23 10:22:39.679023 openbb_polygon-1.2.0/openbb_polygon/utils/__init__.py
--rw-r--r--   0        0        0     3708 2024-04-23 10:22:39.679139 openbb_polygon-1.2.0/openbb_polygon/utils/helpers.py
--rw-r--r--   0        0        0      483 2024-05-15 16:06:03.353141 openbb_polygon-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 openbb_polygon-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      303 2024-05-22 11:48:40.539330 openbb_polygon-1.2.1/README.md
+-rw-r--r--   0        0        0     2871 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-14 16:56:41.933865 openbb_polygon-1.2.1/openbb_polygon/models/__init__.py
+-rw-r--r--   0        0        0     9313 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/models/balance_sheet.py
+-rw-r--r--   0        0        0     7039 2024-05-14 16:57:23.602033 openbb_polygon-1.2.1/openbb_polygon/models/cash_flow.py
+-rw-r--r--   0        0        0     4606 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/company_news.py
+-rw-r--r--   0        0        0     6289 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/crypto_historical.py
+-rw-r--r--   0        0        0     6261 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/currency_historical.py
+-rw-r--r--   0        0        0     5135 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/currency_pairs.py
+-rw-r--r--   0        0        0     9871 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/currency_snapshots.py
+-rw-r--r--   0        0        0     7156 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/equity_historical.py
+-rw-r--r--   0        0        0     8240 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/models/equity_nbbo.py
+-rw-r--r--   0        0        0    13663 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/models/income_statement.py
+-rw-r--r--   0        0        0     6148 2024-05-15 09:21:56.089885 openbb_polygon-1.2.1/openbb_polygon/models/index_historical.py
+-rw-r--r--   0        0        0     3734 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/models/market_indices.py
+-rw-r--r--   0        0        0     6126 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/models/market_snapshots.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/py.typed
+-rw-r--r--   0        0        0       28 2024-05-14 16:56:41.937865 openbb_polygon-1.2.1/openbb_polygon/utils/__init__.py
+-rw-r--r--   0        0        0     3696 2024-05-22 11:48:40.539330 openbb_polygon-1.2.1/openbb_polygon/utils/helpers.py
+-rw-r--r--   0        0        0      483 2024-05-22 13:56:42.483714 openbb_polygon-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      963 1970-01-01 00:00:00.000000 openbb_polygon-1.2.1/PKG-INFO
```

### Comparing `openbb_polygon-1.2.0/openbb_polygon/__init__.py` & `openbb_polygon-1.2.1/openbb_polygon/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/balance_sheet.py` & `openbb_polygon-1.2.1/openbb_polygon/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/cash_flow.py` & `openbb_polygon-1.2.1/openbb_polygon/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/company_news.py` & `openbb_polygon-1.2.1/openbb_polygon/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/crypto_historical.py` & `openbb_polygon-1.2.1/openbb_polygon/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/currency_historical.py` & `openbb_polygon-1.2.1/openbb_polygon/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/currency_pairs.py` & `openbb_polygon-1.2.1/openbb_polygon/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/currency_snapshots.py` & `openbb_polygon-1.2.1/openbb_polygon/models/currency_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/equity_historical.py` & `openbb_polygon-1.2.1/openbb_polygon/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/equity_nbbo.py` & `openbb_polygon-1.2.1/openbb_polygon/models/equity_nbbo.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/income_statement.py` & `openbb_polygon-1.2.1/openbb_polygon/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/index_historical.py` & `openbb_polygon-1.2.1/openbb_polygon/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/market_indices.py` & `openbb_polygon-1.2.1/openbb_polygon/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/models/market_snapshots.py` & `openbb_polygon-1.2.1/openbb_polygon/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_polygon-1.2.0/openbb_polygon/utils/helpers.py` & `openbb_polygon-1.2.1/openbb_polygon/utils/helpers.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 async def response_callback(
     response: ClientResponse, _: ClientSession
 ) -> Union[dict, List[dict]]:
     """Use callback for make_request."""
     data: Dict = await response.json()  # type: ignore
 
     if response.status != 200:
-        message = data.get("error", None) or data.get("message", None)
+        message = data.get("error") or data.get("message")
         raise RuntimeError(f"Error in Polygon request -> {message}")
 
     keys_in_data = "results" in data or "tickers" in data
 
     if not keys_in_data or len(data) == 0:
         raise EmptyDataError()
```

### Comparing `openbb_polygon-1.2.0/PKG-INFO` & `openbb_polygon-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-polygon
-Version: 1.2.0
+Version: 1.2.1
 Summary: Polygon extension for OpenBB
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
 
 # OpenBB Polygon Provider
 
 This extension integrates the [Polygon](https://polygon.io/) data provider into the OpenBB Platform.
 
 ## Installation
```

