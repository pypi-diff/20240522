# Comparing `tmp/openyieldtables-2.2.1.tar.gz` & `tmp/openyieldtables-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openyieldtables-2.2.1.tar", max compression
+gzip compressed data, was "openyieldtables-2.2.2.tar", max compression
```

## Comparing `openyieldtables-2.2.1.tar` & `openyieldtables-2.2.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1085 2024-05-08 14:21:02.502060 openyieldtables-2.2.1/LICENSE
--rw-r--r--   0        0        0     1509 2024-05-08 14:21:02.502060 openyieldtables-2.2.1/README.md
--rw-r--r--   0        0        0     1784 2024-05-08 14:21:03.426052 openyieldtables-2.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-08 14:21:02.502060 openyieldtables-2.2.1/src/openyieldtables/__init__.py
--rw-r--r--   0        0        0   462163 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/data/yield_tables.csv
--rw-r--r--   0        0        0     9481 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/data/yield_tables_meta.csv
--rw-r--r--   0        0        0      119 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/models/__init__.py
--rw-r--r--   0        0        0     1118 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/models/yieldtable.py
--rw-r--r--   0        0        0        0 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/py.typed
--rw-r--r--   0        0        0       55 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/utils/__init__.py
--rw-r--r--   0        0        0     1379 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/utils/utils.py
--rw-r--r--   0        0        0     6249 2024-05-08 14:21:02.506060 openyieldtables-2.2.1/src/openyieldtables/yieldtables.py
--rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 openyieldtables-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1085 2024-05-22 13:49:46.770471 openyieldtables-2.2.2/LICENSE
+-rw-r--r--   0        0        0     1509 2024-05-22 13:49:46.770471 openyieldtables-2.2.2/README.md
+-rw-r--r--   0        0        0     1784 2024-05-22 13:49:47.746473 openyieldtables-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/__init__.py
+-rw-r--r--   0        0        0   462163 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/data/yield_tables.csv
+-rw-r--r--   0        0        0     9481 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/data/yield_tables_meta.csv
+-rw-r--r--   0        0        0      119 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/models/__init__.py
+-rw-r--r--   0        0        0     1118 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/models/yieldtable.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:49:46.774471 openyieldtables-2.2.2/src/openyieldtables/py.typed
+-rw-r--r--   0        0        0       55 2024-05-22 13:49:46.778471 openyieldtables-2.2.2/src/openyieldtables/utils/__init__.py
+-rw-r--r--   0        0        0     1379 2024-05-22 13:49:46.778471 openyieldtables-2.2.2/src/openyieldtables/utils/utils.py
+-rw-r--r--   0        0        0     6249 2024-05-22 13:49:46.778471 openyieldtables-2.2.2/src/openyieldtables/yieldtables.py
+-rw-r--r--   0        0        0     2319 1970-01-01 00:00:00.000000 openyieldtables-2.2.2/PKG-INFO
```

### Comparing `openyieldtables-2.2.1/LICENSE` & `openyieldtables-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/README.md` & `openyieldtables-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/pyproject.toml` & `openyieldtables-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "openyieldtables"
-version = "2.2.1"
+version = "2.2.2"
 description = ""
 authors = ["Tree.ly <hello@tree.ly>", "FMM <fmm@fmm.at>"]
 maintainers = ["FMM <fmm@fmm.at>", "Tree.ly <hello@tree.ly>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/treely/openyieldtables"
 documentation = "https://openyieldtables.readthedocs.io"
```

### Comparing `openyieldtables-2.2.1/src/openyieldtables/data/yield_tables.csv` & `openyieldtables-2.2.2/src/openyieldtables/data/yield_tables.csv`

 * *Files 0% similar despite different names*

```diff
@@ -1456,15 +1456,15 @@
 11;5;50;14.6;13.2;13.7;0.454;1394.0;20.6;124.0;2.5;164.0;9.1;3.3
 11;5;60;17.0;15.6;18.1;0.477;914.0;23.6;176.0;2.9;249.0;8.5;4.1
 11;5;70;18.9;17.6;22.0;0.464;679.0;25.9;221.0;3.2;324.0;7.5;4.6
 11;5;80;20.4;19.2;25.6;0.491;542.0;28.0;264.0;3.3;391.0;6.7;4.9
 11;5;90;21.6;20.4;28.7;0.494;459.0;29.8;299.0;3.3;449.0;5.8;5.0
 11;5;100;22.5;21.3;31.4;0.496;407.0;31.5;333.0;3.3;500.0;5.1;5.0
 11;5;110;23.2;22.1;33.8;0.498;365.0;32.8;362.0;3.3;546.0;4.6;4.9
-11;5;123;23.6;22.6;35.8;0.5;336.0;33.9;383.0;3.2;581.0;3.5;4.8
+11;5;120;23.6;22.6;35.8;0.5;336.0;33.9;383.0;3.2;581.0;3.5;4.8
 11;5;130;24.0;23.0;37.5;0.501;317.0;35.0;402.0;3.2;610.0;2.9;4.7
 11;4;10;1.4;1.2;;;;;;;;;
 11;4;20;3.2;2.9;1.2;;;;;;;;
 11;4;30;5.9;5.3;3.6;;9233.0;9.6;;;;;
 11;4;40;9.1;8.1;7.0;;3863.0;15.0;;;;;
 11;4;50;12.0;10.8;11.4;0.426;1850.0;18.9;87.0;1.7;108.0;;2.1
 11;4;60;14.4;13.0;15.8;0.452;1125.0;22.9;135.0;2.2;185.0;7.7;3.1
```

### Comparing `openyieldtables-2.2.1/src/openyieldtables/data/yield_tables_meta.csv` & `openyieldtables-2.2.2/src/openyieldtables/data/yield_tables_meta.csv`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/src/openyieldtables/models/yieldtable.py` & `openyieldtables-2.2.2/src/openyieldtables/models/yieldtable.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/src/openyieldtables/utils/utils.py` & `openyieldtables-2.2.2/src/openyieldtables/utils/utils.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/src/openyieldtables/yieldtables.py` & `openyieldtables-2.2.2/src/openyieldtables/yieldtables.py`

 * *Files identical despite different names*

### Comparing `openyieldtables-2.2.1/PKG-INFO` & `openyieldtables-2.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openyieldtables
-Version: 2.2.1
+Version: 2.2.2
 Summary: 
 Home-page: https://github.com/treely/openyieldtables
 License: MIT
 Author: Tree.ly
 Author-email: hello@tree.ly
 Maintainer: FMM
 Maintainer-email: fmm@fmm.at
```

