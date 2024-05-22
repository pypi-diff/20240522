# Comparing `tmp/airbyte_source_confluence-0.2.4.tar.gz` & `tmp/airbyte_source_confluence-0.2.4.dev202405221558.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_confluence-0.2.4.tar", max compression
+gzip compressed data, was "airbyte_source_confluence-0.2.4.dev202405221558.tar", max compression
```

## Comparing `airbyte_source_confluence-0.2.4.tar` & `airbyte_source_confluence-0.2.4.dev202405221558.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     4578 2024-05-15 15:22:17.086657 airbyte_source_confluence-0.2.4/README.md
--rw-r--r--   0        0        0      789 2024-05-15 15:27:07.098837 airbyte_source_confluence-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      132 2024-05-15 15:22:17.086657 airbyte_source_confluence-0.2.4/source_confluence/__init__.py
--rw-r--r--   0        0        0    29838 2024-05-15 15:22:17.086657 airbyte_source_confluence-0.2.4/source_confluence/manifest.yaml
--rw-r--r--   0        0        0      242 2024-05-15 15:22:17.086657 airbyte_source_confluence-0.2.4/source_confluence/run.py
--rw-r--r--   0        0        0      479 2024-05-15 15:22:17.086657 airbyte_source_confluence-0.2.4/source_confluence/source.py
--rw-r--r--   0        0        0     5294 1970-01-01 00:00:00.000000 airbyte_source_confluence-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     4578 2024-05-22 15:54:18.039982 airbyte_source_confluence-0.2.4.dev202405221558/README.md
+-rw-r--r--   0        0        0      801 2024-05-22 15:58:25.261827 airbyte_source_confluence-0.2.4.dev202405221558/pyproject.toml
+-rw-r--r--   0        0        0      132 2024-05-22 15:54:18.043982 airbyte_source_confluence-0.2.4.dev202405221558/source_confluence/__init__.py
+-rw-r--r--   0        0        0    29833 2024-05-22 15:54:18.043982 airbyte_source_confluence-0.2.4.dev202405221558/source_confluence/manifest.yaml
+-rw-r--r--   0        0        0      242 2024-05-22 15:54:18.043982 airbyte_source_confluence-0.2.4.dev202405221558/source_confluence/run.py
+-rw-r--r--   0        0        0      479 2024-05-22 15:54:18.043982 airbyte_source_confluence-0.2.4.dev202405221558/source_confluence/source.py
+-rw-r--r--   0        0        0     5308 1970-01-01 00:00:00.000000 airbyte_source_confluence-0.2.4.dev202405221558/PKG-INFO
```

### Comparing `airbyte_source_confluence-0.2.4/README.md` & `airbyte_source_confluence-0.2.4.dev202405221558/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_confluence-0.2.4/pyproject.toml` & `airbyte_source_confluence-0.2.4.dev202405221558/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "0.2.4"
+version = "0.2.4.dev202405221558"
 name = "airbyte-source-confluence"
 description = "Source implementation for Confluence."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
@@ -18,15 +18,15 @@
 repository = "https://github.com/airbytehq/airbyte"
 packages = [
     { include = "source_confluence" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9,<3.12"
-airbyte-cdk = "0.80.0"
+airbyte-cdk = "^0"
 
 [tool.poetry.scripts]
 source-confluence = "source_confluence.run:run"
 
 [tool.poetry.group.dev.dependencies]
 requests-mock = "^1.9.3"
 pytest-mock = "^3.6.1"
```

### Comparing `airbyte_source_confluence-0.2.4/source_confluence/manifest.yaml` & `airbyte_source_confluence-0.2.4.dev202405221558/source_confluence/manifest.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             field_name: start
           page_size_option:
             type: RequestOption
             inject_into: request_parameter
             field_name: limit
           pagination_strategy:
             type: OffsetIncrement
-            page_size: 25
+            page_size: 2
       schema_loader:
         type: InlineSchemaLoader
         schema:
           $ref: "#/schemas/audit"
     blog_posts:
       type: DeclarativeStream
       name: blog_posts
@@ -71,15 +71,15 @@
             field_name: start
           page_size_option:
             type: RequestOption
             inject_into: request_parameter
             field_name: limit
           pagination_strategy:
             type: OffsetIncrement
-            page_size: 25
+            page_size: 2
       schema_loader:
         type: InlineSchemaLoader
         schema:
           $ref: "#/schemas/blog_posts"
     group:
       type: DeclarativeStream
       name: group
@@ -105,15 +105,15 @@
             field_name: start
           page_size_option:
             type: RequestOption
             inject_into: request_parameter
             field_name: limit
           pagination_strategy:
             type: OffsetIncrement
-            page_size: 25
+            page_size: 3
       schema_loader:
         type: InlineSchemaLoader
         schema:
           $ref: "#/schemas/group"
     pages:
       type: DeclarativeStream
       name: pages
@@ -142,15 +142,15 @@
             field_name: start
           page_size_option:
             type: RequestOption
             inject_into: request_parameter
             field_name: limit
           pagination_strategy:
             type: OffsetIncrement
-            page_size: 25
+            page_size: 2
       schema_loader:
         type: InlineSchemaLoader
         schema:
           $ref: "#/schemas/pages"
     space:
       type: DeclarativeStream
       name: space
@@ -178,15 +178,15 @@
             field_name: start
           page_size_option:
             type: RequestOption
             inject_into: request_parameter
             field_name: limit
           pagination_strategy:
             type: OffsetIncrement
-            page_size: 25
+            page_size: 2
       schema_loader:
         type: InlineSchemaLoader
         schema:
           $ref: "#/schemas/space"
   base_requester:
     type: HttpRequester
     url_base: https://{{ config['domain_name'] }}/wiki/rest/api/
```

### Comparing `airbyte_source_confluence-0.2.4/PKG-INFO` & `airbyte_source_confluence-0.2.4.dev202405221558/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: airbyte-source-confluence
-Version: 0.2.4
+Version: 0.2.4.dev202405221558
 Summary: Source implementation for Confluence.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: airbyte-cdk (==0.80.0)
+Requires-Dist: airbyte-cdk (>=0,<1)
 Project-URL: Documentation, https://docs.airbyte.com/integrations/sources/confluence
 Project-URL: Repository, https://github.com/airbytehq/airbyte
 Description-Content-Type: text/markdown
 
 # Confluence source connector
 
 This is the repository for the Confluence source connector, written in Python.
```

