# Comparing `tmp/openbb_federal_reserve-1.2.0.tar.gz` & `tmp/openbb_federal_reserve-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_federal_reserve-1.2.0.tar", max compression
+gzip compressed data, was "openbb_federal_reserve-1.2.1.tar", max compression
```

## Comparing `openbb_federal_reserve-1.2.0.tar` & `openbb_federal_reserve-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0      347 2024-05-15 14:25:55.077678 openbb_federal_reserve-1.2.0/README.md
--rw-r--r--   0        0        0      882 2024-05-14 15:30:05.612043 openbb_federal_reserve-1.2.0/openbb_federal_reserve/__init__.py
--rw-r--r--   0        0        0     2678 2024-04-08 12:02:16.625822 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/fed_rates.py
--rw-r--r--   0        0        0     3538 2024-04-02 11:35:59.435928 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/money_measures.py
--rw-r--r--   0        0        0     3517 2024-05-09 15:04:29.070261 openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/treasury_rates.py
--rw-r--r--   0        0        0      534 2024-05-15 16:06:36.900651 openbb_federal_reserve-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      347 2024-05-22 11:48:40.523330 openbb_federal_reserve-1.2.1/README.md
+-rw-r--r--   0        0        0     1023 2024-05-22 11:48:40.523330 openbb_federal_reserve-1.2.1/openbb_federal_reserve/__init__.py
+-rw-r--r--   0        0        0     2678 2024-05-14 16:56:41.769864 openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/fed_rates.py
+-rw-r--r--   0        0        0     3538 2024-05-14 16:56:41.769864 openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/money_measures.py
+-rw-r--r--   0        0        0     3517 2024-05-15 09:21:56.065885 openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/treasury_rates.py
+-rw-r--r--   0        0        0     3635 2024-05-22 11:48:40.523330 openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/yield_curve.py
+-rw-r--r--   0        0        0      534 2024-05-22 13:58:05.435989 openbb_federal_reserve-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1026 1970-01-01 00:00:00.000000 openbb_federal_reserve-1.2.1/PKG-INFO
```

### Comparing `openbb_federal_reserve-1.2.0/openbb_federal_reserve/__init__.py` & `openbb_federal_reserve-1.2.1/openbb_federal_reserve/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,20 +4,22 @@
 from openbb_federal_reserve.models.fed_rates import FederalReserveFEDFetcher
 from openbb_federal_reserve.models.money_measures import (
     FederalReserveMoneyMeasuresFetcher,
 )
 from openbb_federal_reserve.models.treasury_rates import (
     FederalReserveTreasuryRatesFetcher,
 )
+from openbb_federal_reserve.models.yield_curve import FederalReserveYieldCurveFetcher
 
 federal_reserve_provider = Provider(
     name="federal_reserve",
     website="https://www.federalreserve.gov/data.htm",  #  Not a typo, it's really .htm
     description="""Access data provided by the Federal Reserve System,
 the Central Bank of the United States.""",
     fetcher_dict={
         "TreasuryRates": FederalReserveTreasuryRatesFetcher,
         "MoneyMeasures": FederalReserveMoneyMeasuresFetcher,
         "FEDFUNDS": FederalReserveFEDFetcher,
+        "YieldCurve": FederalReserveYieldCurveFetcher,
     },
     repr_name="Federal Reserve (FED)",
 )
```

### Comparing `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/fed_rates.py` & `openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/fed_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/money_measures.py` & `openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/money_measures.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.2.0/openbb_federal_reserve/models/treasury_rates.py` & `openbb_federal_reserve-1.2.1/openbb_federal_reserve/models/treasury_rates.py`

 * *Files identical despite different names*

### Comparing `openbb_federal_reserve-1.2.0/pyproject.toml` & `openbb_federal_reserve-1.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-federal-reserve"
-version = "1.2.0"
+version = "1.2.1"
 description = "US Federal Reserve Data Extension for OpenBB"
 authors = ["OpenBB <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_federal_reserve" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 federal_reserve = "openbb_federal_reserve:federal_reserve_provider"
```

### Comparing `openbb_federal_reserve-1.2.0/PKG-INFO` & `openbb_federal_reserve-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-federal-reserve
-Version: 1.2.0
+Version: 1.2.1
 Summary: US Federal Reserve Data Extension for OpenBB
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
 
 # OpenBB Federal Reserve Provider
 
 This extension integrates the [Federal Reserve](https://www.federalreserve.gov/data.htm) data provider into the OpenBB Platform.
 
 ## Installation
```

