# Comparing `tmp/uploadthing_py-0.3.0.tar.gz` & `tmp/uploadthing_py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uploadthing_py-0.3.0.tar", max compression
+gzip compressed data, was "uploadthing_py-0.3.1.tar", max compression
```

## Comparing `uploadthing_py-0.3.0.tar` & `uploadthing_py-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     2538 2024-05-20 13:13:12.737624 uploadthing_py-0.3.0/README.md
--rw-r--r--   0        0        0      618 2024-05-21 22:29:25.977438 uploadthing_py-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      663 2024-05-20 12:38:08.833457 uploadthing_py-0.3.0/uploadthing_py/__init__.py
--rw-r--r--   0        0        0     1323 2024-05-20 13:14:21.791225 uploadthing_py-0.3.0/uploadthing_py/builder.py
--rw-r--r--   0        0        0        0 2024-05-19 21:14:05.647788 uploadthing_py-0.3.0/uploadthing_py/py.typed
--rw-r--r--   0        0        0    11603 2024-05-21 22:23:50.569456 uploadthing_py-0.3.0/uploadthing_py/request_handler.py
--rw-r--r--   0        0        0     3719 2024-05-21 22:02:20.251415 uploadthing_py-0.3.0/uploadthing_py/types.py
--rw-r--r--   0        0        0     5555 2024-05-21 21:50:15.091165 uploadthing_py-0.3.0/uploadthing_py/utapi.py
--rw-r--r--   0        0        0     1373 2024-05-21 22:28:42.631048 uploadthing_py-0.3.0/uploadthing_py/utils.py
--rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     2538 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/README.md
+-rw-r--r--   0        0        0      627 2024-05-21 23:06:08.828448 uploadthing_py-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      663 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/__init__.py
+-rw-r--r--   0        0        0     1323 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/builder.py
+-rw-r--r--   0        0        0        0 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/py.typed
+-rw-r--r--   0        0        0    11603 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/request_handler.py
+-rw-r--r--   0        0        0     3719 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/types.py
+-rw-r--r--   0        0        0     5561 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/utapi.py
+-rw-r--r--   0        0        0     1385 2024-05-21 23:05:56.008420 uploadthing_py-0.3.1/uploadthing_py/utils.py
+-rw-r--r--   0        0        0     2893 1970-01-01 00:00:00.000000 uploadthing_py-0.3.1/PKG-INFO
```

### Comparing `uploadthing_py-0.3.0/README.md` & `uploadthing_py-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.0/uploadthing_py/__init__.py` & `uploadthing_py-0.3.1/uploadthing_py/__init__.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.0/uploadthing_py/builder.py` & `uploadthing_py-0.3.1/uploadthing_py/builder.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.0/uploadthing_py/request_handler.py` & `uploadthing_py-0.3.1/uploadthing_py/request_handler.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.0/uploadthing_py/types.py` & `uploadthing_py-0.3.1/uploadthing_py/types.py`

 * *Files identical despite different names*

### Comparing `uploadthing_py-0.3.0/uploadthing_py/utapi.py` & `uploadthing_py-0.3.1/uploadthing_py/utapi.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,9 @@
-import typing as t, logging
+import typing as t
+import logging
 from httpx import AsyncClient, Response
 
 import uploadthing_py
 from uploadthing_py.types import (
     ACL,
     MaybeList,
     File,
```

### Comparing `uploadthing_py-0.3.0/uploadthing_py/utils.py` & `uploadthing_py-0.3.1/uploadthing_py/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-import dataclasses, json, typing as t
+import dataclasses
+import json
+import typing as t
 import hmac
 from hashlib import sha256
 
 
 def json_stringify(o):
     class EnhancedJSONEncoder(json.JSONEncoder):
         def default(self, o):
```

### Comparing `uploadthing_py-0.3.0/PKG-INFO` & `uploadthing_py-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uploadthing.py
-Version: 0.3.0
+Version: 0.3.1
 Summary: Python SDK for UploadThing
 License: MIT
 Author: juliusmarminge
 Author-email: julius0216@outlook.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

