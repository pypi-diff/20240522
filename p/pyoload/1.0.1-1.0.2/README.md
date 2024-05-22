# Comparing `tmp/pyoload-1.0.1.tar.gz` & `tmp/pyoload-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoload-1.0.1.tar", last modified: Sat May  4 00:49:18 2024, max compression
+gzip compressed data, was "pyoload-1.0.2.tar", last modified: Wed May 22 16:20:16 2024, max compression
```

## Comparing `pyoload-1.0.1.tar` & `pyoload-1.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.786731 pyoload-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-04 00:49:16.000000 pyoload-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 00:49:18.786731 pyoload-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2507 2024-05-04 00:49:16.000000 pyoload-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/pyoload/
--rw-r--r--   0 runner    (1001) docker     (127)     6633 2024-05-04 00:49:14.000000 pyoload-1.0.1/pyoload/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/pyoload.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-04 00:49:18.000000 pyoload-1.0.1/pyoload.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-04 00:49:18.786731 pyoload-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1999 2024-05-04 00:49:14.000000 pyoload-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-04 00:49:18.782731 pyoload-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-04 00:49:14.000000 pyoload-1.0.1/tests/test_placeholder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-22 16:20:13.000000 pyoload-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-22 16:20:16.066493 pyoload-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3064 2024-05-22 16:20:13.000000 pyoload-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.062493 pyoload-1.0.2/pyoload/
+-rw-r--r--   0 runner    (1001) docker     (127)    10243 2024-05-22 16:20:11.000000 pyoload-1.0.2/pyoload/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/pyoload.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      226 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 16:20:16.000000 pyoload-1.0.2/pyoload.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:20:16.066493 pyoload-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-22 16:20:11.000000 pyoload-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:20:16.066493 pyoload-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-05-22 16:20:11.000000 pyoload-1.0.2/tests/test_placeholder.py
```

### Comparing `pyoload-1.0.1/LICENSE` & `pyoload-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoload-1.0.1/PKG-INFO` & `pyoload-1.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyoload
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for function argument overload, typechecking and casting
 Home-page: https://github.com/ken-morel/pyoload
 Author: ken-morel
 Author-email: engonken8@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,42 +31,42 @@
 Requires-Dist: flake8-commas; extra == "ci"
 Requires-Dist: flake8-quotes; extra == "ci"
 Requires-Dist: flake8-multiline-containers; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Requires-Dist: pytest-cov; extra == "ci"
 Requires-Dist: coveralls; extra == "ci"
 
-# pip-package-template-docker
+# pyoload
 
 [![Release Status](https://github.com/ken-morel/pyoload/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ken-morel/pyoload/releases)
 [![PyPI package](https://badge.fury.io/py/pyoload.svg)](https://pypi.org/project/pyoload)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyoload)](https://pypi.org/project/pyoload)
 [![Build Status](https://github.com/ken-morel/pyoload/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ken-morel/pyoload/tree/main)
 [![Coverage Status](https://coveralls.io/repos/github/ken-morel/pyoload/badge.svg?branch=main)](https://coveralls.io/github/ken-morel/pyoload?branch=main)
 
 pyoload has two main functions
 
-annotate
-========
+# pyoload.annotate
+
 Is used as a decorator on the function.
 ```python
 
 from pyoload import annotate
 
 @annotate
 def twice(a:int) -> int:
     return a * 2
 
 b = twice(4)
 ```
 The annotate creates a wrapper over the decorated function which checks in for argument types over each function call using `pyoload.matchType(val, spec)`.
 The original function is kept in the `.__pyod_annotate__` attribute.
 
-overload
-========
+# pyoload.overload
+
 Implements function overloading in python via a simple decorator
 
 ```python
 from pyoload import overload
 import math
 cache = {}
 
@@ -83,16 +84,41 @@
 ```
 
 When an overload is registerred, the function name in the form `functionModuleName.functionQualName` is goten using `pyoload.get_name(funcOrClass)` an annotate is gotten using `pyoload.annotate(func, True)`
 and a new list of overloads is created and stored in `pyoload.__overloads__` dictionarry under it's name. A reference to the list of annotated overloads is stored in the functions `.__pyod_overloads__`.
 
 When the function is called, the wrapper tries all the functions registerred to that name to catch a `pyoload.InternalAnnotationError`. If none ran succesfully, it raises an `pyoload.OverloadError`.
 
-Accepted annotations
-====================
+# Casting
+
+All `pyoload.annotate` and `pyoload.overload` both support Cast objects
+instances of `pyoloas.Cast`.
+It uses recursive casting with integrated support for dictionaries, e.g:
+```python
+dict[
+  int,
+  tuple[list[float] | float]
+]
+```
+for a dictionarry mapping of integers to list of floats or floats.
+
+> Note:
+  When a union, e.g `int | str` is passed to Cast, it tries to cast in each of
+  the specified types in the listed order, that is
+
+  ```python
+  cast = pyoload.Cast(int|str)
+  print(repr(cast(3.0)))
+  ```
+
+  Will print `'3.0'` as `3.0` can not be converted to a complex
+
+
+# Accepted annotations
+
 
 In addition to supporting normal plain types,
 pyoload includes support for generic aliasses of iterable types and some other classes:
 
 - `pyoload.Values(iterable)`
   e.g `Values("+-*/")` or `Values(range(6))`
 - `pyoload.Cast(type)`
```

### Comparing `pyoload-1.0.1/README.md` & `pyoload-1.0.2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-# pip-package-template-docker
+# pyoload
 
 [![Release Status](https://github.com/ken-morel/pyoload/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ken-morel/pyoload/releases)
 [![PyPI package](https://badge.fury.io/py/pyoload.svg)](https://pypi.org/project/pyoload)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyoload)](https://pypi.org/project/pyoload)
 [![Build Status](https://github.com/ken-morel/pyoload/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ken-morel/pyoload/tree/main)
 [![Coverage Status](https://coveralls.io/repos/github/ken-morel/pyoload/badge.svg?branch=main)](https://coveralls.io/github/ken-morel/pyoload?branch=main)
 
 pyoload has two main functions
 
-annotate
-========
+# pyoload.annotate
+
 Is used as a decorator on the function.
 ```python
 
 from pyoload import annotate
 
 @annotate
 def twice(a:int) -> int:
     return a * 2
 
 b = twice(4)
 ```
 The annotate creates a wrapper over the decorated function which checks in for argument types over each function call using `pyoload.matchType(val, spec)`.
 The original function is kept in the `.__pyod_annotate__` attribute.
 
-overload
-========
+# pyoload.overload
+
 Implements function overloading in python via a simple decorator
 
 ```python
 from pyoload import overload
 import math
 cache = {}
 
@@ -47,16 +47,41 @@
 ```
 
 When an overload is registerred, the function name in the form `functionModuleName.functionQualName` is goten using `pyoload.get_name(funcOrClass)` an annotate is gotten using `pyoload.annotate(func, True)`
 and a new list of overloads is created and stored in `pyoload.__overloads__` dictionarry under it's name. A reference to the list of annotated overloads is stored in the functions `.__pyod_overloads__`.
 
 When the function is called, the wrapper tries all the functions registerred to that name to catch a `pyoload.InternalAnnotationError`. If none ran succesfully, it raises an `pyoload.OverloadError`.
 
-Accepted annotations
-====================
+# Casting
+
+All `pyoload.annotate` and `pyoload.overload` both support Cast objects
+instances of `pyoloas.Cast`.
+It uses recursive casting with integrated support for dictionaries, e.g:
+```python
+dict[
+  int,
+  tuple[list[float] | float]
+]
+```
+for a dictionarry mapping of integers to list of floats or floats.
+
+> Note:
+  When a union, e.g `int | str` is passed to Cast, it tries to cast in each of
+  the specified types in the listed order, that is
+
+  ```python
+  cast = pyoload.Cast(int|str)
+  print(repr(cast(3.0)))
+  ```
+
+  Will print `'3.0'` as `3.0` can not be converted to a complex
+
+
+# Accepted annotations
+
 
 In addition to supporting normal plain types,
 pyoload includes support for generic aliasses of iterable types and some other classes:
 
 - `pyoload.Values(iterable)`
   e.g `Values("+-*/")` or `Values(range(6))`
 - `pyoload.Cast(type)`
```

### Comparing `pyoload-1.0.1/pyoload/__init__.py` & `pyoload-1.0.2/pyoload/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from typing import Any, GenericAlias, Union
+from types import UnionType
 from functools import wraps, partial
 from inspect import isclass
 
+import sys
+
 
 class AnnotationError(ValueError):
     pass
 
 
 class AnnotationErrors(AnnotationError):
     pass
@@ -35,18 +38,24 @@
 
     def __str__(self):
         return 'Values(' + ', '.join(map(repr, self)) + ')'
 
     __repr__ = __str__
 
 
+Vs = Values
+
+
 def get_name(funcOrCls):
     return funcOrCls.__module__ + '.' + funcOrCls.__qualname__
 
 
+g_n = get_name
+
+
 class Validator:
     def __init__(self, func):
         if not callable(func):
             raise TypeError(self.__class__.__init__.__qualname__)
         self.func = func
 
     def __call__(self, val):
@@ -55,85 +64,171 @@
         except Exception as e:
             raise AnnotationError(
                 f'{type(e)} while using validator method: {get_name(self.func)}' +
                 f'\n{e!s}',
             ) from e
 
 
+Vf = Validator
+
+
 class Cast:
     @staticmethod
-    def cast(val, type):
-        if issubclass(type, Union):
-            type = type.__args__
-        if isinstance(type, tuple):
-            for x in type:
+    def cast(val, totype):
+        if isinstance(totype, GenericAlias):
+            if totype.__origin__ == dict:
+                if len(totype.__args__) == 2:
+                    kt, vt = totype.__args__
+                elif len(totype.__args__) == 1:
+                    kt, vt = Any, totype.__args__[1]
+                print(f"{totype=} {kt=} {vt=}")
+                return {
+                    Cast.cast(k, kt): Cast.cast(v, vt) for k, v in val.items()
+                }
+            else:
+                sub = totype.__args__[0]
+                return totype.__origin__([
+                    Cast.cast(v, sub) for v in val
+                ])
+        if isinstance(totype, UnionType):
+            errors = []
+            for subtype in totype.__args__:
                 try:
-                    return Cast.cast(val, x)
-                except Exception:
-                    pass
+                    return Cast.cast(val, subtype)
+                except Exception as e:
+                    errors.append(e)
             else:
-                raise CastingError()
-        return type(val) if not isinstance(val, type) else val
+                raise e
+        else:
+            return totype(val) if not isinstance(val, totype) else val
 
     def __init__(self, type):
+        """
+        creates a casting object for the specified type
+        """
         self.type = type
 
-    def __call__(self, val):
+    def __call__(self:'Cast', val: Any):
+        '''
+        Calls to the type specified in the object `.type` attribute
+        :param self: The cast onject
+        :param val: the value to be casted
+
+        :return: The casted value
+        '''
         try:
-            return Cast.cast(self.type, val)
+            return Cast.cast(val, self.type)
         except Exception as e:
             raise CastingError(
-                f'Exception while casting: {val!r} to {self.type}',
+                f'Exception({e}) while casting: {val!r} to {self.type}',
             ) from e
 
 
-def typeMatch(val, spec):
-    if spec == Any or spec is None:
+def typeMatch(val: Any, spec:type) -> bool:
+    '''
+    recursively checks if type matches
+    :param val: The value to typecheck
+    :param spec: The type specifier
+
+    :return: A boolean
+    '''
+    if spec == Any or spec is None or val is None:
         return True
-    if isinstance(val, tuple):
-        return isinstance(val, tuple)
     if isinstance(spec, Values):
         return spec(val)
     elif isinstance(spec, Validator):
         return spec(val)
     elif isinstance(spec, GenericAlias):
         if not isinstance(val, spec.__origin__):
             return False
-        sub = spec.__args__
-        for val in val:
-            if not typeMatch(val, sub):
-                return False
+
+        if spec.__origin__ == dict:
+            if len(spec.__args__) == 2:
+                kt, vt = spec.__args__
+            elif len(spec.__args__) == 1:
+                kt, vt = Any, spec.__args__[1]
+            else:
+                return True
+
+            for k, v in val.items():
+                if not typeMatch(k, kt) or not typeMatch(v, vt):
+                    return False
+            else:
+                return True
         else:
-            return True
+            sub = spec.__args__[0]
+            for val in val:
+                if not typeMatch(val, sub):
+                    return False
+            else:
+                return True
     else:
         return isinstance(val, spec)
 
 
-def resolveAnnotations(anno, np, scope=None):
-    for k, v in anno.items():
-        if isinstance(v, str):
-            try:
-                anno[k] = eval(v, np, np)
-            except Exception as e:
-                raise AnnotationResolutionError(
-                    f'Exception: {e!s} while resolving annotation {v!r} of {scope}',
-                ) from e
 
+def get_module(obj: Any):
+    '''
+    gets the module to which an object, function or class belongs
+    :param obj: the object
+    :returns: the module
+    '''
+    return sys.modules[obj.__module__]
+
+
+def resolveAnnotations(obj: Any) -> None:
+    '''
+    Evaluates all the stringized annotations of the argument
+
+    :param obj: The object
+    :returns: None
+    '''
+    if isclass(obj) or hasattr(obj, '__class__'):
+        for k, v in obj.__annotations__.items():
+            if isinstance(v, str):
+                try:
+                    obj.__annotations__[k] = eval(v, dict(vars(get_module(obj))), dict(vars(obj)))
+                except Exception as e:
+                    raise AnnotationResolutionError(
+                        f'Exception: {e!s} while resolving'
+                        f' annotation {e}={v!r} of object {obj!r}',
+                    ) from e
+    elif callable(obj):
+        for k, v in obj.__annotations__.items():
+            if isinstance(v, str):
+                try:
+                    obj.__annotations__[k] = eval(v, obj.__globals__)
+                except Exception as e:
+                    raise AnnotationResolutionError(
+                        f'Exception: {k!s} while resolving'
+                        f' annotation {v!r} of function {obj!r}',
+                        f'globals: {obj.__globals__}'
+                    ) from e
+
+
+def annotate(func:callable, oload:bool=False) -> callable:
+    '''
+    returns a wrapper over the passed function
+    which typechecks arguments on each call
+    :param func: the function to annotate
+    :param oload: internal
 
-def annotate(func, oload=False):
-    """decorator annotates wrapped function"""
+    :return: the wrapper function
+    '''
     if isclass(func):
         return annotateClass(func)
     anno = func.__annotations__
+    if len(anno) == 0:
+        return func
 
     @wraps(func)
     def wrapper(*args, **kw):
         names = tuple(anno.keys())
         if any(isinstance(x, str) for x in anno.values()):
-            resolveAnnotations(anno, func.__globals__, get_name(func))
+            resolveAnnotations(func)
         vals = {}
         try:
             if func.__defaults__:
                 for i, v in enumerate(reversed(func.__defaults__)):
                     vals[names[-1 - i]] = v
             for i, v in enumerate(args):
                 vals[names[i]] = v
@@ -163,29 +258,39 @@
         ret = func(**vals)
         if 'return' in anno:
             if not typeMatch(ret, anno['return']):
                 raise AnnotationError(
                     f"return value {ret!r} does not match annotation: {anno['return']} of function {get_name(func)}",
                 )
         return ret
+    wrapper.__pyod_annotate__ = func
     return wrapper
 
 
 __overloads__ = {}
 
 
-def overload(func, name=None):
+def overload(func:callable, name:str|None=None):
+    '''
+    returns a wrapper over the passed function
+    which typechecks arguments on each call
+    and finds the function instance with same name which does not raise
+    an `InternalAnnotationError` exception
+    :param func: the function to annotate
+    :param oload: internal
+
+    :return: the wrapper function
+    '''
     if isinstance(func, str):
         return partial(overload, name=func)
     if name is None or not isinstance(name, str):
         name = get_name(func)
     if name not in __overloads__:
         __overloads__[name] = []
     __overloads__[name].append(annotate(func, True))
-    func.__overloads__ = __overloads__[name]
 
     @wraps(func)
     def wrapper(*args, **kw):
         for f in __overloads__[name]:
             try:
                 val = f(*args, **kw)
             except InternalAnnotationError:
@@ -193,23 +298,33 @@
             else:
                 break
         else:
             raise OverloadError(
                 f'No overload of function: {get_name(func)} matches types of arguments',
             )
         return val
+
+    wrapper.__pyo_overloads__ = __overloads__[name]
+    wrapper.__pyo_overloads_name__ = name
+
     return wrapper
 
 
 def annotateClass(cls):
+    '''
+    Annotates a class object, wrapping and replacing over it's __setattr__
+    and typechecking over each attribute assignment.
+    If no annotation for the passed object found it sets it to `type(val)`
+    '''
+    if not hasattr(cls, '__annotations__'):
+        cls.__annotations__ = {}
     if isinstance(cls, bool):
         return partial(annotate, recur=cls)
     recur = not hasattr(cls, '__annotate_norecur__')
     setter = cls.__setattr__
-    anno = cls.__annotations__
     if recur:
         for x in dir(cls):
             if hasattr(getattr(cls, x), '__annotations__'):
                 setattr(
                     cls,
                     x,
                     annotate(
@@ -217,24 +332,25 @@
                             cls,
                             x,
                         ),
                     ),
                 )
 
     def new_setter(self, name, value):
-        if any(isinstance(x, str) for x in anno.values()):
-            resolveAnnotations(anno, globals(), get_name(cls))
+        if any(isinstance(x, str) for x in self.__annotations__.values()):
+            resolveAnnotations(self)
 
-        if name not in anno:
-            anno[name] = type(value)
-        if not typeMatch(value, anno[name]):
+        if name not in self.__annotations__:
+            if value is not None:
+                self.__annotations__[name] = type(value)
+        elif not typeMatch(value, self.__annotations__[name]):
             raise AnnotationError(
                 f'value {value!r} does not match annotation' +
-                'of attribute: {name!r}:{anno[name]!r} of object of class {get_name(cls)}',
+                f'of attribute: {name!r}:{self.__annotations__[name]!r} of object of class {get_name(cls)}',
             )
-        else:
-            return setter(self, name, value)
+        
+        return setter(self, name, value)
     cls.__setattr__ = new_setter
     return cls
 
 
-__version__ = '1.0.1'
+__version__ = '1.0.2'
```

### Comparing `pyoload-1.0.1/pyoload.egg-info/PKG-INFO` & `pyoload-1.0.2/pyoload.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pyoload
-Version: 1.0.1
+Version: 1.0.2
 Summary: Python package for function argument overload, typechecking and casting
 Home-page: https://github.com/ken-morel/pyoload
 Author: ken-morel
 Author-email: engonken8@gmail.com
 License: MIT
 Classifier: Intended Audience :: Developers
+Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -30,42 +31,42 @@
 Requires-Dist: flake8-commas; extra == "ci"
 Requires-Dist: flake8-quotes; extra == "ci"
 Requires-Dist: flake8-multiline-containers; extra == "ci"
 Requires-Dist: pytest; extra == "ci"
 Requires-Dist: pytest-cov; extra == "ci"
 Requires-Dist: coveralls; extra == "ci"
 
-# pip-package-template-docker
+# pyoload
 
 [![Release Status](https://github.com/ken-morel/pyoload/actions/workflows/python-publish.yml/badge.svg)](https://github.com/ken-morel/pyoload/releases)
 [![PyPI package](https://badge.fury.io/py/pyoload.svg)](https://pypi.org/project/pyoload)
 [![Supported Python versions](https://img.shields.io/pypi/pyversions/pyoload)](https://pypi.org/project/pyoload)
 [![Build Status](https://github.com/ken-morel/pyoload/actions/workflows/test.yml/badge.svg?branch=main)](https://github.com/ken-morel/pyoload/tree/main)
 [![Coverage Status](https://coveralls.io/repos/github/ken-morel/pyoload/badge.svg?branch=main)](https://coveralls.io/github/ken-morel/pyoload?branch=main)
 
 pyoload has two main functions
 
-annotate
-========
+# pyoload.annotate
+
 Is used as a decorator on the function.
 ```python
 
 from pyoload import annotate
 
 @annotate
 def twice(a:int) -> int:
     return a * 2
 
 b = twice(4)
 ```
 The annotate creates a wrapper over the decorated function which checks in for argument types over each function call using `pyoload.matchType(val, spec)`.
 The original function is kept in the `.__pyod_annotate__` attribute.
 
-overload
-========
+# pyoload.overload
+
 Implements function overloading in python via a simple decorator
 
 ```python
 from pyoload import overload
 import math
 cache = {}
 
@@ -83,16 +84,41 @@
 ```
 
 When an overload is registerred, the function name in the form `functionModuleName.functionQualName` is goten using `pyoload.get_name(funcOrClass)` an annotate is gotten using `pyoload.annotate(func, True)`
 and a new list of overloads is created and stored in `pyoload.__overloads__` dictionarry under it's name. A reference to the list of annotated overloads is stored in the functions `.__pyod_overloads__`.
 
 When the function is called, the wrapper tries all the functions registerred to that name to catch a `pyoload.InternalAnnotationError`. If none ran succesfully, it raises an `pyoload.OverloadError`.
 
-Accepted annotations
-====================
+# Casting
+
+All `pyoload.annotate` and `pyoload.overload` both support Cast objects
+instances of `pyoloas.Cast`.
+It uses recursive casting with integrated support for dictionaries, e.g:
+```python
+dict[
+  int,
+  tuple[list[float] | float]
+]
+```
+for a dictionarry mapping of integers to list of floats or floats.
+
+> Note:
+  When a union, e.g `int | str` is passed to Cast, it tries to cast in each of
+  the specified types in the listed order, that is
+
+  ```python
+  cast = pyoload.Cast(int|str)
+  print(repr(cast(3.0)))
+  ```
+
+  Will print `'3.0'` as `3.0` can not be converted to a complex
+
+
+# Accepted annotations
+
 
 In addition to supporting normal plain types,
 pyoload includes support for generic aliasses of iterable types and some other classes:
 
 - `pyoload.Values(iterable)`
   e.g `Values("+-*/")` or `Values(range(6))`
 - `pyoload.Cast(type)`
```

### Comparing `pyoload-1.0.1/setup.py` & `pyoload-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         # See https://pypi.org/classifiers/
 
         'Intended Audience :: Developers',
 
         # 'Development Status :: 1 - Planning',
         # 'Development Status :: 2 - Pre-Alpha',
         # 'Development Status :: 3 - Alpha',
-        # 'Development Status :: 4 - Beta',
+        'Development Status :: 4 - Beta',
         # 'Development Status :: 5 - Production/Stable',
         # 'Development Status :: 6 - Mature',
         # 'Development Status :: 7 - Inactive',
 
         'License :: OSI Approved :: MIT License',
 
         'Programming Language :: Python',
```

