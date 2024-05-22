# Comparing `tmp/openbb_nasdaq-1.2.0.tar.gz` & `tmp/openbb_nasdaq-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_nasdaq-1.2.0.tar", max compression
+gzip compressed data, was "openbb_nasdaq-1.2.1.tar", max compression
```

## Comparing `openbb_nasdaq-1.2.0.tar` & `openbb_nasdaq-1.2.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      303 2024-05-15 14:25:19.879856 openbb_nasdaq-1.2.0/README.md
--rw-r--r--   0        0        0     2484 2024-05-14 15:30:05.617274 openbb_nasdaq-1.2.0/openbb_nasdaq/__init__.py
--rw-r--r--   0        0        0       35 2024-04-23 10:22:39.674899 openbb_nasdaq-1.2.0/openbb_nasdaq/models/__init__.py
--rw-r--r--   0        0        0     3987 2024-04-23 10:22:39.675013 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_dividend.py
--rw-r--r--   0        0        0     6330 2024-04-23 10:22:39.675292 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_earnings.py
--rw-r--r--   0        0        0     6656 2024-04-02 11:35:59.494640 openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_ipo.py
--rw-r--r--   0        0        0     6111 2024-04-23 10:22:39.675428 openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot.py
--rw-r--r--   0        0        0     2274 2024-04-23 10:22:39.675550 openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot_search.py
--rw-r--r--   0        0        0     5111 2024-05-10 10:40:27.299762 openbb_nasdaq-1.2.0/openbb_nasdaq/models/economic_calendar.py
--rw-r--r--   0        0        0     5043 2024-04-08 12:02:16.661594 openbb_nasdaq-1.2.0/openbb_nasdaq/models/equity_search.py
--rw-r--r--   0        0        0     5163 2024-05-10 10:40:27.300096 openbb_nasdaq-1.2.0/openbb_nasdaq/models/historical_dividends.py
--rw-r--r--   0        0        0     2437 2024-04-08 12:02:16.661718 openbb_nasdaq-1.2.0/openbb_nasdaq/models/lbma_fixing.py
--rw-r--r--   0        0        0     2749 2024-04-08 12:02:16.661815 openbb_nasdaq-1.2.0/openbb_nasdaq/models/sp500_multiples.py
--rw-r--r--   0        0        0     2590 2024-04-08 12:02:16.661906 openbb_nasdaq-1.2.0/openbb_nasdaq/models/top_retail.py
--rw-r--r--   0        0        0        0 2024-04-02 11:35:59.495686 openbb_nasdaq-1.2.0/openbb_nasdaq/py.typed
--rw-r--r--   0        0        0       29 2024-04-23 10:22:39.675762 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/__init__.py
--rw-r--r--   0        0        0     4220 2024-02-29 11:03:36.881453 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/helpers.py
--rw-r--r--   0        0        0     1053 2024-04-08 12:02:16.661991 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/query_params.py
--rw-r--r--   0        0        0    48642 2024-04-08 12:02:16.662176 openbb_nasdaq-1.2.0/openbb_nasdaq/utils/series_ids.py
--rw-r--r--   0        0        0      534 2024-05-15 16:05:35.015231 openbb_nasdaq-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 openbb_nasdaq-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      303 2024-05-22 11:48:40.539330 openbb_nasdaq-1.2.1/README.md
+-rw-r--r--   0        0        0     2484 2024-05-15 09:21:56.085885 openbb_nasdaq-1.2.1/openbb_nasdaq/__init__.py
+-rw-r--r--   0        0        0       35 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/__init__.py
+-rw-r--r--   0        0        0     3987 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_dividend.py
+-rw-r--r--   0        0        0     6330 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_earnings.py
+-rw-r--r--   0        0        0     6634 2024-05-22 11:48:40.539330 openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_ipo.py
+-rw-r--r--   0        0        0     6111 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/cot.py
+-rw-r--r--   0        0        0     2274 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/cot_search.py
+-rw-r--r--   0        0        0     5111 2024-05-15 09:21:56.085885 openbb_nasdaq-1.2.1/openbb_nasdaq/models/economic_calendar.py
+-rw-r--r--   0        0        0     5043 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/equity_search.py
+-rw-r--r--   0        0        0     5163 2024-05-15 09:21:56.085885 openbb_nasdaq-1.2.1/openbb_nasdaq/models/historical_dividends.py
+-rw-r--r--   0        0        0     2437 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/lbma_fixing.py
+-rw-r--r--   0        0        0     2749 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/sp500_multiples.py
+-rw-r--r--   0        0        0     2590 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/models/top_retail.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/py.typed
+-rw-r--r--   0        0        0       29 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/utils/__init__.py
+-rw-r--r--   0        0        0     4220 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/utils/helpers.py
+-rw-r--r--   0        0        0     1053 2024-05-14 16:56:41.921865 openbb_nasdaq-1.2.1/openbb_nasdaq/utils/query_params.py
+-rw-r--r--   0        0        0    48642 2024-05-14 16:56:41.925865 openbb_nasdaq-1.2.1/openbb_nasdaq/utils/series_ids.py
+-rw-r--r--   0        0        0      534 2024-05-22 13:56:36.423694 openbb_nasdaq-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1060 1970-01-01 00:00:00.000000 openbb_nasdaq-1.2.1/PKG-INFO
```

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/__init__.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_dividend.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_dividend.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_earnings.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_earnings.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/calendar_ipo.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/calendar_ipo.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,15 +157,15 @@
             response: List[Dict[Any, Any]] = [{}]
             url = (
                 f"https://api.nasdaq.com/api/ipo/calendar?date={date}"
                 if query.is_spo is False
                 else f"https://api.nasdaq.com/api/ipo/calendar?type=spo&date={date}"
             )
             r = requests.get(url, headers=IPO_HEADERS, timeout=5)
-            r_json = r.json()["data"] if "data" in r.json() else {}
+            r_json = r.json().get("data", {})
             if query.status in r_json:
                 response = (
                     r_json["upcoming"]["upcomingTable"]["rows"]
                     if query.status == "upcoming"
                     else r_json[query.status]["rows"]
                 )
             if response is not None:
```

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/cot.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/cot_search.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/cot_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/economic_calendar.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/economic_calendar.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/equity_search.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/equity_search.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/historical_dividends.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/historical_dividends.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/lbma_fixing.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/lbma_fixing.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/sp500_multiples.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/sp500_multiples.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/models/top_retail.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/models/top_retail.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/helpers.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/query_params.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/utils/query_params.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/openbb_nasdaq/utils/series_ids.py` & `openbb_nasdaq-1.2.1/openbb_nasdaq/utils/series_ids.py`

 * *Files identical despite different names*

### Comparing `openbb_nasdaq-1.2.0/pyproject.toml` & `openbb_nasdaq-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-nasdaq"
-version = "1.2.0"
+version = "1.2.1"
 description = "Nasdaq extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_nasdaq" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 random-user-agent = "^1.0.1"
 nasdaq-data-link = "^1.0.4"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `openbb_nasdaq-1.2.0/PKG-INFO` & `openbb_nasdaq-1.2.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-nasdaq
-Version: 1.2.0
+Version: 1.2.1
 Summary: Nasdaq extension for OpenBB
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
 Requires-Dist: nasdaq-data-link (>=1.0.4,<2.0.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Nasdaq Provider
 
 This extension integrates the [Nasdaq](https://www.nasdaq.com) data provider into the OpenBB Platform.
```

