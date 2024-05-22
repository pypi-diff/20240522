# Comparing `tmp/asqlorm-0.6.5.tar.gz` & `tmp/asqlorm-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.5.tar", max compression
+gzip compressed data, was "asqlorm-0.6.6.tar", max compression
```

## Comparing `asqlorm-0.6.5.tar` & `asqlorm-0.6.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.5/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.5/asqlorm/__init__.py
--rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.5/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44542 2024-04-25 00:06:52.855343 asqlorm-0.6.5/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.5/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.5/asqlorm/utils.py
--rw-r--r--   0        0        0      652 2024-05-13 21:32:47.423151 asqlorm-0.6.5/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 asqlorm-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.6/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.6/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.6/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44663 2024-05-22 16:32:21.189717 asqlorm-0.6.6/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.6/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.6/asqlorm/utils.py
+-rw-r--r--   0        0        0      652 2024-05-22 16:39:17.381231 asqlorm-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 asqlorm-0.6.6/PKG-INFO
```

### Comparing `asqlorm-0.6.5/asqlorm/generator/main.py` & `asqlorm-0.6.6/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.5/asqlorm/models.py` & `asqlorm-0.6.6/asqlorm/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -563,14 +563,16 @@
                             )
                         variables[raw_k] = raw_v
                 field_names_to_value_value = model_v.stmt
             else:
                 v = dump_v
                 if isinstance(v, dict):
                     v = json.dumps(v)
+                if isinstance(v, list):
+                    v = [json.dumps(i) if isinstance(i, dict) else i for i in v]
                 if computed_c := self._node.__computed_columns__.get(k):
                     if computed_c.basemodel_type:
                         if model_v is not None:
                             if computed_c.cardinality == Cardinality.ONE:
                                 v = model_v.model_dump_json()
                             else:
                                 v = (
```

### Comparing `asqlorm-0.6.5/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.6/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.5/asqlorm/utils.py` & `asqlorm-0.6.6/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.5/pyproject.toml` & `asqlorm-0.6.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.5"
+version = "0.6.6"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.6.5/PKG-INFO` & `asqlorm-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.5
+Version: 0.6.6
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

