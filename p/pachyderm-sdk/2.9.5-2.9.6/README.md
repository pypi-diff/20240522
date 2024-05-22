# Comparing `tmp/pachyderm_sdk-2.9.5.tar.gz` & `tmp/pachyderm_sdk-2.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pachyderm_sdk-2.9.5.tar", max compression
+gzip compressed data, was "pachyderm_sdk-2.9.6.tar", max compression
```

## Comparing `pachyderm_sdk-2.9.5.tar` & `pachyderm_sdk-2.9.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0     2913 2024-04-24 19:01:12.229202 pachyderm_sdk-2.9.5/README.md
--rw-r--r--   0        0        0      357 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/__init__.py
--rw-r--r--   0        0        0      645 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/__main__.py
--rw-r--r--   0        0        0        8 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/.gitignore
--rw-r--r--   0        0        0       66 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/__init__.py
--rw-r--r--   0        0        0     3172 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/__init__.py
--rw-r--r--   0        0        0     1036 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/extension.py
--rw-r--r--   0        0        0    31384 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/auth/__init__.py
--rw-r--r--   0        0        0    13046 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/__init__.py
--rw-r--r--   0        0        0     1609 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/extension.py
--rw-r--r--   0        0        0     8236 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/enterprise/__init__.py
--rw-r--r--   0        0        0    12315 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/identity/__init__.py
--rw-r--r--   0        0        0    10507 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/license/__init__.py
--rw-r--r--   0        0        0    56747 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/__init__.py
--rw-r--r--   0        0        0     5447 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/_additions.py
--rw-r--r--   0        0        0    25802 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/extension.py
--rw-r--r--   0        0        0     4018 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/file.py
--rw-r--r--   0        0        0    14258 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pjs/__init__.py
--rw-r--r--   0        0        0    75621 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/__init__.py
--rw-r--r--   0        0        0      679 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/_additions.py
--rw-r--r--   0        0        0     4175 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/extension.py
--rw-r--r--   0        0        0     1113 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/taskapi/__init__.py
--rw-r--r--   0        0        0     6822 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/__init__.py
--rw-r--r--   0        0        0     3614 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/extension.py
--rw-r--r--   0        0        0     1375 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/version/__init__.py
--rw-r--r--   0        0        0     2866 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/__init__.py
--rw-r--r--   0        0        0     1872 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/extension.py
--rw-r--r--   0        0        0    11519 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/client.py
--rw-r--r--   0        0        0     7114 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/config.py
--rw-r--r--   0        0        0     1083 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/constants.py
--rw-r--r--   0        0        0     1570 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/datum_batching.py
--rw-r--r--   0        0        0     1045 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/errors.py
--rw-r--r--   0        0        0     3439 2024-04-24 19:01:12.233202 pachyderm_sdk-2.9.5/pachyderm_sdk/interceptor.py
--rw-r--r--   0        0        0     1490 2024-04-24 19:01:51.973537 pachyderm_sdk-2.9.5/pyproject.toml
--rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.5/PKG-INFO
+-rw-r--r--   0        0        0     2913 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/README.md
+-rw-r--r--   0        0        0      357 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/__init__.py
+-rw-r--r--   0        0        0      645 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/__main__.py
+-rw-r--r--   0        0        0        8 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/.gitignore
+-rw-r--r--   0        0        0       66 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/__init__.py
+-rw-r--r--   0        0        0     3172 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/admin/__init__.py
+-rw-r--r--   0        0        0     1036 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/admin/extension.py
+-rw-r--r--   0        0        0    31384 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/auth/__init__.py
+-rw-r--r--   0        0        0    13046 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/debug/__init__.py
+-rw-r--r--   0        0        0     1609 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/debug/extension.py
+-rw-r--r--   0        0        0     8236 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/enterprise/__init__.py
+-rw-r--r--   0        0        0    12315 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/identity/__init__.py
+-rw-r--r--   0        0        0    10507 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/license/__init__.py
+-rw-r--r--   0        0        0    56747 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/__init__.py
+-rw-r--r--   0        0        0     5447 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/_additions.py
+-rw-r--r--   0        0        0    25802 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/extension.py
+-rw-r--r--   0        0        0     4018 2024-05-14 19:14:34.808304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/file.py
+-rw-r--r--   0        0        0    14258 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pjs/__init__.py
+-rw-r--r--   0        0        0    75621 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/__init__.py
+-rw-r--r--   0        0        0      679 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/_additions.py
+-rw-r--r--   0        0        0     4175 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/extension.py
+-rw-r--r--   0        0        0     1113 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/taskapi/__init__.py
+-rw-r--r--   0        0        0     6822 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/transaction/__init__.py
+-rw-r--r--   0        0        0     3614 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/transaction/extension.py
+-rw-r--r--   0        0        0     1375 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/version/__init__.py
+-rw-r--r--   0        0        0     2866 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/worker/__init__.py
+-rw-r--r--   0        0        0     1872 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/api/worker/extension.py
+-rw-r--r--   0        0        0    11519 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/client.py
+-rw-r--r--   0        0        0     7114 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/config.py
+-rw-r--r--   0        0        0     1083 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/constants.py
+-rw-r--r--   0        0        0     1570 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/datum_batching.py
+-rw-r--r--   0        0        0     1045 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/errors.py
+-rw-r--r--   0        0        0     3439 2024-05-14 19:14:34.812304 pachyderm_sdk-2.9.6/pachyderm_sdk/interceptor.py
+-rw-r--r--   0        0        0     1490 2024-05-14 19:15:14.276617 pachyderm_sdk-2.9.6/pyproject.toml
+-rw-r--r--   0        0        0     4289 1970-01-01 00:00:00.000000 pachyderm_sdk-2.9.6/PKG-INFO
```

### Comparing `pachyderm_sdk-2.9.5/README.md` & `pachyderm_sdk-2.9.6/README.md`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/__main__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/__main__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/admin/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/admin/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/auth/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/debug/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/debug/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/debug/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/enterprise/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/enterprise/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/identity/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/identity/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/license/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/license/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/_additions.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pfs/file.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pfs/file.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pjs/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pjs/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/_additions.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/_additions.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/pps/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/pps/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/taskapi/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/taskapi/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/transaction/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/transaction/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/transaction/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/version/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/version/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/__init__.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/worker/__init__.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/api/worker/extension.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/api/worker/extension.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/client.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/client.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/config.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/config.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/constants.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/constants.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/datum_batching.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/datum_batching.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/errors.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/errors.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pachyderm_sdk/interceptor.py` & `pachyderm_sdk-2.9.6/pachyderm_sdk/interceptor.py`

 * *Files identical despite different names*

### Comparing `pachyderm_sdk-2.9.5/pyproject.toml` & `pachyderm_sdk-2.9.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pachyderm_sdk"
-version = "2.9.5"
+version = "2.9.6"
 description = "Python Pachyderm Client"
 authors = ["Pachyderm Integrations <integrations@pachyderm.io>"]
 license = "Apache 2.0"
 documentation = "https://docs.pachyderm.com/latest/sdk/python/"
 readme = 'README.md'
 repository = "https://github.com/pachyderm/pachyderm/tree/master/python-sdk"
 keywords = ["pachyderm"]
```

### Comparing `pachyderm_sdk-2.9.5/PKG-INFO` & `pachyderm_sdk-2.9.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pachyderm-sdk
-Version: 2.9.5
+Version: 2.9.6
 Summary: Python Pachyderm Client
 Home-page: https://github.com/pachyderm/pachyderm/tree/master/python-sdk
 License: Apache 2.0
 Keywords: pachyderm
 Author: Pachyderm Integrations
 Author-email: integrations@pachyderm.io
 Requires-Python: >=3.8,<4.0
```

