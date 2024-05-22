# Comparing `tmp/fastapi_namespace_vet1ments-0.1.3.tar.gz` & `tmp/fastapi_namespace_vet1ments-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_namespace_vet1ments-0.1.3.tar", last modified: Wed May 22 20:25:54 2024, max compression
+gzip compressed data, was "fastapi_namespace_vet1ments-0.1.4.tar", last modified: Wed May 22 20:54:22 2024, max compression
```

## Comparing `fastapi_namespace_vet1ments-0.1.3.tar` & `fastapi_namespace_vet1ments-0.1.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.812069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/mixin.py
--rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/namespace.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/resource.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.812069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/test.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/types.py
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/typings.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 20:25:47.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:25:54.816069 fastapi_namespace_vet1ments-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 20:25:54.000000 fastapi_namespace_vet1ments-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4238 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13011 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/namespace.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/resource.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/tests/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/tests/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/typings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-05-22 20:54:12.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-22 20:54:22.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      582 2024-05-22 20:54:22.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:54:22.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 20:54:22.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-22 20:54:22.000000 fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:54:22.306855 fastapi_namespace_vet1ments-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-05-22 20:54:20.000000 fastapi_namespace_vet1ments-0.1.4/setup.py
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/LICENSE` & `fastapi_namespace_vet1ments-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.3/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi_namespace_vet1ments
-Version: 0.1.3
+Version: 0.1.4
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/README.md` & `fastapi_namespace_vet1ments-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/mixin.py` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/mixin.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,43 +1,81 @@
 from .resource import Resource
-from typing import Sequence
+from typing import Sequence, ClassVar
 from fastapi.params import Depends
+from .utils import delete_none
+from .typings import MethodHandler, MethodType, ResourceProtocol
 
 class _Meta(type):
+    global_dependencies: Sequence[Depends]
+    get_dependencies: Sequence[Depends]
+    post_dependencies: Sequence[Depends]
+    put_dependencies: Sequence[Depends]
+    delete_dependencies: Sequence[Depends]
+    options_dependencies: Sequence[Depends]
+    head_dependencies: Sequence[Depends]
+    patch_dependencies: Sequence[Depends]
+    trace_dependencies: Sequence[Depends]
+
     def __new__(mcs, name, bases, namespace):
-        global_dependencies: Sequence[Depends] = getattr(bases[0], 'global_dependencies', [])
-        global_dependencies = [*global_dependencies, namespace.get('global_dependencies', [])]
-        get_dependencies: Sequence[Depends] = getattr(bases[0], 'get_dependencies', [])
-        get_dependencies = [*get_dependencies, namespace.get('get_dependencies', [])]
-        post_dependencies: Sequence[Depends] = getattr(bases[0], 'post_dependencies', [])
-        post_dependencies = [*post_dependencies, namespace.get('post_dependencies', [])]
-        put_dependencies: Sequence[Depends] = getattr(bases[0], 'put_dependencies', [])
-        put_dependencies = [*put_dependencies, namespace.get('put_dependencies', [])]
-        delete_dependencies: Sequence[Depends] = getattr(bases[0], 'delete_dependencies', [])
-        delete_dependencies = [*delete_dependencies, namespace.get('delete_dependencies', [])]
-        options_dependencies: Sequence[Depends] = getattr(bases[0], 'options_dependencies', [])
-        options_dependencies = [*options_dependencies, namespace.get('options_dependencies', [])]
-        head_dependencies: Sequence[Depends] = getattr(bases[0], 'head_dependencies', [])
-        head_dependencies = [*head_dependencies, namespace.get('head_dependencies', [])]
-        patch_dependencies: Sequence[Depends] = getattr(bases[0], 'patch_dependencies', [])
-        patch_dependencies = [*patch_dependencies, namespace.get('patch_dependencies', [])]
-        trace_dependencies: Sequence[Depends] = getattr(bases[0], 'trace_dependencies', [])
-        trace_dependencies = [*trace_dependencies, namespace.get('trace_dependencies', [])]
+        global_dependencies: Sequence[Depends] = getattr(bases[0], 'global_dependencies', None)
+        if global_dependencies is not None:
+            _global_dependencies = namespace.get('global_dependencies', [])
+            global_dependencies = [*global_dependencies, *_global_dependencies]
+
+        get_dependencies: Sequence[Depends] = getattr(bases[0], 'get_dependencies', None)
+        if get_dependencies is not None:
+            _get_dependencies = namespace.get('get_dependencies', [])
+            get_dependencies = [*get_dependencies, *_get_dependencies]
+
+        post_dependencies: Sequence[Depends] = getattr(bases[0], 'post_dependencies', None)
+        if post_dependencies is not None:
+            _post_dependencies = namespace.get('post_dependencies', [])
+            post_dependencies = [*post_dependencies, *_post_dependencies]
+
+        put_dependencies: Sequence[Depends] = getattr(bases[0], 'put_dependencies', None)
+        if put_dependencies is not None:
+            _put_dependencies = namespace.get('put_dependencies', [])
+            put_dependencies = [*put_dependencies, *_put_dependencies]
+
+        delete_dependencies: Sequence[Depends] = getattr(bases[0], 'delete_dependencies', None)
+        if delete_dependencies is not None:
+            _delete_dependencies = namespace.get('delete_dependencies', [])
+            delete_dependencies = [*delete_dependencies, *_delete_dependencies]
+
+        options_dependencies: Sequence[Depends] = getattr(bases[0], 'options_dependencies', None)
+        if options_dependencies is not None:
+            _options_dependencies = namespace.get('options_dependencies', [])
+            options_dependencies = [*options_dependencies, *_options_dependencies]
+
+        head_dependencies: Sequence[Depends] = getattr(bases[0], 'head_dependencies', None)
+        if head_dependencies is not None:
+            _head_dependencies = namespace.get('head_dependencies', [])
+            head_dependencies = [*head_dependencies, *_head_dependencies]
+
+        patch_dependencies: Sequence[Depends] = getattr(bases[0], 'patch_dependencies', None)
+        if patch_dependencies is not None:
+            _patch_dependencies = namespace.get('patch_dependencies', [])
+            patch_dependencies = [*patch_dependencies, *_patch_dependencies]
+
+        trace_dependencies: Sequence[Depends] = getattr(bases[0], 'trace_dependencies', None)
+        if trace_dependencies is not None:
+            _trace_dependencies = namespace.get('trace_dependencies', [])
+            trace_dependencies = [*trace_dependencies, *_trace_dependencies]
 
-        namespace.update({
+        namespace.update(delete_none({
             'global_dependencies': global_dependencies,
             'get_dependencies': get_dependencies,
             'post_dependencies': post_dependencies,
             'put_dependencies': put_dependencies,
             'delete_dependencies': delete_dependencies,
             'options_dependencies': options_dependencies,
             'head_dependencies': head_dependencies,
             'patch_dependencies': patch_dependencies,
             'trace_dependencies': trace_dependencies,
-        })
+        }))
         return type.__new__(mcs, name, bases, namespace)
 
 class MixinBase(Resource, metaclass=_Meta):
     global_dependencies: Sequence[Depends]
     get_dependencies: Sequence[Depends]
     post_dependencies: Sequence[Depends]
     put_dependencies: Sequence[Depends]
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/namespace.py` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/namespace.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/resource.py` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/resource.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,49 +3,46 @@
 from fastapi.params import Depends
 from inspect import (
     Parameter,
     Signature,
     signature,
     iscoroutinefunction
 )
-from .typings import MethodHandler, MethodType
+from .typings import MethodHandler, MethodType, ResourceProtocol
 from .utils import gen_op_id
 
 def resource_dependant_name(key: str) -> str:
     return f'{key}_dependencies'
 
-class Resource(metaclass=ABCMeta):
+
+class Resource:
     global_dependencies: Sequence[Depends]
     get_dependencies: Sequence[Depends]
     post_dependencies: Sequence[Depends]
     put_dependencies: Sequence[Depends]
     delete_dependencies: Sequence[Depends]
     options_dependencies: Sequence[Depends]
     head_dependencies: Sequence[Depends]
     patch_dependencies: Sequence[Depends]
     trace_dependencies: Sequence[Depends]
 
-    def __init__(self):
-        self._init = False
-
-
     def get_dependant(self, method_handler, depends: Depends) -> Callable:
         assert isinstance(depends, Depends), "Dependant must be of type Depends!"
         method_handler_signature = signature(method_handler)
         method_handler_parameters = method_handler_signature.parameters
 
         op_id = gen_op_id()
 
         def wrap(**kwargs):
             kwargs.pop(op_id, None)
             return method_handler(**kwargs)
 
         async def async_wrap(**kwargs):
             kwargs.pop(op_id, None)
-            return method_handler(**kwargs)
+            return await method_handler(**kwargs)
 
         params = [
             Parameter(name=op_id, kind=Parameter.POSITIONAL_OR_KEYWORD, default=depends),
             *method_handler_parameters.values()
         ]
 
         if iscoroutinefunction(method_handler):
@@ -65,16 +62,18 @@
             self,
             method_handler,
     ) -> MethodHandler:
         method_func = method_handler
         method_name: MethodType = method_handler.__name__
 
         method_dependencies = getattr(self, resource_dependant_name(method_name), [])
+        method_dependencies = [*method_dependencies]
         method_dependencies.reverse()
         global_dependencies = getattr(self, resource_dependant_name('global'), [])
+        global_dependencies = [*global_dependencies]
         global_dependencies.reverse()
 
-        method_dependencies.extend(global_dependencies)
+        dependencies = [*method_dependencies, *global_dependencies]
 
-        for depends in method_dependencies:
+        for depends in dependencies:
             method_func = self.get_dependant(method_func, depends)
         return method_func
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/tests/test.py` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/tests/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 namespace = Namespace(
     prefix="/abcv",
     dependencies=[Depends(test)]
 )
 
 from fastapi import FastAPI
 from pydantic import BaseModel
+from fastapi_namespace.mixin import MixinBase
+
+def depend_test4(last: str) -> bool:
+    print(last)
+class Test(MixinBase):
+
+    global_dependencies = [Depends(depend_test4)]
+
 
 class ItemResponse(BaseModel):
     id: str
 
 
 
 
@@ -33,18 +41,19 @@
 def depend_get(get: str) -> bool:
     print(get)
 
 def depend_post(post: str) -> bool:
     print(post)
 
 @namespace.route('/{asd}')
-class Root(Resource):
-    __method_dependant__ = [Depends(depend_test), Depends(depend_test2)]
-    __get_dependant__ = [Depends(depend_get)]
-    __post_dependant__ = [Depends(depend_post)]
+class Root(Test):
+
+    global_dependencies = [Depends(depend_test), Depends(depend_test2)]
+    get_dependencies = [Depends(depend_get)]
+    post_dependencies = [Depends(depend_post)]
     def get(self) -> ItemResponse:
         return ItemResponse(id="1234")
 
     async def post(self) -> ItemResponse:
         return ItemResponse(id="1234")
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace/types.py` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace/types.py`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/PKG-INFO` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-namespace-vet1ments
-Version: 0.1.3
+Version: 0.1.4
 Summary: For FastAPI Routing Class
 Author: no hong seok
 Author-email: vet1ments@naver.com
 Maintainer: no hong seok
 Maintainer-email: vet1ments@naver.com
 License: MIT
 Project-URL: Repository, https://github.com/vet1ments/fastapi_namespace
```

### Comparing `fastapi_namespace_vet1ments-0.1.3/fastapi_namespace_vet1ments.egg-info/SOURCES.txt` & `fastapi_namespace_vet1ments-0.1.4/fastapi_namespace_vet1ments.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fastapi_namespace_vet1ments-0.1.3/setup.py` & `fastapi_namespace_vet1ments-0.1.4/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='fastapi_namespace_vet1ments',
     description="For FastAPI Routing Class",
-    version='0.1.3',
+    version='0.1.4',
     long_description=long_description,
     long_description_content_type='text/markdown',
     python_requires='>=3.11.0',
     author="no hong seok",
     author_email="vet1ments@naver.com",
     maintainer="no hong seok",
     maintainer_email="vet1ments@naver.com",
```

