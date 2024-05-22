# Comparing `tmp/odp-0.0.7.tar.gz` & `tmp/odp-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp-0.0.7.tar", max compression
+gzip compressed data, was "odp-0.0.8.tar", max compression
```

## Comparing `odp-0.0.7.tar` & `odp-0.0.8.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      582 2024-05-16 13:50:22.714107 odp-0.0.7/LICENSE
--rw-r--r--   0        0        0     2002 2024-05-16 13:50:22.714494 odp-0.0.7/README.md
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.7/odp/__init__.py
--rw-r--r--   0        0        0       67 2024-05-16 13:50:22.714853 odp-0.0.7/odp/__main__.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.7/odp/cli/__init__.py
--rw-r--r--   0        0        0     4358 2024-05-16 13:58:56.864831 odp-0.0.7/odp/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.7/odp/core/__init__.py
--rw-r--r--   0        0        0     8773 2024-05-16 13:58:56.865397 odp-0.0.7/odp/core/detect_unused.py
--rw-r--r--   0        0        0     3121 2024-05-16 13:59:34.833764 odp-0.0.7/odp/core/snowflake.py
--rw-r--r--   0        0        0     1049 2024-05-16 13:58:56.865903 odp-0.0.7/odp/core/types.py
--rw-r--r--   0        0        0     2046 2024-05-16 14:00:15.859845 odp-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     2906 1970-01-01 00:00:00.000000 odp-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-05-22 18:48:13.696913 odp-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2014 2024-05-22 18:48:53.120329 odp-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.8/odp/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-22 18:48:13.697909 odp-0.0.8/odp/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.8/odp/cli/__init__.py
+-rw-r--r--   0        0        0     4358 2024-05-22 18:48:51.994326 odp-0.0.8/odp/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.8/odp/core/__init__.py
+-rw-r--r--   0        0        0     9113 2024-05-22 18:48:53.121470 odp-0.0.8/odp/core/detect_unused.py
+-rw-r--r--   0        0        0     3121 2024-05-22 18:48:51.994844 odp-0.0.8/odp/core/snowflake.py
+-rw-r--r--   0        0        0     1049 2024-05-22 18:48:51.995066 odp-0.0.8/odp/core/types.py
+-rw-r--r--   0        0        0     2046 2024-05-22 18:49:07.048480 odp-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 odp-0.0.8/PKG-INFO
```

### Comparing `odp-0.0.7/LICENSE` & `odp-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `odp-0.0.7/README.md` & `odp-0.0.8/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -15,21 +15,21 @@
 - **Github repository**: <https://github.com/open-data-products/odp/>
 - **Documentation** <https://open-data-products.github.io/odp/>
 
 ## Dev Usage
 
     poetry install
 
-    poetry run python -m odp detect-unused --info_schema_file=examples/snowflake_info_schema.csv --queries_file=examples/snowflake_query.csv
+    poetry run python -m odp detect-unused --info-schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
 
 or, run with snowflake env:
 
     cat <<EOF > .env
     ODP_SNOWFLAKE_ACCOUNT=your_account
-    ODP_SNOWFLAKE_USER=your_user
+    ODP_SNOWFLAKE_USERNAME=your_user
     ODP_SNOWFLAKE_PASSWORD=your_password
     ODP_SNOWFLAKE_DATABASE=your_database
     ODP_SNOWFLAKE_WAREHOUSE=your_warehouse # optional
     ODP_SNOWFLAKE_ROLE=your_role           # optional
     EOF
 
     poetry run python -m odp detect-unused
```

### Comparing `odp-0.0.7/odp/cli/main.py` & `odp-0.0.8/odp/cli/main.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.7/odp/core/detect_unused.py` & `odp-0.0.8/odp/core/detect_unused.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     # Read queries from a CSV file and return a list of dictionaries where each key is a column in the CSV
     with open(query_file) as f:
         csv_reader = csv.reader(f)
         header = list(map(str.upper, next(csv_reader)))
 
         rows = []
         for _row in csv_reader:
-            row = dict(zip(header,_row))
+            row = dict(zip(header, _row))
             row["START_TIME"] = datetime.fromisoformat(row["START_TIME"])
             query_row = QueryRow(**row)
             if query_row.START_TIME > since_datetime:
                 rows.append(query_row)
 
         return rows
 
@@ -111,22 +111,20 @@
         if column.table not in root.sources:
             continue
 
         table = root.sources[column.table]
         if type(table) != exp.Table:
             continue
 
-        columns.append(
-            (
-                table.catalog,
-                table.db,
-                table.name,
-                column.this.this,
-            )
-        )
+        columns.append((
+            table.catalog,
+            table.db,
+            table.name,
+            column.this.this,
+        ))
     return columns
 
 
 def extract_tables(
     query_text: str,
     database_name: str,
     catalog_name: str,
@@ -141,16 +139,16 @@
             parsed,
             db=database_name,
             catalog=catalog_name,
             schema=schema,
             dialect=dialect.value,
             infer_schema=True,
             expand_stars=False,  # we don't care about columns here
-            validate_qualify_columns=False, # we don't care about columns here
-            qualify_columns=False, # we don't care about columns here
+            validate_qualify_columns=False,  # we don't care about columns here
+            qualify_columns=False,  # we don't care about columns here
         )
         root = build_scope(qualified)
     except Exception as e:
         # todo - debug log these / write to file
         # print("Error parsing query", e, query_text)
         return []
 
@@ -159,21 +157,19 @@
         for _, (_, source) in scope.selected_sources.items():
             if isinstance(source, exp.Table):
                 table_exps.add(source)
 
     # converting table expressions to a list of tuples
     tables = []
     for table_exp in table_exps:
-        tables.append(
-            (
-                table_exp.catalog,
-                table_exp.db,
-                str(table_exp.this.name),
-            )
-        )
+        tables.append((
+            table_exp.catalog,
+            table_exp.db,
+            str(table_exp.this.name),
+        ))
     return tables
 
 
 def summarize_columns(columns):
     # Return a dictionary of column to counts
 
     # Flatten the col vals
@@ -196,17 +192,21 @@
             dialect=dialect,
         )
         for query in queries
     ]
     col_counts = summarize_columns(cols)
 
     # Print the most common columns in a human readable format with one column per line
-    print("Most common columns (20):")
-    for col, count in col_counts.most_common(20):
-        print(f"{col}: {count}")
+    if len(col_counts) > 0:
+        max_len = 20 if len(col_counts) > 20 else len(col_counts)
+        print(f"Most common columns (up to {max_len}):")
+        for col, count in col_counts.most_common(max_len):
+            print(f"{col}: {count}")
+    else:
+        print("No most common columns found in provided date range")
 
     # Identify columns that are never used by comparing the columns in the info schema to the columns in the queries
     info_schema_cols = set(info_schema_flat)
     used_cols = set(col_counts.keys())
     unused_cols = sorted(info_schema_cols - used_cols)
     print(f"Unused columns ({len(unused_cols)}):")
     for col in unused_cols:
@@ -230,18 +230,22 @@
         for query in queries
     ]
 
     tbls = [item for sublist in tables for item in sublist]
     table_counts = Counter(tbls)
 
     # Print the most common tables in a human-readable format with one table per line
-    print("Most common tables (20):")
-    for tbl, count in table_counts.most_common(20):
-        catalog, db, table = (obj.upper() for obj in tbl)
-        print(f"{catalog}.{db}.{table}: {count}")
+    if len(table_counts) > 0:
+        max_len = 20 if len(table_counts) > 20 else len(table_counts)
+        print(f"Most common tables (up to {max_len}):")
+        for tbl, count in table_counts.most_common(max_len):
+            catalog, db, table = (obj.upper() for obj in tbl)
+            print(f"{catalog}.{db}.{table}: {count}")
+    else:
+        print("No most common tables found in provided date range")
 
     # Identify tables that are never used by comparing the tables in the info schema to the tables in the queries
     info_schema_tables = set()
     for table in info_schema_flat:
         info_schema_tables.add((table[0].upper(), table[1].upper(), table[2].upper()))
 
     used_tables = set(table_counts.keys())
```

### Comparing `odp-0.0.7/odp/core/snowflake.py` & `odp-0.0.8/odp/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.7/odp/core/types.py` & `odp-0.0.8/odp/core/types.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.7/pyproject.toml` & `odp-0.0.8/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp"
-version = "0.0.7"
+version = "0.0.8"
 description = "odp"
 authors = ["odp Authors <fdexter@metalytics.dev>"]
 repository = "https://github.com/open-data-products/odp"
 documentation = "https://open-data-products.github.io/odp/"
 readme = "README.md"
 packages = [
   {include = "odp"}
```

### Comparing `odp-0.0.7/PKG-INFO` & `odp-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp
-Version: 0.0.7
+Version: 0.0.8
 Summary: odp
 Home-page: https://github.com/open-data-products/odp
 Author: odp Authors
 Author-email: fdexter@metalytics.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -38,21 +38,21 @@
 - **Github repository**: <https://github.com/open-data-products/odp/>
 - **Documentation** <https://open-data-products.github.io/odp/>
 
 ## Dev Usage
 
     poetry install
 
-    poetry run python -m odp detect-unused --info_schema_file=examples/snowflake_info_schema.csv --queries_file=examples/snowflake_query.csv
+    poetry run python -m odp detect-unused --info-schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
 
 or, run with snowflake env:
 
     cat <<EOF > .env
     ODP_SNOWFLAKE_ACCOUNT=your_account
-    ODP_SNOWFLAKE_USER=your_user
+    ODP_SNOWFLAKE_USERNAME=your_user
     ODP_SNOWFLAKE_PASSWORD=your_password
     ODP_SNOWFLAKE_DATABASE=your_database
     ODP_SNOWFLAKE_WAREHOUSE=your_warehouse # optional
     ODP_SNOWFLAKE_ROLE=your_role           # optional
     EOF
 
     poetry run python -m odp detect-unused
```

