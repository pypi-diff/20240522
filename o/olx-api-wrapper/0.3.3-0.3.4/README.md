# Comparing `tmp/olx-api-wrapper-0.3.3.tar.gz` & `tmp/olx-api-wrapper-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olx-api-wrapper-0.3.3.tar", last modified: Wed May  8 18:05:29 2024, max compression
+gzip compressed data, was "olx-api-wrapper-0.3.4.tar", last modified: Wed May 22 11:20:49 2024, max compression
```

## Comparing `olx-api-wrapper-0.3.3.tar` & `olx-api-wrapper-0.3.4.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.618420 olx-api-wrapper-0.3.3/olx/
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.618420 olx-api-wrapper-0.3.3/olx/partner/
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/advert_logo.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/advert_statistics.py
--rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/adverts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/categories_attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/cities_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/languages_currencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/olx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/paid_features.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/payments.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/threads_messages.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/user_business.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/partner/users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.618420 olx-api-wrapper-0.3.3/olx/public/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/checkout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.618420 olx-api-wrapper-0.3.3/olx/public/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.618420 olx-api-wrapper-0.3.3/olx/public/models/offers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/offers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/offers/filters.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/offers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/offers/offers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/olx/public/models/seo/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/seo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/seo/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/models/seo/popular_searches.py
--rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/offers.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/olx_public.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/olx/public/seo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-08 18:05:29.000000 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-08 18:05:29.000000 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-08 18:05:29.000000 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-08 18:05:29.000000 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-08 18:05:29.000000 olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:29.622420 olx-api-wrapper-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/tests/test_cities_and_districts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-08 18:05:21.000000 olx-api-wrapper-0.3.3/tests/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9874 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.382879 olx-api-wrapper-0.3.4/olx/
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/partner/
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/advert_logo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/advert_statistics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4326 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/adverts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1836 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/categories_attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2674 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/cities_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/languages_currencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5892 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/olx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/paid_features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/payments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3186 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/threads_messages.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/user_business.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/partner/users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/checkout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/offers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/filters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/offers/offers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx/public/models/seo/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/models/seo/popular_searches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3019 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/offers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/olx_public.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/olx/public/seo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10358 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1110 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-05-22 11:20:49.000000 olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      767 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:49.386879 olx-api-wrapper-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7746 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/test_cities_and_districts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-05-22 11:20:42.000000 olx-api-wrapper-0.3.4/tests/test_users.py
```

### Comparing `olx-api-wrapper-0.3.3/LICENSE` & `olx-api-wrapper-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/PKG-INFO` & `olx-api-wrapper-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.3 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.4 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.3/README.md` & `olx-api-wrapper-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/advert_logo.py` & `olx-api-wrapper-0.3.4/olx/partner/advert_logo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/advert_statistics.py` & `olx-api-wrapper-0.3.4/olx/partner/advert_statistics.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/adverts.py` & `olx-api-wrapper-0.3.4/olx/partner/adverts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/auth.py` & `olx-api-wrapper-0.3.4/olx/partner/auth.py`

 * *Files 20% similar despite different names*

```diff
@@ -19,28 +19,42 @@
     def access_token(self):
         return self._access_token
 
     @access_token.setter
     def access_token(self, acces_token: str):
         self._access_token = acces_token
 
-    def authenticate(self, code: str = None):
+    def process_auth(self, request_data: dict) -> AuthResponse:
+        endpoint = self.endpoints["auth"]
+        response = requests.post(self.url + endpoint, json=request_data)
+
+        # TODO: Handle errors
+
+        data = from_dict(AuthResponse, response.json())
+
+        self.access_token = data.access_token
+        self.expires_in = data.expires_in
+
+        return data
+
+    def authenticate(self, code: str = None) -> AuthResponse:
         data = {
             "client_id": self.client_id,
             "client_secret": self.client_secret,
             "scope": self.current_scope,
         }
         if code:
             data["grant_type"] = "authorization_code"
             data["code"] = code
         else:
             data["grant_type"] = "client_credentials"
 
-        endpoint = self.endpoints["auth"]
-        response = requests.post(self.url + endpoint, json=data)
+        return self.process_auth(request_data=data)
 
-        # TODO: Handle errors
-
-        data = from_dict(AuthResponse, response.json())
-
-        self.access_token = data.access_token
-        self.expires_in = data.expires_in
+    def refresh(self, refresh_token: str):
+        data = {
+            "grant_type": "refresh_token",
+            "client_id": self.client_id,
+            "client_secret": self.client_secret,
+            "refresh_token": refresh_token,
+        }
+        return self.process_auth(request_data=data)
```

### Comparing `olx-api-wrapper-0.3.3/olx/partner/categories_attributes.py` & `olx-api-wrapper-0.3.4/olx/partner/categories_attributes.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/cities_districts.py` & `olx-api-wrapper-0.3.4/olx/partner/cities_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/languages_currencies.py` & `olx-api-wrapper-0.3.4/olx/partner/languages_currencies.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/models.py` & `olx-api-wrapper-0.3.4/olx/partner/models.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/olx.py` & `olx-api-wrapper-0.3.4/olx/partner/olx.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/paid_features.py` & `olx-api-wrapper-0.3.4/olx/partner/paid_features.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/payments.py` & `olx-api-wrapper-0.3.4/olx/partner/payments.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/threads_messages.py` & `olx-api-wrapper-0.3.4/olx/partner/threads_messages.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/partner/users.py` & `olx-api-wrapper-0.3.4/olx/partner/users.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/public/checkout.py` & `olx-api-wrapper-0.3.4/olx/public/checkout.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/public/models/offers/filters.py` & `olx-api-wrapper-0.3.4/olx/public/models/offers/filters.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/public/models/offers/offers.py` & `olx-api-wrapper-0.3.4/olx/public/models/offers/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/public/offers.py` & `olx-api-wrapper-0.3.4/olx/public/offers.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx/public/seo.py` & `olx-api-wrapper-0.3.4/olx/public/seo.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/PKG-INFO` & `olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olx-api-wrapper
-Version: 0.3.3
+Version: 0.3.4
 Summary: Unofficial Wrapper for OLX API
 Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: Paweł Stawikowski
 Author-email: pawikoski@gmail.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.3 Summary: Unofficial
+Metadata-Version: 2.1 Name: olx-api-wrapper Version: 0.3.4 Summary: Unofficial
 Wrapper for OLX API Home-page: https://github.com/Pawikoski/olx-api-wrapper
 Author: PaweÅ Stawikowski Author-email: pawikoski@gmail.com License: MIT
 Classifier: Development Status :: 4 - Beta Classifier: Programming Language ::
 Python :: 3.11 Classifier: License :: OSI Approved :: MIT License Classifier:
 Operating System :: OS Independent Description-Content-Type: text/markdown
 License-File: LICENSE [![Contributors][contributors-shield]][contributors-url]
 [![Forks][forks-shield]][forks-url] [![Stargazers][stars-shield]][stars-url] [!
```

### Comparing `olx-api-wrapper-0.3.3/olx_api_wrapper.egg-info/SOURCES.txt` & `olx-api-wrapper-0.3.4/olx_api_wrapper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/setup.py` & `olx-api-wrapper-0.3.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 
 with open("README.md", "r") as readme_file:
     long_description = readme_file.read()
 
 setup(
     name="olx-api-wrapper",
-    version="0.3.3",
+    version="0.3.4",
     description="Unofficial Wrapper for OLX API",
     author="Paweł Stawikowski",
     author_email="pawikoski@gmail.com",
     packages=find_packages(),
     url="https://github.com/Pawikoski/olx-api-wrapper",
     install_requires=["requests", "dacite"],
     long_description=long_description,
```

### Comparing `olx-api-wrapper-0.3.3/tests/test_cities_and_districts.py` & `olx-api-wrapper-0.3.4/tests/test_cities_and_districts.py`

 * *Files identical despite different names*

### Comparing `olx-api-wrapper-0.3.3/tests/test_users.py` & `olx-api-wrapper-0.3.4/tests/test_users.py`

 * *Files identical despite different names*

