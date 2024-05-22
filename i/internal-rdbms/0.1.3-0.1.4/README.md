# Comparing `tmp/internal_rdbms-0.1.3.tar.gz` & `tmp/internal_rdbms-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal_rdbms-0.1.3.tar", max compression
+gzip compressed data, was "internal_rdbms-0.1.4.tar", max compression
```

## Comparing `internal_rdbms-0.1.3.tar` & `internal_rdbms-0.1.4.tar`

### file list

```diff
@@ -1,31 +1,27 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.3/README.md
--rw-r--r--   0        0        0      705 2024-05-22 03:53:24.281799 internal_rdbms-0.1.3/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.3/src/internal/__init__.py
--rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.3/src/internal/base_config.py
--rw-r--r--   0        0        0     8554 2024-05-21 11:02:00.292285 internal_rdbms-0.1.3/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.3/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal_rdbms-0.1.3/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal_rdbms-0.1.3/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal_rdbms-0.1.3/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0       90 2024-05-21 13:22:22.135464 internal_rdbms-0.1.3/src/internal/common_enum/order_type.py
--rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal_rdbms-0.1.3/src/internal/common_enum/service_ticket_event_trigger_type.py
--rw-r--r--   0        0        0     1604 2024-05-21 13:22:22.137838 internal_rdbms-0.1.3/src/internal/const.py
--rw-r--r--   0        0        0     2066 2024-05-22 03:53:24.284850 internal_rdbms-0.1.3/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.3/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.3/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1640 2024-05-21 13:23:31.968522 internal_rdbms-0.1.3/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.3/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.3/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.3/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.3/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.3/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal_rdbms-0.1.3/src/internal/http/requests.py
--rw-r--r--   0        0        0     1173 2024-05-22 03:15:45.315044 internal_rdbms-0.1.3/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.3/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.3/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.3/src/internal/model/__init__.py
--rw-r--r--   0        0        0      710 2024-05-21 10:37:07.808559 internal_rdbms-0.1.3/src/internal/model/base_model.py
--rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.3/src/internal/schema/__init__.py
--rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.3/src/internal/schema/base_schema.py
--rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal_rdbms-0.1.3/src/internal/utils.py
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 internal_rdbms-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.4/README.md
+-rw-r--r--   0        0        0      705 2024-05-22 07:29:57.720665 internal_rdbms-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.4/src/internal/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.4/src/internal/base_config.py
+-rw-r--r--   0        0        0     8554 2024-05-21 11:02:00.292285 internal_rdbms-0.1.4/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.4/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0       90 2024-05-21 13:22:22.135464 internal_rdbms-0.1.4/src/internal/common_enum/order_type.py
+-rw-r--r--   0        0        0     1604 2024-05-21 13:22:22.137838 internal_rdbms-0.1.4/src/internal/const.py
+-rw-r--r--   0        0        0     2066 2024-05-22 03:53:24.284850 internal_rdbms-0.1.4/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.4/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.4/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1640 2024-05-21 13:23:31.968522 internal_rdbms-0.1.4/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.4/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.4/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.4/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.4/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.4/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal_rdbms-0.1.4/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1173 2024-05-22 03:15:45.315044 internal_rdbms-0.1.4/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.4/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.4/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.4/src/internal/model/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-21 10:37:07.808559 internal_rdbms-0.1.4/src/internal/model/base_model.py
+-rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.4/src/internal/schema/__init__.py
+-rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.4/src/internal/schema/base_schema.py
+-rw-r--r--   0        0        0     2753 2024-05-22 07:29:57.723151 internal_rdbms-0.1.4/src/internal/utils.py
+-rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 internal_rdbms-0.1.4/PKG-INFO
```

### Comparing `internal_rdbms-0.1.3/pyproject.toml` & `internal_rdbms-0.1.4/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "internal-rdbms"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Ray <ray@cruisys.com>"]
 readme = "README.md"
 packages = [{include = "internal", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `internal_rdbms-0.1.3/src/internal/base_config.py` & `internal_rdbms-0.1.4/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/base_factory.py` & `internal_rdbms-0.1.4/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/const.py` & `internal_rdbms-0.1.4/src/internal/const.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/database.py` & `internal_rdbms-0.1.4/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/exception/internal_exception.py` & `internal_rdbms-0.1.4/src/internal/exception/internal_exception.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/ext/amazon/aws/__init__.py` & `internal_rdbms-0.1.4/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/http/requests.py` & `internal_rdbms-0.1.4/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/http/responses.py` & `internal_rdbms-0.1.4/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/src/internal/model/base_model.py` & `internal_rdbms-0.1.4/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.3/PKG-INFO` & `internal_rdbms-0.1.4/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal-rdbms
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

