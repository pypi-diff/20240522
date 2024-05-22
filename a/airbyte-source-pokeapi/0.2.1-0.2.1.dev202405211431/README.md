# Comparing `tmp/airbyte_source_pokeapi-0.2.1.tar.gz` & `tmp/airbyte_source_pokeapi-0.2.1.dev202405211431.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pokeapi-0.2.1.tar", max compression
+gzip compressed data, was "airbyte_source_pokeapi-0.2.1.dev202405211431.tar", max compression
```

## Comparing `airbyte_source_pokeapi-0.2.1.tar` & `airbyte_source_pokeapi-0.2.1.dev202405211431.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4527 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/README.md
--rw-r--r--   0        0        0      135 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/main.py
--rw-r--r--   0        0        0      761 2024-05-15 15:25:43.988231 airbyte_source_pokeapi-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/__init__.py
--rw-r--r--   0        0        0    29310 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/run.py
--rw-r--r--   0        0        0      476 2024-05-15 15:20:55.530777 airbyte_source_pokeapi-0.2.1/source_pokeapi/source.py
--rw-r--r--   0        0        0     5232 1970-01-01 00:00:00.000000 airbyte_source_pokeapi-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     4527 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/README.md
+-rw-r--r--   0        0        0      135 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/main.py
+-rw-r--r--   0        0        0      777 2024-05-21 14:31:33.486392 airbyte_source_pokeapi-0.2.1.dev202405211431/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/__init__.py
+-rw-r--r--   0        0        0    29310 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/run.py
+-rw-r--r--   0        0        0      476 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/source.py
+-rw-r--r--   0        0        0     5248 1970-01-01 00:00:00.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/PKG-INFO
```

### Comparing `airbyte_source_pokeapi-0.2.1/README.md` & `airbyte_source_pokeapi-0.2.1.dev202405211431/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_pokeapi-0.2.1/pyproject.toml` & `airbyte_source_pokeapi-0.2.1.dev202405211431/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.1"
+version = "0.2.1.dev202405211431"
 name = "airbyte-source-pokeapi"
 description = "Source implementation for pokeapi."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_pokeapi-0.2.1/source_pokeapi/manifest.yaml` & `airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_pokeapi-0.2.1/PKG-INFO` & `airbyte_source_pokeapi-0.2.1.dev202405211431/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pokeapi
-Version: 0.2.1
+Version: 0.2.1.dev202405211431
 Summary: Source implementation for pokeapi.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

