# Comparing `tmp/llama_index_readers_mongodb-0.1.4.tar.gz` & `tmp/llama_index_readers_mongodb-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_readers_mongodb-0.1.4.tar", max compression
+gzip compressed data, was "llama_index_readers_mongodb-0.1.5.tar", max compression
```

## Comparing `llama_index_readers_mongodb-0.1.4.tar` & `llama_index_readers_mongodb-0.1.5.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       40 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/README.md
--rw-r--r--   0        0        0       96 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/__init__.py
--rw-r--r--   0        0        0     3629 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/base.py
--rw-r--r--   0        0        0     1489 2024-04-09 18:34:43.603445 llama_index_readers_mongodb-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 llama_index_readers_mongodb-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1507 2024-05-22 01:00:14.620773 llama_index_readers_mongodb-0.1.5/README.md
+-rw-r--r--   0        0        0       96 2024-05-22 01:00:14.620773 llama_index_readers_mongodb-0.1.5/llama_index/readers/mongodb/__init__.py
+-rw-r--r--   0        0        0     3633 2024-05-22 01:00:14.620773 llama_index_readers_mongodb-0.1.5/llama_index/readers/mongodb/base.py
+-rw-r--r--   0        0        0     1489 2024-05-22 01:00:14.620773 llama_index_readers_mongodb-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     2124 1970-01-01 00:00:00.000000 llama_index_readers_mongodb-0.1.5/PKG-INFO
```

### Comparing `llama_index_readers_mongodb-0.1.4/llama_index/readers/mongodb/base.py` & `llama_index_readers_mongodb-0.1.5/llama_index/readers/mongodb/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,13 +95,13 @@
             texts = self._flatten(texts)
             text = separator.join(texts)
 
             if metadata_names is None:
                 yield Document(text=text)
             else:
                 try:
-                    metadata = {name: item[name] for name in metadata_names}
+                    metadata = {name: item.get(name) for name in metadata_names}
                 except KeyError as err:
                     raise ValueError(
                         f"{err.args[0]} field not found in Mongo document."
                     ) from err
                 yield Document(text=text, metadata=metadata)
```

### Comparing `llama_index_readers_mongodb-0.1.4/pyproject.toml` & `llama_index_readers_mongodb-0.1.5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 authors = ["Your Name <you@example.com>"]
 description = "llama-index readers mongodb integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 maintainers = ["jerryjliu"]
 name = "llama-index-readers-mongodb"
 readme = "README.md"
-version = "0.1.4"
+version = "0.1.5"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 pymongo = "^4.6.1"
 
 [tool.poetry.group.dev.dependencies]
```

