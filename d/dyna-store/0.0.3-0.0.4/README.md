# Comparing `tmp/dyna_store-0.0.3.tar.gz` & `tmp/dyna_store-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dyna_store-0.0.3.tar", max compression
+gzip compressed data, was "dyna_store-0.0.4.tar", max compression
```

## Comparing `dyna_store-0.0.3.tar` & `dyna_store-0.0.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1071 2024-05-22 12:59:45.062490 dyna_store-0.0.3/LICENSE
--rw-r--r--   0        0        0      650 2024-05-22 12:59:45.062490 dyna_store-0.0.3/README.md
--rw-r--r--   0        0        0       92 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/__init__.py
--rw-r--r--   0        0        0      733 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/inmemory.py
--rw-r--r--   0        0        0     5717 2024-05-22 12:59:45.062490 dyna_store-0.0.3/dyna_store/main.py
--rw-r--r--   0        0        0     1112 2024-05-22 12:59:45.062490 dyna_store-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1448 1970-01-01 00:00:00.000000 dyna_store-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-22 16:59:17.271218 dyna_store-0.0.4/LICENSE
+-rw-r--r--   0        0        0     5361 2024-05-22 16:59:17.271218 dyna_store-0.0.4/README.md
+-rw-r--r--   0        0        0       92 2024-05-22 16:59:17.271218 dyna_store-0.0.4/dyna_store/__init__.py
+-rw-r--r--   0        0        0      636 2024-05-22 16:59:17.271218 dyna_store-0.0.4/dyna_store/inmemory.py
+-rw-r--r--   0        0        0     5020 2024-05-22 16:59:17.271218 dyna_store-0.0.4/dyna_store/main.py
+-rw-r--r--   0        0        0     1096 2024-05-22 16:59:17.271218 dyna_store-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     6126 1970-01-01 00:00:00.000000 dyna_store-0.0.4/PKG-INFO
```

### Comparing `dyna_store-0.0.3/LICENSE` & `dyna_store-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dyna_store-0.0.3/dyna_store/inmemory.py` & `dyna_store-0.0.4/dyna_store/inmemory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,23 +1,18 @@
 from __future__ import annotations
 
 import hashlib
 import json
-from typing import TypeVar
-
-from pydantic import BaseModel
 
 from .main import DynaStore, Metadata, MetadataId
 
 MD5_HASH_LENGTH = 10
 
-V = TypeVar("V", bound=BaseModel)
-
 
-class InMemoryDynaStore(DynaStore[V]):
+class InMemoryDynaStore(DynaStore):
     def init(self) -> None:
         self.db: dict[MetadataId, Metadata] = {}
 
     def save_metadata(self, metadata: Metadata) -> MetadataId:
         metadata_str = json.dumps(metadata)
         hash_ = hashlib.md5(metadata_str.encode()).hexdigest()[:MD5_HASH_LENGTH]  # noqa: S324
         id_ = MetadataId(hash_)
```

### Comparing `dyna_store-0.0.3/pyproject.toml` & `dyna_store-0.0.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "dyna-store"
-version = "0.0.3"
+version = "0.0.4"
 description = "Dynamic metadata storage"
 authors = ["brightnetwork <dev@brightnetwork.co.uk>"]
 repository = "https://github.com/brightnetwork/dyna-store"
 homepage = "https://github.com/brightnetwork/dyna-store"
 documentation = "https://github.com/brightnetwork/dyna-store"
 keywords = ["id", "meta", "store", "high-cardinality", "metadata"]
 readme = "README.md"
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.22"
-pydantic = "^2"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.3"
 mypy = "^1.9.0"
 pytest = "^8.1.1"
 pyright = "^1.1.355"
 pytest-cov = "^4.1.0"
```

