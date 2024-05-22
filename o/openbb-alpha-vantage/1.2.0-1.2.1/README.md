# Comparing `tmp/openbb_alpha_vantage-1.2.0.tar.gz` & `tmp/openbb_alpha_vantage-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_alpha_vantage-1.2.0.tar", max compression
+gzip compressed data, was "openbb_alpha_vantage-1.2.1.tar", max compression
```

## Comparing `openbb_alpha_vantage-1.2.0.tar` & `openbb_alpha_vantage-1.2.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      330 2024-05-15 14:26:22.821035 openbb_alpha_vantage-1.2.0/README.md
--rw-r--r--   0        0        0     1452 2024-05-10 19:27:56.005744 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/__init__.py
--rw-r--r--   0        0        0       28 2024-04-23 10:22:39.651445 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/__init__.py
--rw-r--r--   0        0        0    12458 2024-05-10 10:40:27.289046 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/equity_historical.py
--rw-r--r--   0        0        0     5594 2024-05-14 15:30:05.609782 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/historical_eps.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.752779 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/py.typed
--rw-r--r--   0        0        0       31 2024-04-23 10:22:39.651694 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/__init__.py
--rw-r--r--   0        0        0     2511 2024-04-23 10:22:39.651812 openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/helpers.py
--rw-r--r--   0        0        0      519 2024-05-15 16:06:25.928312 openbb_alpha_vantage-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      330 2024-05-22 11:48:40.463330 openbb_alpha_vantage-1.2.1/README.md
+-rw-r--r--   0        0        0     1452 2024-05-15 09:21:56.057885 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-14 16:56:41.669864 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/models/__init__.py
+-rw-r--r--   0        0        0    12458 2024-05-15 09:21:56.057885 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/models/equity_historical.py
+-rw-r--r--   0        0        0     5610 2024-05-22 11:48:40.463330 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/models/historical_eps.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.669864 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/py.typed
+-rw-r--r--   0        0        0       31 2024-05-14 16:56:41.669864 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/utils/__init__.py
+-rw-r--r--   0        0        0     2511 2024-05-14 16:56:41.669864 openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/utils/helpers.py
+-rw-r--r--   0        0        0      519 2024-05-22 13:57:56.487959 openbb_alpha_vantage-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 openbb_alpha_vantage-1.2.1/PKG-INFO
```

### Comparing `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/__init__.py` & `openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/equity_historical.py` & `openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/models/equity_historical.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/models/historical_eps.py` & `openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/models/historical_eps.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         async def response_callback(response: ClientResponse, _: ClientSession):
             """Response callback function."""
             symbol = response.url.query.get("symbol", None)
             data = await response.json()
             target = (
                 "annualEarnings" if query.period == "annual" else "quarterlyEarnings"
             )
-            message = data.get("Information", "")
+            message = data.get("Information", "")  # type: ignore
             if message:
                 messages.append(message)
                 warn(f"Symbol Error for {symbol}: {message}")
             result: List = []
             # If data is returned, append it to the results list.
             if data:
                 result = [
```

### Comparing `openbb_alpha_vantage-1.2.0/openbb_alpha_vantage/utils/helpers.py` & `openbb_alpha_vantage-1.2.1/openbb_alpha_vantage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_alpha_vantage-1.2.0/pyproject.toml` & `openbb_alpha_vantage-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-alpha-vantage"
-version = "1.2.0"
+version = "1.2.1"
 description = "Alpha Vantage extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_alpha_vantage" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 alpha_vantage = "openbb_alpha_vantage:alpha_vantage_provider"
```

### Comparing `openbb_alpha_vantage-1.2.0/PKG-INFO` & `openbb_alpha_vantage-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-alpha-vantage
-Version: 1.2.0
+Version: 1.2.1
 Summary: Alpha Vantage extension for OpenBB
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
 
 # OpenBB Alpha Vantage Provider
 
 This extension integrates the [Alpha Vantage](https://www.alphavantage.co/) data provider into the OpenBB Platform.
 
 ## Installation
```

