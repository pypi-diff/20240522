# Comparing `tmp/openbb_ecb-1.2.0.tar.gz` & `tmp/openbb_ecb-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_ecb-1.2.0.tar", max compression
+gzip compressed data, was "openbb_ecb-1.2.1.tar", max compression
```

## Comparing `openbb_ecb-1.2.0.tar` & `openbb_ecb-1.2.1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0      299 2024-05-15 14:26:04.197157 openbb_ecb-1.2.0/README.md
--rw-r--r--   0        0        0      931 2024-05-14 15:30:05.611286 openbb_ecb-1.2.0/openbb_ecb/__init__.py
--rw-r--r--   0        0        0       27 2024-04-23 10:22:39.656547 openbb_ecb-1.2.0/openbb_ecb/models/__init__.py
--rw-r--r--   0        0        0     3305 2024-03-21 17:38:35.638719 openbb_ecb-1.2.0/openbb_ecb/models/balance_of_payments.py
--rw-r--r--   0        0        0     2263 2024-02-29 11:03:36.767005 openbb_ecb-1.2.0/openbb_ecb/models/currency_reference_rates.py
--rw-r--r--   0        0        0     4199 2024-04-08 12:02:16.587780 openbb_ecb-1.2.0/openbb_ecb/models/eu_yield_curve.py
--rw-r--r--   0        0        0       24 2024-04-23 10:22:39.656649 openbb_ecb-1.2.0/openbb_ecb/utils/__init__.py
--rw-r--r--   0        0        0    16135 2024-02-29 11:03:36.767215 openbb_ecb-1.2.0/openbb_ecb/utils/bps_series.py
--rw-r--r--   0        0        0     1374 2024-02-29 11:03:36.767284 openbb_ecb-1.2.0/openbb_ecb/utils/ecb_helpers.py
--rw-r--r--   0        0        0     4867 2024-04-08 12:02:16.587857 openbb_ecb-1.2.0/openbb_ecb/utils/yield_curve_series.py
--rw-r--r--   0        0        0      481 2024-05-15 16:07:27.469945 openbb_ecb-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 openbb_ecb-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      299 2024-05-22 11:48:40.467330 openbb_ecb-1.2.1/README.md
+-rw-r--r--   0        0        0     1038 2024-05-22 11:48:40.467330 openbb_ecb-1.2.1/openbb_ecb/__init__.py
+-rw-r--r--   0        0        0       27 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/models/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/models/balance_of_payments.py
+-rw-r--r--   0        0        0     2263 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/models/currency_reference_rates.py
+-rw-r--r--   0        0        0     4199 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/models/eu_yield_curve.py
+-rw-r--r--   0        0        0     5562 2024-05-22 11:48:40.467330 openbb_ecb-1.2.1/openbb_ecb/models/yield_curve.py
+-rw-r--r--   0        0        0       24 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/utils/__init__.py
+-rw-r--r--   0        0        0    16135 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/utils/bps_series.py
+-rw-r--r--   0        0        0     1374 2024-05-14 16:56:41.689864 openbb_ecb-1.2.1/openbb_ecb/utils/ecb_helpers.py
+-rw-r--r--   0        0        0     5356 2024-05-22 11:48:40.467330 openbb_ecb-1.2.1/openbb_ecb/utils/yield_curve_series.py
+-rw-r--r--   0        0        0      481 2024-05-22 13:57:20.963842 openbb_ecb-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      995 1970-01-01 00:00:00.000000 openbb_ecb-1.2.1/PKG-INFO
```

### Comparing `openbb_ecb-1.2.0/openbb_ecb/__init__.py` & `openbb_ecb-1.2.1/openbb_ecb/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """ECB provider module."""
 
 from openbb_core.provider.abstract.provider import Provider
 from openbb_ecb.models.balance_of_payments import ECBBalanceOfPaymentsFetcher
 from openbb_ecb.models.currency_reference_rates import ECBCurrencyReferenceRatesFetcher
 from openbb_ecb.models.eu_yield_curve import ECBEUYieldCurveFetcher
+from openbb_ecb.models.yield_curve import ECBYieldCurveFetcher
 
 ecb_provider = Provider(
     name="ECB",
     website="https://data.ecb.europa.eu",
     description="""The ECB Data Portal provides access to all official ECB statistics.
 The portal also provides options to download data and comprehensive metadata for each dataset.
 Statistical publications and dashboards offer a compilation of key data on selected topics.""",
     fetcher_dict={
         "BalanceOfPayments": ECBBalanceOfPaymentsFetcher,
         "CurrencyReferenceRates": ECBCurrencyReferenceRatesFetcher,
         "EUYieldCurve": ECBEUYieldCurveFetcher,
+        "YieldCurve": ECBYieldCurveFetcher,
     },
     repr_name="European Central Bank (ECB)",
 )
```

### Comparing `openbb_ecb-1.2.0/openbb_ecb/models/balance_of_payments.py` & `openbb_ecb-1.2.1/openbb_ecb/models/balance_of_payments.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.2.0/openbb_ecb/models/currency_reference_rates.py` & `openbb_ecb-1.2.1/openbb_ecb/models/currency_reference_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.2.0/openbb_ecb/models/eu_yield_curve.py` & `openbb_ecb-1.2.1/openbb_ecb/models/eu_yield_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.2.0/openbb_ecb/utils/bps_series.py` & `openbb_ecb-1.2.1/openbb_ecb/utils/bps_series.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.2.0/openbb_ecb/utils/ecb_helpers.py` & `openbb_ecb-1.2.1/openbb_ecb/utils/ecb_helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_ecb-1.2.0/openbb_ecb/utils/yield_curve_series.py` & `openbb_ecb-1.2.1/openbb_ecb/utils/yield_curve_series.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,49 @@
 
 YIELD_TYPE_DICT = {
     "spot_rate": "SR",
     "instantaneous_forward": "IF",
     "par_yield": "PY",
 }
 
+MATURITIES = [
+    "month_3",
+    "month_6",
+    "year_1",
+    "year_2",
+    "year_3",
+    "year_4",
+    "year_5",
+    "year_6",
+    "year_7",
+    "year_8",
+    "year_9",
+    "year_10",
+    "year_11",
+    "year_12",
+    "year_13",
+    "year_14",
+    "year_15",
+    "year_16",
+    "year_17",
+    "year_18",
+    "year_19",
+    "year_20",
+    "year_21",
+    "year_22",
+    "year_23",
+    "year_24",
+    "year_25",
+    "year_26",
+    "year_27",
+    "year_28",
+    "year_29",
+    "year_30",
+]
+
 
 def get_yield_curve_ids(
     rating: Literal["aaa", "all_ratings"] = "aaa",
     yield_curve_type: Literal[
         "spot_rate", "instantaneous_forward", "par_yield"
     ] = "spot_rate",
 ) -> Dict:
```

### Comparing `openbb_ecb-1.2.0/PKG-INFO` & `openbb_ecb-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-ecb
-Version: 1.2.0
+Version: 1.2.1
 Summary: ECB extension for OpenBB
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
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
 Description-Content-Type: text/markdown
 
 # OpenBB ECB Provider
 
 This extension integrates the [ECB](https://data.ecb.europa.eu/) data provider into the OpenBB Platform.
```

