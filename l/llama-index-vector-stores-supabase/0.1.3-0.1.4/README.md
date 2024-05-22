# Comparing `tmp/llama_index_vector_stores_supabase-0.1.3.tar.gz` & `tmp/llama_index_vector_stores_supabase-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_vector_stores_supabase-0.1.3.tar", max compression
+gzip compressed data, was "llama_index_vector_stores_supabase-0.1.4.tar", max compression
```

## Comparing `llama_index_vector_stores_supabase-0.1.3.tar` & `llama_index_vector_stores_supabase-0.1.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       49 2024-02-28 16:59:36.147271 llama_index_vector_stores_supabase-0.1.3/README.md
--rw-r--r--   0        0        0      107 2024-02-28 16:59:36.147271 llama_index_vector_stores_supabase-0.1.3/llama_index/vector_stores/supabase/__init__.py
--rw-r--r--   0        0        0     5760 2024-02-28 18:53:20.650827 llama_index_vector_stores_supabase-0.1.3/llama_index/vector_stores/supabase/base.py
--rw-r--r--   0        0        0     1483 2024-02-28 18:58:29.689403 llama_index_vector_stores_supabase-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      706 1970-01-01 00:00:00.000000 llama_index_vector_stores_supabase-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0       49 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/README.md
+-rw-r--r--   0        0        0      107 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/__init__.py
+-rw-r--r--   0        0        0     6427 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/base.py
+-rw-r--r--   0        0        0     1483 2024-05-22 01:12:50.947597 llama_index_vector_stores_supabase-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      655 1970-01-01 00:00:00.000000 llama_index_vector_stores_supabase-0.1.4/PKG-INFO
```

### Comparing `llama_index_vector_stores_supabase-0.1.3/llama_index/vector_stores/supabase/base.py` & `llama_index_vector_stores_supabase-0.1.4/llama_index/vector_stores/supabase/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,17 +31,31 @@
 
     During query time, the index uses pgvector/Supabase to query for the top
     k most similar nodes.
 
     Args:
         postgres_connection_string (str):
             postgres connection string
-
         collection_name (str):
             name of the collection to store the embeddings in
+        dimension (int, optional):
+            dimension of the embeddings. Defaults to 1536.
+
+    Examples:
+        `pip install llama-index-vector-stores-supabase`
+
+        ```python
+        from llama_index.vector_stores.supabase import SupabaseVectorStore
+
+        # Set up SupabaseVectorStore
+        vector_store = SupabaseVectorStore(
+            postgres_connection_string="postgresql://<user>:<password>@<host>:<port>/<db_name>",
+            collection_name="base_demo",
+        )
+        ```
 
     """
 
     stores_text = True
     flat_metadata = False
     _client: Optional[Any] = PrivateAttr()
     _collection: Optional[Collection] = PrivateAttr()
@@ -63,14 +77,19 @@
                 f"Collection {collection_name} does not exist, "
                 f"try creating one with dimension={dimension}"
             )
             self._collection = self._client.create_collection(
                 name=collection_name, dimension=dimension
             )
 
+    def __del__(self) -> None:
+        """Close the client when the object is deleted."""
+        if self._client is not None:
+            self._client.disconnect()
+
     @property
     def client(self) -> None:
         """Get client."""
         return
 
     def _to_vecs_filters(self, filters: MetadataFilters) -> Any:
         """Convert llama filters to vecs filters. $eq is the only supported operator."""
```

### Comparing `llama_index_vector_stores_supabase-0.1.3/pyproject.toml` & `llama_index_vector_stores_supabase-0.1.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index vector_stores supabase integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-vector-stores-supabase"
 readme = "README.md"
-version = "0.1.3"
+version = "0.1.4"
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<4.0"
 llama-index-core = "^0.10.1"
 vecs = "^0.4.2"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `llama_index_vector_stores_supabase-0.1.3/PKG-INFO` & `llama_index_vector_stores_supabase-0.1.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: llama-index-vector-stores-supabase
-Version: 0.1.3
+Version: 0.1.4
 Summary: llama-index vector_stores supabase integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.8.1,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: llama-index-core (>=0.10.1,<0.11.0)
 Requires-Dist: vecs (>=0.4.2,<0.5.0)
 Description-Content-Type: text/markdown
 
 # LlamaIndex Vector_Stores Integration: Supabase
```

