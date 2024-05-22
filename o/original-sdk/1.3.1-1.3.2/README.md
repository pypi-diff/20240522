# Comparing `tmp/original_sdk-1.3.1.tar.gz` & `tmp/original_sdk-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "original_sdk-1.3.1.tar", last modified: Fri May 10 15:21:40 2024, max compression
+gzip compressed data, was "original_sdk-1.3.2.tar", last modified: Wed May 22 09:15:00 2024, max compression
```

## Comparing `original_sdk-1.3.1.tar` & `original_sdk-1.3.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-10 15:21:32.000000 original_sdk-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-10 15:21:32.000000 original_sdk-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    25099 2024-05-10 15:21:40.647016 original_sdk-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24151 2024-05-10 15:21:32.000000 original_sdk-1.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/__pkg__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/async_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/base/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/base/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk/types/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/original_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/types/rate_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-10 15:21:32.000000 original_sdk-1.3.1/original_sdk/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 15:21:40.647016 original_sdk-1.3.1/original_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    25099 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-10 15:21:40.000000 original_sdk-1.3.1/original_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-10 15:21:32.000000 original_sdk-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 15:21:40.647016 original_sdk-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1788 2024-05-10 15:21:32.000000 original_sdk-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:00.191332 original_sdk-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 09:14:48.000000 original_sdk-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 09:14:48.000000 original_sdk-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    25091 2024-05-22 09:15:00.191332 original_sdk-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24143 2024-05-22 09:14:48.000000 original_sdk-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:00.187332 original_sdk-1.3.2/original_sdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/__pkg__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8647 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/async_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:00.191332 original_sdk-1.3.2/original_sdk/base/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9723 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/base/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:00.191332 original_sdk-1.3.2/original_sdk/types/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/types/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2858 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/types/original_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/types/rate_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      449 2024-05-22 09:14:48.000000 original_sdk-1.3.2/original_sdk/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 09:15:00.191332 original_sdk-1.3.2/original_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    25091 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 09:15:00.000000 original_sdk-1.3.2/original_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-05-22 09:14:48.000000 original_sdk-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 09:15:00.191332 original_sdk-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-05-22 09:14:48.000000 original_sdk-1.3.2/setup.py
```

### Comparing `original_sdk-1.3.1/LICENSE` & `original_sdk-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/PKG-INFO` & `original_sdk-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: original_sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python client for Original.
 Home-page: https://github.com/GetOriginal/original-python
 Author: Alexander Turowicz
 Author-email: support@getoriginal.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -284,15 +284,15 @@
         "is_transferable": True,
         "is_editing": False,
         "mint_for_user_uid": "885810911461",
         "owner_user_uid": "885810911461",
         "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
         "metadata": {
             "name": "random name",
-            "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+            "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "description": "nft_description",
             "original_id": "151854912345",
             "external_url": "external_url@example.com",
             "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "attributes": [
                 {
                     "trait_type": "Stamina Increase",
@@ -332,15 +332,15 @@
             "is_transferable": True,
             "is_editing": False,
             "mint_for_user_uid": "885810911461",
             "owner_user_uid": "885810911461",
             "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
             "metadata": {
                 "name": "random name",
-                "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+                "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "description": "nft_description",
                 "original_id": "151854912345",
                 "external_url": "external_url@example.com",
                 "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "attributes": [
                     {
                         "trait_type": "Stamina Increase",
```

### Comparing `original_sdk-1.3.1/README.md` & `original_sdk-1.3.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -259,15 +259,15 @@
         "is_transferable": True,
         "is_editing": False,
         "mint_for_user_uid": "885810911461",
         "owner_user_uid": "885810911461",
         "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
         "metadata": {
             "name": "random name",
-            "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+            "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "description": "nft_description",
             "original_id": "151854912345",
             "external_url": "external_url@example.com",
             "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "attributes": [
                 {
                     "trait_type": "Stamina Increase",
@@ -307,15 +307,15 @@
             "is_transferable": True,
             "is_editing": False,
             "mint_for_user_uid": "885810911461",
             "owner_user_uid": "885810911461",
             "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
             "metadata": {
                 "name": "random name",
-                "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+                "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "description": "nft_description",
                 "original_id": "151854912345",
                 "external_url": "external_url@example.com",
                 "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "attributes": [
                     {
                         "trait_type": "Stamina Increase",
```

### Comparing `original_sdk-1.3.1/original_sdk/async_client.py` & `original_sdk-1.3.2/original_sdk/async_client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/original_sdk/base/client.py` & `original_sdk-1.3.2/original_sdk/base/client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/original_sdk/client.py` & `original_sdk-1.3.2/original_sdk/client.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/original_sdk/types/exceptions.py` & `original_sdk-1.3.2/original_sdk/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/original_sdk/types/original_response.py` & `original_sdk-1.3.2/original_sdk/types/original_response.py`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/original_sdk.egg-info/PKG-INFO` & `original_sdk-1.3.2/original_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: original-sdk
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python client for Original.
 Home-page: https://github.com/GetOriginal/original-python
 Author: Alexander Turowicz
 Author-email: support@getoriginal.com
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -284,15 +284,15 @@
         "is_transferable": True,
         "is_editing": False,
         "mint_for_user_uid": "885810911461",
         "owner_user_uid": "885810911461",
         "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
         "metadata": {
             "name": "random name",
-            "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+            "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "description": "nft_description",
             "original_id": "151854912345",
             "external_url": "external_url@example.com",
             "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
             "attributes": [
                 {
                     "trait_type": "Stamina Increase",
@@ -332,15 +332,15 @@
             "is_transferable": True,
             "is_editing": False,
             "mint_for_user_uid": "885810911461",
             "owner_user_uid": "885810911461",
             "owner_address": "0x32e28bfe647939d073d39113c697a11e3065ea97",
             "metadata": {
                 "name": "random name",
-                "image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
+                "image": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "description": "nft_description",
                 "original_id": "151854912345",
                 "external_url": "external_url@example.com",
                 "org_image_url": "https://cryptopunks.app/cryptopunks/cryptopunk1081.png",
                 "attributes": [
                     {
                         "trait_type": "Stamina Increase",
```

### Comparing `original_sdk-1.3.1/original_sdk.egg-info/SOURCES.txt` & `original_sdk-1.3.2/original_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/pyproject.toml` & `original_sdk-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `original_sdk-1.3.1/setup.py` & `original_sdk-1.3.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "requests>=2.22.0,<3",
     "aiodns>=2.0.0",
     "aiohttp>=3.6.0,<4",
     "aiofile>=3.1,<4",
     "pyjwt>=2.0.0,<3",
     "typing_extensions; python_version < '3.8'",
 ]
-tests_require = ["pytest<=8.1.1", "pytest-asyncio<=0.21.1", "python-dotenv"]
+tests_require = ["globals", "pytest<=8.1.1", "pytest-asyncio<=0.21.1", "python-dotenv"]
 ci_require = [
     "black",
     "flake8",
     "flake8-isort",
     "flake8-bugbear",
     "pytest-cov",
     "mypy",
```

