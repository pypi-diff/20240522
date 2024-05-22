# Comparing `tmp/data_snack-1.0.3.tar.gz` & `tmp/data_snack-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_snack-1.0.3.tar", last modified: Tue May 21 08:57:49 2024, max compression
+gzip compressed data, was "data_snack-1.0.4.tar", last modified: Wed May 22 11:20:14 2024, max compression
```

## Comparing `data_snack-1.0.3.tar` & `data_snack-1.0.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-21 08:57:42.000000 data_snack-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-21 08:57:42.000000 data_snack-1.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-21 08:57:49.743463 data_snack-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-21 08:57:42.000000 data_snack-1.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-21 08:57:42.000000 data_snack-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 08:57:42.000000 data_snack-1.0.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-21 08:57:49.743463 data_snack-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-21 08:57:42.000000 data_snack-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.735463 data_snack-1.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.735463 data_snack-1.0.3/src/data_snack/
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/connections/
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/memcached.py
--rw-r--r--   0 runner    (1001) docker     (127)     3684 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/mongo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/connections/redis.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/entities/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/entity_meta.py
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/entities/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/key_factories/
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/hash.py
--rw-r--r--   0 runner    (1001) docker     (127)      184 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/key_factories/non_cluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.739463 data_snack-1.0.3/src/data_snack/serializers/
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/dataclass.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/serializers/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/snack.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/src/data_snack/wrap/
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/data_frame.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/entity.py
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-21 08:57:42.000000 data_snack-1.0.3/src/data_snack/wrap/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/src/data_snack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-21 08:57:49.000000 data_snack-1.0.3/src/data_snack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 08:57:49.743463 data_snack-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-21 08:57:42.000000 data_snack-1.0.3/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 11:20:05.000000 data_snack-1.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 11:20:05.000000 data_snack-1.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 11:20:14.351044 data_snack-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 2024-05-22 11:20:05.000000 data_snack-1.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-05-22 11:20:05.000000 data_snack-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-22 11:20:05.000000 data_snack-1.0.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 11:20:14.351044 data_snack-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-05-22 11:20:05.000000 data_snack-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.343044 data_snack-1.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/connections/
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2318 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/memcached.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3711 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/connections/redis.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.347044 data_snack-1.0.4/src/data_snack/entities/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/entity_meta.py
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/entities/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/key_factories/
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/hash.py
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/key_factories/non_cluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/serializers/
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1362 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/dataclass.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/serializers/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6117 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/snack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack/wrap/
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2023 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1893 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/data_frame.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/entity.py
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 11:20:05.000000 data_snack-1.0.4/src/data_snack/wrap/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/src/data_snack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 11:20:14.000000 data_snack-1.0.4/src/data_snack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:20:14.351044 data_snack-1.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-22 11:20:05.000000 data_snack-1.0.4/tests/test_utils.py
```

### Comparing `data_snack-1.0.3/LICENSE` & `data_snack-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/PKG-INFO` & `data_snack-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.3/README.md` & `data_snack-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/setup.cfg` & `data_snack-1.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = data-snack
-version = 1.0.3
+version = 1.0.4
 author = webinterpret-datascience
 author_email = data-science@webinterpret.com
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/webinterpret-ds/data-snack
 project_urls =
```

### Comparing `data_snack-1.0.3/setup.py` & `data_snack-1.0.4/setup.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/connections/base.py` & `data_snack-1.0.4/src/data_snack/connections/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/connections/memcached.py` & `data_snack-1.0.4/src/data_snack/connections/memcached.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/connections/mongo.py` & `data_snack-1.0.4/src/data_snack/connections/mongo.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
 
 @dataclass
 class MongoConnection(Connection):
     connection: "pymongo.database.Database"
 
     def _get_entity_collection(self, entity_type: Type[Entity]) -> pymongo.collection.Collection:
-        collection = self.connection[entity_type.__name__]
+        collection = self.connection[f"{entity_type.__name__}-{entity_type.version}"]
         collection.create_index(
             [(key, pymongo.ASCENDING) for key in entity_type.Meta.keys],
             unique=True
         )
         return collection
 
     def get(self, key: Key) -> Optional[Dict]:
```

### Comparing `data_snack-1.0.3/src/data_snack/connections/redis.py` & `data_snack-1.0.4/src/data_snack/connections/redis.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/entities/entity.py` & `data_snack-1.0.4/src/data_snack/entities/entity.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from abc import ABC
 from dataclasses import dataclass
 from typing import Any, List, get_type_hints
 
 from data_snack.entities.entity_meta import EntityMetaClass
+from data_snack.utils import classproperty
 
 
 @dataclass
 class Entity(ABC, metaclass=EntityMetaClass):
     def __init__(self, *args: Any, **kwargs: Any):
         ...
 
     class Meta:
         keys: List[str] = []
         excluded_fields: List[str] = []
+        version: int
 
     @classmethod
     def get_all_fields(cls) -> List[str]:
         """Gets all Entity fields."""
         return list(get_type_hints(cls))
 
     @classmethod
@@ -33,7 +35,11 @@
         """Gets Entity excluded keys only."""
         return cls.Meta.excluded_fields
 
     @classmethod
     def get_keys(cls) -> List[str]:
         """Gets Entity keys only."""
         return cls.Meta.keys
+
+    @classproperty
+    def version(cls) -> str:
+        return cls.Meta.version
```

### Comparing `data_snack-1.0.3/src/data_snack/entities/entity_meta.py` & `data_snack-1.0.4/src/data_snack/entities/entity_meta.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from .exceptions import (MetaEmptyKeysException, MetaFieldsException,
                          NonExistingMetaError)
 
 
 class EntityMetaClass(ABCMeta):
 
-    meta_fields = ["keys", "excluded_fields"]
+    meta_fields = ["keys", "excluded_fields", "version"]
 
     def __new__(mcs, name, bases, dct):
         entity_class = super().__new__(mcs, name, bases, dct)
         # TODO: consider encapsulation of each validation rule to function to make this class cleaner.
         if "Meta" not in dir(entity_class):
             raise NonExistingMetaError(
                 f"Private class `Meta not defined for {entity_class.__name__}."
```

### Comparing `data_snack-1.0.3/src/data_snack/entities/schema.py` & `data_snack-1.0.4/src/data_snack/entities/schema.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/key_factories/base.py` & `data_snack-1.0.4/src/data_snack/key_factories/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 @dataclass
 class Key(ABC):
     """An abstract key."""
     entity_type: Type[Entity]
     key_values: List[Any]
 
     def __hash__(self):
-        return hash((self.entity_type.__name__, *self.key_values))
+        return hash((self.entity_type.__name__, self.entity_type.version, *self.key_values))
 
     @abstractmethod
     def get_pattern(self, pattern: str) -> str:
         """
         Gets pattern string.
         :return: pattern string in specified format
         """
```

### Comparing `data_snack-1.0.3/src/data_snack/serializers/base.py` & `data_snack-1.0.4/src/data_snack/serializers/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/serializers/dataclass.py` & `data_snack-1.0.4/src/data_snack/serializers/dataclass.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/serializers/json.py` & `data_snack-1.0.4/src/data_snack/serializers/json.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/snack.py` & `data_snack-1.0.4/src/data_snack/snack.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/wrap/base.py` & `data_snack-1.0.4/src/data_snack/wrap/base.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/wrap/data_frame.py` & `data_snack-1.0.4/src/data_snack/wrap/data_frame.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack/wrap/entity.py` & `data_snack-1.0.4/src/data_snack/wrap/entity.py`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/src/data_snack.egg-info/PKG-INFO` & `data_snack-1.0.4/src/data_snack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data_snack
-Version: 1.0.3
+Version: 1.0.4
 Home-page: https://github.com/webinterpret-ds/data-snack
 Author: webinterpret-datascience
 Author-email: data-science@webinterpret.com
 Project-URL: Bug Tracker, https://github.com/webinterpret-ds/data-snack/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
```

### Comparing `data_snack-1.0.3/src/data_snack.egg-info/SOURCES.txt` & `data_snack-1.0.4/src/data_snack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data_snack-1.0.3/tests/test_utils.py` & `data_snack-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

