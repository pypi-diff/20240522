# Comparing `tmp/openbb_cboe-1.2.0.tar.gz` & `tmp/openbb_cboe-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_cboe-1.2.0.tar", max compression
+gzip compressed data, was "openbb_cboe-1.2.1.tar", max compression
```

## Comparing `openbb_cboe-1.2.0.tar` & `openbb_cboe-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      296 2024-05-15 14:26:08.941817 openbb_cboe-1.2.0/README.md
--rw-r--r--   0        0        0     1825 2024-05-14 15:30:05.610928 openbb_cboe-1.2.0/openbb_cboe/__init__.py
--rw-r--r--   0        0        0       38 2024-02-29 11:03:36.758231 openbb_cboe-1.2.0/openbb_cboe/models/__init__.py
--rw-r--r--   0        0        0     3354 2024-04-08 12:02:16.581350 openbb_cboe-1.2.0/openbb_cboe/models/available_indices.py
--rw-r--r--   0        0        0     8396 2024-05-10 10:40:27.290474 openbb_cboe-1.2.0/openbb_cboe/models/equity_historical.py
--rw-r--r--   0        0        0     9663 2024-05-10 10:40:27.290627 openbb_cboe-1.2.0/openbb_cboe/models/equity_quote.py
--rw-r--r--   0        0        0     2149 2024-04-08 12:02:16.581679 openbb_cboe-1.2.0/openbb_cboe/models/equity_search.py
--rw-r--r--   0        0        0     2218 2024-04-23 10:22:39.655242 openbb_cboe-1.2.0/openbb_cboe/models/futures_curve.py
--rw-r--r--   0        0        0     4596 2024-04-08 12:02:16.581852 openbb_cboe-1.2.0/openbb_cboe/models/index_constituents.py
--rw-r--r--   0        0        0     8420 2024-05-10 10:40:27.290789 openbb_cboe-1.2.0/openbb_cboe/models/index_historical.py
--rw-r--r--   0        0        0     3678 2024-04-08 12:02:16.582064 openbb_cboe-1.2.0/openbb_cboe/models/index_search.py
--rw-r--r--   0        0        0     4831 2024-05-09 13:34:29.201648 openbb_cboe-1.2.0/openbb_cboe/models/index_snapshots.py
--rw-r--r--   0        0        0     7796 2024-05-09 13:34:29.201967 openbb_cboe-1.2.0/openbb_cboe/models/options_chains.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.759328 openbb_cboe-1.2.0/openbb_cboe/py.typed
--rw-r--r--   0        0        0       37 2024-02-29 11:03:36.759398 openbb_cboe-1.2.0/openbb_cboe/utils/__init__.py
--rw-r--r--   0        0        0     6467 2024-04-23 10:22:39.655389 openbb_cboe-1.2.0/openbb_cboe/utils/helpers.py
--rw-r--r--   0        0        0      520 2024-05-15 16:06:48.877617 openbb_cboe-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_cboe-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      296 2024-05-22 11:48:40.467330 openbb_cboe-1.2.1/README.md
+-rw-r--r--   0        0        0     1825 2024-05-15 09:21:56.061885 openbb_cboe-1.2.1/openbb_cboe/__init__.py
+-rw-r--r--   0        0        0       38 2024-05-14 16:56:41.677864 openbb_cboe-1.2.1/openbb_cboe/models/__init__.py
+-rw-r--r--   0        0        0     3354 2024-05-14 16:56:41.677864 openbb_cboe-1.2.1/openbb_cboe/models/available_indices.py
+-rw-r--r--   0        0        0     8396 2024-05-15 09:21:56.061885 openbb_cboe-1.2.1/openbb_cboe/models/equity_historical.py
+-rw-r--r--   0        0        0     9663 2024-05-15 09:21:56.061885 openbb_cboe-1.2.1/openbb_cboe/models/equity_quote.py
+-rw-r--r--   0        0        0     2149 2024-05-14 16:56:41.677864 openbb_cboe-1.2.1/openbb_cboe/models/equity_search.py
+-rw-r--r--   0        0        0     2218 2024-05-14 16:56:41.677864 openbb_cboe-1.2.1/openbb_cboe/models/futures_curve.py
+-rw-r--r--   0        0        0     4596 2024-05-14 16:56:41.681864 openbb_cboe-1.2.1/openbb_cboe/models/index_constituents.py
+-rw-r--r--   0        0        0     8420 2024-05-15 09:21:56.061885 openbb_cboe-1.2.1/openbb_cboe/models/index_historical.py
+-rw-r--r--   0        0        0     3678 2024-05-14 16:56:41.681864 openbb_cboe-1.2.1/openbb_cboe/models/index_search.py
+-rw-r--r--   0        0        0     4791 2024-05-22 11:48:40.467330 openbb_cboe-1.2.1/openbb_cboe/models/index_snapshots.py
+-rw-r--r--   0        0        0     7796 2024-05-14 16:57:23.570032 openbb_cboe-1.2.1/openbb_cboe/models/options_chains.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.681864 openbb_cboe-1.2.1/openbb_cboe/py.typed
+-rw-r--r--   0        0        0       37 2024-05-14 16:56:41.681864 openbb_cboe-1.2.1/openbb_cboe/utils/__init__.py
+-rw-r--r--   0        0        0     6488 2024-05-22 11:48:40.467330 openbb_cboe-1.2.1/openbb_cboe/utils/helpers.py
+-rw-r--r--   0        0        0      520 2024-05-22 13:58:22.960047 openbb_cboe-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1049 1970-01-01 00:00:00.000000 openbb_cboe-1.2.1/PKG-INFO
```

### Comparing `openbb_cboe-1.2.0/openbb_cboe/__init__.py` & `openbb_cboe-1.2.1/openbb_cboe/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/available_indices.py` & `openbb_cboe-1.2.1/openbb_cboe/models/available_indices.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/equity_historical.py` & `openbb_cboe-1.2.1/openbb_cboe/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/equity_quote.py` & `openbb_cboe-1.2.1/openbb_cboe/models/equity_quote.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/equity_search.py` & `openbb_cboe-1.2.1/openbb_cboe/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/futures_curve.py` & `openbb_cboe-1.2.1/openbb_cboe/models/futures_curve.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/index_constituents.py` & `openbb_cboe-1.2.1/openbb_cboe/models/index_constituents.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/index_historical.py` & `openbb_cboe-1.2.1/openbb_cboe/models/index_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/index_search.py` & `openbb_cboe-1.2.1/openbb_cboe/models/index_search.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/index_snapshots.py` & `openbb_cboe-1.2.1/openbb_cboe/models/index_snapshots.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 """CBOE Index Snapshots Model."""
 
+# pylint: disable=unused-argument
+
 from datetime import datetime
 from typing import Any, Dict, List, Literal, Optional
 
 from openbb_core.provider.abstract.fetcher import Fetcher
 from openbb_core.provider.standard_models.index_snapshots import (
     IndexSnapshotsData,
     IndexSnapshotsQueryParams,
@@ -23,17 +25,17 @@
 
     region: Optional[Literal["us", "eu"]] = Field(
         default="us",
     )
 
     @field_validator("region", mode="after", check_fields=False)
     @classmethod
-    def validate_region(cls, v: str):
+    def validate_region(cls, v):
         """Validate region."""
-        return "us" if v is None else v
+        return v if v else "us"
 
 
 class CboeIndexSnapshotsData(IndexSnapshotsData):
     """CBOE Index Snapshots Data."""
 
     __alias_dict__ = {
         "prev_close": "prev_day_close",
@@ -85,32 +87,32 @@
     def transform_query(params: Dict[str, Any]) -> CboeIndexSnapshotsQueryParams:
         """Transform the query."""
         return CboeIndexSnapshotsQueryParams(**params)
 
     @staticmethod
     async def aextract_data(
         query: CboeIndexSnapshotsQueryParams,
-        credentials: Optional[Dict[str, str]],  # pylint: disable=unused-argument
+        credentials: Optional[Dict[str, str]],
         **kwargs: Any,
     ) -> List[Dict]:
         """Return the raw data from the Cboe endpoint"""
-
+        url: str = ""
         if query.region == "us":
             url = "https://cdn.cboe.com/api/global/delayed_quotes/quotes/all_us_indices.json"
         if query.region == "eu":
             url = "https://cdn.cboe.com/api/global/european_indices/index_quotes/all-indices.json"
 
         data = await amake_request(url, **kwargs)
-        return data.get("data")
+        return data.get("data")  # type: ignore
 
     @staticmethod
     def transform_data(
-        query: CboeIndexSnapshotsQueryParams,  # pylint: disable=unused-argument
-        data: dict,
-        **kwargs: Any,  # pylint: disable=unused-argument
+        query: CboeIndexSnapshotsQueryParams,
+        data: List[Dict],
+        **kwargs: Any,
     ) -> List[CboeIndexSnapshotsData]:
         """Transform the data to the standard format"""
         if not data:
             raise EmptyDataError()
         df = DataFrame(data)
         percent_cols = [
             "price_change_percent",
```

### Comparing `openbb_cboe-1.2.0/openbb_cboe/models/options_chains.py` & `openbb_cboe-1.2.1/openbb_cboe/models/options_chains.py`

 * *Files identical despite different names*

### Comparing `openbb_cboe-1.2.0/openbb_cboe/utils/helpers.py` & `openbb_cboe-1.2.1/openbb_cboe/utils/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
     if "text" in content_type:
         return await response.text()
     return await response.read()
 
 
 async def get_cboe_data(url, use_cache: bool = True, **kwargs) -> Any:
     """Use the generic Cboe HTTP request."""
+    data: Any = None
     if use_cache is True:
         async with CachedSession(cache=backend) as cached_session:
             try:
                 response = await cached_session.get(url, timeout=10, **kwargs)
                 data = await response_callback(response, None)
             finally:
                 await cached_session.close()
```

### Comparing `openbb_cboe-1.2.0/pyproject.toml` & `openbb_cboe-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "openbb-cboe"
-version = "1.2.0"
+version = "1.2.1"
 description = "CBOE extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_cboe" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 aiohttp-client-cache = "^0.11.0"
 aiosqlite = "^0.20.0"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 cboe = "openbb_cboe:cboe_provider"
```

### Comparing `openbb_cboe-1.2.0/PKG-INFO` & `openbb_cboe-1.2.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: openbb-cboe
-Version: 1.2.0
+Version: 1.2.1
 Summary: CBOE extension for OpenBB
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
 
 # OpenBB CBOE Provider
 
 This extension integrates the [CBOE](https://www.cboe.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

