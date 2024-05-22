# Comparing `tmp/llama_index_embeddings_google-0.1.5.tar.gz` & `tmp/llama_index_embeddings_google-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llama_index_embeddings_google-0.1.5.tar", max compression
+gzip compressed data, was "llama_index_embeddings_google-0.1.6.tar", max compression
```

## Comparing `llama_index_embeddings_google-0.1.5.tar` & `llama_index_embeddings_google-0.1.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       44 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/README.md
--rw-r--r--   0        0        0      320 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/__init__.py
--rw-r--r--   0        0        0     3411 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/gemini.py
--rw-r--r--   0        0        0     2469 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/palm.py
--rw-r--r--   0        0        0     2108 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/univ_sent_encoder.py
--rw-r--r--   0        0        0     1700 2024-04-05 18:55:12.220015 llama_index_embeddings_google-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 llama_index_embeddings_google-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       44 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/README.md
+-rw-r--r--   0        0        0      320 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/__init__.py
+-rw-r--r--   0        0        0     3411 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/gemini.py
+-rw-r--r--   0        0        0     2469 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/palm.py
+-rw-r--r--   0        0        0     2108 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/univ_sent_encoder.py
+-rw-r--r--   0        0        0     1700 2024-05-22 14:28:39.445433 llama_index_embeddings_google-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      760 1970-01-01 00:00:00.000000 llama_index_embeddings_google-0.1.6/PKG-INFO
```

### Comparing `llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/gemini.py` & `llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/gemini.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/palm.py` & `llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/palm.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_google-0.1.5/llama_index/embeddings/google/univ_sent_encoder.py` & `llama_index_embeddings_google-0.1.6/llama_index/embeddings/google/univ_sent_encoder.py`

 * *Files identical despite different names*

### Comparing `llama_index_embeddings_google-0.1.5/pyproject.toml` & `llama_index_embeddings_google-0.1.6/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -25,20 +25,20 @@
 [tool.poetry]
 authors = ["Your Name <you@example.com>"]
 description = "llama-index embeddings google integration"
 exclude = ["**/BUILD"]
 license = "MIT"
 name = "llama-index-embeddings-google"
 readme = "README.md"
-version = "0.1.5"
+version = "0.1.6"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 llama-index-core = "^0.10.11.post1"
-google-generativeai = "^0.4.1"
+google-generativeai = "^0.5.2"
 
 [tool.poetry.dependencies.tensorflow-hub]
 optional = true
 version = "^0.15.0"
 
 [tool.poetry.extras]
 tensorflow = ["tensorflow-hub"]
```

### Comparing `llama_index_embeddings_google-0.1.5/PKG-INFO` & `llama_index_embeddings_google-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: llama-index-embeddings-google
-Version: 0.1.5
+Version: 0.1.6
 Summary: llama-index embeddings google integration
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: tensorflow
-Requires-Dist: google-generativeai (>=0.4.1,<0.5.0)
+Requires-Dist: google-generativeai (>=0.5.2,<0.6.0)
 Requires-Dist: llama-index-core (>=0.10.11.post1,<0.11.0)
 Requires-Dist: tensorflow-hub (>=0.15.0,<0.16.0) ; extra == "tensorflow"
 Description-Content-Type: text/markdown
 
 # LlamaIndex Embeddings Integration: Google
```

