# Comparing `tmp/dpt-0.3.9.tar.gz` & `tmp/dpt-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-0.3.9.tar", last modified: Thu Apr 18 18:34:46 2024, max compression
+gzip compressed data, was "dpt-1.0.0.tar", last modified: Wed May 22 17:12:23 2024, max compression
```

## Comparing `dpt-0.3.9.tar` & `dpt-1.0.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.573165 dpt-0.3.9/
--rw-rw-rw-   0        0        0      188 2024-04-18 18:34:46.571165 dpt-0.3.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.502166 dpt-0.3.9/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-0.3.9/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.556172 dpt-0.3.9/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-0.3.9/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-0.3.9/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-0.3.9/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-0.3.9/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-0.3.9/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.567165 dpt-0.3.9/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-0.3.9/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-0.3.9/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-0.3.9/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-0.3.9/dpt/processor.py
--rw-rw-rw-   0        0        0     5729 2024-04-12 03:20:41.000000 dpt-0.3.9/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-04-18 18:34:46.544207 dpt-0.3.9/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-18 18:34:46.000000 dpt-0.3.9/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 18:34:46.574185 dpt-0.3.9/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-04-18 18:34:40.000000 dpt-0.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.314296 dpt-1.0.0/
+-rw-rw-rw-   0        0        0      188 2024-05-22 17:12:23.313304 dpt-1.0.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.245414 dpt-1.0.0/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.0/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.298294 dpt-1.0.0/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.0/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.0/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.0/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.0/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.0/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.308291 dpt-1.0.0/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.0/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.0/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.0/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.0/dpt/processor.py
+-rw-rw-rw-   0        0        0     5852 2024-05-22 17:09:58.000000 dpt-1.0.0/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.285296 dpt-1.0.0/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:12:23.315316 dpt-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-05-22 17:11:10.000000 dpt-1.0.0/setup.py
```

### Comparing `dpt-0.3.9/dpt/deployment/deploy.py` & `dpt-1.0.0/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.9/dpt/deployment/extract.py` & `dpt-1.0.0/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.9/dpt/management.py` & `dpt-1.0.0/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.9/dpt/mongo/files.py` & `dpt-1.0.0/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.9/dpt/processor.py` & `dpt-1.0.0/dpt/processor.py`

 * *Files identical despite different names*

### Comparing `dpt-0.3.9/dpt/storage.py` & `dpt-1.0.0/dpt/storage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 from pymongo import MongoClient
 from pymongo.database import Database as MongoDatabase
 from pymongo.collection import Collection
-from typing import Any
+from typing import Any, Optional
 import jsonschema
 import copy
 
 
 class ConnectionInfo:
     def __init__(self, connectionString):
         self.connectionString = connectionString
@@ -108,14 +108,20 @@
         pipeline.append({"$out": out._collection_name})
         print(f"read {self._count} documents from {self.get_info()}")
         print("run aggregation:\n", pipeline)
         self.instance().aggregate(pipeline)
         out._update_count_from_collection()
         out.close()
 
+    def create_index(
+        self,
+        keys,
+    ) -> str:
+        self.instance().create_index(keys=keys)
+
 
 class MemoryReader:
     def __init__(self, data: list[dict[str, Any]], schema: dict):
         self._data = data
         self.schema = schema
 
     def _validate(self):
```

