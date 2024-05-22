# Comparing `tmp/crudfastapi-0.0.4.tar.gz` & `tmp/crudfastapi-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.4.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.5.tar", max compression
```

## Comparing `crudfastapi-0.0.4.tar` & `crudfastapi-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    72803 2024-05-15 05:36:35.751891 crudfastapi-0.0.4/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.4/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-15 05:37:08.847450 crudfastapi-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.4/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    72734 2024-05-15 05:56:30.545248 crudfastapi-0.0.5/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.5/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-15 05:56:56.510276 crudfastapi-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.5/PKG-INFO
```

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.5/CRUDFastAPI/crud/fast_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -675,22 +675,20 @@
                 if join_filters:
                     base_query = base_query.where(*join_filters)
 
             if primary_filters:
                 base_query = base_query.where(*primary_filters)
 
             subquery = base_query.subquery()
-            print(base_query, subquery)
             count_query = select(func.count()).select_from(subquery)
         else:
             count_query = select(func.count()).select_from(self.model)
             if primary_filters:
                 count_query = count_query.where(*primary_filters)
 
-        print(count_query)
         total_count: Optional[int] = await db.scalar(count_query)
         if total_count is None:
             raise ValueError("Could not find the count.")
 
         return total_count
 
     async def get_multi(
```

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.5/CRUDFastAPI/crud/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.5/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.5/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.5/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.5/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.5/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.5/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/LICENSE` & `crudfastapi-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/pyproject.toml` & `crudfastapi-0.0.5/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CRUDFastAPI"
-version = "0.0.4"
+version = "0.0.5"
 description = "CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Mithun Thomas <mithunthomas003@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mithun2003/CRUDFastAPI"
 include = ["LICENSE"]
```

### Comparing `crudfastapi-0.0.4/README.md` & `crudfastapi-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.4/PKG-INFO` & `crudfastapi-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.4
+Version: 0.0.5
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

