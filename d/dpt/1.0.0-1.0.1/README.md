# Comparing `tmp/dpt-1.0.0.tar.gz` & `tmp/dpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dpt-1.0.0.tar", last modified: Wed May 22 17:12:23 2024, max compression
+gzip compressed data, was "dpt-1.0.1.tar", last modified: Wed May 22 17:45:16 2024, max compression
```

## Comparing `dpt-1.0.0.tar` & `dpt-1.0.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.314296 dpt-1.0.0/
--rw-rw-rw-   0        0        0      188 2024-05-22 17:12:23.313304 dpt-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.245414 dpt-1.0.0/dpt/
--rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.0/dpt/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.298294 dpt-1.0.0/dpt/deployment/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.0/dpt/deployment/__init__.py
--rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.0/dpt/deployment/common.py
--rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.0/dpt/deployment/deploy.py
--rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.0/dpt/deployment/extract.py
--rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.0/dpt/management.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.308291 dpt-1.0.0/dpt/mongo/
--rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.0/dpt/mongo/__init__.py
--rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.0/dpt/mongo/commands.py
--rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.0/dpt/mongo/files.py
--rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.0/dpt/processor.py
--rw-rw-rw-   0        0        0     5852 2024-05-22 17:09:58.000000 dpt-1.0.0/dpt/storage.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:12:23.285296 dpt-1.0.0/dpt.egg-info/
--rw-rw-rw-   0        0        0      188 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-22 17:12:23.000000 dpt-1.0.0/dpt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-22 17:12:23.315316 dpt-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      338 2024-05-22 17:11:10.000000 dpt-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:45:16.984944 dpt-1.0.1/
+-rw-rw-rw-   0        0        0      188 2024-05-22 17:45:16.982941 dpt-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-22 17:45:16.954372 dpt-1.0.1/dpt/
+-rw-rw-rw-   0        0        0      123 2024-03-05 23:00:59.000000 dpt-1.0.1/dpt/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:45:16.976940 dpt-1.0.1/dpt/deployment/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:57:26.000000 dpt-1.0.1/dpt/deployment/__init__.py
+-rw-rw-rw-   0        0        0      110 2024-02-01 20:25:45.000000 dpt-1.0.1/dpt/deployment/common.py
+-rw-rw-rw-   0        0        0     9539 2024-04-14 15:36:27.000000 dpt-1.0.1/dpt/deployment/deploy.py
+-rw-rw-rw-   0        0        0     1054 2024-02-01 20:24:35.000000 dpt-1.0.1/dpt/deployment/extract.py
+-rw-rw-rw-   0        0        0     1981 2024-02-01 20:24:46.000000 dpt-1.0.1/dpt/management.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:45:16.981952 dpt-1.0.1/dpt/mongo/
+-rw-rw-rw-   0        0        0        4 2024-02-01 03:59:35.000000 dpt-1.0.1/dpt/mongo/__init__.py
+-rw-rw-rw-   0        0        0      266 2024-01-27 22:13:49.000000 dpt-1.0.1/dpt/mongo/commands.py
+-rw-rw-rw-   0        0        0     1032 2024-01-28 00:52:12.000000 dpt-1.0.1/dpt/mongo/files.py
+-rw-rw-rw-   0        0        0    13269 2024-04-14 20:36:18.000000 dpt-1.0.1/dpt/processor.py
+-rw-rw-rw-   0        0        0     6622 2024-05-22 17:43:31.000000 dpt-1.0.1/dpt/storage.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:45:16.969952 dpt-1.0.1/dpt.egg-info/
+-rw-rw-rw-   0        0        0      188 2024-05-22 17:45:16.000000 dpt-1.0.1/dpt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      374 2024-05-22 17:45:16.000000 dpt-1.0.1/dpt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:45:16.000000 dpt-1.0.1/dpt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2024-05-22 17:45:16.000000 dpt-1.0.1/dpt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 17:45:16.000000 dpt-1.0.1/dpt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:45:16.985940 dpt-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      338 2024-05-22 17:45:01.000000 dpt-1.0.1/setup.py
```

### Comparing `dpt-1.0.0/dpt/deployment/deploy.py` & `dpt-1.0.1/dpt/deployment/deploy.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.0/dpt/deployment/extract.py` & `dpt-1.0.1/dpt/deployment/extract.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.0/dpt/management.py` & `dpt-1.0.1/dpt/management.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.0/dpt/mongo/files.py` & `dpt-1.0.1/dpt/mongo/files.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.0/dpt/processor.py` & `dpt-1.0.1/dpt/processor.py`

 * *Files identical despite different names*

### Comparing `dpt-1.0.0/dpt/storage.py` & `dpt-1.0.1/dpt/storage.py`

 * *Files 5% similar despite different names*

```diff
@@ -98,17 +98,36 @@
             if step_name in ["$lookup", "$graphLookup", "$unionWith"]:
                 coll_ref = step.get("from") or step.get("coll")
                 if isinstance(coll_ref, DbReader):
                     step["from"] = coll_ref._collection_name
                 else:
                     raise Exception(bad_ref_text(step, coll_ref))
 
+    def _create_lookup_indexes(self, item: list[dict] | dict):
+        objects = []
+        if isinstance(item, dict):
+            objects = [item]
+        if isinstance(item, list):
+            objects = item
+        for obj in objects:
+            if isinstance(obj, dict):
+                for name in obj:
+                    if name == "$lookup":
+                        spec = obj["$lookup"]
+                        coll_name = spec["from"]
+                        field = spec["foreignField"]
+                        coll = self.instance().database[coll_name]
+                        ind_opt = (field, 1)
+                        coll.create_index([ind_opt])
+                    self._create_lookup_indexes(obj[name])
+
     def aggregate(self, out: DbWriter, pipeline: list[dict[str, Any]]):
         self._update_count_from_collection()
         self._prepare_pipeline(pipeline)
+        self._create_lookup_indexes(pipeline)
         pipeline.append({"$out": out._collection_name})
         print(f"read {self._count} documents from {self.get_info()}")
         print("run aggregation:\n", pipeline)
         self.instance().aggregate(pipeline)
         out._update_count_from_collection()
         out.close()
```

