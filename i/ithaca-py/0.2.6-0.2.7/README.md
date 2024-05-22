# Comparing `tmp/ithaca_py-0.2.6.tar.gz` & `tmp/ithaca_py-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ithaca_py-0.2.6.tar", max compression
+gzip compressed data, was "ithaca_py-0.2.7.tar", max compression
```

## Comparing `ithaca_py-0.2.6.tar` & `ithaca_py-0.2.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      983 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/README.md
--rw-r--r--   0        0        0     5147 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/__init__.py
--rw-r--r--   0        0        0     3870 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/analytics.py
--rw-r--r--   0        0        0    10809 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/auth.py
--rw-r--r--   0        0        0     5589 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/calculation.py
--rw-r--r--   0        0        0     3526 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/client.py
--rw-r--r--   0        0        0     1846 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/constants.py
--rw-r--r--   0        0        0    12592 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/fundlock.py
--rw-r--r--   0        0        0      603 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/market.py
--rw-r--r--   0        0        0     7370 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/orders.py
--rw-r--r--   0        0        0     1373 2024-05-16 10:01:41.538275 ithaca_py-0.2.6/ithaca/protocol.py
--rw-r--r--   0        0        0     2406 2024-05-16 10:01:41.542275 ithaca_py-0.2.6/ithaca/socket.py
--rw-r--r--   0        0        0      929 2024-05-16 10:01:41.542275 ithaca_py-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0      983 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/README.md
+-rw-r--r--   0        0        0     5147 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/__init__.py
+-rw-r--r--   0        0        0     3870 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/analytics.py
+-rw-r--r--   0        0        0    10809 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/auth.py
+-rw-r--r--   0        0        0     5589 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/calculation.py
+-rw-r--r--   0        0        0     3668 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/client.py
+-rw-r--r--   0        0        0     1846 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/constants.py
+-rw-r--r--   0        0        0    12592 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/fundlock.py
+-rw-r--r--   0        0        0      603 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/market.py
+-rw-r--r--   0        0        0     7370 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/orders.py
+-rw-r--r--   0        0        0     1373 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/protocol.py
+-rw-r--r--   0        0        0     2406 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/ithaca/socket.py
+-rw-r--r--   0        0        0      929 2024-05-22 05:51:36.389991 ithaca_py-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     1828 1970-01-01 00:00:00.000000 ithaca_py-0.2.7/PKG-INFO
```

### Comparing `ithaca_py-0.2.6/README.md` & `ithaca_py-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/__init__.py` & `ithaca_py-0.2.7/ithaca/__init__.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/analytics.py` & `ithaca_py-0.2.7/ithaca/analytics.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/auth.py` & `ithaca_py-0.2.7/ithaca/auth.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/calculation.py` & `ithaca_py-0.2.7/ithaca/calculation.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/client.py` & `ithaca_py-0.2.7/ithaca/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -59,19 +59,27 @@
 
     def trade_history(
         self,
         date_from: int = None,
         date_to: int = None,
         offset: int = None,
         limit: int = None,
+        status: str = None,
     ):
         """Get trade history."""
         """date_from/to are timestamps in backend"""
-        body = {"from": date_from, "to": date_to, "offset": offset, "limit": limit}
-        if date_from or date_to or offset or limit:
+        body = {key: value for key, value in {
+            'from': date_from,
+            'to': date_to,
+            'offset': offset,
+            'limit': limit,
+            'status': status
+        }.items() if value is not None}
+
+        if body:
             return self.parent.post("/clientapi/tradeHistory", json=body)
         else:
             return self.parent.post("/clientapi/tradeHistory")
 
     def historical_positions(self, expiry, _filter="NO_DETAILS"):
         """Get client historical positions.
```

### Comparing `ithaca_py-0.2.6/ithaca/constants.py` & `ithaca_py-0.2.7/ithaca/constants.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/fundlock.py` & `ithaca_py-0.2.7/ithaca/fundlock.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/market.py` & `ithaca_py-0.2.7/ithaca/market.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/orders.py` & `ithaca_py-0.2.7/ithaca/orders.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/protocol.py` & `ithaca_py-0.2.7/ithaca/protocol.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/ithaca/socket.py` & `ithaca_py-0.2.7/ithaca/socket.py`

 * *Files identical despite different names*

### Comparing `ithaca_py-0.2.6/pyproject.toml` & `ithaca_py-0.2.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ithaca_py"
-version = "0.2.6"
+version = "0.2.7"
 description = "Ithaca Protocol SDK"
 authors = ["nhaga <nhaga5@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ithaca"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `ithaca_py-0.2.6/PKG-INFO` & `ithaca_py-0.2.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ithaca_py
-Version: 0.2.6
+Version: 0.2.7
 Summary: Ithaca Protocol SDK
 Author: nhaga
 Author-email: nhaga5@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

