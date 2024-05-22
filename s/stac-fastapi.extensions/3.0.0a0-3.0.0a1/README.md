# Comparing `tmp/stac_fastapi_extensions-3.0.0a0.tar.gz` & `tmp/stac_fastapi_extensions-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_extensions-3.0.0a0.tar", last modified: Mon May  6 16:07:34 2024, max compression
+gzip compressed data, was "stac_fastapi_extensions-3.0.0a1.tar", last modified: Wed May 22 11:04:01 2024, max compression
```

## Comparing `stac_fastapi_extensions-3.0.0a0.tar` & `stac_fastapi_extensions-3.0.0a1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-06 16:07:34.714635 stac_fastapi_extensions-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.702635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.706635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.706635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/context.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/pagination.py
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/token_pagination.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/query.py
--rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/request.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     7704 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/bulk_transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:34.000000 stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:34.710635 stac_fastapi_extensions-3.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-06 16:07:22.000000 stac_fastapi_extensions-3.0.0a0/tests/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.164817 stac_fastapi_extensions-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-22 11:04:01.164817 stac_fastapi_extensions-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-22 11:04:01.164817 stac_fastapi_extensions-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.156817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.156817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/context.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2399 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4700 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/pagination.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/token_pagination.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/query/
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/query/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)      468 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/query/request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8130 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/third_party/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/third_party/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/third_party/bulk_transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1353 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:04:01.000000 stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:04:01.160817 stac_fastapi_extensions-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5884 2024-05-22 11:03:45.000000 stac_fastapi_extensions-3.0.0a1/tests/test_transaction.py
```

### Comparing `stac_fastapi_extensions-3.0.0a0/PKG-INFO` & `stac_fastapi_extensions-3.0.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_extensions-3.0.0a0/setup.py` & `stac_fastapi_extensions-3.0.0a1/setup.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/__init__.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/__init__.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/context.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/context.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/fields.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/fields.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/fields/request.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/fields/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/filter.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/filter.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/filter/request.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/filter/request.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,31 +1,17 @@
 """Filter extension request models."""
 
-from enum import Enum
-from typing import Any, Dict, Optional
+from typing import Any, Dict, Literal, Optional
 
 import attr
 from pydantic import BaseModel, Field
 
 from stac_fastapi.types.search import APIRequest
 
-
-class FilterLang(str, Enum):
-    """Choices for filter-lang value in a POST request.
-
-    Based on
-    https://github.com/stac-api-extensions/filter#queryables
-
-    Note the addition of cql2-json, which is used by the pgstac backend,
-    but is not included in the spec above.
-    """
-
-    cql_json = "cql-json"
-    cql2_json = "cql2-json"
-    cql2_text = "cql2-text"
+FilterLang = Literal["cql-json", "cql2-json", "cql2-text"]
 
 
 @attr.s
 class FilterExtensionGetRequest(APIRequest):
     """Filter extension GET request model."""
 
     filter: Optional[str] = attr.ib(default=None)
```

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/pagination.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/pagination/token_pagination.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/pagination/token_pagination.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/query/query.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/query/query.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/request.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/request.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/sort/sort.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/sort/sort.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/core/transaction.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/core/transaction.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,25 +45,28 @@
         POST /collections
         PUT /collections/{collection_id}
         DELETE /collections/{collection_id}
         POST /collections/{collection_id}/items
         PUT /collections/{collection_id}/items
         DELETE /collections/{collection_id}/items
 
-    https://github.com/radiantearth/stac-api-spec/blob/master/ogcapi-features/extensions/transaction/README.md
+    https://github.com/stac-api-extensions/transaction
+    https://github.com/stac-api-extensions/collection-transaction
 
     Attributes:
         client: CRUD application logic
+
     """
 
     client: Union[AsyncBaseTransactionsClient, BaseTransactionsClient] = attr.ib()
     settings: ApiSettings = attr.ib()
     conformance_classes: List[str] = attr.ib(
         factory=lambda: [
-            "https://api.stacspec.org/v1.0.0-rc.3/ogcapi-features/extensions/transaction",
+            "https://api.stacspec.org/v1.0.0/ogcapi-features/extensions/transaction",
+            "https://api.stacspec.org/v1.0.0/collections/extensions/transaction",
         ]
     )
     schema_href: Optional[str] = attr.ib(default=None)
     router: APIRouter = attr.ib(factory=APIRouter)
     response_class: Type[Response] = attr.ib(default=JSONResponse)
 
     def register_create_item(self):
@@ -128,14 +131,19 @@
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=create_async_endpoint(self.client.delete_item, ItemUri),
         )
 
+    def register_patch_item(self):
+        """Register patch item endpoint (PATCH
+        /collections/{collection_id}/items/{item_id})."""
+        raise NotImplementedError
+
     def register_create_collection(self):
         """Register create collection endpoint (POST /collections)."""
         self.router.add_api_route(
             name="Create Collection",
             path="/collections",
             status_code=201,
             response_model=Collection if self.settings.enable_response_models else None,
@@ -192,14 +200,18 @@
             response_class=self.response_class,
             response_model_exclude_unset=True,
             response_model_exclude_none=True,
             methods=["DELETE"],
             endpoint=create_async_endpoint(self.client.delete_collection, CollectionUri),
         )
 
+    def register_patch_collection(self):
+        """Register patch collection endpoint (PATCH /collections/{collection_id})."""
+        raise NotImplementedError
+
     def register(self, app: FastAPI) -> None:
         """Register the extension with a FastAPI application.
 
         Args:
             app: target FastAPI application.
 
         Returns:
```

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi/extensions/third_party/bulk_transactions.py` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi/extensions/third_party/bulk_transactions.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/PKG-INFO` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.extensions
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
```

### Comparing `stac_fastapi_extensions-3.0.0a0/stac_fastapi.extensions.egg-info/SOURCES.txt` & `stac_fastapi_extensions-3.0.0a1/stac_fastapi.extensions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_extensions-3.0.0a0/tests/test_transaction.py` & `stac_fastapi_extensions-3.0.0a1/tests/test_transaction.py`

 * *Files identical despite different names*

