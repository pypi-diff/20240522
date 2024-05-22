# Comparing `tmp/openbb_etf-1.2.0.tar.gz` & `tmp/openbb_etf-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_etf-1.2.0.tar", max compression
+gzip compressed data, was "openbb_etf-1.2.1.tar", max compression
```

## Comparing `openbb_etf-1.2.0.tar` & `openbb_etf-1.2.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      225 2024-05-15 14:34:21.677648 openbb_etf-1.2.0/README.md
--rw-r--r--   0        0        0       28 2024-02-29 11:03:36.737607 openbb_etf-1.2.0/openbb_etf/__init__.py
--rw-r--r--   0        0        0       21 2024-02-29 11:03:36.737701 openbb_etf-1.2.0/openbb_etf/discovery/__init__.py
--rw-r--r--   0        0        0     1770 2024-04-08 12:02:16.528487 openbb_etf-1.2.0/openbb_etf/discovery/discovery_router.py
--rw-r--r--   0        0        0     6392 2024-04-23 10:22:39.603236 openbb_etf-1.2.0/openbb_etf/etf_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.737920 openbb_etf-1.2.0/openbb_etf/py.typed
--rw-r--r--   0        0        0      467 2024-05-15 16:04:50.102434 openbb_etf-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 openbb_etf-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      225 2024-05-22 11:48:40.403330 openbb_etf-1.2.1/README.md
+-rw-r--r--   0        0        0       28 2024-05-14 16:56:41.565863 openbb_etf-1.2.1/openbb_etf/__init__.py
+-rw-r--r--   0        0        0       21 2024-05-14 16:56:41.565863 openbb_etf-1.2.1/openbb_etf/discovery/__init__.py
+-rw-r--r--   0        0        0     1770 2024-05-14 16:56:41.565863 openbb_etf-1.2.1/openbb_etf/discovery/discovery_router.py
+-rw-r--r--   0        0        0     5625 2024-05-22 11:48:40.407330 openbb_etf-1.2.1/openbb_etf/etf_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.565863 openbb_etf-1.2.1/openbb_etf/py.typed
+-rw-r--r--   0        0        0      467 2024-05-22 13:55:53.703553 openbb_etf-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      827 1970-01-01 00:00:00.000000 openbb_etf-1.2.1/PKG-INFO
```

### Comparing `openbb_etf-1.2.0/openbb_etf/discovery/discovery_router.py` & `openbb_etf-1.2.1/openbb_etf/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_etf-1.2.0/openbb_etf/etf_router.py` & `openbb_etf-1.2.1/openbb_etf/etf_router.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """ETF Router."""
 
-from openbb_core.app.deprecation import OpenBBDeprecationWarning
 from openbb_core.app.model.command_context import CommandContext
 from openbb_core.app.model.example import APIEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.provider_interface import (
     ExtraParams,
     ProviderChoices,
     StandardParams,
@@ -168,35 +167,14 @@
     extra_params: ExtraParams,
 ) -> OBBject:
     """Use this function to get the holdings dates, if available."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
-    model="EtfHoldingsPerformance",
-    deprecated=True,
-    deprecation=OpenBBDeprecationWarning(
-        message="This endpoint is deprecated; pass a list of holdings symbols directly to"
-        + " `/equity/price/performance` instead.",
-        since=(4, 1),
-        expected_removal=(4, 2),
-    ),
-    examples=[APIEx(parameters={"symbol": "XLK", "provider": "fmp"})],
-)
-async def holdings_performance(
-    cc: CommandContext,
-    provider_choices: ProviderChoices,
-    standard_params: StandardParams,
-    extra_params: ExtraParams,
-) -> OBBject:
-    """Get the recent price performance of each ticker held in the ETF."""
-    return await OBBject.from_query(Query(**locals()))
-
-
-@router.command(
     model="EtfEquityExposure",
     examples=[
         APIEx(parameters={"symbol": "MSFT", "provider": "fmp"}),
         APIEx(
             description="This function accepts multiple tickers.",
             parameters={"symbol": "MSFT,AAPL", "provider": "fmp"},
         ),
```

### Comparing `openbb_etf-1.2.0/PKG-INFO` & `openbb_etf-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: openbb-etf
-Version: 1.2.0
+Version: 1.2.1
 Summary: ETF extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB Team
 Author-email: hello@openbb.co
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 # ETF data extension for OpenBB SDK
 
 This extension provides a set of commands for ETF data retrieval.
 
 ## Installation
```

