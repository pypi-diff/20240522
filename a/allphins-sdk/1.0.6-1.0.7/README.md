# Comparing `tmp/allphins_sdk-1.0.6.tar.gz` & `tmp/allphins_sdk-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allphins_sdk-1.0.6.tar", max compression
+gzip compressed data, was "allphins_sdk-1.0.7.tar", max compression
```

## Comparing `allphins_sdk-1.0.6.tar` & `allphins_sdk-1.0.7.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0      800 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/README.md
--rw-r--r--   0        0        0      685 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/allphins/__init__.py
--rw-r--r--   0        0        0      104 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/allphins/client/__init__.py
--rw-r--r--   0        0        0     3480 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/allphins/client/auth.py
--rw-r--r--   0        0        0     6343 2024-03-29 16:31:28.007368 allphins_sdk-1.0.6/allphins/client/client.py
--rw-r--r--   0        0        0     1328 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/allphins/client/result.py
--rw-r--r--   0        0        0      289 2024-03-28 15:27:18.810495 allphins_sdk-1.0.6/allphins/const.py
--rw-r--r--   0        0        0    14442 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/interface.py
--rw-r--r--   0        0        0      404 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/__init__.py
--rw-r--r--   0        0        0     2086 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/base.py
--rw-r--r--   0        0        0     1875 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/datasource.py
--rw-r--r--   0        0        0     3231 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/policy.py
--rw-r--r--   0        0        0     2775 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/portfolio.py
--rw-r--r--   0        0        0      749 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/risk.py
--rw-r--r--   0        0        0      257 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/scenario.py
--rw-r--r--   0        0        0      814 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/models/scenario_list.py
--rw-r--r--   0        0        0      336 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/singleton.py
--rw-r--r--   0        0        0     2259 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/status.py
--rw-r--r--   0        0        0      552 2024-03-28 15:27:18.811495 allphins_sdk-1.0.6/allphins/utils.py
--rw-r--r--   0        0        0     1755 2024-03-29 16:31:28.007368 allphins_sdk-1.0.6/pyproject.toml
--rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 allphins_sdk-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0      800 2024-03-28 15:27:18.810495 allphins_sdk-1.0.7/README.md
+-rw-r--r--   0        0        0      685 2024-03-28 15:27:18.810495 allphins_sdk-1.0.7/allphins/__init__.py
+-rw-r--r--   0        0        0      104 2024-03-28 15:27:18.810495 allphins_sdk-1.0.7/allphins/client/__init__.py
+-rw-r--r--   0        0        0     3480 2024-04-15 15:16:18.724744 allphins_sdk-1.0.7/allphins/client/auth.py
+-rw-r--r--   0        0        0     6422 2024-04-15 15:15:11.448524 allphins_sdk-1.0.7/allphins/client/client.py
+-rw-r--r--   0        0        0     1328 2024-03-28 15:27:18.810495 allphins_sdk-1.0.7/allphins/client/result.py
+-rw-r--r--   0        0        0      372 2024-04-15 15:14:01.734268 allphins_sdk-1.0.7/allphins/const.py
+-rw-r--r--   0        0        0    14442 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/interface.py
+-rw-r--r--   0        0        0      404 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/__init__.py
+-rw-r--r--   0        0        0     2086 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/base.py
+-rw-r--r--   0        0        0     1875 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/datasource.py
+-rw-r--r--   0        0        0     3231 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/policy.py
+-rw-r--r--   0        0        0     2775 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/portfolio.py
+-rw-r--r--   0        0        0      749 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/risk.py
+-rw-r--r--   0        0        0      257 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/scenario.py
+-rw-r--r--   0        0        0      814 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/models/scenario_list.py
+-rw-r--r--   0        0        0      336 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/singleton.py
+-rw-r--r--   0        0        0     2259 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/status.py
+-rw-r--r--   0        0        0      552 2024-03-28 15:27:18.811495 allphins_sdk-1.0.7/allphins/utils.py
+-rw-r--r--   0        0        0     1755 2024-04-15 15:16:00.968417 allphins_sdk-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0     1373 1970-01-01 00:00:00.000000 allphins_sdk-1.0.7/PKG-INFO
```

### Comparing `allphins_sdk-1.0.6/README.md` & `allphins_sdk-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/__init__.py` & `allphins_sdk-1.0.7/allphins/__init__.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/client/auth.py` & `allphins_sdk-1.0.7/allphins/client/auth.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,8 +94,8 @@
     def get_authentication_header(self) -> dict:
         """Get the authentication header to be added in any requests.
 
         Returns:
             The authentication header.
             Example: {'Authorization': 'Bearer xxxx'}.
         """
-        return {'Authorization': f'Bearer {self._access_token}', 'User-Agent': 'Allphins SDK/1.0.4'}
+        return {'Authorization': f'Bearer {self._access_token}', 'User-Agent': 'Allphins SDK/1.0.7'}
```

### Comparing `allphins_sdk-1.0.6/allphins/client/client.py` & `allphins_sdk-1.0.7/allphins/client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import requests
 from requests import HTTPError
 from requests import Response
 from tqdm import tqdm
 
 from allphins.client.auth import Auth
+from allphins.const import SSL_IGNORE
 from allphins.singleton import Singleton
 from allphins.status import HTTP_403_FORBIDDEN
 
 
 class Client(metaclass=Singleton):
     """Client to bundle configuration needed for API requests.
 
@@ -150,15 +151,17 @@
         if headers is None:
             headers = {}
 
         auth_header = self.auth.get_authentication_header()
         headers = {**headers, **auth_header}
         url = self._set_page_size(url, page_size)
 
-        response = requests.request(method, url, headers=headers, json=json, timeout=self.REQUEST_TIMEOUT)
+        response = requests.request(
+            method, url, headers=headers, json=json, timeout=self.REQUEST_TIMEOUT, verify=SSL_IGNORE
+        )
         return response
 
     @staticmethod
     def _set_page_size(url: str, page_size: Optional[int]) -> str:
         """Append the pagination to the url.
 
         By default, the API paginates the results. To get all the results, we explicitly set the pageSize to None.
```

### Comparing `allphins_sdk-1.0.6/allphins/client/result.py` & `allphins_sdk-1.0.7/allphins/client/result.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/interface.py` & `allphins_sdk-1.0.7/allphins/interface.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/base.py` & `allphins_sdk-1.0.7/allphins/models/base.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/datasource.py` & `allphins_sdk-1.0.7/allphins/models/datasource.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/policy.py` & `allphins_sdk-1.0.7/allphins/models/policy.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/portfolio.py` & `allphins_sdk-1.0.7/allphins/models/portfolio.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/risk.py` & `allphins_sdk-1.0.7/allphins/models/risk.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/models/scenario_list.py` & `allphins_sdk-1.0.7/allphins/models/scenario_list.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/status.py` & `allphins_sdk-1.0.7/allphins/status.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/allphins/utils.py` & `allphins_sdk-1.0.7/allphins/utils.py`

 * *Files identical despite different names*

### Comparing `allphins_sdk-1.0.6/pyproject.toml` & `allphins_sdk-1.0.7/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 convention = "google"
 
 [tool.coverage.run]
 disable_warnings = ["no-data-corrllected"]
 
 [tool.poetry]
 name = "allphins-sdk"
-version = "1.0.6"
+version = "1.0.7"
 description = "Allphins SDK for Python"
 authors = ["Florent <florent@allphins.com>"]
 readme = "README.md"
 packages = [{include = "allphins"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `allphins_sdk-1.0.6/PKG-INFO` & `allphins_sdk-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allphins-sdk
-Version: 1.0.6
+Version: 1.0.7
 Summary: Allphins SDK for Python
 Author: Florent
 Author-email: florent@allphins.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

