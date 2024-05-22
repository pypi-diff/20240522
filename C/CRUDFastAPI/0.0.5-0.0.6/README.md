# Comparing `tmp/crudfastapi-0.0.5.tar.gz` & `tmp/crudfastapi-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crudfastapi-0.0.5.tar", max compression
+gzip compressed data, was "crudfastapi-0.0.6.tar", max compression
```

## Comparing `crudfastapi-0.0.5.tar` & `crudfastapi-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/__init__.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/crud/__init__.py
--rw-r--r--   0        0        0    72734 2024-05-15 05:56:30.545248 crudfastapi-0.0.5/CRUDFastAPI/crud/fast_crud.py
--rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.5/CRUDFastAPI/crud/helper.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/__init__.py
--rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/crud_router.py
--rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/endpoint_creator.py
--rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/endpoint/helper.py
--rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/exceptions/__init__.py
--rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/exceptions/http_exceptions.py
--rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/__init__.py
--rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/helper.py
--rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/response.py
--rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/paginated/schemas.py
--rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/CRUDFastAPI/py.typed
--rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/LICENSE
--rw-r--r--   0        0        0     1498 2024-05-15 05:56:56.510276 crudfastapi-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.5/README.md
--rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      403 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/crud/__init__.py
+-rw-r--r--   0        0        0    73003 2024-05-22 08:16:17.811640 crudfastapi-0.0.6/CRUDFastAPI/crud/fast_crud.py
+-rw-r--r--   0        0        0     6121 2024-05-15 05:35:59.523525 crudfastapi-0.0.6/CRUDFastAPI/crud/helper.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/endpoint/__init__.py
+-rw-r--r--   0        0        0    10362 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/endpoint/crud_router.py
+-rw-r--r--   0        0        0    24496 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/endpoint/endpoint_creator.py
+-rw-r--r--   0        0        0     3993 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/endpoint/helper.py
+-rw-r--r--   0        0        0       64 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/exceptions/__init__.py
+-rw-r--r--   0        0        0     2105 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/exceptions/http_exceptions.py
+-rw-r--r--   0        0        0      255 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/paginated/__init__.py
+-rw-r--r--   0        0        0      821 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/paginated/helper.py
+-rw-r--r--   0        0        0     1034 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/paginated/response.py
+-rw-r--r--   0        0        0      397 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/paginated/schemas.py
+-rw-r--r--   0        0        0        0 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/CRUDFastAPI/py.typed
+-rw-r--r--   0        0        0     1088 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1498 2024-05-22 08:18:14.584652 crudfastapi-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8347 2024-05-14 02:36:21.061981 crudfastapi-0.0.6/README.md
+-rw-r--r--   0        0        0     9370 1970-01-01 00:00:00.000000 crudfastapi-0.0.6/PKG-INFO
```

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/crud/fast_crud.py` & `crudfastapi-0.0.6/CRUDFastAPI/crud/fast_crud.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import Any, Generic, TypeVar, Union, Optional
-from datetime import datetime, timezone
+from datetime import datetime, timezone, UTC
 
 from pydantic import BaseModel, ValidationError
 from sqlalchemy import select, update, delete, func, inspect, asc, desc, or_
 from sqlalchemy.exc import ArgumentError, MultipleResultsFound, NoResultFound
 from sqlalchemy.sql import Join
 from sqlalchemy.ext.asyncio import AsyncSession
 from sqlalchemy.engine.row import Row
@@ -1477,14 +1477,15 @@
 
     async def update(
         self,
         db: AsyncSession,
         object: Union[UpdateSchemaType, dict[str, Any]],
         allow_multiple: bool = False,
         commit: bool = True,
+        timezone: bool = False,
         **kwargs: Any,
     ) -> None:
         """
         Updates an existing record or multiple records in the database based on specified filters. This method allows for precise targeting of records to update.
         It supports advanced filtering through comparison operators:
             '__gt' (greater than),
             '__lt' (less than),
@@ -1496,14 +1497,15 @@
             '__startswith' (start with)
 
         Args:
             db: The database session to use for the operation.
             object: A Pydantic schema or dictionary containing the update data.
             allow_multiple: If True, allows updating multiple records that match the filters. If False, raises an error if more than one record matches the filters.
             commit: If True, commits the transaction immediately. Default is True.
+            timezone: If True, add timezone in the update_at. Default is False.
             **kwargs: Filters to identify the record(s) to update, supporting advanced comparison operators for refined querying.
 
         Returns:
             None
 
         Raises:
             MultipleResultsFound: If `allow_multiple` is False and more than one record matches the filters.
@@ -1533,15 +1535,19 @@
         if isinstance(object, dict):
             update_data = object
         else:
             update_data = object.model_dump(exclude_unset=True)
 
         updated_at_col = getattr(self.model, self.updated_at_column, None)
         if updated_at_col:
-            update_data[self.updated_at_column] = datetime.now(timezone.utc)
+            if timezone:
+                update_data[self.updated_at_column] = datetime.now(UTC)
+            else:
+                update_data[self.updated_at_column] = datetime.now(UTC).replace(timezone=None)
+            
 
         update_data_keys = set(update_data.keys())
         model_columns = {column.name for column in inspect(self.model).c}
         extra_fields = update_data_keys - model_columns
         if extra_fields:
             raise ValueError(f"Extra fields provided: {extra_fields}")
```

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/crud/helper.py` & `crudfastapi-0.0.6/CRUDFastAPI/crud/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/endpoint/crud_router.py` & `crudfastapi-0.0.6/CRUDFastAPI/endpoint/crud_router.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/endpoint/endpoint_creator.py` & `crudfastapi-0.0.6/CRUDFastAPI/endpoint/endpoint_creator.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/endpoint/helper.py` & `crudfastapi-0.0.6/CRUDFastAPI/endpoint/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/exceptions/http_exceptions.py` & `crudfastapi-0.0.6/CRUDFastAPI/exceptions/http_exceptions.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/paginated/helper.py` & `crudfastapi-0.0.6/CRUDFastAPI/paginated/helper.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/CRUDFastAPI/paginated/response.py` & `crudfastapi-0.0.6/CRUDFastAPI/paginated/response.py`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/LICENSE` & `crudfastapi-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/pyproject.toml` & `crudfastapi-0.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "CRUDFastAPI"
-version = "0.0.5"
+version = "0.0.6"
 description = "CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities."
 authors = ["Mithun Thomas <mithunthomas003@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mithun2003/CRUDFastAPI"
 include = ["LICENSE"]
```

### Comparing `crudfastapi-0.0.5/README.md` & `crudfastapi-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `crudfastapi-0.0.5/PKG-INFO` & `crudfastapi-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CRUDFastAPI
-Version: 0.0.5
+Version: 0.0.6
 Summary: CRUDFastAPI is a Python package for FastAPI, offering robust async CRUD operations and flexible endpoint creation utilities.
 Home-page: https://github.com/mithun2003/CRUDFastAPI
 License: MIT
 Keywords: fastapi,crud,async,sqlalchemy,pydantic,fastcrud,crudfastapi
 Author: Mithun Thomas
 Author-email: mithunthomas003@gmail.com
 Requires-Python: >=3.9,<4.0
```

