# Comparing `tmp/asqlorm-0.6.7.tar.gz` & `tmp/asqlorm-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.7.tar", max compression
+gzip compressed data, was "asqlorm-0.6.8.tar", max compression
```

## Comparing `asqlorm-0.6.7.tar` & `asqlorm-0.6.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.7/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.7/asqlorm/__init__.py
--rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.7/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44663 2024-05-22 16:32:21.189717 asqlorm-0.6.7/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.7/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.7/asqlorm/utils.py
--rw-r--r--   0        0        0      649 2024-05-22 16:40:35.432712 asqlorm-0.6.7/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.6.7/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.8/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.8/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.8/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44933 2024-05-22 19:36:16.672251 asqlorm-0.6.8/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.8/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.8/asqlorm/utils.py
+-rw-r--r--   0        0        0      649 2024-05-22 19:36:39.640941 asqlorm-0.6.8/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.6.8/PKG-INFO
```

### Comparing `asqlorm-0.6.7/asqlorm/generator/main.py` & `asqlorm-0.6.8/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.7/asqlorm/models.py` & `asqlorm-0.6.8/asqlorm/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -912,15 +912,21 @@
             logger.debug("[REFRESH AFTER]")
             # what about composite primary keys? Or no primary keys?
             kwargs = {k: raw_val[k] for k in self._node.__primary_keys__}
             return await self._gerror(conn=conn, **kwargs)
         else:
             parsed_d: dict[str, T.Any] = {}
             for k, v in raw_val.items():
-                if k not in self._node.__computed_columns__:
+                if k in self._node.__computed_columns__:
+                    if self._node.__computed_columns__[k].override:
+                        parsed_d[k] = v
+                    else:
+                        # this is a computed field and there should have been a refresh?
+                        pass
+                else:
                     parsed_d[k] = v
             return self.parse_node(**parsed_d)
 
     async def nodes_from_raw_vals(
         self,
         raw_vals: T.Sequence[RowMapping],
         conn: AsyncConnection | None,
```

### Comparing `asqlorm-0.6.7/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.8/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.7/asqlorm/utils.py` & `asqlorm-0.6.8/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.7/pyproject.toml` & `asqlorm-0.6.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.7"
+version = "0.6.8"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.6.7/PKG-INFO` & `asqlorm-0.6.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.7
+Version: 0.6.8
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

