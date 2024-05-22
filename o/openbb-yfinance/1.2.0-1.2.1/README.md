# Comparing `tmp/openbb_yfinance-1.2.0.tar.gz` & `tmp/openbb_yfinance-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_yfinance-1.2.0.tar", max compression
+gzip compressed data, was "openbb_yfinance-1.2.1.tar", max compression
```

## Comparing `openbb_yfinance-1.2.0.tar` & `openbb_yfinance-1.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0      323 2024-05-15 14:24:24.418114 openbb_yfinance-1.2.0/README.md
--rw-r--r--   0        0        0     4166 2024-05-14 15:30:05.622090 openbb_yfinance-1.2.0/openbb_yfinance/__init__.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.979066 openbb_yfinance-1.2.0/openbb_yfinance/models/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-23 10:22:39.801074 openbb_yfinance-1.2.0/openbb_yfinance/models/active.py
--rw-r--r--   0        0        0     3071 2024-04-08 12:02:16.765334 openbb_yfinance-1.2.0/openbb_yfinance/models/aggressive_small_caps.py
--rw-r--r--   0        0        0     2036 2024-04-23 10:22:39.801195 openbb_yfinance-1.2.0/openbb_yfinance/models/available_indices.py
--rw-r--r--   0        0        0     3266 2024-04-08 12:02:16.765440 openbb_yfinance-1.2.0/openbb_yfinance/models/balance_sheet.py
--rw-r--r--   0        0        0     3296 2024-04-08 12:02:16.765519 openbb_yfinance-1.2.0/openbb_yfinance/models/cash_flow.py
--rw-r--r--   0        0        0     2869 2024-05-10 10:40:27.305123 openbb_yfinance-1.2.0/openbb_yfinance/models/company_news.py
--rw-r--r--   0        0        0     3456 2024-05-10 10:40:27.305369 openbb_yfinance-1.2.0/openbb_yfinance/models/crypto_historical.py
--rw-r--r--   0        0        0     3367 2024-05-10 10:40:27.305501 openbb_yfinance-1.2.0/openbb_yfinance/models/currency_historical.py
--rw-r--r--   0        0        0     6677 2024-05-10 10:40:27.305644 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_historical.py
--rw-r--r--   0        0        0     5868 2024-05-10 10:40:27.305756 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_profile.py
--rw-r--r--   0        0        0     3896 2024-05-10 10:40:27.305887 openbb_yfinance-1.2.0/openbb_yfinance/models/equity_quote.py
--rw-r--r--   0        0        0     2851 2024-04-02 11:35:59.651682 openbb_yfinance-1.2.0/openbb_yfinance/models/etf_historical.py
--rw-r--r--   0        0        0    10128 2024-05-10 10:40:27.306032 openbb_yfinance-1.2.0/openbb_yfinance/models/etf_info.py
--rw-r--r--   0        0        0     2255 2024-04-08 12:02:16.766367 openbb_yfinance-1.2.0/openbb_yfinance/models/futures_curve.py
--rw-r--r--   0        0        0     4717 2024-05-10 10:40:27.306188 openbb_yfinance-1.2.0/openbb_yfinance/models/futures_historical.py
--rw-r--r--   0        0        0     2984 2024-04-08 12:02:16.766529 openbb_yfinance-1.2.0/openbb_yfinance/models/gainers.py
--rw-r--r--   0        0        0     3119 2024-04-08 12:02:16.766617 openbb_yfinance-1.2.0/openbb_yfinance/models/growth_tech_equities.py
--rw-r--r--   0        0        0     2437 2024-04-08 12:02:16.766677 openbb_yfinance-1.2.0/openbb_yfinance/models/historical_dividends.py
--rw-r--r--   0        0        0     3412 2024-04-08 12:02:16.766770 openbb_yfinance-1.2.0/openbb_yfinance/models/income_statement.py
--rw-r--r--   0        0        0     4069 2024-05-10 10:40:27.306306 openbb_yfinance-1.2.0/openbb_yfinance/models/index_historical.py
--rw-r--r--   0        0        0     2379 2024-04-08 12:02:16.766930 openbb_yfinance-1.2.0/openbb_yfinance/models/key_executives.py
--rw-r--r--   0        0        0    10194 2024-05-10 10:40:27.306403 openbb_yfinance-1.2.0/openbb_yfinance/models/key_metrics.py
--rw-r--r--   0        0        0     2969 2024-04-08 12:02:16.767101 openbb_yfinance-1.2.0/openbb_yfinance/models/losers.py
--rw-r--r--   0        0        0     4682 2024-05-10 10:40:27.308919 openbb_yfinance-1.2.0/openbb_yfinance/models/market_indices.py
--rw-r--r--   0        0        0     4236 2024-05-10 10:40:27.309704 openbb_yfinance-1.2.0/openbb_yfinance/models/price_target_consensus.py
--rw-r--r--   0        0        0     6039 2024-05-10 10:40:27.309963 openbb_yfinance-1.2.0/openbb_yfinance/models/share_statistics.py
--rw-r--r--   0        0        0     3294 2024-04-08 12:02:16.767403 openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_growth_equities.py
--rw-r--r--   0        0        0     3127 2024-04-08 12:02:16.767490 openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_large_caps.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.980652 openbb_yfinance-1.2.0/openbb_yfinance/py.typed
--rw-r--r--   0        0        0       37 2024-02-29 11:03:36.980745 openbb_yfinance-1.2.0/openbb_yfinance/utils/__init__.py
--rw-r--r--   0        0        0     8379 2024-04-02 11:35:59.654237 openbb_yfinance-1.2.0/openbb_yfinance/utils/futures.csv
--rw-r--r--   0        0        0     6552 2024-04-23 10:22:39.801794 openbb_yfinance-1.2.0/openbb_yfinance/utils/helpers.py
--rw-r--r--   0        0        0    26952 2024-04-08 12:02:16.767762 openbb_yfinance-1.2.0/openbb_yfinance/utils/references.py
--rw-r--r--   0        0        0      510 2024-05-15 16:05:12.832912 openbb_yfinance-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 openbb_yfinance-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      323 2024-05-22 11:48:40.551330 openbb_yfinance-1.2.1/README.md
+-rw-r--r--   0        0        0     4166 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/active.py
+-rw-r--r--   0        0        0     3071 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/aggressive_small_caps.py
+-rw-r--r--   0        0        0     2036 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/available_indices.py
+-rw-r--r--   0        0        0     3266 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/balance_sheet.py
+-rw-r--r--   0        0        0     3296 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/cash_flow.py
+-rw-r--r--   0        0        0     2869 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/company_news.py
+-rw-r--r--   0        0        0     3456 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/crypto_historical.py
+-rw-r--r--   0        0        0     3367 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/currency_historical.py
+-rw-r--r--   0        0        0     6677 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/equity_historical.py
+-rw-r--r--   0        0        0     5868 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/equity_profile.py
+-rw-r--r--   0        0        0     3896 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/equity_quote.py
+-rw-r--r--   0        0        0     2851 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/etf_historical.py
+-rw-r--r--   0        0        0    10128 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/etf_info.py
+-rw-r--r--   0        0        0     2255 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/futures_curve.py
+-rw-r--r--   0        0        0     4717 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/futures_historical.py
+-rw-r--r--   0        0        0     2984 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/gainers.py
+-rw-r--r--   0        0        0     3119 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/growth_tech_equities.py
+-rw-r--r--   0        0        0     2437 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/historical_dividends.py
+-rw-r--r--   0        0        0     3412 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/income_statement.py
+-rw-r--r--   0        0        0     4069 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/index_historical.py
+-rw-r--r--   0        0        0     2379 2024-05-14 16:56:42.345866 openbb_yfinance-1.2.1/openbb_yfinance/models/key_executives.py
+-rw-r--r--   0        0        0    10194 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/key_metrics.py
+-rw-r--r--   0        0        0     2969 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/models/losers.py
+-rw-r--r--   0        0        0     4682 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/market_indices.py
+-rw-r--r--   0        0        0     4236 2024-05-15 09:21:56.109886 openbb_yfinance-1.2.1/openbb_yfinance/models/price_target_consensus.py
+-rw-r--r--   0        0        0     6039 2024-05-15 09:21:56.113885 openbb_yfinance-1.2.1/openbb_yfinance/models/share_statistics.py
+-rw-r--r--   0        0        0     3294 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/models/undervalued_growth_equities.py
+-rw-r--r--   0        0        0     3127 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/models/undervalued_large_caps.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/py.typed
+-rw-r--r--   0        0        0       37 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/utils/__init__.py
+-rw-r--r--   0        0        0     8379 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/utils/futures.csv
+-rw-r--r--   0        0        0     6552 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/utils/helpers.py
+-rw-r--r--   0        0        0    26952 2024-05-14 16:56:42.349866 openbb_yfinance-1.2.1/openbb_yfinance/utils/references.py
+-rw-r--r--   0        0        0      510 2024-05-22 13:57:09.439804 openbb_yfinance-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1027 1970-01-01 00:00:00.000000 openbb_yfinance-1.2.1/PKG-INFO
```

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/__init__.py` & `openbb_yfinance-1.2.1/openbb_yfinance/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/active.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/active.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/aggressive_small_caps.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/aggressive_small_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/available_indices.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/balance_sheet.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/balance_sheet.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/cash_flow.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/company_news.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/crypto_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/crypto_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/currency_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/currency_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_profile.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/equity_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/equity_quote.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/etf_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/etf_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/etf_info.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/futures_curve.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/futures_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/futures_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/gainers.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/gainers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/growth_tech_equities.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/growth_tech_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/historical_dividends.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/income_statement.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/index_historical.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/key_executives.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/key_executives.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/key_metrics.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/losers.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/losers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/market_indices.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/price_target_consensus.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/share_statistics.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_growth_equities.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/undervalued_growth_equities.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/models/undervalued_large_caps.py` & `openbb_yfinance-1.2.1/openbb_yfinance/models/undervalued_large_caps.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/utils/futures.csv` & `openbb_yfinance-1.2.1/openbb_yfinance/utils/futures.csv`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/utils/helpers.py` & `openbb_yfinance-1.2.1/openbb_yfinance/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/openbb_yfinance/utils/references.py` & `openbb_yfinance-1.2.1/openbb_yfinance/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_yfinance-1.2.0/PKG-INFO` & `openbb_yfinance-1.2.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-yfinance
-Version: 1.2.0
+Version: 1.2.1
 Summary: yfinance extension for OpenBB
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
 Requires-Dist: yfinance (>=0.2.27,<0.3.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Yahoo!Finance Provider
 
 This extension integrates the [Yahoo!Finance](https://finance.yahoo.com/) data provider into the OpenBB Platform.
```

