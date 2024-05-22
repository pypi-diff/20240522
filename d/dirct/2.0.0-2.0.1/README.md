# Comparing `tmp/dirct-2.0.0.tar.gz` & `tmp/dirct-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dirct-2.0.0.tar", max compression
+gzip compressed data, was "dirct-2.0.1.tar", max compression
```

## Comparing `dirct-2.0.0.tar` & `dirct-2.0.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0    35149 2023-10-02 12:22:41.491068 dirct-2.0.0/LICENSE
--rw-r--r--   0        0        0     5302 2023-10-02 12:22:41.491068 dirct-2.0.0/README.md
--rw-r--r--   0        0        0      179 2023-10-02 12:22:41.491068 dirct-2.0.0/dirct/__init__.py
--rw-r--r--   0        0        0     1349 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/_base_dirct.py
--rw-r--r--   0        0        0     1358 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/_self_dirct.py
--rw-r--r--   0        0        0     1522 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/_sub_dict.py
--rw-r--r--   0        0        0     3107 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/dirct.py
--rw-r--r--   0        0        0      450 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/exceptions.py
--rw-r--r--   0        0        0      194 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/key_mappers/__init__.py
--rw-r--r--   0        0        0     1587 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/key_mappers/basename_key_mapper.py
--rw-r--r--   0        0        0      347 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/key_mappers/exact_key_mapper.py
--rw-r--r--   0        0        0      502 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/key_mappers/key_mapper.py
--rw-r--r--   0        0        0     1700 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/loaders.py
--rw-r--r--   0        0        0        1 2023-10-02 12:22:41.495069 dirct-2.0.0/dirct/py.typed
--rw-r--r--   0        0        0      818 2023-10-02 12:22:54.779284 dirct-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     6010 1970-01-01 00:00:00.000000 dirct-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 09:18:02.792297 dirct-2.0.1/LICENSE
+-rw-r--r--   0        0        0     5302 2024-05-22 09:18:02.792297 dirct-2.0.1/README.md
+-rw-r--r--   0        0        0      178 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/__init__.py
+-rw-r--r--   0        0        0     1349 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/_base_dirct.py
+-rw-r--r--   0        0        0     1358 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/_self_dirct.py
+-rw-r--r--   0        0        0     1522 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/_sub_dict.py
+-rw-r--r--   0        0        0     3107 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/dirct.py
+-rw-r--r--   0        0        0      450 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/exceptions.py
+-rw-r--r--   0        0        0      194 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/key_mappers/__init__.py
+-rw-r--r--   0        0        0     1587 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/key_mappers/basename_key_mapper.py
+-rw-r--r--   0        0        0      347 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/key_mappers/exact_key_mapper.py
+-rw-r--r--   0        0        0      502 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/key_mappers/key_mapper.py
+-rw-r--r--   0        0        0     1692 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/loaders.py
+-rw-r--r--   0        0        0        1 2024-05-22 09:18:02.792297 dirct-2.0.1/dirct/py.typed
+-rw-r--r--   0        0        0      780 2024-05-22 09:18:10.076369 dirct-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     6041 1970-01-01 00:00:00.000000 dirct-2.0.1/PKG-INFO
```

### Comparing `dirct-2.0.0/LICENSE` & `dirct-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/README.md` & `dirct-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/_base_dirct.py` & `dirct-2.0.1/dirct/_base_dirct.py`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/_self_dirct.py` & `dirct-2.0.1/dirct/_self_dirct.py`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/_sub_dict.py` & `dirct-2.0.1/dirct/_sub_dict.py`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/dirct.py` & `dirct-2.0.1/dirct/dirct.py`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/key_mappers/basename_key_mapper.py` & `dirct-2.0.1/dirct/key_mappers/basename_key_mapper.py`

 * *Files identical despite different names*

### Comparing `dirct-2.0.0/dirct/loaders.py` & `dirct-2.0.1/dirct/loaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,16 +17,15 @@
 
     def __call__(self, path: Path) -> Any:
         if any(path.name.endswith(ext) for ext in self._ext):
             return self.load(path)
         raise UnsupportedFileError
 
     @abstractmethod
-    def load(self, path: Path) -> Any:
-        ...
+    def load(self, path: Path) -> Any: ...
 
 
 class TomlLoader(FileExtensionLoader):
     def __init__(self) -> None:
         super().__init__(".toml")
 
     def load(self, path: Path) -> dict[str, Any]:
```

### Comparing `dirct-2.0.0/pyproject.toml` & `dirct-2.0.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,32 @@
 [tool.poetry]
 name = "dirct"
 # Version is overwritten at build time by CI based on git tag
-version = "2.0.0"
+version = "2.0.1"
 description = "A dict that reflects the contents of a directory."
 authors = ["Abraham Murciano <abrahammurciano@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/abrahammurciano/python-dirct"
 documentation = "https://abrahammurciano.github.io/python-dirct/dirct"
 keywords = []
 
 [tool.poetry.dependencies]
-python = "^3.11"
-pyyaml = "^6.0.1"
-more-itertools = "^10.1.0"
+python = ">=3.11"
+pyyaml = ">=6.0.1"
+more-itertools = ">=10.1.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "*"
 black = "*"
 pdoc3 = "*"
 toml = "*"
 types-toml = "*"
 mypy = "*"
-
-[tool.poetry.group.dev.dependencies]
-types-pyyaml = "^6.0.12.12"
+types-pyyaml = "*"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.mypy]
 exclude = [".venv", "venv"]
```

### Comparing `dirct-2.0.0/PKG-INFO` & `dirct-2.0.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: dirct
-Version: 2.0.0
+Version: 2.0.1
 Summary: A dict that reflects the contents of a directory.
 Home-page: https://github.com/abrahammurciano/python-dirct
 License: GPLv3
 Author: Abraham Murciano
 Author-email: abrahammurciano@gmail.com
-Requires-Python: >=3.11,<4.0
+Requires-Python: >=3.11
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: more-itertools (>=10.1.0,<11.0.0)
-Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: more-itertools (>=10.1.0)
+Requires-Dist: pyyaml (>=6.0.1)
 Project-URL: Documentation, https://abrahammurciano.github.io/python-dirct/dirct
 Project-URL: Repository, https://github.com/abrahammurciano/python-dirct
 Description-Content-Type: text/markdown
 
 # dirct
 A dict that reflects the contents of a directory.
```

