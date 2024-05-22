# Comparing `tmp/insensitive_strenum-1.0.0.tar.gz` & `tmp/insensitive_strenum-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "insensitive_strenum-1.0.0.tar", max compression
+gzip compressed data, was "insensitive_strenum-1.0.1.tar", max compression
```

## Comparing `insensitive_strenum-1.0.0.tar` & `insensitive_strenum-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-10-01 10:46:53.321908 insensitive_strenum-1.0.0/LICENSE
--rw-r--r--   0        0        0     1024 2023-10-01 10:46:53.321908 insensitive_strenum-1.0.0/README.md
--rw-r--r--   0        0        0      534 2023-10-01 10:46:53.321908 insensitive_strenum-1.0.0/insensitive_strenum/__init__.py
--rw-r--r--   0        0        0        1 2023-10-01 10:46:53.321908 insensitive_strenum-1.0.0/insensitive_strenum/py.typed
--rw-r--r--   0        0        0      740 2023-10-01 10:47:04.422141 insensitive_strenum-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     1691 1970-01-01 00:00:00.000000 insensitive_strenum-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 08:18:56.915291 insensitive_strenum-1.0.1/LICENSE
+-rw-r--r--   0        0        0     1024 2024-05-22 08:18:56.915291 insensitive_strenum-1.0.1/README.md
+-rw-r--r--   0        0        0      533 2024-05-22 08:18:56.919291 insensitive_strenum-1.0.1/insensitive_strenum/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-22 08:18:56.919291 insensitive_strenum-1.0.1/insensitive_strenum/py.typed
+-rw-r--r--   0        0        0      741 2024-05-22 08:19:07.767317 insensitive_strenum-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1737 1970-01-01 00:00:00.000000 insensitive_strenum-1.0.1/PKG-INFO
```

### Comparing `insensitive_strenum-1.0.0/LICENSE` & `insensitive_strenum-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `insensitive_strenum-1.0.0/README.md` & `insensitive_strenum-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `insensitive_strenum-1.0.0/insensitive_strenum/__init__.py` & `insensitive_strenum-1.0.1/insensitive_strenum/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 """
 .. include:: ../README.md
 """
 
-
 import importlib.metadata as metadata
 
 __version__ = metadata.version(__package__ or __name__)
 __all__ = ("InsensitiveStrEnum",)
 
 
 from enum import StrEnum
```

### Comparing `insensitive_strenum-1.0.0/pyproject.toml` & `insensitive_strenum-1.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "insensitive-strenum"
 # Version is overwritten at build time by CI based on git tag
-version = "1.0.0"
+version = "1.0.1"
 description = "A case insensitive StrEnum"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-insensitive-strenum"
 documentation = "https://abrahammurciano.github.io/python-insensitive-strenum/insensitive-strenum"
 keywords = []
 
 [tool.poetry.dependencies]
-python = "^3.11"
+python = ">=3.11"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 pdoc3 = "*"
 toml = "*"
 types-toml = "*"
```

### Comparing `insensitive_strenum-1.0.0/PKG-INFO` & `insensitive_strenum-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: insensitive-strenum
-Version: 1.0.0
+Version: 1.0.1
 Summary: A case insensitive StrEnum
 Home-page: https://github.com/abrahammurciano/python-insensitive-strenum
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Project-URL: Documentation, https://abrahammurciano.github.io/python-insensitive-strenum/insensitive-strenum
 Project-URL: Repository, https://github.com/abrahammurciano/python-insensitive-strenum
 Description-Content-Type: text/markdown
 
 # insensitive-strenum
 A case insensitive StrEnum
```

