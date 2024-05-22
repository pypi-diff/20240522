# Comparing `tmp/polyapi_python-0.2.5.dev8.tar.gz` & `tmp/polyapi_python-0.2.5.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polyapi_python-0.2.5.dev8.tar", last modified: Tue May 14 20:34:28 2024, max compression
+gzip compressed data, was "polyapi_python-0.2.5.dev9.tar", last modified: Wed May 15 14:25:04 2024, max compression
```

## Comparing `polyapi_python-0.2.5.dev8.tar` & `polyapi_python-0.2.5.dev9.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/polyapi/
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/client.py
--rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/error_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/typedefs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7108 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/polyapi/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-14 20:34:28.000000 polyapi_python-0.2.5.dev8/polyapi_python.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-14 20:34:28.186940 polyapi_python-0.2.5.dev8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-14 20:34:28.182940 polyapi_python-0.2.5.dev8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_function_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_rendered_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)      400 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-14 20:34:24.000000 polyapi_python-0.2.5.dev8/tests/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:25:04.162922 polyapi_python-0.2.5.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 14:25:04.158921 polyapi_python-0.2.5.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2984 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:25:04.158921 polyapi_python-0.2.5.dev9/polyapi/
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1863 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5336 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2484 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2292 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2398 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/error_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7957 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3560 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1894 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/typedefs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4200 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/polyapi/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:25:04.158921 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4859 2024-05-15 14:25:04.000000 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-15 14:25:04.000000 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:25:04.000000 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-15 14:25:04.000000 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-15 14:25:04.000000 polyapi_python-0.2.5.dev9/polyapi_python.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:25:04.162922 polyapi_python-0.2.5.dev9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:25:04.158921 polyapi_python-0.2.5.dev9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    11107 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2933 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_function_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_rendered_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2120 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2137 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-15 14:24:59.000000 polyapi_python-0.2.5.dev9/tests/test_variables.py
```

### Comparing `polyapi_python-0.2.5.dev8/LICENSE` & `polyapi_python-0.2.5.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/PKG-INFO` & `polyapi_python-0.2.5.dev9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev8
+Version: 0.2.5.dev9
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev8/README.md` & `polyapi_python-0.2.5.dev9/README.md`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/__init__.py` & `polyapi_python-0.2.5.dev9/polyapi/__init__.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/api.py` & `polyapi_python-0.2.5.dev9/polyapi/api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/auth.py` & `polyapi_python-0.2.5.dev9/polyapi/auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/cli.py` & `polyapi_python-0.2.5.dev9/polyapi/cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/client.py` & `polyapi_python-0.2.5.dev9/polyapi/client.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/config.py` & `polyapi_python-0.2.5.dev9/polyapi/config.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/constants.py` & `polyapi_python-0.2.5.dev9/polyapi/constants.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/error_handler.py` & `polyapi_python-0.2.5.dev9/polyapi/error_handler.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/execute.py` & `polyapi_python-0.2.5.dev9/polyapi/execute.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/function_cli.py` & `polyapi_python-0.2.5.dev9/polyapi/function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/generate.py` & `polyapi_python-0.2.5.dev9/polyapi/generate.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/rendered_spec.py` & `polyapi_python-0.2.5.dev9/polyapi/rendered_spec.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/schema.py` & `polyapi_python-0.2.5.dev9/polyapi/schema.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import logging
 import contextlib
 from typing import Dict
 from jsonschema_gentypes.cli import process_config
 from jsonschema_gentypes import configuration
 import tempfile
 import json
 
@@ -27,14 +28,29 @@
     with tempfile.NamedTemporaryFile(
         mode="w", delete=False, prefix="polyapi_", suffix=".json"
     ) as temp_file:
         json.dump(input_data, temp_file)
         return temp_file.name
 
 
+def wrapped_generate_schema_types(type_spec: dict, root, fallback_type):
+    if not root:
+        root = "MyList" if fallback_type == "List" else "MyDict"
+
+    try:
+        return clean_title(root), generate_schema_types(type_spec, root=root)
+    except RecursionError:
+        # some schemas are so huge, our library cant handle it
+        # TODO identify critical recursion penalty and maybe switch underlying logic to iterative?
+        return fallback_type, ""
+    except:
+        logging.exception(f"Error when generating schema type: {type_spec}")
+        return fallback_type, ""
+
+
 def generate_schema_types(input_data: Dict, root=None):
     """takes in a Dict representing a schema as input then appends the resulting python code to the output file"""
     _cleanup_input_for_gentypes(input_data)
     tmp_input = _temp_store_input_data(input_data)
     tmp_output = tempfile.NamedTemporaryFile(
         mode="w", delete=False, prefix="polyapi_", suffix=".py"
     ).name
```

### Comparing `polyapi_python-0.2.5.dev8/polyapi/server.py` & `polyapi_python-0.2.5.dev9/polyapi/server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/typedefs.py` & `polyapi_python-0.2.5.dev9/polyapi/typedefs.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/utils.py` & `polyapi_python-0.2.5.dev9/polyapi/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 import re
 import os
-import logging
 from typing import Tuple, List
 from colorama import Fore, Style
 from polyapi.constants import BASIC_PYTHON_TYPES
 from polyapi.typedefs import PropertySpecification, PropertyType
-from polyapi.schema import generate_schema_types, clean_title, map_primitive_types
+from polyapi.schema import wrapped_generate_schema_types, clean_title, map_primitive_types
 
 
 # this string should be in every __init__ file.
 # it contains all the imports needed for the function or variable code to run
 CODE_IMPORTS = "from typing import List, Dict, Any, TypedDict, Optional, Callable\nimport logging\nimport requests\nimport socketio  # type: ignore\nfrom polyapi.config import get_api_key_and_url\nfrom polyapi.execute import execute, execute_post, variable_get, variable_update\n\n"
+FALLBACK_TYPES = {"Dict", "List"}
 
 
 def init_the_init(full_path: str) -> None:
     init_path = os.path.join(full_path, "__init__.py")
     if not os.path.exists(init_path):
         with open(init_path, "w") as f:
             f.write(CODE_IMPORTS)
@@ -92,19 +92,15 @@
             return map_primitive_types(value), ""
     elif type_spec["kind"] == "primitive":
         return map_primitive_types(type_spec["type"]), ""
     elif type_spec["kind"] == "array":
         if type_spec.get("items"):
             items = type_spec["items"]
             if items.get("$ref"):
-                try:
-                    return "ResponseType", generate_schema_types(type_spec, root="ResponseType")  # type: ignore
-                except:
-                    logging.exception(f"Error when generating schema type: {type_spec}")
-                    return "Dict", ""
+                return wrapped_generate_schema_types(type_spec, "ResponseType", "Dict")  # type: ignore
             else:
                 item_type, _ = get_type_and_def(items)
                 title = f"List[{item_type}]"
                 title = clean_title(title)
                 return title, ""
         else:
             return "List", ""
@@ -112,40 +108,30 @@
         return "None", ""
     elif type_spec["kind"] == "object":
         if type_spec.get("schema"):
             schema = type_spec["schema"]
             title = schema.get("title", "")
             if title:
                 assert isinstance(title, str)
-                title = clean_title(title)
-                try:
-                    return title, generate_schema_types(schema, root=title)  # type: ignore
-                except:
-                    logging.exception(f"Error when generating schema type: {schema}")
-                    return "Dict", ""
+                return wrapped_generate_schema_types(schema, title, "Dict")  # type: ignore
 
             elif schema.get("items"):
                 # fallback to schema $ref name if no explicit title
                 items = schema.get("items")  # type: ignore
                 title = items.get("title", "")  # type: ignore
                 if not title:
                     # title is actually a reference to another schema
                     title = items.get("$ref", "")  # type: ignore
 
                 title = title.rsplit("/", 1)[-1]
-                title = clean_title(title)
                 if not title:
                     return "List", ""
 
                 title = f"List[{title}]"
-                try:
-                    return title, generate_schema_types(schema, root=title)
-                except:
-                    logging.exception(f"Error when generating schema type: {schema}")
-                    return "List", ""
+                return wrapped_generate_schema_types(schema, title, "List")
             else:
                 return "Any", ""
         else:
             return "Dict", ""
     elif type_spec["kind"] == "function":
         arg_types = []
         arg_defs = []
```

### Comparing `polyapi_python-0.2.5.dev8/polyapi/variables.py` & `polyapi_python-0.2.5.dev9/polyapi/variables.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi/webhook.py` & `polyapi_python-0.2.5.dev9/polyapi/webhook.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/polyapi_python.egg-info/PKG-INFO` & `polyapi_python-0.2.5.dev9/polyapi_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polyapi-python
-Version: 0.2.5.dev8
+Version: 0.2.5.dev9
 Summary: The Python Client for PolyAPI, the IPaaS by Developers for Developers
 Author-email: Dan Fellin <dan@polyapi.io>
 License: MIT License
         
         Copyright (c) 2023 PolyAPI Inc.
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `polyapi_python-0.2.5.dev8/polyapi_python.egg-info/SOURCES.txt` & `polyapi_python-0.2.5.dev9/polyapi_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/pyproject.toml` & `polyapi_python-0.2.5.dev9/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=61.2", "wheel"]
 
 [project]
 name = "polyapi-python"
-version = "0.2.5.dev8"
+version = "0.2.5.dev9"
 description = "The Python Client for PolyAPI, the IPaaS by Developers for Developers"
 authors = [{ name = "Dan Fellin", email = "dan@polyapi.io" }]
 dependencies = [
     "requests==2.31.0",
     "typing_extensions==4.10.0",
     "jsonschema-gentypes==2.4.0",
     "pydantic==2.6.4",
```

### Comparing `polyapi_python-0.2.5.dev8/tests/test_api.py` & `polyapi_python-0.2.5.dev9/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_auth.py` & `polyapi_python-0.2.5.dev9/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_function_cli.py` & `polyapi_python-0.2.5.dev9/tests/test_function_cli.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_rendered_spec.py` & `polyapi_python-0.2.5.dev9/tests/test_rendered_spec.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_server.py` & `polyapi_python-0.2.5.dev9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_utils.py` & `polyapi_python-0.2.5.dev9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `polyapi_python-0.2.5.dev8/tests/test_variables.py` & `polyapi_python-0.2.5.dev9/tests/test_variables.py`

 * *Files identical despite different names*

