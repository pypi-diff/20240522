# Comparing `tmp/lenient_string_formatter-1.1.0.tar.gz` & `tmp/lenient_string_formatter-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lenient_string_formatter-1.1.0.tar", max compression
+gzip compressed data, was "lenient_string_formatter-1.1.1.tar", max compression
```

## Comparing `lenient_string_formatter-1.1.0.tar` & `lenient_string_formatter-1.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/LICENSE
--rw-r--r--   0        0        0     3784 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/README.md
--rw-r--r--   0        0        0     2065 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/lenient_string_formatter/__init__.py
--rw-r--r--   0        0        0     3041 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/lenient_string_formatter/_disposable_lenient_formatter.py
--rw-r--r--   0        0        0      313 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/lenient_string_formatter/_missing.py
--rw-r--r--   0        0        0        1 2024-04-11 08:39:02.956769 lenient_string_formatter-1.1.0/lenient_string_formatter/py.typed
--rw-r--r--   0        0        0      851 2024-04-11 08:39:12.188837 lenient_string_formatter-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     4618 1970-01-01 00:00:00.000000 lenient_string_formatter-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/LICENSE
+-rw-r--r--   0        0        0     4078 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/README.md
+-rw-r--r--   0        0        0     1955 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/lenient_string_formatter/__init__.py
+-rw-r--r--   0        0        0     3041 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/lenient_string_formatter/_disposable_lenient_formatter.py
+-rw-r--r--   0        0        0      313 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/lenient_string_formatter/_missing.py
+-rw-r--r--   0        0        0        1 2024-05-22 07:24:43.752063 lenient_string_formatter-1.1.1/lenient_string_formatter/py.typed
+-rw-r--r--   0        0        0      851 2024-05-22 07:24:51.472006 lenient_string_formatter-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4912 1970-01-01 00:00:00.000000 lenient_string_formatter-1.1.1/PKG-INFO
```

### Comparing `lenient_string_formatter-1.1.0/LICENSE` & `lenient_string_formatter-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lenient_string_formatter-1.1.0/README.md` & `lenient_string_formatter-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -21,63 +21,66 @@
 
 [![Source Code - GitHub](https://img.shields.io/badge/Source_Code-GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=%23FFFFFF)](https://github.com/abrahammurciano/python-lenient-string-formatter.git)
 
 [![PyPI - lenient-string-formatter](https://img.shields.io/badge/PyPI-lenient_string_formatter-006DAD?style=for-the-badge&logo=PyPI&logoColor=%23FFD242)](https://pypi.org/project/lenient-string-formatter/)
 
 ## Usage
 
-This package provides the `LenientFormatter` class, a subclass of Python's built-in `string.Formatter`. You can use it in the same way as you would use the built-in formatter.
+This package provides a function called `lformat` that you can use to format strings in a lenient way. You can use it in the same way as you would use Python's built-in `str.format` method.
+
+This package also provides the `LenientFormatter` class, a subclass of Python's built-in `string.Formatter`. It is used internally by the `lformat` function, but it can be used directly or subclassed if you need more control over the formatting process.
+
+The examples below will use the `lformat` function. `LenientFormatter().format` can be used in the same way.
 
 ### Basic example
 
 ```python
-from lenient_string_formatter import LenientFormatter
+from lenient_string_formatter import lformat
 
-formatter = LenientFormatter()
 template = "{} {} {a} {b}"
-formatted = formatter.format(template, 1, 2, a=3, b=4)
+formatted = lformat(template, 1, 2, a=3, b=4)
 assert formatted == "1 2 3 4"
 ```
 
 ### Unmatched fields
 
 Unmatched fields are left untouched instead of raising exceptions.
 
 ```python
 template = "{} {} {a} {b}"
-formatted = formatter.format(template, 1, a=3)
+formatted = lformat(template, 1, a=3)
 assert formatted == "1 {} 3 {b}"
 ```
 
 ### Mixing numbered and auto-numbered fields
 
 Explicitly numbered fields are matched according to their index, while auto-numbered fields are matched according to their order in the arguments. They are matched independently of each other.
 
 ```python
 template = "{1} {}"
-formatted = formatter.format(template, 1, 2)
+formatted = lformat(template, 1, 2)
 assert formatted == "2 1"
 ```
 
 ### Unnumbered field with key/attribute access
 
 The built-in formatter raises a KeyError when an unnumbered field is used with key/attribute access. This is a bug in the built-in formatter (https://bugs.python.org/issue27307). This implementation doesn't have this bug.
 
 ```python
 from types import SimpleNamespace
 
 template = "{.attr} {[0]}"
-formatted = formatter.format(template, SimpleNamespace(attr=1), [2])
+formatted = lformat(template, SimpleNamespace(attr=1), [2])
 assert formatted == "1 2"
 ```
 
 ### Format specifiers and conversion flags for unmatched fields
 
 Unmatched fields are left untouched. This includes any format specifiers and conversion flags that are applied to the field. Furthermore, if the field is matched but the format specifier has a field which is unmatched, or vice versa, the field is still left untouched.
 
 For example, below `{a:3}` and `{b!r}` have no matching values, and neither `c=3` nor `f=4` provide enough values to completely fill the fields `{c:{d}}` and `{e:{f}}`, so all fields are left untouched.
 
 ```python
 template = "{a:3} {b!r} {c:{d}} {e:{f}}"
-formatted = formatter.format(template, c=3, f=4)
+formatted = lformat(template, c=3, f=4)
 assert formatted == template
 ```
```

### Comparing `lenient_string_formatter-1.1.0/lenient_string_formatter/__init__.py` & `lenient_string_formatter-1.1.1/lenient_string_formatter/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 """
 .. include:: ../README.md
 """
 
-import importlib.metadata as metadata
 from string import Formatter
 from typing import Any, Mapping, Sequence
 
 from lenient_string_formatter._disposable_lenient_formatter import (
     DisposableLenientFormatter,
 )
 
-__version__ = metadata.version(__package__ or __name__)
-
 
 class LenientFormatter(Formatter):
     """A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising exceptions.
 
     The following exceptions that are normally raised by the built-in string formatter are caught and handled as follows:
 
     - KeyError and IndexError will not be raised if a field in the template is not matched by the arguments. Instead, the field will be left untouched in the output string.
@@ -41,8 +38,8 @@
         format_string: The format string to be formatted.
         *args: The positional arguments to be used for formatting.
         **kwargs: The keyword arguments to be used for formatting.
     """
     return _formatter.format(format_string, *args, **kwargs)
 
 
-__all__ = ("LenientFormatter", "lformat", "__version__")
+__all__ = ("LenientFormatter", "lformat")
```

### Comparing `lenient_string_formatter-1.1.0/lenient_string_formatter/_disposable_lenient_formatter.py` & `lenient_string_formatter-1.1.1/lenient_string_formatter/_disposable_lenient_formatter.py`

 * *Files identical despite different names*

### Comparing `lenient_string_formatter-1.1.0/pyproject.toml` & `lenient_string_formatter-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "lenient-string-formatter"
 # Version is overwritten at build time by CI based on git tag
-version = "1.1.0"
+version = "1.1.1"
 description = "A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising a KeyError."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-lenient-string-formatter"
 documentation = "https://abrahammurciano.github.io/python-lenient-string-formatter/lenient-string-formatter"
 keywords = []
```

### Comparing `lenient_string_formatter-1.1.0/PKG-INFO` & `lenient_string_formatter-1.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lenient-string-formatter
-Version: 1.1.0
+Version: 1.1.1
 Summary: A lenient string formatter that leaves unmatched fields untouched in the output string instead of raising a KeyError.
 Home-page: https://github.com/abrahammurciano/python-lenient-string-formatter
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
@@ -38,63 +38,66 @@
 
 [![Source Code - GitHub](https://img.shields.io/badge/Source_Code-GitHub-181717?style=for-the-badge&logo=GitHub&logoColor=%23FFFFFF)](https://github.com/abrahammurciano/python-lenient-string-formatter.git)
 
 [![PyPI - lenient-string-formatter](https://img.shields.io/badge/PyPI-lenient_string_formatter-006DAD?style=for-the-badge&logo=PyPI&logoColor=%23FFD242)](https://pypi.org/project/lenient-string-formatter/)
 
 ## Usage
 
-This package provides the `LenientFormatter` class, a subclass of Python's built-in `string.Formatter`. You can use it in the same way as you would use the built-in formatter.
+This package provides a function called `lformat` that you can use to format strings in a lenient way. You can use it in the same way as you would use Python's built-in `str.format` method.
+
+This package also provides the `LenientFormatter` class, a subclass of Python's built-in `string.Formatter`. It is used internally by the `lformat` function, but it can be used directly or subclassed if you need more control over the formatting process.
+
+The examples below will use the `lformat` function. `LenientFormatter().format` can be used in the same way.
 
 ### Basic example
 
 ```python
-from lenient_string_formatter import LenientFormatter
+from lenient_string_formatter import lformat
 
-formatter = LenientFormatter()
 template = "{} {} {a} {b}"
-formatted = formatter.format(template, 1, 2, a=3, b=4)
+formatted = lformat(template, 1, 2, a=3, b=4)
 assert formatted == "1 2 3 4"
 ```
 
 ### Unmatched fields
 
 Unmatched fields are left untouched instead of raising exceptions.
 
 ```python
 template = "{} {} {a} {b}"
-formatted = formatter.format(template, 1, a=3)
+formatted = lformat(template, 1, a=3)
 assert formatted == "1 {} 3 {b}"
 ```
 
 ### Mixing numbered and auto-numbered fields
 
 Explicitly numbered fields are matched according to their index, while auto-numbered fields are matched according to their order in the arguments. They are matched independently of each other.
 
 ```python
 template = "{1} {}"
-formatted = formatter.format(template, 1, 2)
+formatted = lformat(template, 1, 2)
 assert formatted == "2 1"
 ```
 
 ### Unnumbered field with key/attribute access
 
 The built-in formatter raises a KeyError when an unnumbered field is used with key/attribute access. This is a bug in the built-in formatter (https://bugs.python.org/issue27307). This implementation doesn't have this bug.
 
 ```python
 from types import SimpleNamespace
 
 template = "{.attr} {[0]}"
-formatted = formatter.format(template, SimpleNamespace(attr=1), [2])
+formatted = lformat(template, SimpleNamespace(attr=1), [2])
 assert formatted == "1 2"
 ```
 
 ### Format specifiers and conversion flags for unmatched fields
 
 Unmatched fields are left untouched. This includes any format specifiers and conversion flags that are applied to the field. Furthermore, if the field is matched but the format specifier has a field which is unmatched, or vice versa, the field is still left untouched.
 
 For example, below `{a:3}` and `{b!r}` have no matching values, and neither `c=3` nor `f=4` provide enough values to completely fill the fields `{c:{d}}` and `{e:{f}}`, so all fields are left untouched.
 
 ```python
 template = "{a:3} {b!r} {c:{d}} {e:{f}}"
-formatted = formatter.format(template, c=3, f=4)
+formatted = lformat(template, c=3, f=4)
 assert formatted == template
 ```
```

