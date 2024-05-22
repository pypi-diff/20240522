# Comparing `tmp/typed-monads-0.4.6.tar.gz` & `tmp/typed_monads-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "typed-monads-0.4.6.tar", last modified: Sun Apr 10 08:35:45 2022, max compression
+gzip compressed data, was "typed_monads-0.4.7.tar", last modified: Wed May 22 07:41:56 2024, max compression
```

## Comparing `typed-monads-0.4.6.tar` & `typed_monads-0.4.7.tar`

### file list

```diff
@@ -1,26 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 08:35:45.421597 typed-monads-0.4.6/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-04-10 08:35:27.000000 typed-monads-0.4.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-04-10 08:35:45.421597 typed-monads-0.4.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     5521 2022-04-10 08:35:27.000000 typed-monads-0.4.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 08:35:45.421597 typed-monads-0.4.6/monads/
--rw-r--r--   0 runner    (1001) docker     (121)      382 2022-04-10 08:35:40.000000 typed-monads-0.4.6/monads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      741 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/applicative.py
--rw-r--r--   0 runner    (1001) docker     (121)     5000 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/currying.py
--rw-r--r--   0 runner    (1001) docker     (121)     2723 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/fastapi.py
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/functor.py
--rw-r--r--   0 runner    (1001) docker     (121)     2093 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/future.py
--rw-r--r--   0 runner    (1001) docker     (121)     3126 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/list.py
--rw-r--r--   0 runner    (1001) docker     (121)     5362 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/maybe.py
--rw-r--r--   0 runner    (1001) docker     (121)     1134 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/monad.py
--rw-r--r--   0 runner    (1001) docker     (121)     2013 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/monoid.py
--rw-r--r--   0 runner    (1001) docker     (121)     2670 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/reader.py
--rw-r--r--   0 runner    (1001) docker     (121)     3964 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/result.py
--rw-r--r--   0 runner    (1001) docker     (121)     3098 2022-04-10 08:35:27.000000 typed-monads-0.4.6/monads/set.py
--rw-r--r--   0 runner    (1001) docker     (121)      151 2022-04-10 08:35:27.000000 typed-monads-0.4.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      189 2022-04-10 08:35:45.421597 typed-monads-0.4.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1257 2022-04-10 08:35:40.000000 typed-monads-0.4.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-04-10 08:35:45.421597 typed-monads-0.4.6/typed_monads.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     6327 2022-04-10 08:35:45.000000 typed-monads-0.4.6/typed_monads.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      420 2022-04-10 08:35:45.000000 typed-monads-0.4.6/typed_monads.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-04-10 08:35:45.000000 typed-monads-0.4.6/typed_monads.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-04-10 08:35:45.000000 typed-monads-0.4.6/typed_monads.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:41:56.462171 typed_monads-0.4.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 07:41:40.000000 typed_monads-0.4.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-22 07:41:56.462171 typed_monads-0.4.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5521 2024-05-22 07:41:40.000000 typed_monads-0.4.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:41:56.462171 typed_monads-0.4.7/monads/
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-05-22 07:41:54.000000 typed_monads-0.4.7/monads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/applicative.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4856 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/currying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/fastapi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/functor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2093 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/future.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3126 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5357 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/maybe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1134 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/monad.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/monoid.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-05-22 07:41:40.000000 typed_monads-0.4.7/monads/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-05-22 07:41:40.000000 typed_monads-0.4.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-22 07:41:56.462171 typed_monads-0.4.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-22 07:41:54.000000 typed_monads-0.4.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:41:56.462171 typed_monads-0.4.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_applicatives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_currying.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_fastapy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_functors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_future.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4018 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_monads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_monoids.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4830 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-22 07:41:40.000000 typed_monads-0.4.7/tests/test_set.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 07:41:56.462171 typed_monads-0.4.7/typed_monads.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6290 2024-05-22 07:41:56.000000 typed_monads-0.4.7/typed_monads.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-05-22 07:41:56.000000 typed_monads-0.4.7/typed_monads.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 07:41:56.000000 typed_monads-0.4.7/typed_monads.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 07:41:56.000000 typed_monads-0.4.7/typed_monads.egg-info/top_level.txt
```

### Comparing `typed-monads-0.4.6/LICENSE` & `typed_monads-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/PKG-INFO` & `typed_monads-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: typed-monads
-Version: 0.4.6
+Version: 0.4.7
 Summary: Type-annotated monad implementations for Python 3.7+
 Home-page: https://github.com/sammyrulez/typed-monads
 Author: Correl Roush, Sam Reghenzi
 Author-email: correl@gmail.com, sammyrulez@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -240,9 +238,7 @@
 for n in Just("one"):
   ...
 
 ```
 
 The same apply for *Results*
 
-
-
```

### Comparing `typed-monads-0.4.6/README.md` & `typed_monads-0.4.7/README.md`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/applicative.py` & `typed_monads-0.4.7/monads/applicative.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/currying.py` & `typed_monads-0.4.7/monads/currying.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,119 +17,101 @@
     def __repr__(self):  # pragma: no cover
         module = self.function.__module__
         name = getattr(self.function, "__name__", repr(self.function))
         signature = inspect.signature(self)
         return f"<Curried {module}.{name}{signature}>"
 
 
-class CurriedUnary(Curried[A, Result]):
-    ...
+class CurriedUnary(Curried[A, Result]): ...
 
 
 class CurriedBinary(Curried[A, CurriedUnary[B, Result]]):
     @overload
-    def __call__(self, environment: A) -> CurriedUnary[B, Result]:
-        ...
+    def __call__(self, environment: A) -> CurriedUnary[B, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B) -> Result:
-        ...
+    def __call__(self, environment: A, b: B) -> Result: ...
 
     def __call__(self, *args):
         return reduce(lambda f, x: f(x), args, self.function)
 
 
 class CurriedTernary(Curried[A, CurriedBinary[B, C, Result]]):
     @overload
-    def __call__(self, environment: A) -> CurriedBinary[B, C, Result]:
-        ...
+    def __call__(self, environment: A) -> CurriedBinary[B, C, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B) -> CurriedUnary[C, Result]:
-        ...
+    def __call__(self, environment: A, b: B) -> CurriedUnary[C, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C) -> Result:
-        ...
+    def __call__(self, environment: A, b: B, c: C) -> Result: ...
 
     def __call__(self, *args):
         return reduce(lambda f, x: f(x), args, self.function)
 
 
 class CurriedQuaternary(Curried[A, CurriedTernary[B, C, D, Result]]):
     @overload
-    def __call__(self, environment: A) -> CurriedTernary[B, C, D, Result]:
-        ...
+    def __call__(self, environment: A) -> CurriedTernary[B, C, D, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B) -> CurriedBinary[C, D, Result]:
-        ...
+    def __call__(self, environment: A, b: B) -> CurriedBinary[C, D, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C) -> CurriedUnary[D, Result]:
-        ...
+    def __call__(self, environment: A, b: B, c: C) -> CurriedUnary[D, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C, d: D) -> Result:
-        ...
+    def __call__(self, environment: A, b: B, c: C, d: D) -> Result: ...
 
     def __call__(self, *args):
         return reduce(lambda f, x: f(x), args, self.function)
 
 
 class CurriedQuinary(Curried[A, CurriedQuaternary[B, C, D, E, Result]]):
     @overload
-    def __call__(self, environment: A) -> CurriedQuaternary[B, C, D, E, Result]:
-        ...
+    def __call__(self, environment: A) -> CurriedQuaternary[B, C, D, E, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B) -> CurriedTernary[C, D, E, Result]:
-        ...
+    def __call__(self, environment: A, b: B) -> CurriedTernary[C, D, E, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C) -> CurriedBinary[D, E, Result]:
-        ...
+    def __call__(self, environment: A, b: B, c: C) -> CurriedBinary[D, E, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C, d: D) -> CurriedUnary[E, Result]:
-        ...
+    def __call__(self, environment: A, b: B, c: C, d: D) -> CurriedUnary[E, Result]: ...
 
     @overload
-    def __call__(self, environment: A, b: B, c: C, d: D, e: E) -> Result:
-        ...
+    def __call__(self, environment: A, b: B, c: C, d: D, e: E) -> Result: ...
 
     def __call__(self, *args):
         return reduce(lambda f, x: f(x), args, self.function)
 
 
 @overload
-def curry(f: Callable[[A], Result]) -> CurriedUnary[A, Result]:
-    ...
+def curry(f: Callable[[A], Result]) -> CurriedUnary[A, Result]: ...
 
 
 @overload
-def curry(f: Callable[[A, B], Result]) -> CurriedBinary[A, B, Result]:
-    ...
+def curry(f: Callable[[A, B], Result]) -> CurriedBinary[A, B, Result]: ...
 
 
 @overload
-def curry(f: Callable[[A, B, C], Result]) -> CurriedTernary[A, B, C, Result]:
-    ...
+def curry(f: Callable[[A, B, C], Result]) -> CurriedTernary[A, B, C, Result]: ...
 
 
 @overload
-def curry(f: Callable[[A, B, C, D], Result]) -> CurriedQuaternary[A, B, C, D, Result]:
-    ...
+def curry(
+    f: Callable[[A, B, C, D], Result]
+) -> CurriedQuaternary[A, B, C, D, Result]: ...
 
 
 @overload
 def curry(
     f: Callable[[A, B, C, D, E], Result]
-) -> CurriedQuinary[A, B, C, D, E, Result]:
-    ...
+) -> CurriedQuinary[A, B, C, D, E, Result]: ...
 
 
 def curry(f):
     signature = inspect.signature(f)
     parameters = list(signature.parameters.values())
 
     def wrapped(args, remaining):
@@ -157,38 +139,35 @@
             else:
                 raise ValueError("Cannot curry a function with more than 5 arguments")
 
     return wrapped([], f.__code__.co_argcount)
 
 
 @overload
-def uncurry(f: CurriedUnary[A, Result]) -> Callable[[A], Result]:
-    ...
+def uncurry(f: CurriedUnary[A, Result]) -> Callable[[A], Result]: ...
 
 
 @overload
-def uncurry(f: CurriedBinary[A, B, Result]) -> Callable[[A, B], Result]:
-    ...
+def uncurry(f: CurriedBinary[A, B, Result]) -> Callable[[A, B], Result]: ...
 
 
 @overload
-def uncurry(f: CurriedTernary[A, B, C, Result]) -> Callable[[A, B, C], Result]:
-    ...
+def uncurry(f: CurriedTernary[A, B, C, Result]) -> Callable[[A, B, C], Result]: ...
 
 
 @overload
-def uncurry(f: CurriedQuaternary[A, B, C, D, Result]) -> Callable[[A, B, C, D], Result]:
-    ...
+def uncurry(
+    f: CurriedQuaternary[A, B, C, D, Result]
+) -> Callable[[A, B, C, D], Result]: ...
 
 
 @overload
 def uncurry(
     f: CurriedQuinary[A, B, C, D, E, Result]
-) -> Callable[[A, B, C, D, E], Result]:
-    ...
+) -> Callable[[A, B, C, D, E], Result]: ...
 
 
 def uncurry(f):
     def wrapped(*args):
         return reduce(lambda _f, x: _f(x), args, f)
 
     return update_wrapper(wrapped, f)
```

### Comparing `typed-monads-0.4.6/monads/fastapi.py` & `typed_monads-0.4.7/monads/fastapi.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/future.py` & `typed_monads-0.4.7/monads/future.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/list.py` & `typed_monads-0.4.7/monads/list.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/maybe.py` & `typed_monads-0.4.7/monads/maybe.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         if isinstance(self, Just):
             return self.value
         else:
             return default
 
     @classmethod
     def fromResult(cls, m: result.Result[T, E]) -> Maybe[T]:
-        return m.map(Maybe.pure).withDefault(Nothing())
+        return m.map(Maybe[T].pure).withDefault(Nothing())
 
     def toResult(self, error: E) -> result.Result[T, E]:
         if isinstance(self, Just):
             return result.Ok(self.value)
         else:
             return result.Err(error)
 
@@ -135,16 +135,15 @@
         if isinstance(self.value, Maybe):
             return cast(Maybe, self.value).flatten()
         else:
             return Just(self.value)
 
 
 class Nothing(Maybe[T]):
-    def __init__(self) -> None:
-        ...
+    def __init__(self) -> None: ...
 
     def __eq__(self, other: object):
         return isinstance(other, Nothing)
 
     def __repr__(self) -> str:  # pragma: no cover
         return "<Nothing>"
```

### Comparing `typed-monads-0.4.6/monads/monad.py` & `typed_monads-0.4.7/monads/monad.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/monoid.py` & `typed_monads-0.4.7/monads/monoid.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/monads/reader.py` & `typed_monads-0.4.7/monads/reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .monad import Monad
 
 T = TypeVar("T")
 S = TypeVar("S")
 Env = TypeVar("Env")
 F = Callable[[Env], T]
 
+
 # TODO Reader Monad Eample
 class Reader(Monad[T], Generic[Env, T]):
     def __init__(self, function: F) -> None:
         update_wrapper(self, function)
         self.function = function
 
     def __call__(self, environment: Env) -> T:
```

### Comparing `typed-monads-0.4.6/monads/result.py` & `typed_monads-0.4.7/monads/result.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         if isinstance(self, Ok):
             return self.value
         else:
             return default
 
     @classmethod
     def fromMaybe(cls, m: maybe.Maybe[T], error: E) -> Result[T, E]:
-        return m.map(Result.pure).withDefault(Err(error))
+        return m.map(Result[T, E].pure).withDefault(Err(error))
 
     def toMaybe(self) -> maybe.Maybe[T]:
         return self.map(maybe.Maybe.pure).withDefault(maybe.Nothing())
 
     @classmethod
     def fromOptional(cls, value: Optional[T], error: E) -> Result[T, E]:
         if value is None:
```

### Comparing `typed-monads-0.4.6/monads/set.py` & `typed_monads-0.4.7/monads/set.py`

 * *Files identical despite different names*

### Comparing `typed-monads-0.4.6/setup.py` & `typed_monads-0.4.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 
 setup(
     name="typed-monads",
-    version="0.4.6",
+    version="0.4.7",
     author="Correl Roush, Sam Reghenzi",
     author_email="correl@gmail.com, sammyrulez@gmail.com",
     description="Type-annotated monad implementations for Python 3.7+",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sammyrulez/typed-monads",
     packages=["monads"],
```

### Comparing `typed-monads-0.4.6/typed_monads.egg-info/PKG-INFO` & `typed_monads-0.4.7/typed_monads.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: typed-monads
-Version: 0.4.6
+Version: 0.4.7
 Summary: Type-annotated monad implementations for Python 3.7+
 Home-page: https://github.com/sammyrulez/typed-monads
 Author: Correl Roush, Sam Reghenzi
 Author-email: correl@gmail.com, sammyrulez@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -240,9 +238,7 @@
 for n in Just("one"):
   ...
 
 ```
 
 The same apply for *Results*
 
-
-
```

