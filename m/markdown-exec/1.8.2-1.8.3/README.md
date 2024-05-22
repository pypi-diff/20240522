# Comparing `tmp/markdown_exec-1.8.2.tar.gz` & `tmp/markdown_exec-1.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "markdown_exec-1.8.2.tar", last modified: Mon May 20 18:15:57 2024, max compression
+gzip compressed data, was "markdown_exec-1.8.3.tar", last modified: Wed May 22 11:36:53 2024, max compression
```

## Comparing `markdown_exec-1.8.2.tar` & `markdown_exec-1.8.3.tar`

### file list

```diff
@@ -1,33 +1,34 @@
--rw-r--r--   0        0        0      754 2024-03-20 15:30:02.179261 markdown_exec-1.8.2/LICENSE
--rw-r--r--   0        0        0     3367 2024-03-20 15:30:04.979225 markdown_exec-1.8.2/README.md
--rw-r--r--   0        0        0     1844 2024-05-20 18:15:57.868931 markdown_exec-1.8.2/pyproject.toml
--rw-r--r--   0        0        0     4366 2024-03-20 15:30:04.982558 markdown_exec-1.8.2/src/markdown_exec/__init__.py
--rw-r--r--   0        0        0     8090 2024-04-15 16:45:33.050727 markdown_exec-1.8.2/src/markdown_exec/ansi.css
--rw-r--r--   0        0        0     2840 2024-03-20 15:30:02.289260 markdown_exec-1.8.2/src/markdown_exec/debug.py
--rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.2/src/markdown_exec/formatters/__init__.py
--rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.2/src/markdown_exec/formatters/base.py
--rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.2/src/markdown_exec/formatters/bash.py
--rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.2/src/markdown_exec/formatters/console.py
--rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.2/src/markdown_exec/formatters/markdown.py
--rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.2/src/markdown_exec/formatters/pycon.py
--rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.2/src/markdown_exec/formatters/pyodide.py
--rw-r--r--   0        0        0     3029 2024-05-20 18:13:12.803878 markdown_exec-1.8.2/src/markdown_exec/formatters/python.py
--rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.2/src/markdown_exec/formatters/sh.py
--rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.2/src/markdown_exec/formatters/tree.py
--rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.2/src/markdown_exec/logger.py
--rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.2/src/markdown_exec/mkdocs_plugin.py
--rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.2/src/markdown_exec/processors.py
--rw-r--r--   0        0        0        0 2024-03-20 15:30:02.292593 markdown_exec-1.8.2/src/markdown_exec/py.typed
--rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.2/src/markdown_exec/pyodide.css
--rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.2/src/markdown_exec/pyodide.js
--rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.2/src/markdown_exec/rendering.py
--rw-r--r--   0        0        0      166 2024-03-20 15:30:02.299260 markdown_exec-1.8.2/tests/__init__.py
--rw-r--r--   0        0        0      635 2024-03-20 15:30:04.982558 markdown_exec-1.8.2/tests/conftest.py
--rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.2/tests/test_base_formatter.py
--rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.2/tests/test_converter.py
--rw-r--r--   0        0        0     4787 2024-05-20 18:02:38.502897 markdown_exec-1.8.2/tests/test_python.py
--rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.2/tests/test_shell.py
--rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.2/tests/test_toc.py
--rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.2/tests/test_tree.py
--rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.2/tests/test_validator.py
--rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 markdown_exec-1.8.2/PKG-INFO
+-rw-r--r--   0        0        0      754 2024-03-20 15:30:02.179261 markdown_exec-1.8.3/LICENSE
+-rw-r--r--   0        0        0     3367 2024-03-20 15:30:04.979225 markdown_exec-1.8.3/README.md
+-rw-r--r--   0        0        0     1844 2024-05-22 11:36:53.699600 markdown_exec-1.8.3/pyproject.toml
+-rw-r--r--   0        0        0     4366 2024-03-20 15:30:04.982558 markdown_exec-1.8.3/src/markdown_exec/__init__.py
+-rw-r--r--   0        0        0     8090 2024-04-15 16:45:33.050727 markdown_exec-1.8.3/src/markdown_exec/ansi.css
+-rw-r--r--   0        0        0     2840 2024-03-20 15:30:02.289260 markdown_exec-1.8.3/src/markdown_exec/debug.py
+-rw-r--r--   0        0        0       51 2023-11-05 16:57:00.630087 markdown_exec-1.8.3/src/markdown_exec/formatters/__init__.py
+-rw-r--r--   0        0        0      323 2024-05-22 11:25:15.318786 markdown_exec-1.8.3/src/markdown_exec/formatters/_exec_python.py
+-rw-r--r--   0        0        0     4761 2023-11-05 16:57:00.653419 markdown_exec-1.8.3/src/markdown_exec/formatters/base.py
+-rw-r--r--   0        0        0      886 2023-11-05 16:57:00.653419 markdown_exec-1.8.3/src/markdown_exec/formatters/bash.py
+-rw-r--r--   0        0        0      815 2023-11-05 16:57:00.670086 markdown_exec-1.8.3/src/markdown_exec/formatters/console.py
+-rw-r--r--   0        0        0      276 2023-11-05 16:57:00.683419 markdown_exec-1.8.3/src/markdown_exec/formatters/markdown.py
+-rw-r--r--   0        0        0      854 2023-11-05 16:57:00.706752 markdown_exec-1.8.3/src/markdown_exec/formatters/pycon.py
+-rw-r--r--   0        0        0     2898 2024-01-05 17:48:17.990589 markdown_exec-1.8.3/src/markdown_exec/formatters/pyodide.py
+-rw-r--r--   0        0        0     3025 2024-05-22 11:25:15.322119 markdown_exec-1.8.3/src/markdown_exec/formatters/python.py
+-rw-r--r--   0        0        0      876 2023-11-05 16:57:00.726752 markdown_exec-1.8.3/src/markdown_exec/formatters/sh.py
+-rw-r--r--   0        0        0     2046 2023-11-05 16:57:00.746751 markdown_exec-1.8.3/src/markdown_exec/formatters/tree.py
+-rw-r--r--   0        0        0     2109 2023-11-05 16:57:00.760085 markdown_exec-1.8.3/src/markdown_exec/logger.py
+-rw-r--r--   0        0        0     4701 2024-01-05 18:36:32.567651 markdown_exec-1.8.3/src/markdown_exec/mkdocs_plugin.py
+-rw-r--r--   0        0        0     4291 2024-01-05 17:35:28.675090 markdown_exec-1.8.3/src/markdown_exec/processors.py
+-rw-r--r--   0        0        0        0 2024-03-20 15:30:02.292593 markdown_exec-1.8.3/src/markdown_exec/py.typed
+-rw-r--r--   0        0        0      849 2024-01-05 17:48:17.990589 markdown_exec-1.8.3/src/markdown_exec/pyodide.css
+-rw-r--r--   0        0        0     3845 2024-01-05 17:48:17.993923 markdown_exec-1.8.3/src/markdown_exec/pyodide.js
+-rw-r--r--   0        0        0     9459 2024-01-05 18:00:40.526407 markdown_exec-1.8.3/src/markdown_exec/rendering.py
+-rw-r--r--   0        0        0      166 2024-03-20 15:30:02.299260 markdown_exec-1.8.3/tests/__init__.py
+-rw-r--r--   0        0        0      635 2024-03-20 15:30:04.982558 markdown_exec-1.8.3/tests/conftest.py
+-rw-r--r--   0        0        0     1443 2023-11-05 16:57:00.873417 markdown_exec-1.8.3/tests/test_base_formatter.py
+-rw-r--r--   0        0        0     2080 2023-11-05 16:57:00.893416 markdown_exec-1.8.3/tests/test_converter.py
+-rw-r--r--   0        0        0     5406 2024-05-22 11:28:38.262455 markdown_exec-1.8.3/tests/test_python.py
+-rw-r--r--   0        0        0     2027 2023-11-05 16:57:00.936749 markdown_exec-1.8.3/tests/test_shell.py
+-rw-r--r--   0        0        0     2335 2023-11-05 16:57:00.983415 markdown_exec-1.8.3/tests/test_toc.py
+-rw-r--r--   0        0        0      488 2023-11-05 16:57:00.983415 markdown_exec-1.8.3/tests/test_tree.py
+-rw-r--r--   0        0        0      995 2023-11-05 16:57:01.013414 markdown_exec-1.8.3/tests/test_validator.py
+-rw-r--r--   0        0        0     4954 1970-01-01 00:00:00.000000 markdown_exec-1.8.3/PKG-INFO
```

### Comparing `markdown_exec-1.8.2/LICENSE` & `markdown_exec-1.8.3/LICENSE`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/README.md` & `markdown_exec-1.8.3/README.md`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/pyproject.toml` & `markdown_exec-1.8.3/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Software Development",
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "pymdown-extensions>=9",
 ]
-version = "1.8.2"
+version = "1.8.3"
 
 [project.license]
 text = "ISC"
 
 [project.optional-dependencies]
 ansi = [
     "pygments-ansi-color",
```

### Comparing `markdown_exec-1.8.2/src/markdown_exec/__init__.py` & `markdown_exec-1.8.3/src/markdown_exec/__init__.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/ansi.css` & `markdown_exec-1.8.3/src/markdown_exec/ansi.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/debug.py` & `markdown_exec-1.8.3/src/markdown_exec/debug.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/base.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/base.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/bash.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/bash.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/console.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/console.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/pycon.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/pycon.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/pyodide.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/pyodide.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/python.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/python.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import traceback
 from collections import defaultdict
 from functools import partial
 from io import StringIO
 from types import ModuleType
 from typing import Any
 
+from markdown_exec.formatters._exec_python import exec_python
 from markdown_exec.formatters.base import ExecutionError, base_format
 from markdown_exec.rendering import code_block
 
 _sessions_globals: dict[str, dict] = defaultdict(dict)
 _sessions_counter: dict[str | None, int] = defaultdict(int)
 _code_blocks: dict[str, list[str]] = {}
 
@@ -63,16 +64,15 @@
     exec_globals["__name__"] = module_name
     sys.modules[module_name] = ModuleType(module_name)
 
     buffer = StringIO()
     exec_globals["print"] = partial(_buffer_print, buffer)
 
     try:
-        compiled = compile(code, filename=code_block_id, mode="exec")
-        exec(compiled, exec_globals)  # noqa: S102
+        exec_python(code, code_block_id, exec_globals)
     except Exception as error:  # noqa: BLE001
         trace = traceback.TracebackException.from_exception(error)
         for frame in trace.stack:
             if frame.filename.startswith("<code block: "):
                 frame._line = _code_blocks[frame.filename][frame.lineno - 1]  # type: ignore[attr-defined,operator]
         raise ExecutionError(code_block("python", "".join(trace.format()), **extra)) from error
     return buffer.getvalue()
```

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/sh.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/sh.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/formatters/tree.py` & `markdown_exec-1.8.3/src/markdown_exec/formatters/tree.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/logger.py` & `markdown_exec-1.8.3/src/markdown_exec/logger.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/mkdocs_plugin.py` & `markdown_exec-1.8.3/src/markdown_exec/mkdocs_plugin.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/processors.py` & `markdown_exec-1.8.3/src/markdown_exec/processors.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/pyodide.css` & `markdown_exec-1.8.3/src/markdown_exec/pyodide.css`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/pyodide.js` & `markdown_exec-1.8.3/src/markdown_exec/pyodide.js`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/src/markdown_exec/rendering.py` & `markdown_exec-1.8.3/src/markdown_exec/rendering.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/conftest.py` & `markdown_exec-1.8.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/test_base_formatter.py` & `markdown_exec-1.8.3/tests/test_base_formatter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/test_converter.py` & `markdown_exec-1.8.3/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/test_python.py` & `markdown_exec-1.8.3/tests/test_python.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for the Python formatters."""
 
 from __future__ import annotations
 
+import re
 from textwrap import dedent
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import pytest
     from markdown import Markdown
 
@@ -199,7 +200,32 @@
 
             print(f"`{func.__module__}`")
             ```
             """,
         ),
     )
     assert "_code_block_n" in html
+
+
+def test_future_annotations_do_not_leak_into_user_code(md: Markdown) -> None:
+    """Assert future annotations do not leak into user code.
+
+    Parameters:
+        md: A Markdown instance (fixture).
+    """
+    html = md.convert(
+        dedent(
+            """
+            ```python exec="1"
+            class Int:
+                ...
+
+            def f(x: Int) -> None:
+                return x + 1.0
+
+            print(f"`{f.__annotations__['x']}`")
+            ```
+            """,
+        ),
+    )
+    assert "<code>Int</code>" not in html
+    assert re.search(r"class '_code_block_n\d+_\.Int'", html)
```

### Comparing `markdown_exec-1.8.2/tests/test_shell.py` & `markdown_exec-1.8.3/tests/test_shell.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/test_toc.py` & `markdown_exec-1.8.3/tests/test_toc.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/tests/test_validator.py` & `markdown_exec-1.8.3/tests/test_validator.py`

 * *Files identical despite different names*

### Comparing `markdown_exec-1.8.2/PKG-INFO` & `markdown_exec-1.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: markdown-exec
-Version: 1.8.2
+Version: 1.8.3
 Summary: Utilities to execute code blocks in Markdown files.
 Keywords: markdown,python,exec,shell,bash,mkdocs
 Author-Email: =?utf-8?q?Timoth=C3=A9e_Mazzucotelli?= <dev@pawamoy.fr>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
```

