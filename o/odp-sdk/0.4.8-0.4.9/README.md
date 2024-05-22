# Comparing `tmp/odp_sdk-0.4.8.tar.gz` & `tmp/odp_sdk-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odp_sdk-0.4.8.tar", max compression
+gzip compressed data, was "odp_sdk-0.4.9.tar", max compression
```

## Comparing `odp_sdk-0.4.8.tar` & `odp_sdk-0.4.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1052 2024-04-19 13:36:25.680702 odp_sdk-0.4.8/LICENSE
--rw-r--r--   0        0        0      836 2024-04-19 13:36:25.680702 odp_sdk-0.4.8/README.md
--rw-r--r--   0        0        0       30 2024-04-19 13:36:25.680702 odp_sdk-0.4.8/odp_sdk/__init__.py
--rw-r--r--   0        0        0    12698 2024-04-19 13:36:25.680702 odp_sdk-0.4.8/odp_sdk/auth.py
--rw-r--r--   0        0        0     1941 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/client.py
--rw-r--r--   0        0        0       84 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/dto/__init__.py
--rw-r--r--   0        0        0      856 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/dto/file_dto.py
--rw-r--r--   0        0        0     1938 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/dto/resource_dto.py
--rw-r--r--   0        0        0      846 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/dto/table_spec.py
--rw-r--r--   0        0        0     1391 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/dto/tabular_store.py
--rw-r--r--   0        0        0     1012 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/exc.py
--rw-r--r--   0        0        0     7933 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/http_client.py
--rw-r--r--   0        0        0     8303 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/raw_storage_client.py
--rw-r--r--   0        0        0     6759 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/resource_client.py
--rw-r--r--   0        0        0    17200 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/tabular_storage_client.py
--rw-r--r--   0        0        0       39 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/utils/__init__.py
--rw-r--r--   0        0        0     1789 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/utils/json.py
--rw-r--r--   0        0        0     4249 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/utils/ndjson.py
--rw-r--r--   0        0        0      170 2024-04-19 13:36:25.684702 odp_sdk-0.4.8/odp_sdk/utils/package_utils.py
--rw-r--r--   0        0        0     1172 2024-04-19 13:36:46.348672 odp_sdk-0.4.8/pyproject.toml
--rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 odp_sdk-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0     1052 2024-04-23 12:13:47.307722 odp_sdk-0.4.9/LICENSE
+-rw-r--r--   0        0        0      836 2024-04-23 12:13:47.307722 odp_sdk-0.4.9/README.md
+-rw-r--r--   0        0        0       30 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/__init__.py
+-rw-r--r--   0        0        0    12698 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/auth.py
+-rw-r--r--   0        0        0     1941 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/client.py
+-rw-r--r--   0        0        0       84 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/dto/__init__.py
+-rw-r--r--   0        0        0      856 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/dto/file_dto.py
+-rw-r--r--   0        0        0     1938 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/dto/resource_dto.py
+-rw-r--r--   0        0        0      846 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/dto/table_spec.py
+-rw-r--r--   0        0        0     1391 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/dto/tabular_store.py
+-rw-r--r--   0        0        0     1012 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/exc.py
+-rw-r--r--   0        0        0     7933 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/http_client.py
+-rw-r--r--   0        0        0     8303 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/raw_storage_client.py
+-rw-r--r--   0        0        0     6759 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/resource_client.py
+-rw-r--r--   0        0        0    17200 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/tabular_storage_client.py
+-rw-r--r--   0        0        0       39 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/utils/__init__.py
+-rw-r--r--   0        0        0     1789 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/utils/json.py
+-rw-r--r--   0        0        0     4273 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/utils/ndjson.py
+-rw-r--r--   0        0        0      170 2024-04-23 12:13:47.311723 odp_sdk-0.4.9/odp_sdk/utils/package_utils.py
+-rw-r--r--   0        0        0     1172 2024-04-23 12:14:07.787859 odp_sdk-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0     1618 1970-01-01 00:00:00.000000 odp_sdk-0.4.9/PKG-INFO
```

### Comparing `odp_sdk-0.4.8/LICENSE` & `odp_sdk-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/README.md` & `odp_sdk-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/auth.py` & `odp_sdk-0.4.9/odp_sdk/auth.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/client.py` & `odp_sdk-0.4.9/odp_sdk/client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/dto/file_dto.py` & `odp_sdk-0.4.9/odp_sdk/dto/file_dto.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/dto/resource_dto.py` & `odp_sdk-0.4.9/odp_sdk/dto/resource_dto.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/dto/table_spec.py` & `odp_sdk-0.4.9/odp_sdk/dto/table_spec.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/dto/tabular_store.py` & `odp_sdk-0.4.9/odp_sdk/dto/tabular_store.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/exc.py` & `odp_sdk-0.4.9/odp_sdk/exc.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/http_client.py` & `odp_sdk-0.4.9/odp_sdk/http_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/raw_storage_client.py` & `odp_sdk-0.4.9/odp_sdk/raw_storage_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/resource_client.py` & `odp_sdk-0.4.9/odp_sdk/resource_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/tabular_storage_client.py` & `odp_sdk-0.4.9/odp_sdk/tabular_storage_client.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/utils/json.py` & `odp_sdk-0.4.9/odp_sdk/utils/json.py`

 * *Files identical despite different names*

### Comparing `odp_sdk-0.4.8/odp_sdk/utils/ndjson.py` & `odp_sdk-0.4.9/odp_sdk/utils/ndjson.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import json
 from collections import deque
-from io import BytesIO, StringIO
+from io import StringIO
 from typing import IO, Deque, Iterable, Optional, cast
 from warnings import warn
 
 from .json import JsonParser, JsonType
 
 DEFAULT_JSON_PARSER = cast(JsonParser, json)
 
@@ -25,62 +25,65 @@
 
         Args:
             s: String to parse, either this or 'fp' must be set
             fp: File-like object to parse, either this or 's' must be set
             json_parser: JSON parser to use, defaults to the standard `json` module
         """
         self.json_parser = json_parser
-        self.line = ""
+        self.line = []
         self.delimiter_stack: Deque[str] = deque()
 
         if s and fp:
             raise ValueError("Either 's' or 'fp' must be set, but now both")
         elif not s and not fp:
             raise ValueError("Either 's' or 'fp' must be set")
 
-        self.fb = fp if fp else (StringIO(s) if isinstance(s, str) else BytesIO(s))
+        if fp:
+            self.fb = fp
+        elif isinstance(s, str):
+            self.fb = StringIO(s)
+        else:
+            self.fb = StringIO(s.decode())
 
     def _consume_line(self) -> JsonType:
         """Consume a line from the file-like object
 
         Returns:
             Parsed JSON object
         """
         if self.delimiter_stack:
             warn("Attempting to parse NDJSON line while the delimiter stack was non-empty")
 
-        obj = self.json_parser.loads(self.line)
-        self.line = ""
+        obj = self.json_parser.loads("".join(self.line))
+        self.line = []
         self.delimiter_stack.clear()
 
         return obj
 
     def __iter__(self) -> Iterable[JsonType]:
         return cast(Iterable[JsonType], self)
 
     def __next__(self) -> JsonType:
         while True:
             try:
                 s = next(self.fb)
             except StopIteration:
-                if self.line:
+                if len(self.line) > 0:
                     return self._consume_line()
                 raise
 
             for c in s:
-                if isinstance(c, int):
-                    c = chr(c)
                 last_delimiter = self.delimiter_stack[-1] if self.delimiter_stack else None
 
                 in_quote = last_delimiter in {"'", '"', "\\"}
 
                 if c == "\n" and not in_quote:
                     return self._consume_line()
 
-                self.line += c
+                self.line.append(c)
                 if in_quote:
                     if last_delimiter == "\\":
                         self.delimiter_stack.pop()
                     elif c == "\\":
                         self.delimiter_stack.append(c)
                     elif c == last_delimiter:
                         self.delimiter_stack.pop()
```

### Comparing `odp_sdk-0.4.8/pyproject.toml` & `odp_sdk-0.4.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odp-sdk"
-version = "0.4.8"
+version = "0.4.9"
 description = "ODP Python SDK"
 authors = ["Thomas Li Fredriksen <thomas.fredriksen@oceandata.earth>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "odp_sdk"}]
 
 [tool.poetry.dependencies]
```

### Comparing `odp_sdk-0.4.8/PKG-INFO` & `odp_sdk-0.4.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odp-sdk
-Version: 0.4.8
+Version: 0.4.9
 Summary: ODP Python SDK
 License: MIT
 Author: Thomas Li Fredriksen
 Author-email: thomas.fredriksen@oceandata.earth
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: odp-sdk Version: 0.4.8 Summary: ODP Python SDK
+Metadata-Version: 2.1 Name: odp-sdk Version: 0.4.9 Summary: ODP Python SDK
 License: MIT Author: Thomas Li Fredriksen Author-email:
 thomas.fredriksen@oceandata.earth Requires-Python: >=3.10,<4.0 Classifier:
 License :: OSI Approved :: MIT License Classifier: Programming Language ::
 Python :: 3 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Provides-Extra: pandas Requires-Dist: cryptography
 (>=41.0.5,<43.0.0) Requires-Dist: msal (>=1.24.1,<2.0.0) Requires-Dist: msal-
```

