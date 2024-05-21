# Comparing `tmp/snowflake-snowpark-python-1.8.0.tar.gz` & `tmp/snowflake-snowpark-python-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snowflake-snowpark-python-1.8.0.tar", last modified: Fri Sep 15 20:48:12 2023, max compression
+gzip compressed data, was "snowflake-snowpark-python-1.9.0.tar", last modified: Mon Oct 16 18:52:42 2023, max compression
```

## Comparing `snowflake-snowpark-python-1.8.0.tar` & `snowflake-snowpark-python-1.9.0.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.415862 snowflake-snowpark-python-1.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35931 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      242 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    43249 2023-09-15 20:48:12.415862 snowflake-snowpark-python-1.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4761 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-09-15 20:48:12.415862 snowflake-snowpark-python-1.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.407862 snowflake-snowpark-python-1.8.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.407862 snowflake-snowpark-python-1.8.0/src/snowflake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.411862 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.411862 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.415862 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39182 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    36458 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     7168 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
--rw-r--r--   0 runner    (1001) docker     (127)    11320 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    44868 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py
--rw-r--r--   0 runner    (1001) docker     (127)    41929 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/table_function.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3365 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py
--rw-r--r--   0 runner    (1001) docker     (127)    26803 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/code_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    16330 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/error_message.py
--rw-r--r--   0 runner    (1001) docker     (127)    22428 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/packaging_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    26531 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/server_connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/telemetry.py
--rw-r--r--   0 runner    (1001) docker     (127)    24339 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/type_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    42172 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/udf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    28018 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16568 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/async_job.py
--rw-r--r--   0 runner    (1001) docker     (127)    34332 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/column.py
--rw-r--r--   0 runner    (1001) docker     (127)      550 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/context.py
--rw-r--r--   0 runner    (1001) docker     (127)   158150 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    23472 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_na_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    31616 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_reader.py
--rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_stat_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    15570 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    17528 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/file_operation.py
--rw-r--r--   0 runner    (1001) docker     (127)     8301 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/files.py
--rw-r--r--   0 runner    (1001) docker     (127)   304476 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/query_history.py
--rw-r--r--   0 runner    (1001) docker     (127)    18102 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/relational_grouped_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (127)    12095 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/row.py
--rw-r--r--   0 runner    (1001) docker     (127)   118446 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/session.py
--rw-r--r--   0 runner    (1001) docker     (127)    41967 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/stored_procedure.py
--rw-r--r--   0 runner    (1001) docker     (127)    29974 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/table.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/table_function.py
--rw-r--r--   0 runner    (1001) docker     (127)    15093 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    31885 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udaf.py
--rw-r--r--   0 runner    (1001) docker     (127)    48976 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udf.py
--rw-r--r--   0 runner    (1001) docker     (127)    42468 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udtf.py
--rw-r--r--   0 runner    (1001) docker     (127)      151 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2023-09-15 20:48:03.000000 snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/window.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-15 20:48:12.415862 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    43249 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      328 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2023-09-15 20:48:12.000000 snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.508105 snowflake-snowpark-python-1.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    36522 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11365 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2023-10-16 18:52:42.508105 snowflake-snowpark-python-1.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 18:52:42.508105 snowflake-snowpark-python-1.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4408 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.500105 snowflake-snowpark-python-1.9.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.500105 snowflake-snowpark-python-1.9.0/src/snowflake/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.504105 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.504105 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.508105 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39182 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36799 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7611 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11320 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3550 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44868 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42554 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3698 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2112 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3365 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26803 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/code_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16330 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/error_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22428 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/packaging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26531 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/server_connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11337 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/telemetry.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24356 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/type_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42283 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/udf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28018 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16568 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/async_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34332 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/column.py
+-rw-r--r--   0 runner    (1001) docker     (127)      550 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)   158150 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23472 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_na_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31616 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11159 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_stat_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15570 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6357 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17528 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/file_operation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8301 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)   304476 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18102 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/relational_grouped_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12095 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/row.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119546 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/session.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41967 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/stored_procedure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29974 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/table.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/table_function.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15093 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31885 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udaf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    48976 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42468 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udtf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2023-10-16 18:52:30.000000 snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/window.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 18:52:42.508105 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    44029 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2023-10-16 18:52:42.000000 snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/top_level.txt
```

### Comparing `snowflake-snowpark-python-1.8.0/CHANGELOG.md` & `snowflake-snowpark-python-1.9.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,27 @@
 # Release History
 
+## 1.9.0 (2023-10-13)
+
+### New Features
+
+- Added support for the Python 3.11 runtime environment.
+
+### Dependency updates
+
+- Added back the dependency of `typing-extensions`.
+
+### Bug Fixes
+
+- Fixed a bug where imports from permanent stage locations were ignored for temporary stored procedures, UDTFs, UDFs, and UDAFs.
+- Revert back to using CTAS (create table as select) statement for `Dataframe.writer.save_as_table` which does not need insert permission for writing tables.
+
+### New Features
+- Support `PythonObjJSONEncoder` json-serializable objects for `ARRAY` and `OBJECT` literals.
+
 ## 1.8.0 (2023-09-14)
 
 ### New Features
 
 - Added support for VOLATILE/IMMUTABLE keyword when registering UDFs.
 - Added support for specifying clustering keys when saving dataframes using `DataFrame.save_as_table`.
 - Accept `Iterable` objects input for `schema` when creating dataframes using `Session.create_dataframe`.
```

### Comparing `snowflake-snowpark-python-1.8.0/LICENSE.txt` & `snowflake-snowpark-python-1.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/PKG-INFO` & `snowflake-snowpark-python-1.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -21,28 +21,31 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: setuptools>=40.6.0
 Requires-Dist: wheel
 Requires-Dist: snowflake-connector-python<4.0.0,>=3.2.0
+Requires-Dist: typing-extensions<5.0.0,>=4.1.0
 Requires-Dist: pyyaml
-Requires-Dist: cloudpickle<=2.0.0,>=1.6.0
+Requires-Dist: cloudpickle<=2.0.0,>=1.6.0; python_version < "3.11"
+Requires-Dist: cloudpickle==2.2.1; python_version ~= "3.11"
 Provides-Extra: pandas
 Requires-Dist: snowflake-connector-python[pandas]<4.0.0,>=3.2.0; extra == "pandas"
 Provides-Extra: secure-local-storage
 Requires-Dist: snowflake-connector-python[secure-local-storage]<4.0.0,>=3.2.0; extra == "secure-local-storage"
 Provides-Extra: development
 Requires-Dist: pytest; extra == "development"
 Requires-Dist: pytest-cov; extra == "development"
@@ -67,15 +70,15 @@
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
 You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8, 3.9 or 3.10 virtual environment.
+to create a Python 3.8, 3.9, 3.10 or 3.11 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
@@ -145,14 +148,32 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
+## 1.9.0 (2023-10-13)
+
+### New Features
+
+- Added support for the Python 3.11 runtime environment.
+
+### Dependency updates
+
+- Added back the dependency of `typing-extensions`.
+
+### Bug Fixes
+
+- Fixed a bug where imports from permanent stage locations were ignored for temporary stored procedures, UDTFs, UDFs, and UDAFs.
+- Revert back to using CTAS (create table as select) statement for `Dataframe.writer.save_as_table` which does not need insert permission for writing tables.
+
+### New Features
+- Support `PythonObjJSONEncoder` json-serializable objects for `ARRAY` and `OBJECT` literals.
+
 ## 1.8.0 (2023-09-14)
 
 ### New Features
 
 - Added support for VOLATILE/IMMUTABLE keyword when registering UDFs.
 - Added support for specifying clustering keys when saving dataframes using `DataFrame.save_as_table`.
 - Accept `Iterable` objects input for `schema` when creating dataframes using `Session.create_dataframe`.
```

### Comparing `snowflake-snowpark-python-1.8.0/README.md` & `snowflake-snowpark-python-1.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
 You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8, 3.9 or 3.10 virtual environment.
+to create a Python 3.8, 3.9, 3.10 or 3.11 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
```

### Comparing `snowflake-snowpark-python-1.8.0/setup.py` & `snowflake-snowpark-python-1.9.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -11,32 +11,26 @@
 SRC_DIR = os.path.join(THIS_DIR, "src")
 SNOWPARK_SRC_DIR = os.path.join(SRC_DIR, "snowflake", "snowpark")
 CONNECTOR_DEPENDENCY_VERSION = ">=3.2.0, <4.0.0"
 INSTALL_REQ_LIST = [
     "setuptools>=40.6.0",
     "wheel",
     f"snowflake-connector-python{CONNECTOR_DEPENDENCY_VERSION}",
+    # snowpark directly depends on typing-extension, so we should not remove it even if connector also depends on it.
+    "typing-extensions>=4.1.0, <5.0.0",
     "pyyaml",
 ]
-CLOUDPICKLE_REQ_LIST = ["cloudpickle>=1.6.0,<=2.0.0"]
-REQUIRED_PYTHON_VERSION = ">=3.8, <3.11"
+CLOUDPICKLE_REQ_LIST = [
+    "cloudpickle>=1.6.0,<=2.0.0;python_version<'3.11'",
+    "cloudpickle==2.2.1;python_version~='3.11'",  # backend only supports cloudpickle 2.2.1 + python 3.11 at the moment
+]
+REQUIRED_PYTHON_VERSION = ">=3.8, <3.12"
 
 if os.getenv("SNOWFLAKE_IS_PYTHON_RUNTIME_TEST", False):
-    # this allows us to update the cloudpickle dependency by env var when building package privately
-    # without re-releasing package just to update the dependency, example if we want to lower cloudpickle dep to 2.1.0:
-    # SNOWFLAKE_IS_PYTHON_RUNTIME_TEST=1 CLOUDPICKLE_PYTHON_311_DEPENDENCY="cloudpickle==2.1.0;python_version~='3.11'" pip install .
-    CLOUDPICKLE_PYTHON_311_DEPENDENCY = os.getenv(
-        "CLOUDPICKLE_PYTHON_311_DEPENDENCY",
-        "cloudpickle==2.2.1;python_version~='3.11'",
-    )
     REQUIRED_PYTHON_VERSION = ">=3.8"
-    CLOUDPICKLE_REQ_LIST = [
-        "cloudpickle>=1.6.0,<=2.0.0;python_version<'3.11'",
-        CLOUDPICKLE_PYTHON_311_DEPENDENCY,
-    ]
 
 INSTALL_REQ_LIST.extend(CLOUDPICKLE_REQ_LIST)
 
 # read the version
 VERSION = ()
 with open(os.path.join(SNOWPARK_SRC_DIR, "version.py"), encoding="utf-8") as f:
     exec(f.read())
@@ -108,14 +102,15 @@
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
         "Programming Language :: SQL",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Database",
         "Topic :: Software Development",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Application Frameworks",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Scientific/Engineering :: Information Analysis",
     ],
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/__init__.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/__init__.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/analyzer_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -711,22 +711,30 @@
         f"{COMMA.join([QUESTION_MARK] * len(column_names))}{RIGHT_PARENTHESIS}"
     )
 
 
 def create_table_as_select_statement(
     table_name: str,
     child: str,
+    column_definition: str,
     replace: bool = False,
     error: bool = True,
     table_type: str = EMPTY_STRING,
+    clustering_key: Optional[Iterable[str]] = None,
 ) -> str:
+    cluster_by_clause = (
+        (CLUSTER_BY + LEFT_PARENTHESIS + COMMA.join(clustering_key) + RIGHT_PARENTHESIS)
+        if clustering_key
+        else EMPTY_STRING
+    )
     return (
         f"{CREATE}{OR + REPLACE if replace else EMPTY_STRING} {table_type.upper()} {TABLE}"
         f"{IF + NOT + EXISTS if not replace and not error else EMPTY_STRING}"
-        f" {table_name}{AS}{project_statement([], child)}"
+        f" {table_name}{LEFT_PARENTHESIS}{column_definition}{RIGHT_PARENTHESIS}"
+        f"{cluster_by_clause} {AS}{project_statement([], child)}"
     )
 
 
 def limit_statement(
     row_count: str, offset: str, child: str, on_top_of_order_by: bool
 ) -> str:
     return (
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/binary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/binary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/datatype_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from array import array
 from datetime import date, datetime, time, timedelta, timezone
 from decimal import Decimal
 from typing import Any
 
 import snowflake.snowpark._internal.analyzer.analyzer_utils as analyzer_utils
 from snowflake.snowpark._internal.type_utils import convert_sp_to_sf_type
+from snowflake.snowpark._internal.utils import PythonObjJSONEncoder
 from snowflake.snowpark.types import (
     ArrayType,
     BinaryType,
     BooleanType,
     DataType,
     DateType,
     DecimalType,
@@ -65,14 +66,17 @@
             return "NULL :: FLOAT"
     if isinstance(datatype, StringType):
         if value is None:
             return f"NULL :: {analyzer_utils.string(datatype.length)}"
     if isinstance(datatype, BooleanType):
         if value is None:
             return "NULL :: BOOLEAN"
+    if isinstance(datatype, VariantType):
+        if value is None:
+            return "NULL :: VARIANT"
     if value is None:
         return "NULL"
 
     # Not nulls
     if isinstance(value, str) and isinstance(datatype, StringType):
         # If this is used in a values statement (e.g., create_dataframe),
         # the sql value has to be casted to make sure the varchar length
@@ -132,18 +136,22 @@
             trimmed_ms = value.strftime("%H:%M:%S.%f")[:-3]
             return f"TIME('{trimmed_ms}')"
 
     if isinstance(value, (list, bytes, bytearray)) and isinstance(datatype, BinaryType):
         return f"'{binascii.hexlify(value).decode()}' :: BINARY"
 
     if isinstance(value, (list, tuple, array)) and isinstance(datatype, ArrayType):
-        return f"PARSE_JSON({str_to_sql(json.dumps(value))}) :: ARRAY"
+        return f"PARSE_JSON({str_to_sql(json.dumps(value, cls=PythonObjJSONEncoder))}) :: ARRAY"
 
     if isinstance(value, dict) and isinstance(datatype, MapType):
-        return f"PARSE_JSON({str_to_sql(json.dumps(value))}) :: OBJECT"
+        return f"PARSE_JSON({str_to_sql(json.dumps(value, cls=PythonObjJSONEncoder))}) :: OBJECT"
+
+    if isinstance(datatype, VariantType):
+        # PARSE_JSON returns VARIANT, so no need to append :: VARIANT here explicitly.
+        return f"PARSE_JSON({str_to_sql(json.dumps(value, cls=PythonObjJSONEncoder))})"
 
     raise TypeError(f"Unsupported datatype {datatype}, value {value} by to_sql()")
 
 
 def schema_expression(data_type: DataType, is_nullable: bool) -> str:
     if is_nullable:
         if isinstance(data_type, GeographyType):
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/grouping_set.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/schema_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/select_statement.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -559,19 +559,20 @@
         column_names: Optional[Iterable[str]],
         mode: SaveMode,
         table_type: str,
         clustering_keys: Iterable[str],
         child: SnowflakePlan,
     ) -> SnowflakePlan:
         full_table_name = ".".join(table_name)
+        column_definition = attribute_to_schema_string(child.attributes)
 
         def get_create_and_insert_plan(child: SnowflakePlan, replace=False, error=True):
             create_table = create_table_statement(
                 full_table_name,
-                attribute_to_schema_string(child.attributes),
+                column_definition,
                 replace=replace,
                 error=error,
                 table_type=table_type,
                 clustering_key=clustering_keys,
             )
 
             # so that dataframes created from non-select statements,
@@ -608,28 +609,51 @@
                     ),
                     child,
                     None,
                 )
             else:
                 return get_create_and_insert_plan(child, replace=False, error=False)
         elif mode == SaveMode.OVERWRITE:
-            return get_create_and_insert_plan(child, replace=True)
+            return self.build(
+                lambda x: create_table_as_select_statement(
+                    full_table_name,
+                    x,
+                    column_definition,
+                    replace=True,
+                    table_type=table_type,
+                    clustering_key=clustering_keys,
+                ),
+                child,
+                None,
+            )
         elif mode == SaveMode.IGNORE:
-            if self.session._table_exists(table_name):
-                return self.build(
-                    lambda x: create_table_as_select_statement(
-                        full_table_name, x, error=False, table_type=table_type
-                    ),
-                    child,
-                    None,
-                )
-            else:
-                return get_create_and_insert_plan(child, replace=False, error=False)
+            return self.build(
+                lambda x: create_table_as_select_statement(
+                    full_table_name,
+                    x,
+                    column_definition,
+                    error=False,
+                    table_type=table_type,
+                    clustering_key=clustering_keys,
+                ),
+                child,
+                None,
+            )
         elif mode == SaveMode.ERROR_IF_EXISTS:
-            return get_create_and_insert_plan(child, replace=False, error=True)
+            return self.build(
+                lambda x: create_table_as_select_statement(
+                    full_table_name,
+                    x,
+                    column_definition,
+                    table_type=table_type,
+                    clustering_key=clustering_keys,
+                ),
+                child,
+                None,
+            )
 
     def limit(
         self,
         limit_expr: str,
         offset_expr: str,
         child: SnowflakePlan,
         on_top_of_oder_by: bool,
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/snowflake_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/sort_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/table_function.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/table_merge_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/unary_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/unary_plan_node.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/analyzer/window_expression.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/code_generation.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/code_generation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/error_message.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/error_message.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/packaging_utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/packaging_utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/server_connection.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/server_connection.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/telemetry.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/telemetry.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/type_utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/type_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -219,14 +219,15 @@
     dict,
 )
 VALID_SNOWPARK_TYPES_FOR_LITERAL_VALUE = (
     *PYTHON_TO_SNOW_TYPE_MAPPINGS.values(),
     _NumericType,
     ArrayType,
     MapType,
+    VariantType,
 )
 
 # Mapping Python array types to DataType
 ARRAY_SIGNED_INT_TYPECODE_CTYPE_MAPPINGS = {
     "b": ctypes.c_byte,
     "h": ctypes.c_short,
     "i": ctypes.c_int,
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/udf_utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/udf_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -345,19 +345,14 @@
             raise ValueError(
                 f"name must be specified for permanent {get_error_message_abbr(object_type)}"
             )
         if not stage_location:
             raise ValueError(
                 f"stage_location must be specified for permanent {get_error_message_abbr(object_type)}"
             )
-    else:
-        if stage_location:
-            logger.warn(
-                "is_permanent is False therefore stage_location will be ignored"
-            )
 
     if parallel < 1 or parallel > 99:
         raise ValueError(
             "Supported values of parallel are from 1 to 99, " f"but got {parallel}"
         )
 
 
@@ -811,20 +806,24 @@
     max_batch_size: Optional[int] = None,
     *,
     statement_params: Optional[Dict[str, str]] = None,
     source_code_display: bool = False,
     skip_upload_on_content_match: bool = False,
     is_permanent: bool = False,
 ) -> Tuple[str, str, str, str, str, bool]:
-    upload_stage = (
+    import_only_stage = (
         unwrap_stage_location_single_quote(stage_location)
-        if stage_location and is_permanent
+        if stage_location
         else session.get_session_stage()
     )
 
+    upload_and_import_stage = (
+        import_only_stage if is_permanent else session.get_session_stage()
+    )
+
     # resolve packages
     resolved_packages = (
         session._resolve_packages(packages, include_pandas=is_pandas_udf)
         if packages is not None
         else session._resolve_packages(
             [],
             session._packages,
@@ -846,19 +845,24 @@
             else:
                 raise TypeError(
                     f"{get_error_message_abbr(object_type).replace(' ', '-')}-level import can only be a file path (str) "
                     "or a tuple of the file path (str) and the import path (str)."
                 )
             udf_level_imports[resolved_import_tuple[0]] = resolved_import_tuple[1:]
         all_urls = session._resolve_imports(
-            upload_stage, udf_level_imports, statement_params=statement_params
+            import_only_stage,
+            upload_and_import_stage,
+            udf_level_imports,
+            statement_params=statement_params,
         )
     elif imports is None:
         all_urls = session._resolve_imports(
-            upload_stage, statement_params=statement_params
+            import_only_stage,
+            upload_and_import_stage,
+            statement_params=statement_params,
         )
     else:
         all_urls = []
 
     dest_prefix = get_udf_upload_prefix(udf_name)
 
     # Upload closure to stage if it is beyond inline closure size limit
@@ -879,25 +883,25 @@
             is_dataframe_input,
             max_batch_size,
             source_code_display=source_code_display,
         )
         if len(code) > _MAX_INLINE_CLOSURE_SIZE_BYTES:
             dest_prefix = get_udf_upload_prefix(udf_name)
             upload_file_stage_location = normalize_remote_file_or_dir(
-                f"{upload_stage}/{dest_prefix}/{udf_file_name}"
+                f"{upload_and_import_stage}/{dest_prefix}/{udf_file_name}"
             )
             udf_file_name_base = os.path.splitext(udf_file_name)[0]
             with io.BytesIO() as input_stream:
                 with zipfile.ZipFile(
                     input_stream, mode="w", compression=zipfile.ZIP_DEFLATED
                 ) as zf:
                     zf.writestr(f"{udf_file_name_base}.py", code)
                 session._conn.upload_stream(
                     input_stream=input_stream,
-                    stage_location=upload_stage,
+                    stage_location=upload_and_import_stage,
                     dest_filename=udf_file_name,
                     dest_prefix=dest_prefix,
                     parallel=parallel,
                     source_compression="DEFLATE",
                     compress_data=False,
                     overwrite=True,
                     is_in_udf=True,
@@ -920,19 +924,19 @@
         handler = f"{udf_file_name_base}.{func[1]}"
 
         if func[0].startswith(STAGE_PREFIX):
             upload_file_stage_location = None
             all_urls.append(func[0])
         else:
             upload_file_stage_location = normalize_remote_file_or_dir(
-                f"{upload_stage}/{dest_prefix}/{udf_file_name}"
+                f"{upload_and_import_stage}/{dest_prefix}/{udf_file_name}"
             )
             session._conn.upload_file(
                 path=func[0],
-                stage_location=upload_stage,
+                stage_location=upload_and_import_stage,
                 dest_prefix=dest_prefix,
                 parallel=parallel,
                 compress_data=False,
                 overwrite=True,
                 skip_upload_on_content_match=skip_upload_on_content_match,
             )
             all_urls.append(upload_file_stage_location)
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/_internal/utils.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/_internal/utils.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/async_job.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/async_job.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/column.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/column.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/context.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/context.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_na_functions.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_na_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_reader.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_reader.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_stat_functions.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_stat_functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/dataframe_writer.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/dataframe_writer.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/exceptions.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/exceptions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/file_operation.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/file_operation.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/files.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/files.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/functions.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/functions.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/query_history.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/query_history.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/relational_grouped_dataframe.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/relational_grouped_dataframe.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/row.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/row.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/session.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/session.py`

 * *Files 1% similar despite different names*

```diff
@@ -681,27 +681,34 @@
                 leading_path,
             )
         else:
             return trimmed_path, None, None
 
     def _resolve_imports(
         self,
-        stage_location: str,
+        import_only_stage: str,
+        upload_and_import_stage: str,
         udf_level_import_paths: Optional[
             Dict[str, Tuple[Optional[str], Optional[str]]]
         ] = None,
         *,
         statement_params: Optional[Dict[str, str]] = None,
     ) -> List[str]:
         """Resolve the imports and upload local files (if any) to the stage."""
         resolved_stage_files = []
         stage_file_list = self._list_files_in_stage(
-            stage_location, statement_params=statement_params
+            import_only_stage, statement_params=statement_params
+        )
+
+        normalized_import_only_location = unwrap_stage_location_single_quote(
+            import_only_stage
+        )
+        normalized_upload_and_import_location = unwrap_stage_location_single_quote(
+            upload_and_import_stage
         )
-        normalized_stage_location = unwrap_stage_location_single_quote(stage_location)
 
         import_paths = udf_level_import_paths or self._import_paths
         for path, (prefix, leading_path) in import_paths.items():
             # stage file
             if path.startswith(STAGE_PREFIX):
                 resolved_stage_files.append(path)
             else:
@@ -709,48 +716,53 @@
                     f"{os.path.basename(path)}.zip"
                     if os.path.isdir(path) or path.endswith(".py")
                     else os.path.basename(path)
                 )
                 filename_with_prefix = f"{prefix}/{filename}"
                 if filename_with_prefix in stage_file_list:
                     _logger.debug(
-                        f"{filename} exists on {normalized_stage_location}, skipped"
+                        f"{filename} exists on {normalized_import_only_location}, skipped"
+                    )
+                    resolved_stage_files.append(
+                        normalize_remote_file_or_dir(
+                            f"{normalized_import_only_location}/{filename_with_prefix}"
+                        )
                     )
                 else:
                     # local directory or .py file
                     if os.path.isdir(path) or path.endswith(".py"):
                         with zip_file_or_directory_to_stream(
                             path, leading_path
                         ) as input_stream:
                             self._conn.upload_stream(
                                 input_stream=input_stream,
-                                stage_location=normalized_stage_location,
+                                stage_location=normalized_upload_and_import_location,
                                 dest_filename=filename,
                                 dest_prefix=prefix,
                                 source_compression="DEFLATE",
                                 compress_data=False,
                                 overwrite=True,
                                 is_in_udf=True,
                                 skip_upload_on_content_match=True,
                             )
                     # local file
                     else:
                         self._conn.upload_file(
                             path=path,
-                            stage_location=normalized_stage_location,
+                            stage_location=normalized_upload_and_import_location,
                             dest_prefix=prefix,
                             compress_data=False,
                             overwrite=True,
                             skip_upload_on_content_match=True,
                         )
-                resolved_stage_files.append(
-                    normalize_remote_file_or_dir(
-                        f"{normalized_stage_location}/{filename_with_prefix}"
+                    resolved_stage_files.append(
+                        normalize_remote_file_or_dir(
+                            f"{normalized_upload_and_import_location}/{filename_with_prefix}"
+                        )
                     )
-                )
 
         return resolved_stage_files
 
     def _list_files_in_stage(
         self,
         stage_location: Optional[str] = None,
         *,
@@ -806,15 +818,15 @@
             >>> from snowflake.snowpark.functions import udf
             >>> import numpy
             >>> import pandas
             >>> import dateutil
             >>> # add numpy with the latest version on Snowflake Anaconda
             >>> # and pandas with the version "1.3.*"
             >>> # and dateutil with the local version in your environment
-            >>> session.add_packages("numpy", "pandas==1.4.*", dateutil)
+            >>> session.add_packages("numpy", "pandas==1.5.*", dateutil)
             >>> @udf
             ... def get_package_name_udf() -> list:
             ...     return [numpy.__name__, pandas.__name__, dateutil.__name__]
             >>> session.sql(f"select {get_package_name_udf.name}()").to_df("col1").show()
             ----------------
             |"COL1"        |
             ----------------
@@ -1163,21 +1175,32 @@
 
         # Add dependency packages
         if dependency_packages:
             for package in dependency_packages:
                 name = package.name
                 version = package.specs[0][1] if package.specs else None
 
+                # result_dict is a mapping of package name -> package_spec, example
+                # {'pyyaml': 'pyyaml==6.0',
+                #  'networkx': 'networkx==3.1',
+                #  'numpy': 'numpy',
+                #  'scikit-learn': 'scikit-learn==1.2.2',
+                #  'python-dateutil': 'python-dateutil==2.8.2'}
                 # Add to packages dictionary
                 if name in result_dict:
-                    if version is not None and result_dict[name] != str(package):
-                        raise ValueError(
-                            f"Cannot add dependency package '{name}=={version}' "
-                            f"because {result_dict[name]} is already added."
-                        )
+                    if version is not None:
+                        added_package_has_version = "==" in result_dict[name]
+                        if added_package_has_version and result_dict[name] != str(
+                            package
+                        ):
+                            raise ValueError(
+                                f"Cannot add dependency package '{name}=={version}' "
+                                f"because {result_dict[name]} is already added."
+                            )
+                        result_dict[name] = str(package)
                 else:
                     result_dict[name] = str(package)
 
         # Always include cloudpickle
         extra_modules = [cloudpickle]
         if include_pandas:
             extra_modules.append("pandas")
@@ -1703,15 +1726,14 @@
 
     @property
     def connection(self) -> "SnowflakeConnection":
         """Returns a :class:`SnowflakeConnection` object that allows you to access the connection between the current session
         and Snowflake server."""
         return self._conn._conn
 
-
     def _run_query(
         self,
         query: str,
         is_ddl_on_temp_object: bool = False,
         log_on_exception: bool = True,
     ) -> List[Any]:
         return self._conn.run_query(
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/stored_procedure.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/stored_procedure.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/table.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/table.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/table_function.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/table_function.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/types.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/types.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udaf.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udaf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udf.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/udtf.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/udtf.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake/snowpark/window.py` & `snowflake-snowpark-python-1.9.0/src/snowflake/snowpark/window.py`

 * *Files identical despite different names*

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/PKG-INFO` & `snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snowflake-snowpark-python
-Version: 1.8.0
+Version: 1.9.0
 Summary: Snowflake Snowpark for Python
 Home-page: https://www.snowflake.com/
 Author: Snowflake, Inc
 Author-email: snowflake-python-libraries-dl@snowflake.com
 License: Apache License, Version 2.0
 Project-URL: Documentation, https://docs.snowflake.com/en/developer-guide/snowpark/python/index.html
 Project-URL: Source, https://github.com/snowflakedb/snowpark-python
@@ -21,28 +21,31 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: SQL
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Requires-Python: >=3.8, <3.11
+Requires-Python: >=3.8, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: setuptools>=40.6.0
 Requires-Dist: wheel
 Requires-Dist: snowflake-connector-python<4.0.0,>=3.2.0
+Requires-Dist: typing-extensions<5.0.0,>=4.1.0
 Requires-Dist: pyyaml
-Requires-Dist: cloudpickle<=2.0.0,>=1.6.0
+Requires-Dist: cloudpickle<=2.0.0,>=1.6.0; python_version < "3.11"
+Requires-Dist: cloudpickle==2.2.1; python_version ~= "3.11"
 Provides-Extra: pandas
 Requires-Dist: snowflake-connector-python[pandas]<4.0.0,>=3.2.0; extra == "pandas"
 Provides-Extra: secure-local-storage
 Requires-Dist: snowflake-connector-python[secure-local-storage]<4.0.0,>=3.2.0; extra == "secure-local-storage"
 Provides-Extra: development
 Requires-Dist: pytest; extra == "development"
 Requires-Dist: pytest-cov; extra == "development"
@@ -67,15 +70,15 @@
 ## Getting started
 
 ### Have your Snowflake account ready
 If you don't have a Snowflake account yet, you can [sign up for a 30-day free trial account][sign up trial].
 
 ### Create a Python virtual environment
 You can use [miniconda][miniconda], [anaconda][anaconda], or [virtualenv][virtualenv]
-to create a Python 3.8, 3.9 or 3.10 virtual environment.
+to create a Python 3.8, 3.9, 3.10 or 3.11 virtual environment.
 
 To have the best experience when using it with UDFs, [creating a local conda environment with the Snowflake channel][use snowflake channel] is recommended.
 
 ### Install the library to the Python virtual environment
 ```bash
 pip install snowflake-snowpark-python
 ```
@@ -145,14 +148,32 @@
 [snowflake lab sample code]: https://github.com/Snowflake-Labs/snowpark-python-demos
 [samples]: https://github.com/snowflakedb/snowpark-python/blob/main/README.md#samples
 [contributing]: https://github.com/snowflakedb/snowpark-python/blob/main/CONTRIBUTING.md
 
 
 # Release History
 
+## 1.9.0 (2023-10-13)
+
+### New Features
+
+- Added support for the Python 3.11 runtime environment.
+
+### Dependency updates
+
+- Added back the dependency of `typing-extensions`.
+
+### Bug Fixes
+
+- Fixed a bug where imports from permanent stage locations were ignored for temporary stored procedures, UDTFs, UDFs, and UDAFs.
+- Revert back to using CTAS (create table as select) statement for `Dataframe.writer.save_as_table` which does not need insert permission for writing tables.
+
+### New Features
+- Support `PythonObjJSONEncoder` json-serializable objects for `ARRAY` and `OBJECT` literals.
+
 ## 1.8.0 (2023-09-14)
 
 ### New Features
 
 - Added support for VOLATILE/IMMUTABLE keyword when registering UDFs.
 - Added support for specifying clustering keys when saving dataframes using `DataFrame.save_as_table`.
 - Accept `Iterable` objects input for `schema` when creating dataframes using `Session.create_dataframe`.
```

### Comparing `snowflake-snowpark-python-1.8.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt` & `snowflake-snowpark-python-1.9.0/src/snowflake_snowpark_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

