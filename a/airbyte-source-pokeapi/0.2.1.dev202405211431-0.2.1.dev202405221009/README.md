# Comparing `tmp/airbyte_source_pokeapi-0.2.1.dev202405211431.tar.gz` & `tmp/airbyte_source_pokeapi-0.2.1.dev202405221009.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_pokeapi-0.2.1.dev202405211431.tar", max compression
+gzip compressed data, was "airbyte_source_pokeapi-0.2.1.dev202405221009.tar", max compression
```

## Comparing `airbyte_source_pokeapi-0.2.1.dev202405211431.tar` & `airbyte_source_pokeapi-0.2.1.dev202405221009.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     4527 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/README.md
--rw-r--r--   0        0        0      135 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/main.py
--rw-r--r--   0        0        0      777 2024-05-21 14:31:33.486392 airbyte_source_pokeapi-0.2.1.dev202405211431/pyproject.toml
--rw-r--r--   0        0        0      126 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/__init__.py
--rw-r--r--   0        0        0    29310 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/manifest.yaml
--rw-r--r--   0        0        0      227 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/run.py
--rw-r--r--   0        0        0      476 2024-05-21 12:17:11.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/source.py
--rw-r--r--   0        0        0     5248 1970-01-01 00:00:00.000000 airbyte_source_pokeapi-0.2.1.dev202405211431/PKG-INFO
+-rw-r--r--   0        0        0     4527 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/README.md
+-rw-r--r--   0        0        0      135 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/main.py
+-rw-r--r--   0        0        0      777 2024-05-22 10:09:55.122528 airbyte_source_pokeapi-0.2.1.dev202405221009/pyproject.toml
+-rw-r--r--   0        0        0      126 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/source_pokeapi/__init__.py
+-rw-r--r--   0        0        0    29310 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/source_pokeapi/manifest.yaml
+-rw-r--r--   0        0        0      227 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/source_pokeapi/run.py
+-rw-r--r--   0        0        0      476 2024-05-22 10:05:34.976315 airbyte_source_pokeapi-0.2.1.dev202405221009/source_pokeapi/source.py
+-rw-r--r--   0        0        0     5248 1970-01-01 00:00:00.000000 airbyte_source_pokeapi-0.2.1.dev202405221009/PKG-INFO
```

### Comparing `airbyte_source_pokeapi-0.2.1.dev202405211431/README.md` & `airbyte_source_pokeapi-0.2.1.dev202405221009/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_pokeapi-0.2.1.dev202405211431/pyproject.toml` & `airbyte_source_pokeapi-0.2.1.dev202405221009/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.1.dev202405211431"
+version = "0.2.1.dev202405221009"
 name = "airbyte-source-pokeapi"
 description = "Source implementation for pokeapi."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_pokeapi-0.2.1.dev202405211431/source_pokeapi/manifest.yaml` & `airbyte_source_pokeapi-0.2.1.dev202405221009/source_pokeapi/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_pokeapi-0.2.1.dev202405211431/PKG-INFO` & `airbyte_source_pokeapi-0.2.1.dev202405221009/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-pokeapi
-Version: 0.2.1.dev202405211431
+Version: 0.2.1.dev202405221009
 Summary: Source implementation for pokeapi.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

