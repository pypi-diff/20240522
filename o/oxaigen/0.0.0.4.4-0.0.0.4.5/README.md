# Comparing `tmp/oxaigen-0.0.0.4.4.tar.gz` & `tmp/oxaigen-0.0.0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.4.4.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.5.tar", max compression
```

## Comparing `oxaigen-0.0.0.4.4.tar` & `oxaigen-0.0.0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.4/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.4/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.4/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.4/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     5715 2024-05-22 13:04:29.274106 oxaigen-0.0.0.4.4/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.4/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.4/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.4/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.4/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.4/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.4/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.4/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.4/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     2181 2024-05-22 13:01:58.475194 oxaigen-0.0.0.4.4/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.4/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.4/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.4/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.4/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      827 2024-05-22 13:05:02.105739 oxaigen-0.0.0.4.4/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.4/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.5/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.5/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.5/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.5/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     5715 2024-05-22 13:04:29.274106 oxaigen-0.0.0.4.5/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.5/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.5/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.5/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.5/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.5/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.5/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.5/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.5/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2324 2024-05-22 13:10:17.818740 oxaigen-0.0.0.4.5/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.5/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.5/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     4163 2024-05-22 13:08:50.416970 oxaigen-0.0.0.4.5/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.5/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      827 2024-05-22 13:10:20.897194 oxaigen-0.0.0.4.5/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.5/PKG-INFO
```

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4.5/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4.5/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/config.py` & `oxaigen-0.0.0.4.5/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4.5/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4.5/oxaigen/src/util/api.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,26 +2,28 @@
 import os
 import requests
 from typing import Dict, Any
 
 from ..constant import ACCESS_TOKEN
 from ..config import API_ENDPOINT
 from .exception import OxaigenApiException
-from .token import refresh_tokens
+from .token import refresh_tokens, get_access_token_from_token_file
 
 
 def run_api_query(query: str, variables: Dict[str, Any]) -> Dict[str, Any]:
     """
     Util function to call the Oxaigen Private Client API and handles authorization errors
     """
     try:
         access_token = os.environ.get(ACCESS_TOKEN)
         if not access_token:
-            refresh_tokens()
-            access_token = os.environ.get(ACCESS_TOKEN)
+            access_token = get_access_token_from_token_file()
+            if not access_token:
+                refresh_tokens()
+                access_token = get_access_token_from_token_file()
 
         # Define the payload
         payload = {
             "query": query,
             "variables": variables
         }
         headers = {
```

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/util/exception.py` & `oxaigen-0.0.0.4.5/oxaigen/src/util/exception.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4.5/oxaigen/src/util/token.py`

 * *Files 4% similar despite different names*

```diff
@@ -116,14 +116,27 @@
 
         with open(TOKEN_FILE_PATH, "w") as token_file:
             json.dump(token_data, token_file, indent=4)
     else:
         raise OxaigenSDKException(message="Invalid TokenReturn")
 
 
+def get_access_token_from_token_file() -> Optional[str]:
+    """
+    Get refresh
+    """
+    try:
+        with open(TOKEN_FILE_PATH, "r") as token_file:
+            token = json.load(token_file)
+        return token['accessToken']
+    except Exception as e:
+        logging.log(e)
+        return None
+
+
 def get_refresh_token_from_token_file() -> Optional[str]:
     """
     Get refresh
     """
     try:
         with open(TOKEN_FILE_PATH, "r") as token_file:
             token = json.load(token_file)
```

### Comparing `oxaigen-0.0.0.4.4/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4.5/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.4/pyproject.toml` & `oxaigen-0.0.0.4.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.4.4"
+version = "0.0.0.4.5"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
```

### Comparing `oxaigen-0.0.0.4.4/PKG-INFO` & `oxaigen-0.0.0.4.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.4.4
+Version: 0.0.0.4.5
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
```

