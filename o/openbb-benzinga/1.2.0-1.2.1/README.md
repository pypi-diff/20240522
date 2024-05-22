# Comparing `tmp/openbb_benzinga-1.2.0.tar.gz` & `tmp/openbb_benzinga-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_benzinga-1.2.0.tar", max compression
+gzip compressed data, was "openbb_benzinga-1.2.1.tar", max compression
```

## Comparing `openbb_benzinga-1.2.0.tar` & `openbb_benzinga-1.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      312 2024-05-15 14:21:47.631780 openbb_benzinga-1.2.0/README.md
--rw-r--r--   0        0        0      898 2024-05-14 15:30:05.610153 openbb_benzinga-1.2.0/openbb_benzinga/__init__.py
--rw-r--r--   0        0        0       32 2024-04-23 10:22:39.652736 openbb_benzinga-1.2.0/openbb_benzinga/models/__init__.py
--rw-r--r--   0        0        0    18109 2024-05-10 10:40:27.289939 openbb_benzinga-1.2.0/openbb_benzinga/models/analyst_search.py
--rw-r--r--   0        0        0     6206 2024-05-10 10:40:27.290127 openbb_benzinga-1.2.0/openbb_benzinga/models/company_news.py
--rw-r--r--   0        0        0     9807 2024-05-10 10:40:27.290287 openbb_benzinga-1.2.0/openbb_benzinga/models/price_target.py
--rw-r--r--   0        0        0     5809 2024-04-08 12:02:16.579354 openbb_benzinga-1.2.0/openbb_benzinga/models/world_news.py
--rw-r--r--   0        0        0        0 2024-02-29 11:03:36.754477 openbb_benzinga-1.2.0/openbb_benzinga/py.typed
--rw-r--r--   0        0        0       31 2024-04-23 10:22:39.653147 openbb_benzinga-1.2.0/openbb_benzinga/utils/__init__.py
--rw-r--r--   0        0        0      489 2024-05-15 16:07:32.771241 openbb_benzinga-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 openbb_benzinga-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      312 2024-05-22 11:48:40.467330 openbb_benzinga-1.2.1/README.md
+-rw-r--r--   0        0        0      898 2024-05-15 09:21:56.057885 openbb_benzinga-1.2.1/openbb_benzinga/__init__.py
+-rw-r--r--   0        0        0       32 2024-05-14 16:56:41.673864 openbb_benzinga-1.2.1/openbb_benzinga/models/__init__.py
+-rw-r--r--   0        0        0    18109 2024-05-15 09:21:56.057885 openbb_benzinga-1.2.1/openbb_benzinga/models/analyst_search.py
+-rw-r--r--   0        0        0     6206 2024-05-15 09:21:56.057885 openbb_benzinga-1.2.1/openbb_benzinga/models/company_news.py
+-rw-r--r--   0        0        0    10009 2024-05-22 11:48:40.467330 openbb_benzinga-1.2.1/openbb_benzinga/models/price_target.py
+-rw-r--r--   0        0        0     5809 2024-05-14 16:56:41.673864 openbb_benzinga-1.2.1/openbb_benzinga/models/world_news.py
+-rw-r--r--   0        0        0        0 2024-05-14 16:56:41.673864 openbb_benzinga-1.2.1/openbb_benzinga/py.typed
+-rw-r--r--   0        0        0       31 2024-05-14 16:56:41.673864 openbb_benzinga-1.2.1/openbb_benzinga/utils/__init__.py
+-rw-r--r--   0        0        0      489 2024-05-22 13:56:10.759609 openbb_benzinga-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      974 1970-01-01 00:00:00.000000 openbb_benzinga-1.2.1/PKG-INFO
```

### Comparing `openbb_benzinga-1.2.0/openbb_benzinga/__init__.py` & `openbb_benzinga-1.2.1/openbb_benzinga/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.2.0/openbb_benzinga/models/analyst_search.py` & `openbb_benzinga-1.2.1/openbb_benzinga/models/analyst_search.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.2.0/openbb_benzinga/models/company_news.py` & `openbb_benzinga-1.2.1/openbb_benzinga/models/company_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.2.0/openbb_benzinga/models/price_target.py` & `openbb_benzinga-1.2.1/openbb_benzinga/models/price_target.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,51 +44,59 @@
 
     Source: https://docs.benzinga.io/benzinga-apis/calendar/get-ratings
     """
 
     __alias_dict__ = {
         "limit": "pagesize",
         "symbol": "parameters[tickers]",
+        "date": "parameters[date]",
+        "start_date": "parameters[date_from]",
+        "end_date": "parameters[date_to]",
+        "updated": "parameters[updated]",
+        "importance": "parameters[importance]",
+        "action": "parameters[action]",
+        "analyst_ids": "parameters[analyst_id]",
+        "firm_ids": "parameters[firm_id]",
+    }
+    __json_schema_extra__ = {
+        "symbol": ["multiple_items_allowed"],
+        "analyst_ids": ["multiple_items_allowed"],
+        "firm_ids": ["multiple_items_allowed"],
+        "fields": ["multiple_items_allowed"],
     }
-    __json_schema_extra__ = {"symbol": {"multiple_items_allowed": True}}
 
     page: Optional[int] = Field(
         default=0,
         description="Page offset. For optimization, performance and technical reasons,"
         + " page offsets are limited from 0 - 100000. Limit the query results by other parameters such as date."
         + " Used in conjunction with the limit and date parameters.",
     )
     date: Optional[dateType] = Field(
         default=None,
         description="Date for calendar data, shorthand for date_from and date_to.",
-        alias="parameters[date]",
     )
     start_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("start_date", ""),
-        alias="parameters[date_from]",
     )
     end_date: Optional[dateType] = Field(
         default=None,
         description=QUERY_DESCRIPTIONS.get("end_date", ""),
-        alias="parameters[date_to]",
     )
     updated: Optional[Union[dateType, int]] = Field(
         default=None,
         description="Records last Updated Unix timestamp (UTC)."
         + " This will force the sort order to be Greater Than or Equal to the timestamp indicated."
         + " The date can be a date string or a Unix timestamp."
         + " The date string must be in the format of YYYY-MM-DD.",
-        alias="parameters[updated]",
     )
     importance: Optional[int] = Field(
         default=None,
         description="Importance level to filter by."
         + " Uses Greater Than or Equal To the importance indicated",
-        alias="parameters[importance]",
     )
     action: Optional[
         Literal[
             "downgrades",
             "maintains",
             "reinstates",
             "reiterates",
@@ -99,26 +107,23 @@
             "removes",
             "suspends",
             "firm_dissolved",
         ]
     ] = Field(
         default=None,
         description="Filter by a specific action_company.",
-        alias="parameters[action]",
     )
     analyst_ids: Optional[Union[List[str], str]] = Field(
         default=None,
         description="Comma-separated list of analyst (person) IDs."
         + " Omitting will bring back all available analysts.",
-        alias="parameters[analyst_id]",
     )
     firm_ids: Optional[Union[List[str], str]] = Field(
         default=None,
         description="Comma-separated list of firm IDs.",
-        alias="parameters[firm_id]",
     )
     fields: Optional[Union[List[str], str]] = Field(
         default=None,
         description="Comma-separated list of fields to include in the response."
         " See https://docs.benzinga.io/benzinga-apis/calendar/get-ratings to learn about the available fields.",
     )
```

### Comparing `openbb_benzinga-1.2.0/openbb_benzinga/models/world_news.py` & `openbb_benzinga-1.2.1/openbb_benzinga/models/world_news.py`

 * *Files identical despite different names*

### Comparing `openbb_benzinga-1.2.0/PKG-INFO` & `openbb_benzinga-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-benzinga
-Version: 1.2.0
+Version: 1.2.1
 Summary: Benzinga extension for OpenBB
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
 
 # OpenBB Benzinga Provider
 
 This extension integrates the [Benzinga](https://www.benzinga.com/) data provider into the OpenBB Platform.
 
 ## Installation
```

