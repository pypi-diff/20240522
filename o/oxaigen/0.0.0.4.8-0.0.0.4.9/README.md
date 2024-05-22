# Comparing `tmp/oxaigen-0.0.0.4.8.tar.gz` & `tmp/oxaigen-0.0.0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.4.8.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.9.tar", max compression
```

## Comparing `oxaigen-0.0.0.4.8.tar` & `oxaigen-0.0.0.4.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.8/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.8/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.8/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.8/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     5715 2024-05-22 13:04:29.274106 oxaigen-0.0.0.4.8/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.8/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.8/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.8/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.8/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.8/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.8/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.8/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.8/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     2218 2024-05-22 13:25:45.588812 oxaigen-0.0.0.4.8/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.8/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.8/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     4117 2024-05-22 13:16:05.444588 oxaigen-0.0.0.4.8/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.8/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      827 2024-05-22 13:25:49.011104 oxaigen-0.0.0.4.8/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.8/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.9/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.9/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.9/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.9/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     5715 2024-05-22 13:04:29.274106 oxaigen-0.0.0.4.9/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.9/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.9/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.9/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.9/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.9/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.9/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.9/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.9/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2274 2024-05-22 13:27:25.297576 oxaigen-0.0.0.4.9/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.9/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.9/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     4117 2024-05-22 13:16:05.444588 oxaigen-0.0.0.4.9/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.9/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      827 2024-05-22 13:27:34.124373 oxaigen-0.0.0.4.9/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.9/PKG-INFO
```

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4.9/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4.9/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/config.py` & `oxaigen-0.0.0.4.9/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4.9/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4.9/oxaigen/src/util/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,28 +35,28 @@
             raise OxaigenApiException(message=f"Oxaigen Client API connection error: {str(response.text)}")
 
         response_data = response.json()
 
         if "data" not in response_data:
             raise KeyError("Unknown API response, invalid query or input arguments provided.")
 
-        auth_failure = False
-
         response_data_dict: Dict = response_data["data"]
 
-        for key, value in response_data_dict:
-            # e.g. key == 'getS3AssetDownloadLink',
-            # e.g. value == {'__typename': 'AssetNotFound', 'errorMessage': 'Asset with asset key ["xxx"] not found.'}
-            try:
-                if "__typename" in value:
-                    if value["__typename"] == "AuthenticationError":
-                        auth_failure = True
-                        break
-            except KeyError:
-                continue
-
-        if auth_failure:
-            raise OxaigenApiException(message=f"Oxaigen Client API authentication error: please login again!")
+        # TODO: TO FIX!
+        auth_failure = False
+        # for key, value in response_data_dict:
+        #     # e.g. key == 'getS3AssetDownloadLink',
+        #     # e.g. value == {'__typename': 'AssetNotFound', 'errorMessage': 'Asset with asset key ["xxx"] not found.'}
+        #     try:
+        #         if "__typename" in value:
+        #             if value["__typename"] == "AuthenticationError":
+        #                 auth_failure = True
+        #                 break
+        #     except KeyError:
+        #         continue
+        #
+        # if auth_failure:
+        #     raise OxaigenApiException(message=f"Oxaigen Client API authentication error: please login again!")
 
         return response_data_dict
     except Exception as e:
         raise OxaigenApiException(message=f"Could not perform API call, error: {str(e)}")
```

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/util/exception.py` & `oxaigen-0.0.0.4.9/oxaigen/src/util/exception.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4.9/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4.9/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.8/pyproject.toml` & `oxaigen-0.0.0.4.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.4.8"
+version = "0.0.0.4.9"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
```

### Comparing `oxaigen-0.0.0.4.8/PKG-INFO` & `oxaigen-0.0.0.4.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.4.8
+Version: 0.0.0.4.9
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
```

