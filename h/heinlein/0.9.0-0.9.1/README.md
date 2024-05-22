# Comparing `tmp/heinlein-0.9.0.tar.gz` & `tmp/heinlein-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heinlein-0.9.0.tar", max compression
+gzip compressed data, was "heinlein-0.9.1.tar", max compression
```

## Comparing `heinlein-0.9.0.tar` & `heinlein-0.9.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
--rw-r--r--   0        0        0     2260 2024-03-07 20:11:13.089527 heinlein-0.9.0/README.md
--rw-r--r--   0        0        0      153 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/__init__.py
--rw-r--r--   0        0        0       60 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/api/__init__.py
--rw-r--r--   0        0        0     1235 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/api/_cmds.py
--rw-r--r--   0        0        0     1246 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/cmds.py
--rw-r--r--   0        0        0       61 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/__init__.py
--rw-r--r--   0        0        0     3267 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/cmds.json
--rw-r--r--   0        0        0       47 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/config.json
--rw-r--r--   0        0        0      327 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/config.py
--rw-r--r--   0        0        0       50 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/default.json
--rw-r--r--   0        0        0      116 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/dtypes/catalog.json
--rw-r--r--   0        0        0      412 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/dtypes/dtypes.json
--rw-r--r--   0        0        0      115 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/config/region/region.json
--rw-r--r--   0        0        0      166 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dataset/__init__.py
--rw-r--r--   0        0        0     9772 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dataset/dataset.py
--rw-r--r--   0        0        0        1 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/__init__.py
--rw-r--r--   0        0        0     4109 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/catalog.py
--rw-r--r--   0        0        0      641 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/dobj.py
--rw-r--r--   0        0        0      122 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/handlers/__init__.py
--rw-r--r--   0        0        0     6867 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/handlers/catalog.py
--rw-r--r--   0        0        0      475 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/handlers/handler.py
--rw-r--r--   0        0        0     1440 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/handlers/mask.py
--rw-r--r--   0        0        0     1257 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/handlers/utilities.py
--rw-r--r--   0        0        0     9486 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/dtypes/mask.py
--rw-r--r--   0        0        0      191 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/entrypoint.py
--rw-r--r--   0        0        0      642 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/locations.py
--rw-r--r--   0        0        0      102 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/manager/__init__.py
--rw-r--r--   0        0        0    13350 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/manager/manager.py
--rw-r--r--   0        0        0      158 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/region/__init__.py
--rw-r--r--   0        0        0     4317 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/region/base.py
--rw-r--r--   0        0        0     2046 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/region/footprint.py
--rw-r--r--   0        0        0     5959 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/region/region.py
--rw-r--r--   0        0        0     1856 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/region/sampling.py
--rw-r--r--   0        0        0      158 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/utilities/__init__.py
--rw-r--r--   0        0        0     3444 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/utilities/split.py
--rw-r--r--   0        0        0     2695 2024-03-07 20:11:13.253526 heinlein-0.9.0/heinlein/utilities/utilities.py
--rw-r--r--   0        0        0     1279 2024-03-07 20:11:13.253526 heinlein-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 heinlein-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     2260 2024-05-22 19:39:07.211451 heinlein-0.9.1/README.md
+-rw-r--r--   0        0        0      175 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/__init__.py
+-rw-r--r--   0        0        0       60 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/api/__init__.py
+-rw-r--r--   0        0        0     1235 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/api/_cmds.py
+-rw-r--r--   0        0        0     1246 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/cmds.py
+-rw-r--r--   0        0        0       61 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/__init__.py
+-rw-r--r--   0        0        0     3267 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/cmds.json
+-rw-r--r--   0        0        0       47 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/config.json
+-rw-r--r--   0        0        0      327 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/config.py
+-rw-r--r--   0        0        0       50 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/default.json
+-rw-r--r--   0        0        0      116 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/dtypes/catalog.json
+-rw-r--r--   0        0        0      412 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/dtypes/dtypes.json
+-rw-r--r--   0        0        0      115 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/config/region/region.json
+-rw-r--r--   0        0        0      166 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dataset/__init__.py
+-rw-r--r--   0        0        0     9772 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dataset/dataset.py
+-rw-r--r--   0        0        0        1 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/__init__.py
+-rw-r--r--   0        0        0     4109 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/catalog.py
+-rw-r--r--   0        0        0      641 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/dobj.py
+-rw-r--r--   0        0        0      122 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/handlers/__init__.py
+-rw-r--r--   0        0        0     6867 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/handlers/catalog.py
+-rw-r--r--   0        0        0      475 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/handlers/handler.py
+-rw-r--r--   0        0        0     1440 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/handlers/mask.py
+-rw-r--r--   0        0        0     1257 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/handlers/utilities.py
+-rw-r--r--   0        0        0     9486 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/dtypes/mask.py
+-rw-r--r--   0        0        0      191 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/entrypoint.py
+-rw-r--r--   0        0        0      642 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/locations.py
+-rw-r--r--   0        0        0      102 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/manager/__init__.py
+-rw-r--r--   0        0        0    13350 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/manager/manager.py
+-rw-r--r--   0        0        0      158 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/region/__init__.py
+-rw-r--r--   0        0        0     4317 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/region/base.py
+-rw-r--r--   0        0        0     2687 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/region/footprint.py
+-rw-r--r--   0        0        0     5959 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/region/region.py
+-rw-r--r--   0        0        0     1856 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/region/sampling.py
+-rw-r--r--   0        0        0      158 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/utilities/__init__.py
+-rw-r--r--   0        0        0     3444 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/utilities/split.py
+-rw-r--r--   0        0        0     2695 2024-05-22 19:39:07.391453 heinlein-0.9.1/heinlein/utilities/utilities.py
+-rw-r--r--   0        0        0     1279 2024-05-22 19:39:07.395453 heinlein-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 heinlein-0.9.1/PKG-INFO
```

### Comparing `heinlein-0.9.0/README.md` & `heinlein-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/api/_cmds.py` & `heinlein-0.9.1/heinlein/api/_cmds.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/cmds.py` & `heinlein-0.9.1/heinlein/cmds.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/config/cmds.json` & `heinlein-0.9.1/heinlein/config/cmds.json`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dataset/dataset.py` & `heinlein-0.9.1/heinlein/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/catalog.py` & `heinlein-0.9.1/heinlein/dtypes/catalog.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/dobj.py` & `heinlein-0.9.1/heinlein/dtypes/dobj.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/handlers/catalog.py` & `heinlein-0.9.1/heinlein/dtypes/handlers/catalog.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/handlers/mask.py` & `heinlein-0.9.1/heinlein/dtypes/handlers/mask.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/handlers/utilities.py` & `heinlein-0.9.1/heinlein/dtypes/handlers/utilities.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/dtypes/mask.py` & `heinlein-0.9.1/heinlein/dtypes/mask.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/locations.py` & `heinlein-0.9.1/heinlein/locations.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/manager/manager.py` & `heinlein-0.9.1/heinlein/manager/manager.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/region/base.py` & `heinlein-0.9.1/heinlein/region/base.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/region/footprint.py` & `heinlein-0.9.1/heinlein/region/footprint.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from functools import singledispatchmethod
+
 import astropy.units as u
 from shapely import GeometryCollection, STRtree, union_all
 
 from .region import BaseRegion
 from .sampling import Sampler
 
 
@@ -32,28 +34,44 @@
     def __init__(self, regions: dict[str, BaseRegion], *args, **kwargs):
         self._regnames = list(regions.keys())
         self._regions = list(regions.values())
         self._tree = build_tree(self._regions)
         self._footprint = build_footprint(self._regions)
         self._sampler = Sampler(self._footprint)
 
+    @singledispatchmethod
     def get_overlapping_regions(self, region: BaseRegion):
         """
         Returns a list of regions that overlap with the given region
         """
         overlap_idx = self._tree.query(region.geometry)
         overlaps = [self._regions[i] for i in overlap_idx]
         overlaps = filter(lambda x: x.intersects(region), overlaps)
         return list(overlaps)
 
-    def get_overlapping_region_names(self, region: BaseRegion):
+    @get_overlapping_regions.register
+    def _(self, region: list):
+        region_overlaps = [self._tree.query(other.geometry) for other in region]
+        overlaps = [
+            [self._regions[i] for i in overlaps] for overlaps in region_overlaps
+        ]
+        overlaps = [
+            [o for o in overlap if o.intersects(region[i])]
+            for i, overlap in enumerate(overlaps)
+        ]
+        return overlaps
+
+    def get_overlapping_region_names(self, region: BaseRegion | list[BaseRegion]):
         """
         Returns a list of region names that overlap with the given region
         """
-        return [r.name for r in self.get_overlapping_regions(region)]
+        overlaps = self.get_overlapping_regions(region)
+        if isinstance(region, list):
+            return [[r.name for r in o] for o in overlaps]
+        return [r.name for r in overlaps]
 
     def sample(self, n: int = 1, tolerance: u.Quantity = None, *args, **kwargs):
         """
         Return n random points from the footprint
         """
         if n == 1:
             return self._sampler.sample(tolerance=tolerance)
```

### Comparing `heinlein-0.9.0/heinlein/region/region.py` & `heinlein-0.9.1/heinlein/region/region.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/region/sampling.py` & `heinlein-0.9.1/heinlein/region/sampling.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/utilities/split.py` & `heinlein-0.9.1/heinlein/utilities/split.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/heinlein/utilities/utilities.py` & `heinlein-0.9.1/heinlein/utilities/utilities.py`

 * *Files identical despite different names*

### Comparing `heinlein-0.9.0/pyproject.toml` & `heinlein-0.9.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 
 [tool.poetry]
 name = "heinlein"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Patrick Wells <pwells@ucdavis.edu>"]
 readme = "README.md"
 exclude = ["surveys"]
 
 
 [tool.poetry.dependencies]
```

### Comparing `heinlein-0.9.0/PKG-INFO` & `heinlein-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heinlein
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Patrick Wells
 Author-email: pwells@ucdavis.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

