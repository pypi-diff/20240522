# Comparing `tmp/Peliqan-1.6.2.tar.gz` & `tmp/Peliqan-1.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Peliqan-1.6.2.tar", last modified: Mon May 13 15:08:53 2024, max compression
+gzip compressed data, was "Peliqan-1.6.3.tar", last modified: Wed May 22 06:39:44 2024, max compression
```

## Comparing `Peliqan-1.6.2.tar` & `Peliqan-1.6.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.686333 Peliqan-1.6.2/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-13 15:08:53.686174 Peliqan-1.6.2/PKG-INFO
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.682064 Peliqan-1.6.2/Peliqan.egg-info/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/PKG-INFO
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/SOURCES.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/dependency_links.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/requires.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-13 15:08:53.000000 Peliqan-1.6.2/Peliqan.egg-info/top_level.txt
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.2/README.md
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.683782 Peliqan-1.6.2/peliqan/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-13 13:52:39.000000 Peliqan-1.6.2/peliqan/__init__.py
-drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-13 15:08:53.685734 Peliqan-1.6.2/peliqan/client/
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/__init__.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/backend_service.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     2747 2024-05-13 14:34:03.000000 Peliqan-1.6.2/peliqan/client/base.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10609 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/dbclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/sftpclient.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.6.2/peliqan/client/writeback.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    28778 2024-05-13 13:50:10.000000 Peliqan-1.6.2/peliqan/core.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.6.2/peliqan/exceptions.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.2/peliqan/local_test.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       40 2024-05-10 13:32:52.000000 Peliqan-1.6.2/peliqan/utils.py
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-13 15:08:53.686392 Peliqan-1.6.2/setup.cfg
--rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.6.2/setup.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.590258 Peliqan-1.6.3/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-22 06:39:44.590105 Peliqan-1.6.3/PKG-INFO
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.585207 Peliqan-1.6.3/Peliqan.egg-info/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      665 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/PKG-INFO
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      437 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/SOURCES.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        1 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/dependency_links.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       16 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/requires.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)        8 2024-05-22 06:39:44.000000 Peliqan-1.6.3/Peliqan.egg-info/top_level.txt
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1411 2023-08-02 11:35:09.000000 Peliqan-1.6.3/README.md
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.587417 Peliqan-1.6.3/peliqan/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      872 2024-05-22 06:37:04.000000 Peliqan-1.6.3/peliqan/__init__.py
+drwxr-xr-x   0 sudarshanv.s.   (501) staff       (20)        0 2024-05-22 06:39:44.589634 Peliqan-1.6.3/peliqan/client/
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      421 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/__init__.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    17466 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/client/backend_service.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1743 2024-05-20 14:08:33.000000 Peliqan-1.6.3/peliqan/client/base.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    10806 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/client/dbclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      928 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/sftpclient.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     4549 2024-05-13 13:01:35.000000 Peliqan-1.6.3/peliqan/client/writeback.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    29172 2024-05-22 06:06:57.000000 Peliqan-1.6.3/peliqan/core.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)      393 2024-05-10 06:48:15.000000 Peliqan-1.6.3/peliqan/exceptions.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)    20342 2024-03-21 07:17:47.000000 Peliqan-1.6.3/peliqan/local_test.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1118 2024-05-20 14:08:33.000000 Peliqan-1.6.3/peliqan/utils.py
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)       38 2024-05-22 06:39:44.590318 Peliqan-1.6.3/setup.cfg
+-rw-r--r--   0 sudarshanv.s.   (501) staff       (20)     1371 2024-05-10 06:48:22.000000 Peliqan-1.6.3/setup.py
```

### Comparing `Peliqan-1.6.2/PKG-INFO` & `Peliqan-1.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.2
+Version: 1.6.3
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.2/Peliqan.egg-info/PKG-INFO` & `Peliqan-1.6.3/Peliqan.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Peliqan
-Version: 1.6.2
+Version: 1.6.3
 Summary: This package is an sdk that allows any python client to connect with a Peliqan environment.
 Home-page: https://peliqan.io/
 Author: Peliqan.io
 Author-email: dev@peliqan.io
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `Peliqan-1.6.2/README.md` & `Peliqan-1.6.3/README.md`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.2/peliqan/__init__.py` & `Peliqan-1.6.3/peliqan/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "1.6.2"
+__version__ = "1.6.3"
 __author__ = 'Peliqan.io'
 __credits__ = 'Peliqan.io'
 
 __all__ = [
     "Peliqan",
     "BasePeliqanClient"
 ]
```

### Comparing `Peliqan-1.6.2/peliqan/client/backend_service.py` & `Peliqan-1.6.3/peliqan/client/backend_service.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.2/peliqan/client/base.py` & `Peliqan-1.6.3/peliqan/client/base.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,48 +1,11 @@
-from json import JSONEncoder
-
 import requests
 
-from peliqan.exceptions import PeliqanClientException, PeliqanJsonSerializerException
-
-
-def _serialize_data(obj):
-    if isinstance(obj, dict):
-        for k in obj:
-            obj[k] = _serialize_data(obj[k])
-
-        formatted_obj = obj
-    elif type(obj) in (list, tuple):
-        obj_len = len(obj)
-        for i in range(obj_len):
-            obj[i] = _serialize_data(obj[i])
-
-        formatted_obj = obj
-
-    elif isinstance(obj, (int, float, str)):
-        formatted_obj = obj
-        if isinstance(obj, float) and str(obj) == 'nan':
-            formatted_obj = None
-
-    elif isinstance(obj, type(None)):
-        formatted_obj = None
-
-    else:
-        try:
-            formatted_obj = JSONEncoder().encode(obj)
-        except Exception as e:
-            try:
-                formatted_obj = str(obj)
-            except Exception:
-                raise PeliqanJsonSerializerException(
-                    f"Could not serialize {obj.__class__.__name__} with value {obj}. "
-                    f"Original error is {e}"
-                )
-
-    return formatted_obj
+from peliqan.exceptions import PeliqanClientException
+from peliqan.utils import _serialize_data
 
 
 class BaseClient:
 
     def __init__(self, jwt, backend_url):
         self.JWT = jwt
         self.BACKEND_URL = backend_url
```

### Comparing `Peliqan-1.6.2/peliqan/client/dbclient.py` & `Peliqan-1.6.3/peliqan/client/dbclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import pandas
+
 from peliqan.exceptions import PeliqanClientException, OperationNotSupported
 from peliqan.client.base import BaseClient
 from peliqan.utils import Empty
 
 import pandas as pd
 import json
 
@@ -71,15 +73,15 @@
             column_type[0:6].lower() == "double" or
             column_type[0:5].lower() == "float" or
             column_type[0:7].lower() == "decimal" or
             column_type[0:7].lower() == "numeric"
         ):
             type_name = pd.Float64Dtype()
 
-        elif(
+        elif (
             column_type[0:3].lower() == "int" or
             column_type[0:6].lower() == "bigint" or
             column_type[0:3].lower() == "num"
         ):  # todo add more field types
             type_name = pd.Int64Dtype()
 
         elif column_type[0:4].lower() == "bool":
@@ -154,19 +156,25 @@
         kwargs = {'query': query}
         response = self.db_via_proxy(db_name, None, None, None, 'execute', **kwargs)
         return response
 
     def write(self, schema_name, table_name, records, object_schema=None, pk=None, db_name=None):
         if pk is None:
             pk = []
+
+        if isinstance(records, pandas.DataFrame):
+            records.replace({pandas.NaT: None, pandas.NA: None}, inplace=True)
+            records = records.to_dict('records')
+
         if not isinstance(records, list):
             if isinstance(records, dict):
                 records = [records]
             else:
                 raise PeliqanClientException("records has to be either a list or a dict")
+
         if not isinstance(pk, list):
             if isinstance(pk, str):
                 pk = [pk]
             else:
                 raise PeliqanClientException("pk has to be either a string or a list")
 
         _check_record_byte_size(records)
```

### Comparing `Peliqan-1.6.2/peliqan/client/sftpclient.py` & `Peliqan-1.6.3/peliqan/client/sftpclient.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.2/peliqan/client/writeback.py` & `Peliqan-1.6.3/peliqan/client/writeback.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.2/peliqan/core.py` & `Peliqan-1.6.3/peliqan/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,19 +183,41 @@
                     'detail': 'The sync task has completed.',
                     'syncing': False
                 }
 
             time.sleep(interval)
             count += 1
 
-    def run_pipeline(self, connection_name=None, connection_id=None, is_async=True):
-        return self.refresh_connection(connection_name, connection_id, is_async, only_pipelines=True)
+    def run_pipeline(self, connection_name=None, connection_id=None, tables=None, is_async=True):
+        return self.refresh_connection(
+            connection_name,
+            connection_id,
+            tables,
+            is_async,
+            only_pipelines=True
+        )
 
-    def refresh_connection(self, connection_name=None, connection_id=None, is_async=True, only_pipelines=False):
-        base_url = f"{self.BACKEND_URL}/api/servers/%s/syncdb/" + ("?pipeline=true" if only_pipelines else "")
+    def refresh_connection(
+        self,
+        connection_name=None,
+        connection_id=None,
+        tables=None,
+        is_async=True,
+        only_pipelines=False
+    ):
+        if not isinstance(tables, (list, tuple, type(None))):
+            tables = [tables]
+
+        tables = ','.join(table for table in tables) if tables else ""
+
+        pipeline = "true" if only_pipelines else "false"
+
+        base_url = (
+            f"{self.BACKEND_URL}/api/servers/%s/syncdb/?pipeline={pipeline}&tables={tables}"
+        )
         response = self.__service_client__.refresh_resource(resource_type='connection', refresh_baseurl=base_url,
                                                             resource_name=connection_name, resource_id=connection_id)
 
         if not is_async:
             response = self._retry_get_resource_status(
                 lambda: self.get_refresh_connection_status(connection_name=connection_name, connection_id=connection_id,
                                                            task_id=response.get('task_id'))
```

### Comparing `Peliqan-1.6.2/peliqan/local_test.py` & `Peliqan-1.6.3/peliqan/local_test.py`

 * *Files identical despite different names*

### Comparing `Peliqan-1.6.2/setup.py` & `Peliqan-1.6.3/setup.py`

 * *Files identical despite different names*

