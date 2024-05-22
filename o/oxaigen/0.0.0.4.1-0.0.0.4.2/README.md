# Comparing `tmp/oxaigen-0.0.0.4.1.tar.gz` & `tmp/oxaigen-0.0.0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.4.1.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.2.tar", max compression
```

## Comparing `oxaigen-0.0.0.4.1.tar` & `oxaigen-0.0.0.4.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.1/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.1/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.1/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.1/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     6034 2024-05-22 12:46:41.029891 oxaigen-0.0.0.4.1/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.1/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2673 2024-05-22 12:42:13.132340 oxaigen-0.0.0.4.1/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.1/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.1/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.1/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.1/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     5077 2024-05-22 12:35:12.802233 oxaigen-0.0.0.4.1/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.1/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     1996 2024-05-22 00:18:31.367628 oxaigen-0.0.0.4.1/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      976 2024-05-22 12:33:36.476086 oxaigen-0.0.0.4.1/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.1/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.1/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.1/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      827 2024-05-22 12:46:48.315750 oxaigen-0.0.0.4.1/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.1/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.2/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.2/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.2/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.2/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     6034 2024-05-22 12:46:41.029891 oxaigen-0.0.0.4.2/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.2/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2673 2024-05-22 12:42:13.132340 oxaigen-0.0.0.4.2/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.2/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.2/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.2/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.2/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     5077 2024-05-22 12:35:12.802233 oxaigen-0.0.0.4.2/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.2/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2163 2024-05-22 12:55:07.222872 oxaigen-0.0.0.4.2/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      990 2024-05-22 12:51:54.034505 oxaigen-0.0.0.4.2/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.2/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.2/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.2/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      827 2024-05-22 12:52:13.286234 oxaigen-0.0.0.4.2/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.2/PKG-INFO
```

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4.2/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4.2/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/config.py` & `oxaigen-0.0.0.4.2/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4.2/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4.2/oxaigen/src/util/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,14 +31,18 @@
         # Send the request
         response = requests.post(API_ENDPOINT, json=payload, headers=headers)
         if response.status_code != 200:
             raise OxaigenApiException(message=f"Oxaigen Client API connection error: {str(response.text)}")
 
         response_data = response.json()
 
+        if "data" not in response_data:
+            print(response_data)
+            raise KeyError("Unknown API response, invalid query or input arguments provided.")
+
         auth_failure = False
         for item in response_data["data"]:
             try:
                 if item["__typename"] == "AuthenticationError":
                     auth_failure = True
                     break
             except KeyError:
@@ -54,9 +58,7 @@
             response = requests.post(API_ENDPOINT, json=payload, headers=new_headers)
             if response.status_code != 200:
                 raise OxaigenApiException(message=f"Oxaigen Client API connection error: {str(response.text)}")
 
         return response_data["data"]
     except Exception:
         raise OxaigenApiException(message='Invalid login input, try again!')
-
-
```

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/util/exception.py` & `oxaigen-0.0.0.4.2/oxaigen/src/util/exception.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,22 +16,22 @@
 
 
 class OxaigenSDKException(OxaigenException):
     """
     Raised when an Oxaigen SDk error occurs.
     """
 
-    def __init__(self, message, error: Optional[Any], *args):
+    def __init__(self, message, error: Optional[Any] = None, *args):
         log_message = f"Exception occurred: {message}. SDK Error: {str(error)}"
         logger.debug(log_message)
         super().__init__(message, *args)
 
 
 class OxaigenApiException(OxaigenException):
     """
     Raised when an API related error occurs.
     """
 
-    def __init__(self, message, error: Optional[Any], *args):
+    def __init__(self, message, error: Optional[Any] = None, *args):
         log_message = f"Exception occurred: {message}. API Error: {str(error)}"
         logger.debug(log_message)
         super().__init__(message, *args)
```

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4.2/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4.2/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.1/pyproject.toml` & `oxaigen-0.0.0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.4.1"
+version = "0.0.0.4.2"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
```

### Comparing `oxaigen-0.0.0.4.1/PKG-INFO` & `oxaigen-0.0.0.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.4.1
+Version: 0.0.0.4.2
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
```

