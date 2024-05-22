# Comparing `tmp/openbb_oecd-1.2.0.tar.gz` & `tmp/openbb_oecd-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openbb_oecd-1.2.0.tar", max compression
+gzip compressed data, was "openbb_oecd-1.2.1.tar", max compression
```

## Comparing `openbb_oecd-1.2.0.tar` & `openbb_oecd-1.2.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      297 2024-05-15 14:29:02.754868 openbb_oecd-1.2.0/README.md
--rw-r--r--   0        0        0     1145 2024-05-14 15:30:05.617681 openbb_oecd-1.2.0/openbb_oecd/__init__.py
--rw-r--r--   0        0        0     4658 2024-04-08 12:02:16.665635 openbb_oecd-1.2.0/openbb_oecd/models/composite_leading_indicator.py
--rw-r--r--   0        0        0     4292 2024-04-08 12:02:16.665758 openbb_oecd-1.2.0/openbb_oecd/models/gdp_forecast.py
--rw-r--r--   0        0        0     3725 2024-04-08 12:02:16.665882 openbb_oecd-1.2.0/openbb_oecd/models/gdp_nominal.py
--rw-r--r--   0        0        0     3920 2024-04-08 12:02:16.665998 openbb_oecd-1.2.0/openbb_oecd/models/gdp_real.py
--rw-r--r--   0        0        0     4952 2024-04-08 12:02:16.666084 openbb_oecd-1.2.0/openbb_oecd/models/long_term_interest_rate.py
--rw-r--r--   0        0        0     4960 2024-04-08 12:02:16.666136 openbb_oecd-1.2.0/openbb_oecd/models/short_term_interest_rate.py
--rw-r--r--   0        0        0     6141 2024-04-08 12:02:16.666230 openbb_oecd-1.2.0/openbb_oecd/models/unemployment.py
--rw-r--r--   0        0        0    13133 2024-04-08 12:02:16.666349 openbb_oecd-1.2.0/openbb_oecd/utils/constants.py
--rw-r--r--   0        0        0     8810 2024-04-23 10:22:39.676912 openbb_oecd-1.2.0/openbb_oecd/utils/helpers.py
--rw-r--r--   0        0        0      511 2024-05-15 16:06:20.543758 openbb_oecd-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_oecd-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      297 2024-05-22 11:48:40.539330 openbb_oecd-1.2.1/README.md
+-rw-r--r--   0        0        0     1145 2024-05-15 09:21:56.085885 openbb_oecd-1.2.1/openbb_oecd/__init__.py
+-rw-r--r--   0        0        0     4658 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/composite_leading_indicator.py
+-rw-r--r--   0        0        0     4292 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/gdp_forecast.py
+-rw-r--r--   0        0        0     3725 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/gdp_nominal.py
+-rw-r--r--   0        0        0     3920 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/gdp_real.py
+-rw-r--r--   0        0        0     4952 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/long_term_interest_rate.py
+-rw-r--r--   0        0        0     4960 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/short_term_interest_rate.py
+-rw-r--r--   0        0        0     6141 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/models/unemployment.py
+-rw-r--r--   0        0        0    13133 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/utils/constants.py
+-rw-r--r--   0        0        0     8810 2024-05-14 16:56:41.933865 openbb_oecd-1.2.1/openbb_oecd/utils/helpers.py
+-rw-r--r--   0        0        0      511 2024-05-22 13:57:03.735785 openbb_oecd-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1031 1970-01-01 00:00:00.000000 openbb_oecd-1.2.1/PKG-INFO
```

### Comparing `openbb_oecd-1.2.0/openbb_oecd/__init__.py` & `openbb_oecd-1.2.1/openbb_oecd/__init__.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/composite_leading_indicator.py` & `openbb_oecd-1.2.1/openbb_oecd/models/composite_leading_indicator.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/gdp_forecast.py` & `openbb_oecd-1.2.1/openbb_oecd/models/gdp_forecast.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/gdp_nominal.py` & `openbb_oecd-1.2.1/openbb_oecd/models/gdp_nominal.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/gdp_real.py` & `openbb_oecd-1.2.1/openbb_oecd/models/gdp_real.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/long_term_interest_rate.py` & `openbb_oecd-1.2.1/openbb_oecd/models/long_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/short_term_interest_rate.py` & `openbb_oecd-1.2.1/openbb_oecd/models/short_term_interest_rate.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/models/unemployment.py` & `openbb_oecd-1.2.1/openbb_oecd/models/unemployment.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/utils/constants.py` & `openbb_oecd-1.2.1/openbb_oecd/utils/constants.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/openbb_oecd/utils/helpers.py` & `openbb_oecd-1.2.1/openbb_oecd/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `openbb_oecd-1.2.0/PKG-INFO` & `openbb_oecd-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: openbb-oecd
-Version: 1.2.0
+Version: 1.2.1
 Summary: OECD extension for OpenBB
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
 Requires-Dist: defusedxml (>=0.8.0rc2,<0.9.0)
-Requires-Dist: openbb-core (>=1.2.1,<2.0.0)
+Requires-Dist: openbb-core (>=1.2.3,<2.0.0)
 Requires-Dist: urllib3 (>1.26.16)
 Description-Content-Type: text/markdown
 
 # OpenBB OECD Provider
 
 This extension integrates the [OECD](https://stats.oecd.org) data provider into the OpenBB Platform.
```

