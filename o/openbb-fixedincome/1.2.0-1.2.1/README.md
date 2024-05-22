# Comparing `tmp/openbb_fixedincome-1.2.0.tar.gz` & `tmp/openbb_fixedincome-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_fixedincome-1.2.0.tar", max compression
+gzip compressed data, was "openbb_fixedincome-1.2.1.tar", max compression
```

## Comparing `openbb_fixedincome-1.2.0.tar` & `openbb_fixedincome-1.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      425 2024-05-15 14:28:02.311514 openbb_fixedincome-1.2.0/README.md
--rw-r--r--   0        0        0       32 2024-02-29 11:03:36.738645 openbb_fixedincome-1.2.0/openbb_fixedincome/__init__.py
--rw-r--r--   0        0        0       52 2024-02-29 11:03:36.738725 openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/__init__.py
--rw-r--r--   0        0        0     4950 2024-04-08 12:02:16.529389 openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/corporate_router.py
--rw-r--r--   0        0        0     1582 2024-04-23 10:22:39.604538 openbb_fixedincome-1.2.0/openbb_fixedincome/fixedincome_router.py
--rw-r--r--   0        0        0       53 2024-02-29 11:03:36.738953 openbb_fixedincome-1.2.0/openbb_fixedincome/government/__init__.py
--rw-r--r--   0        0        0     4485 2024-04-08 12:02:16.529631 openbb_fixedincome-1.2.0/openbb_fixedincome/government/government_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.739091 openbb_fixedincome-1.2.0/openbb_fixedincome/py.typed
--rw-r--r--   0        0        0       43 2024-02-29 11:03:36.739181 openbb_fixedincome-1.2.0/openbb_fixedincome/rate/__init__.py
--rw-r--r--   0        0        0     6955 2024-04-08 12:02:16.529749 openbb_fixedincome-1.2.0/openbb_fixedincome/rate/rate_router.py
--rw-r--r--   0        0        0       50 2024-02-29 11:03:36.739375 openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/__init__.py
--rw-r--r--   0        0        0     3076 2024-04-08 12:02:16.529856 openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/spreads_router.py
--rw-r--r--   0        0        0      509 2024-05-15 16:04:32.741103 openbb_fixedincome-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 openbb_fixedincome-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      425 2024-05-22 11:48:40.407330 openbb_fixedincome-1.2.1/README.md
+-rw-r--r--   0        0        0       32 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/__init__.py
+-rw-r--r--   0        0        0       52 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/corporate/__init__.py
+-rw-r--r--   0        0        0     4950 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/corporate/corporate_router.py
+-rw-r--r--   0        0        0     1582 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/fixedincome_router.py
+-rw-r--r--   0        0        0       53 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/government/__init__.py
+-rw-r--r--   0        0        0     6003 2024-05-22 11:48:40.407330 openbb_fixedincome-1.2.1/openbb_fixedincome/government/government_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/py.typed
+-rw-r--r--   0        0        0       43 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/rate/__init__.py
+-rw-r--r--   0        0        0     6955 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/rate/rate_router.py
+-rw-r--r--   0        0        0       50 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/spreads/__init__.py
+-rw-r--r--   0        0        0     3076 2024-05-14 16:56:41.565863 openbb_fixedincome-1.2.1/openbb_fixedincome/spreads/spreads_router.py
+-rw-r--r--   0        0        0      509 2024-05-22 13:55:09.527406 openbb_fixedincome-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1094 1970-01-01 00:00:00.000000 openbb_fixedincome-1.2.1/PKG-INFO
```

### Comparing `openbb_fixedincome-1.2.0/openbb_fixedincome/corporate/corporate_router.py` & `openbb_fixedincome-1.2.1/openbb_fixedincome/corporate/corporate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.2.0/openbb_fixedincome/fixedincome_router.py` & `openbb_fixedincome-1.2.1/openbb_fixedincome/fixedincome_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.2.0/openbb_fixedincome/government/government_router.py` & `openbb_fixedincome-1.2.1/openbb_fixedincome/government/government_router.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Fixed Income Government Router."""
 
+from openbb_core.app.deprecation import OpenBBDeprecationWarning
 from openbb_core.app.model.command_context import CommandContext
 from openbb_core.app.model.example import APIEx
 from openbb_core.app.model.obbject import OBBject
 from openbb_core.app.provider_interface import (
     ExtraParams,
     ProviderChoices,
     StandardParams,
@@ -13,15 +14,53 @@
 
 router = Router(prefix="/government")
 
 # pylint: disable=unused-argument
 
 
 @router.command(
+    model="YieldCurve",
+    examples=[
+        APIEx(parameters={"provider": "federal_reserve"}),
+        APIEx(parameters={"date": "2023-05-01,2024-05-01", "provider": "fmp"}),
+        APIEx(
+            parameters={
+                "date": "2023-05-01",
+                "country": "united_kingdom",
+                "provider": "econdb",
+            }
+        ),
+        APIEx(parameters={"provider": "ecb", "yield_curve_type": "par_yield"}),
+        APIEx(
+            parameters={
+                "provider": "fred",
+                "yield_curve_type": "real",
+                "date": "2023-05-01,2024-05-01",
+            }
+        ),
+    ],
+)
+async def yield_curve(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:  # type: ignore
+    """Get yield curve data by country and date."""
+    return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
     model="USYieldCurve",
+    deprecated=True,
+    deprecation=OpenBBDeprecationWarning(
+        message="This endpoint will be removed in a future version. Use, `/fixedincome/government/yield_curve`, instead.",
+        since=(4, 2),
+        expected_removal=(4, 4),
+    ),
     examples=[
         APIEx(parameters={"provider": "fred"}),
         APIEx(parameters={"inflation_adjusted": True, "provider": "fred"}),
     ],
 )
 async def us_yield_curve(
     cc: CommandContext,
@@ -31,14 +70,20 @@
 ) -> OBBject:  # type: ignore
     """US Yield Curve. Get United States yield curve."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="EUYieldCurve",
+    deprecated=True,
+    deprecation=OpenBBDeprecationWarning(
+        message="This endpoint will be removed in a future version. Use, `/fixedincome/government/yield_curve`, instead.",
+        since=(4, 2),
+        expected_removal=(4, 4),
+    ),
     examples=[
         APIEx(parameters={"provider": "ecb"}),
         APIEx(parameters={"yield_curve_type": "spot_rate", "provider": "ecb"}),
     ],
 )
 async def eu_yield_curve(
     cc: CommandContext,
```

### Comparing `openbb_fixedincome-1.2.0/openbb_fixedincome/rate/rate_router.py` & `openbb_fixedincome-1.2.1/openbb_fixedincome/rate/rate_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.2.0/openbb_fixedincome/spreads/spreads_router.py` & `openbb_fixedincome-1.2.1/openbb_fixedincome/spreads/spreads_router.py`

 * *Files identical despite different names*

### Comparing `openbb_fixedincome-1.2.0/PKG-INFO` & `openbb_fixedincome-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-fixedincome
-Version: 1.2.0
+Version: 1.2.1
 Summary: Fixed income extension for OpenBB
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
 
 # OpenBB Fixed Income Extension
 
 This extension provides fixed income data for the OpenBB Platform.
 
 Features of the Fixed Income extension include information on government bonds and central bank rates.
```

