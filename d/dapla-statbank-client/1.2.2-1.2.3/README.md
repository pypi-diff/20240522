# Comparing `tmp/dapla_statbank_client-1.2.2.tar.gz` & `tmp/dapla_statbank_client-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_statbank_client-1.2.2.tar", max compression
+gzip compressed data, was "dapla_statbank_client-1.2.3.tar", max compression
```

## Comparing `dapla_statbank_client-1.2.2.tar` & `dapla_statbank_client-1.2.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1074 2024-05-02 11:59:16.170213 dapla_statbank_client-1.2.2/LICENSE
--rw-r--r--   0        0        0    12373 2024-05-02 11:59:26.766121 dapla_statbank_client-1.2.2/README.md
--rw-r--r--   0        0        0     4224 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/pyproject.toml
--rw-r--r--   0        0        0     1720 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/__init__.py
--rw-r--r--   0        0        0     4105 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/api_types.py
--rw-r--r--   0        0        0     7555 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/apidata.py
--rw-r--r--   0        0        0     4007 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/auth.py
--rw-r--r--   0        0        0    20311 2024-05-02 11:59:26.770120 dapla_statbank_client-1.2.2/src/statbank/client.py
--rw-r--r--   0        0        0     1136 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/globals.py
--rw-r--r--   0        0        0        0 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/py.typed
--rw-r--r--   0        0        0     1304 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/statbank_logger.py
--rw-r--r--   0        0        0    14268 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/transfer.py
--rw-r--r--   0        0        0    17765 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/uttrekk.py
--rw-r--r--   0        0        0    26391 2024-05-02 11:59:16.174213 dapla_statbank_client-1.2.2/src/statbank/uttrekk_validations.py
--rw-r--r--   0        0        0    13761 1970-01-01 00:00:00.000000 dapla_statbank_client-1.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2024-05-22 10:14:35.850199 dapla_statbank_client-1.2.3/LICENSE
+-rw-r--r--   0        0        0    12373 2024-05-22 10:14:35.850199 dapla_statbank_client-1.2.3/README.md
+-rw-r--r--   0        0        0     4224 2024-05-22 10:14:45.430286 dapla_statbank_client-1.2.3/pyproject.toml
+-rw-r--r--   0        0        0     1720 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/__init__.py
+-rw-r--r--   0        0        0     4105 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/api_types.py
+-rw-r--r--   0        0        0     7555 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/apidata.py
+-rw-r--r--   0        0        0     4007 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/auth.py
+-rw-r--r--   0        0        0    20340 2024-05-22 10:14:45.430286 dapla_statbank_client-1.2.3/src/statbank/client.py
+-rw-r--r--   0        0        0     1136 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/globals.py
+-rw-r--r--   0        0        0        0 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/py.typed
+-rw-r--r--   0        0        0     1304 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/statbank_logger.py
+-rw-r--r--   0        0        0    14268 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/transfer.py
+-rw-r--r--   0        0        0    17765 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/uttrekk.py
+-rw-r--r--   0        0        0    26391 2024-05-22 10:14:35.854200 dapla_statbank_client-1.2.3/src/statbank/uttrekk_validations.py
+-rw-r--r--   0        0        0    13761 1970-01-01 00:00:00.000000 dapla_statbank_client-1.2.3/PKG-INFO
```

### Comparing `dapla_statbank_client-1.2.2/LICENSE` & `dapla_statbank_client-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/README.md` & `dapla_statbank_client-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/pyproject.toml` & `dapla_statbank_client-1.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-statbank-client"
-version = "1.2.2"
+version = "1.2.3"
 description = "Handles data transfer Statbank <-> Dapla for Statistics Norway"
 authors = ["Statistics Norway", "Carl F. Corneil <cfc@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-statbank-client"
 repository = "https://github.com/statisticsnorway/dapla-statbank-client"
 documentation = "https://statisticsnorway.github.io/dapla-statbank-client"
```

### Comparing `dapla_statbank_client-1.2.2/src/statbank/__init__.py` & `dapla_statbank_client-1.2.3/src/statbank/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/api_types.py` & `dapla_statbank_client-1.2.3/src/statbank/api_types.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/apidata.py` & `dapla_statbank_client-1.2.3/src/statbank/apidata.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/auth.py` & `dapla_statbank_client-1.2.3/src/statbank/auth.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/client.py` & `dapla_statbank_client-1.2.3/src/statbank/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -185,18 +185,18 @@
         Args:
             date (datetime): date-picker widget, or a date-string formatted as 2000-12-31
 
         Raises:
             TypeError: If the date-parameter is of type other than datetime, string, or ipywidgets.DatePicker.
         """
         if isinstance(date, widgets.DatePicker):
-            date_date: dt.datetime = dt.datetime.combine(
-                date.value.today(),
+            date_date = dt.datetime.combine(
+                date.value,
                 dt.datetime.min.time(),
-            )
+            ).astimezone(OSLO_TIMEZONE) + dt.timedelta(hours=1)
         elif isinstance(date, str):
             date_date = dt.datetime.strptime(date, "%Y-%m-%d").astimezone(
                 OSLO_TIMEZONE,
             ) + dt.timedelta(hours=1)
         elif isinstance(date, dt.datetime):
             date_date = date
         else:
```

### Comparing `dapla_statbank_client-1.2.2/src/statbank/globals.py` & `dapla_statbank_client-1.2.3/src/statbank/globals.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/statbank_logger.py` & `dapla_statbank_client-1.2.3/src/statbank/statbank_logger.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/transfer.py` & `dapla_statbank_client-1.2.3/src/statbank/transfer.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/uttrekk.py` & `dapla_statbank_client-1.2.3/src/statbank/uttrekk.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/src/statbank/uttrekk_validations.py` & `dapla_statbank_client-1.2.3/src/statbank/uttrekk_validations.py`

 * *Files identical despite different names*

### Comparing `dapla_statbank_client-1.2.2/PKG-INFO` & `dapla_statbank_client-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-statbank-client
-Version: 1.2.2
+Version: 1.2.3
 Summary: Handles data transfer Statbank <-> Dapla for Statistics Norway
 Home-page: https://github.com/statisticsnorway/dapla-statbank-client
 License: MIT
 Author: Statistics Norway
 Requires-Python: >=3.10,<4
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
```

