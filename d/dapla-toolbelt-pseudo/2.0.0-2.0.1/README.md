# Comparing `tmp/dapla_toolbelt_pseudo-2.0.0.tar.gz` & `tmp/dapla_toolbelt_pseudo-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-2.0.0.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-2.0.1.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-2.0.0.tar` & `dapla_toolbelt_pseudo-2.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2024-05-16 07:20:09.574995 dapla_toolbelt_pseudo-2.0.0/LICENSE
--rw-r--r--   0        0        0    18193 2024-05-16 07:20:09.574995 dapla_toolbelt_pseudo-2.0.0/README.md
--rw-r--r--   0        0        0     4936 2024-05-16 07:20:18.702990 dapla_toolbelt_pseudo-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     1455 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1938 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      766 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0    11244 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      555 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    11313 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/baseclasses.py
--rw-r--r--   0        0        0     5851 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0     8255 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0     2945 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/api.py
--rw-r--r--   0        0        0    10591 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/core.py
--rw-r--r--   0        0        0     5419 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/mutable_dataframe.py
--rw-r--r--   0        0        0     8797 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0    12681 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0    10268 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4451 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5603 2024-05-16 07:20:09.578995 dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    19723 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-22 08:14:05.770042 dapla_toolbelt_pseudo-2.0.1/LICENSE
+-rw-r--r--   0        0        0    18193 2024-05-22 08:14:05.770042 dapla_toolbelt_pseudo-2.0.1/README.md
+-rw-r--r--   0        0        0     4936 2024-05-22 08:14:19.678177 dapla_toolbelt_pseudo-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1455 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1938 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      766 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0    11244 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      555 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    11313 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/baseclasses.py
+-rw-r--r--   0        0        0     5851 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0     8255 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0     2945 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/models/api.py
+-rw-r--r--   0        0        0    10591 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/models/core.py
+-rw-r--r--   0        0        0     5654 2024-05-22 08:14:19.678177 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/mutable_dataframe.py
+-rw-r--r--   0        0        0     8797 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0    12681 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0    10268 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4451 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5603 2024-05-22 08:14:05.774042 dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    19723 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-2.0.1/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-2.0.0/LICENSE` & `dapla_toolbelt_pseudo-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/README.md` & `dapla_toolbelt_pseudo-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/pyproject.toml` & `dapla_toolbelt_pseudo-2.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "2.0.0"
+version = "2.0.1"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/types.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/baseclasses.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/baseclasses.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/client.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/depseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/api.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/models/api.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/models/core.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/models/core.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/mutable_dataframe.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/mutable_dataframe.py`

 * *Files 10% similar despite different names*

```diff
@@ -113,15 +113,18 @@
     rules: list[tuple[PseudoRule, PseudoRule | None]],
     metrics: Counter[str],
     prefix: str = "",
 ) -> t.Generator[FieldMatch, None, None]:
     for index, col in enumerate(items):
         if col is None:
             continue
-        elif isinstance(col.get("datatype"), dict):
+
+        # Ignoring mypy error for dict key check in the second condition,
+        # since we know the dict exists in the first condition
+        elif isinstance(col.get("datatype"), dict) and ("Struct" in col.get("datatype") or "List" in col.get("datatype")):  # type: ignore[operator]
             next_prefix = (
                 f"{prefix}[{index}]" if col["name"] == "" else f"{prefix}/{col['name']}"
             )
             yield from _traverse_dataframe_dict(
                 col["values"], rules, metrics, next_prefix
             )
         elif len(col["values"]) > 0 and any(v is not None for v in col["values"]):
```

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/pseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/repseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/result.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-2.0.1/src/dapla_pseudo/v1/validation.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-2.0.0/PKG-INFO` & `dapla_toolbelt_pseudo-2.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 2.0.0
+Version: 2.0.1
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
```

