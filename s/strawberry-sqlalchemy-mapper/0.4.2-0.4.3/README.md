# Comparing `tmp/strawberry_sqlalchemy_mapper-0.4.2.tar.gz` & `tmp/strawberry_sqlalchemy_mapper-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "strawberry_sqlalchemy_mapper-0.4.2.tar", max compression
+gzip compressed data, was "strawberry_sqlalchemy_mapper-0.4.3.tar", max compression
```

## Comparing `strawberry_sqlalchemy_mapper-0.4.2.tar` & `strawberry_sqlalchemy_mapper-0.4.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1076 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/LICENSE.txt
--rw-r--r--   0        0        0     6485 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/README.md
--rw-r--r--   0        0        0     5570 2023-12-29 21:02:03.727076 strawberry_sqlalchemy_mapper-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      883 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/__init__.py
--rw-r--r--   0        0        0     1225 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/exc.py
--rw-r--r--   0        0        0    24255 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/field.py
--rw-r--r--   0        0        0     3355 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/loader.py
--rw-r--r--   0        0        0    35816 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/mapper.py
--rw-r--r--   0        0        0        0 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/ordering.py
--rw-r--r--   0        0        0        0 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/py.typed
--rw-r--r--   0        0        0    11660 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/relay.py
--rw-r--r--   0        0        0      210 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/scalars.py
--rw-r--r--   0        0        0      464 2023-12-29 21:01:44.935042 strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/utils.py
--rw-r--r--   0        0        0     8207 1970-01-01 00:00:00.000000 strawberry_sqlalchemy_mapper-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0       71 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/AUTHORS.rst
+-rw-r--r--   0        0        0     1076 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/LICENSE.txt
+-rw-r--r--   0        0        0     6485 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/README.md
+-rw-r--r--   0        0        0     5570 2024-05-22 14:26:13.007474 strawberry_sqlalchemy_mapper-0.4.3/pyproject.toml
+-rw-r--r--   0        0        0      883 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/__init__.py
+-rw-r--r--   0        0        0     1225 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/exc.py
+-rw-r--r--   0        0        0    24255 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/field.py
+-rw-r--r--   0        0        0     3355 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/loader.py
+-rw-r--r--   0        0        0    36291 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/mapper.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/ordering.py
+-rw-r--r--   0        0        0        0 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/py.typed
+-rw-r--r--   0        0        0    11660 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/relay.py
+-rw-r--r--   0        0        0      210 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/scalars.py
+-rw-r--r--   0        0        0      464 2024-05-22 14:25:55.251422 strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/utils.py
+-rw-r--r--   0        0        0     8207 1970-01-01 00:00:00.000000 strawberry_sqlalchemy_mapper-0.4.3/PKG-INFO
```

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/LICENSE.txt` & `strawberry_sqlalchemy_mapper-0.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/README.md` & `strawberry_sqlalchemy_mapper-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/pyproject.toml` & `strawberry_sqlalchemy_mapper-0.4.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "strawberry-sqlalchemy-mapper"
 packages = [ { include = "strawberry_sqlalchemy_mapper", from = "src" } ]
-version = "0.4.2"
+version = "0.4.3"
 description = "A library for autogenerating Strawberry GraphQL types from SQLAlchemy models."
 authors = ["Tim Dumol <tim@timdumol.com>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["graphql", "sqlalchemy", "strawberry"]
 
 homepage = "https://strawberry.rocks/"
```

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/__init__.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/exc.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/exc.py`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/field.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/field.py`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/loader.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/loader.py`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/mapper.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/mapper.py`

 * *Files 1% similar despite different names*

```diff
@@ -459,21 +459,30 @@
         Wrap a resolver that returns an array of model types to return
         a Connection instead.
         """
         connection_type = self._connection_type_for(type_name)
         edge_type = self._edge_type_for(type_name)
 
         async def wrapper(self, info: Info):
+            # TODO: Add pagination support to dataloader resolvers
+            edges = [
+                edge_type.resolve_edge(
+                    related_object,
+                    cursor=i,
+                )
+                for i, related_object in enumerate(await resolver(self, info))
+            ]
             return connection_type(
-                edges=[
-                    edge_type(
-                        node=related_object,
-                    )
-                    for related_object in await resolver(self, info)
-                ]
+                edges=edges,
+                page_info=relay.PageInfo(
+                    has_next_page=False,
+                    has_previous_page=False,
+                    start_cursor=edges[0].cursor if edges else None,
+                    end_cursor=edges[-1].cursor if edges else None,
+                ),
             )
 
         setattr(wrapper, _IS_GENERATED_RESOLVER_KEY, True)
 
         return wrapper
 
     def relationship_resolver_for(
@@ -728,15 +737,17 @@
                     self._add_annotation(
                         type_, key, strawberry_type, generated_field_keys
                     )
                     sqlalchemy_field = cast(
                         StrawberryField,
                         field(
                             resolver=self.association_proxy_resolver_for(
-                                mapper, descriptor, strawberry_type  # type: ignore[arg-type]
+                                mapper,
+                                descriptor,
+                                strawberry_type,  # type: ignore[arg-type]
                             )
                         ),
                     )
                     assert not sqlalchemy_field.init
                     setattr(type_, key, sqlalchemy_field)
                 elif isinstance(descriptor, hybrid_property):
                     if (
```

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/src/strawberry_sqlalchemy_mapper/relay.py` & `strawberry_sqlalchemy_mapper-0.4.3/src/strawberry_sqlalchemy_mapper/relay.py`

 * *Files identical despite different names*

### Comparing `strawberry_sqlalchemy_mapper-0.4.2/PKG-INFO` & `strawberry_sqlalchemy_mapper-0.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: strawberry-sqlalchemy-mapper
-Version: 0.4.2
+Version: 0.4.3
 Summary: A library for autogenerating Strawberry GraphQL types from SQLAlchemy models.
 Home-page: https://strawberry.rocks/
 License: MIT
 Keywords: graphql,sqlalchemy,strawberry
 Author: Tim Dumol
 Author-email: tim@timdumol.com
 Requires-Python: >=3.8,<4.0
```

