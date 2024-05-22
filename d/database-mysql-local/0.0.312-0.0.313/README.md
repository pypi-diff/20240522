# Comparing `tmp/database_mysql_local-0.0.312.tar.gz` & `tmp/database_mysql_local-0.0.313.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.312.tar", last modified: Wed May 22 11:32:42 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.313.tar", last modified: Wed May 22 15:44:07 2024, max compression
```

## Comparing `database_mysql_local-0.0.312.tar` & `database_mysql_local-0.0.313.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:32:42.040281 database_mysql_local-0.0.312/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 11:32:42.040281 database_mysql_local-0.0.312/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:32:42.036281 database_mysql_local-0.0.312/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:32:42.040281 database_mysql_local-0.0.312/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    53626 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:32:42.040281 database_mysql_local-0.0.312/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 11:32:42.000000 database_mysql_local-0.0.312/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 11:32:42.000000 database_mysql_local-0.0.312/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:32:42.000000 database_mysql_local-0.0.312/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 11:32:42.000000 database_mysql_local-0.0.312/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 11:32:42.000000 database_mysql_local-0.0.312/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 11:31:35.000000 database_mysql_local-0.0.312/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 11:32:42.040281 database_mysql_local-0.0.312/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 11:32:05.000000 database_mysql_local-0.0.312/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.573252 database_mysql_local-0.0.313/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5234 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3182 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53626 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30389 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   630271 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4510 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 15:44:07.000000 database_mysql_local-0.0.313/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-22 15:43:08.000000 database_mysql_local-0.0.313/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 15:44:07.577252 database_mysql_local-0.0.313/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-22 15:43:35.000000 database_mysql_local-0.0.313/setup.py
```

### Comparing `database_mysql_local-0.0.312/PKG-INFO` & `database_mysql_local-0.0.313/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.312
+Version: 0.0.313
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.312/README.md` & `database_mysql_local-0.0.313/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.313/database_mysql_local/src/connector.py`

 * *Files 13% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.connection: mysql.connector = None
         self._cursor: Optional[Cursor] = None
         self._connect_to_db()
         connections_pool[schema_name] = self
 
     def reconnect(self) -> None:
         self.connection.reconnect()
-        self._cursor = self.cursor()
+        self._cursor = self.cursor(close_previous=True)
         self.set_schema(self.schema)
 
     def _connect_to_db(self):
         self.connection = mysql.connector.connect(
             host=self.host,
             user=self.user,
             password=self.password,
@@ -79,32 +79,38 @@
     def database_info(self):
         return f"host={self.host}, user={self.user}, schema={self.schema}"
 
     def close(self) -> None:
         try:
             if self._cursor:
                 self._cursor.close()
-                logger.info("Cursor closed successfully.")
+                logger.info(f"Cursor closed successfully for schema: {self.schema}")
         except Exception as exception:
             logger.error(f"connection.py close() {self.database_info()}", object={"exception": exception})
 
         if self.connection and self.connection.is_connected():
             self.connection.close()
             connections_pool.pop(self.schema, None)
             logger.info("Connection closed successfully.")
 
-    def cursor(self, *, dictionary: bool = None, buffered: bool = None, raw: bool = None,
+    def cursor(self, *, close_previous: bool = True, cache_previous: bool = False, dictionary: bool = None, buffered: bool = None, raw: bool = None,
                prepared: bool = None, named_tuple: bool = None, cursor_class=None) -> Cursor:
+        if cache_previous and self._cursor:
+            cursor_instance = self._cursor
+            return cursor_instance
+
         cursor_instance = Cursor(self.connection.cursor(
             dictionary=dictionary, buffered=buffered, raw=raw, prepared=prepared,
             named_tuple=named_tuple, cursor_class=cursor_class))
+        if close_previous and self._cursor:
+            self._cursor.close()
+        self._cursor = cursor_instance
         return cursor_instance
 
     def commit(self) -> None:
-
         self.connection.commit()
 
     def set_schema(self, new_schema: Optional[str]) -> None:
         if not new_schema:
             return
         if self.schema == new_schema:
             return
@@ -117,13 +123,11 @@
             self.schema = new_schema
             logger.info(f"Switched to schema: {new_schema}")
         else:
             raise Exception(
                 "Connection is not established. The database will be used on the next connect.")
 
     def rollback(self):
-
         self.connection.rollback()
 
     def start_transaction(self):
-
         self.connection.start_transaction()
```

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.313/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/cursor.py` & `database_mysql_local-0.0.313/database_mysql_local/src/cursor.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.313/database_mysql_local/src/generic_crud.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.313/database_mysql_local/src/generic_crud_ml.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.313/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/point.py` & `database_mysql_local-0.0.313/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.313/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.313/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.313/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.313/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.313/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.313/database_mysql_local.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.312
+Version: 0.0.313
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.312/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.313/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/pyproject.toml` & `database_mysql_local-0.0.313/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.312/setup.py` & `database_mysql_local-0.0.313/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.312',
+    version='0.0.313',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

