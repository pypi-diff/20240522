# Comparing `tmp/llama_index_graph_stores_nebula-0.1.2.tar.gz` & `tmp/llama_index_graph_stores_nebula-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_graph_stores_nebula-0.1.2.tar", max compression
+gzip compressed data, was "llama_index_graph_stores_nebula-0.1.3.tar", max compression
```

## Comparing `llama_index_graph_stores_nebula-0.1.2.tar` & `llama_index_graph_stores_nebula-0.1.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       46 2024-02-13 13:53:01.641289 llama_index_graph_stores_nebula-0.1.2/README.md
--rw-r--r--   0        0        0       98 2024-02-13 13:53:01.641524 llama_index_graph_stores_nebula-0.1.2/llama_index/graph_stores/nebula/__init__.py
--rw-r--r--   0        0        0    25688 2024-02-13 13:53:01.641629 llama_index_graph_stores_nebula-0.1.2/llama_index/graph_stores/nebula/base.py
--rw-r--r--   0        0        0     1481 2024-02-21 17:11:22.167783 llama_index_graph_stores_nebula-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      707 1970-01-01 00:00:00.000000 llama_index_graph_stores_nebula-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0       46 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/README.md
+-rw-r--r--   0        0        0       98 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/__init__.py
+-rw-r--r--   0        0        0    25688 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/base.py
+-rw-r--r--   0        0        0     1481 2024-05-22 04:36:10.141452 llama_index_graph_stores_nebula-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0      656 1970-01-01 00:00:00.000000 llama_index_graph_stores_nebula-0.1.3/PKG-INFO
```

### Comparing `llama_index_graph_stores_nebula-0.1.2/llama_index/graph_stores/nebula/base.py` & `llama_index_graph_stores_nebula-0.1.3/llama_index/graph_stores/nebula/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -220,16 +220,16 @@
         session_pool = SessionPool(
             os.environ["NEBULA_USER"],
             os.environ["NEBULA_PASSWORD"],
             self._space_name,
             [(graphd_host, int(graphd_port))],
         )
 
-        seesion_pool_config = SessionPoolConfig()
-        session_pool.init(seesion_pool_config)
+        session_pool_config = SessionPoolConfig()
+        session_pool.init(session_pool_config)
         self._session_pool = session_pool
         return self._session_pool
 
     def _get_vid_type(self) -> str:
         """Get vid type."""
         return (
             self.execute(f"DESCRIBE SPACE {self._space_name}")
```

### Comparing `llama_index_graph_stores_nebula-0.1.2/pyproject.toml` & `llama_index_graph_stores_nebula-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index graph stores nebula integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-graph-stores-nebula"
 readme = "README.md"
-version = "0.1.2"
+version = "0.1.3"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 nebula3-python = "^3.4.0"
 
 [tool.poetry.group.dev.dependencies]
```

