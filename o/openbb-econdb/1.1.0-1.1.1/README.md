# Comparing `tmp/openbb_econdb-1.1.0.tar.gz` & `tmp/openbb_econdb-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_econdb-1.1.0.tar", max compression
+gzip compressed data, was "openbb_econdb-1.1.1.tar", max compression
```

## Comparing `openbb_econdb-1.1.0.tar` & `openbb_econdb-1.1.1.tar`

### file list

```diff
@@ -1,17 +1,19 @@
--rw-r--r--   0        0        0      300 2024-05-15 14:25:59.871940 openbb_econdb-1.1.0/README.md
--rw-r--r--   0        0        0     1130 2024-05-14 15:30:05.611645 openbb_econdb-1.1.0/openbb_econdb/__init__.py
--rw-r--r--   0        0        0       21 2024-05-09 13:34:29.202341 openbb_econdb-1.1.0/openbb_econdb/models/__init__.py
--rw-r--r--   0        0        0     3207 2024-05-09 13:34:29.202409 openbb_econdb-1.1.0/openbb_econdb/models/available_indicators.py
--rw-r--r--   0        0        0    12510 2024-05-10 10:40:27.291012 openbb_econdb-1.1.0/openbb_econdb/models/country_profile.py
--rw-r--r--   0        0        0    20336 2024-05-10 10:40:27.291148 openbb_econdb-1.1.0/openbb_econdb/models/economic_indicators.py
--rw-r--r--   0        0        0       24 2024-05-09 13:34:29.202928 openbb_econdb-1.1.0/openbb_econdb/utils/__init__.py
--rw-r--r--   0        0        0    22272 2024-05-15 14:15:28.219567 openbb_econdb-1.1.0/openbb_econdb/utils/helpers.py
--rw-r--r--   0        0        0    24368 2024-05-09 13:34:29.203457 openbb_econdb-1.1.0/openbb_econdb/utils/indicator_countries.json
--rw-r--r--   0        0        0     5244 2024-05-09 13:34:29.203595 openbb_econdb-1.1.0/openbb_econdb/utils/indicators_descriptions.json
--rw-r--r--   0        0        0     8156 2024-05-09 15:04:29.069737 openbb_econdb-1.1.0/openbb_econdb/utils/main_indicators.py
--rw-r--r--   0        0        0    66758 2024-05-09 13:34:29.203958 openbb_econdb-1.1.0/openbb_econdb/utils/multipliers.json
--rw-r--r--   0        0        0    87109 2024-05-09 13:34:29.204232 openbb_econdb-1.1.0/openbb_econdb/utils/scales.json
--rw-r--r--   0        0        0    73815 2024-05-09 13:34:29.204491 openbb_econdb-1.1.0/openbb_econdb/utils/symbol_to_indicator.json
--rw-r--r--   0        0        0    90624 2024-05-09 13:34:29.204948 openbb_econdb-1.1.0/openbb_econdb/utils/units.json
--rw-r--r--   0        0        0      532 2024-05-15 16:06:59.444263 openbb_econdb-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 openbb_econdb-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0      300 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/README.md
+-rw-r--r--   0        0        0     1246 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/models/__init__.py
+-rw-r--r--   0        0        0     3207 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/models/available_indicators.py
+-rw-r--r--   0        0        0    12510 2024-05-15 09:21:56.065885 openbb_econdb-1.1.1/openbb_econdb/models/country_profile.py
+-rw-r--r--   0        0        0    20098 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/models/economic_indicators.py
+-rw-r--r--   0        0        0     7534 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/models/yield_curve.py
+-rw-r--r--   0        0        0       24 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/__init__.py
+-rw-r--r--   0        0        0    22272 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/utils/helpers.py
+-rw-r--r--   0        0        0    24368 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/indicator_countries.json
+-rw-r--r--   0        0        0     5244 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/indicators_descriptions.json
+-rw-r--r--   0        0        0     8206 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/utils/main_indicators.py
+-rw-r--r--   0        0        0    66758 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/multipliers.json
+-rw-r--r--   0        0        0    87109 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/scales.json
+-rw-r--r--   0        0        0    73815 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/symbol_to_indicator.json
+-rw-r--r--   0        0        0    90624 2024-05-14 16:57:23.574032 openbb_econdb-1.1.1/openbb_econdb/utils/units.json
+-rw-r--r--   0        0        0     7477 2024-05-22 11:48:40.519330 openbb_econdb-1.1.1/openbb_econdb/utils/yield_curves.py
+-rw-r--r--   0        0        0      532 2024-05-22 13:55:58.983570 openbb_econdb-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1057 1970-01-01 00:00:00.000000 openbb_econdb-1.1.1/PKG-INFO
```

### Comparing `openbb_econdb-1.1.0/openbb_econdb/__init__.py` & `openbb_econdb-1.1.1/openbb_econdb/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """EconDB provider module."""
 
 from openbb_core.provider.abstract.provider import Provider
 from openbb_econdb.models.available_indicators import EconDbAvailableIndicatorsFetcher
 from openbb_econdb.models.country_profile import EconDbCountryProfileFetcher
 from openbb_econdb.models.economic_indicators import EconDbEconomicIndicatorsFetcher
+from openbb_econdb.models.yield_curve import EconDbYieldCurveFetcher
 
 econdb_provider = Provider(
     name="EconDB",
     website="https://econdb.com",
     description="""The mission of the company is to process information in ways that
 facilitate understanding of the economic situation at different granularity levels.
 
@@ -17,10 +18,11 @@
     credentials=[
         "api_key"
     ],  # Can be left as None, an attempt to use a temporary token will be made.
     fetcher_dict={
         "AvailableIndicators": EconDbAvailableIndicatorsFetcher,
         "CountryProfile": EconDbCountryProfileFetcher,
         "EconomicIndicators": EconDbEconomicIndicatorsFetcher,
+        "YieldCurve": EconDbYieldCurveFetcher,
     },
     repr_name="EconDB",
 )
```

### Comparing `openbb_econdb-1.1.0/openbb_econdb/models/available_indicators.py` & `openbb_econdb-1.1.1/openbb_econdb/models/available_indicators.py`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/models/country_profile.py` & `openbb_econdb-1.1.1/openbb_econdb/models/country_profile.py`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/models/economic_indicators.py` & `openbb_econdb-1.1.1/openbb_econdb/models/economic_indicators.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,22 +381,17 @@
                     scale in ["Units", "PERCENT"]
                     and units == "DOMESTIC"
                     and "COMMODITY:Commodity" in add_info
                 ):
                     units = "USD"
                 elif scale == "Units":
                     units = (
-                        (
-                            add_info["UNIT_MEASURE:UNIT_MEASURE"]
-                            if "UNIT_MEASURE:UNIT_MEASURE" in add_info
-                            else (
-                                add_info["UNIT:Unit of measure"]
-                                if "UNIT:Unit of measure" in add_info
-                                else units
-                            )
+                        add_info.get(
+                            "UNIT_MEASURE:UNIT_MEASURE",
+                            add_info.get("UNIT:Unit of measure", units),
                         )
                         if units != "USD"
                         else units
                     )
             units = units.replace("PC:Percentage", "PERCENT")
             if ", " in units:
                 units = units.split(", ")[1]
```

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/helpers.py` & `openbb_econdb-1.1.1/openbb_econdb/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/indicator_countries.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/indicator_countries.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/indicators_descriptions.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/indicators_descriptions.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/main_indicators.py` & `openbb_econdb-1.1.1/openbb_econdb/utils/main_indicators.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Main Indicators"""
 
 from datetime import datetime, timedelta
-from typing import Dict, List, Literal
+from typing import Dict, List, Literal, Union
 
 from aiohttp_client_cache import SQLiteBackend
 from aiohttp_client_cache.session import CachedSession
 from numpy import arange
 from openbb_core.app.utils import get_user_cache_directory
 from openbb_core.provider.utils.helpers import amake_request
 from openbb_econdb.utils.helpers import COUNTRY_MAP, THREE_LETTER_ISO_MAP
@@ -68,14 +68,15 @@
     "OILPROD",
     "POP",
 ]
 
 
 async def fetch_data(url, use_cache: bool = True):
     """Fetch the data with or without the cached session object."""
+    response: Union[dict, List[dict]] = {}
     if use_cache is True:
         cache_dir = f"{get_user_cache_directory()}/http/econdb_main_indicators"
         async with CachedSession(
             cache=SQLiteBackend(cache_dir, expire_after=3600 * 24)
         ) as session:
             try:
                 response = await amake_request(url, session=session)
```

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/multipliers.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/multipliers.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/scales.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/scales.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/symbol_to_indicator.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/symbol_to_indicator.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/openbb_econdb/utils/units.json` & `openbb_econdb-1.1.1/openbb_econdb/utils/units.json`

 * *Files identical despite different names*

### Comparing `openbb_econdb-1.1.0/pyproject.toml` & `openbb_econdb-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-econdb"
-version = "1.1.0"
+version = "1.1.1"
 description = "EconDB extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_econdb" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 aiohttp-client-cache = "^0.11.0"
 aiosqlite = "^0.20.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_econdb-1.1.0/PKG-INFO` & `openbb_econdb-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openbb-econdb
-Version: 1.1.0
+Version: 1.1.1
 Summary: EconDB extension for OpenBB
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
 Requires-Dist: aiohttp-client-cache (>=0.11.0,<0.12.0)
 Requires-Dist: aiosqlite (>=0.20.0,<0.21.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB EconDB Provider
 
 This extension integrates the [EconDB](https://econdb.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

