# Comparing `tmp/types-pep8-naming-0.13.0.5.tar.gz` & `tmp/types-pep8-naming-0.14.0.20240522.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-pep8-naming-0.13.0.5.tar", last modified: Thu Jul 20 15:16:54 2023, max compression
+gzip compressed data, was "types-pep8-naming-0.14.0.20240522.tar", last modified: Wed May 22 02:22:19 2024, max compression
```

## Comparing `types-pep8-naming-0.13.0.5.tar` & `types-pep8-naming-0.14.0.20240522.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-20 15:16:53.000000 types-pep8-naming-0.13.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:16:54.225600 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:16:54.000000 types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:19.124894 types-pep8-naming-0.14.0.20240522/
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 02:22:19.124894 types-pep8-naming-0.14.0.20240522/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:19.120895 types-pep8-naming-0.14.0.20240522/pep8ext_naming-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      144 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/pep8ext_naming-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/pep8ext_naming-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/pep8ext_naming-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 02:22:19.124894 types-pep8-naming-0.14.0.20240522/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-05-22 02:22:18.000000 types-pep8-naming-0.14.0.20240522/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 02:22:19.120895 types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-05-22 02:22:19.000000 types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-22 02:22:19.000000 types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 02:22:19.000000 types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-22 02:22:19.000000 types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/top_level.txt
```

### Comparing `types-pep8-naming-0.13.0.5/CHANGELOG.md` & `types-pep8-naming-0.14.0.20240522/CHANGELOG.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## 0.14.0.20240522 (2024-05-22)
+
+[stubsabot] Bump pep8-naming to 0.14.* (#11924)
+
 ## 0.13.0.5 (2023-07-20)
 
 Add an upstream_repository field to METADATA.toml (#10487)
 
 Closes: #10478
 
 ## 0.13.0.4 (2023-05-10)
```

### Comparing `types-pep8-naming-0.13.0.5/PKG-INFO` & `types-pep8-naming-0.14.0.20240522/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: types-pep8-naming
-Version: 0.13.0.5
+Version: 0.14.0.20240522
 Summary: Typing stubs for pep8-naming
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for pep8-naming
 
-This is a PEP 561 type stub package for the `pep8-naming` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pep8-naming`](https://github.com/PyCQA/pep8-naming) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pep8-naming`. The source for this package can be found at
+`pep8-naming`.
+
+This version of `types-pep8-naming` aims to provide accurate annotations
+for `pep8-naming==0.14.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

### Comparing `types-pep8-naming-0.13.0.5/pep8ext_naming-stubs/__init__.pyi` & `types-pep8-naming-0.14.0.20240522/pep8ext_naming-stubs/__init__.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 from _typeshed import Incomplete
 from argparse import Namespace
 from collections.abc import Generator, Iterable
 from typing import Any
 
 __version__: str
 
-PYTHON_VERSION: tuple[int, int, int]
 CLASS_METHODS: frozenset[str]
 METACLASS_BASES: frozenset[str]
 METHOD_CONTAINER_NODES: set[ast.AST]
 
 class NamingChecker:
     name: str
     version: str
```

### Comparing `types-pep8-naming-0.13.0.5/setup.py` & `types-pep8-naming-0.14.0.20240522/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,49 +1,55 @@
 from setuptools import setup
 
 name = "types-pep8-naming"
 description = "Typing stubs for pep8-naming"
 long_description = '''
 ## Typing stubs for pep8-naming
 
-This is a PEP 561 type stub package for the `pep8-naming` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pep8-naming`](https://github.com/PyCQA/pep8-naming) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pep8-naming`. The source for this package can be found at
+`pep8-naming`.
+
+This version of `types-pep8-naming` aims to provide accurate annotations
+for `pep8-naming==0.14.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="0.13.0.5",
+      version="0.14.0.20240522",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=[],
       packages=['pep8ext_naming-stubs'],
       package_data={'pep8ext_naming-stubs': ['__init__.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
+      python_requires=">=3.8",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-pep8-naming-0.13.0.5/types_pep8_naming.egg-info/PKG-INFO` & `types-pep8-naming-0.14.0.20240522/types_pep8_naming.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 Metadata-Version: 2.1
 Name: types-pep8-naming
-Version: 0.13.0.5
+Version: 0.14.0.20240522
 Summary: Typing stubs for pep8-naming
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/pep8-naming.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Typing :: Stubs Only
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 ## Typing stubs for pep8-naming
 
-This is a PEP 561 type stub package for the `pep8-naming` package. It
-can be used by type-checking tools like
+This is a [PEP 561](https://peps.python.org/pep-0561/)
+type stub package for the [`pep8-naming`](https://github.com/PyCQA/pep8-naming) package.
+It can be used by type-checking tools like
 [mypy](https://github.com/python/mypy/),
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
-`pep8-naming`. The source for this package can be found at
+`pep8-naming`.
+
+This version of `types-pep8-naming` aims to provide accurate annotations
+for `pep8-naming==0.14.*`.
+The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/pep8-naming. All fixes for
 types and metadata should be contributed there.
 
 This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
 If you find that annotations are missing, feel free to contribute and help complete them.
 
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
-with mypy 1.4.1, pyright 1.1.318, and
-pytype 2023.6.16.
+This package was generated from typeshed commit `489e8dbf41d3350388331b2303bd4f3d13ecbfff` and was tested
+with mypy 1.10.0, pyright 1.1.363, and
+pytype 2024.4.11.
```

