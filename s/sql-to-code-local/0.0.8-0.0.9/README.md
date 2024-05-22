# Comparing `tmp/sql-to-code-local-0.0.8.tar.gz` & `tmp/sql-to-code-local-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sql-to-code-local-0.0.8.tar", last modified: Sun Jan  7 10:42:08 2024, max compression
+gzip compressed data, was "sql-to-code-local-0.0.9.tar", last modified: Sun Jan  7 11:32:05 2024, max compression
```

## Comparing `sql-to-code-local-0.0.8.tar` & `sql-to-code-local-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-07 10:41:41.000000 sql-to-code-local-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-07 10:41:41.000000 sql-to-code-local-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-01-07 10:41:41.000000 sql-to-code-local-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/sql_to_code/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/sql_to_code/src/
--rw-r--r--   0 runner    (1001) docker     (127)     6271 2024-01-07 10:41:41.000000 sql-to-code-local-0.0.8/sql_to_code/src/sqltocode.py
--rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-01-07 10:41:41.000000 sql-to-code-local-0.0.8/sql_to_code/src/table_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 10:42:08.326298 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-07 10:42:08.000000 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-01-07 10:42:08.000000 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 10:42:08.000000 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-07 10:42:08.000000 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-07 10:42:08.000000 sql-to-code-local-0.0.8/sql_to_code_local.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:32:05.177157 sql-to-code-local-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-07 11:32:05.177157 sql-to-code-local-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-01-07 11:31:42.000000 sql-to-code-local-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-01-07 11:31:42.000000 sql-to-code-local-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-07 11:32:05.177157 sql-to-code-local-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1377 2024-01-07 11:31:42.000000 sql-to-code-local-0.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:32:05.169157 sql-to-code-local-0.0.9/sql_to_code_local/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:32:05.177157 sql-to-code-local-0.0.9/sql_to_code_local/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-01-07 11:31:42.000000 sql-to-code-local-0.0.9/sql_to_code_local/src/sqltocode.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13880 2024-01-07 11:31:42.000000 sql-to-code-local-0.0.9/sql_to_code_local/src/table_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-07 11:32:05.177157 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-01-07 11:32:05.000000 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-01-07 11:32:05.000000 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-07 11:32:05.000000 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-01-07 11:32:05.000000 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-01-07 11:32:05.000000 sql-to-code-local-0.0.9/sql_to_code_local.egg-info/top_level.txt
```

### Comparing `sql-to-code-local-0.0.8/PKG-INFO` & `sql-to-code-local-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-to-code-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles sql-to-code-local Local Python
 Home-page: https://github.com/circ-zone/sql2code-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

### Comparing `sql-to-code-local-0.0.8/README.md` & `sql-to-code-local-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `sql-to-code-local-0.0.8/pyproject.toml` & `sql-to-code-local-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -7,13 +7,13 @@
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [tool.poetry]
 # TODO: Please update the name, similar to storage-local (suffix -local)
 name = "sql-to-code-local"
 # I believe we are still using the version from setup.py and not from here until potery will work
-version = "0.0.8" # https://pypi.org/project/sql-to-code-local i.e. https://pypi.org/project/storage-local/
+version = "0.0.9" # https://pypi.org/project/sql-to-code-local i.e. https://pypi.org/project/storage-local/
 description = "sql-to-code-local Python Package"
 readme = "README.md"
 authors = [
     "Circlez.ai <info@circlez.ai>",
 ]
```

### Comparing `sql-to-code-local-0.0.8/setup.py` & `sql-to-code-local-0.0.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 REPO_NAME = "sql-to-code-local"
-package_dir = "sql_to_code"
+package_dir = REPO_NAME.replace("-", "_")
 
 setuptools.setup(
     name=REPO_NAME,  # https://pypi.org/project/sql-to-code-local
-    version='0.0.8',  # update each time
+    version='0.0.9',  # update each time
     author="Circles",
     author_email="info@circles.life",
     description="PyPI Package for Circles sql-to-code-local Local Python",
     long_description="PyPI Package for Circles sql-to-code-local Local Python",
     long_description_content_type='text/markdown',
     # TODO: fix the link in the following comment
     url="https://github.com/circ-zone/sql2code-local-python-package",
```

### Comparing `sql-to-code-local-0.0.8/sql_to_code/src/sqltocode.py` & `sql-to-code-local-0.0.9/sql_to_code_local/src/sqltocode.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,25 +115,26 @@
     Sql2code = SQL2Code(default_schema_name=args.schema)
     logger.info("\n---------- Success to connect MySql Circles Ai Server ---------- \n")
     if args.columns is None:
         data = Sql2code.read_table(args.table)
     else:
         data = Sql2code.read_table(args.table, args.columns.split(',') if args.columns else None)
 
-    # Write data to a .py file as a dictionary of dictionaries
-    file_name = args.table.rsplit('_', 1)[0]
-    with open(f"{args.output_path}/{file_name}.py", 'w') as f:
-        f.write(f"{file_name} = {{\n")
-        for i in range(len(data["table_name"])):
-            f.write(f"    '{data['table_name'][i]}': {{\n")
-            for key, values in data.items():
-                if key != "table_name":
-                    f.write(f"        '{key}': {repr(values[i])},\n")
-            f.write("    },\n")
-        f.write("}\n")
+    if args.language == 'Python' and args.format == 'dictionary':
+        # Write data to a .py file as a dictionary of dictionaries
+        file_name = args.table.rsplit('_', 1)[0]
+        with open(f"{args.output_path}/{file_name}.py", 'w') as f:
+            f.write(f"{file_name} = {{\n")
+            for i in range(len(data["table_name"])):
+                f.write(f"    '{data['table_name'][i]}': {{\n")
+                for key, values in data.items():
+                    if key != "table_name":
+                        f.write(f"        '{key}': {repr(values[i])},\n")
+                f.write("    },\n")
+            f.write("}\n")
     '''
     # Write data to a .py file as a class of classes
     with open(f"{args.output_path}/{args.table}.py", 'w') as f:
         # Write the wrapper class definition to the file
         f.write(f"class {args.table.upper()}:\n")
         for i in range(len(data["table_name"])):
             # Write the class definition to the file, indented under the wrapper class
```

### Comparing `sql-to-code-local-0.0.8/sql_to_code/src/table_definition.py` & `sql-to-code-local-0.0.9/sql_to_code_local/src/table_definition.py`

 * *Files identical despite different names*

### Comparing `sql-to-code-local-0.0.8/sql_to_code_local.egg-info/PKG-INFO` & `sql-to-code-local-0.0.9/sql_to_code_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sql-to-code-local
-Version: 0.0.8
+Version: 0.0.9
 Summary: PyPI Package for Circles sql-to-code-local Local Python
 Home-page: https://github.com/circ-zone/sql2code-local-python-package
 Author: Circles
 Author-email: info@circles.life
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: Other/Proprietary License
 Classifier: Operating System :: OS Independent
```

