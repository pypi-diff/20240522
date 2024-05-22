# Comparing `tmp/openbb_government_us-1.2.0.tar.gz` & `tmp/openbb_government_us-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_government_us-1.2.0.tar", max compression
+gzip compressed data, was "openbb_government_us-1.2.1.tar", max compression
```

## Comparing `openbb_government_us-1.2.0.tar` & `openbb_government_us-1.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      318 2024-05-15 14:25:32.440933 openbb_government_us-1.2.0/README.md
--rw-r--r--   0        0        0      976 2024-05-14 15:30:05.616106 openbb_government_us-1.2.0/openbb_government_us/__init__.py
--rw-r--r--   0        0        0       24 2024-02-29 11:03:36.873377 openbb_government_us-1.2.0/openbb_government_us/models/__init__.py
--rw-r--r--   0        0        0     2724 2024-04-08 12:02:16.650213 openbb_government_us-1.2.0/openbb_government_us/models/treasury_auctions.py
--rw-r--r--   0        0        0     5138 2024-05-09 13:34:29.221479 openbb_government_us-1.2.0/openbb_government_us/models/treasury_prices.py
--rw-r--r--   0        0        0       34 2024-04-23 10:22:39.670563 openbb_government_us-1.2.0/openbb_government_us/utils/__init__.py
--rw-r--r--   0        0        0      296 2024-04-02 11:35:59.475353 openbb_government_us-1.2.0/openbb_government_us/utils/helpers.py
--rw-r--r--   0        0        0      548 2024-05-15 16:06:14.659267 openbb_government_us-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 openbb_government_us-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      318 2024-05-22 11:48:40.535330 openbb_government_us-1.2.1/README.md
+-rw-r--r--   0        0        0      976 2024-05-15 09:21:56.081885 openbb_government_us-1.2.1/openbb_government_us/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-14 16:56:41.901865 openbb_government_us-1.2.1/openbb_government_us/models/__init__.py
+-rw-r--r--   0        0        0     2724 2024-05-14 16:56:41.901865 openbb_government_us-1.2.1/openbb_government_us/models/treasury_auctions.py
+-rw-r--r--   0        0        0     5138 2024-05-14 16:57:23.590032 openbb_government_us-1.2.1/openbb_government_us/models/treasury_prices.py
+-rw-r--r--   0        0        0       34 2024-05-14 16:56:41.901865 openbb_government_us-1.2.1/openbb_government_us/utils/__init__.py
+-rw-r--r--   0        0        0      296 2024-05-14 16:56:41.901865 openbb_government_us-1.2.1/openbb_government_us/utils/helpers.py
+-rw-r--r--   0        0        0      548 2024-05-22 13:56:25.771659 openbb_government_us-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1040 1970-01-01 00:00:00.000000 openbb_government_us-1.2.1/PKG-INFO
```

### Comparing `openbb_government_us-1.2.0/openbb_government_us/__init__.py` & `openbb_government_us-1.2.1/openbb_government_us/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.2.0/openbb_government_us/models/treasury_auctions.py` & `openbb_government_us-1.2.1/openbb_government_us/models/treasury_auctions.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.2.0/openbb_government_us/models/treasury_prices.py` & `openbb_government_us-1.2.1/openbb_government_us/models/treasury_prices.py`

 * *Files identical despite different names*

### Comparing `openbb_government_us-1.2.0/pyproject.toml` & `openbb_government_us-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "openbb-government-us"
-version = "1.2.0"
+version = "1.2.1"
 description = "US Government Data Extension for OpenBB"
 authors = ["OpenBB <hello@openbb.co>"]
 license = "AGPL-3.0-only"
 readme = "README.md"
 packages = [{ include = "openbb_government_us" }]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-openbb-core = "^1.2.1"
+openbb-core = "^1.2.3"
 random-user-agent = "^1.0.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.plugins."openbb_provider_extension"]
```

### Comparing `openbb_government_us-1.2.0/PKG-INFO` & `openbb_government_us-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: openbb-government-us
-Version: 1.2.0
+Version: 1.2.1
 Summary: US Government Data Extension for OpenBB
 License: AGPL-3.0-only
 Author: OpenBB
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
 Requires-Dist: random-user-agent (>=1.0.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # OpenBB Government US Provider
 
 This extension integrates the [US Government](https://data.gov) data provider into the OpenBB Platform.
```

