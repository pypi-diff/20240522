# Comparing `tmp/oxaigen-0.0.0.4.3.tar.gz` & `tmp/oxaigen-0.0.0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.4.3.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.4.tar", max compression
```

## Comparing `oxaigen-0.0.0.4.3.tar` & `oxaigen-0.0.0.4.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.3/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.3/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.3/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.3/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     6034 2024-05-22 12:46:41.029891 oxaigen-0.0.0.4.3/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.3/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.3/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.3/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.3/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.3/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.3/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.3/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.3/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     2163 2024-05-22 12:55:07.222872 oxaigen-0.0.0.4.3/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.3/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.3/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.3/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.3/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      827 2024-05-22 12:58:59.817782 oxaigen-0.0.0.4.3/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.3/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.4/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.4/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.4/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.4/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     5715 2024-05-22 13:04:29.274106 oxaigen-0.0.0.4.4/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.4/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.4/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.4/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.4/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.4/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.4/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.4/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.4/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2181 2024-05-22 13:01:58.475194 oxaigen-0.0.0.4.4/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.4/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.4/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.4/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.4/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      827 2024-05-22 13:05:02.105739 oxaigen-0.0.0.4.4/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.4/PKG-INFO
```

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4.4/oxaigen/src/asset/asset.py`

 * *Files 0% similar despite different names*

```diff
@@ -102,45 +102,45 @@
     """
     Function to get a temporary download link from the Oxaigen Client API to a file in the Oxaigen data plane
     """
     if not run_id:
         run_id = ""
 
     query = """
-            query GetDownloadLink($assetKey: [String!]!, $runId: String = "") {
-              getS3AssetDownloadLink(assetKey: $assetKey, runId: $runId) {
-                ... on AssetDownloadLink {
-                  __typename
-                  downloadUrl
-                  fileSize
-                  fileType
-                  lastModified
-                }
-                ... on AssetNotFound {
-                  __typename
-                  errorMessage
-                }
-                ... on AssetDownloadError {
-                  __typename
-                  errorMessage
-                }
-                ... on AuthenticationError {
-                  __typename
-                  errorMessage
-                }
-                ... on AuthorizationError {
-                  __typename
-                  errorMessage
-                }
-              }
-            }
+query GetDownloadLink($assetKey: [String!]!, $runId: String = "") {
+  getS3AssetDownloadLink(assetKey: $assetKey, runId: $runId) {
+    ... on AssetDownloadLink {
+      __typename
+      downloadUrl
+      fileSize
+      fileType
+      lastModified
+    }
+    ... on AssetNotFound {
+      __typename
+      errorMessage
+    }
+    ... on AssetDownloadError {
+      __typename
+      errorMessage
+    }
+    ... on AuthenticationError {
+      __typename
+      errorMessage
+    }
+    ... on AuthorizationError {
+      __typename
+      errorMessage
+    }
+  }
+}
             """
 
     variables = {
-        "assetKey": asset_key,
+        "assetKey": str(asset_key),
         "runId": run_id
     }
 
     return run_api_query(query=query, variables=variables)
 
 
 def _download_asset_file(url: str, file_path: str, file_name: str):
```

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4.4/oxaigen/src/authentication/authentication.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/config.py` & `oxaigen-0.0.0.4.4/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4.4/oxaigen/src/storage/data_storage.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4.4/oxaigen/src/util/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,9 +56,9 @@
             }
             # re-send the request
             response = requests.post(API_ENDPOINT, json=payload, headers=new_headers)
             if response.status_code != 200:
                 raise OxaigenApiException(message=f"Oxaigen Client API connection error: {str(response.text)}")
 
         return response_data["data"]
-    except Exception:
-        raise OxaigenApiException(message='Invalid login input, try again!')
+    except Exception as e:
+        raise OxaigenApiException(message=f"Could not perform API call, error: {str(e)}")
```

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/util/exception.py` & `oxaigen-0.0.0.4.4/oxaigen/src/util/exception.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4.4/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4.4/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.3/pyproject.toml` & `oxaigen-0.0.0.4.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.4.3"
+version = "0.0.0.4.4"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
```

### Comparing `oxaigen-0.0.0.4.3/PKG-INFO` & `oxaigen-0.0.0.4.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.4.3
+Version: 0.0.0.4.4
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
```

