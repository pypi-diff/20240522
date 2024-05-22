# Comparing `tmp/asqlorm-0.7.1.tar.gz` & `tmp/asqlorm-0.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.7.1.tar", max compression
+gzip compressed data, was "asqlorm-0.7.2.tar", max compression
```

## Comparing `asqlorm-0.7.1.tar` & `asqlorm-0.7.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.7.1/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.7.1/asqlorm/__init__.py
--rw-r--r--   0        0        0    32021 2024-05-22 20:45:31.616947 asqlorm-0.7.1/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44933 2024-05-22 20:37:43.023429 asqlorm-0.7.1/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.7.1/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.7.1/asqlorm/utils.py
--rw-r--r--   0        0        0      649 2024-05-22 20:46:57.678304 asqlorm-0.7.1/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.7.2/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.7.2/asqlorm/__init__.py
+-rw-r--r--   0        0        0    32025 2024-05-22 20:59:52.032063 asqlorm-0.7.2/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44933 2024-05-22 20:37:43.023429 asqlorm-0.7.2/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.7.2/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.7.2/asqlorm/utils.py
+-rw-r--r--   0        0        0      649 2024-05-22 20:59:59.358106 asqlorm-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.7.2/PKG-INFO
```

### Comparing `asqlorm-0.7.1/asqlorm/generator/main.py` & `asqlorm-0.7.2/asqlorm/generator/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -552,15 +552,15 @@
                         [f"{n}={n}" for n in link.annotations_by_kwarg.keys()]
                     )
                 else:
                     names_str = ""
                 update_qb_str = f"self._node.__computed_links__['{link_name}'].update_qb(self._qb{names_str})"
             resolver_func_strs.append(
                 f"""
-    def {link_name}(self, resolver: T.Optional["{link_table.node_name}"] = None, key: str = "{link_name}"{kwargs_str}) -> "{table.node_name}":
+    def {link_name}(self, resolver: T.Optional["{link_table.resolver_name}"] = None, key: str = "{link_name}"{kwargs_str}) -> "{table.node_name}":
         self.add_child(
             key=key,
             resolver = resolver or {link_table.resolver_name}(),
             cardinality={'Cardinality.ONE' if link.cardinality == Cardinality.ONE else 'Cardinality.MANY'},
             from_=\"\"\"{link.from_}\"\"\",
             is_required={'False' if link.is_nullable else 'True'}
         )
```

### Comparing `asqlorm-0.7.1/asqlorm/models.py` & `asqlorm-0.7.2/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.1/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.7.2/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.1/asqlorm/utils.py` & `asqlorm-0.7.2/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.7.1/pyproject.toml` & `asqlorm-0.7.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.7.1"
+version = "0.7.2"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.7.1/PKG-INFO` & `asqlorm-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.7.1
+Version: 0.7.2
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

