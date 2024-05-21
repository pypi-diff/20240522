# Comparing `tmp/sqlakeyset-2.0.1708907391.tar.gz` & `tmp/sqlakeyset-2.0.1716332987.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlakeyset-2.0.1708907391.tar", max compression
+gzip compressed data, was "sqlakeyset-2.0.1716332987.tar", max compression
```

## Comparing `sqlakeyset-2.0.1708907391.tar` & `sqlakeyset-2.0.1716332987.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1210 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/LICENSE
--rw-r--r--   0        0        0     8444 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/README.rst
--rw-r--r--   0        0        0     1295 2024-02-26 00:29:51.216832 sqlakeyset-2.0.1708907391/pyproject.toml
--rw-r--r--   0        0        0      631 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/__init__.py
--rw-r--r--   0        0        0     2767 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/asyncio.py
--rw-r--r--   0        0        0    15033 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/columns.py
--rw-r--r--   0        0        0       37 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/constants.py
--rw-r--r--   0        0        0    14164 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/paging.py
--rw-r--r--   0        0        0        0 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/py.typed
--rw-r--r--   0        0        0    10330 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/results.py
--rw-r--r--   0        0        0      347 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/serial/__init__.py
--rw-r--r--   0        0        0     5756 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/serial/serial.py
--rw-r--r--   0        0        0     2498 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/sqla.py
--rw-r--r--   0        0        0     2613 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/sqla13.py
--rw-r--r--   0        0        0     1754 2024-02-26 00:29:47.024868 sqlakeyset-2.0.1708907391/sqlakeyset/sqla14.py
--rw-r--r--   0        0        0     4321 2024-02-26 00:29:47.028868 sqlakeyset-2.0.1708907391/sqlakeyset/sqla20.py
--rw-r--r--   0        0        0      768 2024-02-26 00:29:47.028868 sqlakeyset-2.0.1708907391/sqlakeyset/types.py
--rw-r--r--   0        0        0     9304 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1708907391/PKG-INFO
+-rw-r--r--   0        0        0     1210 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/LICENSE
+-rw-r--r--   0        0        0     8444 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/README.rst
+-rw-r--r--   0        0        0     1295 2024-05-21 23:09:47.206138 sqlakeyset-2.0.1716332987/pyproject.toml
+-rw-r--r--   0        0        0      631 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/__init__.py
+-rw-r--r--   0        0        0     2767 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/asyncio.py
+-rw-r--r--   0        0        0    15033 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/columns.py
+-rw-r--r--   0        0        0       37 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/constants.py
+-rw-r--r--   0        0        0    14164 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/paging.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/py.typed
+-rw-r--r--   0        0        0    10330 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/results.py
+-rw-r--r--   0        0        0      347 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/serial/__init__.py
+-rw-r--r--   0        0        0     5756 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/serial/serial.py
+-rw-r--r--   0        0        0     2498 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/sqla.py
+-rw-r--r--   0        0        0     2613 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/sqla13.py
+-rw-r--r--   0        0        0     1754 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/sqla14.py
+-rw-r--r--   0        0        0     4321 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/sqla20.py
+-rw-r--r--   0        0        0      768 2024-05-21 23:09:42.554164 sqlakeyset-2.0.1716332987/sqlakeyset/types.py
+-rw-r--r--   0        0        0     9304 1970-01-01 00:00:00.000000 sqlakeyset-2.0.1716332987/PKG-INFO
```

### Comparing `sqlakeyset-2.0.1708907391/LICENSE` & `sqlakeyset-2.0.1716332987/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/README.rst` & `sqlakeyset-2.0.1716332987/README.rst`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/pyproject.toml` & `sqlakeyset-2.0.1716332987/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry-core>=1.0.0",]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "sqlakeyset"
-version = "2.0.1708907391"
+version = "2.0.1716332987"
 authors = [ "Robert Lechte <robertlechte@gmail.com>", "Anthony Carapetis <anthony.carapetis@gmail.com>",]
 license = "Unlicense"
 readme = "README.rst"
 description = "offset-free paging for sqlalchemy"
 repository = "https://github.com/djrobstep/sqlakeyset"
 homepage = "https://github.com/djrobstep/sqlakeyset"
```

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/__init__.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/__init__.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/asyncio.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/asyncio.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/columns.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/columns.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/paging.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/paging.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/results.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/results.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/serial/serial.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/serial/serial.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/sqla.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/sqla.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/sqla13.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/sqla13.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/sqla14.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/sqla14.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/sqla20.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/sqla20.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/sqlakeyset/types.py` & `sqlakeyset-2.0.1716332987/sqlakeyset/types.py`

 * *Files identical despite different names*

### Comparing `sqlakeyset-2.0.1708907391/PKG-INFO` & `sqlakeyset-2.0.1716332987/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlakeyset
-Version: 2.0.1708907391
+Version: 2.0.1716332987
 Summary: offset-free paging for sqlalchemy
 Home-page: https://github.com/djrobstep/sqlakeyset
 License: Unlicense
 Author: Robert Lechte
 Author-email: robertlechte@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
```

