# Comparing `tmp/internal_rdbms-0.1.0.tar.gz` & `tmp/internal_rdbms-0.1.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "internal_rdbms-0.1.0.tar", max compression
+gzip compressed data, was "internal_rdbms-0.1.0a0.tar", max compression
```

## Comparing `internal_rdbms-0.1.0.tar` & `internal_rdbms-0.1.0a0.tar`

### file list

```diff
@@ -1,30 +1,31 @@
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.0/README.md
--rw-r--r--   0        0        0      705 2024-05-21 12:58:33.360155 internal_rdbms-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.0/src/internal/__init__.py
--rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.0/src/internal/base_config.py
--rw-r--r--   0        0        0     8554 2024-05-21 11:02:00.292285 internal_rdbms-0.1.0/src/internal/base_factory.py
--rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.0/src/internal/common_enum/__init__.py
--rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal_rdbms-0.1.0/src/internal/common_enum/contact_type.py
--rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal_rdbms-0.1.0/src/internal/common_enum/event_type.py
--rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal_rdbms-0.1.0/src/internal/common_enum/operator_type.py
--rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal_rdbms-0.1.0/src/internal/common_enum/service_ticket_event_trigger_type.py
--rw-r--r--   0        0        0     1602 2024-05-21 11:02:00.295431 internal_rdbms-0.1.0/src/internal/const.py
--rw-r--r--   0        0        0     2054 2024-05-21 03:50:35.787913 internal_rdbms-0.1.0/src/internal/database.py
--rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.0/src/internal/exception/__init__.py
--rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.0/src/internal/exception/base_exception.py
--rw-r--r--   0        0        0     1651 2024-03-04 06:00:01.259424 internal_rdbms-0.1.0/src/internal/exception/internal_exception.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.0/src/internal/ext/__init__.py
--rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.0/src/internal/ext/amazon/__init__.py
--rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.0/src/internal/ext/amazon/aws/__init__.py
--rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.0/src/internal/ext/amazon/aws/const.py
--rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.0/src/internal/http/__init__.py
--rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal_rdbms-0.1.0/src/internal/http/requests.py
--rw-r--r--   0        0        0     1184 2024-05-20 03:16:02.967726 internal_rdbms-0.1.0/src/internal/http/responses.py
--rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.0/src/internal/interface/__init__.py
--rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.0/src/internal/interface/base_interface.py
--rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.0/src/internal/model/__init__.py
--rw-r--r--   0        0        0      710 2024-05-21 10:37:07.808559 internal_rdbms-0.1.0/src/internal/model/base_model.py
--rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.0/src/internal/schema/__init__.py
--rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.0/src/internal/schema/base_schema.py
--rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal_rdbms-0.1.0/src/internal/utils.py
--rw-r--r--   0        0        0     1112 1970-01-01 00:00:00.000000 internal_rdbms-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776995 internal_rdbms-0.1.0a0/README.md
+-rw-r--r--   0        0        0      706 2024-05-21 13:22:22.129180 internal_rdbms-0.1.0a0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-22 02:32:48.776948 internal_rdbms-0.1.0a0/src/internal/__init__.py
+-rw-r--r--   0        0        0      892 2024-05-21 10:53:42.491696 internal_rdbms-0.1.0a0/src/internal/base_config.py
+-rw-r--r--   0        0        0     8554 2024-05-21 11:02:00.292285 internal_rdbms-0.1.0a0/src/internal/base_factory.py
+-rw-r--r--   0        0        0        0 2024-02-13 10:57:40.969610 internal_rdbms-0.1.0a0/src/internal/common_enum/__init__.py
+-rw-r--r--   0        0        0      142 2024-02-13 11:01:26.248123 internal_rdbms-0.1.0a0/src/internal/common_enum/contact_type.py
+-rw-r--r--   0        0        0      114 2024-03-19 08:47:41.966209 internal_rdbms-0.1.0a0/src/internal/common_enum/event_type.py
+-rw-r--r--   0        0        0      125 2024-02-13 11:01:26.244153 internal_rdbms-0.1.0a0/src/internal/common_enum/operator_type.py
+-rw-r--r--   0        0        0       90 2024-05-21 13:22:22.135464 internal_rdbms-0.1.0a0/src/internal/common_enum/order_type.py
+-rw-r--r--   0        0        0      511 2024-04-09 02:21:45.907592 internal_rdbms-0.1.0a0/src/internal/common_enum/service_ticket_event_trigger_type.py
+-rw-r--r--   0        0        0     1604 2024-05-21 13:22:22.137838 internal_rdbms-0.1.0a0/src/internal/const.py
+-rw-r--r--   0        0        0     2054 2024-05-21 03:50:35.787913 internal_rdbms-0.1.0a0/src/internal/database.py
+-rw-r--r--   0        0        0        0 2023-12-15 06:58:26.332564 internal_rdbms-0.1.0a0/src/internal/exception/__init__.py
+-rw-r--r--   0        0        0      363 2024-01-28 10:00:28.362441 internal_rdbms-0.1.0a0/src/internal/exception/base_exception.py
+-rw-r--r--   0        0        0     1640 2024-05-21 13:23:31.968522 internal_rdbms-0.1.0a0/src/internal/exception/internal_exception.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564151 internal_rdbms-0.1.0a0/src/internal/ext/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-17 16:40:56.564243 internal_rdbms-0.1.0a0/src/internal/ext/amazon/__init__.py
+-rw-r--r--   0        0        0      834 2024-01-29 02:46:13.060361 internal_rdbms-0.1.0a0/src/internal/ext/amazon/aws/__init__.py
+-rw-r--r--   0        0        0      109 2023-12-11 01:32:53.463567 internal_rdbms-0.1.0a0/src/internal/ext/amazon/aws/const.py
+-rw-r--r--   0        0        0        0 2023-11-10 12:37:53.063137 internal_rdbms-0.1.0a0/src/internal/http/__init__.py
+-rw-r--r--   0        0        0     1675 2024-04-23 08:00:48.112326 internal_rdbms-0.1.0a0/src/internal/http/requests.py
+-rw-r--r--   0        0        0     1184 2024-05-20 03:16:02.967726 internal_rdbms-0.1.0a0/src/internal/http/responses.py
+-rw-r--r--   0        0        0        0 2023-12-29 03:03:59.978251 internal_rdbms-0.1.0a0/src/internal/interface/__init__.py
+-rw-r--r--   0        0        0      340 2024-01-28 03:32:05.468971 internal_rdbms-0.1.0a0/src/internal/interface/base_interface.py
+-rw-r--r--   0        0        0        0 2023-11-29 11:18:12.218216 internal_rdbms-0.1.0a0/src/internal/model/__init__.py
+-rw-r--r--   0        0        0      710 2024-05-21 10:37:07.808559 internal_rdbms-0.1.0a0/src/internal/model/base_model.py
+-rw-r--r--   0        0        0        0 2024-01-03 02:21:34.411884 internal_rdbms-0.1.0a0/src/internal/schema/__init__.py
+-rw-r--r--   0        0        0      324 2024-05-20 06:08:36.689816 internal_rdbms-0.1.0a0/src/internal/schema/base_schema.py
+-rw-r--r--   0        0        0     1509 2024-04-08 11:20:32.745396 internal_rdbms-0.1.0a0/src/internal/utils.py
+-rw-r--r--   0        0        0     1114 1970-01-01 00:00:00.000000 internal_rdbms-0.1.0a0/PKG-INFO
```

### Comparing `internal_rdbms-0.1.0/pyproject.toml` & `internal_rdbms-0.1.0a0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "internal-rdbms"
-version = "0.1.0"
+version = "0.1.0a"
 description = ""
 authors = ["Ray <ray@cruisys.com>"]
 readme = "README.md"
 packages = [{include = "internal", from = "src"}]
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `internal_rdbms-0.1.0/src/internal/base_config.py` & `internal_rdbms-0.1.0a0/src/internal/base_config.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/base_factory.py` & `internal_rdbms-0.1.0a0/src/internal/base_factory.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/const.py` & `internal_rdbms-0.1.0a0/src/internal/const.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 
 SECONDS_PER_YEAR = 30758400
 SECONDS_PER_DAY = 86400
 SECONDS_PER_MIN = 60
 
 DEF_PAGE_NO = 1
 DEF_PAGE_SIZE = 15
-DEF_ORDER = '-id'
+DEF_ORDER_BY = 'id'
 
 APS_EVENT_CODE = {
     1: 'EVENT_SCHEDULER_STARTED',
     2: 'EVENT_SCHEDULER_SHUTDOWN',
     4: 'EVENT_SCHEDULER_PAUSED',
     8: 'EVENT_SCHEDULER_RESUMED',
     16: 'EVENT_EXECUTOR_ADDED',
```

### Comparing `internal_rdbms-0.1.0/src/internal/database.py` & `internal_rdbms-0.1.0a0/src/internal/database.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/exception/internal_exception.py` & `internal_rdbms-0.1.0a0/src/internal/exception/internal_exception.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,47 +1,47 @@
 from fastapi import status
 from .base_exception import InternalBaseException
 
 
 class BadGatewayException(InternalBaseException):
     code = "error_bad_gateway"
-    message = "Bad gateway"
+    message = "請求失敗"
 
     def __init__(self, message: str = None, **kwargs):
         _message = message or self.message
         super().__init__(status.HTTP_502_BAD_GATEWAY, self.code, _message, **kwargs)
 
 
 class GatewayTimeoutException(InternalBaseException):
     code = "error_gateway_timeout"
-    message = "Gateway timeout"
+    message = "請求逾時"
 
     def __init__(self, message: str = None, **kwargs):
         _message = message or self.message
         super().__init__(status.HTTP_504_GATEWAY_TIMEOUT, self.code, _message, **kwargs)
 
 
 class DatabaseInitializeFailureException(InternalBaseException):
     code = "error_database_initialize"
-    message = "Database initialize failure"
+    message = "資料庫初始化失敗"
 
     def __init__(self, message: str = None, **kwargs):
         _message = message or self.message
         super().__init__(status.HTTP_500_INTERNAL_SERVER_ERROR, self.code, _message, **kwargs)
 
 
 class DatabaseConnectFailureException(InternalBaseException):
     code = "error_database_connect"
-    message = "Database connect failure"
+    message = "資料庫連線失敗"
 
     def __init__(self, message: str = None, **kwargs):
         _message = message or self.message
         super().__init__(status.HTTP_500_INTERNAL_SERVER_ERROR, self.code, _message, **kwargs)
 
 
 class NoChangeException(InternalBaseException):
     code = "error_no_change"
-    message = "Document no change"
+    message = "資料未異動"
 
     def __init__(self, message: str = None, **kwargs):
         _message = message or self.message
         super().__init__(status.HTTP_200_OK, self.code, _message, **kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `internal_rdbms-0.1.0/src/internal/ext/amazon/aws/__init__.py` & `internal_rdbms-0.1.0a0/src/internal/ext/amazon/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/http/requests.py` & `internal_rdbms-0.1.0a0/src/internal/http/requests.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/http/responses.py` & `internal_rdbms-0.1.0a0/src/internal/http/responses.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/model/base_model.py` & `internal_rdbms-0.1.0a0/src/internal/model/base_model.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/src/internal/utils.py` & `internal_rdbms-0.1.0a0/src/internal/utils.py`

 * *Files identical despite different names*

### Comparing `internal_rdbms-0.1.0/PKG-INFO` & `internal_rdbms-0.1.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: internal-rdbms
-Version: 0.1.0
+Version: 0.1.0a0
 Summary: 
 Author: Ray
 Author-email: ray@cruisys.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

