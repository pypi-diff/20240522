# Comparing `tmp/snakemake_storage_plugin_sharepoint-0.3.0.tar.gz` & `tmp/snakemake_storage_plugin_sharepoint-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.3.0.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_sharepoint-0.4.0.tar", max compression
```

## Comparing `snakemake_storage_plugin_sharepoint-0.3.0.tar` & `snakemake_storage_plugin_sharepoint-0.4.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1058 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/LICENSE
--rw-r--r--   0        0        0      292 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/README.md
--rw-r--r--   0        0        0      958 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      322 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/__init__.py
--rw-r--r--   0        0        0     7364 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/object.py
--rw-r--r--   0        0        0     4023 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/provider.py
--rw-r--r--   0        0        0     4190 2024-05-03 18:54:45.799045 snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/settings.py
--rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1058 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/LICENSE
+-rw-r--r--   0        0        0      292 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/README.md
+-rw-r--r--   0        0        0      958 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      322 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/__init__.py
+-rw-r--r--   0        0        0     9132 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/object.py
+-rw-r--r--   0        0        0     6501 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/provider.py
+-rw-r--r--   0        0        0     4199 2024-05-21 19:45:18.943494 snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/settings.py
+-rw-r--r--   0        0        0     1260 1970-01-01 00:00:00.000000 snakemake_storage_plugin_sharepoint-0.4.0/PKG-INFO
```

### Comparing `snakemake_storage_plugin_sharepoint-0.3.0/LICENSE` & `snakemake_storage_plugin_sharepoint-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_sharepoint-0.3.0/pyproject.toml` & `snakemake_storage_plugin_sharepoint-0.4.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-sharepoint"
-version = "0.3.0"
+version = "0.4.0"
 description = "Snakemake storage plugin for reading and writing files on Microsoft SharePoint."
 authors = [
     "Hugo Lapre <hugo.lapre@brabantwater.nl>",
 ]
 readme = "README.md"
 repository = "https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/sharepoint.html"
```

### Comparing `snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/object.py` & `snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/object.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 # Required:
 # Implementation of storage object (also check out
 # snakemake_interface_storage_plugins.storage_object for more base class options)
+import dataclasses
 import datetime
+import urllib.parse as urlparse
 from contextlib import contextmanager
 from functools import partial
 from typing import TYPE_CHECKING, Any, Generator, Literal, Optional
-from urllib.parse import urlparse
 
 import requests
 from snakemake_interface_common.exceptions import WorkflowError
 from snakemake_interface_common.logging import get_logger
 from snakemake_interface_storage_plugins.io import IOCacheStorageInterface, Mtime
 from snakemake_interface_storage_plugins.storage_object import (
     StorageObjectRead,
@@ -22,14 +23,21 @@
 
 __all__ = ["StorageObject"]
 
 HTTPVerb = Literal["GET", "POST", "HEAD"]
 logger = get_logger()
 
 
+@dataclasses.dataclass
+class QueryParseResult:
+    library: str
+    filepath: str
+    overwrite: Optional[bool]
+
+
 class StorageObject(StorageObjectRead, StorageObjectWrite):
     DIGEST_URL = "{site_url}/_api/contextinfo"
     GET_FILE_URL = (
         "{site_url}/_api/web/GetFolderByServerRelativeUrl('{folder}')/"
         "Files('{filename}')"
     )
     DOWNLOAD_FILE_URL = (
@@ -56,23 +64,53 @@
         self.library: str
         self.filepath: str
         super().__init__(query, keep_local, retrieve, provider)
 
     def __post_init__(self):
         if (site_url := self.provider.settings.site_url) is None:
             raise WorkflowError("No site URL specified")
-        parsed_site = urlparse(site_url)
+        parsed_site = urlparse.urlparse(site_url)
         self.site_url = site_url.rstrip("/")
         self.site_netloc = parsed_site.netloc
 
-        parsed_query = urlparse(self.query)
-        self.library = parsed_query.netloc
-        self.filepath = parsed_query.path.lstrip("/")
-
-        self.allow_overwrite = self.provider.settings.allow_overwrite or False
+        parsed_query = self.parse_query(self.query)
+        self.library = parsed_query.library
+        self.filepath = parsed_query.filepath
+        self.set_overwrite(parsed_query.overwrite)
+
+    def set_overwrite(self, overwrite: Optional[bool]) -> None:
+        match self.provider.settings.allow_overwrite:
+            case False:
+                self.allow_overwrite = False
+            case True:
+                self.allow_overwrite = overwrite or True
+            case _:
+                self.allow_overwrite = overwrite or False
+
+    @classmethod
+    def parse_query(cls, query: str) -> QueryParseResult:
+        parsed_query = urlparse.urlparse(query)
+        querystring = urlparse.parse_qs(parsed_query.query, keep_blank_values=True)
+        overwrite_string = querystring.get("overwrite", ["none"])[0].lower()
+        match overwrite_string:
+            case "true":
+                overwrite = True
+            case "":
+                overwrite = True
+            case "false":
+                overwrite = False
+            case "none":
+                overwrite = None
+            case _:
+                raise WorkflowError(f"Invalid overwrite value: {overwrite_string}")
+        return QueryParseResult(
+            library=parsed_query.netloc,
+            filepath=parsed_query.path.lstrip("/"),
+            overwrite=overwrite,
+        )
 
     async def inventory(self, cache: IOCacheStorageInterface):
         """From this file, try to find as much existence and modification date
         information as possible. Only retrieve that information that comes for free
         given the current object.
         """
         with self.httpr(self.GET_FILE_URL) as r:
@@ -112,36 +150,47 @@
     # The type: ignore is necessary because the return type is not compatible with the
     # base class:
     # https://github.com/snakemake/snakemake-interface-storage-plugins/pull/48
     def local_suffix(self) -> str:  # type: ignore
         return "/".join([self.site_netloc, self.library, self.filepath])
 
     def store_object(self):
+        logger.debug("Getting form digest value")
         with self.httpr(self.DIGEST_URL, "POST") as r:
             try:
                 r.raise_for_status()
             except requests.HTTPError as e:
                 raise WorkflowError(
                     f"Failed to get form digest value for {self.query}"
                 ) from e
 
             digest_value = r.json()["d"]["GetContextWebInformation"]["FormDigestValue"]
 
         headers = {"x-requestdigest": digest_value}
 
+        logger.info(f"Uploading {self.query}")
         with open(self.local_path(), "rb") as file:
             with self.httpr(
                 self.UPLOAD_FILE_URL, "POST", headers=headers, data=file.read()
             ) as r:
                 try:
                     r.raise_for_status()
                 except requests.HTTPError as e:
-                    raise WorkflowError(f"Failed to store {self.query}") from e
+                    en_dis_abled = (
+                        "enabled"
+                        if self.allow_overwrite
+                        else "disabled, allow by adding ?overwrite to the query"
+                    )
+                    raise WorkflowError(
+                        f"Failed to store {self.query} "
+                        f"(overwrite is {en_dis_abled})"
+                    ) from e
 
     def remove(self):
+        logger.debug(f"Removing {self.query} is not implemented.")
         pass
 
     @contextmanager  # makes this a context manager. after 'yield' is __exit__()
     def httpr(
         self,
         url: str,
         verb: HTTPVerb = "GET",
```

### Comparing `snakemake_storage_plugin_sharepoint-0.3.0/snakemake_storage_plugin_sharepoint/settings.py` & `snakemake_storage_plugin_sharepoint-0.4.0/snakemake_storage_plugin_sharepoint/settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,16 +106,16 @@
     site_url: Optional[str] = dataclasses.field(
         default=None,
         metadata={
             "help": "The URL of the SharePoint site.",
             "env_var": True,
         },
     )
-    allow_overwrite: bool = dataclasses.field(
-        default=False,
+    allow_overwrite: Optional[bool] = dataclasses.field(
+        default=None,
         metadata={
             "help": "Allow overwriting files in the SharePoint site.",
         },
     )
     upload_timeout: int = dataclasses.field(
         default=1000,
         metadata={
```

### Comparing `snakemake_storage_plugin_sharepoint-0.3.0/PKG-INFO` & `snakemake_storage_plugin_sharepoint-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-sharepoint
-Version: 0.3.0
+Version: 0.4.0
 Summary: Snakemake storage plugin for reading and writing files on Microsoft SharePoint.
 Home-page: https://github.com/Hugovdberg/snakemake-storage-plugin-sharepoint
 License: MIT
 Keywords: snakemake,plugin,storage,sharepoint
 Author: Hugo Lapre
 Author-email: hugo.lapre@brabantwater.nl
 Requires-Python: >=3.11,<4.0
```

