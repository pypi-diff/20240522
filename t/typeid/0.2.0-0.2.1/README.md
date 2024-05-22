# Comparing `tmp/typeid-0.2.0.tar.gz` & `tmp/typeid-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typeid-0.2.0.tar", max compression
+gzip compressed data, was "typeid-0.2.1.tar", max compression
```

## Comparing `typeid-0.2.0.tar` & `typeid-0.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 11:53:12.620224 typeid-0.2.0/LICENSE
--rw-r--r--   0        0        0     2067 2024-05-22 15:40:19.782174 typeid-0.2.0/README.md
--rw-r--r--   0        0        0      474 2024-05-22 15:40:49.475427 typeid-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3850 2024-05-22 15:33:55.219867 typeid-0.2.0/typeid/__init__.py
--rw-r--r--   0        0        0     1283 2024-05-22 15:35:58.509544 typeid-0.2.0/typeid/sqla.py
--rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 typeid-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 11:53:12.620224 typeid-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2067 2024-05-22 15:40:19.782174 typeid-0.2.1/README.md
+-rw-r--r--   0        0        0      474 2024-05-22 19:20:17.189916 typeid-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3895 2024-05-22 19:19:39.306869 typeid-0.2.1/typeid/__init__.py
+-rw-r--r--   0        0        0     1283 2024-05-22 15:35:58.509544 typeid-0.2.1/typeid/sqla.py
+-rw-r--r--   0        0        0     2596 1970-01-01 00:00:00.000000 typeid-0.2.1/PKG-INFO
```

### Comparing `typeid-0.2.0/LICENSE` & `typeid-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `typeid-0.2.0/README.md` & `typeid-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `typeid-0.2.0/typeid/__init__.py` & `typeid-0.2.1/typeid/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,17 @@
 
         # If the user wants sqla support, these additional classes will be
         # generated
         if enable_sqla:
             from .sqla import GUID
 
             sqla_name = f"{name}SQLA"
-            sqla_typeid_class = type(name, (GUID,), dict(typeid_class=typeid_class))
+            sqla_typeid_class = type(
+                name, (GUID,), dict(typeid_class=typeid_class, cache_ok=True)
+            )
             globals()[sqla_name] = sqla_typeid_class
             ret[sqla_name] = sqla_typeid_class
     return AttrDict(ret)
 
 
 if __name__ == "__main__":
     import doctest
```

### Comparing `typeid-0.2.0/typeid/sqla.py` & `typeid-0.2.1/typeid/sqla.py`

 * *Files identical despite different names*

### Comparing `typeid-0.2.0/PKG-INFO` & `typeid-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: typeid
-Version: 0.2.0
+Version: 0.2.1
 Summary: UUID-compatible Typed IDs with prefixes
 License: MIT
 Author: Fabian Schuh
 Author-email: info@chainsquad.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

