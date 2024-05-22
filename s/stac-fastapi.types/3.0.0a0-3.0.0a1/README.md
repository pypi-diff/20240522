# Comparing `tmp/stac_fastapi_types-3.0.0a0.tar.gz` & `tmp/stac_fastapi_types-3.0.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stac_fastapi_types-3.0.0a0.tar", last modified: Mon May  6 16:07:31 2024, max compression
+gzip compressed data, was "stac_fastapi_types-3.0.0a1.tar", last modified: Wed May 22 11:03:57 2024, max compression
```

## Comparing `stac_fastapi_types-3.0.0a0.tar` & `stac_fastapi_types-3.0.0a1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.234578 stac_fastapi_types-3.0.0a0/stac_fastapi/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.234578 stac_fastapi_types-3.0.0a0/stac_fastapi/types/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/conformance.py
--rw-r--r--   0 runner    (1001) docker     (127)    24819 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/links.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3729 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/rfc3339.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/stac.py
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/stac_fastapi/types/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1376 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-06 16:07:31.000000 stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-06 16:07:31.238577 stac_fastapi_types-3.0.0a0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/tests/test_limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-05-06 16:07:22.000000 stac_fastapi_types-3.0.0a0/tests/test_rfc3339.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:57.836791 stac_fastapi_types-3.0.0a1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 11:03:57.836791 stac_fastapi_types-3.0.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-05-22 11:03:57.836791 stac_fastapi_types-3.0.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:57.828791 stac_fastapi_types-3.0.0a1/stac_fastapi/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:57.832791 stac_fastapi_types-3.0.0a1/stac_fastapi/types/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1011 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24450 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      886 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3369 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/rfc3339.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/stac.py
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/stac_fastapi/types/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:57.832791 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 11:03:57.000000 stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 11:03:57.832791 stac_fastapi_types-3.0.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      594 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/tests/test_limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4393 2024-05-22 11:03:45.000000 stac_fastapi_types-3.0.0a1/tests/test_rfc3339.py
```

### Comparing `stac_fastapi_types-3.0.0a0/PKG-INFO` & `stac_fastapi_types-3.0.0a1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi>=0.100.0
+Requires-Dist: fastapi-slim
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: pydantic-settings>=2
-Requires-Dist: stac_pydantic>=3
-Requires-Dist: pystac==1.*
+Requires-Dist: stac_pydantic~=3.1
 Requires-Dist: iso8601<2.2.0,>=1.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
```

### Comparing `stac_fastapi_types-3.0.0a0/setup.py` & `stac_fastapi_types-3.0.0a1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,19 +2,18 @@
 
 from setuptools import find_namespace_packages, setup
 
 with open("README.md") as f:
     desc = f.read()
 
 install_requires = [
-    "fastapi>=0.100.0",
+    "fastapi-slim",
     "attrs>=23.2.0",
     "pydantic-settings>=2",
-    "stac_pydantic>=3",
-    "pystac==1.*",
+    "stac_pydantic~=3.1",
     "iso8601>=1.0.2,<2.2.0",
 ]
 
 extra_reqs = {
     "dev": [
         "pytest",
         "pytest-cov",
```

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/config.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/config.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/conformance.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/conformance.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/core.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -376,21 +376,18 @@
             extension_schemas=[],
         )
 
         # Add Queryables link
         if self.extension_is_enabled("FilterExtension"):
             landing_page["links"].append(
                 {
-                    # TODO: replace this with Relations.queryables.value,
-                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/queryables",
-                    # TODO: replace this with MimeTypes.jsonschema,
-                    "type": "application/schema+json",
+                    "rel": Relations.queryables.value,
+                    "type": MimeTypes.jsonschema.value,
                     "title": "Queryables",
                     "href": urljoin(base_url, "queryables"),
-                    "method": "GET",
                 }
             )
 
         # Add Collections links
         collections = self.all_collections(request=kwargs["request"])
 
         for collection in collections["collections"]:
@@ -582,18 +579,16 @@
             extension_schemas=[],
         )
 
         # Add Queryables link
         if self.extension_is_enabled("FilterExtension"):
             landing_page["links"].append(
                 {
-                    # TODO: replace this with Relations.queryables.value,
-                    "rel": "http://www.opengis.net/def/rel/ogc/1.0/queryables",
-                    # TODO: replace this with MimeTypes.jsonschema,
-                    "type": "application/schema+json",
+                    "rel": Relations.queryables.value,
+                    "type": MimeTypes.jsonschema.value,
                     "title": "Queryables",
                     "href": urljoin(base_url, "queryables"),
                     "method": "GET",
                 }
             )
 
         # Add Collections links
```

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/errors.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/errors.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/extension.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/extension.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/links.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/links.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/rfc3339.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/rfc3339.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,29 +2,56 @@
 
 import re
 from datetime import datetime, timezone
 from typing import Optional, Tuple, Union
 
 import iso8601
 from fastapi import HTTPException
-from pystac.utils import datetime_to_str
 
 RFC33339_PATTERN = (
     r"^(\d\d\d\d)\-(\d\d)\-(\d\d)(T|t)(\d\d):(\d\d):(\d\d)([.]\d+)?"
     r"(Z|([-+])(\d\d):(\d\d))$"
 )
 
 DateTimeType = Union[
     datetime,
     Tuple[datetime, datetime],
     Tuple[datetime, None],
     Tuple[None, datetime],
 ]
 
 
+# Borrowed from pystac - https://github.com/stac-utils/pystac/blob/f5e4cf4a29b62e9ef675d4a4dac7977b09f53c8f/pystac/utils.py#L370-L394
+def datetime_to_str(dt: datetime, timespec: str = "auto") -> str:
+    """Converts a :class:`datetime.datetime` instance to an ISO8601 string in the
+    `RFC 3339, section 5.6
+    <https://datatracker.ietf.org/doc/html/rfc3339#section-5.6>`__ format required by
+    the :stac-spec:`STAC Spec <master/item-spec/common-metadata.md#date-and-time>`.
+
+    Args:
+        dt : The datetime to convert.
+        timespec: An optional argument that specifies the number of additional
+            terms of the time to include. Valid options are 'auto', 'hours',
+            'minutes', 'seconds', 'milliseconds' and 'microseconds'. The default value
+            is 'auto'.
+
+    Returns:
+        str: The ISO8601 (RFC 3339) formatted string representing the datetime.
+    """
+    if dt.tzinfo is None:
+        dt = dt.replace(tzinfo=timezone.utc)
+
+    timestamp = dt.isoformat(timespec=timespec)
+    zulu = "+00:00"
+    if timestamp.endswith(zulu):
+        timestamp = f"{timestamp[: -len(zulu)]}Z"
+
+    return timestamp
+
+
 def rfc3339_str_to_datetime(s: str) -> datetime:
     """Convert a string conforming to RFC 3339 to a :class:`datetime.datetime`.
 
     Uses :meth:`iso8601.parse_date` under the hood.
 
     Args:
         s (str) : The string to convert to :class:`datetime.datetime`.
@@ -63,24 +90,25 @@
     if ".." in date_str or not date_str:
         raise ValueError("Invalid date format.")
     return rfc3339_str_to_datetime(date_str)
 
 
 def str_to_interval(interval: Optional[str]) -> Optional[DateTimeType]:
     """
-    Extract a tuple of datetime objects from an interval string defined by the OGC API.
-    The interval can either be a single datetime or a range with start and end datetime.
+    Extract a single datetime object or a tuple of datetime objects from an
+    interval string defined by the OGC API. The interval can either be a
+    single datetime or a range with start and end datetime.
 
     Args:
         interval (Optional[str]): The interval string to convert to datetime objects,
         or None if no datetime is specified.
 
     Returns:
-        Optional[DateTimeType]: A tuple of datetime.datetime objects or
-        None if input is None.
+        Optional[DateTimeType]: A single datetime.datetime object, a tuple of
+        datetime.datetime objects, or None if input is None.
 
     Raises:
         HTTPException: If the string is not valid for various reasons such as being empty,
         having more than one slash, or if date formats are invalid.
     """
     if interval is None:
         return None
@@ -93,14 +121,17 @@
         raise HTTPException(
             status_code=400,
             detail="Interval string contains more than one forward slash.",
         )
 
     try:
         start = parse_single_date(values[0]) if values[0] not in ["..", ""] else None
+        if len(values) == 1:
+            return start
+
         end = (
             parse_single_date(values[1])
             if len(values) > 1 and values[1] not in ["..", ""]
             else None
         )
     except (ValueError, iso8601.ParseError) as e:
         raise HTTPException(status_code=400, detail=str(e))
```

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/search.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/search.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi/types/stac.py` & `stac_fastapi_types-3.0.0a1/stac_fastapi/types/stac.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/PKG-INFO` & `stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stac-fastapi.types
-Version: 3.0.0a0
+Version: 3.0.0a1
 Summary: An implementation of STAC API based on the FastAPI framework.
 Home-page: https://github.com/stac-utils/stac-fastapi
 Author: Arturo Engineering
 Author-email: engineering@arturo.ai
 License: MIT
 Keywords: STAC FastAPI COG
 Classifier: Intended Audience :: Developers
@@ -14,19 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Requires-Dist: fastapi>=0.100.0
+Requires-Dist: fastapi-slim
 Requires-Dist: attrs>=23.2.0
 Requires-Dist: pydantic-settings>=2
-Requires-Dist: stac_pydantic>=3
-Requires-Dist: pystac==1.*
+Requires-Dist: stac_pydantic~=3.1
 Requires-Dist: iso8601<2.2.0,>=1.0.2
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-cov; extra == "dev"
 Requires-Dist: pytest-asyncio; extra == "dev"
 Requires-Dist: pre-commit; extra == "dev"
 Requires-Dist: requests; extra == "dev"
```

### Comparing `stac_fastapi_types-3.0.0a0/stac_fastapi.types.egg-info/SOURCES.txt` & `stac_fastapi_types-3.0.0a1/stac_fastapi.types.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/tests/test_limit.py` & `stac_fastapi_types-3.0.0a1/tests/test_limit.py`

 * *Files identical despite different names*

### Comparing `stac_fastapi_types-3.0.0a0/tests/test_rfc3339.py` & `stac_fastapi_types-3.0.0a1/tests/test_rfc3339.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from datetime import timezone
+from datetime import datetime, timezone
 
 import pytest
 from fastapi import HTTPException
 
 from stac_fastapi.types.rfc3339 import (
     now_in_utc,
     now_to_rfc3339_str,
@@ -82,35 +82,53 @@
 
 @pytest.mark.parametrize("test_input", valid_datetimes)
 def test_parse_valid_str_to_datetime(test_input):
     assert rfc3339_str_to_datetime(test_input)
 
 
 @pytest.mark.parametrize("test_input", invalid_intervals)
-def test_parse_invalid_interval_to_datetime(test_input):
+def test_str_to_interval_with_invalid_interval(test_input):
     with pytest.raises(HTTPException) as exc_info:
         str_to_interval(test_input)
     assert (
         exc_info.value.status_code == 400
-    ), "Should return a 400 status code for invalid intervals"
+    ), "str_to_interval should return a 400 status code for invalid interval"
 
 
-@pytest.mark.parametrize("test_input", valid_intervals)
-def test_parse_valid_interval_to_datetime(test_input):
-    assert str_to_interval(test_input)
+@pytest.mark.parametrize("test_input", invalid_datetimes)
+def test_str_to_interval_with_invalid_datetime(test_input):
+    with pytest.raises(HTTPException) as exc_info:
+        str_to_interval(test_input)
+    assert (
+        exc_info.value.status_code == 400
+    ), "str_to_interval should return a 400 status code for invalid datetime"
 
 
-def test_now_functions() -> None:
-    now1 = now_in_utc()
-    now2 = now_in_utc()
+@pytest.mark.parametrize("test_input", valid_intervals)
+def test_str_to_interval_with_valid_interval(test_input):
+    assert isinstance(
+        str_to_interval(test_input), tuple
+    ), "str_to_interval should return tuple for multi-value input"
 
-    assert now1 < now2
-    assert now1.tzinfo == timezone.utc
 
-    rfc3339_str_to_datetime(now_to_rfc3339_str())
+@pytest.mark.parametrize("test_input", valid_datetimes)
+def test_str_to_interval_with_valid_datetime(test_input):
+    assert isinstance(
+        str_to_interval(test_input), datetime
+    ), "str_to_interval should return single datetime for single-value input"
 
 
 def test_str_to_interval_with_none():
     """Test that str_to_interval returns None when provided with None."""
     assert (
         str_to_interval(None) is None
     ), "str_to_interval should return None when input is None"
+
+
+def test_now_functions() -> None:
+    now1 = now_in_utc()
+    now2 = now_in_utc()
+
+    assert now1 < now2
+    assert now1.tzinfo == timezone.utc
+
+    rfc3339_str_to_datetime(now_to_rfc3339_str())
```

