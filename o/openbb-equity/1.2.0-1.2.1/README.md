# Comparing `tmp/openbb_equity-1.2.0.tar.gz` & `tmp/openbb_equity-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_equity-1.2.0.tar", max compression
+gzip compressed data, was "openbb_equity-1.2.1.tar", max compression
```

## Comparing `openbb_equity-1.2.0.tar` & `openbb_equity-1.2.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      811 2024-05-15 14:27:57.593072 openbb_equity-1.2.0/README.md
--rw-r--r--   0        0        0       19 2024-02-29 11:03:36.735289 openbb_equity-1.2.0/openbb_equity/__init__.py
--rw-r--r--   0        0        0       23 2024-02-29 11:03:36.735486 openbb_equity-1.2.0/openbb_equity/calendar/__init__.py
--rw-r--r--   0        0        0     3363 2024-04-08 12:02:16.526785 openbb_equity-1.2.0/openbb_equity/calendar/calendar_router.py
--rw-r--r--   0        0        0       27 2024-02-29 11:03:36.735656 openbb_equity-1.2.0/openbb_equity/compare/__init__.py
--rw-r--r--   0        0        0     2336 2024-04-23 10:22:39.601068 openbb_equity-1.2.0/openbb_equity/compare/compare_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735800 openbb_equity-1.2.0/openbb_equity/darkpool/__init__.py
--rw-r--r--   0        0        0     1114 2024-04-23 10:22:39.601202 openbb_equity-1.2.0/openbb_equity/darkpool/darkpool_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.735942 openbb_equity-1.2.0/openbb_equity/discovery/__init__.py
--rw-r--r--   0        0        0     5816 2024-04-23 10:22:39.601331 openbb_equity-1.2.0/openbb_equity/discovery/discovery_router.py
--rw-r--r--   0        0        0     3493 2024-04-23 10:22:39.601428 openbb_equity-1.2.0/openbb_equity/equity_router.py
--rw-r--r--   0        0        0       17 2024-02-29 11:03:36.736112 openbb_equity-1.2.0/openbb_equity/estimates/__init__.py
--rw-r--r--   0        0        0     4366 2024-05-14 15:30:05.607022 openbb_equity-1.2.0/openbb_equity/estimates/estimates_router.py
--rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736244 openbb_equity-1.2.0/openbb_equity/fundamental/__init__.py
--rw-r--r--   0        0        0    14607 2024-04-08 12:02:16.527537 openbb_equity-1.2.0/openbb_equity/fundamental/fundamental_router.py
--rw-r--r--   0        0        0       24 2024-02-29 11:03:36.736420 openbb_equity-1.2.0/openbb_equity/ownership/__init__.py
--rw-r--r--   0        0        0     3787 2024-04-23 10:22:39.601673 openbb_equity-1.2.0/openbb_equity/ownership/ownership_router.py
--rw-r--r--   0        0        0       20 2024-02-29 11:03:36.736541 openbb_equity-1.2.0/openbb_equity/price/__init__.py
--rw-r--r--   0        0        0     2288 2024-05-02 09:00:10.663331 openbb_equity-1.2.0/openbb_equity/price/price_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.736634 openbb_equity-1.2.0/openbb_equity/py.typed
--rw-r--r--   0        0        0       14 2024-02-29 11:03:36.736696 openbb_equity-1.2.0/openbb_equity/shorts/__init__.py
--rw-r--r--   0        0        0     1654 2024-04-08 12:02:16.527854 openbb_equity-1.2.0/openbb_equity/shorts/shorts_router.py
--rw-r--r--   0        0        0      478 2024-05-15 16:04:38.767137 openbb_equity-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 openbb_equity-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      811 2024-05-22 11:48:40.403330 openbb_equity-1.2.1/README.md
+-rw-r--r--   0        0        0       19 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/calendar/__init__.py
+-rw-r--r--   0        0        0     3363 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/calendar/calendar_router.py
+-rw-r--r--   0        0        0       27 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/compare/__init__.py
+-rw-r--r--   0        0        0     3214 2024-05-22 11:48:40.403330 openbb_equity-1.2.1/openbb_equity/compare/compare_router.py
+-rw-r--r--   0        0        0       17 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/darkpool/__init__.py
+-rw-r--r--   0        0        0     1114 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/darkpool/darkpool_router.py
+-rw-r--r--   0        0        0       17 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/discovery/__init__.py
+-rw-r--r--   0        0        0     5816 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/discovery/discovery_router.py
+-rw-r--r--   0        0        0     3493 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/equity_router.py
+-rw-r--r--   0        0        0       17 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/estimates/__init__.py
+-rw-r--r--   0        0        0     5128 2024-05-22 11:48:40.403330 openbb_equity-1.2.1/openbb_equity/estimates/estimates_router.py
+-rw-r--r--   0        0        0       20 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/fundamental/__init__.py
+-rw-r--r--   0        0        0    14607 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/fundamental/fundamental_router.py
+-rw-r--r--   0        0        0       24 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/ownership/__init__.py
+-rw-r--r--   0        0        0     3787 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/ownership/ownership_router.py
+-rw-r--r--   0        0        0       20 2024-05-14 16:56:41.561863 openbb_equity-1.2.1/openbb_equity/price/__init__.py
+-rw-r--r--   0        0        0     2288 2024-05-14 16:56:41.565863 openbb_equity-1.2.1/openbb_equity/price/price_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.565863 openbb_equity-1.2.1/openbb_equity/py.typed
+-rw-r--r--   0        0        0       14 2024-05-14 16:56:41.565863 openbb_equity-1.2.1/openbb_equity/shorts/__init__.py
+-rw-r--r--   0        0        0     1654 2024-05-14 16:56:41.565863 openbb_equity-1.2.1/openbb_equity/shorts/shorts_router.py
+-rw-r--r--   0        0        0      478 2024-05-22 13:55:47.311531 openbb_equity-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1469 1970-01-01 00:00:00.000000 openbb_equity-1.2.1/PKG-INFO
```

### Comparing `openbb_equity-1.2.0/README.md` & `openbb_equity-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/calendar/calendar_router.py` & `openbb_equity-1.2.1/openbb_equity/calendar/calendar_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/compare/compare_router.py` & `openbb_equity-1.2.1/openbb_equity/compare/compare_router.py`

 * *Files 22% similar despite different names*

```diff
@@ -67,7 +67,38 @@
 ) -> OBBject:
     """Get company data grouped by sector, industry or country and display either performance or valuation metrics.
 
     Valuation metrics include price to earnings, price to book, price to sales ratios and price to cash flow.
     Performance metrics include the stock price change for different time periods.
     """
     return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
+    model="CompareCompanyFacts",
+    examples=[
+        APIEx(parameters={"provider": "sec"}),
+        APIEx(
+            parameters={
+                "provider": "sec",
+                "fact": "PaymentsForRepurchaseOfCommonStock",
+                "year": 2023,
+            }
+        ),
+        APIEx(
+            parameters={
+                "provider": "sec",
+                "symbol": "NVDA,AAPL,AMZN,MSFT,GOOG,SMCI",
+                "fact": "RevenueFromContractWithCustomerExcludingAssessedTax",
+                "year": 2024,
+            }
+        ),
+    ],
+)
+async def company_facts(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Copmare reported company facts and fundamental data points."""
+    return await OBBject.from_query(Query(**locals()))
```

### Comparing `openbb_equity-1.2.0/openbb_equity/darkpool/darkpool_router.py` & `openbb_equity-1.2.1/openbb_equity/darkpool/darkpool_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/discovery/discovery_router.py` & `openbb_equity-1.2.1/openbb_equity/discovery/discovery_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/equity_router.py` & `openbb_equity-1.2.1/openbb_equity/equity_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/estimates/estimates_router.py` & `openbb_equity-1.2.1/openbb_equity/estimates/estimates_router.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,14 +113,44 @@
     extra_params: ExtraParams,
 ) -> OBBject:
     """Get forward sales estimates."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
+    model="ForwardEbitdaEstimates",
+    examples=[
+        APIEx(parameters={"provider": "intrinio"}),
+        APIEx(
+            parameters={
+                "symbol": "AAPL",
+                "fiscal_period": "annual",
+                "provider": "intrinio",
+            }
+        ),
+        APIEx(
+            parameters={
+                "symbol": "AAPL,MSFT",
+                "fiscal_period": "quarter",
+                "provider": "fmp",
+            }
+        ),
+    ],
+)
+async def forward_ebitda(
+    cc: CommandContext,
+    provider_choices: ProviderChoices,
+    standard_params: StandardParams,
+    extra_params: ExtraParams,
+) -> OBBject:
+    """Get forward EBITDA estimates."""
+    return await OBBject.from_query(Query(**locals()))
+
+
+@router.command(
     model="ForwardEpsEstimates",
     examples=[
         APIEx(parameters={"symbol": "AAPL", "provider": "intrinio"}),
         APIEx(
             parameters={
                 "fiscal_year": 2025,
                 "fiscal_period": "fy",
```

### Comparing `openbb_equity-1.2.0/openbb_equity/fundamental/fundamental_router.py` & `openbb_equity-1.2.1/openbb_equity/fundamental/fundamental_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/ownership/ownership_router.py` & `openbb_equity-1.2.1/openbb_equity/ownership/ownership_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/price/price_router.py` & `openbb_equity-1.2.1/openbb_equity/price/price_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/openbb_equity/shorts/shorts_router.py` & `openbb_equity-1.2.1/openbb_equity/shorts/shorts_router.py`

 * *Files identical despite different names*

### Comparing `openbb_equity-1.2.0/PKG-INFO` & `openbb_equity-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-equity
-Version: 1.2.0
+Version: 1.2.1
 Summary: Equity extension for OpenBB
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
 
 # OpenBB Equity Extension
 
 This extension provides equity market data tools for the OpenBB Platform.
 
 Features of the Equity extension include:
```

