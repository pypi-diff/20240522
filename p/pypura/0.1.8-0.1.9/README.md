# Comparing `tmp/pypura-0.1.8.tar.gz` & `tmp/pypura-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pypura-0.1.8.tar", max compression
+gzip compressed data, was "pypura-0.1.9.tar", max compression
```

## Comparing `pypura-0.1.8.tar` & `pypura-0.1.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1071 2023-08-15 16:50:47.479831 pypura-0.1.8/LICENSE
--rw-r--r--   0        0        0       76 2023-08-15 16:50:47.479831 pypura-0.1.8/README.md
--rw-r--r--   0        0        0      761 2023-08-15 16:51:08.171836 pypura-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      251 2023-08-15 16:51:08.175836 pypura-0.1.8/pypura/__init__.py
--rw-r--r--   0        0        0      414 2023-08-15 16:50:47.479831 pypura-0.1.8/pypura/const.py
--rw-r--r--   0        0        0      200 2023-08-15 16:50:47.479831 pypura-0.1.8/pypura/exceptions.py
--rw-r--r--   0        0        0    68656 2023-08-15 16:50:47.479831 pypura-0.1.8/pypura/fragrances.json
--rw-r--r--   0        0        0     6705 2023-08-15 16:50:47.483831 pypura-0.1.8/pypura/pura.py
--rw-r--r--   0        0        0        0 2023-08-15 16:50:47.483831 pypura-0.1.8/pypura/py.typed
--rw-r--r--   0        0        0      803 2023-08-15 16:50:47.483831 pypura-0.1.8/pypura/utils.py
--rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 pypura-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-09-01 14:54:50.951799 pypura-0.1.9/LICENSE
+-rw-r--r--   0        0        0       76 2023-09-01 14:54:50.951799 pypura-0.1.9/README.md
+-rw-r--r--   0        0        0      761 2023-09-01 14:55:14.423985 pypura-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0      251 2023-09-01 14:55:14.427985 pypura-0.1.9/pypura/__init__.py
+-rw-r--r--   0        0        0      414 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/const.py
+-rw-r--r--   0        0        0      200 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/exceptions.py
+-rw-r--r--   0        0        0    69720 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/fragrances.json
+-rw-r--r--   0        0        0     6744 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/pura.py
+-rw-r--r--   0        0        0        0 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/py.typed
+-rw-r--r--   0        0        0      803 2023-09-01 14:54:50.955799 pypura-0.1.9/pypura/utils.py
+-rw-r--r--   0        0        0      685 1970-01-01 00:00:00.000000 pypura-0.1.9/PKG-INFO
```

### Comparing `pypura-0.1.8/LICENSE` & `pypura-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pypura-0.1.8/pyproject.toml` & `pypura-0.1.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pypura"
-version = "0.1.8"
+version = "0.1.9"
 description = "Python package for interacting with Pura smart fragrance diffuser"
 authors = ["Nathan Spencer <natekspencer@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 include = ["pypura/py.typed"]
 
 [tool.poetry.dependencies]
```

### Comparing `pypura-0.1.8/pypura/fragrances.json` & `pypura-0.1.9/pypura/fragrances.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9845916795069337%*

 * *Differences: {'insert': "[(0, OrderedDict([('name', 'Apple Orchard'), ('type', 'Car Fragrance'), ('sku', "*

 * *           "'TPRC'), ('brand', 'Pura')])), (24, OrderedDict([('name', 'Winter White'), ('type', "*

 * *           "'Car Fragrance'), ('sku', 'WTWC'), ('brand', 'ILLUME')])), (133, OrderedDict([('name', "*

 * *           "'Chestnut Embers'), ('type', 'Fragrance'), ('sku', 'CNEH'), ('brand', 'Capri "*

 * *           "Blue')])), (163, OrderedDict([('name', 'Cranberry Fizz'), ('type', 'Fragrance'), "*

 * *           "('sku', 'PTZH'), ('br […]*

```diff
@@ -1,9 +1,15 @@
 [
     {
+        "brand": "Pura",
+        "name": "Apple Orchard",
+        "sku": "TPRC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "LAFCO",
         "name": "Chamomile Lavender",
         "sku": "AJWC",
         "type": "Car Fragrance"
     },
     {
         "brand": "LAFCO",
@@ -134,14 +140,20 @@
     {
         "brand": "Pura",
         "name": "White Tea No. 1",
         "sku": "WHTC",
         "type": "Car Fragrance"
     },
     {
+        "brand": "ILLUME",
+        "name": "Winter White",
+        "sku": "WTWC",
+        "type": "Car Fragrance"
+    },
+    {
         "brand": "James Harden",
         "name": "13-Confidence",
         "sku": "CGO",
         "type": "Fragrance"
     },
     {
         "brand": "James Harden",
@@ -782,14 +794,20 @@
     {
         "brand": "Apotheke",
         "name": "Charcoal",
         "sku": "WRTH",
         "type": "Fragrance"
     },
     {
+        "brand": "Capri Blue",
+        "name": "Chestnut Embers",
+        "sku": "CNEH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "ILLUME",
         "name": "Citrus Crush",
         "sku": "ICC",
         "type": "Fragrance"
     },
     {
         "brand": "ILLUME",
@@ -956,14 +974,20 @@
     {
         "brand": "Pura",
         "name": "Cranberry Fizz",
         "sku": "PTZ",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "Cranberry Fizz",
+        "sku": "PTZH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Abbott",
         "name": "Crescent Beach",
         "sku": "FVB",
         "type": "Fragrance"
     },
     {
         "brand": "Abbott",
@@ -1544,14 +1568,20 @@
     {
         "brand": "Pura",
         "name": "Holly Berry",
         "sku": "HBY",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "Holly Berry",
+        "sku": "HBYH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Homesick",
         "name": "Home Office",
         "sku": "HMO",
         "type": "Fragrance"
     },
     {
         "brand": "Homesick",
@@ -1820,14 +1850,20 @@
     {
         "brand": "Pura",
         "name": "Lavender Fields",
         "sku": "NGLH",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "Lavender Fields",
+        "sku": "LFPH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Anthropologie",
         "name": "Leather & Leaves",
         "sku": "LLAH",
         "type": "Fragrance"
     },
     {
         "brand": "Thymes",
@@ -1922,14 +1958,20 @@
     {
         "brand": "Brooklyn Candle Studio",
         "name": "Love Potion",
         "sku": "LPO",
         "type": "Fragrance"
     },
     {
+        "brand": "Brooklyn Candle Studio",
+        "name": "Love Potion",
+        "sku": "LPOH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "K. Hall Designs",
         "name": "MILK",
         "sku": "NKL",
         "type": "Fragrance"
     },
     {
         "brand": "K. Hall Designs",
@@ -2768,14 +2810,20 @@
     {
         "brand": "Pure Placid",
         "name": "Rose & Berry",
         "sku": "KPBH",
         "type": "Fragrance"
     },
     {
+        "brand": "Pure Placid",
+        "name": "Rose & Berry",
+        "sku": "KBPH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Pura",
         "name": "Rose & Wild Blackberry",
         "sku": "VQS",
         "type": "Fragrance"
     },
     {
         "brand": "NEST New York",
@@ -3650,14 +3698,20 @@
     {
         "brand": "LAFCO",
         "name": "White Grapefruit",
         "sku": "WGRH",
         "type": "Fragrance"
     },
     {
+        "brand": "Pura",
+        "name": "White Pumpkin",
+        "sku": "YWPH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "Tommy Bahama",
         "name": "White Tea Blossom",
         "sku": "WTB",
         "type": "Fragrance"
     },
     {
         "brand": "Tommy Bahama",
@@ -3692,14 +3746,20 @@
     {
         "brand": "Apotheke",
         "name": "White Vetiver",
         "sku": "VXEH",
         "type": "Fragrance"
     },
     {
+        "brand": "Capri Blue",
+        "name": "Wild Citron",
+        "sku": "CWPH",
+        "type": "Fragrance"
+    },
+    {
         "brand": "NEST New York",
         "name": "Wild Mint & Eucalyptus",
         "sku": "WME",
         "type": "Fragrance"
     },
     {
         "brand": "NEST New York",
```

### Comparing `pypura-0.1.8/pypura/pura.py` & `pypura-0.1.9/pypura/pura.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
 
     def logout(self) -> None:
         """Logout of all clients (including app)."""
         self.get_user().logout()
 
     def get_devices(self) -> Any:
         """Get devices."""
-        return self.__get("users/devices")
+        return self.__get("users/devices", params={"types": "wall,car,tabletop"})
 
     def set_always_on(self, device_id: str, *, bay: int) -> bool:
         """Set always on."""
         json = {"bay": bay}
         resp = self.__post(f"devices/{device_id}/always-on", json=json)
         return resp.get("success") is True
```

### Comparing `pypura-0.1.8/pypura/utils.py` & `pypura-0.1.9/pypura/utils.py`

 * *Files identical despite different names*

### Comparing `pypura-0.1.8/PKG-INFO` & `pypura-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pypura
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python package for interacting with Pura smart fragrance diffuser
 License: MIT
 Author: Nathan Spencer
 Author-email: natekspencer@gmail.com
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

