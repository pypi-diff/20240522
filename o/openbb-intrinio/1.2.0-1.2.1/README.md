# Comparing `tmp/openbb_intrinio-1.2.0.tar.gz` & `tmp/openbb_intrinio-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_intrinio-1.2.0.tar", max compression
+gzip compressed data, was "openbb_intrinio-1.2.1.tar", max compression
```

## Comparing `openbb_intrinio-1.2.0.tar` & `openbb_intrinio-1.2.1.tar`

### file list

```diff
@@ -1,46 +1,47 @@
--rw-r--r--   0        0        0      308 2024-05-15 14:25:27.915403 openbb_intrinio-1.2.0/README.md
--rw-r--r--   0        0        0     5944 2024-05-14 15:30:05.616440 openbb_intrinio-1.2.0/openbb_intrinio/__init__.py
--rw-r--r--   0        0        0       33 2024-02-29 11:03:36.874926 openbb_intrinio-1.2.0/openbb_intrinio/models/__init__.py
--rw-r--r--   0        0        0    22763 2024-05-09 13:34:29.221940 openbb_intrinio-1.2.0/openbb_intrinio/models/balance_sheet.py
--rw-r--r--   0        0        0     7533 2024-04-08 12:02:16.650967 openbb_intrinio-1.2.0/openbb_intrinio/models/calendar_ipo.py
--rw-r--r--   0        0        0    14753 2024-04-08 12:02:16.651055 openbb_intrinio-1.2.0/openbb_intrinio/models/cash_flow.py
--rw-r--r--   0        0        0     3603 2024-04-02 11:35:59.478049 openbb_intrinio-1.2.0/openbb_intrinio/models/company_filings.py
--rw-r--r--   0        0        0     9166 2024-05-10 10:40:27.297354 openbb_intrinio-1.2.0/openbb_intrinio/models/company_news.py
--rw-r--r--   0        0        0     2939 2024-05-09 15:04:29.071560 openbb_intrinio-1.2.0/openbb_intrinio/models/currency_pairs.py
--rw-r--r--   0        0        0     9171 2024-05-09 15:04:29.071762 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_historical.py
--rw-r--r--   0        0        0     2382 2024-05-10 10:40:27.297486 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_info.py
--rw-r--r--   0        0        0     4980 2024-05-10 10:40:27.297645 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_quote.py
--rw-r--r--   0        0        0     2975 2024-04-02 11:35:59.478839 openbb_intrinio-1.2.0/openbb_intrinio/models/equity_search.py
--rw-r--r--   0        0        0     7327 2024-04-23 10:22:39.671958 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_holdings.py
--rw-r--r--   0        0        0    29033 2024-05-10 10:40:27.297866 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_info.py
--rw-r--r--   0        0        0     8343 2024-05-10 10:40:27.298055 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_price_performance.py
--rw-r--r--   0        0        0     4669 2024-04-08 12:02:16.651932 openbb_intrinio-1.2.0/openbb_intrinio/models/etf_search.py
--rw-r--r--   0        0        0     2805 2024-04-02 11:35:59.479335 openbb_intrinio-1.2.0/openbb_intrinio/models/financial_attributes.py
--rw-r--r--   0        0        0    12104 2024-04-02 11:35:59.479441 openbb_intrinio-1.2.0/openbb_intrinio/models/financial_ratios.py
--rw-r--r--   0        0        0     8423 2024-05-10 10:40:27.298213 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_eps_estimates.py
--rw-r--r--   0        0        0     5005 2024-05-14 15:30:05.616608 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_pe_estimates.py
--rw-r--r--   0        0        0     9700 2024-05-10 10:40:27.298372 openbb_intrinio-1.2.0/openbb_intrinio/models/forward_sales_estimates.py
--rw-r--r--   0        0        0     3716 2024-04-02 11:35:59.479494 openbb_intrinio-1.2.0/openbb_intrinio/models/fred_series.py
--rw-r--r--   0        0        0     5102 2024-05-10 10:40:27.298529 openbb_intrinio-1.2.0/openbb_intrinio/models/historical_attributes.py
--rw-r--r--   0        0        0     3651 2024-04-08 12:02:16.652255 openbb_intrinio-1.2.0/openbb_intrinio/models/historical_dividends.py
--rw-r--r--   0        0        0    21817 2024-04-08 12:02:16.652375 openbb_intrinio-1.2.0/openbb_intrinio/models/income_statement.py
--rw-r--r--   0        0        0     3682 2024-05-10 10:40:27.298668 openbb_intrinio-1.2.0/openbb_intrinio/models/index_historical.py
--rw-r--r--   0        0        0     6561 2024-04-08 12:02:16.652664 openbb_intrinio-1.2.0/openbb_intrinio/models/insider_trading.py
--rw-r--r--   0        0        0     4374 2024-04-02 11:35:59.480067 openbb_intrinio-1.2.0/openbb_intrinio/models/institutional_ownership.py
--rw-r--r--   0        0        0    12545 2024-05-10 10:40:27.298912 openbb_intrinio-1.2.0/openbb_intrinio/models/key_metrics.py
--rw-r--r--   0        0        0     3369 2024-05-10 10:40:27.299106 openbb_intrinio-1.2.0/openbb_intrinio/models/latest_attributes.py
--rw-r--r--   0        0        0     3120 2024-04-02 11:35:59.480302 openbb_intrinio-1.2.0/openbb_intrinio/models/market_indices.py
--rw-r--r--   0        0        0     8901 2024-04-23 10:22:39.672601 openbb_intrinio-1.2.0/openbb_intrinio/models/market_snapshots.py
--rw-r--r--   0        0        0     4745 2024-04-08 12:02:16.653091 openbb_intrinio-1.2.0/openbb_intrinio/models/options_chains.py
--rw-r--r--   0        0        0    11285 2024-04-08 12:02:16.653227 openbb_intrinio-1.2.0/openbb_intrinio/models/options_unusual.py
--rw-r--r--   0        0        0     6519 2024-05-10 10:40:27.299281 openbb_intrinio-1.2.0/openbb_intrinio/models/price_target_consensus.py
--rw-r--r--   0        0        0     5359 2024-04-02 11:35:59.480930 openbb_intrinio-1.2.0/openbb_intrinio/models/reported_financials.py
--rw-r--r--   0        0        0     2399 2024-04-02 11:35:59.481011 openbb_intrinio-1.2.0/openbb_intrinio/models/search_attributes.py
--rw-r--r--   0        0        0     3113 2024-04-02 11:35:59.481085 openbb_intrinio-1.2.0/openbb_intrinio/models/share_statistics.py
--rw-r--r--   0        0        0     8655 2024-05-09 13:34:29.227363 openbb_intrinio-1.2.0/openbb_intrinio/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.876946 openbb_intrinio-1.2.0/openbb_intrinio/py.typed
--rw-r--r--   0        0        0       32 2024-02-29 11:03:36.877031 openbb_intrinio-1.2.0/openbb_intrinio/utils/__init__.py
--rw-r--r--   0        0        0     4006 2024-04-23 10:22:39.673143 openbb_intrinio-1.2.0/openbb_intrinio/utils/helpers.py
--rw-r--r--   0        0        0     5352 2024-04-08 12:02:16.653631 openbb_intrinio-1.2.0/openbb_intrinio/utils/references.py
--rw-r--r--   0        0        0      515 2024-05-15 16:07:06.280254 openbb_intrinio-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_intrinio-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      308 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/README.md
+-rw-r--r--   0        0        0     6124 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/__init__.py
+-rw-r--r--   0        0        0       33 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/__init__.py
+-rw-r--r--   0        0        0    22843 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/balance_sheet.py
+-rw-r--r--   0        0        0     7533 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/calendar_ipo.py
+-rw-r--r--   0        0        0    14753 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/cash_flow.py
+-rw-r--r--   0        0        0     3603 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/company_filings.py
+-rw-r--r--   0        0        0    10042 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/company_news.py
+-rw-r--r--   0        0        0     2939 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/currency_pairs.py
+-rw-r--r--   0        0        0     9171 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/equity_historical.py
+-rw-r--r--   0        0        0     2382 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/equity_info.py
+-rw-r--r--   0        0        0     4965 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/equity_quote.py
+-rw-r--r--   0        0        0     2975 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/equity_search.py
+-rw-r--r--   0        0        0     7327 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/etf_holdings.py
+-rw-r--r--   0        0        0    29033 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/etf_info.py
+-rw-r--r--   0        0        0     8343 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/etf_price_performance.py
+-rw-r--r--   0        0        0     4669 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/etf_search.py
+-rw-r--r--   0        0        0     2805 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/financial_attributes.py
+-rw-r--r--   0        0        0    12104 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/financial_ratios.py
+-rw-r--r--   0        0        0     6798 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/forward_ebitda_estimates.py
+-rw-r--r--   0        0        0     8423 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/forward_eps_estimates.py
+-rw-r--r--   0        0        0     5005 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/forward_pe_estimates.py
+-rw-r--r--   0        0        0     9700 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/forward_sales_estimates.py
+-rw-r--r--   0        0        0     3716 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/fred_series.py
+-rw-r--r--   0        0        0     5102 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/historical_attributes.py
+-rw-r--r--   0        0        0     3651 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/historical_dividends.py
+-rw-r--r--   0        0        0    21817 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/income_statement.py
+-rw-r--r--   0        0        0     3682 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/index_historical.py
+-rw-r--r--   0        0        0     6561 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/insider_trading.py
+-rw-r--r--   0        0        0     4374 2024-05-14 16:56:41.905865 openbb_intrinio-1.2.1/openbb_intrinio/models/institutional_ownership.py
+-rw-r--r--   0        0        0    12545 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/key_metrics.py
+-rw-r--r--   0        0        0     3369 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/latest_attributes.py
+-rw-r--r--   0        0        0     3120 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/market_indices.py
+-rw-r--r--   0        0        0     8901 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/market_snapshots.py
+-rw-r--r--   0        0        0     4745 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/options_chains.py
+-rw-r--r--   0        0        0    11285 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/options_unusual.py
+-rw-r--r--   0        0        0     6519 2024-05-15 09:21:56.081885 openbb_intrinio-1.2.1/openbb_intrinio/models/price_target_consensus.py
+-rw-r--r--   0        0        0     5359 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/reported_financials.py
+-rw-r--r--   0        0        0     2399 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/search_attributes.py
+-rw-r--r--   0        0        0     3113 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/models/share_statistics.py
+-rw-r--r--   0        0        0     9355 2024-05-22 11:48:40.539330 openbb_intrinio-1.2.1/openbb_intrinio/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/py.typed
+-rw-r--r--   0        0        0       32 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/utils/__init__.py
+-rw-r--r--   0        0        0     4006 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/utils/helpers.py
+-rw-r--r--   0        0        0     5352 2024-05-14 16:56:41.909865 openbb_intrinio-1.2.1/openbb_intrinio/utils/references.py
+-rw-r--r--   0        0        0      515 2024-05-22 13:57:26.391860 openbb_intrinio-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1017 1970-01-01 00:00:00.000000 openbb_intrinio-1.2.1/PKG-INFO
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/__init__.py` & `openbb_intrinio-1.2.1/openbb_intrinio/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 from openbb_intrinio.models.etf_holdings import IntrinioEtfHoldingsFetcher
 from openbb_intrinio.models.etf_info import IntrinioEtfInfoFetcher
 from openbb_intrinio.models.etf_price_performance import (
     IntrinioEtfPricePerformanceFetcher,
 )
 from openbb_intrinio.models.etf_search import IntrinioEtfSearchFetcher
 from openbb_intrinio.models.financial_ratios import IntrinioFinancialRatiosFetcher
+from openbb_intrinio.models.forward_ebitda_estimates import (
+    IntrinioForwardEbitdaEstimatesFetcher,
+)
 from openbb_intrinio.models.forward_eps_estimates import (
     IntrinioForwardEpsEstimatesFetcher,
 )
 from openbb_intrinio.models.forward_pe_estimates import (
     IntrinioForwardPeEstimatesFetcher,
 )
 from openbb_intrinio.models.forward_sales_estimates import (
@@ -75,14 +78,15 @@
         "EquitySearch": IntrinioEquitySearchFetcher,
         "EtfHistorical": IntrinioEquityHistoricalFetcher,
         "EtfHoldings": IntrinioEtfHoldingsFetcher,
         "EtfInfo": IntrinioEtfInfoFetcher,
         "EtfPricePerformance": IntrinioEtfPricePerformanceFetcher,
         "EtfSearch": IntrinioEtfSearchFetcher,
         "FinancialRatios": IntrinioFinancialRatiosFetcher,
+        "ForwardEbitdaEstimates": IntrinioForwardEbitdaEstimatesFetcher,
         "ForwardEpsEstimates": IntrinioForwardEpsEstimatesFetcher,
         "ForwardPeEstimates": IntrinioForwardPeEstimatesFetcher,
         "ForwardSalesEstimates": IntrinioForwardSalesEstimatesFetcher,
         "FredSeries": IntrinioFredSeriesFetcher,
         "HistoricalAttributes": IntrinioHistoricalAttributesFetcher,
         "HistoricalDividends": IntrinioHistoricalDividendsFetcher,
         "IncomeStatement": IntrinioIncomeStatementFetcher,
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/balance_sheet.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/balance_sheet.py`

 * *Files 1% similar despite different names*

```diff
@@ -441,20 +441,20 @@
             f"{item['fiscal_year']}-{item['fiscal_period']}"
             for item in fundamentals_data
         ]
         fiscal_periods = fiscal_periods[: query.limit]
 
         async def callback(response: ClientResponse, _: Any) -> Dict:
             """Return the response."""
-            statement_data = await response.json()
+            statement_data = await response.json()  # type: ignore
             return {
-                "period_ending": statement_data["fundamental"]["end_date"],
-                "fiscal_year": statement_data["fundamental"]["fiscal_year"],
-                "fiscal_period": statement_data["fundamental"]["fiscal_period"],
-                "financials": statement_data["standardized_financials"],
+                "period_ending": statement_data["fundamental"]["end_date"],  # type: ignore
+                "fiscal_year": statement_data["fundamental"]["fiscal_year"],  # type: ignore
+                "fiscal_period": statement_data["fundamental"]["fiscal_period"],  # type: ignore
+                "financials": statement_data["standardized_financials"],  # type: ignore
             }
 
         urls = [
             f"{base_url}/fundamentals/{query.symbol}-{statement_code}-{p}/standardized_financials?api_key={api_key}"
             for p in fiscal_periods
         ]
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/calendar_ipo.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/calendar_ipo.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/cash_flow.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/cash_flow.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/company_filings.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/company_filings.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/company_news.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/company_news.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Intrinio Company News Model."""
 
 import asyncio
-from datetime import datetime
+from datetime import datetime, timedelta
 from typing import Any, Dict, List, Literal, Optional, Union
+from warnings import warn
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.company_news import (
     CompanyNewsData,
     CompanyNewsQueryParams,
 )
 from openbb_core.provider.utils.errors import EmptyDataError
@@ -62,21 +63,25 @@
     is_spam: Optional[bool] = Field(
         default=None,
         description="Filter whether it is marked as spam or not."
         + " Unsupported for yahoo source.",
     )
     business_relevance_greater_than: Optional[float] = Field(
         default=None,
+        ge=0,
+        le=1,
         description="News stories will have a business relevance score more than this value."
-        + " Unsupported for yahoo source.",
+        + " Unsupported for yahoo source. Value is a decimal between 0 and 1.",
     )
     business_relevance_less_than: Optional[float] = Field(
         default=None,
+        ge=0,
+        le=1,
         description="News stories will have a business relevance score less than this value."
-        + " Unsupported for yahoo source.",
+        + " Unsupported for yahoo source. Value is a decimal between 0 and 1.",
     )
 
 
 class IntrinioCompanyNewsData(CompanyNewsData):
     """Intrinio Company News Data."""
 
     __alias_dict__ = {
@@ -160,15 +165,26 @@
     ]
 ):
     """Transform the query, extract and transform the data from the Intrinio endpoints."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> IntrinioCompanyNewsQueryParams:
         """Transform the query params."""
-        return IntrinioCompanyNewsQueryParams(**params)
+        transformed_params = params
+        if not transformed_params.get("start_date"):
+            transformed_params["start_date"] = (
+                datetime.now() - timedelta(days=365)
+            ).date()
+        if not transformed_params.get("end_date"):
+            transformed_params["end_date"] = (datetime.now() + timedelta(days=1)).date()
+        if transformed_params["start_date"] == transformed_params["end_date"]:
+            transformed_params["end_date"] = (
+                transformed_params["end_date"] + timedelta(days=1)
+            ).date()
+        return IntrinioCompanyNewsQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
         query: IntrinioCompanyNewsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
@@ -195,45 +211,51 @@
             data = []
             data.extend([{"symbol": symbol, **d} for d in _data])
             articles = len(data)
             next_page = result.get("next_page")
             # query.limit can be None...
             limit = query.limit or 2500
             while next_page and limit > articles:
-                url = f"{base_url}/{symbol}/news?{query_str}&api_key={api_key}&next_page={next_page}"
+                url = (
+                    f"{base_url}/{symbol}/news?{query_str}"
+                    + f"&page_size={query.limit}&api_key={api_key}&next_page={next_page}"
+                )
                 result = await get_data(url, session=session, **kwargs)
                 _data = result.get("news", [])
                 if _data:
                     data.extend([{"symbol": symbol, **d} for d in _data])
                     articles = len(data)
                 next_page = result.get("next_page")
-            # Remove duplicates based on URL
             return data
 
         seen = set()
 
         async def get_one(symbol):
             """Get the data for one symbol."""
-            # TODO: Change page_size to a more appropriate value when Intrinio fixes the bug in this param.
-            url = f"{base_url}/{symbol}/news?{query_str}&page_size=99&api_key={api_key}"
+            url = f"{base_url}/{symbol}/news?{query_str}&page_size={query.limit}&api_key={api_key}"
             data = await amake_request(url, response_callback=callback, **kwargs)
+            if not data:
+                warn(f"No data found for: {symbol}")
             if data:
                 data = [x for x in data if not (x["url"] in seen or seen.add(x["url"]))]  # type: ignore
                 news.extend(
                     sorted(data, key=lambda x: x["publication_date"], reverse=True)[
                         : query.limit
                     ]
                 )
 
         tasks = [get_one(symbol) for symbol in symbols]
 
         await asyncio.gather(*tasks)
 
         if not news:
-            raise EmptyDataError("Error: The request was returned as empty.")
+            raise EmptyDataError(
+                "Error: The request was returned as empty."
+                + " Try adjusting the requested date ranges, if applicable."
+            )
 
         return news
 
     # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: IntrinioCompanyNewsQueryParams, data: List[Dict], **kwargs: Any
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/currency_pairs.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/currency_pairs.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_historical.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_info.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/equity_info.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_quote.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/equity_quote.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,15 +84,15 @@
         return v if v else None
 
     @field_validator("exchange", "market_center", mode="before", check_fields=False)
     @classmethod
     def validate_listing_venue(cls, v):
         """Validate listing venue and remove empty strings."""
         if v:
-            return VENUES[v] if v in VENUES else v
+            return VENUES.get(v, v)
         return None
 
 
 class IntrinioEquityQuoteFetcher(
     Fetcher[
         IntrinioEquityQuoteQueryParams,
         List[IntrinioEquityQuoteData],
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/equity_search.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_holdings.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/etf_holdings.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_info.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/etf_info.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_price_performance.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/etf_price_performance.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/etf_search.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/etf_search.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/financial_attributes.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/financial_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/financial_ratios.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/financial_ratios.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/forward_eps_estimates.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/forward_eps_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/forward_pe_estimates.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/forward_pe_estimates.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,26 +36,26 @@
         "year1": "forward_pe_year1",
         "year2": "forward_pe_year2",
         "year3": "forward_pe_year3",
         "year4": "forward_pe_year4",
         "year5": "forward_pe_year5",
         "peg_ratio_year1": "forward_peg_ratio_year1",
         "eps_ttm": "latest_ttm_eps",
-        "last_udpated": "updated_date",
+        "last_updated": "updated_date",
     }
 
     peg_ratio_year1: Optional[float] = Field(
         default=None,
         description="Estimated Forward PEG ratio for the next fiscal year.",
     )
     eps_ttm: Optional[float] = Field(
         default=None,
         description="The latest trailing twelve months earnings per share.",
     )
-    last_udpated: Optional[dateType] = Field(
+    last_updated: Optional[dateType] = Field(
         default=None,
         description="The date the data was last updated.",
     )
 
 
 class IntrinioForwardPeEstimatesFetcher(
     Fetcher[IntrinioForwardPeEstimatesQueryParams, List[IntrinioForwardPeEstimatesData]]
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/forward_sales_estimates.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/forward_sales_estimates.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/fred_series.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/fred_series.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/historical_attributes.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/historical_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/historical_dividends.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/income_statement.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/income_statement.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/index_historical.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/insider_trading.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/insider_trading.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/institutional_ownership.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/institutional_ownership.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/key_metrics.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/key_metrics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/latest_attributes.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/latest_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/market_indices.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/market_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/market_snapshots.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/market_snapshots.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/options_chains.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/options_unusual.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/options_unusual.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/price_target_consensus.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/price_target_consensus.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/reported_financials.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/reported_financials.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/search_attributes.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/search_attributes.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/share_statistics.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/share_statistics.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/models/world_news.py` & `openbb_intrinio-1.2.1/openbb_intrinio/models/world_news.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 """Intrinio World News Model."""
 
-from datetime import datetime
+# pylint: disable=unused-argument
+
+from datetime import datetime, timedelta
 from typing import Any, Dict, List, Literal, Optional, Union
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.world_news import (
     WorldNewsData,
     WorldNewsQueryParams,
 )
@@ -56,21 +58,25 @@
     is_spam: Optional[bool] = Field(
         default=None,
         description="Filter whether it is marked as spam or not."
         + " Unsupported for yahoo source.",
     )
     business_relevance_greater_than: Optional[float] = Field(
         default=None,
+        ge=0,
+        le=1,
         description="News stories will have a business relevance score more than this value."
-        + " Unsupported for yahoo source.",
+        + " Unsupported for yahoo source. Value is a decimal between 0 and 1.",
     )
     business_relevance_less_than: Optional[float] = Field(
         default=None,
+        ge=0,
+        le=1,
         description="News stories will have a business relevance score less than this value."
-        + " Unsupported for yahoo source.",
+        + " Unsupported for yahoo source. Value is a decimal between 0 and 1.",
     )
 
 
 class IntrinioWorldNewsData(WorldNewsData):
     """Intrinio World News Data."""
 
     __alias_dict__ = {
@@ -157,15 +163,24 @@
     ]
 ):
     """Intrinio World News Fetcher."""
 
     @staticmethod
     def transform_query(params: Dict[str, Any]) -> IntrinioWorldNewsQueryParams:
         """Transform the query params."""
-        return IntrinioWorldNewsQueryParams(**params)
+        transformed_params = params
+        if not transformed_params.get("start_date"):
+            transformed_params["start_date"] = datetime.now().date()
+        if not transformed_params.get("end_date"):
+            transformed_params["end_date"] = (datetime.now() + timedelta(days=1)).date()
+        if transformed_params["start_date"] == transformed_params["end_date"]:
+            transformed_params["end_date"] = (
+                transformed_params["end_date"] + timedelta(days=1)
+            ).date()
+        return IntrinioWorldNewsQueryParams(**transformed_params)
 
     @staticmethod
     async def aextract_data(
         query: IntrinioWorldNewsQueryParams,
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
@@ -175,31 +190,29 @@
         base_url = "https://api-v2.intrinio.com/companies"
         ignore = (
             ["symbol", "page_size", "is_spam"]
             if not query.source or query.source == "yahoo"
             else ["symbol", "page_size"]
         )
         query_str = get_querystring(query.model_dump(by_alias=True), ignore)
-        # TODO: Change page_size to a more appropriate value when Intrinio fixes the bug in this param.
-        url = f"{base_url}/news?{query_str}&page_size=99&api_key={api_key}"
-
+        url = f"{base_url}/news?{query_str}&page_size={query.limit}&api_key={api_key}"
         seen = set()
 
         async def callback(response, session):
             """Response callback."""
             result = await response.json()
             _data = result.get("news", [])
             data = []
             data.extend(
                 [x for x in _data if not (x["url"] in seen or seen.add(x["url"]))]  # type: ignore
             )
             articles = len(data)
             next_page = result.get("next_page")
             while next_page and articles < query.limit:
-                url = f"{base_url}/news?{query_str}&page_size=99&api_key={api_key}&next_page={next_page}"
+                url = f"{base_url}/news?{query_str}&page_size={query.limit}&api_key={api_key}&next_page={next_page}"
                 result = await get_data(url, session=session, **kwargs)
                 _data = result.get("news", [])
                 if _data:
                     # Remove duplicates based on URL
                     data.extend(
                         [
                             x
@@ -209,24 +222,26 @@
                     )
                     articles = len(data)
                 next_page = result.get("next_page")
             return sorted(data, key=lambda x: x["publication_date"], reverse=True)[
                 : query.limit
             ]
 
-        return await amake_request(url, response_callback=callback, **kwargs)
+        return await amake_request(url, response_callback=callback, **kwargs)  # type: ignore
 
-    # pylint: disable=unused-argument
     @staticmethod
     def transform_data(
         query: IntrinioWorldNewsQueryParams, data: List[Dict], **kwargs: Any
     ) -> List[IntrinioWorldNewsData]:
         """Return the transformed data."""
         if not data:
-            raise EmptyDataError("Error: The request was returned as empty.")
+            raise EmptyDataError(
+                "Error: The request was returned as empty."
+                + " Try adjusting the requested date ranges, if applicable."
+            )
         results: List[IntrinioWorldNewsData] = []
         for item in data:
             body = item.get("body", {})
             if not body:
                 item["text"] = item.pop("summary")
             if body:
                 _ = item.pop("body")
```

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/utils/helpers.py` & `openbb_intrinio-1.2.1/openbb_intrinio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/openbb_intrinio/utils/references.py` & `openbb_intrinio-1.2.1/openbb_intrinio/utils/references.py`

 * *Files identical despite different names*

### Comparing `openbb_intrinio-1.2.0/pyproject.toml` & `openbb_intrinio-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "openbb-intrinio"
-version = "1.2.0"
+version = "1.2.1"
 description = "Intrinio extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_intrinio" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests-cache = "^1.1.0"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 intrinio = "openbb_intrinio:intrinio_provider"
```

### Comparing `openbb_intrinio-1.2.0/PKG-INFO` & `openbb_intrinio-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-intrinio
-Version: 1.2.0
+Version: 1.2.1
 Summary: Intrinio extension for OpenBB
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
 
 # OpenBB Intrinio Provider
 
 This extension integrates the [Intrinio](https://intrinio.com/) data provider into the OpenBB Platform.
```

