# Comparing `tmp/pyodide-py-0.26.0a4.tar.gz` & `tmp/pyodide_py-0.26.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-py-0.26.0a4.tar", last modified: Thu Mar 14 11:06:33 2024, max compression
+gzip compressed data, was "pyodide_py-0.26.0a5.tar", last modified: Tue May 21 20:08:13 2024, max compression
```

## Comparing `pyodide-py-0.26.0a4.tar` & `pyodide_py-0.26.0a5.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:33.828560 pyodide-py-0.26.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-14 11:06:33.828560 pyodide-py-0.26.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:33.824560 pyodide-py-0.26.0a4/_pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19878 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/_base.py
--rw-r--r--   0 runner    (1001) docker     (127)    48709 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/_core_docs.py
--rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/_importhook.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/docs_argspec.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/docstring.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/_pyodide/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:33.824560 pyodide-py-0.26.0a4/pyodide/
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/_package_loader.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/_run_js.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/_state.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/code.py
--rw-r--r--   0 runner    (1001) docker     (127)    20810 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/console.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:33.824560 pyodide-py-0.26.0a4/pyodide/ffi/
--rw-r--r--   0 runner    (1001) docker     (127)     1407 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/ffi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/ffi/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/http.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    21372 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyodide/webloop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:33.828560 pyodide-py-0.26.0a4/pyodide_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-03-14 11:06:33.000000 pyodide-py-0.26.0a4/pyodide_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-03-14 11:06:33.000000 pyodide-py-0.26.0a4/pyodide_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:06:33.000000 pyodide-py-0.26.0a4/pyodide_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-03-14 11:06:33.000000 pyodide-py-0.26.0a4/pyodide_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      876 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 11:06:33.828560 pyodide-py-0.26.0a4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       99 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-03-14 11:06:26.000000 pyodide-py-0.26.0a4/webbrowser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1196 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/_pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19878 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49263 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_core_docs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6940 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/_importhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/docs_argspec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/docstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/jsbind.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/_pyodide/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide/
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12183 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_package_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_run_js.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/code.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20812 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/console.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide/ffi/
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/ffi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3875 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/ffi/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9465 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    21376 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyodide/webloop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 20:08:13.698667 pyodide_py-0.26.0a5/pyodide_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      631 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-21 20:08:13.000000 pyodide_py-0.26.0a5/pyodide_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      876 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 20:08:13.702667 pyodide_py-0.26.0a5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      421 2024-05-21 20:08:06.000000 pyodide_py-0.26.0a5/webbrowser.py
```

### Comparing `pyodide-py-0.26.0a4/PKG-INFO` & `pyodide_py-0.26.0a5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.26.0a4
+Version: 0.26.0a5
 Summary: A Python package providing core interpreter functionality for Pyodide
 Author: Pyodide developers
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.26.0a4/README.md` & `pyodide_py-0.26.0a5/README.md`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/_pyodide/__init__.py` & `pyodide_py-0.26.0a5/_pyodide/__init__.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/_pyodide/_base.py` & `pyodide_py-0.26.0a5/_pyodide/_base.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/_pyodide/_core_docs.py` & `pyodide_py-0.26.0a5/_pyodide/_core_docs.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,14 +112,24 @@
     _js_type_flags: Any = 0
 
     def __new__(cls, arg=None, *args, **kwargs):
         if arg is _instantiate_token:
             return super().__new__(cls)
         raise TypeError(f"{cls.__name__} cannot be instantiated.")
 
+    def bind_sig(self, signature: Any) -> "JsProxy":
+        """Creates a copy of the JsProxy with a signature bound to it.
+
+        .. admonition:: Experimental
+           :class: warning
+
+           This feature is not yet stable, nor really documented.
+        """
+        return self
+
     @property
     def js_id(self) -> int:
         """An id number which can be used as a dictionary/set key if you want to
         key on JavaScript object identity.
 
         If two ``JsProxy`` are made with the same backing JavaScript object, they
         will have the same ``js_id``.
@@ -361,40 +371,36 @@
     """
 
     _js_type_flags = ["IS_AWAITABLE"]
 
     @overload
     def then(
         self, onfulfilled: None, onrejected: Callable[[BaseException], Awaitable[S]], /
-    ) -> "JsPromise[S]":
-        ...
+    ) -> "JsPromise[S]": ...
 
     @overload
     def then(
         self, onfulfilled: None, onrejected: Callable[[BaseException], S], /
-    ) -> "JsPromise[S]":
-        ...
+    ) -> "JsPromise[S]": ...
 
     @overload
     def then(
         self,
         onfulfilled: Callable[[T], Awaitable[S]],
         onrejected: Callable[[BaseException], Awaitable[S]] | None = None,
         /,
-    ) -> "JsPromise[S]":
-        ...
+    ) -> "JsPromise[S]": ...
 
     @overload
     def then(
         self,
         onfulfilled: Callable[[T], S],
         onrejected: Callable[[BaseException], S] | None = None,
         /,
-    ) -> "JsPromise[S]":
-        ...
+    ) -> "JsPromise[S]": ...
 
     @docs_argspec(
         "(self, onfulfilled: Callable[[T], Awaitable[S] | S] | None, onrejected: Callable[[BaseException], Awaitable[S] | S] | None = None, /) -> 'JsPromise[S]'"
     )
     def then(
         self,
         onfulfilled: Any,
@@ -406,20 +412,18 @@
         when the promise resolves.
         """
         pass
 
     @overload
     def catch(
         self, onrejected: Callable[[BaseException], Awaitable[S]], /
-    ) -> "JsPromise[S]":
-        ...
+    ) -> "JsPromise[S]": ...
 
     @overload
-    def catch(self, onrejected: Callable[[BaseException], S], /) -> "JsPromise[S]":
-        ...
+    def catch(self, onrejected: Callable[[BaseException], S], /) -> "JsPromise[S]": ...
 
     @docs_argspec(
         "(self, onrejected: Callable[[BaseException], Awaitable[S] | S], /) -> 'JsPromise[S]'"
     )
     def catch(self, onrejected: Any, /) -> Any:
         """The :js:meth:`Promise.catch` API, wrapped to manage the lifetimes of the
         handler.
@@ -666,26 +670,24 @@
     @overload
     def throw(
         self,
         typ: type[BaseException],
         val: BaseException | object = ...,
         tb: TracebackType | None = ...,
         /,
-    ) -> T_co:
-        ...
+    ) -> T_co: ...
 
     @overload
     def throw(
         self,
         typ: BaseException,
         val: None = ...,
         tb: TracebackType | None = ...,
         /,
-    ) -> T_co:
-        ...
+    ) -> T_co: ...
 
     @docs_argspec("(self, error: BaseException, /) -> T_co")
     def throw(
         self,
         *args: Any,
     ) -> T_co:
         """
@@ -797,26 +799,24 @@
     @overload
     def athrow(
         self,
         typ: type[BaseException],
         val: BaseException | object = ...,
         tb: TracebackType | None = ...,
         /,
-    ) -> Awaitable[T_co]:
-        ...
+    ) -> Awaitable[T_co]: ...
 
     @overload
     def athrow(
         self,
         typ: BaseException,
         val: None = ...,
         tb: TracebackType | None = ...,
         /,
-    ) -> Awaitable[T_co]:
-        ...
+    ) -> Awaitable[T_co]: ...
 
     @docs_argspec("(self, error: BaseException, /) -> T_co")
     def athrow(self, value: Any, *args: Any) -> Awaitable[T_co]:
         """Resumes the execution and raises an exception at the point where the
         generator was paused.
 
         The awaitable returned by ``athrow()`` method will return the next value
@@ -852,31 +852,27 @@
 
 class JsArray(JsIterable[T], Generic[T], MutableSequence[T], metaclass=_ABCMeta):
     """A JsProxy of an :js:class:`Array`, :js:class:`NodeList`, or :js:class:`TypedArray`"""
 
     _js_type_flags = ["IS_ARRAY", "IS_NODE_LIST", "IS_TYPEDARRAY"]
 
     @overload
-    def __getitem__(self, idx: int) -> T:
-        ...
+    def __getitem__(self, idx: int) -> T: ...
 
     @overload
-    def __getitem__(self, idx: slice) -> "JsArray[T]":
-        ...
+    def __getitem__(self, idx: slice) -> "JsArray[T]": ...
 
     def __getitem__(self, idx):
         raise NotImplementedError
 
     @overload
-    def __setitem__(self, idx: int, value: T) -> None:
-        ...
+    def __setitem__(self, idx: int, value: T) -> None: ...
 
     @overload
-    def __setitem__(self, idx: slice, value: Iterable[T]) -> None:
-        ...
+    def __setitem__(self, idx: slice, value: Iterable[T]) -> None: ...
 
     def __setitem__(self, idx, value):
         pass
 
     def __delitem__(self, idx: int | slice) -> None:
         pass
 
@@ -995,33 +991,29 @@
         raise NotImplementedError
 
     def values(self) -> ValuesView[VT_co]:
         """Return a :py:class:`~collections.abc.ValuesView` for the map."""
         raise NotImplementedError
 
     @overload
-    def get(self, key: KT, /) -> VT_co | None:
-        ...
+    def get(self, key: KT, /) -> VT_co | None: ...
 
     @overload
-    def get(self, key: KT, default: VT_co | T, /) -> VT_co | T:
-        ...
+    def get(self, key: KT, default: VT_co | T, /) -> VT_co | T: ...
 
     @docs_argspec("(self, key: KT, default: VT_co | None, /) -> VT_co")
     def get(self, key: KT, default: Any = None, /) -> VT_co:
         r"""If ``key in self``, returns ``self[key]``. Otherwise returns ``default``."""
         raise NotImplementedError
 
 
 class _SupportsKeysAndGetItem(Protocol[KT, VT_co]):
-    def keys(self) -> Iterable[KT]:
-        ...
+    def keys(self) -> Iterable[KT]: ...
 
-    def __getitem__(self, __key: KT) -> VT_co:
-        ...
+    def __getitem__(self, __key: KT) -> VT_co: ...
 
 
 class JsMutableMap(
     JsMap[KT, VT], Generic[KT, VT], MutableMapping[KT, VT], metaclass=_ABCMeta
 ):
     """A JavaScript mutable map
 
@@ -1033,20 +1025,18 @@
     Also proxies returned by :py:meth:`JsProxy.as_object_map` are instances of
     ``JsMap`` .
     """
 
     _js_type_flags = ["HAS_GET | HAS_SET | HAS_LENGTH | IS_ITERABLE", "IS_OBJECT_MAP"]
 
     @overload
-    def pop(self, key: KT, /) -> VT:
-        ...
+    def pop(self, key: KT, /) -> VT: ...
 
     @overload
-    def pop(self, key: KT, default: VT | T = ..., /) -> VT | T:
-        ...
+    def pop(self, key: KT, default: VT | T = ..., /) -> VT | T: ...
 
     @docs_argspec("(self, key: KT, default: VT | None = None, /) -> VT")
     def pop(self, key: KT, default: Any = None, /) -> Any:
         r"""If ``key in self``, return ``self[key]`` and remove key from ``self``. Otherwise
         returns ``default``.
         """
         raise NotImplementedError
@@ -1063,24 +1053,21 @@
         """
         raise NotImplementedError
 
     def clear(self) -> None:
         """Empty out the map entirely."""
 
     @overload
-    def update(self, __m: _SupportsKeysAndGetItem[KT, VT], **kwargs: VT) -> None:
-        ...
+    def update(self, __m: _SupportsKeysAndGetItem[KT, VT], **kwargs: VT) -> None: ...
 
     @overload
-    def update(self, __m: Iterable[tuple[KT, VT]], **kwargs: VT) -> None:
-        ...
+    def update(self, __m: Iterable[tuple[KT, VT]], **kwargs: VT) -> None: ...
 
     @overload
-    def update(self, **kwargs: VT) -> None:
-        ...
+    def update(self, **kwargs: VT) -> None: ...
 
     @docs_argspec(
         "(self, other : Mapping[KT, VT] | Iterable[tuple[KT, VT]] = None , /, **kwargs) -> None"
     )
     def update(self, *args: Any, **kwargs: Any) -> None:
         r"""Updates ``self`` from ``other`` and ``kwargs``.
 
@@ -1205,14 +1192,15 @@
     def style(self) -> Any:
         pass
 
 
 # from pyproxy.c
 
 
+@docs_argspec("(obj: Callable[..., Any], /) -> JsOnceCallable")
 def create_once_callable(
     obj: Callable[..., Any], /, *, _may_syncify: bool = False
 ) -> JsOnceCallable:
     """Wrap a Python Callable in a JavaScript function that can be called once.
 
     After being called the proxy will decrement the reference count
     of the Callable. The JavaScript function also has a ``destroy`` API that
@@ -1273,16 +1261,15 @@
     dict_converter: Callable[[Iterable[JsArray[Any]]], JsProxy] | None = None,
     default_converter: (
         Callable[
             [Any, Callable[[Any], JsProxy], Callable[[Any, JsProxy], None]], JsProxy
         ]
         | None
     ) = None,
-) -> JsArray[Any]:
-    ...
+) -> JsArray[Any]: ...
 
 
 @overload
 def to_js(
     obj: dict[Any, Any],
     /,
     *,
@@ -1292,16 +1279,15 @@
     dict_converter: None,
     default_converter: (
         Callable[
             [Any, Callable[[Any], JsProxy], Callable[[Any, JsProxy], None]], JsProxy
         ]
         | None
     ) = None,
-) -> JsMap[Any, Any]:
-    ...
+) -> JsMap[Any, Any]: ...
 
 
 @overload
 def to_js(
     obj: Any,
     /,
     *,
@@ -1311,16 +1297,15 @@
     dict_converter: Callable[[Iterable[JsArray[Any]]], JsProxy] | None = None,
     default_converter: (
         Callable[
             [Any, Callable[[Any], JsProxy], Callable[[Any, JsProxy], None]], JsProxy
         ]
         | None
     ) = None,
-) -> Any:
-    ...
+) -> Any: ...
 
 
 def to_js(
     obj: Any,
     /,
     *,
     depth: int = -1,
@@ -1492,15 +1477,26 @@
     and :py:func:`to_js`. This method is necessary because indexing the Array from
     Python automatically unwraps the PyProxy into the wrapped Python object.
     """
     pass
 
 
 def run_sync(x: Awaitable[T]) -> T:
-    """Hi!"""
+    """Block until an awaitable is resolved.
+
+    Only works if JS Promise integration is enabled in the runtime and the
+    current Python call stack was entered via :js:func:`pyodide.runPythonAsync`,
+    by calling an async Python function, or via
+    :js:func:`~pyodide.ffi.PyCallable.callPromising`.
+
+    .. admonition:: Experimental
+        :class: warning
+
+        This feature is not yet stable.
+    """
     raise NotImplementedError
 
 
 __name__ = _save_name
 del _save_name
 
 __all__ = [
```

### Comparing `pyodide-py-0.26.0a4/_pyodide/_importhook.py` & `pyodide_py-0.26.0a5/_pyodide/_importhook.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/_pyodide/docs_argspec.py` & `pyodide_py-0.26.0a5/_pyodide/docs_argspec.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/_pyodide/docstring.py` & `pyodide_py-0.26.0a5/_pyodide/docstring.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/__init__.py` & `pyodide_py-0.26.0a5/pyodide/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 #
 # All pure Python code that does not require js or pyodide_js should go in
 # the _pyodide package.
 #
 # This package is imported by the test suite as well, and currently we don't use
 # pytest mocks for js or pyodide_js, so make sure to test "if IN_BROWSER" before
 # importing from these.
-__version__ = "0.26.0a4"
+__version__ = "0.26.0a5"
 
 __all__ = ["__version__", "console", "code", "ffi", "http", "webloop"]
 
 from . import _state  # noqa: F401
 from .webloop import _initialize_event_loop
 
 _initialize_event_loop()
```

### Comparing `pyodide-py-0.26.0a4/pyodide/_package_loader.py` & `pyodide_py-0.26.0a5/pyodide/_package_loader.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/_state.py` & `pyodide_py-0.26.0a5/pyodide/_state.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/code.py` & `pyodide_py-0.26.0a5/pyodide/code.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/console.py` & `pyodide_py-0.26.0a5/pyodide/console.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,17 +279,17 @@
         self.stdin_callback = stdin_callback
         self.stdout_callback = stdout_callback
         self.stderr_callback = stderr_callback
         self.filename = filename
         self.buffer = []
         self._lock = asyncio.Lock()
         self._streams_redirected = False
-        self._stream_generator: Generator[
-            None, None, None
-        ] | None = None  # track persistent stream redirection
+        self._stream_generator: Generator[None, None, None] | None = (
+            None  # track persistent stream redirection
+        )
         if persistent_stream_redirection:
             self.persistent_redirect_streams()
         self._completer = rlcompleter.Completer(self.globals)
         # all nonalphanums except '.'
         # see https://github.com/python/cpython/blob/a4258e8cd776ba655cc54ba54eaeffeddb0a267c/Modules/readline.c#L1211
         self.completer_word_break_characters = (
             """ \t\n`~!@#$%^&*()-=+[{]}\\|;:'\",<>/?"""
```

### Comparing `pyodide-py-0.26.0a4/pyodide/ffi/__init__.py` & `pyodide_py-0.26.0a5/pyodide/ffi/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,11 +50,12 @@
     "JsDomElement",
     "JsCallable",
     "JsTypedArray",
     "create_once_callable",
     "create_proxy",
     "destroy_proxies",
     "to_js",
+    "run_sync",
     "IN_BROWSER",
     "register_js_module",
     "unregister_js_module",
 ]
```

### Comparing `pyodide-py-0.26.0a4/pyodide/ffi/wrappers.py` & `pyodide_py-0.26.0a5/pyodide/ffi/wrappers.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/http.py` & `pyodide_py-0.26.0a5/pyodide/http.py`

 * *Files identical despite different names*

### Comparing `pyodide-py-0.26.0a4/pyodide/webloop.py` & `pyodide_py-0.26.0a5/pyodide/webloop.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,40 +26,36 @@
     """
 
     @overload
     def then(
         self,
         onfulfilled: None,
         onrejected: Callable[[BaseException], Awaitable[S]],
-    ) -> "PyodideFuture[S]":
-        ...
+    ) -> "PyodideFuture[S]": ...
 
     @overload
     def then(
         self,
         onfulfilled: None,
         onrejected: Callable[[BaseException], S],
-    ) -> "PyodideFuture[S]":
-        ...
+    ) -> "PyodideFuture[S]": ...
 
     @overload
     def then(
         self,
         onfulfilled: Callable[[T], Awaitable[S]],
         onrejected: Callable[[BaseException], Awaitable[S]] | None = None,
-    ) -> "PyodideFuture[S]":
-        ...
+    ) -> "PyodideFuture[S]": ...
 
     @overload
     def then(
         self,
         onfulfilled: Callable[[T], S],
         onrejected: Callable[[BaseException], S] | None = None,
-    ) -> "PyodideFuture[S]":
-        ...
+    ) -> "PyodideFuture[S]": ...
 
     def then(
         self,
         onfulfilled: Callable[[T], S | Awaitable[S]] | None,
         onrejected: Callable[[BaseException], S | Awaitable[S]] | None = None,
     ) -> "PyodideFuture[S]":
         """When the Future is done, either execute onfulfilled with the result
@@ -124,20 +120,18 @@
 
         self.add_done_callback(wrapper)
         return result
 
     @overload
     def catch(
         self, onrejected: Callable[[BaseException], Awaitable[S]]
-    ) -> "PyodideFuture[S]":
-        ...
+    ) -> "PyodideFuture[S]": ...
 
     @overload
-    def catch(self, onrejected: Callable[[BaseException], S]) -> "PyodideFuture[S]":
-        ...
+    def catch(self, onrejected: Callable[[BaseException], S]) -> "PyodideFuture[S]": ...
 
     def catch(
         self, onrejected: Callable[[BaseException], object]
     ) -> "PyodideFuture[Any]":
         """Equivalent to ``then(None, onrejected)``"""
         return self.then(None, onrejected)
 
@@ -270,15 +264,15 @@
     #
     # Scheduling methods: use browser.setTimeout to schedule tasks on the browser event loop.
     #
 
     def call_soon(
         self,
         callback: Callable[..., Any],
-        *args: Any,
+        *args: Any,  # type: ignore[override]
         context: contextvars.Context | None = None,
     ) -> asyncio.Handle:
         """Arrange for a callback to be called as soon as possible.
 
         Any positional arguments after the callback will be passed to
         the callback when it is called.
 
@@ -286,15 +280,15 @@
         """
         delay = 0
         return self.call_later(delay, callback, *args, context=context)
 
     def call_soon_threadsafe(
         self,
         callback: Callable[..., Any],
-        *args: Any,
+        *args: Any,  # type: ignore[override]
         context: contextvars.Context | None = None,
     ) -> asyncio.Handle:
         """Like ``call_soon()``, but thread-safe.
 
         We have no threads so everything is "thread safe", and we just use ``call_soon``.
         """
         return self.call_soon(callback, *args, context=context)
```

### Comparing `pyodide-py-0.26.0a4/pyodide_py.egg-info/PKG-INFO` & `pyodide_py-0.26.0a5/pyodide_py.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyodide-py
-Version: 0.26.0a4
+Version: 0.26.0a5
 Summary: A Python package providing core interpreter functionality for Pyodide
 Author: Pyodide developers
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
```

### Comparing `pyodide-py-0.26.0a4/pyodide_py.egg-info/SOURCES.txt` & `pyodide_py-0.26.0a5/pyodide_py.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 ./webbrowser.py
 ./_pyodide/__init__.py
 ./_pyodide/_base.py
 ./_pyodide/_core_docs.py
 ./_pyodide/_importhook.py
 ./_pyodide/docs_argspec.py
 ./_pyodide/docstring.py
+./_pyodide/jsbind.py
 ./_pyodide/py.typed
 ./pyodide/__init__.py
 ./pyodide/_core.py
 ./pyodide/_package_loader.py
 ./pyodide/_run_js.py
 ./pyodide/_state.py
 ./pyodide/code.py
```

### Comparing `pyodide-py-0.26.0a4/pyproject.toml` & `pyodide_py-0.26.0a5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyodide-py"
-version = "0.26.0a4"
+version = "0.26.0a5"
 authors = [{name = "Pyodide developers"}]
 description = "A Python package providing core interpreter functionality for Pyodide"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Operating System :: OS Independent",
 ]
```

