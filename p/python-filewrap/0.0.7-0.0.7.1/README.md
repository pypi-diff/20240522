# Comparing `tmp/python_filewrap-0.0.7.tar.gz` & `tmp/python_filewrap-0.0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_filewrap-0.0.7.tar", max compression
+gzip compressed data, was "python_filewrap-0.0.7.1.tar", max compression
```

## Comparing `python_filewrap-0.0.7.tar` & `python_filewrap-0.0.7.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.7/LICENSE
--rwxr-xr-x   0        0        0    16575 2024-05-19 10:27:45.457631 python_filewrap-0.0.7/filewrap/__init__.py
--rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.7/filewrap/py.typed
--rw-r--r--   0        0        0     1171 2024-05-19 10:28:03.090629 python_filewrap-0.0.7/pyproject.toml
--rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.7/readme.md
--rw-r--r--   0        0        0     1362 1970-01-01 00:00:00.000000 python_filewrap-0.0.7/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 python_filewrap-0.0.7.1/LICENSE
+-rwxr-xr-x   0        0        0    16632 2024-05-22 17:10:33.789304 python_filewrap-0.0.7.1/filewrap/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-30 04:55:37.590943 python_filewrap-0.0.7.1/filewrap/py.typed
+-rw-r--r--   0        0        0     1173 2024-05-22 17:11:00.216885 python_filewrap-0.0.7.1/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-05-14 10:43:51.477479 python_filewrap-0.0.7.1/readme.md
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 python_filewrap-0.0.7.1/PKG-INFO
```

### Comparing `python_filewrap-0.0.7/LICENSE` & `python_filewrap-0.0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `python_filewrap-0.0.7/filewrap/__init__.py` & `python_filewrap-0.0.7.1/filewrap/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,32 +17,34 @@
 from collections.abc import Awaitable, AsyncIterable, Iterable
 from functools import update_wrapper
 from inspect import isawaitable, iscoroutinefunction
 from itertools import chain
 from collections.abc import AsyncIterator, Callable, Iterator
 from shutil import COPY_BUFSIZE # type: ignore
 from threading import Lock
-from typing import Any, Protocol, TypeVar
+from typing import runtime_checkable, Any, Protocol, TypeVar
 
 try:
     from collections.abc import Buffer # type: ignore
 except ImportError:
     Buffer = Any
 
 from asynctools import async_chain, ensure_async, ensure_aiter
 
 
 _T_co = TypeVar("_T_co", covariant=True)
 _T_contra = TypeVar("_T_contra", contravariant=True)
 
 
+@runtime_checkable
 class SupportsRead(Protocol[_T_co]):
     def read(self, __length: int = ...) -> _T_co: ...
 
 
+@runtime_checkable
 class SupportsWrite(Protocol[_T_contra]):
     def write(self, __s: _T_contra) -> object: ...
 
 
 def bio_chunk_iter(
     bio: SupportsRead[Buffer] | Callable[[int], Buffer], 
     /,
```

### Comparing `python_filewrap-0.0.7/pyproject.toml` & `python_filewrap-0.0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-filewrap"
-version = "0.0.7"
+version = "0.0.7.1"
 description = "Python file wrappers."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap"
 keywords = ["file", "wrapper"]
```

### Comparing `python_filewrap-0.0.7/PKG-INFO` & `python_filewrap-0.0.7.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-filewrap
-Version: 0.0.7
+Version: 0.0.7.1
 Summary: Python file wrappers.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/python-filewrap
 License: MIT
 Keywords: file,wrapper
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Requires-Python: >=3.10,<4.0
```

