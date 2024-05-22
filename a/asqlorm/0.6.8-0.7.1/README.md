# Comparing `tmp/asqlorm-0.6.8.tar.gz` & `tmp/asqlorm-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.8.tar", max compression
+gzip compressed data, was "asqlorm-0.7.1.tar", max compression
```

## Comparing `asqlorm-0.6.8.tar` & `asqlorm-0.7.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.8/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.8/asqlorm/__init__.py
--rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.8/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44933 2024-05-22 19:36:16.672251 asqlorm-0.6.8/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.8/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.8/asqlorm/utils.py
--rw-r--r--   0        0        0      649 2024-05-22 19:36:39.640941 asqlorm-0.6.8/pyproject.toml
--rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.6.8/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.7.1/asqlorm/__init__.py
+-rw-r--r--   0        0        0    32021 2024-05-22 20:45:31.616947 asqlorm-0.7.1/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44933 2024-05-22 20:37:43.023429 asqlorm-0.7.1/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.7.1/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.7.1/asqlorm/utils.py
+-rw-r--r--   0        0        0      649 2024-05-22 20:46:57.678304 asqlorm-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.7.1/PKG-INFO
```

### Comparing `asqlorm-0.6.8/asqlorm/generator/main.py` & `asqlorm-0.7.1/asqlorm/generator/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import typing as T
 import re
 from black import format_str, FileMode
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, Field, computed_field
 import psycopg
 
 from asqlorm.utils import TYPES_MAP
 from asqlorm.models import (
     Node,
     Resolver,
     ComputedColumn,
@@ -15,33 +15,24 @@
 
 
 class GeneratorError(Exception):
     pass
 
 
 class TableConfig(BaseModel):
+    node_name_override: str | None = None
+    resolver_name_override: str | None = None
+    insert_name_override: str | None = None
+    patch_name_override: str | None = None
+
     base_node: T.Type[Node] | None = None
     base_resolver: T.Type[Resolver] | None = None
     # columns_to_default_include: set[str] = Field(default_factory=set)
 
 
-class Ref(BaseModel):
-    table_name: str
-    column_name: str
-    is_nullable: bool
-
-    @classmethod
-    def from_str(cls, s: str, is_nullable: bool):
-        ref_table_name = s[: s.index("(")]
-        ref_col_name = s[s.index("(") + 1 : s.index(")")]
-        return cls(
-            table_name=ref_table_name, column_name=ref_col_name, is_nullable=is_nullable
-        )
-
-
 DEFAULT_ENUMS_QUERY: str = """
 SELECT n.nspname   AS schema_name,
        t.typname   AS enum_type,
        e.enumlabel AS enum_value
 FROM pg_type t
          JOIN
      pg_enum e ON t.oid = e.enumtypid
@@ -197,18 +188,74 @@
 
 class Table(BaseModel):
     name: str
     comment: str | None
     columns: list[Column] = Field(default_factory=list)
     constraints: str | None = None
 
+    config: TableConfig | None
+
+    @computed_field
+    def node_name(self) -> str:
+        if self.config:
+            if self.config.node_name_override:
+                return self.config.node_name_override
+            if self.config.base_node and self.config.base_node.__name__ != "Node":
+                return self.config.base_node.__name__
+        return convert_to_variable_name(self.name)
+
+    @computed_field
+    def resolver_name(self) -> str:
+        if self.config:
+            if self.config.resolver_name_override:
+                return self.config.resolver_name_override
+            if (
+                self.config.base_resolver
+                and self.config.base_resolver.__name__ != "Resolver"
+            ):
+                return self.config.base_resolver.__name__
+        return f"{self.node_name}Resolver"
+
+    @computed_field
+    def insert_name(self) -> str:
+        if self.config and self.config.insert_name_override:
+            return self.config.insert_name_override
+        return f"{self.node_name}Insert"
+
+    @computed_field
+    def patch_name(self) -> str:
+        if self.config and self.config.patch_name_override:
+            return self.config.patch_name_override
+        return f"{self.node_name}Patch"
+
     def __hash__(self):
         return hash(self.name)
 
 
+class Ref(BaseModel):
+    table_name: str
+    column_name: str
+    is_nullable: bool
+
+    table: Table
+
+    @classmethod
+    def from_str(
+        cls, s: str, is_nullable: bool, tables_by_name: dict[str, Table]
+    ) -> "Ref":
+        ref_table_name = s[: s.index("(")]
+        ref_col_name = s[s.index("(") + 1 : s.index(")")]
+        return cls(
+            table_name=ref_table_name,
+            column_name=ref_col_name,
+            is_nullable=is_nullable,
+            table=tables_by_name[ref_table_name],
+        )
+
+
 def build_nodes_and_resolvers_str(
     *,
     db_dsn: str,
     base_node: T.Type[Node] | None = None,
     base_resolver: T.Type[Resolver] | None = None,
     configs_by_table_name: dict[str, TableConfig],
     custom_columns_query: str = DEFAULT_COLUMNS_QUERY,
@@ -223,14 +270,15 @@
             cur.execute(custom_tables_query)
             for record in cur.fetchall():
                 table_name = record["table_name"]
                 table = Table(
                     name=table_name,
                     comment=record["comment"],
                     constraints=record["constraints"],
+                    config=configs_by_table_name.get(table_name),
                 )
                 tables_by_name[table_name] = table
             cur.execute(custom_columns_query)
             for record in cur.fetchall():
                 table_name = record["table_name"]
                 tables_by_name[table_name].columns.append(
                     Column(
@@ -262,15 +310,14 @@
     if base_resolver:
         base_resolver_name = f"{base_resolver.__name__}__"
         mixin_strs.append(
             f"from {base_resolver.__module__} import {base_resolver.__name__} as {base_resolver_name}"
         )
     else:
         base_resolver_name = "Resolver"
-
     for table in tables_by_name.values():
         # table config first
         table_config = configs_by_table_name.get(table.name)
         base_node_import_name: str | None = None
         base_resolver_import_name: str | None = None
         computed_columns_str = (
             "\t__computed_columns__: T.ClassVar[dict[str, ComputedColumn]] = {}"
@@ -333,15 +380,14 @@
                     )
             if table_config.base_resolver:
                 base_resolver_import_name = f"{table_config.base_resolver.__name__}__"
                 mixin_strs.append(
                     f"from {table_config.base_resolver.__module__} import {table_config.base_resolver.__name__} as {base_resolver_import_name}"
                 )
 
-        safe_table_name = convert_to_variable_name(table.name)
         get_params: set[str] = set()
         primary_keys: list[str] = []
 
         # first, add composite keys to get params
         if table.constraints:
             matches = re.findall(
                 r"PRIMARY KEY \(PRIMARY KEY \((.*?)\)", table.constraints
@@ -402,14 +448,15 @@
                     ):
                         if not col.is_nullable:
                             get_params.add(f"{col.name}: {python_anno} = None")
                     elif constraint.startswith("FOREIGN KEY:"):
                         col_names_to_refs[col.name] = Ref.from_str(
                             s=constraint[constraint.index("references ") + 11 :],
                             is_nullable=col.is_nullable,
+                            tables_by_name=tables_by_name,
                         )
                     elif constraint.startswith("PRIMARY KEY:"):
                         # handling this later
                         continue
                     else:
                         raise GeneratorError(f"Invalid constraint: {constraint=}")
 
@@ -468,34 +515,32 @@
         for c_name, ref in col_names_to_refs.items():
             safe_c_name = convert_to_variable_name(c_name)
             c_name_key = f"_{ref.column_name}"
             if c_name_key in safe_c_name:
                 safe_c_name = safe_c_name[: safe_c_name.rindex(f"_{ref.column_name}")]
             else:
                 safe_c_name = f"{safe_c_name}_"
-            safe_target_table_name = convert_to_variable_name(ref.table_name)
-            safe_rez_name = f"{safe_target_table_name}Resolver"
             resolver_func_strs.append(
                 f"""
-    def {safe_c_name}(self, resolver: T.Optional["{safe_rez_name}"] = None, key: str = "{safe_c_name}") -> "{safe_table_name}Resolver":
+    def {safe_c_name}(self, resolver: T.Optional["{ref.table.resolver_name}"] = None, key: str = "{safe_c_name}") -> "{table.resolver_name}":
         self.add_child(
             key=key,
-            resolver = resolver or {safe_rez_name}(),
+            resolver = resolver or {ref.table.resolver_name}(),
             cardinality=Cardinality.ONE,
             from_='FROM "{ref.table_name}" $current WHERE $current.{ref.column_name} = $parent.{c_name}',
             is_required={'True' if not ref.is_nullable else 'False'}
         )
         return self
             """
             )
             node_func_strs.append(
-                f'def {safe_c_name}(self, key: str = "{safe_c_name}") -> "{safe_target_table_name}": return self._resolve_node(key=key)'
+                f'def {safe_c_name}(self, key: str = "{safe_c_name}") -> "{ref.table.node_name}": return self._resolve_node(key=key)'
             )
         for link_name, link in computed_links.items():
-            target_rez_name = f"{link.node_name}Resolver"
+            link_table = tables_by_name.get(link.node_name)
             kwargs_strs: list[str] = []
             if link.annotations_by_kwarg:
                 for var_name, var_anno in link.annotations_by_kwarg.items():
                     kwargs_strs.append(f"{var_name}: {var_anno}")
 
             kwargs_str = ""
             update_qb_str = ""
@@ -507,30 +552,30 @@
                         [f"{n}={n}" for n in link.annotations_by_kwarg.keys()]
                     )
                 else:
                     names_str = ""
                 update_qb_str = f"self._node.__computed_links__['{link_name}'].update_qb(self._qb{names_str})"
             resolver_func_strs.append(
                 f"""
-    def {link_name}(self, resolver: T.Optional["{target_rez_name}"] = None, key: str = "{link_name}"{kwargs_str}) -> "{safe_table_name}Resolver":
+    def {link_name}(self, resolver: T.Optional["{link_table.node_name}"] = None, key: str = "{link_name}"{kwargs_str}) -> "{table.node_name}":
         self.add_child(
             key=key,
-            resolver = resolver or {target_rez_name}(),
+            resolver = resolver or {link_table.resolver_name}(),
             cardinality={'Cardinality.ONE' if link.cardinality == Cardinality.ONE else 'Cardinality.MANY'},
             from_=\"\"\"{link.from_}\"\"\",
             is_required={'False' if link.is_nullable else 'True'}
         )
         {update_qb_str}
         return self
             """
             )
             target_node_name = (
-                f'"{link.node_name}"'
+                f'"{link_table.node_name}"'
                 if link.cardinality == Cardinality.ONE
-                else f'list["{link.node_name}"]'
+                else f'list["{link_table.node_name}"]'
             )
             if link.is_nullable:
                 target_node_name = f"T.Optional[{target_node_name}]"
             node_func_strs.append(
                 f'def {link_name}(self, key: str = "{link_name}") -> {target_node_name}: return self._resolve_node(key=key)'
             )
 
@@ -539,93 +584,93 @@
 
         get_col_names = [p.split(":")[0] for p in get_params]
         get_inner_params = ", ".join(sorted([f"{n}={n}" for n in get_col_names]))
         col_str = "\n".join(sorted([f"\t{c}" for c in col_strs]))
 
         node_strs.append(
             f"""
-class {safe_table_name}({base_node_import_name or base_node_name}):
+class {table.node_name}({base_node_import_name or base_node_name}):
 {col_str}
 {node_func_str}
 {computed_columns_str}
 {columns_in_order_str}
 {table_name_str}
 {primary_keys_str}
         """
         )
         insert_str = "\n".join(sorted([f"\t{c}" for c in insert_fields_strs]))
         insert_strs.append(
             f"""
-class {safe_table_name}Insert(Insert):
+class {table.insert_name}(Insert):
 {insert_str}
             """
         )
         if patch_fields_strs:
             patch_str = "\n".join(sorted([f"\t{c}" for c in patch_fields_strs]))
             patch_strs.append(
                 f"""
-class {safe_table_name}Patch(Patch):
+class {table.patch_name}(Patch):
 {patch_str}
                 """
             )
 
         if get_params:
             joined_get_params = ", ".join(sorted(get_params))
             get_strs = f"""
-    async def get(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {safe_table_name} | None:
+    async def get(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {table.node_name} | None:
         return await self._get(conn=conn, {get_inner_params})
 
-    async def gerror(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {safe_table_name}:
+    async def gerror(self, conn: AsyncConnection | None = None, *, {joined_get_params}) -> {table.node_name}:
         return await self._gerror(conn=conn, {get_inner_params})
 
-    async def query(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> list[{safe_table_name}]:
+    async def query(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> list[{table.node_name}]:
         return await self._query(conn=conn, format_sql=format_sql, log_query=log_query)
 
-    async def first_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name} | None:
+    async def first_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {table.node_name} | None:
         return await super().first_or_none(conn=conn, format_sql=format_sql, log_query=log_query)
 
-    async def first(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name}:
+    async def first(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {table.node_name}:
         return await super().first(conn=conn, format_sql=format_sql, log_query=log_query)
 
-    async def one_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name} | None:
+    async def one_or_none(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {table.node_name} | None:
         return await super().one_or_none(conn=conn, format_sql=format_sql, log_query=log_query)
 
-    async def one(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {safe_table_name}:
+    async def one(self, conn: AsyncConnection | None = None, *, format_sql: bool = False, log_query: bool = False) -> {table.node_name}:
         return await super().one(conn=conn, format_sql=format_sql, log_query=log_query)
 
-    def filter_by(self, *, {filter_by_params_str}) -> "{safe_table_name}Resolver":
+    def filter_by(self, *, {filter_by_params_str}) -> "{table.resolver_name}":
         return self._filter_by({filter_by_inner_params})
 
-    def filter_in(self, *, {filter_in_params_str}) -> "{safe_table_name}Resolver":
+    def filter_in(self, *, {filter_in_params_str}) -> "{table.resolver_name}":
         return self._filter_in({filter_in_inner_params})
 
-    async def insert_one(self, insert: {safe_table_name}Insert, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> {safe_table_name}:
+    async def insert_one(self, insert: {table.insert_name}, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> {table.node_name}:
         return await super().insert_one(insert=insert, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh, conflict=conflict)
 
-    async def insert_one_or_none(self, insert: {safe_table_name}Insert, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> T.Optional[{safe_table_name}]:
+    async def insert_one_or_none(self, insert: {table.insert_name}, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False, conflict: Conflict | None = None) -> T.Optional[{table.node_name}]:
         return await super().insert_one_or_none(insert=insert, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh, conflict=conflict)
 
-    async def insert_many(self, inserts: list[{safe_table_name}Insert], conflict: Conflict | None = None, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False) -> list[{safe_table_name}]:
+    async def insert_many(self, inserts: list[{table.insert_name}], conflict: Conflict | None = None, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_insert: bool = False, force_refresh: bool = False) -> list[{table.node_name}]:
         return await super().insert_many(inserts=inserts, conflict=conflict, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_insert=commit_after_insert, force_refresh=force_refresh)
 
-    async def delete_one_or_none(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> T.Optional[{safe_table_name}]:
+    async def delete_one_or_none(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> T.Optional[{table.node_name}]:
         return await super().delete_one_or_none(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete)
 
-    async def delete_one(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> {safe_table_name}:
+    async def delete_one(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False) -> {table.node_name}:
         return await super().delete_one(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete)
 
-    async def delete_many(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False, delete_all: bool = False) -> list[{safe_table_name}]:
+    async def delete_many(self, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_delete: bool = False, delete_all: bool = False) -> list[{table.node_name}]:
         return await super().delete_many(format_sql=format_sql, log_query=log_query, conn=conn, commit_after_delete=commit_after_delete, delete_all=delete_all)
             """
             if patch_fields_strs:
                 patch_one_str = f"""
-    async def patch_one(self, patch: {safe_table_name}Patch, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False) -> {safe_table_name}:
+    async def patch_one(self, patch: {table.patch_name}, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False) -> {table.node_name}:
         return await super().patch_one(patch=patch, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_patch=commit_after_patch, force_refresh=force_refresh)
 
-    async def patch_many(self, patch: {safe_table_name}Patch, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False, patch_all: bool = False) -> list[{safe_table_name}]:
+    async def patch_many(self, patch: {table.patch_name}, *, format_sql: bool = False, log_query: bool = False, conn: AsyncConnection | None = None, commit_after_patch: bool = False, force_refresh: bool = False, patch_all: bool = False) -> list[{table.node_name}]:
         return await super().patch_many(patch=patch, format_sql=format_sql, log_query=log_query, conn=conn, commit_after_patch=commit_after_patch, force_refresh=force_refresh, patch_all=patch_all)
                 """
                 get_strs = f"{get_strs}\n{patch_one_str}"
         else:
             get_strs = ""
 
         include_col_anno_strs: list[str] = []
@@ -641,22 +686,22 @@
                 else:
                     include_col_anno_strs.append(f"{col.name}: bool = False")
                 include_col_inner_strs.append(f"{col.name}={col.name}")
 
         if include_col_anno_strs:
             include_col_str: str = ", ".join(sorted(include_col_anno_strs))
             include_col_inner_strs: str = ", ".join(sorted(include_col_inner_strs))
-            include_func_str = f'def include(self, *, {include_col_str}) -> "{safe_table_name}Resolver": return self._include({include_col_inner_strs})'
+            include_func_str = f'def include(self, *, {include_col_str}) -> "{table.resolver_name}": return self._include({include_col_inner_strs})'
         else:
             include_func_str = ""
 
         resolver_strs.append(
             f"""
-class {safe_table_name}Resolver({base_resolver_import_name or base_resolver_name}):
-    _node = {safe_table_name}
+class {table.resolver_name}({base_resolver_import_name or base_resolver_name}):
+    _node = {table.node_name}
 
 {get_strs}
 {resolver_func_str}
     {include_func_str}
         """
         )
     all_strs = [
```

### Comparing `asqlorm-0.6.8/asqlorm/models.py` & `asqlorm-0.7.1/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.8/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.7.1/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.8/asqlorm/utils.py` & `asqlorm-0.7.1/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.8/pyproject.toml` & `asqlorm-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.8"
+version = "0.7.1"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
```

### Comparing `asqlorm-0.6.8/PKG-INFO` & `asqlorm-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.8
+Version: 0.7.1
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
```

