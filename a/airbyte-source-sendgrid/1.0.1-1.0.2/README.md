# Comparing `tmp/airbyte_source_sendgrid-1.0.1.tar.gz` & `tmp/airbyte_source_sendgrid-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "airbyte_source_sendgrid-1.0.1.tar", max compression
+gzip compressed data, was "airbyte_source_sendgrid-1.0.2.tar", max compression
```

## Comparing `airbyte_source_sendgrid-1.0.1.tar` & `airbyte_source_sendgrid-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     4547 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/README.md
--rw-r--r--   0        0        0      770 2024-05-20 18:15:15.688460 airbyte_source_sendgrid-1.0.1/pyproject.toml
--rw-r--r--   0        0        0       65 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/__init__.py
--rw-r--r--   0        0        0     3498 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/config_migrations.py
--rw-r--r--   0        0        0    25729 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/manifest.yaml
--rw-r--r--   0        0        0      362 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/run.py
--rw-r--r--   0        0        0     1362 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/schemas/contacts.json
--rw-r--r--   0        0        0      998 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/source.py
--rw-r--r--   0        0        0     8694 2024-05-20 04:01:28.000000 airbyte_source_sendgrid-1.0.1/source_sendgrid/streams.py
--rw-r--r--   0        0        0     5294 1970-01-01 00:00:00.000000 airbyte_source_sendgrid-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     4547 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/README.md
+-rw-r--r--   0        0        0      770 2024-05-22 15:15:52.361138 airbyte_source_sendgrid-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0       65 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/__init__.py
+-rw-r--r--   0        0        0     3498 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/config_migrations.py
+-rw-r--r--   0        0        0    25729 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/manifest.yaml
+-rw-r--r--   0        0        0      362 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/run.py
+-rw-r--r--   0        0        0     1362 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/schemas/contacts.json
+-rw-r--r--   0        0        0     1014 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/source.py
+-rw-r--r--   0        0        0     8679 2024-05-22 14:54:34.000000 airbyte_source_sendgrid-1.0.2/source_sendgrid/streams.py
+-rw-r--r--   0        0        0     5294 1970-01-01 00:00:00.000000 airbyte_source_sendgrid-1.0.2/PKG-INFO
```

### Comparing `airbyte_source_sendgrid-1.0.1/README.md` & `airbyte_source_sendgrid-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `airbyte_source_sendgrid-1.0.1/pyproject.toml` & `airbyte_source_sendgrid-1.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
     "poetry-core>=1.0.0",
 ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
-version = "1.0.1"
+version = "1.0.2"
 name = "airbyte-source-sendgrid"
 description = "Source implementation for Sendgrid."
 authors = [
     "Airbyte <contact@airbyte.io>",
 ]
 license = "MIT"
 readme = "README.md"
```

### Comparing `airbyte_source_sendgrid-1.0.1/source_sendgrid/config_migrations.py` & `airbyte_source_sendgrid-1.0.2/source_sendgrid/config_migrations.py`

 * *Files identical despite different names*

### Comparing `airbyte_source_sendgrid-1.0.1/source_sendgrid/manifest.yaml` & `airbyte_source_sendgrid-1.0.2/source_sendgrid/manifest.yaml`

 * *Files identical despite different names*

### Comparing `airbyte_source_sendgrid-1.0.1/source_sendgrid/schemas/contacts.json` & `airbyte_source_sendgrid-1.0.2/source_sendgrid/schemas/contacts.json`

 * *Files identical despite different names*

### Comparing `airbyte_source_sendgrid-1.0.1/source_sendgrid/source.py` & `airbyte_source_sendgrid-1.0.2/source_sendgrid/source.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # Copyright (c) 2023 Airbyte, Inc., all rights reserved.
 #
 
 from typing import Any, List, Mapping
 
 from airbyte_cdk.sources.declarative.yaml_declarative_source import YamlDeclarativeSource
 from airbyte_cdk.sources.streams import Stream
-from airbyte_cdk.sources.streams.http.auth import TokenAuthenticator
+from airbyte_cdk.sources.streams.http.requests_native_auth import TokenAuthenticator
 
 from .streams import Contacts
 
 
 # Hybrid Declarative Source
 class SourceSendgrid(YamlDeclarativeSource):
     def __init__(self):
```

### Comparing `airbyte_source_sendgrid-1.0.1/source_sendgrid/streams.py` & `airbyte_source_sendgrid-1.0.2/source_sendgrid/streams.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,15 +54,15 @@
     encoding = "utf-8"
 
     def path(self, **kwargs) -> str:
         return "v3/marketing/contacts/exports"
 
     @default_backoff_handler(max_tries=5, factor=15)
     def _send_http_request(self, method: str, url: str, stream: bool = False, enable_auth: bool = True):
-        headers = self.authenticator.get_auth_header() if enable_auth else None
+        headers = self._session.auth.get_auth_header() if enable_auth else None
         response = self._session.request(method, url=url, headers=headers, stream=stream)
         if response.status_code not in [200, 202]:
             self.logger.error(f"error body: {response.text}")
         response.raise_for_status()
         return response
 
     def read_records(
@@ -155,17 +155,16 @@
         Return the tuple containing string with file path of downloaded binary data (Saved temporarily) and file encoding.
         """
         # set filepath for binary data from response
         decompressor = zlib.decompressobj(zlib.MAX_WBITS | 32)
 
         url_parsed = urlparse(url)
         tmp_file = os.path.realpath(os.path.basename(url_parsed.path[1:-5]))
-        with closing(self._send_http_request("GET", f"{url}", stream=True, enable_auth=False)) as response, open(
-            tmp_file, "wb"
-        ) as data_file:
+        download_session = requests.get(f"{url}", stream=True)
+        with closing(download_session) as response, open(tmp_file, "wb") as data_file:
             for chunk in response.iter_content(chunk_size=chunk_size):
                 try:
                     # see if it's compressed. we are seeing some that are not all of a sudden.
                     # but let's also guard against the case where sendgrid changes it back.
                     data_file.write(decompressor.decompress(chunk))
                 except zlib.error as e:
                     # it's not actually compressed!
```

### Comparing `airbyte_source_sendgrid-1.0.1/PKG-INFO` & `airbyte_source_sendgrid-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airbyte-source-sendgrid
-Version: 1.0.1
+Version: 1.0.2
 Summary: Source implementation for Sendgrid.
 Home-page: https://airbyte.com
 License: MIT
 Author: Airbyte
 Author-email: contact@airbyte.io
 Requires-Python: >=3.9,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

