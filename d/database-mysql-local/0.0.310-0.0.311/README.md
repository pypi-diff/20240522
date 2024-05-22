# Comparing `tmp/database_mysql_local-0.0.310.tar.gz` & `tmp/database_mysql_local-0.0.311.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "database_mysql_local-0.0.310.tar", last modified: Mon May 20 22:40:44 2024, max compression
+gzip compressed data, was "database_mysql_local-0.0.311.tar", last modified: Tue May 21 14:15:07 2024, max compression
```

## Comparing `database_mysql_local-0.0.310.tar` & `database_mysql_local-0.0.311.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.875030 database_mysql_local-0.0.310/database_mysql_local/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/database_mysql_local/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/connector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3337 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/cursor.py
--rw-r--r--   0 runner    (1001) docker     (127)    51577 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_crud.py
--rw-r--r--   0 runner    (1001) docker     (127)    31830 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_crud_ml.py
--rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/generic_mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/point.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/polygon.py
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/sync_conflict_resolution.py
--rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/database_mysql_local/src/table_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/to_sql_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/database_mysql_local/src/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/database_mysql_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-20 22:40:44.000000 database_mysql_local-0.0.310/database_mysql_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-20 22:39:49.000000 database_mysql_local-0.0.310/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 22:40:44.879030 database_mysql_local-0.0.310/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-20 22:40:14.000000 database_mysql_local-0.0.310/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:15:07.655236 database_mysql_local-0.0.311/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 14:15:07.655236 database_mysql_local-0.0.311/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3519 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:15:07.647236 database_mysql_local-0.0.311/database_mysql_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:15:07.655236 database_mysql_local-0.0.311/database_mysql_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4894 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/database_mysql_local/src/connector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4223 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/database_mysql_local/src/cursor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53030 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/database_mysql_local/src/generic_crud.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31551 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/database_mysql_local/src/generic_crud_ml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6907 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/generic_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/point.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/polygon.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/sync_conflict_resolution.py
+-rw-r--r--   0 runner    (1001) docker     (127)   595483 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/database_mysql_local/src/table_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/to_sql_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4378 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/database_mysql_local/src/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 14:15:07.655236 database_mysql_local-0.0.311/database_mysql_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-05-21 14:15:07.000000 database_mysql_local-0.0.311/database_mysql_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-21 14:15:07.000000 database_mysql_local-0.0.311/database_mysql_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 14:15:07.000000 database_mysql_local-0.0.311/database_mysql_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-21 14:15:07.000000 database_mysql_local-0.0.311/database_mysql_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-21 14:15:07.000000 database_mysql_local-0.0.311/database_mysql_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-21 14:14:09.000000 database_mysql_local-0.0.311/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 14:15:07.655236 database_mysql_local-0.0.311/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-21 14:14:35.000000 database_mysql_local-0.0.311/setup.py
```

### Comparing `database_mysql_local-0.0.310/PKG-INFO` & `database_mysql_local-0.0.311/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.310
+Version: 0.0.311
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.310/README.md` & `database_mysql_local-0.0.311/README.md`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/connector.py` & `database_mysql_local-0.0.311/database_mysql_local/src/connector.py`

 * *Files 6% similar despite different names*

```diff
@@ -76,32 +76,31 @@
         self._cursor = self.cursor()
         self.set_schema(self.schema)
 
     def database_info(self):
         return f"host={self.host}, user={self.user}, schema={self.schema}"
 
     def close(self) -> None:
-
         try:
             if self._cursor:
                 self._cursor.close()
                 logger.info("Cursor closed successfully.")
         except Exception as exception:
             logger.error(f"connection.py close() {self.database_info()}", object={"exception": exception})
 
         if self.connection and self.connection.is_connected():
             self.connection.close()
             connections_pool.pop(self.schema, None)
             logger.info("Connection closed successfully.")
 
-    def cursor(self, dictionary=False, buffered=False) -> Cursor:
-
+    def cursor(self, *, dictionary: bool = None, buffered: bool = None, raw: bool = None,
+               prepared: bool = None, named_tuple: bool = None, cursor_class=None) -> Cursor:
         cursor_instance = Cursor(self.connection.cursor(
-            dictionary=dictionary, buffered=buffered))
-
+            dictionary=dictionary, buffered=buffered, raw=raw, prepared=prepared,
+            named_tuple=named_tuple, cursor_class=cursor_class))
         return cursor_instance
 
     def commit(self) -> None:
 
         self.connection.commit()
 
     def set_schema(self, new_schema: Optional[str]) -> None:
```

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/constants.py` & `database_mysql_local-0.0.311/database_mysql_local/src/constants.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/generic_crud.py` & `database_mysql_local-0.0.311/database_mysql_local/src/generic_crud.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import mysql.connector
 from database_infrastructure_local.number_generator import NumberGenerator
 from logger_local.MetaLogger import MetaLogger
 from user_context_remote.user_context import UserContext
 
 from .connector import Connector
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_CODE_OBJECT
+from .cursor import Cursor
 from .table_definition import table_definition
 from .utils import (process_insert_data_dict, process_update_data_dict, get_where_params, where_skip_null_values,
                     validate_none_select_table_name, validate_single_clause_value,
                     validate_select_table_name, detect_if_is_test_data, generate_table_name,
                     generate_view_name, generate_column_name, get_entity_type_by_table_name)
 
 
@@ -87,20 +88,20 @@
             data_dict=data_dict, add_created_user_id=True, schema_name=schema_name, table_name=table_name)
 
         columns, values, data_dict = process_insert_data_dict(data_dict=data_dict)
         # We removed the IGNORE from the SQL Statement as we want to return the id of the existing row
         insert_query = "INSERT " + \
                        f"INTO `{schema_name}`.`{table_name}` ({columns}) " \
                        f"VALUES ({values});"
-
         try:
-            self.cursor.execute(insert_query, tuple(data_dict.values()))
+            cursor = self.get_cursor()
+            cursor.execute(insert_query, tuple(data_dict.values()))
             if commit_changes:
                 self.connection.commit()
-            inserted_id = self.cursor.lastrowid()
+            inserted_id = cursor.lastrowid()
         except mysql.connector.errors.IntegrityError as exception:
             if ignore_duplicate:
                 self.logger.warning("GenericCRUD.insert: existing record found, selecting it's id."
                                     f"(table_name={table_name}, data_dict={data_dict})")
                 inserted_id = self._get_existing_duplicate_id(schema_name, table_name, exception)
             else:
                 raise exception
@@ -147,16 +148,16 @@
         columns = ", ".join(f"`{key}`" for key in data_dict)
         values = ", ".join(["%s"] * len(data_dict))
         sql_statement = f"""
         INSERT INTO `{schema_name}`.`{table_name}` ({columns})
         VALUES ({values});
         """
         sql_parameters = list(zip(*data_dict.values()))
-
-        self.cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
+        cursor = self.get_cursor()
+        cursor.executemany(sql_statement=sql_statement, sql_parameters=sql_parameters)
         if commit_changes:
             self.connection.commit()
 
     def upsert(self, *, schema_name: str = None, table_name: str = None, view_table_name: str = None,
                data_dict: dict = None, data_json: dict = None,
                data_dict_compare: dict = None, data_json_compare: dict = None,
                order_by: str = None, compare_with_or: bool = False) -> Optional[int]:
@@ -187,19 +188,16 @@
             else:
                 where_clauses.append(f"{key}=%s")
                 params.append(value)
 
         where_clause = " OR " if compare_with_or else " AND "
         where_clause = where_clause.join(where_clauses)
 
-        old_cursor = self.cursor
-        cursor = None
         try:
-            cursor = self.connection.cursor()
-            self.cursor = cursor
+            cursor = self.get_cursor()
             table_id = self.select_one_value_by_where(
                 schema_name=schema_name, view_table_name=view_table_name, select_clause_value=column_name,
                 where=where_clause, params=tuple(params), order_by=order_by)
             if table_id:
                 self.update_by_column_and_value(
                     schema_name=schema_name, table_name=table_name, column_name=column_name, column_value=table_id,
                     data_dict=data_dict, commit_changes=False)
@@ -207,18 +205,15 @@
                 table_id = self.insert(schema_name=schema_name, table_name=table_name, data_dict=data_dict,
                                        commit_changes=False, ignore_duplicate=True)
             self.connection.commit()
         except Exception as exception:
             self.connection.rollback()
             raise exception
         finally:
-            self.cursor = old_cursor
             self.default_schema_name = old_schema_name
-            if cursor:
-                cursor.close()
             self.logger.debug(object=locals())
         return table_id
 
     def _get_existing_duplicate_id(self, schema_name: str, table_name: str, error: Exception) -> int or None:
         """Error examples:
         - Duplicate entry 'test@gmail.com' for key 'email_address_table.email_address.unique'
         - Duplicate entry '1' for key 'test_mysql_table.PRIMARY'
@@ -230,64 +225,63 @@
         duplicate_value = match.group(1)
         duplicate_column_name = match.group(2).split('.')[1]
         if duplicate_column_name == "PRIMARY":
             return int(duplicate_value)
         if duplicate_column_name.endswith("_UNIQUE"):
             duplicate_column_name = duplicate_column_name.split('_')[0]
 
-        query = """
-        SELECT COLUMN_NAME
-        FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
-        WHERE TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY";
-        """
-        self.cursor.execute(query, (table_name,))
-        column_name = (self.cursor.fetchone() or [None])[0]
+        column_name = self.get_primary_key(schema_name=schema_name, table_name=table_name)
         if not column_name:
             raise error  # Column name for constraint not found
         select_query = f"SELECT {column_name} FROM `{schema_name}`.`{table_name}` WHERE {duplicate_column_name} = %s LIMIT 1;"
-        self.cursor.execute(select_query, (duplicate_value,))
-        existing_duplicate_id = (self.cursor.fetchone() or [None])[0]
+        cursor = self.get_cursor()
+        self.connection.commit()
+        cursor.execute(select_query, (duplicate_value,))
+        existing_duplicate_id = (cursor.fetchone() or [None])[0]
+
         self.logger.debug(object=locals())
         return existing_duplicate_id
 
     def update_by_id(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.update_by_id is deprecated, use update_by_column_and_value instead.")
         return self.update_by_column_and_value(schema_name=schema_name, table_name=table_name,
                                                column_name=column_name, column_value=column_value,
                                                id_column_name=id_column_name, id_column_value=id_column_value,
                                                data_dict=data_dict, data_json=data_json,
                                                limit=limit, order_by=order_by, commit_changes=commit_changes)
 
     def update_by_column_and_value(
             self, *, schema_name: str = None, table_name: str = None, column_name: str = None, column_value: Any = None,
             id_column_name: str = None, id_column_value: Any = None, data_dict: dict = None, data_json: dict = None,
-            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> None:
+            limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None, commit_changes: bool = True) -> int or None:
         """Updates data in the table by ID."""
         column_name = self._deprecated_id_column(id_column_name, column_name)
         column_value = column_value or id_column_value
         data_dict = data_json or self._data_json_to_dict(data_dict)
         table_name = table_name or self.default_table_name
         column_name = column_name or self.default_column_name
 
         if column_name:
             where, params = get_where_params(column_name, column_value)
-            self.update_by_where(schema_name=schema_name, table_name=table_name, where=where,
-                                 data_dict=data_dict, params=params,
-                                 limit=limit, order_by=order_by, commit_changes=commit_changes)
+            last_row_id = self.update_by_where(
+                schema_name=schema_name, table_name=table_name, where=where, data_dict=data_dict,
+                params=params, limit=limit, order_by=order_by, commit_changes=commit_changes)
+            return last_row_id
+
         else:
             raise Exception("Update by id requires an column_name")
 
     def update_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
                         params: tuple = None, data_dict: dict = None, data_json: dict = None,
                         limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None,
-                        commit_changes: bool = True) -> None:
+                        commit_changes: bool = True) -> int or None:
         """Updates data in the table by WHERE.
         Example:
         "UPDATE table_name SET A=A_val, B=B_val WHERE C=C_val AND D=D_val"
         translates into:
         update_by_where(table_name="table_name",
                         data_dict={"A": A_val, "B": B_val},
                         where="C=%s AND D=%s",
@@ -306,55 +300,64 @@
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET {set_values} updated_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where} " + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
         params = params or tuple()
-        self.cursor.execute(update_query, tuple(data_dict.values()) + params)
+        cursor = self.get_cursor()
+        cursor.execute(update_query, tuple(data_dict.values()) + params)
         if commit_changes:
             self.connection.commit()
+        last_row_id = cursor.lastrowid()
+        return last_row_id
 
     def delete_by_id(self, *, schema_name: str = None, table_name: str = None,
                      column_name: str = None, column_value: Any = None,
-                     id_column_name: str = None, id_column_value: Any = None) -> None:
+                     id_column_name: str = None, id_column_value: Any = None) -> int:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning("GenericCRUD.delete_by_id is deprecated, use delete_by_column_and_value instead.")
-        return self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
-                                               column_name=column_name, column_value=column_value,
-                                               id_column_name=id_column_name, id_column_value=id_column_value)
+        affected_rows = self.delete_by_column_and_value(schema_name=schema_name, table_name=table_name,
+                                                        column_name=column_name, column_value=column_value,
+                                                        id_column_name=id_column_name, id_column_value=id_column_value)
+        return affected_rows
 
     def delete_by_column_and_value(self, *, schema_name: str = None, table_name: str = None,
                                    column_name: str = None, column_value: Any = None,
-                                   id_column_name: str = None, id_column_value: Any = None) -> None:
+                                   id_column_name: str = None, id_column_value: Any = None) -> int:
         """Deletes data from the table by id"""
         # checks are done inside delete_by_where
         column_name = self._deprecated_id_column(id_column_name, column_name) or self.default_column_name
         column_value = column_value or id_column_value
         if column_name:  # column_value can be empty
             where, params = get_where_params(column_name, column_value)
-            self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where, params=params)
+            affected_rows = self.delete_by_where(schema_name=schema_name, table_name=table_name, where=where,
+                                                 params=params)
+            return affected_rows
         else:
             raise Exception("Delete by id requires an column_name and column_value.")
 
     def delete_by_where(self, *, schema_name: str = None, table_name: str = None, where: str = None,
-                        params: tuple = None) -> None:
+                        params: tuple = None) -> int:
         """Deletes data from the table by WHERE."""
 
         table_name = table_name or self.default_table_name
         schema_name = schema_name or self.default_schema_name
         self._validate_args(args=locals())
         if not where:
             raise Exception("delete_by_where requires a 'where'")
 
         update_query = f"UPDATE `{schema_name}`.`{table_name}` " \
                        f"SET end_timestamp=CURRENT_TIMESTAMP() " \
                        f"WHERE {where};"
-        self.cursor.execute(update_query, params)
+        cursor = self.get_cursor()
+        cursor.execute(update_query, params)
         self.connection.commit()
+        affected_rows = cursor.get_row_count()
+        return affected_rows
 
     # Main select function
     def select_multi_tuple_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, limit: int = DEFAULT_SQL_SELECT_LIMIT,
             order_by: str = "") -> list:
         """Selects multiple rows from the table based on a WHERE clause and returns them as a list of tuples."""
@@ -370,21 +373,26 @@
         # select_clause_value = ",".join([f"`{x.strip()}`" for x in select_clause_value.split(",") if x != "*"])
         # TODO: If is_test_data exists in the table and is_test_data=False, add `AND is_test_data=0` to avoid users getting test data
         #   (but the tests should be allowed to access real data)
         if (self.is_test_data and (view_table_name or "").replace("_view", "") ==
                 (self.default_table_name or "").replace("_table", "")):
             # test data does not appear in the view, but we still wants to access it in tests (partial solution).
             view_table_name = self.default_table_name
+            if where:
+                where += " AND end_timestamp IS NULL "  # not deleted
         select_query = f"SELECT {'DISTINCT' if distinct else ''} {select_clause_value} " \
                        f"FROM `{schema_name}`.`{view_table_name}` " + \
                        (f"WHERE {where} " if where else "") + \
                        (f"ORDER BY {order_by} " if order_by else "") + \
                        f"LIMIT {limit};"
-        self.cursor.execute(select_query, params)
-        result = self.cursor.fetchall()
+        cursor = self.get_cursor()
+        self.connection.commit()  # https://bugs.mysql.com/bug.php?id=102053
+        cursor.execute(select_query, params)
+        result = cursor.fetchall()
+
         self.logger.debug(object=locals())
         return result
 
     def select_multi_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False,
             limit: int = DEFAULT_SQL_SELECT_LIMIT, order_by: str = None) -> list:
@@ -441,15 +449,15 @@
             distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table by ID and returns it as a dictionary (column_name: value)"""
         column_name = column_name or id_column_name
         column_value = column_value or id_column_value
         result = self.select_one_tuple_by_column_and_value(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             column_name=column_name, column_value=column_value, distinct=distinct, order_by=order_by)
-        return self.convert_to_dict(result, select_clause_value)
+        return self.convert_to_dict(row=result, select_clause_value=select_clause_value)
 
     def select_one_value_by_id(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             column_name: str = None, column_value: Any = None, id_column_name: str = None, id_column_value: Any = None,
             distinct: bool = False, order_by: str = "", skip_null_values: bool = True) -> Any:
         if datetime.now() > datetime(2024, 5, 25):
             self.logger.warning(
@@ -492,15 +500,15 @@
     def select_one_dict_by_where(
             self, *, schema_name: str = None, view_table_name: str = None, select_clause_value: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "") -> dict:
         """Selects one row from the table based on a WHERE clause and returns it as a dictionary."""
         result = self.select_one_tuple_by_where(
             schema_name=schema_name, view_table_name=view_table_name, select_clause_value=select_clause_value,
             where=where, params=params, distinct=distinct, order_by=order_by)
-        return self.convert_to_dict(result, select_clause_value)
+        return self.convert_to_dict(row=result, select_clause_value=select_clause_value)
 
     def select_one_value_by_where(
             self, *, select_clause_value: str, schema_name: str = None, view_table_name: str = None,
             where: str = None, params: tuple = None, distinct: bool = False, order_by: str = "",
             skip_null_values: bool = True) -> Any:
         """Selects one value from the table based on a WHERE clause and returns it."""
         select_clause_value = select_clause_value or self.default_select_clause_value
@@ -618,52 +626,72 @@
         return self.convert_multi_to_dict(result, select_clause_value)
 
     def is_column_in_table(self, column_name: str, schema_name: str = None, table_name: str = None) -> bool:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         if not column_name:
             raise Exception("is_column_in_table requires a column_name")
-        columns = self.get_columns_dict(schema_name=schema_name, table_name=table_name)
-        is_column_in_table_result = (column_name in columns)
+        table_columns = self.get_table_columns(schema_name=schema_name, table_name=table_name)
+        is_column_in_table_result = (column_name in table_columns)
         self.logger.debug(object=locals())
         return is_column_in_table_result
 
     # TODO: use table_definition_table to improve performance
     # TODO: replace with redis in the future with table_definition_table
     @lru_cache
-    def get_columns_dict(self, schema_name: str = None, table_name: str = None) -> dict:
+    def get_table_columns(self, schema_name: str = None, table_name: str = None) -> tuple:
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         select_query = "SELECT column_name " \
                        "FROM information_schema.columns " \
                        "WHERE TABLE_SCHEMA = %s " \
                        "AND TABLE_NAME = %s;"
         params = (schema_name, table_name)
-        self.cursor.execute(select_query, params)
-        result = self.cursor.fetchall()
-        columns_dict = {row[0]: None for row in result}
+        cursor = self.get_cursor()
+        self.connection.commit()
+        cursor.execute(select_query, params)
+        result = cursor.fetchall()
+
+        columns_tuple = tuple(x[0] for x in result)
         self.logger.debug(object=locals())
-        return columns_dict
+        return columns_tuple
+
+
+    @lru_cache
+    def get_primary_key(self, schema_name: str = None, table_name: str = None) -> str or None:
+        schema_name = schema_name or self.default_schema_name
+        table_name = table_name or self.default_table_name
+        query = """
+        SELECT COLUMN_NAME
+        FROM INFORMATION_SCHEMA.KEY_COLUMN_USAGE
+        WHERE TABLE_SCHEMA = %s AND TABLE_NAME = %s AND CONSTRAINT_NAME = "PRIMARY"
+        LIMIT 1;
+        """
+        cursor = self.get_cursor()
+        self.connection.commit()
+        cursor.execute(query, (schema_name, table_name))
+        column_name = (cursor.fetchone() or [None])[0]
+        return column_name
 
     # helper functions:
     def convert_to_dict(self, row: tuple, select_clause_value: str = None) -> dict:
         """Returns a dictionary of the column names and their values."""
         select_clause_value = select_clause_value or self.default_select_clause_value
         if select_clause_value == "*":
-            column_names = [col[0] for col in self.cursor.description()]
+            column_names = self.cursor.column_names()
         else:
             column_names = [x.strip() for x in select_clause_value.split(",")]
         dict_result = dict(zip(column_names, row or tuple()))
         self.logger.debug(object=locals())
         return dict_result
 
     def convert_multi_to_dict(self, rows: list[tuple], select_clause_value: str = None) -> list[dict]:
         """Converts multiple rows to dictionaries."""
-        multiple_dict_result = [self.convert_to_dict(row, select_clause_value) for row in rows]
-        self.logger.debug(object=locals())
+        multiple_dict_result = [self.convert_to_dict(row=row, select_clause_value=select_clause_value)
+                                for row in rows]
         return multiple_dict_result
 
     def _validate_args(self, args: dict) -> None:
         # args = locals() of the calling function
         required_args = ("table_name", "view_table_name", "schema_name", "select_clause_value")  # TODO: , "data_dict")
         for arg_name, arg_value in args.items():
             message = ""
@@ -697,74 +725,75 @@
         identifier = NumberGenerator.get_random_identifier(
             schema_name="identifier", view_name="identifier_view", identifier_column_name="identifier")
         data_dict["identifier"] = identifier
         # We can't use self.insert, as it would cause an infinite loop
         insert_query = "INSERT " + \
                        "INTO `identifier`.`identifier_table` (identifier, entity_type_id) " \
                        "VALUES (%s, %s);"
-        self.cursor.execute(insert_query, (identifier, identifier_entity_type_id))
+        cursor = self.get_cursor()
+        cursor.execute(insert_query, (identifier, identifier_entity_type_id))
         self.connection.commit()
 
     # TODO: add warning logs
     def __add_create_updated_user_profile_ids(self, data_dict: dict, add_created_user_id: bool = False,
                                               schema_name: str = None, table_name: str = None) -> dict:
         """Adds created_user_id and updated_user_id to data_dict."""
         # if get_environment_name() not in (EnvironmentName.DVLP1.value, EnvironmentName.PROD1.value):
         # TODO data_dict = data_dict.copy() ?
         schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
-        columns_dict = self.get_columns_dict(schema_name=schema_name, table_name=table_name)
+        table_columns = self.get_table_columns(schema_name=schema_name, table_name=table_name)
         if add_created_user_id:
-            if "created_user_id" in columns_dict:
+            if "created_user_id" in table_columns:
                 data_dict["created_user_id"] = self.user_context.get_effective_user_id()
             else:
                 self.__log_warning("created_user_id", schema_name, table_name)
-            if "created_real_user_id" in columns_dict:
+            if "created_real_user_id" in table_columns:
                 data_dict["created_real_user_id"] = self.user_context.get_real_user_id()
             else:
                 self.__log_warning("created_real_user_id", schema_name, table_name)
-            if "created_effective_user_id" in columns_dict:
+            if "created_effective_user_id" in table_columns:
                 data_dict["created_effective_user_id"] = self.user_context.get_effective_user_id()
             else:
                 self.__log_warning("created_effective_user_id", schema_name, table_name)
-            if "created_effective_profile_id" in columns_dict:
+            if "created_effective_profile_id" in table_columns:
                 data_dict["created_effective_profile_id"] = self.user_context.get_effective_profile_id()
             else:
                 self.__log_warning("created_effective_profile_id", schema_name, table_name)
-            if "number" in columns_dict:
+            if "number" in table_columns:
                 # TODO: the commented line caused errors, we need to check it
                 # view_name = self.default_view_table_name or self._get_view_name(table_name)
                 view_name = table_name
                 number = NumberGenerator.get_random_number(schema_name=schema_name, view_name=view_name)
                 data_dict["number"] = number
             else:
                 self.__log_warning("number", schema_name, table_name)
 
-            if "identifier" in columns_dict:
+            if "identifier" in table_columns:
                 self.__add_identifier(data_dict=data_dict, table_name=table_name)
             else:
                 self.__log_warning("identifier", schema_name, table_name)
-        if "updated_user_id" in columns_dict:
+        if "updated_user_id" in table_columns:
             data_dict["updated_user_id"] = self.user_context.get_effective_user_id()
         else:
             self.__log_warning("updated_user_id", schema_name, table_name)
-        if "updated_real_user_id" in columns_dict:
+        if "updated_real_user_id" in table_columns:
             data_dict["updated_real_user_id"] = self.user_context.get_real_user_id()
         else:
             self.__log_warning("updated_real_user_id", schema_name, table_name)
-        if "updated_effective_user_id" in columns_dict:
+        if "updated_effective_user_id" in table_columns:
             data_dict["updated_effective_user_id"] = self.user_context.get_effective_user_id()
         else:
             self.__log_warning("updated_effective_user_id", schema_name, table_name)
-        if "updated_effective_profile_id" in columns_dict:
+        if "updated_effective_profile_id" in table_columns:
             data_dict["updated_effective_profile_id"] = self.user_context.get_effective_profile_id()
         else:
             self.__log_warning("updated_effective_profile_id", schema_name, table_name)
         # TODO: later we may want to add a check for the table_definition to see if there is a column for is_test_data
-        if "is_test_data" in columns_dict:
+        if "is_test_data" in table_columns:
             data_dict["is_test_data"] = self.is_test_data
         else:
             self.__log_warning("is_test_data", schema_name, table_name)
         # else:
         #     schema_name = schema_name or self.schema_name
         #     table_name = table_name or self.default_table_name
         #     if add_created_user_id:
@@ -817,14 +846,22 @@
             self.connection.set_schema(schema_name)
             self.default_schema_name = schema_name
 
     def close(self) -> None:
         """Closes the connection to the database (we usually do not have to call this)"""
         self.connection.close()
 
+    def get_cursor(self, close_first: bool = False) -> Cursor:
+        """Get a new cursor"""
+        if close_first and not self.cursor.is_closed():
+            self.cursor.close()
+        if self.cursor.is_closed():
+            self.cursor = self.connection.cursor()
+        return self.cursor
+
     # TODO: test this method
     def get_test_entity_id(self, *, entity_name: str, insert_function: callable, insert_kwargs: dict = None,
                            entity_creator: callable = None, create_kwargs: dict = None,
                            schema_name: str = None, view_name: str = None) -> int:
         """
         1. Check if there's an entity with is `is_test_data=True`.
         2. If there is, return its id.
```

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/generic_crud_ml.py` & `database_mysql_local-0.0.311/database_mysql_local/src/generic_crud_ml.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,19 +8,24 @@
 from .constants import DEFAULT_SQL_SELECT_LIMIT, LOGGER_CRUD_ML_CODE_OBJECT
 from .generic_crud import GenericCRUD
 from .utils import generate_column_name, generate_view_name
 
 IS_MAIN_COLUMN_NAME = "is_main"
 
 
+# TODO If I understand, there are two things:
+# is_main in data_ml_dict
+# table_definition_table.is_main_column
+# I'm not sure we need additional parameter.
 class GenericCRUDML(GenericCRUD, metaclass=MetaLogger, object=LOGGER_CRUD_ML_CODE_OBJECT):
     """A class that provides generic CRUD functionality for tables with multi-language support."""
 
     def __init__(self, default_schema_name: str, default_table_name: str = None, default_view_table_name: str = None,
-                 default_ml_view_table_name: str = None, default_column_name: str = None, default_id_column_name: str = None,
+                 default_ml_view_table_name: str = None, default_column_name: str = None,
+                 default_id_column_name: str = None,
                  is_main_column_name: str = IS_MAIN_COLUMN_NAME,
                  is_test_data: bool = False) -> None:
         """Initializes the GenericCRUDML class. If connection is not provided,
         a new connection will be created."""
         if default_table_name is not None:
             self.default_ml_table_name = self._create_ml_table_name(default_table_name)
             default_view_table_name = default_view_table_name
@@ -65,20 +70,15 @@
         data_ml_dict = data_ml_json or self._data_json_to_dict(data_ml_dict)
         lang_code_str = self._get_lang_code_str(lang_code=lang_code, data_ml_dict=data_ml_dict)
         old_schema_name = self.default_schema_name
         self.default_schema_name = schema_name or self.default_schema_name
         table_name = table_name or self.default_table_name
         ml_table_name = ml_table_name or self.default_ml_table_name
 
-        old_cursor = self.cursor
-        cursor = None
         try:
-            cursor = self.connection.cursor()
-            self.cursor = cursor
-
             # if this is the first insert of this data, is_main should be 1
             if is_main is not None:
                 if table_id is None:
                     is_main = 1
                 elif is_main == 1:
                     self._update_old_main_value_to_zero(table_id, table_name)
                 data_ml_dict[self.is_main_column_name] = is_main
@@ -104,18 +104,15 @@
                                       commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
         finally:
-            self.cursor = old_cursor
             self.default_schema_name = old_schema_name
-            if cursor:
-                cursor.close()
         return table_id, ml_table_id
 
     def add_value_if_not_exist(self, *, data_dict: dict = None, data_ml_dict: dict = None,
                                data_json: dict = None, data_ml_json: dict = None,
                                table_id: int = None, lang_code: LangCode = None,
                                is_main: int = 0, table_name: str = None,
                                ml_table_name: str = None, schema_name: str = None,
@@ -164,21 +161,15 @@
         ml_table_name = ml_table_name or self.default_ml_table_name
         column_name = generate_column_name(table_name)
 
         if table_id is None:
             raise ValueError("table_id is required for update_value")
         if ml_table_id is None:
             raise ValueError("ml_table_id is required for update_value")
-
-        old_cursor = self.cursor
-        cursor = None
         try:
-            cursor = self.connection.cursor()
-            self.cursor = cursor
-
             if is_main is not None:
                 if is_main == 1:
                     self._update_old_main_value_to_zero(table_id, table_name)
                 if data_dict:
                     self.update_by_id(data_dict=data_dict, table_name=table_name, column_name=column_name,
                                       id_column_value=table_id, limit=limit, order_by=order_by, commit_changes=False)
                 data_ml_dict[self.is_main_column_name] = is_main
@@ -191,18 +182,15 @@
                               id_column_value=ml_table_id, limit=limit, order_by=order_by, commit_changes=False)
 
             self.connection.commit()
         except Exception as e:
             self.connection.rollback()
             raise e
         finally:
-            self.cursor = old_cursor
             self.default_schema_name = old_schema_name
-            if cursor:
-                cursor.close()
         return table_id, ml_table_id
 
     def upsert_value(self, *, data_dict: dict = None, data_ml_dict: dict = None,
                      data_json: dict = None, data_ml_json: dict = None,
                      table_id: int = None, data_dict_compare: dict = None, lang_code: LangCode = None,
                      is_main: int = 0, table_name: str = None,
                      ml_table_name: str = None, schema_name: str = None,
```

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/generic_mapping.py` & `database_mysql_local-0.0.311/database_mysql_local/src/generic_mapping.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/point.py` & `database_mysql_local-0.0.311/database_mysql_local/src/point.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/polygon.py` & `database_mysql_local-0.0.311/database_mysql_local/src/polygon.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/sync_conflict_resolution.py` & `database_mysql_local-0.0.311/database_mysql_local/src/sync_conflict_resolution.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/table_definition.py` & `database_mysql_local-0.0.311/database_mysql_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/to_sql_interface.py` & `database_mysql_local-0.0.311/database_mysql_local/src/to_sql_interface.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local/src/utils.py` & `database_mysql_local-0.0.311/database_mysql_local/src/utils.py`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/database_mysql_local.egg-info/PKG-INFO` & `database_mysql_local-0.0.311/database_mysql_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: database-mysql-local
-Version: 0.0.310
+Version: 0.0.311
 Home-page: https://github.com/circles-zone/database-mysql-local-python-package
 Author: Circles
 Author-email: info@circles.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
```

### Comparing `database_mysql_local-0.0.310/database_mysql_local.egg-info/SOURCES.txt` & `database_mysql_local-0.0.311/database_mysql_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/pyproject.toml` & `database_mysql_local-0.0.311/pyproject.toml`

 * *Files identical despite different names*

### Comparing `database_mysql_local-0.0.310/setup.py` & `database_mysql_local-0.0.311/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 PACKAGE_NAME = "database-mysql-local"
 package_dir = PACKAGE_NAME.replace("-", "_")
 
 setuptools.setup(
     name=PACKAGE_NAME,  # https://pypi.org/project/database-mysql-local
-    version='0.0.310',
+    version='0.0.311',
     author="Circles",
     author_email="info@circles.ai",
     url=f"https://github.com/circles-zone/{PACKAGE_NAME}-python-package",
     packages=[package_dir],
     package_dir={package_dir: f'{package_dir}/src'},
     package_data={package_dir: ['*.py']},
     long_description="Database MySQL Local",
```

