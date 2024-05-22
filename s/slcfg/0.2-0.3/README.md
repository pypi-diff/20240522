# Comparing `tmp/slcfg-0.2.tar.gz` & `tmp/slcfg-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slcfg-0.2.tar", max compression
+gzip compressed data, was "slcfg-0.3.tar", max compression
```

## Comparing `slcfg-0.2.tar` & `slcfg-0.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1062 2024-02-11 13:25:40.884860 slcfg-0.2/LICENSE
--rw-r--r--   0        0        0        0 2024-02-11 13:25:40.907861 slcfg-0.2/README.md
--rw-r--r--   0        0        0     2453 2024-02-11 13:25:40.884860 slcfg-0.2/pyproject.toml
--rw-r--r--   0        0        0      890 2024-02-11 13:25:40.884860 slcfg-0.2/slcfg/__init__.py
--rw-r--r--   0        0        0      440 2024-02-11 13:25:40.884860 slcfg-0.2/slcfg/config.py
--rw-r--r--   0        0        0     1067 2024-02-11 13:25:40.884860 slcfg-0.2/slcfg/environment.py
--rw-r--r--   0        0        0     1975 2024-02-11 13:25:40.885860 slcfg-0.2/slcfg/item.py
--rw-r--r--   0        0        0     2249 2024-02-11 13:25:40.885860 slcfg-0.2/slcfg/layer.py
--rw-r--r--   0        0        0        0 2024-02-11 13:25:40.907861 slcfg-0.2/slcfg/py.typed
--rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 slcfg-0.2/PKG-INFO
+-rw-r--r--   0        0        0     1062 2024-05-22 19:19:21.309418 slcfg-0.3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-22 19:19:21.340419 slcfg-0.3/README.md
+-rw-r--r--   0        0        0     2453 2024-05-22 19:19:21.309418 slcfg-0.3/pyproject.toml
+-rw-r--r--   0        0        0     1136 2024-05-22 19:19:21.309418 slcfg-0.3/slcfg/__init__.py
+-rw-r--r--   0        0        0      440 2024-05-22 19:19:21.309418 slcfg-0.3/slcfg/config.py
+-rw-r--r--   0        0        0     1067 2024-05-22 19:19:21.310418 slcfg-0.3/slcfg/environment.py
+-rw-r--r--   0        0        0     1975 2024-05-22 19:19:21.310418 slcfg-0.3/slcfg/item.py
+-rw-r--r--   0        0        0     3410 2024-05-22 19:19:21.310418 slcfg-0.3/slcfg/layer.py
+-rw-r--r--   0        0        0        0 2024-05-22 19:19:21.340419 slcfg-0.3/slcfg/py.typed
+-rw-r--r--   0        0        0      387 1970-01-01 00:00:00.000000 slcfg-0.3/PKG-INFO
```

### Comparing `slcfg-0.2/LICENSE` & `slcfg-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `slcfg-0.2/pyproject.toml` & `slcfg-0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "slcfg"
-version = "0.2"
+version = "0.3"
 description = "Simple Layered Configuration library"
 authors = ["Florian Daude <floriandaude@hotmail.fr>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.12"
```

### Comparing `slcfg-0.2/slcfg/environment.py` & `slcfg-0.3/slcfg/environment.py`

 * *Files identical despite different names*

### Comparing `slcfg-0.2/slcfg/item.py` & `slcfg-0.3/slcfg/item.py`

 * *Files identical despite different names*

### Comparing `slcfg-0.2/slcfg/layer.py` & `slcfg-0.3/slcfg/layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,95 +1,135 @@
 import abc
+import base64
 import dataclasses
 import io
 import json
 import os
 import pathlib
 import tomllib
 import typing
 
 from slcfg import item
 
-type Transformer[T, S] = typing.Callable[[T], S]
+type _AbstractTransformer[T, S] = typing.Callable[[T], S]
 type Layer = Source[item.Items]
 
 
 @dataclasses.dataclass
 class Source[T](abc.ABC):
     getter: typing.Callable[[], T]
 
-    def __or__[S](self, t: Transformer[T, S]):
+    def __or__[S](self, t: _AbstractTransformer[T, S]):
         return Source(getter=lambda: t(self.getter()))
 
 
-### File Sources
+@dataclasses.dataclass
+class Transformer[T, S]:
+    handler: _AbstractTransformer[T, S]
+
+    def __call__(self, t: T):
+        return self.handler(t)
+
+    def __or__[U](self, other: _AbstractTransformer[S, U]):
+        return Transformer[T, U](handler=lambda t: other(self.handler(t)))
+
 
+### Sources
 
-def file_source(path: pathlib.Path, *, optional: bool):
+
+def source[T](v: T) -> Source[T]:
+    return Source(getter=lambda: v)
+
+
+def file_source(path: pathlib.Path, *, optional: bool = False):
     def getter():
         try:
             return io.BytesIO(path.read_bytes())
         except FileNotFoundError:
             if optional:
                 return io.BytesIO()
             raise
 
     return Source(getter=getter)
 
 
-def file_layer(
-    path: pathlib.Path, parser: Transformer[io.BytesIO, typing.Any], *, optional: bool = False
-):
-    return file_source(path, optional=optional) | parser | item.list_items
-
+def env_source():
+    return Source(getter=lambda: list(os.environ.items()))
 
-def json_file_layer(path: pathlib.Path, *, optional: bool = False):
-    return file_layer(path, json.load, optional=optional)
 
+def env_var_source(name: str, *, optional: bool = False):
+    def getter():
+        if (value := os.environ.get(name)) is not None:
+            return value
+        if optional:
+            return ''
+        raise KeyError(name)
 
-def toml_file_layer(path: pathlib.Path, *, optional: bool = False):
-    return file_layer(path, tomllib.load, optional=optional)
+    return Source(getter=getter)
 
 
-### Env Sources
+### Transformers
 
 
-def env_source():
-    return Source(getter=lambda: list(os.environ.items()))
+base64_transform = Transformer(base64.b64decode) | io.BytesIO
+hex_transform = Transformer(bytes.fromhex) | io.BytesIO
+utf8_transform = Transformer(str.encode) | io.BytesIO
+json_transform = Transformer(json.load) | item.list_items
+toml_transform = Transformer(tomllib.load) | item.list_items
 
 
-def case_transform(vars: list[tuple[str, str]]):
+def _case_transform(vars: list[tuple[str, str]]):
     return [(k.lower(), v) for k, v in vars]
 
 
-def prefix_transformer(prefix: str):
+def _prefix_transform(prefix: str):
     def transormer(vars: list[tuple[str, str]]):
         return [(k.removeprefix(prefix), v) for k, v in vars if k.startswith(prefix)]
 
     return transormer
 
 
-def delimiter_transformer(delimiter: str):
+def _delimiter_transform(delimiter: str):
     def transormer(vars: list[tuple[str, str]]):
         return [(k.split(delimiter), v) for k, v in vars]
 
     return transormer
 
 
 def item_transform(vars: list[tuple[list[str], str]]) -> item.Items:
     return [item.Item(k, v) for k, v in vars]
 
 
+### Shortcuts
+
+
+def json_file_layer(path: pathlib.Path, *, optional: bool = False):
+    return file_source(path, optional=optional) | json_transform
+
+
+def toml_file_layer(path: pathlib.Path, *, optional: bool = False):
+    return file_source(path, optional=optional) | toml_transform
+
+
+def base64_env_json(var_name: str, *, optional: bool = False):
+    return env_var_source(var_name, optional=optional) | base64_transform | json_transform
+
+
+def base64_env_toml(var_name: str, *, optional: bool = False):
+    return env_var_source(var_name, optional=optional) | base64_transform | toml_transform
+
+
 def env_layer(prefix: str, nested_delimiter: str, *, case_sensitive: bool = False):
     source = env_source()
 
     if not case_sensitive:
         prefix = prefix.lower()
         nested_delimiter = nested_delimiter.lower()
-        source = source | case_transform
+        source = source | _case_transform
 
     return (
-        source
-        | prefix_transformer(prefix)
-        | delimiter_transformer(nested_delimiter)
-        | item_transform
+        source | _prefix_transform(prefix) | _delimiter_transform(nested_delimiter) | item_transform
     )
+
+
+def value_layer(value: item.ValueTree):
+    return source(value) | item.list_items
```

