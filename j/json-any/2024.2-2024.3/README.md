# Comparing `tmp/json-any-2024.2.tar.gz` & `tmp/json_any-2024.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json-any-2024.2.tar", last modified: Fri Feb 16 11:14:53 2024, max compression
+gzip compressed data, was "json_any-2024.3.tar", last modified: Wed May 22 07:36:18 2024, max compression
```

## Comparing `json-any-2024.2.tar` & `json_any-2024.3.tar`

### file list

```diff
@@ -1,33 +1,37 @@
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.769057 json-any-2024.2/
--rwx------   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json-any-2024.2/MANIFEST.in
--rw-r--r--   0 eric      (1000) users      (984)     4780 2024-02-16 11:14:53.769057 json-any-2024.2/PKG-INFO
--rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json-any-2024.2/README-LICENCE-utf8.txt
--rwx------   0 eric      (1000) users      (984)     4018 2023-07-17 12:03:11.000000 json-any-2024.2/README.rst
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.762390 json-any-2024.2/documentation/
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.765723 json-any-2024.2/documentation/wiki/
--rwx------   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json-any-2024.2/documentation/wiki/description.asciidoc
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.765723 json-any-2024.2/json_any/
--rwx------   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json-any-2024.2/json_any/__init__.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.765723 json-any-2024.2/json_any/catalog/
--rwx------   0 eric      (1000) users      (984)     2268 2024-02-16 10:39:07.000000 json-any-2024.2/json_any/catalog/module.py
--rwx------   0 eric      (1000) users      (984)     5399 2024-02-16 11:05:20.000000 json-any-2024.2/json_any/catalog/type.py
--rwx------   0 eric      (1000) users      (984)     1914 2023-12-09 10:20:46.000000 json-any-2024.2/json_any/constant.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.769057 json-any-2024.2/json_any/extension/
--rwx------   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json-any-2024.2/json_any/extension/module.py
--rwx------   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json-any-2024.2/json_any/extension/numpy.py
--rwx------   0 eric      (1000) users      (984)     2251 2023-10-04 09:23:36.000000 json-any-2024.2/json_any/extension/pandas.py
--rwx------   0 eric      (1000) users      (984)     3306 2023-07-18 09:13:52.000000 json-any-2024.2/json_any/extension/type.py
--rwx------   0 eric      (1000) users      (984)    12837 2024-02-16 11:14:34.000000 json-any-2024.2/json_any/json_to_object.py
--rwx------   0 eric      (1000) users      (984)    14745 2024-02-16 11:14:34.000000 json-any-2024.2/json_any/object_to_json.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.769057 json-any-2024.2/json_any/task/
--rwx------   0 eric      (1000) users      (984)     3348 2023-07-17 07:04:05.000000 json-any-2024.2/json_any/task/compression.py
--rwx------   0 eric      (1000) users      (984)     8337 2024-02-16 11:14:34.000000 json-any-2024.2/json_any/task/storage.py
--rwx------   0 eric      (1000) users      (984)     1575 2024-02-16 11:14:13.000000 json-any-2024.2/json_any/version.py
-drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-02-16 11:14:53.769057 json-any-2024.2/json_any.egg-info/
--rw-r--r--   0 eric      (1000) users      (984)     4780 2024-02-16 11:14:53.000000 json-any-2024.2/json_any.egg-info/PKG-INFO
--rw-r--r--   0 eric      (1000) users      (984)      573 2024-02-16 11:14:53.000000 json-any-2024.2/json_any.egg-info/SOURCES.txt
--rw-r--r--   0 eric      (1000) users      (984)        1 2024-02-16 11:14:53.000000 json-any-2024.2/json_any.egg-info/dependency_links.txt
--rw-r--r--   0 eric      (1000) users      (984)        9 2024-02-16 11:14:53.000000 json-any-2024.2/json_any.egg-info/top_level.txt
--rwx------   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json-any-2024.2/pyproject.toml
--rw-r--r--   0 eric      (1000) users      (984)       38 2024-02-16 11:14:53.769057 json-any-2024.2/setup.cfg
--rwx------   0 eric      (1000) users      (984)     5320 2023-07-13 15:24:10.000000 json-any-2024.2/setup.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.455531 json_any-2024.3/
+-rwx------   0 eric      (1000) users      (984)      109 2022-07-04 12:52:08.000000 json_any-2024.3/MANIFEST.in
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2024-05-22 07:36:18.455531 json_any-2024.3/PKG-INFO
+-rwx------   0 eric      (1000) users      (984)    21778 2019-02-21 09:59:58.000000 json_any-2024.3/README-LICENCE-utf8.txt
+-rwx------   0 eric      (1000) users      (984)     4018 2023-07-17 12:03:11.000000 json_any-2024.3/README.rst
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.448864 json_any-2024.3/documentation/
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/documentation/wiki/
+-rwx------   0 eric      (1000) users      (984)     1854 2022-07-05 06:50:56.000000 json_any-2024.3/documentation/wiki/description.asciidoc
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/json_any/
+-rwx------   0 eric      (1000) users      (984)     1749 2023-07-13 12:47:03.000000 json_any-2024.3/json_any/__init__.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/json_any/catalog/
+-rwx------   0 eric      (1000) users      (984)     2268 2024-02-16 10:39:07.000000 json_any-2024.3/json_any/catalog/module.py
+-rwx------   0 eric      (1000) users      (984)     4341 2024-05-22 07:03:57.000000 json_any-2024.3/json_any/catalog/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/json_any/constant/
+-rw-r--r--   0 eric      (1000) users      (984)     1919 2024-05-22 06:52:31.000000 json_any-2024.3/json_any/constant/compression.py
+-rwx------   0 eric      (1000) users      (984)     1914 2023-12-09 10:20:46.000000 json_any-2024.3/json_any/constant/json.py
+-rw-r--r--   0 eric      (1000) users      (984)     2714 2024-05-22 06:42:15.000000 json_any-2024.3/json_any/constant/module.py
+-rw-r--r--   0 eric      (1000) users      (984)     2085 2024-05-22 06:34:56.000000 json_any-2024.3/json_any/constant/type.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/json_any/extension/
+-rwx------   0 eric      (1000) users      (984)     2417 2023-07-13 15:36:06.000000 json_any-2024.3/json_any/extension/module.py
+-rwx------   0 eric      (1000) users      (984)     8143 2023-07-13 13:13:57.000000 json_any-2024.3/json_any/extension/numpy.py
+-rwx------   0 eric      (1000) users      (984)     2251 2023-10-04 09:23:36.000000 json_any-2024.3/json_any/extension/pandas.py
+-rwx------   0 eric      (1000) users      (984)     3311 2024-05-22 06:26:24.000000 json_any-2024.3/json_any/extension/type.py
+-rwx------   0 eric      (1000) users      (984)    12913 2024-05-22 07:03:57.000000 json_any-2024.3/json_any/json_to_object.py
+-rwx------   0 eric      (1000) users      (984)    14816 2024-05-22 07:03:57.000000 json_any-2024.3/json_any/object_to_json.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.452198 json_any-2024.3/json_any/task/
+-rwx------   0 eric      (1000) users      (984)     3298 2024-05-22 07:33:38.000000 json_any-2024.3/json_any/task/compression.py
+-rwx------   0 eric      (1000) users      (984)     7990 2024-05-22 07:33:40.000000 json_any-2024.3/json_any/task/storage.py
+-rwx------   0 eric      (1000) users      (984)     1575 2024-05-21 15:29:16.000000 json_any-2024.3/json_any/version.py
+drwxr-xr-x   0 eric      (1000) users      (984)        0 2024-05-22 07:36:18.455531 json_any-2024.3/json_any.egg-info/
+-rw-r--r--   0 eric      (1000) users      (984)     4780 2024-05-22 07:36:18.000000 json_any-2024.3/json_any.egg-info/PKG-INFO
+-rw-r--r--   0 eric      (1000) users      (984)      665 2024-05-22 07:36:18.000000 json_any-2024.3/json_any.egg-info/SOURCES.txt
+-rw-r--r--   0 eric      (1000) users      (984)        1 2024-05-22 07:36:18.000000 json_any-2024.3/json_any.egg-info/dependency_links.txt
+-rw-r--r--   0 eric      (1000) users      (984)        9 2024-05-22 07:36:18.000000 json_any-2024.3/json_any.egg-info/top_level.txt
+-rwx------   0 eric      (1000) users      (984)      104 2022-05-10 10:05:52.000000 json_any-2024.3/pyproject.toml
+-rw-r--r--   0 eric      (1000) users      (984)       38 2024-05-22 07:36:18.455531 json_any-2024.3/setup.cfg
+-rwx------   0 eric      (1000) users      (984)     5351 2024-05-22 07:04:41.000000 json_any-2024.3/setup.py
```

### Comparing `json-any-2024.2/PKG-INFO` & `json_any-2024.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2024.2
+Version: 2024.3
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2024.2/README-LICENCE-utf8.txt` & `json_any-2024.3/README-LICENCE-utf8.txt`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/README.rst` & `json_any-2024.3/README.rst`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/documentation/wiki/description.asciidoc` & `json_any-2024.3/documentation/wiki/description.asciidoc`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/__init__.py` & `json_any-2024.3/json_any/__init__.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/catalog/module.py` & `json_any-2024.3/json_any/catalog/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/catalog/type.py` & `json_any-2024.3/json_any/catalog/type.py`

 * *Files 16% similar despite different names*

```diff
@@ -26,42 +26,46 @@
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import types as t
+import typing as h
 from array import array as py_array_t
 from datetime import date as date_t
 from datetime import datetime as date_time_t
 from datetime import time as time_t
 from datetime import timedelta as time_delta_t
 from datetime import timezone as time_zone_t
 from decimal import Decimal as decimal_t
 from enum import Enum as enum_t
 from fractions import Fraction as fraction_t
 from io import BytesIO as io_bytes_t
 from io import StringIO as io_string_t
 from pathlib import PurePath as path_t
 from typing import NamedTuple as named_tuple_t
-from typing import Sequence
 from uuid import UUID as uuid_t
 
 from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs, xrry
-from json_any.constant import MODULE_TYPE_SEPARATOR
-
-BUILTIN_BYTES_CONTAINERS = (bytes, bytearray)
-BUILTIN_CONTAINERS = (frozenset, list, set, tuple)
-JSON_TYPE: dict[type, str] = {}  # Matches non-builtin types with module-name_type-name.
-JSON_TYPE_PREFIX_PATHLIB = f"{path_t.__module__}{MODULE_TYPE_SEPARATOR}"
-
-BUILTIN_BYTES_CONTAINERS_NAMES = tuple(
-    _tpe.__name__ for _tpe in BUILTIN_BYTES_CONTAINERS
+from json_any.constant.json import MODULE_TYPE_SEPARATOR
+from json_any.constant.module import (
+    NETWORKX_CLASSES,
+    NUMPY_ARRAY_CLASSES,
+    PANDAS_CLASSES,
+    SCIPY_ARRAY_CLASSES,
+    XARRAY_CLASSES,
+)
+from json_any.constant.type import (
+    BUILTIN_BYTES_CONTAINERS,
+    BUILTIN_BYTES_CONTAINERS_NAMES,
+    BUILTIN_CONTAINERS,
+    BUILTIN_CONTAINERS_NAMES,
+    JSON_TYPE,
 )
-BUILTIN_CONTAINERS_NAMES = tuple(_tpe.__name__ for _tpe in BUILTIN_CONTAINERS)
 
 
 def ContainerWithName(name: str, /) -> type:
     """"""
     if name in BUILTIN_BYTES_CONTAINERS_NAMES:
         return BUILTIN_BYTES_CONTAINERS[BUILTIN_BYTES_CONTAINERS_NAMES.index(name)]
     else:
@@ -80,17 +84,16 @@
 
 
 def TypeNameOf(json_type: str, /) -> str:
     """"""
     return json_type[(json_type.rindex(MODULE_TYPE_SEPARATOR) + 1) :]
 
 
-def _AddJsonTypes(types: Sequence[type], /) -> None:
+def _AddJsonTypes(types: h.Sequence[type], /) -> None:
     """"""
-    global JSON_TYPE
 
     for type_ in types:
         JSON_TYPE[type_] = f"{type_.__module__}{MODULE_TYPE_SEPARATOR}{type_.__name__}"
 
 
 _AddJsonTypes(
     (
@@ -106,61 +109,23 @@
         time_delta_t,
         time_t,
         time_zone_t,
         uuid_t,
     )
 )
 
-
-# Note: When there is a single class of interest in a module, the purpose of a *_CLASSES
-# tuple is to have an homogeneous dealing of all modules.
-
-if pypl is None:
-    MATPLOTLIB_CLASSES = ()
-else:
+if pypl is not None:
     figure_t = pypl.Figure
-    MATPLOTLIB_CLASSES = (figure_t,)
-    # Unfortunately, figure_t.__nodule__ is reported as "matplotlib.figure" instead of
+    # Unfortunately, figure_t.__module__ is reported as "matplotlib.figure" instead of
     # the expected "matplotlib.pyplot".
     JSON_TYPE[figure_t] = f"{pypl.__name__}{MODULE_TYPE_SEPARATOR}{figure_t.__name__}"
-
-if grph is None:
-    NETWORKX_CLASSES = ()
-else:
-    NETWORKX_CLASSES = (grph.Graph, grph.DiGraph, grph.MultiGraph, grph.MultiDiGraph)
+if grph is not None:
     _AddJsonTypes(NETWORKX_CLASSES)
-
-if nmpy is None:
-    JSON_TYPE_NUMPY_SCALAR = ""
-    np_array_t = None
-    NUMPY_ARRAY_CLASSES = ()
-else:
-    JSON_TYPE_NUMPY_SCALAR = f"{nmpy.__name__}{MODULE_TYPE_SEPARATOR}SCALAR"
+if nmpy is not None:
     np_array_t = nmpy.ndarray
-    NUMPY_ARRAY_CLASSES = (np_array_t,)
     _AddJsonTypes(NUMPY_ARRAY_CLASSES)
-
-if pnds is None:
-    PANDAS_CLASSES = ()
-else:
-    PANDAS_CLASSES = (pnds.Series, pnds.DataFrame)
+if pnds is not None:
     _AddJsonTypes(PANDAS_CLASSES)
-
-if sprs is None:
-    SCIPY_ARRAY_CLASSES = ()
-else:
-    SCIPY_ARRAY_CLASSES = (
-        sprs.bsr_array,
-        sprs.coo_array,
-        sprs.csc_array,
-        sprs.csr_array,
-        sprs.dia_array,
-        sprs.dok_array,
-        sprs.lil_array,
-    )
+if sprs is not None:
     _AddJsonTypes(SCIPY_ARRAY_CLASSES)
-
-if xrry is None:
-    XARRAY_CLASSES = ()
-else:
-    XARRAY_CLASSES = (xrry.DataArray, xrry.Dataset)
+if xrry is not None:
     _AddJsonTypes(XARRAY_CLASSES)
```

### Comparing `json-any-2024.2/json_any/constant.py` & `json_any-2024.3/json_any/constant/json.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/extension/module.py` & `json_any-2024.3/json_any/extension/module.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/extension/numpy.py` & `json_any-2024.3/json_any/extension/numpy.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/extension/pandas.py` & `json_any-2024.3/json_any/extension/pandas.py`

 * *Files identical despite different names*

### Comparing `json-any-2024.2/json_any/extension/type.py` & `json_any-2024.3/json_any/extension/type.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 import dataclasses as dtcl
 from typing import Any, Callable, Union
 
-from json_any.constant import MODULE_TYPE_SEPARATOR
+from json_any.constant.json import MODULE_TYPE_SEPARATOR
 from json_any.extension.module import ElementInModule
 
 builders_h = dict[str, Callable[[Any], Any]]
 description_h = tuple[str, Any]
 descriptors_h = dict[str, Callable[[Any], Any]]
```

### Comparing `json-any-2024.2/json_any/json_to_object.py` & `json_any-2024.3/json_any/json_to_object.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,19 +32,14 @@
 import dataclasses as dtcl
 import json
 import pathlib as pthl
 from typing import Any
 
 from json_any.catalog.module import grph, nmpy, pnds, pypl, sprs, xrry
 from json_any.catalog.type import (
-    BUILTIN_BYTES_CONTAINERS_NAMES,
-    BUILTIN_CONTAINERS_NAMES,
-    JSON_TYPE,
-    JSON_TYPE_NUMPY_SCALAR,
-    JSON_TYPE_PREFIX_PATHLIB,
     ContainerWithName,
     TypeIsInModule,
     TypeNameOf,
     date_t,
     date_time_t,
     decimal_t,
     enum_t,
@@ -54,22 +49,29 @@
     named_tuple_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
-from json_any.constant import (
+from json_any.constant.json import (
     CUSTOM_PREFIX,
     DATACLASS_PREFIX,
     NEW_FROM_JSON_DESCRIPTION,
     STANDARD_PREFIX,
     TYPE_PREFIX,
     UNHANDLED_PREFIX,
 )
+from json_any.constant.module import JSON_TYPE_NUMPY_SCALAR
+from json_any.constant.type import (
+    BUILTIN_BYTES_CONTAINERS_NAMES,
+    BUILTIN_CONTAINERS_NAMES,
+    JSON_TYPE,
+    JSON_TYPE_PREFIX_PATHLIB,
+)
 from json_any.extension.module import ElementInModule
 from json_any.extension.numpy import AsNumpyArray
 from json_any.extension.type import (
     TypeFromJsonType,
     builders_h,
     description_h,
     unfound_t,
```

### Comparing `json-any-2024.2/json_any/object_to_json.py` & `json_any-2024.3/json_any/object_to_json.py`

 * *Files 3% similar despite different names*

```diff
@@ -25,38 +25,22 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-# TODO: Add xarray support.
-#     See https://docs.xarray.dev/en/stable/generated/xarray.DataArray.from_dict.html#xarray.DataArray.from_dict
-#         https://docs.xarray.dev/en/stable/generated/xarray.DataArray.to_dict.html#xarray.DataArray.to_dict
-#     and similarly for datasets.
-
 import dataclasses as dtcl
 import importlib as imlb
 import json
 import sys as sstm
 import typing as h
 
 from json_any.catalog.module import grph
 from json_any.catalog.type import (
-    BUILTIN_BYTES_CONTAINERS,
-    BUILTIN_CONTAINERS,
-    JSON_TYPE,
-    JSON_TYPE_NUMPY_SCALAR,
-    JSON_TYPE_PREFIX_PATHLIB,
-    MATPLOTLIB_CLASSES,
-    NETWORKX_CLASSES,
-    NUMPY_ARRAY_CLASSES,
-    PANDAS_CLASSES,
-    SCIPY_ARRAY_CLASSES,
-    XARRAY_CLASSES,
     date_t,
     date_time_t,
     decimal_t,
     enum_t,
     fraction_t,
     io_bytes_t,
     io_string_t,
@@ -64,23 +48,38 @@
     path_t,
     py_array_t,
     time_delta_t,
     time_t,
     time_zone_t,
     uuid_t,
 )
-from json_any.constant import (
+from json_any.constant.json import (
     CUSTOM_PREFIX,
     DATACLASS_PREFIX,
     DESCRIPTION_FOR_JSON,
     JSONING_ERROR_MARKER,
     STANDARD_PREFIX,
     TYPE_PREFIX,
     UNHANDLED_PREFIX,
 )
+from json_any.constant.module import (
+    JSON_TYPE_NUMPY_SCALAR,
+    MATPLOTLIB_CLASSES,
+    NETWORKX_CLASSES,
+    NUMPY_ARRAY_CLASSES,
+    PANDAS_CLASSES,
+    SCIPY_ARRAY_CLASSES,
+    XARRAY_CLASSES,
+)
+from json_any.constant.type import (
+    BUILTIN_BYTES_CONTAINERS,
+    BUILTIN_CONTAINERS,
+    JSON_TYPE,
+    JSON_TYPE_PREFIX_PATHLIB,
+)
 from json_any.extension.numpy import (
     AsMostConciseRepresentation,
     AsScalarRepresentation,
     IsNumpyScalar,
 )
 from json_any.extension.type import (
     IsFullyDataclassBased,
@@ -89,14 +88,19 @@
     description_h,
     descriptors_h,
 )
 
 _HISTORY_INDENTATION = 4 * " "
 
 
+# TODO: JSON alternatives:
+#     https://pymongo.readthedocs.io/en/stable/api/bson/index.html
+#     https://ubjson.org/libraries/
+#     https://en.wikipedia.org/wiki/CBOR
+#     https://pypi.org/project/newsmile/    https://github.com/FasterXML/smile-format-specification
 def JsonStringOf(
     instance: h.Any, /, *, descriptors: descriptors_h = None
 ) -> tuple[str, h.Sequence[str] | None]:
     """"""
     history = []
     jsonable = _JsonableVersionOf(
         instance, history, "", highest_level_call=True, descriptors=descriptors
```

### Comparing `json-any-2024.2/json_any/task/compression.py` & `json_any-2024.3/json_any/task/compression.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,28 +25,28 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-from typing import Callable
-
+from json_any.constant.compression import (
+    STANDARD_COMPRESSOR,
+    STANDARD_COMPRESSOR_MODULES,
+    STANDARD_DECOMPRESSOR,
+    de_compressor_h,
+)
 from json_any.extension.module import ElementInModule
 
-STANDARD_COMPRESSOR_MODULES = ("bz2", "gzip", "lzma", "zlib")
-STANDARD_COMPRESSOR = "compress"
-STANDARD_DECOMPRESSOR = "decompress"
-
 
 def CompressedVersion(
     jsoned: str,
     /,
     *args,
-    compressor: str | Callable[[bytes, ...], bytes] = STANDARD_COMPRESSOR_MODULES[0],
+    compressor: str | de_compressor_h = STANDARD_COMPRESSOR_MODULES[0],
     **kwargs,
 ) -> bytes:
     """"""
     if isinstance(compressor, str):
         if compressor in STANDARD_COMPRESSOR_MODULES:
             Compressed, _ = ElementInModule(STANDARD_COMPRESSOR, compressor)
             if Compressed is None:
@@ -62,15 +62,15 @@
     return Compressed(jsoned.encode(), *args, **kwargs)
 
 
 def DecompressedVersion(
     compressed: bytes,
     /,
     *args,
-    decompressor: str | Callable[[bytes, ...], bytes] = STANDARD_COMPRESSOR_MODULES[0],
+    decompressor: str | de_compressor_h = STANDARD_COMPRESSOR_MODULES[0],
     **kwargs,
 ) -> str:
     """"""
     if isinstance(decompressor, str):
         if decompressor in STANDARD_COMPRESSOR_MODULES:
             Decompressed, _ = ElementInModule(STANDARD_DECOMPRESSOR, decompressor)
             if Decompressed is None:
@@ -79,9 +79,9 @@
                     f'or has no "{STANDARD_DECOMPRESSOR}" function.'
                 )
         else:
             raise ValueError(f"{decompressor}: Unhandled compression module.")
     else:
         Decompressed = decompressor
 
-    decompressed = Decompressed(compressed, *args, **kwargs)
-    return decompressed.decode()
+    output = Decompressed(compressed, *args, **kwargs)
+    return output.decode()
```

### Comparing `json-any-2024.2/json_any/task/storage.py` & `json_any-2024.3/json_any/task/storage.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,65 +28,67 @@
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
 from io import BytesIO as bytes_io_t
 from io import StringIO as string_io_t
 from pathlib import Path as path_t
-from typing import Any, Callable, Hashable, NoReturn, Sequence
+from typing import Any, NoReturn, Sequence
 
+from json_any.constant.compression import (
+    STANDARD_COMPRESSOR_EXTENSIONS,
+    STANDARD_COMPRESSOR_MODULES,
+    de_compressor_h,
+)
 from json_any.extension.type import builders_h, descriptors_h
 from json_any.json_to_object import ObjectFromJsonString
 from json_any.object_to_json import JsonStringOf
-from json_any.task.compression import (
-    STANDARD_COMPRESSOR_MODULES,
-    CompressedVersion,
-    DecompressedVersion,
-)
+from json_any.task.compression import CompressedVersion, DecompressedVersion
 
-STANDARD_COMPRESSOR_EXTENSIONS = {
-    None: ".json",
-    "bz2": ".json.bz2",
-    "gzip": ".json.gz",
-    "lzma": ".json.lzma",
-    "zlib": ".json.zlib",
-}
-DECOMPRESSOR_AUTO = "AUTO"
+_DEFAULT_DE_COMPRESSOR = "Please use default (de)compressor"
 
 
 def StoreAsJSON(
     instance: Any,
     path: str | path_t | bytes_io_t | string_io_t,
     /,
     *args,
     descriptors: descriptors_h = None,
-    compressor: (
-        str | Callable[[bytes, ...], bytes] | None
-    ) = STANDARD_COMPRESSOR_MODULES[0],
+    compressor: str | de_compressor_h | None = _DEFAULT_DE_COMPRESSOR,
     should_continue_on_error: bool = False,
     should_add_standard_extension: bool = True,
     should_overwrite_path: bool = False,
     **kwargs,
 ) -> path_t | Sequence[str] | None:
     """"""
     if isinstance(path, str):
         path = path_t(path)
 
-    if (
-        isinstance(path, path_t)
-        and isinstance(compressor, Hashable)
-        and (compressor in STANDARD_COMPRESSOR_EXTENSIONS)
-    ):
+    if isinstance(path, path_t):
         extensions = path.suffixes
-        if extensions.__len__() > 0:
-            _CheckCompressorAndStdExtensionMatching(
-                compressor, "compressor", extensions
-            )
-        elif should_add_standard_extension:
-            path = path.with_suffix(STANDARD_COMPRESSOR_EXTENSIONS[compressor])
+        if compressor == _DEFAULT_DE_COMPRESSOR:
+            if extensions.__len__() > 0:
+                compressor = _De_CompressorFromExtension(extensions)
+            else:
+                compressor = STANDARD_COMPRESSOR_MODULES[0]
+                if should_add_standard_extension:
+                    path = path.with_suffix(STANDARD_COMPRESSOR_EXTENSIONS[compressor])
+        elif isinstance(compressor, str):
+            if extensions.__len__() > 0:
+                _CheckDeCompressorAndStdExtensionMatching(
+                    compressor, "compressor", extensions
+                )
+            elif should_add_standard_extension and (
+                compressor in STANDARD_COMPRESSOR_EXTENSIONS
+            ):
+                # If compressor not in STANDARD_COMPRESSOR_EXTENSIONS, the error will be
+                # handled when actually compressing.
+                path = path.with_suffix(STANDARD_COMPRESSOR_EXTENSIONS[compressor])
+    elif compressor == _DEFAULT_DE_COMPRESSOR:
+        compressor = STANDARD_COMPRESSOR_MODULES[0]
 
     if (
         isinstance(path, path_t)
         and path.exists()
         and not (path.is_file() and should_overwrite_path)
     ):
         message = f"{path}: Path exists and is not a file or should not be overwritten."
@@ -123,62 +125,44 @@
 
 
 def LoadFromJSON(
     path: str | path_t | bytes_io_t | string_io_t,
     /,
     *args,
     builders: builders_h = None,
-    decompressor: str | Callable[[bytes, ...], bytes] | None = DECOMPRESSOR_AUTO,
+    decompressor: str | de_compressor_h | None = _DEFAULT_DE_COMPRESSOR,
     should_continue_on_error: bool = False,
     **kwargs,
 ) -> Any:
     """"""
     if isinstance(path, str):
         path = path_t(path)
 
     if isinstance(path, path_t):
         extensions = path.suffixes
-        if decompressor == DECOMPRESSOR_AUTO:
+        if decompressor == _DEFAULT_DE_COMPRESSOR:
             if extensions.__len__() > 0:
-                decompressor = _DecompressorFromExtension(extensions)
+                decompressor = _De_CompressorFromExtension(extensions)
             else:
-                raise ValueError(
-                    f"{path.name}: Decompressor selection cannot be left to loader "
-                    f"when loading from a path without extension."
-                )
-        elif (
-            (extensions.__len__() > 0)
-            and isinstance(decompressor, Hashable)
-            and (decompressor in STANDARD_COMPRESSOR_EXTENSIONS)
-        ):
-            _CheckCompressorAndStdExtensionMatching(
+                decompressor = STANDARD_COMPRESSOR_MODULES[0]
+        elif isinstance(decompressor, str) and (extensions.__len__() > 0):
+            _CheckDeCompressorAndStdExtensionMatching(
                 decompressor, "decompressor", extensions
             )
 
         if decompressor is None:
             mode = "r"
         else:
             mode = "rb"
         with open(path, mode=mode) as json_accessor:
             content = json_accessor.read()
-    elif decompressor == DECOMPRESSOR_AUTO:
-        raise ValueError(
-            f"{decompressor}: Decompressor selection cannot be left to loader "
-            f"when not loading from path."
-        )
     else:
-        if (isinstance(path, bytes_io_t) and (decompressor is None)) or (
-            isinstance(path, string_io_t) and (decompressor is not None)
-        ):
-            raise ValueError(
-                f"T.{type(path).__name__}, D.{decompressor}: Path-like type T and "
-                f"decompression D mismatch. Expected={bytes_io_t} with decompression, "
-                f"or {string_io_t} without decompression."
-            )
         content = path.read()
+        if decompressor == _DEFAULT_DE_COMPRESSOR:
+            decompressor = STANDARD_COMPRESSOR_MODULES[0]
 
     if decompressor is None:
         jsoned = content
     else:
         jsoned = DecompressedVersion(
             content,
             *args,
@@ -189,50 +173,44 @@
     return ObjectFromJsonString(
         jsoned,
         builders=builders,
         should_continue_on_error=should_continue_on_error,
     )
 
 
-def _CheckCompressorAndStdExtensionMatching(
-    compressor: Hashable, actual: str, extensions: Sequence[str], /
-) -> None | NoReturn:
-    """
-    Actually, compressor or decompressor, with "actual" allowing to make the difference.
-    """
+def _De_CompressorFromExtension(extensions: Sequence[str], /) -> str | None | NoReturn:
+    """"""
     full_extension = "".join(extensions)
-    found = False
     for (
         std_compressor,
         std_full_extension,
     ) in STANDARD_COMPRESSOR_EXTENSIONS.items():
         if full_extension.lower() == std_full_extension:
-            found = compressor == std_compressor
-            break
+            return std_compressor
 
-    if not found:
-        initial = actual[0].upper()
-        expected = " or ".join(
-            f"{initial}.{_key}+E.{_vle}"
-            for _key, _vle in STANDARD_COMPRESSOR_EXTENSIONS.items()
-        )
-        raise ValueError(
-            f"{initial}.{compressor}, E.{full_extension}: {actual.capitalize()} "
-            f"{initial} and extension E do not match. Expected={expected}."
-        )
+    expected = " or ".join(STANDARD_COMPRESSOR_EXTENSIONS.values())
+    raise ValueError(
+        f"{full_extension}: Not a valid extension for automatic (de)compressor "
+        f"selection. Expected={expected}."
+    )
 
 
-def _DecompressorFromExtension(extensions: Sequence[str], /) -> str | None | NoReturn:
+def _CheckDeCompressorAndStdExtensionMatching(
+    de_compressor: str, actual: str, extensions: Sequence[str], /
+) -> None | NoReturn:
     """"""
+    if de_compressor not in STANDARD_COMPRESSOR_MODULES:
+        raise ValueError(f"{de_compressor}: Unhandled (de)compression module.")
+
     full_extension = "".join(extensions)
-    for (
-        std_compressor,
-        std_full_extension,
-    ) in STANDARD_COMPRESSOR_EXTENSIONS.items():
-        if full_extension.lower() == std_full_extension:
-            return std_compressor
+    if full_extension.lower() == STANDARD_COMPRESSOR_EXTENSIONS[de_compressor]:
+        return
 
-    expected = " or ".join(STANDARD_COMPRESSOR_EXTENSIONS.values())
+    first_as_capital = actual[0].upper()
+    expected = " or ".join(
+        f"{first_as_capital}.{_key}+E.{_vle}"
+        for _key, _vle in STANDARD_COMPRESSOR_EXTENSIONS.items()
+    )
     raise ValueError(
-        f"{full_extension}: Not a valid extension for automatic decompressor "
-        f"selection. Expected={expected}."
+        f"{first_as_capital}.{de_compressor}, E.{full_extension}: {actual.capitalize()} "
+        f"{first_as_capital} and extension E do not match. Expected={expected}."
     )
```

### Comparing `json-any-2024.2/json_any/version.py` & `json_any-2024.3/json_any/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,8 +25,8 @@
 # requirements in conditions enabling the security of their systems and/or
 # data to be ensured and,  more generally, to use and operate it in the
 # same conditions as regards security.
 #
 # The fact that you are presently reading this means that you have had
 # knowledge of the CeCILL license and that you accept its terms.
 
-__version__ = "2024.2"
+__version__ = "2024.3"
```

### Comparing `json-any-2024.2/json_any.egg-info/PKG-INFO` & `json_any-2024.3/json_any.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-any
-Version: 2024.2
+Version: 2024.3
 Summary: JSON and unJSON objects of any type
 Home-page: https://src.koda.cnrs.fr/eric.debreuve/json-any/
 Author: Eric Debreuve
 Author-email: eric.debreuve@cnrs.fr
 License: CeCILL-2.1
 Project-URL: Documentation, https://src.koda.cnrs.fr/eric.debreuve/json-any//-/wikis/home
 Project-URL: Source, https://src.koda.cnrs.fr/eric.debreuve/json-any/
```

### Comparing `json-any-2024.2/json_any.egg-info/SOURCES.txt` & `json_any-2024.3/json_any.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 MANIFEST.in
 README-LICENCE-utf8.txt
 README.rst
 pyproject.toml
 setup.py
 documentation/wiki/description.asciidoc
 json_any/__init__.py
-json_any/constant.py
 json_any/json_to_object.py
 json_any/object_to_json.py
 json_any/version.py
 json_any.egg-info/PKG-INFO
 json_any.egg-info/SOURCES.txt
 json_any.egg-info/dependency_links.txt
 json_any.egg-info/top_level.txt
 json_any/catalog/module.py
 json_any/catalog/type.py
+json_any/constant/compression.py
+json_any/constant/json.py
+json_any/constant/module.py
+json_any/constant/type.py
 json_any/extension/module.py
 json_any/extension/numpy.py
 json_any/extension/pandas.py
 json_any/extension/type.py
 json_any/task/compression.py
 json_any/task/storage.py
```

### Comparing `json-any-2024.2/setup.py` & `json_any-2024.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -69,14 +69,15 @@
 PYPI_AUDIENCE = "Developers"
 PYPI_STATUS = "4 - Beta"
 
 IMPORT_NAME = "json_any"
 PACKAGES = [
     IMPORT_NAME,
     f"{IMPORT_NAME}.catalog",
+    f"{IMPORT_NAME}.constant",
     f"{IMPORT_NAME}.extension",
     f"{IMPORT_NAME}.task",
 ]
 EXCLUDED_FOLDERS = (
     f"{IMPORT_NAME}.documentation",
 )
 ENTRY_POINTS = {
```

