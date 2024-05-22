# Comparing `tmp/voluptuous_openapi-0.0.3.tar.gz` & `tmp/voluptuous_openapi-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voluptuous_openapi-0.0.3.tar", last modified: Sun May 12 14:39:24 2024, max compression
+gzip compressed data, was "voluptuous_openapi-0.0.4.tar", last modified: Wed May 22 01:08:19 2024, max compression
```

## Comparing `voluptuous_openapi-0.0.3.tar` & `voluptuous_openapi-0.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9331 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/tests/test_lib.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/voluptuous_openapi/
--rw-r--r--   0 runner    (1001) docker     (127)     8208 2024-05-12 14:39:16.000000 voluptuous_openapi-0.0.3/voluptuous_openapi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-12 14:39:24.701876 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-12 14:39:24.000000 voluptuous_openapi-0.0.3/voluptuous_openapi.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:08:19.607448 voluptuous_openapi-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)    11346 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 01:08:19.607448 voluptuous_openapi-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 01:08:19.611448 voluptuous_openapi-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:08:19.607448 voluptuous_openapi-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/tests/test_lib.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:08:19.607448 voluptuous_openapi-0.0.4/voluptuous_openapi/
+-rw-r--r--   0 runner    (1001) docker     (127)     8237 2024-05-22 01:08:10.000000 voluptuous_openapi-0.0.4/voluptuous_openapi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:08:19.607448 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:08:19.000000 voluptuous_openapi-0.0.4/voluptuous_openapi.egg-info/zip-safe
```

### Comparing `voluptuous_openapi-0.0.3/LICENSE` & `voluptuous_openapi-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `voluptuous_openapi-0.0.3/README.md` & `voluptuous_openapi-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `voluptuous_openapi-0.0.3/tests/test_lib.py` & `voluptuous_openapi-0.0.4/tests/test_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,14 +104,18 @@
     assert {
         "type": "object",
         "properties": {"x": {"type": "integer"}},
         "required": [],
         "additionalProperties": {"type": "string"},
     } == convert(vol.Schema({"x": int, str: str}))
 
+    assert {"type": "object", "properties": {}, "required": []} == convert(
+        vol.Schema({})
+    )
+
 
 def test_tuple():
     assert {"type": "array", "items": {"type": "string"}} == convert(vol.Schema(tuple))
     assert {"type": "array", "items": {"type": "string"}} == convert(
         vol.Schema(tuple[Any])
     )
     assert {"type": "array", "items": {"type": "integer"}} == convert(
```

### Comparing `voluptuous_openapi-0.0.3/voluptuous_openapi/__init__.py` & `voluptuous_openapi-0.0.4/voluptuous_openapi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,15 +87,15 @@
             else:
                 properties[str(pkey)] = pval
 
             if isinstance(key, vol.Required):
                 required.append(str(pkey))
 
         val = {"type": "object"}
-        if properties:
+        if properties or not additional_properties:
             val["properties"] = properties
             val["required"] = required
         if additional_properties:
             val["additionalProperties"] = additional_properties
         return val
 
     if isinstance(schema, vol.All):
```

