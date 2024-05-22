# Comparing `tmp/lazymap-1.0.0.tar.gz` & `tmp/lazymap-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazymap-1.0.0.tar", max compression
+gzip compressed data, was "lazymap-1.0.1.tar", max compression
```

## Comparing `lazymap-1.0.0.tar` & `lazymap-1.0.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2024-05-05 16:16:09.163723 lazymap-1.0.0/LICENSE
--rw-r--r--   0        0        0     3390 2024-05-05 16:16:09.163723 lazymap-1.0.0/README.md
--rw-r--r--   0        0        0     4585 2024-05-05 16:16:09.163723 lazymap-1.0.0/lazymap/__init__.py
--rw-r--r--   0        0        0        1 2024-05-05 16:16:09.163723 lazymap-1.0.0/lazymap/py.typed
--rw-r--r--   0        0        0      750 2024-05-05 16:16:20.799845 lazymap-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     4278 1970-01-01 00:00:00.000000 lazymap-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 08:06:48.147073 lazymap-1.0.1/LICENSE
+-rw-r--r--   0        0        0     3390 2024-05-22 08:06:48.147073 lazymap-1.0.1/README.md
+-rw-r--r--   0        0        0     4585 2024-05-22 08:06:48.147073 lazymap-1.0.1/lazymap/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-22 08:06:48.147073 lazymap-1.0.1/lazymap/py.typed
+-rw-r--r--   0        0        0      752 2024-05-22 08:06:56.555237 lazymap-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 lazymap-1.0.1/PKG-INFO
```

### Comparing `lazymap-1.0.0/LICENSE` & `lazymap-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lazymap-1.0.0/README.md` & `lazymap-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `lazymap-1.0.0/lazymap/__init__.py` & `lazymap-1.0.1/lazymap/__init__.py`

 * *Files identical despite different names*

### Comparing `lazymap-1.0.0/pyproject.toml` & `lazymap-1.0.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [tool.poetry]
 name = "lazymap"
 # Version is overwritten at build time by CI based on git tag
-version = "1.0.0"
+version = "1.0.1"
 description = "A lazy mapping whose values are evaluated when accessed"
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-lazymap"
 documentation = "https://abrahammurciano.github.io/python-lazymap/lazymap"
 keywords = []
 
 [tool.poetry.dependencies]
-python = "^3.8"
-typing-extensions = "^4.11.0"
+python = ">=3.8"
+typing-extensions = ">=4.11.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "*"
 black = "*"
 pdoc3 = "*"
 toml = "*"
 types-toml = "*"
```

### Comparing `lazymap-1.0.0/PKG-INFO` & `lazymap-1.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: lazymap
-Version: 1.0.0
+Version: 1.0.1
 Summary: A lazy mapping whose values are evaluated when accessed
 Home-page: https://github.com/abrahammurciano/python-lazymap
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.8
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: typing-extensions (>=4.11.0,<5.0.0)
+Requires-Dist: typing-extensions (>=4.11.0)
 Project-URL: Documentation, https://abrahammurciano.github.io/python-lazymap/lazymap
 Project-URL: Repository, https://github.com/abrahammurciano/python-lazymap
 Description-Content-Type: text/markdown
 
 # lazymap
 
 A lazy mapping whose values are evaluated when accessed
```

