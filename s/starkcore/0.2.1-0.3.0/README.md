# Comparing `tmp/starkcore-0.2.1.tar.gz` & `tmp/starkcore-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starkcore-0.2.1.tar", last modified: Wed Mar  6 22:56:33 2024, max compression
+gzip compressed data, was "starkcore-0.3.0.tar", last modified: Tue May 21 23:16:56 2024, max compression
```

## Comparing `starkcore-0.2.1.tar` & `starkcore-0.3.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-03-06 22:56:33.594572 starkcore-0.2.1/
--rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.2.1/LICENSE.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.2.1/MANIFEST.in
--rw-r--r--   0 caiodottori   (501) staff       (20)      885 2024-03-06 22:56:33.594385 starkcore-0.2.1/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.2.1/README.md
--rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-03-06 22:56:33.594672 starkcore-0.2.1/setup.cfg
--rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.2.1/setup.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-03-06 22:56:33.555379 starkcore-0.2.1/starkcore/
--rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-03-06 22:55:45.000000 starkcore-0.2.1/starkcore/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.2.1/starkcore/environment.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/error.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/key.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-03-06 22:56:33.563488 starkcore-0.2.1/starkcore/user/
--rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.2.1/starkcore/user/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/user/__organization.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/user/__project.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.2.1/starkcore/user/__publicuser.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/user/__user.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-03-06 22:56:33.593954 starkcore-0.2.1/starkcore/utils/
--rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/__init__.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/api.py
--rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/cache.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/case.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.2.1/starkcore/utils/checks.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/compatibility.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/enum.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.2.1/starkcore/utils/host.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.2.1/starkcore/utils/parse.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     2780 2022-09-07 13:21:49.000000 starkcore-0.2.1/starkcore/utils/request.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/resource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)     7748 2024-03-06 22:52:50.000000 starkcore-0.2.1/starkcore/utils/rest.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.2.1/starkcore/utils/subresource.py
--rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.2.1/starkcore/utils/url.py
-drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-03-06 22:56:33.557763 starkcore-0.2.1/starkcore.egg-info/
--rw-r--r--   0 caiodottori   (501) staff       (20)      885 2024-03-06 22:56:33.000000 starkcore-0.2.1/starkcore.egg-info/PKG-INFO
--rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-03-06 22:56:33.000000 starkcore-0.2.1/starkcore.egg-info/SOURCES.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-03-06 22:56:33.000000 starkcore-0.2.1/starkcore.egg-info/dependency_links.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-03-06 22:56:33.000000 starkcore-0.2.1/starkcore.egg-info/requires.txt
--rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-03-06 22:56:33.000000 starkcore-0.2.1/starkcore.egg-info/top_level.txt
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.053411 starkcore-0.3.0/
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1068 2022-05-11 20:37:59.000000 starkcore-0.3.0/LICENSE.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       49 2022-05-11 20:37:59.000000 starkcore-0.3.0/MANIFEST.in
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-21 23:16:56.053246 starkcore-0.3.0/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      458 2022-05-11 20:37:59.000000 starkcore-0.3.0/README.md
+-rw-r--r--   0 caiodottori   (501) staff       (20)       38 2024-05-21 23:16:56.053477 starkcore-0.3.0/setup.cfg
+-rw-r--r--   0 caiodottori   (501) staff       (20)      760 2022-05-11 20:37:59.000000 starkcore-0.3.0/setup.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.011342 starkcore-0.3.0/starkcore/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      198 2024-05-21 23:16:13.000000 starkcore-0.3.0/starkcore/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      120 2022-09-05 16:45:10.000000 starkcore-0.3.0/starkcore/environment.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      846 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/error.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      898 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/key.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.023490 starkcore-0.3.0/starkcore/user/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      134 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/user/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2842 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__organization.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     1940 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__project.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      161 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/user/__publicuser.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      452 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/user/__user.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.052862 starkcore-0.3.0/starkcore/utils/
+-rw-r--r--   0 caiodottori   (501) staff       (20)       25 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/__init__.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2015 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/api.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)       12 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/cache.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      340 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/case.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2613 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/utils/checks.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      166 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/compatibility.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      264 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/enum.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      105 2022-09-07 13:21:49.000000 starkcore-0.3.0/starkcore/utils/host.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2501 2022-09-07 16:26:14.000000 starkcore-0.3.0/starkcore/utils/parse.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     2886 2024-05-21 23:14:22.000000 starkcore-0.3.0/starkcore/utils/request.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      311 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/resource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)     9218 2024-05-21 23:14:22.000000 starkcore-0.3.0/starkcore/utils/rest.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      614 2022-05-11 20:37:59.000000 starkcore-0.3.0/starkcore/utils/subresource.py
+-rw-r--r--   0 caiodottori   (501) staff       (20)      600 2023-05-19 17:51:46.000000 starkcore-0.3.0/starkcore/utils/url.py
+drwxr-xr-x   0 caiodottori   (501) staff       (20)        0 2024-05-21 23:16:56.013517 starkcore-0.3.0/starkcore.egg-info/
+-rw-r--r--   0 caiodottori   (501) staff       (20)      804 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/PKG-INFO
+-rw-r--r--   0 caiodottori   (501) staff       (20)      798 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/SOURCES.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)        1 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/dependency_links.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       40 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/requires.txt
+-rw-r--r--   0 caiodottori   (501) staff       (20)       16 2024-05-21 23:16:55.000000 starkcore-0.3.0/starkcore.egg-info/top_level.txt
```

### Comparing `starkcore-0.2.1/LICENSE.txt` & `starkcore-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/PKG-INFO` & `starkcore-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.2.1
+Version: 0.3.0
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
-Description: # Stark Core Python SDK
-        
-        Welcome to the Stark Core Python SDK!
-        This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
-        
-        # Help and Feedback
-        
-        If you have any questions about our SDK, just send us an email.
-        We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
-        We also love feedback, so don't be shy about sharing your thoughts with us.
-        
-        Email: help@starkbank.com
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Stark Core Python SDK
+
+Welcome to the Stark Core Python SDK!
+This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
+
+# Help and Feedback
+
+If you have any questions about our SDK, just send us an email.
+We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
+We also love feedback, so don't be shy about sharing your thoughts with us.
+
+Email: help@starkbank.com
+
+
```

### Comparing `starkcore-0.2.1/setup.py` & `starkcore-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/error.py` & `starkcore-0.3.0/starkcore/error.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/key.py` & `starkcore-0.3.0/starkcore/key.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/user/__organization.py` & `starkcore-0.3.0/starkcore/user/__organization.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/user/__project.py` & `starkcore-0.3.0/starkcore/user/__project.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/utils/api.py` & `starkcore-0.3.0/starkcore/utils/api.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/utils/checks.py` & `starkcore-0.3.0/starkcore/utils/checks.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/utils/parse.py` & `starkcore-0.3.0/starkcore/utils/parse.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/utils/request.py` & `starkcore-0.3.0/starkcore/utils/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 from .url import urlencode
 from .checks import check_user, check_language
 from ..user.__publicuser import PublicUser
 
 
 class Response:
 
-    def __init__(self, status, content):
+    def __init__(self, status, content, headers):
         self.status = status
         self.content = content
+        self.headers = headers
 
     def json(self):
         return loads(self.content.decode("utf-8"))
 
 
 def fetch(host, sdk_version, user, method, path, payload=None, query=None,
-          api_version="v2", language="en-US", timeout=15):
+          prefix="", api_version="v2", language="en-US", timeout=15):
     user = check_user(user)
     language = check_language(language)
 
     service = {
         StarkHost.infra: "starkinfra",
         StarkHost.bank: "starkbank",
         StarkHost.sign: "starksign",
@@ -34,15 +35,16 @@
     url = {
         Environment.production:  "https://api.{service}.com/",
         Environment.sandbox:     "https://sandbox.api.{service}.com/",
     }[user.environment].format(service=service) + api_version
 
     url = "{base_url}/{path}{query}".format(base_url=url, path=path, query=urlencode(query))
 
-    agent = "Python-{major}.{minor}.{micro}-SDK-{host}-{sdk_version}".format(
+    agent = "{prefix}Python-{major}.{minor}.{micro}-SDK-{host}-{sdk_version}".format(
+        prefix=prefix + "-" if prefix else "",
         major=python_version.major,
         minor=python_version.minor,
         micro=python_version.micro,
         host=host,
         sdk_version=sdk_version,
     )
```

### Comparing `starkcore-0.2.1/starkcore/utils/rest.py` & `starkcore-0.3.0/starkcore/utils/rest.py`

 * *Files 10% similar despite different names*

```diff
@@ -204,42 +204,43 @@
         language=language,
         timeout=timeout,
     ).json()
     entity = json[last_name(resource)]
     return from_api_json(resource, entity)
 
 
-def get_raw(sdk_version, host, api_version, path, user, language, timeout, **query):
-    return fetch(
+def get_raw(sdk_version, host, api_version, path, user, language, timeout, query):
+    return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
         method=get,
         path=path,
         query=query,
         api_version=api_version,
+        prefix="Joker",
         language=language,
         timeout=timeout,
-    ).json()
+    ))
 
 
 def post_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
-    return fetch(
+    return _parse_response_data(fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
         method=post,
         path=path,
         payload=payload,
         query=query,
         api_version=api_version,
+        prefix="Joker",
         language=language,
         timeout=timeout,
-    ).json()
-
+    ))
 
 
 def put_multi(sdk_version, host, api_version, user, resource, entities, language, timeout, **query):
     json = fetch(
         host=host,
         sdk_version=sdk_version,
         user=user,
@@ -249,7 +250,61 @@
         query=query,
         api_version=api_version,
         language=language,
         timeout=timeout,
     ).json()
     entities = json[last_name_plural(resource)]
     return [from_api_json(resource, entity) for entity in entities]
+
+
+def patch_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+    return _parse_response_data(fetch(
+        host=host,
+        sdk_version=sdk_version,
+        user=user,
+        method=patch,
+        path=path,
+        payload=payload,
+        query=query,
+        api_version=api_version,
+        prefix="Joker",
+        language=language,
+        timeout=timeout,
+    ))
+
+
+def put_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+    return _parse_response_data(fetch(
+        host=host,
+        sdk_version=sdk_version,
+        user=user,
+        method=put,
+        path=path,
+        payload=payload,
+        query=query,
+        api_version=api_version,
+        prefix="Joker",
+        language=language,
+        timeout=timeout,
+    ))
+
+
+def delete_raw(sdk_version, host, api_version, path, payload, user, language, timeout, **query):
+    return _parse_response_data(fetch(
+        host=host,
+        sdk_version=sdk_version,
+        user=user,
+        method=delete,
+        path=path,
+        payload=payload,
+        query=query,
+        api_version=api_version,
+        prefix="Joker",
+        language=language,
+        timeout=timeout,
+    ))
+
+
+def _parse_response_data(response):
+    if response.headers.get("content-type") == "application/json":
+        return response.json()
+    return response.content
```

### Comparing `starkcore-0.2.1/starkcore/utils/subresource.py` & `starkcore-0.3.0/starkcore/utils/subresource.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore/utils/url.py` & `starkcore-0.3.0/starkcore/utils/url.py`

 * *Files identical despite different names*

### Comparing `starkcore-0.2.1/starkcore.egg-info/PKG-INFO` & `starkcore-0.3.0/starkcore.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 Metadata-Version: 2.1
 Name: starkcore
-Version: 0.2.1
+Version: 0.3.0
 Summary: Basic SDK functionalities for the starkbank and starkinfra SDKs
 Home-page: https://github.com/starkinfra/core-python
 Author: Stark Infra
 Author-email: developers@starkbank.com
 License: MIT License
-Description: # Stark Core Python SDK
-        
-        Welcome to the Stark Core Python SDK!
-        This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
-        
-        # Help and Feedback
-        
-        If you have any questions about our SDK, just send us an email.
-        We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
-        We also love feedback, so don't be shy about sharing your thoughts with us.
-        
-        Email: help@starkbank.com
-        
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+# Stark Core Python SDK
+
+Welcome to the Stark Core Python SDK!
+This tool offers the basic functionalities used by our starkbank and starkinfra Python SDKs to operate our APIs. 
+
+# Help and Feedback
+
+If you have any questions about our SDK, just send us an email.
+We will respond you quickly, pinky promise. We are here to help you integrate with us ASAP.
+We also love feedback, so don't be shy about sharing your thoughts with us.
+
+Email: help@starkbank.com
+
+
```

### Comparing `starkcore-0.2.1/starkcore.egg-info/SOURCES.txt` & `starkcore-0.3.0/starkcore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

