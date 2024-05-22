# Comparing `tmp/openbb_tradingeconomics-1.2.0.tar.gz` & `tmp/openbb_tradingeconomics-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_tradingeconomics-1.2.0.tar", max compression
+gzip compressed data, was "openbb_tradingeconomics-1.2.1.tar", max compression
```

## Comparing `openbb_tradingeconomics-1.2.0.tar` & `openbb_tradingeconomics-1.2.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      342 2024-05-15 14:24:32.425446 openbb_tradingeconomics-1.2.0/README.md
--rw-r--r--   0        0        0      944 2024-05-14 15:30:05.620721 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/__init__.py
--rw-r--r--   0        0        0     8326 2024-05-15 12:02:12.290758 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/models/economic_calendar.py
--rw-r--r--   0        0        0     4616 2024-04-23 10:22:39.799520 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/countries.py
--rw-r--r--   0        0        0     4104 2024-05-14 15:30:05.621205 openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/url_generator.py
--rw-r--r--   0        0        0      538 2024-05-15 16:07:37.861279 openbb_tradingeconomics-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      342 2024-05-22 11:48:40.551330 openbb_tradingeconomics-1.2.1/README.md
+-rw-r--r--   0        0        0      944 2024-05-15 09:21:56.105885 openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/__init__.py
+-rw-r--r--   0        0        0     8320 2024-05-22 11:48:40.551330 openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/models/economic_calendar.py
+-rw-r--r--   0        0        0     4616 2024-05-14 16:56:42.341866 openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/utils/countries.py
+-rw-r--r--   0        0        0     4104 2024-05-15 09:21:56.105885 openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/utils/url_generator.py
+-rw-r--r--   0        0        0      538 2024-05-22 13:56:15.627626 openbb_tradingeconomics-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1021 1970-01-01 00:00:00.000000 openbb_tradingeconomics-1.2.1/PKG-INFO
```

### Comparing `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/__init__.py` & `openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/models/economic_calendar.py` & `openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/models/economic_calendar.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
     )
 
     @field_validator("importance", mode="before", check_fields=False)
     @classmethod
     def importance_to_number(cls, v):
         """Convert importance to number."""
         value_to_string = {1: "Low", 2: "Medium", 3: "High"}
-        return value_to_string.get(v, None) if v else None
+        return value_to_string.get(v) if v else None
 
     @field_validator("date", "last_updated", mode="before", check_fields=False)
     @classmethod
     def validate_datetime(cls, v: str) -> datetime:
         """Validate the datetime values."""
         dt = to_datetime(v, utc=True)
         return dt.replace(microsecond=0)
```

### Comparing `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/countries.py` & `openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/utils/countries.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.2.0/openbb_tradingeconomics/utils/url_generator.py` & `openbb_tradingeconomics-1.2.1/openbb_tradingeconomics/utils/url_generator.py`

 * *Files identical despite different names*

### Comparing `openbb_tradingeconomics-1.2.0/pyproject.toml` & `openbb_tradingeconomics-1.2.1/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-tradingeconomics"
-version = "1.2.0"
+version = "1.2.1"
 description = "Trading Economics extension for OpenBB"
 authors = ["OpenBB Team <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_tradingeconomics" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
 tradingeconomics = "openbb_tradingeconomics:tradingeconomics_provider"
```

### Comparing `openbb_tradingeconomics-1.2.0/PKG-INFO` & `openbb_tradingeconomics-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-tradingeconomics
-Version: 1.2.0
+Version: 1.2.1
 Summary: Trading Economics extension for OpenBB
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
 
 # OpenBB Trading Economics Provider
 
 This extension integrates the [Trading Economics](https://docs.tradingeconomics.com/) data provider into the OpenBB SDK.
 
 ## Installation
```

