# Comparing `tmp/st_cookies_manager-0.2.0.tar.gz` & `tmp/st_cookies_manager-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "st_cookies_manager-0.2.0.tar", max compression
+gzip compressed data, was "st_cookies_manager-0.2.1.tar", max compression
```

## Comparing `st_cookies_manager-0.2.0.tar` & `st_cookies_manager-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      452 2024-05-21 22:20:37.433197 st_cookies_manager-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1056 2024-05-21 22:19:16.534542 st_cookies_manager-0.2.0/README.md
--rw-r--r--   0        0        0      158 2021-12-25 13:07:28.302986 st_cookies_manager-0.2.0/st_cookies_manager/__init__.py
--rw-r--r--   0        0        0     3175 2021-12-25 13:19:00.787009 st_cookies_manager-0.2.0/st_cookies_manager/cookie_manager.py
--rw-r--r--   0        0        0     3655 2024-05-21 22:23:33.285083 st_cookies_manager-0.2.0/st_cookies_manager/encrypted_cookie_manager.py
--rw-r--r--   0        0        0      660 2024-05-21 22:20:31.799143 st_cookies_manager-0.2.0/st_cookies_manager/package.json
--rw-r--r--   0        0        0      142 2021-12-24 22:35:18.681804 st_cookies_manager-0.2.0/st_cookies_manager/public/index.html
--rw-r--r--   0        0        0     1468 2021-12-25 13:31:19.011431 st_cookies_manager-0.2.0/st_cookies_manager/src/index.ts
--rw-r--r--   0        0        0       40 2021-12-24 20:27:49.402720 st_cookies_manager-0.2.0/st_cookies_manager/src/react-app-env.d.ts
--rw-r--r--   0        0        0      535 2021-12-24 20:27:49.410720 st_cookies_manager-0.2.0/st_cookies_manager/tsconfig.json
--rw-r--r--   0        0        0     1600 1970-01-01 00:00:00.000000 st_cookies_manager-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      452 2024-05-21 22:33:09.314460 st_cookies_manager-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1049 2024-05-21 22:31:47.172028 st_cookies_manager-0.2.1/README.md
+-rw-r--r--   0        0        0      158 2021-12-25 13:07:28.302986 st_cookies_manager-0.2.1/st_cookies_manager/__init__.py
+-rw-r--r--   0        0        0     3175 2021-12-25 13:19:00.787009 st_cookies_manager-0.2.1/st_cookies_manager/cookie_manager.py
+-rw-r--r--   0        0        0     3655 2024-05-21 22:23:33.285083 st_cookies_manager-0.2.1/st_cookies_manager/encrypted_cookie_manager.py
+-rw-r--r--   0        0        0      660 2024-05-21 22:31:54.245020 st_cookies_manager-0.2.1/st_cookies_manager/package.json
+-rw-r--r--   0        0        0      142 2021-12-24 22:35:18.681804 st_cookies_manager-0.2.1/st_cookies_manager/public/index.html
+-rw-r--r--   0        0        0     1468 2021-12-25 13:31:19.011431 st_cookies_manager-0.2.1/st_cookies_manager/src/index.ts
+-rw-r--r--   0        0        0       40 2021-12-24 20:27:49.402720 st_cookies_manager-0.2.1/st_cookies_manager/src/react-app-env.d.ts
+-rw-r--r--   0        0        0      535 2021-12-24 20:27:49.410720 st_cookies_manager-0.2.1/st_cookies_manager/tsconfig.json
+-rw-r--r--   0        0        0     1593 1970-01-01 00:00:00.000000 st_cookies_manager-0.2.1/PKG-INFO
```

### Comparing `st_cookies_manager-0.2.0/README.md` & `st_cookies_manager-0.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Streamlit Cookies Manager
 
 Access and change browser cookies from Streamlit scripts:
 
 ```python
 import os
 import streamlit as st
-from streamlit_cookies_manager import EncryptedCookieManager
+from st_cookies_manager import EncryptedCookieManager
 
 # This should be on top of your script
 cookies = EncryptedCookieManager(
     # This prefix will get added to all your cookie names.
     # This way you can run your app on Streamlit Cloud without cookie name clashes with other apps.
     prefix="ktosiek/st-cookies-manager/",
     # You should really setup a long COOKIES_PASSWORD secret if you're running on Streamlit Cloud.
```

### Comparing `st_cookies_manager-0.2.0/st_cookies_manager/cookie_manager.py` & `st_cookies_manager-0.2.1/st_cookies_manager/cookie_manager.py`

 * *Files identical despite different names*

### Comparing `st_cookies_manager-0.2.0/st_cookies_manager/encrypted_cookie_manager.py` & `st_cookies_manager-0.2.1/st_cookies_manager/encrypted_cookie_manager.py`

 * *Files identical despite different names*

### Comparing `st_cookies_manager-0.2.0/st_cookies_manager/package.json` & `st_cookies_manager-0.2.1/st_cookies_manager/package.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'0.2.1'"}*

```diff
@@ -24,9 +24,9 @@
     "private": true,
     "scripts": {
         "build": "react-scripts build",
         "eject": "react-scripts eject",
         "start": "react-scripts start",
         "test": "react-scripts test"
     },
-    "version": "0.2.0"
+    "version": "0.2.1"
 }
```

### Comparing `st_cookies_manager-0.2.0/st_cookies_manager/src/index.ts` & `st_cookies_manager-0.2.1/st_cookies_manager/src/index.ts`

 * *Files identical despite different names*

### Comparing `st_cookies_manager-0.2.0/st_cookies_manager/tsconfig.json` & `st_cookies_manager-0.2.1/st_cookies_manager/tsconfig.json`

 * *Files identical despite different names*

### Comparing `st_cookies_manager-0.2.0/PKG-INFO` & `st_cookies_manager-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: st-cookies-manager
-Version: 0.2.0
+Version: 0.2.1
 Summary: Access and save cookies from Streamlit
 License: Apache-2.0
 Author: Eleonoraai
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -17,15 +17,15 @@
 # Streamlit Cookies Manager
 
 Access and change browser cookies from Streamlit scripts:
 
 ```python
 import os
 import streamlit as st
-from streamlit_cookies_manager import EncryptedCookieManager
+from st_cookies_manager import EncryptedCookieManager
 
 # This should be on top of your script
 cookies = EncryptedCookieManager(
     # This prefix will get added to all your cookie names.
     # This way you can run your app on Streamlit Cloud without cookie name clashes with other apps.
     prefix="ktosiek/st-cookies-manager/",
     # You should really setup a long COOKIES_PASSWORD secret if you're running on Streamlit Cloud.
```

