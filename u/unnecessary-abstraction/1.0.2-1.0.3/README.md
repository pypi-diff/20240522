# Comparing `tmp/unnecessary_abstraction-1.0.2.tar.gz` & `tmp/unnecessary-abstraction-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unnecessary_abstraction-1.0.2.tar", max compression
+gzip compressed data, was "unnecessary-abstraction-1.0.3.tar", last modified: Wed May 22 10:54:48 2024, max compression
```

## Comparing `unnecessary_abstraction-1.0.2.tar` & `unnecessary-abstraction-1.0.3.tar`

### file list

```diff
@@ -1,10 +1,18 @@
--rw-r--r--   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary_abstraction-1.0.2/database_interface/__init__.py
--rw-r--r--   0        0        0     3789 2024-04-17 10:39:30.000000 unnecessary_abstraction-1.0.2/database_interface/database.py
--rw-r--r--   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary_abstraction-1.0.2/database_interface/database_interface.py
--rw-r--r--   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary_abstraction-1.0.2/database_interface/postgis_interface.py
--rw-r--r--   0        0        0    16687 2024-05-06 13:30:00.401742 unnecessary_abstraction-1.0.2/database_interface/postgres_interface.py
--rw-r--r--   0        0        0     3801 2024-05-05 02:09:59.336969 unnecessary_abstraction-1.0.2/database_interface/schema_objects.py
--rw-r--r--   0        0        0    12833 2024-05-05 02:09:29.709757 unnecessary_abstraction-1.0.2/database_interface/sqlite_interface.py
--rw-r--r--   0        0        0      419 2024-05-07 00:14:00.579999 unnecessary_abstraction-1.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-05 12:17:36.486574 unnecessary_abstraction-1.0.2/README.md
--rw-r--r--   0        0        0      495 1970-01-01 00:00:00.000000 unnecessary_abstraction-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 10:54:48.888293 unnecessary-abstraction-1.0.3/
+-rw-rw-rw-   0        0        0      348 2024-05-22 10:54:48.888293 unnecessary-abstraction-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 10:54:48.878292 unnecessary-abstraction-1.0.3/database_interface/
+-rw-rw-rw-   0        0        0      306 2024-04-17 21:48:39.000000 unnecessary-abstraction-1.0.3/database_interface/__init__.py
+-rw-rw-rw-   0        0        0     3275 2024-05-22 10:40:22.000000 unnecessary-abstraction-1.0.3/database_interface/database.py
+-rw-rw-rw-   0        0        0    15397 2024-02-24 03:42:20.000000 unnecessary-abstraction-1.0.3/database_interface/database_interface.py
+-rw-rw-rw-   0        0        0     1499 2024-04-09 10:09:47.000000 unnecessary-abstraction-1.0.3/database_interface/postgis_interface.py
+-rw-rw-rw-   0        0        0    16298 2024-05-22 10:39:23.000000 unnecessary-abstraction-1.0.3/database_interface/postgres_interface.py
+-rw-rw-rw-   0        0        0     3803 2024-05-22 10:33:50.000000 unnecessary-abstraction-1.0.3/database_interface/schema_objects.py
+-rw-rw-rw-   0        0        0    12833 2024-05-05 02:09:29.000000 unnecessary-abstraction-1.0.3/database_interface/sqlite_interface.py
+-rw-rw-rw-   0        0        0       42 2024-05-22 10:54:48.888293 unnecessary-abstraction-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      721 2024-05-22 10:54:29.000000 unnecessary-abstraction-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 10:54:48.887292 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/
+-rw-rw-rw-   0        0        0      348 2024-05-22 10:54:48.000000 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      502 2024-05-22 10:54:48.000000 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 10:54:48.000000 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-05-22 10:54:48.000000 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-22 10:54:48.000000 unnecessary-abstraction-1.0.3/unnecessary_abstraction.egg-info/top_level.txt
```

### Comparing `unnecessary_abstraction-1.0.2/database_interface/database.py` & `unnecessary-abstraction-1.0.3/database_interface/database.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,72 +9,72 @@
 
 class Database(Protocol):
 
     @property
     def db_conn(self) -> psycopg2.extensions.connection:
         ...
 
-    def table_from_records(self, table_name:str, table_records:list[dict], col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None, postgresql_schema:str="public") -> None:
+    def table_from_records(self, table_name:str, table_records:list[dict], col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None) -> None:
         ...
 
-    def table_append_records(self, table_name:str, table_records:list[dict[str]], postgresql_schema:str="public") -> None:
+    def table_append_records(self, table_name:str, table_records:list[dict[str]]) -> None:
         ...
     
-    def update_with_unique_records(self, table_name:str, records:list[dict], unique_key_col:str, postgresql_schema:str="public") -> None:
+    def update_with_unique_records(self, table_name:str, records:list[dict], unique_key_col:str) -> None:
         ...
 
-    def delete_rows(self, table_name:str, where_clause:str, postgresql_schema:str="public") -> None:
+    def delete_rows(self, table_name:str, where_clause:str) -> None:
         ...
 
     def append_csv_to_table(self, table_name:str, csv_path:str) -> None:
         ...
     
     def records_to_csv(self, csv_name:str, csv_path:str) -> None:
         ...
 
-    def create_blank_table(self, table_name:str, schema:SQLSchema, postgresql_schema:str="public") -> None:
+    def create_blank_table(self, table_name:str, schema:SQLSchema) -> None:
         ...
     
     def csv_to_records(self, csv_path:str) -> list[dict]:
         ...
 
-    def csv_to_table(self, csv_path:str, col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None, postgresql_schema:str = "public") -> None:
+    def csv_to_table(self, csv_path:str, col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None) -> None:
         ...
 
-    def table_to_records(self, table_name:str, columns:str="*", where_clause:str="", postgresql_schema:str="public") -> list[dict]:
+    def table_to_records(self, table_name:str, columns:str="*", where_clause:str="") -> list[dict]:
         ...
     
-    def table_to_csv(self, table_name:str, save_path:str=".", columns:str="*", where_clause:str="", postgresql_schema:str="public") -> None:
+    def table_to_csv(self, table_name:str, save_path:str=".", columns:str="*", where_clause:str="") -> None:
         ...
 
     def drop_table(self, table_name:str) -> None:
         ...
     
-    def delete_all_records(self, table_name:str, postgresql_schema:str="public") -> None:
+    def delete_all_records(self, table_name:str) -> None:
         ...
 
-    def add_column(self, table_name:str, col_name:str, data_type:DB_TYPE_LIST, postgresql_schema:str="public") -> None:
+    def add_column(self, table_name:str, col_name:str, data_type:DB_TYPE_LIST) -> None:
         ...
     
-    def drop_column(self, table_name:str, col_name:str, postgresql_schema:str="public") -> None:
+    def drop_column(self, table_name:str, col_name:str) -> None:
         ...
     
-    def rename_column(self, table_name:str, col_name:str, new_col_name:str, postgresql_schema:str="public") -> None:
+    def rename_column(self, table_name:str, col_name:str, new_col_name:str) -> None:
         ...
 
-    def rename_table(self, table_name:str, new_table_name:str, postgresql_schema:str="public") -> None:
+    def rename_table(self, table_name:str, new_table_name:str) -> None:
         ...
 
-    def list_tables(self, postgresql_schema:str="public") -> list[str]:
+    def list_tables(self) -> list[str]:
         ...
 
-    def get_schema(self, table_name:str, postgresql_schema:str="public") -> SQLSchema:
+    def get_schema(self, table_name:str) -> SQLSchema:
         ...
 
-    def get_table(self, table_name:str, columns:str="*", where_clause:str="", postgresql_schema:str="public") -> list[tuple]:
+    def get_table(self, table_name:str, columns:str="*", where_clause:str="") -> list[tuple]:
         ...
 
     def evaluate_schema(self, records:list[dict], col_overrides:list[SQLColumn]=[]) -> SQLSchema:
         ...
 
     def select_table_statement(self, table_name:str, columns:str="*", where_clause:str="") -> str:
         ...
```

### Comparing `unnecessary_abstraction-1.0.2/database_interface/database_interface.py` & `unnecessary-abstraction-1.0.3/database_interface/database_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.2/database_interface/postgis_interface.py` & `unnecessary-abstraction-1.0.3/database_interface/postgis_interface.py`

 * *Files identical despite different names*

### Comparing `unnecessary_abstraction-1.0.2/database_interface/postgres_interface.py` & `unnecessary-abstraction-1.0.3/database_interface/postgres_interface.py`

 * *Files 11% similar despite different names*

```diff
@@ -18,58 +18,59 @@
                      "real": "real", "double precision": "double precision", "decimal": "decimal", "numeric": "numeric", 
                      "smallserial": "smallserial", "serial": "serial", "bigserial": "bigserial", "geometry": "text", "text": "text", 
                      "timestamp": "timestamp", "timestamp with time zone": "timestamp with time zone", "boolean": "boolean",
                      "date": "date", "time with time zone": "time with time zone", "time": "time", "interval": "interval",
                      "uuid": "uuid DEFAULT gen_random_uuid()", "json": "json", "jsonb": "jsonb"}
 
 class PostgreSQL(Database):
-    def __init__(self, db_name:str, username:str, password:str, host="localhost", port=5432, type_map=POSTGRES_TYPE_MAP):
+    def __init__(self, db_name:str, username:str, password:str, schema:str, host="localhost", port=5432, type_map=POSTGRES_TYPE_MAP):
         self.__db_conn = psycopg2.connect(database=db_name, user=username, password=password, host=host, port=port)
         self.__binding_char = "%s"
         self.__type_map = type_map
+        self.__schema_namespace = schema
 
     @property
     def db_conn(self):
         return self.__db_conn
 
-    def table_from_records(self, table_name:str, table_records:list[dict], col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None, postgresql_schema:str="public") -> None:
+    def table_from_records(self, table_name:str, table_records:list[dict], col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None) -> None:
         schema:SQLSchema = schema_override
         if not schema_override:
             schema = self.evaluate_schema(table_records, col_overrides)
 
-        create_statement = self.create_table_statement(f"{postgresql_schema}.{table_name}", schema)
-        insert_statement = self.insert_into_table_statement(f"{postgresql_schema}.{table_name}", schema)
+        create_statement = self.create_table_statement(f"{self.__schema_namespace}.{table_name}", schema)
+        insert_statement = self.insert_into_table_statement(f"{self.__schema_namespace}.{table_name}", schema)
         table_records_sql = [tuple(val for val in row.values()) for row in table_records]
 
         cur = self.db_conn.cursor()
         cur.execute(create_statement)
         cur.executemany(insert_statement, table_records_sql)
         self.db_conn.commit()
 
-    def table_append_records(self, table_name:str, table_records:list[dict[str]], postgresql_schema:str="public") -> None:
-        schema = self.get_schema(table_name, postgresql_schema)
+    def table_append_records(self, table_name:str, table_records:list[dict[str]]) -> None:
+        schema = self.get_schema(table_name, self.__schema_namespace)
         schema.filter_columns(list(table_records[0].keys()))
         
-        insert_statement = self.insert_into_table_statement(f"{postgresql_schema}.{table_name}", schema)
+        insert_statement = self.insert_into_table_statement(f"{self.__schema_namespace}.{table_name}", schema)
         table_records_sql = [tuple(val for val in row.values()) for row in table_records]
 
         cur = self.db_conn.cursor()
         cur.executemany(insert_statement, table_records_sql)
         self.db_conn.commit()
 
-    def update_with_unique_records(self, table_name:str, records:list[dict], unique_key_col:str, postgresql_schema:str="public") -> None:
+    def update_with_unique_records(self, table_name:str, records:list[dict], unique_key_col:str) -> None:
         cur = self.db_conn.cursor()
         for row in records:
-            update_statement = self.create_update_statement(f"{postgresql_schema}.{table_name}", row, f"WHERE {unique_key_col}='{row[unique_key_col]}'")
+            update_statement = self.create_update_statement(f"{self.__schema_namespace}.{table_name}", row, f"WHERE {unique_key_col}='{row[unique_key_col]}'")
             cur.execute(update_statement)
         self.db_conn.commit()
 
-    def delete_rows(self, table_name:str, where_clause:str, postgresql_schema:str="public") -> None:
+    def delete_rows(self, table_name:str, where_clause:str) -> None:
         cur = self.db_conn.cursor()
-        delete_statement = self.create_delete_statement(f"{postgresql_schema}.{table_name}", where_clause)
+        delete_statement = self.create_delete_statement(f"{self.__schema_namespace}.{table_name}", where_clause)
         cur.execute(delete_statement)
         self.db_conn.commit()
 
     def append_csv_to_table(self, table_name:str, csv_path:str) -> None:
         csv_path:pathlib.Path = pathlib.Path(csv_path)
         with open(csv_path, newline='') as csv_file:
             reader = csv.DictReader(csv_file)
@@ -79,16 +80,16 @@
     def records_to_csv(self, records:list[dict], csv_name:str, csv_path:str) -> None:
         headers = records[0].keys()
         with open(f"{csv_path}\\{csv_name}.csv", "w", newline='') as f:
             writer = csv.DictWriter(f, headers)
             writer.writeheader()
             writer.writerows(records)
 
-    def create_blank_table(self, table_name:str, schema:SQLSchema, postgresql_schema:str="public") -> None:
-        sql = self.create_table_statement(f"{postgresql_schema}.{table_name}", schema)
+    def create_blank_table(self, table_name:str, schema:SQLSchema) -> None:
+        sql = self.create_table_statement(f"{self.__schema_namespace}.{table_name}", schema)
         cur = self.db_conn.cursor()
         cur.execute(sql)
         self.db_conn.commit()
         
     def csv_to_records(self, csv_path:str) -> list[dict]:
         csv_path:pathlib.Path = pathlib.Path(csv_path)
         with open(csv_path, newline='') as csv_file:
@@ -98,85 +99,85 @@
         for row in records:
             for key, val in row.items():
                 if val == '':
                     row[key] = None
     
         return records
     
-    def csv_to_table(self, csv_path:str, col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None, postgresql_schema:str = "public") -> None:
+    def csv_to_table(self, csv_path:str, col_overrides:list[SQLColumn]=[], schema_override:SQLSchema=None) -> None:
         csv_name = pathlib.Path(csv_path).stem
         records = self.csv_to_records(csv_path)
         if csv_name in self.list_tables():
             print(f"{csv_name} is already a table in the database. You can alternatively use append_csv() if this is intended")
             return
-        self.table_from_records(csv_name, records, col_overrides, schema_override, postgresql_schema)
+        self.table_from_records(csv_name, records, col_overrides, schema_override, self.__schema_namespace)
 
-    def table_to_records(self, table_name:str, columns:str="*", where_clause:str="", postgresql_schema:str="public") -> list[dict]:
-        schema:SQLSchema = self.get_schema(table_name, postgresql_schema)
-        table_data = self.get_table(table_name, columns, where_clause, postgresql_schema)
+    def table_to_records(self, table_name:str, columns:str="*", where_clause:str="") -> list[dict]:
+        schema:SQLSchema = self.get_schema(table_name, self.__schema_namespace)
+        table_data = self.get_table(table_name, columns, where_clause, self.__schema_namespace)
 
         if columns != "*":
             schema.filter_columns(columns.split(", "))
             
         records = []
         for row in table_data:
             record_row = {}
             for col_name, sql_col in schema.schema_map.items():
                 record_row[col_name] = row[sql_col.position - 1]
             records.append(record_row)
 
         return records
 
-    def table_to_csv(self, table_name:str, save_path:str=".", columns:str="*", where_clause:str="", postgresql_schema:str="public") -> None:
-        table_records = self.table_to_records(table_name, columns, where_clause, postgresql_schema)
+    def table_to_csv(self, table_name:str, save_path:str=".", columns:str="*", where_clause:str="") -> None:
+        table_records = self.table_to_records(table_name, columns, where_clause, self.__schema_namespace)
         headers:dict = table_records[0]
         headers = headers.keys()
 
         with open(f"{save_path}\\{table_name}.csv", 'w', newline='') as csv_file:
             writer = csv.DictWriter(csv_file, fieldnames=headers)
             writer.writeheader()
             writer.writerows(table_records)
     
-    def drop_table(self, table_name:str, postgresql_schema:str) -> None:
+    def drop_table(self, table_name:str) -> None:
         cur = self.db_conn.cursor()
-        cur.execute(f"DROP TABLE IF EXISTS {postgresql_schema}.{table_name}")
+        cur.execute(f"DROP TABLE IF EXISTS {self.__schema_namespace}.{table_name}")
         self.db_conn.commit()
     
-    def delete_all_records(self, table_name:str, postgresql_schema:str="public") -> None:
+    def delete_all_records(self, table_name:str) -> None:
         cur = self.db_conn.cursor()
-        cur.execute(f"DELETE FROM {postgresql_schema}.{table_name}")
+        cur.execute(f"DELETE FROM {self.__schema_namespace}.{table_name}")
         self.db_conn.commit()
 
-    def add_column(self, table_name:str, col_name:str, data_type:POSTGRES_TYPES, postgresql_schema:str="public") -> None:
+    def add_column(self, table_name:str, col_name:str, data_type:POSTGRES_TYPES) -> None:
         cur = self.db_conn.cursor()
-        sql_statement = f"ALTER TABLE {postgresql_schema}.{table_name} ADD {col_name} {self.__type_map[data_type]}"
+        sql_statement = f"ALTER TABLE {self.__schema_namespace}.{table_name} ADD {col_name} {self.__type_map[data_type]}"
         cur.execute(sql_statement)
         self.db_conn.commit()
     
-    def drop_column(self, table_name:str, col_name:str, postgresql_schema:str="public") -> None:
+    def drop_column(self, table_name:str, col_name:str) -> None:
         cur = self.db_conn.cursor()
-        sql_statement = f"ALTER TABLE {postgresql_schema}.{table_name} DROP COLUMN {col_name}"
+        sql_statement = f"ALTER TABLE {self.__schema_namespace}.{table_name} DROP COLUMN {col_name}"
         cur.execute(sql_statement)
         self.db_conn.commit()
     
-    def rename_column(self, table_name:str, col_name:str, new_col_name:str, postgresql_schema:str="public") -> None:
+    def rename_column(self, table_name:str, col_name:str, new_col_name:str) -> None:
         cur = self.db_conn.cursor()
-        sql_statement = f"ALTER TABLE {postgresql_schema}.{table_name} RENAME COLUMN {col_name} TO {new_col_name}"
+        sql_statement = f"ALTER TABLE {self.__schema_namespace}.{table_name} RENAME COLUMN {col_name} TO {new_col_name}"
         cur.execute(sql_statement)
         self.db_conn.commit()
 
-    def rename_table(self, table_name:str, new_table_name:str, postgresql_schema:str="public") -> None:
+    def rename_table(self, table_name:str, new_table_name:str) -> None:
         cur = self.db_conn.cursor()
-        sql_statement = f"ALTER TABLE {postgresql_schema}.{table_name} RENAME TO {new_table_name}"
+        sql_statement = f"ALTER TABLE {self.__schema_namespace}.{table_name} RENAME TO {new_table_name}"
         cur.execute(sql_statement)
         self.db_conn.commit()
 
-    def alter_column(self, table_name:str, col_name:str, data_type:POSTGRES_TYPES, postgresql_schema:str="public") -> None:
+    def alter_column(self, table_name:str, col_name:str, data_type:POSTGRES_TYPES) -> None:
         cur = self.db_conn.cursor()
-        sql_statement = f"ALTER TABLE {postgresql_schema}.{table_name} ALTER COLUMN {col_name} {self.__type_map[data_type]}"
+        sql_statement = f"ALTER TABLE {self.__schema_namespace}.{table_name} ALTER COLUMN {col_name} {self.__type_map[data_type]}"
         cur.execute(sql_statement)
         self.db_conn.commit()
 
     def create_trigger_function(self, function_name:str, function_sql:str) -> None:
         create_function = f"CREATE OR REPLACE FUNCTION {function_name}() RETURNS trigger AS $$"
         create_function += f"BEGIN {function_sql}"
         create_function += "END; $$ LANGUAGE plpgsql;"
@@ -190,37 +191,37 @@
         trigger_sql += f"AFTER {after_action} ON {table_name}"
         trigger_sql += f"FOR EACH {for_each} EXECUTE FUNCTION {call_function}();"
 
         cur = self.db_conn.cursor()
         cur.execute(trigger_sql)
         self.db_conn.commit()
 
-    def list_tables(self, postgresql_schema:str="public") -> list[str]:
+    def list_tables(self) -> list[str]:
         cur = self.db_conn.cursor()
-        sql = f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{postgresql_schema}'"
+        sql = f"SELECT table_name FROM information_schema.tables WHERE table_schema = '{self.__schema_namespace}'"
         cur.execute(sql)
         return [table[0] for table in cur.fetchall()]
 
-    def get_schema(self, table_name:str, postgresql_schema:str="public") -> SQLSchema:
-        GET_COL_SCHEMA = f"SELECT column_name, data_type, ordinal_position, is_nullable FROM information_schema.columns WHERE table_schema='{postgresql_schema}' AND table_name='{table_name}'"
+    def get_schema(self, table_name:str) -> SQLSchema:
+        GET_COL_SCHEMA = f"SELECT column_name, data_type, ordinal_position, is_nullable FROM information_schema.columns WHERE table_schema='{self.__schema_namespace}' AND table_name='{table_name}'"
         cur = self.db_conn.cursor()
         cur.execute(GET_COL_SCHEMA)
         col_list = []
         for col in cur.fetchall():
             if col[3] == 'YES':
                 nullable = True
             else:
                 nullable = False
             col_list.append(SQLColumn(col[0], col[1], col[2], nullable))
 
         schema = SQLSchema(col_list)
         return schema
     
-    def get_table(self, table_name:str, columns:str="*", where_clause:str="", postgresql_schema:str="public") -> list[tuple]:
-        select_statement = self.select_table_statement(f"{postgresql_schema}.{table_name}", columns, where_clause)
+    def get_table(self, table_name:str, columns:str="*", where_clause:str="") -> list[tuple]:
+        select_statement = self.select_table_statement(f"{self.__schema_namespace}.{table_name}", columns, where_clause)
         cur = self.db_conn.cursor()
         cur.execute(select_statement)
         return cur.fetchall()
 
     def evaluate_schema(self, records:list[dict], col_overrides:list[SQLColumn]=[]) -> SQLSchema:
 
         def find_non_null_record(records:list[dict], col_name:str):
```

### Comparing `unnecessary_abstraction-1.0.2/database_interface/schema_objects.py` & `unnecessary-abstraction-1.0.3/database_interface/schema_objects.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         self.check_constraint:str = check_constraint
 
     def __repr__(self) -> str:
         text = f"{self.name} (data_type: {self.data_type}, position: {self.position}, nullable: {self.nullable}, unique: {self.is_unique}, "
         if self.is_primary_key:
             text += f"Primary Key, "
         if self.foreign_key:
-            text += f"Foreign Key: references {self.foreign_key['refences_table']} ({self.foreign_key['references_col']}, "
+            text += f"Foreign Key: references {self.foreign_key['references_table']} ({self.foreign_key['references_col']}, "
         if self.check_constraint:
             text += f"Check Constraint: {self.check_constraint}, "
         
         text = text[:-2] + ")"
         return text
 
 class SQLSchema:
```

### Comparing `unnecessary_abstraction-1.0.2/database_interface/sqlite_interface.py` & `unnecessary-abstraction-1.0.3/database_interface/sqlite_interface.py`

 * *Files identical despite different names*

