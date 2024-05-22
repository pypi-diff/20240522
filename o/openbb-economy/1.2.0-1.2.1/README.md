# Comparing `tmp/openbb_economy-1.2.0.tar.gz` & `tmp/openbb_economy-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_economy-1.2.0.tar", max compression
+gzip compressed data, was "openbb_economy-1.2.1.tar", max compression
```

## Comparing `openbb_economy-1.2.0.tar` & `openbb_economy-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      334 2024-05-15 14:27:51.744569 openbb_economy-1.2.0/README.md
--rw-r--r--   0        0        0       32 2024-04-23 10:22:39.599846 openbb_economy-1.2.0/openbb_economy/__init__.py
--rw-r--r--   0        0        0    12007 2024-05-09 15:04:29.063912 openbb_economy-1.2.0/openbb_economy/economy_router.py
--rw-r--r--   0        0        0     1754 2024-04-23 10:22:39.600176 openbb_economy-1.2.0/openbb_economy/gdp/gdp_router.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.734317 openbb_economy-1.2.0/openbb_economy/py.typed
--rw-r--r--   0        0        0      484 2024-05-15 16:03:57.437693 openbb_economy-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 openbb_economy-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      334 2024-05-22 11:48:40.403330 openbb_economy-1.2.1/README.md
+-rw-r--r--   0        0        0       32 2024-05-14 16:56:41.561863 openbb_economy-1.2.1/openbb_economy/__init__.py
+-rw-r--r--   0        0        0    12124 2024-05-22 11:48:40.403330 openbb_economy-1.2.1/openbb_economy/economy_router.py
+-rw-r--r--   0        0        0     1754 2024-05-14 16:56:41.561863 openbb_economy-1.2.1/openbb_economy/gdp/gdp_router.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.561863 openbb_economy-1.2.1/openbb_economy/py.typed
+-rw-r--r--   0        0        0      484 2024-05-22 13:55:36.803497 openbb_economy-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      994 1970-01-01 00:00:00.000000 openbb_economy-1.2.1/PKG-INFO
```

### Comparing `openbb_economy-1.2.0/openbb_economy/economy_router.py` & `openbb_economy-1.2.1/openbb_economy/economy_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,14 +89,16 @@
     """Get Market Risk Premium by country."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="BalanceOfPayments",
     examples=[
+        APIEx(parameters={"provider": "fred"}),
+        APIEx(parameters={"provider": "fred", "country": "brazil"}),
         APIEx(parameters={"provider": "ecb"}),
         APIEx(parameters={"report_type": "summary", "provider": "ecb"}),
         APIEx(
             description="The `country` parameter will override the `report_type`.",
             parameters={"country": "united_states", "provider": "ecb"},
         ),
     ],
```

### Comparing `openbb_economy-1.2.0/openbb_economy/gdp/gdp_router.py` & `openbb_economy-1.2.1/openbb_economy/gdp/gdp_router.py`

 * *Files identical despite different names*

### Comparing `openbb_economy-1.2.0/PKG-INFO` & `openbb_economy-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-economy
-Version: 1.2.0
+Version: 1.2.1
 Summary: Economy extension for OpenBB
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
 
 # OpenBB Economy Extension
 
 The Economy extension provides global macroeconomic data access for the OpenBB Platform.
 
 ## Installation
```

