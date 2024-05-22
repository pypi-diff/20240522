# Comparing `tmp/openbb_tmx-1.1.0.tar.gz` & `tmp/openbb_tmx-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tmx-1.1.0.tar", max compression
+gzip compressed data, was "openbb_tmx-1.1.1.tar", max compression
```

## Comparing `openbb_tmx-1.1.0.tar` & `openbb_tmx-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     2637 2024-05-15 14:32:00.047970 openbb_tmx-1.1.0/README.md
--rw-r--r--   0        0        0     3325 2024-05-14 15:30:05.619866 openbb_tmx-1.1.0/openbb_tmx/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 10:22:39.794265 openbb_tmx-1.1.0/openbb_tmx/models/__init__.py
--rw-r--r--   0        0        0     4695 2024-04-08 12:02:16.691753 openbb_tmx-1.1.0/openbb_tmx/models/available_indices.py
--rw-r--r--   0        0        0     6306 2024-05-09 15:04:29.073848 openbb_tmx-1.1.0/openbb_tmx/models/bond_prices.py
--rw-r--r--   0        0        0     5166 2024-05-09 15:04:29.073990 openbb_tmx-1.1.0/openbb_tmx/models/calendar_earnings.py
--rw-r--r--   0        0        0     5814 2024-04-08 12:02:16.691957 openbb_tmx-1.1.0/openbb_tmx/models/company_filings.py
--rw-r--r--   0        0        0     4653 2024-05-10 10:40:27.302449 openbb_tmx-1.1.0/openbb_tmx/models/company_news.py
--rw-r--r--   0        0        0     8853 2024-05-10 10:40:27.302575 openbb_tmx-1.1.0/openbb_tmx/models/equity_historical.py
--rw-r--r--   0        0        0     5461 2024-05-10 10:40:27.302741 openbb_tmx-1.1.0/openbb_tmx/models/equity_profile.py
--rw-r--r--   0        0        0    12481 2024-05-10 10:40:27.302886 openbb_tmx-1.1.0/openbb_tmx/models/equity_quote.py
--rw-r--r--   0        0        0     2223 2024-04-08 12:02:16.692386 openbb_tmx-1.1.0/openbb_tmx/models/equity_search.py
--rw-r--r--   0        0        0     3644 2024-05-10 10:40:27.303031 openbb_tmx-1.1.0/openbb_tmx/models/etf_countries.py
--rw-r--r--   0        0        0     5093 2024-05-09 15:04:29.074766 openbb_tmx-1.1.0/openbb_tmx/models/etf_holdings.py
--rw-r--r--   0        0        0     8463 2024-05-10 10:40:27.303171 openbb_tmx-1.1.0/openbb_tmx/models/etf_info.py
--rw-r--r--   0        0        0     9711 2024-05-09 15:04:29.075187 openbb_tmx-1.1.0/openbb_tmx/models/etf_search.py
--rw-r--r--   0        0        0     2633 2024-04-08 12:02:16.692727 openbb_tmx-1.1.0/openbb_tmx/models/etf_sectors.py
--rw-r--r--   0        0        0     4479 2024-04-23 10:22:39.794929 openbb_tmx-1.1.0/openbb_tmx/models/gainers.py
--rw-r--r--   0        0        0     3584 2024-04-08 12:02:16.692861 openbb_tmx-1.1.0/openbb_tmx/models/historical_dividends.py
--rw-r--r--   0        0        0     3098 2024-04-23 10:22:39.795036 openbb_tmx-1.1.0/openbb_tmx/models/index_constituents.py
--rw-r--r--   0        0        0     2837 2024-04-08 12:02:16.692990 openbb_tmx-1.1.0/openbb_tmx/models/index_sectors.py
--rw-r--r--   0        0        0    10349 2024-05-09 15:04:29.075380 openbb_tmx-1.1.0/openbb_tmx/models/index_snapshots.py
--rw-r--r--   0        0        0     6105 2024-04-23 10:22:39.795263 openbb_tmx-1.1.0/openbb_tmx/models/insider_trading.py
--rw-r--r--   0        0        0     3293 2024-04-08 12:02:16.693188 openbb_tmx-1.1.0/openbb_tmx/models/options_chains.py
--rw-r--r--   0        0        0     5996 2024-05-10 10:40:27.303285 openbb_tmx-1.1.0/openbb_tmx/models/price_target_consensus.py
--rw-r--r--   0        0        0     5132 2024-05-09 13:34:29.362361 openbb_tmx-1.1.0/openbb_tmx/models/treasury_prices.py
--rw-r--r--   0        0        0        0 2024-04-08 12:02:16.693325 openbb_tmx-1.1.0/openbb_tmx/py.typed
--rw-r--r--   0        0        0       26 2024-04-23 10:22:39.795468 openbb_tmx-1.1.0/openbb_tmx/utils/__init__.py
--rw-r--r--   0        0        0    10195 2024-04-08 12:02:16.693456 openbb_tmx-1.1.0/openbb_tmx/utils/gql.py
--rw-r--r--   0        0        0    38670 2024-04-23 10:22:39.795669 openbb_tmx-1.1.0/openbb_tmx/utils/helpers.py
--rw-r--r--   0        0        0      662 2024-05-15 16:07:21.293855 openbb_tmx-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 openbb_tmx-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2637 2024-05-22 11:48:40.547330 openbb_tmx-1.1.1/README.md
+-rw-r--r--   0        0        0     3325 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/__init__.py
+-rw-r--r--   0        0        0     4695 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/available_indices.py
+-rw-r--r--   0        0        0     6306 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/bond_prices.py
+-rw-r--r--   0        0        0     5166 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/calendar_earnings.py
+-rw-r--r--   0        0        0     5814 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/company_filings.py
+-rw-r--r--   0        0        0     4653 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/company_news.py
+-rw-r--r--   0        0        0     8853 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/equity_historical.py
+-rw-r--r--   0        0        0     5461 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/equity_profile.py
+-rw-r--r--   0        0        0    12481 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/equity_quote.py
+-rw-r--r--   0        0        0     2223 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/equity_search.py
+-rw-r--r--   0        0        0     3644 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/etf_countries.py
+-rw-r--r--   0        0        0     5093 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/etf_holdings.py
+-rw-r--r--   0        0        0     8463 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/etf_info.py
+-rw-r--r--   0        0        0     9711 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/etf_search.py
+-rw-r--r--   0        0        0     2633 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/etf_sectors.py
+-rw-r--r--   0        0        0     4479 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/gainers.py
+-rw-r--r--   0        0        0     3584 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/historical_dividends.py
+-rw-r--r--   0        0        0     3098 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/index_constituents.py
+-rw-r--r--   0        0        0     2837 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/index_sectors.py
+-rw-r--r--   0        0        0    10349 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/index_snapshots.py
+-rw-r--r--   0        0        0     6105 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/insider_trading.py
+-rw-r--r--   0        0        0     3293 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/models/options_chains.py
+-rw-r--r--   0        0        0     5996 2024-05-15 09:21:56.101885 openbb_tmx-1.1.1/openbb_tmx/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5132 2024-05-14 16:57:23.742033 openbb_tmx-1.1.1/openbb_tmx/models/treasury_prices.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/py.typed
+-rw-r--r--   0        0        0       26 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/utils/__init__.py
+-rw-r--r--   0        0        0    10195 2024-05-14 16:56:42.153866 openbb_tmx-1.1.1/openbb_tmx/utils/gql.py
+-rw-r--r--   0        0        0    38691 2024-05-22 11:48:40.547330 openbb_tmx-1.1.1/openbb_tmx/utils/helpers.py
+-rw-r--r--   0        0        0      662 2024-05-22 13:56:05.199591 openbb_tmx-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     3578 1970-01-01 00:00:00.000000 openbb_tmx-1.1.1/PKG-INFO
```

### Comparing `openbb_tmx-1.1.0/README.md` & `openbb_tmx-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/__init__.py` & `openbb_tmx-1.1.1/openbb_tmx/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/available_indices.py` & `openbb_tmx-1.1.1/openbb_tmx/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/bond_prices.py` & `openbb_tmx-1.1.1/openbb_tmx/models/bond_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/calendar_earnings.py` & `openbb_tmx-1.1.1/openbb_tmx/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/company_filings.py` & `openbb_tmx-1.1.1/openbb_tmx/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/company_news.py` & `openbb_tmx-1.1.1/openbb_tmx/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/equity_historical.py` & `openbb_tmx-1.1.1/openbb_tmx/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/equity_profile.py` & `openbb_tmx-1.1.1/openbb_tmx/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/equity_quote.py` & `openbb_tmx-1.1.1/openbb_tmx/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/equity_search.py` & `openbb_tmx-1.1.1/openbb_tmx/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/etf_countries.py` & `openbb_tmx-1.1.1/openbb_tmx/models/etf_countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/etf_holdings.py` & `openbb_tmx-1.1.1/openbb_tmx/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/etf_info.py` & `openbb_tmx-1.1.1/openbb_tmx/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/etf_search.py` & `openbb_tmx-1.1.1/openbb_tmx/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/etf_sectors.py` & `openbb_tmx-1.1.1/openbb_tmx/models/etf_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/gainers.py` & `openbb_tmx-1.1.1/openbb_tmx/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/historical_dividends.py` & `openbb_tmx-1.1.1/openbb_tmx/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/index_constituents.py` & `openbb_tmx-1.1.1/openbb_tmx/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/index_sectors.py` & `openbb_tmx-1.1.1/openbb_tmx/models/index_sectors.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/index_snapshots.py` & `openbb_tmx-1.1.1/openbb_tmx/models/index_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/insider_trading.py` & `openbb_tmx-1.1.1/openbb_tmx/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/options_chains.py` & `openbb_tmx-1.1.1/openbb_tmx/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/price_target_consensus.py` & `openbb_tmx-1.1.1/openbb_tmx/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/models/treasury_prices.py` & `openbb_tmx-1.1.1/openbb_tmx/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/utils/gql.py` & `openbb_tmx-1.1.1/openbb_tmx/utils/gql.py`

 * *Files identical despite different names*

### Comparing `openbb_tmx-1.1.0/openbb_tmx/utils/helpers.py` & `openbb_tmx-1.1.1/openbb_tmx/utils/helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -277,14 +277,15 @@
 async def get_data_from_url(
     url: str,
     use_cache: bool = True,
     backend: Optional[SQLiteBackend] = None,
     **kwargs: Any,
 ) -> Any:
     """Make an asynchronous HTTP request to a static file."""
+    data: Any = None
     if use_cache is True:
         async with CachedSession(cache=backend) as cached_session:
             try:
                 response = await cached_session.get(url, **kwargs)
                 data = await response_callback(response, None)
             finally:
                 await cached_session.close()
```

### Comparing `openbb_tmx-1.1.0/pyproject.toml` & `openbb_tmx-1.1.1/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [tool.poetry]
 name = "openbb-tmx"
-version = "1.1.0"
+version = "1.1.1"
 description = "Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API."
 authors = ["OpenBB <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_tmx" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp-client-cache = "^0.11.0"
 aiosqlite = "^0.20.0"
 random-user-agent = "^1.0.1"
 exchange-calendars = "^4.2.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tmx = "openbb_tmx:tmx_provider"
```

### Comparing `openbb_tmx-1.1.0/PKG-INFO` & `openbb_tmx-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openbb-tmx
-Version: 1.1.0
+Version: 1.1.1
 Summary: Unofficial TMX data provider extension for the OpenBB Platform - Public Canadian markets data for Python and Fast API.
 License: AGPL-3.0-only
 Author: OpenBB
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp-client-cache (>=0.11.0,<0.12.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
 Requires-Dist: exchange-calendars (>=4.2.8,<5.0.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB TMX Provider
 
 This extension integrates the [TMX](https://www.tmx.com) data provider into the OpenBB Platform.
```

