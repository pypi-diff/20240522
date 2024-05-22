# Comparing `tmp/openbb_derivatives-1.2.0.tar.gz` & `tmp/openbb_derivatives-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_derivatives-1.2.0.tar", max compression
+gzip compressed data, was "openbb_derivatives-1.2.1.tar", max compression
```

## Comparing `openbb_derivatives-1.2.0.tar` & `openbb_derivatives-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      289 2024-05-15 14:23:09.824094 openbb_derivatives-1.2.0/README.md
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.731747 openbb_derivatives-1.2.0/openbb_derivatives/__init__.py
--rw-r--r--   0        0        0      372 2024-04-23 10:22:39.595836 openbb_derivatives-1.2.0/openbb_derivatives/derivatives_router.py
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.731881 openbb_derivatives-1.2.0/openbb_derivatives/futures/__init__.py
--rw-r--r--   0        0        0     1846 2024-04-08 16:55:49.545455 openbb_derivatives-1.2.0/openbb_derivatives/futures/futures_router.py
--rw-r--r--   0        0        0       15 2024-02-29 11:03:36.732008 openbb_derivatives-1.2.0/openbb_derivatives/options/__init__.py
--rw-r--r--   0        0        0     1692 2024-04-08 16:46:02.628100 openbb_derivatives-1.2.0/openbb_derivatives/options/options_router.py
--rw-r--r--   0        0        0      508 2024-05-15 16:04:03.158775 openbb_derivatives-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 openbb_derivatives-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      289 2024-05-22 11:48:40.399330 openbb_derivatives-1.2.1/README.md
+-rw-r--r--   0        0        0       15 2024-05-14 16:56:41.557863 openbb_derivatives-1.2.1/openbb_derivatives/__init__.py
+-rw-r--r--   0        0        0      372 2024-05-14 16:56:41.557863 openbb_derivatives-1.2.1/openbb_derivatives/derivatives_router.py
+-rw-r--r--   0        0        0       15 2024-05-14 16:56:41.557863 openbb_derivatives-1.2.1/openbb_derivatives/futures/__init__.py
+-rw-r--r--   0        0        0     1846 2024-05-14 16:56:41.557863 openbb_derivatives-1.2.1/openbb_derivatives/futures/futures_router.py
+-rw-r--r--   0        0        0       15 2024-05-14 16:56:41.557863 openbb_derivatives-1.2.1/openbb_derivatives/options/__init__.py
+-rw-r--r--   0        0        0     1710 2024-05-22 13:43:02.476925 openbb_derivatives-1.2.1/openbb_derivatives/options/options_router.py
+-rw-r--r--   0        0        0      508 2024-05-22 13:54:51.543346 openbb_derivatives-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      957 1970-01-01 00:00:00.000000 openbb_derivatives-1.2.1/PKG-INFO
```

### Comparing `openbb_derivatives-1.2.0/openbb_derivatives/futures/futures_router.py` & `openbb_derivatives-1.2.1/openbb_derivatives/futures/futures_router.py`

 * *Files identical despite different names*

### Comparing `openbb_derivatives-1.2.0/openbb_derivatives/options/options_router.py` & `openbb_derivatives-1.2.1/openbb_derivatives/options/options_router.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     """Get the complete options chain for a ticker."""
     return await OBBject.from_query(Query(**locals()))
 
 
 @router.command(
     model="OptionsUnusual",
     examples=[
-        APIEx(parameters={"provider": "intrinio"}),
+        APIEx(parameters={"symbol": "TSLA", "provider": "intrinio"}),
         APIEx(
             description="Use the 'symbol' parameter to get the most recent activity for a specific symbol.",
             parameters={"symbol": "TSLA", "provider": "intrinio"},
         ),
     ],
 )
 async def unusual(
```

### Comparing `openbb_derivatives-1.2.0/PKG-INFO` & `openbb_derivatives-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-derivatives
-Version: 1.2.0
+Version: 1.2.1
 Summary: Derivatives extension for OpenBB
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
 
 # OpenBB Derivatives Extension
 
 This extension provides derivatives data for the OpenBB Platform.
 
 ## Installation
```

