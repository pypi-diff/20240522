# Comparing `tmp/odp-0.0.8.tar.gz` & `tmp/odp-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp-0.0.8.tar", max compression
+gzip compressed data, was "odp-0.0.9.tar", max compression
```

## Comparing `odp-0.0.8.tar` & `odp-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      582 2024-05-22 18:48:13.696913 odp-0.0.8/LICENSE
--rw-r--r--   0        0        0     2014 2024-05-22 18:48:53.120329 odp-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.8/odp/__init__.py
--rw-r--r--   0        0        0       67 2024-05-22 18:48:13.697909 odp-0.0.8/odp/__main__.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.8/odp/cli/__init__.py
--rw-r--r--   0        0        0     4358 2024-05-22 18:48:51.994326 odp-0.0.8/odp/cli/main.py
--rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.8/odp/core/__init__.py
--rw-r--r--   0        0        0     9113 2024-05-22 18:48:53.121470 odp-0.0.8/odp/core/detect_unused.py
--rw-r--r--   0        0        0     3121 2024-05-22 18:48:51.994844 odp-0.0.8/odp/core/snowflake.py
--rw-r--r--   0        0        0     1049 2024-05-22 18:48:51.995066 odp-0.0.8/odp/core/types.py
--rw-r--r--   0        0        0     2046 2024-05-22 18:49:07.048480 odp-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 odp-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      582 2024-05-22 18:48:13.696913 odp-0.0.9/LICENSE
+-rw-r--r--   0        0        0     2009 2024-05-22 18:52:02.684867 odp-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.352855 odp-0.0.9/odp/__init__.py
+-rw-r--r--   0        0        0       67 2024-05-22 18:48:13.697909 odp-0.0.9/odp/__main__.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353425 odp-0.0.9/odp/cli/__init__.py
+-rw-r--r--   0        0        0     4384 2024-05-22 19:03:49.781288 odp-0.0.9/odp/cli/main.py
+-rw-r--r--   0        0        0        0 2024-05-13 16:35:32.353850 odp-0.0.9/odp/core/__init__.py
+-rw-r--r--   0        0        0     9103 2024-05-22 18:55:50.063130 odp-0.0.9/odp/core/detect_unused.py
+-rw-r--r--   0        0        0     3121 2024-05-22 18:48:51.994844 odp-0.0.9/odp/core/snowflake.py
+-rw-r--r--   0        0        0     1049 2024-05-22 18:48:51.995066 odp-0.0.9/odp/core/types.py
+-rw-r--r--   0        0        0     2046 2024-05-22 19:04:09.971319 odp-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2913 1970-01-01 00:00:00.000000 odp-0.0.9/PKG-INFO
```

### Comparing `odp-0.0.8/LICENSE` & `odp-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odp-0.0.8/README.md` & `odp-0.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 - **Github repository**: <https://github.com/open-data-products/odp/>
 - **Documentation** <https://open-data-products.github.io/odp/>
 
 ## Dev Usage
 
     poetry install
 
-    poetry run python -m odp detect-unused --info-schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
+    poetry run python -m odp detect-unused --schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
 
 or, run with snowflake env:
 
     cat <<EOF > .env
     ODP_SNOWFLAKE_ACCOUNT=your_account
     ODP_SNOWFLAKE_USERNAME=your_user
     ODP_SNOWFLAKE_PASSWORD=your_password
```

### Comparing `odp-0.0.8/odp/cli/main.py` & `odp-0.0.9/odp/cli/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,23 @@
+import os
+
 import click
 from dotenv import load_dotenv
 
 from odp.core.detect_unused import (
     build_info_schema,
     detect_unused_columns,
     detect_unused_tables,
     read_info_schema_from_file,
     read_queries,
 )
 from odp.core.snowflake import get_snowflake_queries, get_snowflake_schema, load_snowflake_credentials
 from odp.core.types import Dialect, Grain, validate_dialect, validate_grain
 
-load_dotenv()
+load_dotenv(dotenv_path=os.path.join(os.getcwd(), ".env"))
 
 
 @click.group(name="odp")
 def cli():
     pass
 
 
@@ -24,15 +26,15 @@
     help="""
 Detect unused columns in SQL queries.
 Requires two files: a query file and an information schema file.
 Run `show-queries` to see the SQL queries to run against your
 Snowflake instance to generate the two files.""",
 )
 @click.option("--queries-file", help="The SQL query file to analyze.")
-@click.option("--info-schema-file", help="The file containing the information schema for the database.")
+@click.option("--schema-file", help="The file containing the information schema for the database.")
 @click.option(
     "--dialect",
     type=click.Choice([d.value for d in Dialect]),
     callback=validate_dialect,
     default="snowflake",
     help="The type of warehouse to connect to. Currently only snowflake is supported.",
 )
@@ -47,25 +49,25 @@
     "--since-days",
     type=click.INT,
     default=60,
     help="Count as 'unused' any asset that has not been queried in the last N days. Defaults to 60 days",
 )
 def cli_detect_unused_columns(
     queries_file: str | None,
-    info_schema_file: str | None,
+    schema_file: str | None,
     dialect: Dialect,
     grain: Grain,
     since_days: int,
 ):
-    if queries_file and info_schema_file:
+    if queries_file and schema_file:
         queries = read_queries(queries_file, since_days)
         print(f"Read {len(queries)} queries from {queries_file}")
 
-        info_schema, info_schema_flat = read_info_schema_from_file(info_schema_file)
-        print(f"Read {len(info_schema_flat)} information schema rows from {info_schema_file}")
+        info_schema, info_schema_flat = read_info_schema_from_file(schema_file)
+        print(f"Read {len(info_schema_flat)} information schema rows from {schema_file}")
         if grain == Grain.column:
             detect_unused_columns(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.table:
             detect_unused_tables(queries, info_schema, info_schema_flat, dialect)
         elif grain == Grain.schema:
             raise NotImplementedError("Schema grain is not yet supported")
 
@@ -75,15 +77,15 @@
         try:
             credentials = load_snowflake_credentials()
         except KeyError as e:
             raise ValueError(
                 f"""
 Missing or invalid parameters: {e}. Please provide either
 
-   1. both of --info_schema-file and --queries-file (use "odp show-queries" to learn how to generate these)
+   1. both of --info-schema-file and --queries-file (use "odp show-queries" to learn how to generate these)
    2. valid crendentials via env, e.g. ODP_SNOWFLAKE_ACCOUNT, ODP_SNOWFLAKE_USER, etc
             """
             ) from e
 
         schema = get_snowflake_schema(credentials)
         queries = get_snowflake_queries(credentials, since_days)
 
@@ -111,15 +113,15 @@
 SELECT *
 FROM SNOWFLAKE.ACCOUNT_USAGE.QUERY_HISTORY
 WHERE QUERY_TEXT ILIKE 'select%'
 ORDER BY START_TIME DESC
 LIMIT 10000; -- or start_time > $SOME_DATE to get columns unused in the last N days
 
 
--- info_schema_file
+-- schema_file
 
 use database MY_DATABASE; -- change me
 
 SELECT
 TABLE_CATALOG,
 TABLE_SCHEMA,
 TABLE_NAME,
```

### Comparing `odp-0.0.8/odp/core/detect_unused.py` & `odp-0.0.9/odp/core/detect_unused.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,19 +26,19 @@
             query_row = QueryRow(**row)
             if query_row.START_TIME > since_datetime:
                 rows.append(query_row)
 
         return rows
 
 
-def read_info_schema_from_file(info_schema_file) -> tuple[dict, list[tuple]]:
+def read_info_schema_from_file(schema_file) -> tuple[dict, list[tuple]]:
     # Read the info schema from a CSV file and return it as both a nested dictionary and a flat list
     # Format is: catalog -> schema -> table name -> column name
     schema_rows: list[SchemaRow] = []
-    with open(info_schema_file) as f:
+    with open(schema_file) as f:
         csv_reader = csv.reader(f)
         next(csv_reader)  # Skip header
         for row in csv_reader:
             catalog, schema_name, table_name, column_name = map(str.upper, row)
             schema_rows.append(
                 SchemaRow(
                     TABLE_CATALOG=catalog,
```

### Comparing `odp-0.0.8/odp/core/snowflake.py` & `odp-0.0.9/odp/core/snowflake.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.8/odp/core/types.py` & `odp-0.0.9/odp/core/types.py`

 * *Files identical despite different names*

### Comparing `odp-0.0.8/pyproject.toml` & `odp-0.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp"
-version = "0.0.8"
+version = "0.0.9"
 description = "odp"
 authors = ["odp Authors <fdexter@metalytics.dev>"]
 repository = "https://github.com/open-data-products/odp"
 documentation = "https://open-data-products.github.io/odp/"
 readme = "README.md"
 packages = [
   {include = "odp"}
```

### Comparing `odp-0.0.8/PKG-INFO` & `odp-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp
-Version: 0.0.8
+Version: 0.0.9
 Summary: odp
 Home-page: https://github.com/open-data-products/odp
 Author: odp Authors
 Author-email: fdexter@metalytics.dev
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -38,15 +38,15 @@
 - **Github repository**: <https://github.com/open-data-products/odp/>
 - **Documentation** <https://open-data-products.github.io/odp/>
 
 ## Dev Usage
 
     poetry install
 
-    poetry run python -m odp detect-unused --info-schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
+    poetry run python -m odp detect-unused --schema-file=examples/snowflake/info-schema.csv --queries-file=examples/snowflake/query-history.csv
 
 or, run with snowflake env:
 
     cat <<EOF > .env
     ODP_SNOWFLAKE_ACCOUNT=your_account
     ODP_SNOWFLAKE_USERNAME=your_user
     ODP_SNOWFLAKE_PASSWORD=your_password
```

