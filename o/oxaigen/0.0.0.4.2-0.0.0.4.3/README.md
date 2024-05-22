# Comparing `tmp/oxaigen-0.0.0.4.2.tar.gz` & `tmp/oxaigen-0.0.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oxaigen-0.0.0.4.2.tar", max compression
+gzip compressed data, was "oxaigen-0.0.0.4.3.tar", max compression
```

## Comparing `oxaigen-0.0.0.4.2.tar` & `oxaigen-0.0.0.4.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.2/README.md
--rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.2/oxaigen/__init__.py
--rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.2/oxaigen/src/__init__.py
--rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.2/oxaigen/src/asset/__init__.py
--rw-r--r--   0        0        0     6034 2024-05-22 12:46:41.029891 oxaigen-0.0.0.4.2/oxaigen/src/asset/asset.py
--rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.2/oxaigen/src/authentication/__init__.py
--rw-r--r--   0        0        0     2673 2024-05-22 12:42:13.132340 oxaigen-0.0.0.4.2/oxaigen/src/authentication/authentication.py
--rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.2/oxaigen/src/config.py
--rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.2/oxaigen/src/constant.py
--rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.2/oxaigen/src/main.py
--rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.2/oxaigen/src/storage/__init__.py
--rw-r--r--   0        0        0     5077 2024-05-22 12:35:12.802233 oxaigen-0.0.0.4.2/oxaigen/src/storage/data_storage.py
--rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.2/oxaigen/src/util/__init__.py
--rw-r--r--   0        0        0     2163 2024-05-22 12:55:07.222872 oxaigen-0.0.0.4.2/oxaigen/src/util/api.py
--rw-r--r--   0        0        0      990 2024-05-22 12:51:54.034505 oxaigen-0.0.0.4.2/oxaigen/src/util/exception.py
--rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.2/oxaigen/src/util/logging.py
--rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.2/oxaigen/src/util/token.py
--rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.2/oxaigen/src/util/util.py
--rw-r--r--   0        0        0      827 2024-05-22 12:52:13.286234 oxaigen-0.0.0.4.2/pyproject.toml
--rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.2/PKG-INFO
+-rw-r--r--   0        0        0      251 2024-05-21 16:40:01.974635 oxaigen-0.0.0.4.3/README.md
+-rw-r--r--   0        0        0      112 2024-05-21 18:27:06.168091 oxaigen-0.0.0.4.3/oxaigen/__init__.py
+-rw-r--r--   0        0        0       24 2024-05-21 17:54:21.224181 oxaigen-0.0.0.4.3/oxaigen/src/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-21 18:25:26.885319 oxaigen-0.0.0.4.3/oxaigen/src/asset/__init__.py
+-rw-r--r--   0        0        0     6034 2024-05-22 12:46:41.029891 oxaigen-0.0.0.4.3/oxaigen/src/asset/asset.py
+-rw-r--r--   0        0        0       25 2024-05-21 16:33:07.147095 oxaigen-0.0.0.4.3/oxaigen/src/authentication/__init__.py
+-rw-r--r--   0        0        0     2655 2024-05-22 12:57:53.116060 oxaigen-0.0.0.4.3/oxaigen/src/authentication/authentication.py
+-rw-r--r--   0        0        0     1348 2024-05-22 11:51:20.803630 oxaigen-0.0.0.4.3/oxaigen/src/config.py
+-rw-r--r--   0        0        0      127 2024-05-22 11:51:09.438253 oxaigen-0.0.0.4.3/oxaigen/src/constant.py
+-rw-r--r--   0        0        0      439 2024-05-22 12:27:20.233246 oxaigen-0.0.0.4.3/oxaigen/src/main.py
+-rw-r--r--   0        0        0       23 2024-05-22 01:05:48.100558 oxaigen-0.0.0.4.3/oxaigen/src/storage/__init__.py
+-rw-r--r--   0        0        0     4896 2024-05-22 12:58:53.803577 oxaigen-0.0.0.4.3/oxaigen/src/storage/data_storage.py
+-rw-r--r--   0        0        0       24 2024-05-21 16:40:38.535727 oxaigen-0.0.0.4.3/oxaigen/src/util/__init__.py
+-rw-r--r--   0        0        0     2163 2024-05-22 12:55:07.222872 oxaigen-0.0.0.4.3/oxaigen/src/util/api.py
+-rw-r--r--   0        0        0      906 2024-05-22 12:57:41.116790 oxaigen-0.0.0.4.3/oxaigen/src/util/exception.py
+-rw-r--r--   0        0        0      254 2024-05-22 00:44:20.848444 oxaigen-0.0.0.4.3/oxaigen/src/util/logging.py
+-rw-r--r--   0        0        0     3860 2024-05-22 00:06:58.773848 oxaigen-0.0.0.4.3/oxaigen/src/util/token.py
+-rw-r--r--   0        0        0      823 2024-05-22 12:31:01.295414 oxaigen-0.0.0.4.3/oxaigen/src/util/util.py
+-rw-r--r--   0        0        0      827 2024-05-22 12:58:59.817782 oxaigen-0.0.0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      805 1970-01-01 00:00:00.000000 oxaigen-0.0.0.4.3/PKG-INFO
```

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/asset/asset.py` & `oxaigen-0.0.0.4.3/oxaigen/src/asset/asset.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/authentication/authentication.py` & `oxaigen-0.0.0.4.3/oxaigen/src/authentication/authentication.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,15 +26,15 @@
             OxaigenSDKException: If there is an invalid login input or an unknown error during login.
             OxaigenApiException: If the API returns a connection error or an invalid token response.
         """
         try:
             username = input("Enter your username:")
             password = getpass.getpass("Enter your password: ")
         except Exception as e:
-            raise OxaigenSDKException(message='Invalid login input, try again!', error=e)
+            raise OxaigenSDKException(message='Invalid login input, try again!')
 
         # Define the GraphQL mutation
         mutation = '''
         mutation LoginMutation($username: String!, $password: String!) {
           login(username: $username, password: $password) {
             ... on TokenReturn {
               __typename
@@ -77,8 +77,8 @@
             process_token_return(token_return=token_return)
 
             logging.info("Login successful! Token stored!")
 
         except OxaigenApiException:
             raise
         except Exception as e:
-            raise OxaigenSDKException(message=f"Login failed due to unknown error: {str(e)}", error=e)
+            raise OxaigenSDKException(message=f"Login failed due to unknown error: {str(e)}")
```

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/config.py` & `oxaigen-0.0.0.4.3/oxaigen/src/config.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/storage/data_storage.py` & `oxaigen-0.0.0.4.3/oxaigen/src/storage/data_storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,22 +125,13 @@
         try:
             with open(file, 'rb') as f:
                 try:
                     return pickle.load(f)
                 except (pickle.UnpicklingError, AttributeError):
                     f.seek(0)  # Reset the file pointer to the beginning
                     return f.read()
-        except FileNotFoundError as e:
-            raise OxaigenSDKException(
-                message=f"File not found: {file}. Please check the file path and try again.",
-                error=e
-            )
-        except IOError as e:
-            raise OxaigenSDKException(
-                message=f"IO error occurred while accessing the file: {file}",
-                error=e
-            )
-        except Exception as e:
-            raise OxaigenSDKException(
-                message=f"An unexpected error occurred while loading the file: {file}.",
-                error=e,
-            )
+        except FileNotFoundError:
+            raise OxaigenSDKException(message=f"File not found: {file}. Please check the file path and try again.")
+        except IOError:
+            raise OxaigenSDKException(message=f"IO error occurred while accessing the file: {file}")
+        except Exception:
+            raise OxaigenSDKException(message=f"An unexpected error occurred while loading the file: {file}.")
```

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/util/api.py` & `oxaigen-0.0.0.4.3/oxaigen/src/util/api.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/util/token.py` & `oxaigen-0.0.0.4.3/oxaigen/src/util/token.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.2/oxaigen/src/util/util.py` & `oxaigen-0.0.0.4.3/oxaigen/src/util/util.py`

 * *Files identical despite different names*

### Comparing `oxaigen-0.0.0.4.2/pyproject.toml` & `oxaigen-0.0.0.4.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oxaigen"
-version = "0.0.0.4.2"
+version = "0.0.0.4.3"
 description = "Oxaigen Python SDK"
 authors = ["Luca Roggeveen Name <luca@oxaigen.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10.12"
 pydantic = "==2.7.1"
```

### Comparing `oxaigen-0.0.0.4.2/PKG-INFO` & `oxaigen-0.0.0.4.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oxaigen
-Version: 0.0.0.4.2
+Version: 0.0.0.4.3
 Summary: Oxaigen Python SDK
 Author: Luca Roggeveen Name
 Author-email: luca@oxaigen.com
 Requires-Python: >=3.10.12,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: boto3 (>=1.34.44,<2.0.0)
```

