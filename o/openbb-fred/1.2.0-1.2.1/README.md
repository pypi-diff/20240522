# Comparing `tmp/openbb_fred-1.2.0.tar.gz` & `tmp/openbb_fred-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fred-1.2.0.tar", max compression
+gzip compressed data, was "openbb_fred-1.2.1.tar", max compression
```

## Comparing `openbb_fred-1.2.0.tar` & `openbb_fred-1.2.1.tar`

### file list

```diff
@@ -1,33 +1,35 @@
--rw-r--r--   0        0        0      317 2024-05-15 14:25:37.598005 openbb_fred-1.2.0/README.md
--rw-r--r--   0        0        0     4116 2024-05-14 15:30:05.615680 openbb_fred-1.2.0/openbb_fred/__init__.py
--rw-r--r--   0        0        0     2760 2024-02-29 11:03:36.866196 openbb_fred-1.2.0/openbb_fred/models/ameribor_rates.py
--rw-r--r--   0        0        0     2404 2024-02-29 11:03:36.866284 openbb_fred-1.2.0/openbb_fred/models/cp.py
--rw-r--r--   0        0        0     2953 2024-05-10 10:40:27.296801 openbb_fred-1.2.0/openbb_fred/models/cpi.py
--rw-r--r--   0        0        0     2764 2024-04-08 12:02:16.648313 openbb_fred-1.2.0/openbb_fred/models/dwpcr_rates.py
--rw-r--r--   0        0        0     2483 2024-02-29 11:03:36.866494 openbb_fred-1.2.0/openbb_fred/models/ecb_interest_rates.py
--rw-r--r--   0        0        0     2675 2024-02-29 11:03:36.866551 openbb_fred-1.2.0/openbb_fred/models/estr_rates.py
--rw-r--r--   0        0        0     2347 2024-02-29 11:03:36.866626 openbb_fred-1.2.0/openbb_fred/models/fed_projections.py
--rw-r--r--   0        0        0     2204 2024-02-29 11:03:36.866706 openbb_fred-1.2.0/openbb_fred/models/fed_rates.py
--rw-r--r--   0        0        0     2567 2024-02-29 11:03:36.866781 openbb_fred-1.2.0/openbb_fred/models/ffrmc.py
--rw-r--r--   0        0        0     3466 2024-04-08 12:02:16.648416 openbb_fred-1.2.0/openbb_fred/models/hqm.py
--rw-r--r--   0        0        0     3205 2024-02-29 11:03:36.866951 openbb_fred-1.2.0/openbb_fred/models/ice_bofa.py
--rw-r--r--   0        0        0     1794 2024-02-29 11:03:36.867021 openbb_fred-1.2.0/openbb_fred/models/iorb_rates.py
--rw-r--r--   0        0        0     3440 2024-02-29 11:03:36.867092 openbb_fred-1.2.0/openbb_fred/models/moody.py
--rw-r--r--   0        0        0     8525 2024-04-08 12:02:16.648506 openbb_fred-1.2.0/openbb_fred/models/regional.py
--rw-r--r--   0        0        0     6344 2024-05-09 13:34:29.220357 openbb_fred-1.2.0/openbb_fred/models/search.py
--rw-r--r--   0        0        0     6726 2024-05-10 10:40:27.296996 openbb_fred-1.2.0/openbb_fred/models/series.py
--rw-r--r--   0        0        0     2150 2024-02-29 11:03:36.867365 openbb_fred-1.2.0/openbb_fred/models/sofr_rates.py
--rw-r--r--   0        0        0     2382 2024-02-29 11:03:36.867442 openbb_fred-1.2.0/openbb_fred/models/sonia_rates.py
--rw-r--r--   0        0        0     2732 2024-05-10 10:40:27.297174 openbb_fred-1.2.0/openbb_fred/models/spot.py
--rw-r--r--   0        0        0     2225 2024-02-29 11:03:36.867578 openbb_fred-1.2.0/openbb_fred/models/tbffr.py
--rw-r--r--   0        0        0     2305 2024-02-29 11:03:36.867653 openbb_fred-1.2.0/openbb_fred/models/tmc.py
--rw-r--r--   0        0        0     3257 2024-02-29 11:03:36.867734 openbb_fred-1.2.0/openbb_fred/models/us_yield_curve.py
--rw-r--r--   0        0        0    58622 2024-02-29 11:03:36.867879 openbb_fred-1.2.0/openbb_fred/utils/commercial_paper.csv
--rw-r--r--   0        0        0   125899 2024-02-29 11:03:36.868080 openbb_fred-1.2.0/openbb_fred/utils/corporate_spot_rates.csv
--rw-r--r--   0        0        0    20963 2024-02-29 11:03:36.868229 openbb_fred-1.2.0/openbb_fred/utils/cpi.csv
--rw-r--r--   0        0        0     2395 2024-04-08 12:02:16.648982 openbb_fred-1.2.0/openbb_fred/utils/fred_base.py
--rw-r--r--   0        0        0     6113 2024-04-08 12:02:16.649089 openbb_fred-1.2.0/openbb_fred/utils/fred_helpers.py
--rw-r--r--   0        0        0    10219 2024-02-29 11:03:36.868524 openbb_fred-1.2.0/openbb_fred/utils/harmonized_cpi.csv
--rw-r--r--   0        0        0   227110 2024-02-29 11:03:36.868834 openbb_fred-1.2.0/openbb_fred/utils/ice_bofa_indices.csv
--rw-r--r--   0        0        0      465 2024-05-15 16:05:55.488948 openbb_fred-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 openbb_fred-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      317 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/README.md
+-rw-r--r--   0        0        0     4403 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/openbb_fred/__init__.py
+-rw-r--r--   0        0        0     2760 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/ameribor_rates.py
+-rw-r--r--   0        0        0     4383 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/openbb_fred/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2404 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/cp.py
+-rw-r--r--   0        0        0     2953 2024-05-15 09:21:56.077885 openbb_fred-1.2.1/openbb_fred/models/cpi.py
+-rw-r--r--   0        0        0     2764 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/dwpcr_rates.py
+-rw-r--r--   0        0        0     2483 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/ecb_interest_rates.py
+-rw-r--r--   0        0        0     2675 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/estr_rates.py
+-rw-r--r--   0        0        0     2347 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/fed_projections.py
+-rw-r--r--   0        0        0     2204 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/fed_rates.py
+-rw-r--r--   0        0        0     2567 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/ffrmc.py
+-rw-r--r--   0        0        0     3466 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/hqm.py
+-rw-r--r--   0        0        0     3205 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/ice_bofa.py
+-rw-r--r--   0        0        0     1794 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/iorb_rates.py
+-rw-r--r--   0        0        0     3440 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/moody.py
+-rw-r--r--   0        0        0     8525 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/regional.py
+-rw-r--r--   0        0        0     6356 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/openbb_fred/models/search.py
+-rw-r--r--   0        0        0     6726 2024-05-15 09:21:56.077885 openbb_fred-1.2.1/openbb_fred/models/series.py
+-rw-r--r--   0        0        0     2150 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/sofr_rates.py
+-rw-r--r--   0        0        0     2382 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/sonia_rates.py
+-rw-r--r--   0        0        0     2732 2024-05-15 09:21:56.077885 openbb_fred-1.2.1/openbb_fred/models/spot.py
+-rw-r--r--   0        0        0     2225 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/tbffr.py
+-rw-r--r--   0        0        0     2305 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/tmc.py
+-rw-r--r--   0        0        0     3257 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/models/us_yield_curve.py
+-rw-r--r--   0        0        0     3858 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/openbb_fred/models/yield_curve.py
+-rw-r--r--   0        0        0    58622 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/utils/commercial_paper.csv
+-rw-r--r--   0        0        0   125899 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/utils/corporate_spot_rates.csv
+-rw-r--r--   0        0        0    20963 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/utils/cpi.csv
+-rw-r--r--   0        0        0     2395 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/utils/fred_base.py
+-rw-r--r--   0        0        0    10771 2024-05-22 11:48:40.531330 openbb_fred-1.2.1/openbb_fred/utils/fred_helpers.py
+-rw-r--r--   0        0        0    10219 2024-05-14 16:56:41.893864 openbb_fred-1.2.1/openbb_fred/utils/harmonized_cpi.csv
+-rw-r--r--   0        0        0   227110 2024-05-14 16:56:41.897865 openbb_fred-1.2.1/openbb_fred/utils/ice_bofa_indices.csv
+-rw-r--r--   0        0        0      465 2024-05-22 13:56:31.167677 openbb_fred-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      971 1970-01-01 00:00:00.000000 openbb_fred-1.2.1/PKG-INFO
```

### Comparing `openbb_fred-1.2.0/openbb_fred/__init__.py` & `openbb_fred-1.2.1/openbb_fred/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """FRED provider module."""
 
 from openbb_core.provider.abstract.provider import Provider
 from openbb_fred.models.ameribor_rates import FREDAMERIBORFetcher
+from openbb_fred.models.balance_of_payments import FredBalanceOfPaymentsFetcher
 from openbb_fred.models.cp import FREDCommercialPaperFetcher
 from openbb_fred.models.cpi import FREDConsumerPriceIndexFetcher
 from openbb_fred.models.dwpcr_rates import FREDDiscountWindowPrimaryCreditRateFetcher
 from openbb_fred.models.ecb_interest_rates import (
     FREDEuropeanCentralBankInterestRatesFetcher,
 )
 from openbb_fred.models.estr_rates import FREDESTRFetcher
@@ -22,26 +23,30 @@
 )
 from openbb_fred.models.series import FredSeriesFetcher
 from openbb_fred.models.sofr_rates import FREDSOFRFetcher
 from openbb_fred.models.sonia_rates import FREDSONIAFetcher
 from openbb_fred.models.spot import FREDSpotRateFetcher
 from openbb_fred.models.tbffr import FREDSelectedTreasuryBillFetcher
 from openbb_fred.models.tmc import FREDTreasuryConstantMaturityFetcher
-from openbb_fred.models.us_yield_curve import FREDYieldCurveFetcher
+from openbb_fred.models.us_yield_curve import (
+    FREDYieldCurveFetcher as FREDUSYieldCurveFetcher,
+)
+from openbb_fred.models.yield_curve import FREDYieldCurveFetcher
 
 fred_provider = Provider(
     name="fred",
     website="https://fred.stlouisfed.org",
     description="""Federal Reserve Economic Data is a database maintained by the
 Research division of the Federal Reserve Bank of St. Louis that has more than
 816,000 economic time series from various sources.""",
     credentials=["api_key"],
     fetcher_dict={
+        "BalanceOfPayments": FredBalanceOfPaymentsFetcher,
         "ConsumerPriceIndex": FREDConsumerPriceIndexFetcher,
-        "USYieldCurve": FREDYieldCurveFetcher,
+        "USYieldCurve": FREDUSYieldCurveFetcher,
         "SOFR": FREDSOFRFetcher,
         "ESTR": FREDESTRFetcher,
         "SONIA": FREDSONIAFetcher,
         "AMERIBOR": FREDAMERIBORFetcher,
         "FEDFUNDS": FREDFEDFetcher,
         "PROJECTIONS": FREDPROJECTIONFetcher,
         "IORB": FREDIORBFetcher,
@@ -54,12 +59,13 @@
         "FredSeries": FredSeriesFetcher,
         "FredRegional": FredRegionalDataFetcher,
         "SpotRate": FREDSpotRateFetcher,
         "HighQualityMarketCorporateBond": FREDHighQualityMarketCorporateBondFetcher,
         "TreasuryConstantMaturity": FREDTreasuryConstantMaturityFetcher,
         "SelectedTreasuryConstantMaturity": FREDSelectedTreasuryConstantMaturityFetcher,
         "SelectedTreasuryBill": FREDSelectedTreasuryBillFetcher,
+        "YieldCurve": FREDYieldCurveFetcher,
     },
     repr_name="Federal Reserve Economic Data | St. Louis FED (FRED)",
     v3_credentials=["API_FRED_KEY"],
     instructions='Go to: https://fred.stlouisfed.org\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827137-d143ba4c-72cb-467d-a7f4-5cc27c597aec.png)\n\nClick on, "My Account", create a new account or sign in with Google:\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827011-65cdd501-27e3-436f-bd9d-b0d8381d46a7.png)\n\nAfter completing the sign-up, go to "My Account", and select "API Keys". Then, click on, "Request API Key".\n\n![FRED](https://user-images.githubusercontent.com/46355364/207827577-c869f989-4ef4-4949-ab57-6f3931f2ae9d.png)\n\nFill in the box for information about the use-case for FRED, and by clicking, "Request API key", at the bottom of the page, the API key will be issued.\n\n![FRED](https://user-images.githubusercontent.com/46355364/207828032-0a32d3b8-1378-4db2-9064-aa1eb2111632.png)',  # noqa: E501  pylint: disable=line-too-long
 )
```

### Comparing `openbb_fred-1.2.0/openbb_fred/models/ameribor_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/ameribor_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/cp.py` & `openbb_fred-1.2.1/openbb_fred/models/cp.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/cpi.py` & `openbb_fred-1.2.1/openbb_fred/models/cpi.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/dwpcr_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/dwpcr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/ecb_interest_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/ecb_interest_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/estr_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/estr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/fed_projections.py` & `openbb_fred-1.2.1/openbb_fred/models/fed_projections.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/fed_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/ffrmc.py` & `openbb_fred-1.2.1/openbb_fred/models/ffrmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/hqm.py` & `openbb_fred-1.2.1/openbb_fred/models/hqm.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/ice_bofa.py` & `openbb_fred-1.2.1/openbb_fred/models/ice_bofa.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/iorb_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/iorb_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/moody.py` & `openbb_fred-1.2.1/openbb_fred/models/moody.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/regional.py` & `openbb_fred-1.2.1/openbb_fred/models/regional.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/search.py` & `openbb_fred-1.2.1/openbb_fred/models/search.py`

 * *Files 1% similar despite different names*

```diff
@@ -117,18 +117,18 @@
         credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Extract the raw data."""
         api_key = credentials.get("fred_api_key") if credentials else ""
 
         if query.series_id is not None:
-            results = []
+            results: List = []
 
             async def get_one(_id: str):
-                data = {}
+                data: Dict = {}
                 url = f"https://api.stlouisfed.org/geofred/series/group?series_id={_id}&api_key={api_key}&file_type=json"
                 response = await amake_request(url)
                 data = response.get("series_group")  # type: ignore
                 if data:
                     data.update({"series_id": _id})
                     results.append(data)
```

### Comparing `openbb_fred-1.2.0/openbb_fred/models/series.py` & `openbb_fred-1.2.1/openbb_fred/models/series.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/sofr_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/sofr_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/sonia_rates.py` & `openbb_fred-1.2.1/openbb_fred/models/sonia_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/spot.py` & `openbb_fred-1.2.1/openbb_fred/models/spot.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/tbffr.py` & `openbb_fred-1.2.1/openbb_fred/models/tbffr.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/tmc.py` & `openbb_fred-1.2.1/openbb_fred/models/tmc.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/models/us_yield_curve.py` & `openbb_fred-1.2.1/openbb_fred/models/us_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/commercial_paper.csv` & `openbb_fred-1.2.1/openbb_fred/utils/commercial_paper.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/corporate_spot_rates.csv` & `openbb_fred-1.2.1/openbb_fred/utils/corporate_spot_rates.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/cpi.csv` & `openbb_fred-1.2.1/openbb_fred/utils/cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/fred_base.py` & `openbb_fred-1.2.1/openbb_fred/utils/fred_base.py`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/harmonized_cpi.csv` & `openbb_fred-1.2.1/openbb_fred/utils/harmonized_cpi.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/openbb_fred/utils/ice_bofa_indices.csv` & `openbb_fred-1.2.1/openbb_fred/utils/ice_bofa_indices.csv`

 * *Files identical despite different names*

### Comparing `openbb_fred-1.2.0/PKG-INFO` & `openbb_fred-1.2.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-fred
-Version: 1.2.0
+Version: 1.2.1
 Summary: FRED extension for OpenBB
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
 
 # OpenBB FRED Provider
 
 This extension integrates the [FRED](https://fred.stlouisfed.org/docs/api/fred/) data provider into the OpenBB Platform.
 
 ## Installation
```

