# Comparing `tmp/fastapi_namespace_vet1ments-0.1.2.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.2.tar", last modified: Thu May 16 17:56:55 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.3.tar", last modified: Wed May 22 20:25:54 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.2.tar` & `fastapi_namespace_vet1ments-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12546 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)       72 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-16 17:56:47.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 17:56:55.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      526 2024-05-16 17:56:55.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:56:55.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 17:56:55.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 17:56:55.000000 fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 17:56:55.426450 fastapi_namespace_vet1ments-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-16 17:56:53.000000 fastapi_namespace_vet1ments-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.812069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.812069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.2/LICENSE` & `fastapi_namespace_vet1ments-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.2/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.2
+Version: 0.1.3
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.2/README.md` & `fastapi_namespace_vet1ments-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/namespace.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-from starlette.types import (
-    ASGIApp,
-    Lifespan
-)
-from starlette.routing import BaseRoute
+from starlette.routing import BaseRoute, Match
+from starlette.types import ASGIApp, Lifespan, Receive, Scope, Send
+from starlette.datastructures import URL
+from starlette.responses import RedirectResponse
+from starlette._utils import get_route_path
 from fastapi import APIRouter
 from fastapi.types import (
     IncEx,
 )
 from fastapi.responses import JSONResponse as ORJSONResponse
 from fastapi.routing import APIRoute
 from fastapi.utils import generate_unique_id
-from fastapi import Depends, Response
+from fastapi import Response
+from fastapi.params import Depends
 
 from .resource import Resource
 from .types import (
     MethodDocument,
     DecoratedCallable
 )
-
 from typing import (
     Optional,
     Callable,
     Sequence,
     Type,
     Any,
     Literal,
@@ -36,16 +36,16 @@
     route in 
     resource set doc
 
 """
 
 __methods__ = ['get', 'post', 'put', 'delete', 'options', 'head', 'patch', 'trace']
 
-class Namespace(APIRouter):
 
+class Namespace(APIRouter):
     def __init__(
             self,
             *,
             prefix: str | None = "",
             tags: list[str | Enum] | None = None,
             dependencies: Sequence[Depends] = None,
             default_response_class: Type[Response] = ORJSONResponse,
@@ -74,14 +74,22 @@
             dependency_overrides_provider=dependency_overrides_provider,
             route_class=route_class,
             lifespan=lifespan,
             deprecated=deprecated,
             include_in_schema=include_in_schema,
             generate_unique_id_function=generate_unique_id_function
         )
+        self.get = None
+        self.post = None
+        self.put = None
+        self.delete = None
+        self.options = None
+        self.head = None
+        self.patch = None
+        self.trace = None
 
     def route(
             self,
             path,
             *,
             response_model: Any = None,
             status_code: int | None = None,
@@ -239,17 +247,20 @@
             })
         default_summary = f"{func.__self__.__class__.__name__}_{func.__name__}"
         kwargs.update({
             "summary": default_summary if (summary := kwargs.get("summary", None)) is None else f"{summary} {default_summary}"
         })
         func.__func__.__meth_doc__ = delete_none(kwargs)
 
+        new_func = func.__self__.get_method_handler(
+            func
+        )
         self.add_api_route(
             path=path,
-            endpoint=func,
+            endpoint=new_func,
             methods=[method.upper()],
             **func.__func__.__meth_doc__
         )
 
     def doc(
             self,
             summary: str | None = None,
```

### Comparing `fastapi_namespace_vet1ments-0.1.2/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.2
+Version: 0.1.3
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.2/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 LICENSE
 README.md
 setup.py
 fastapi_namespace/__init__.py
+fastapi_namespace/mixin.py
 fastapi_namespace/namespace.py
 fastapi_namespace/resource.py
 fastapi_namespace/types.py
+fastapi_namespace/typings.py
 fastapi_namespace/utils.py
 fastapi_namespace/tests/__init__.py
 fastapi_namespace/tests/test.py
 fastapi_namespace/tests/test2.py
 fastapi_namespace_vet1ments.egg-info/PKG-INFO
 fastapi_namespace_vet1ments.egg-info/SOURCES.txt
 fastapi_namespace_vet1ments.egg-info/dependency_links.txt
```

### Comparing `fastapi_namespace_vet1ments-0.1.2/setup.py` & `fastapi_namespace_vet1ments-0.1.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.2',
+    version='0.1.3',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

