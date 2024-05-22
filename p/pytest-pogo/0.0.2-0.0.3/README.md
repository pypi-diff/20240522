# Comparing `tmp/pytest_pogo-0.0.2.tar.gz` & `tmp/pytest_pogo-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_pogo-0.0.2.tar", max compression
+gzip compressed data, was "pytest_pogo-0.0.3.tar", max compression
```

## Comparing `pytest_pogo-0.0.2.tar` & `pytest_pogo-0.0.3.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      812 2024-03-11 11:12:22.461009 pytest_pogo-0.0.2/README.md
--rw-r--r--   0        0        0     2835 2024-03-11 11:12:22.461009 pytest_pogo-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      414 2024-03-11 11:12:22.461009 pytest_pogo-0.0.2/pytest_pogo/__init__.py
--rw-r--r--   0        0        0     1957 1970-01-01 00:00:00.000000 pytest_pogo-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      938 2024-05-22 09:56:53.348272 pytest_pogo-0.0.3/README.md
+-rw-r--r--   0        0        0     2835 2024-05-22 09:56:53.352272 pytest_pogo-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1218 2024-05-22 09:56:53.352272 pytest_pogo-0.0.3/pytest_pogo/__init__.py
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 pytest_pogo-0.0.3/PKG-INFO
```

### Comparing `pytest_pogo-0.0.2/README.md` & `pytest_pogo-0.0.3/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # Pytest plugin for Pogo migrate - asyncpg migration tooling
-[![image](https://img.shields.io/pypi/v/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
-[![image](https://img.shields.io/pypi/l/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
-[![image](https://img.shields.io/pypi/pyversions/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
+[![image](https://img.shields.io/pypi/v/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
+[![image](https://img.shields.io/pypi/l/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
+[![image](https://img.shields.io/pypi/pyversions/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
 ![style](https://github.com/NRWLDev/pytest-pogo/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/pytest-pogo/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/pytest-pogo/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/pytest-pogo)
 
 
 Provides `pogo_engine` fixture which will apply local migrations at the start
 of the test session, and roll them back at the end.
+
+Additionally provides `pogo_engine_verbose` fixture, if migrations do not
+appear to be applying correctly, this will capture the verbose logs.
```

### Comparing `pytest_pogo-0.0.2/pyproject.toml` & `pytest_pogo-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pytest-pogo"
-version = "0.0.2"
+version = "0.0.3"
 description = "Pytest plugin for pogo-migrate"
 readme = "README.md"
 homepage = "https://github.com/NRWLDev/pytest-pogo"
 authors = [
     "Daniel Edgecombe <daniel@nrwl.co>"
 ]
 maintainers = [
@@ -41,15 +41,15 @@
 pre-commit = "^3.0.2"
 
 # Release management
 changelog-gen = {version = "^0.9", extras = ["bump-my-version"]}
 asyncpg = "^0.29.0"
 
 [tool.bumpversion]
-current_version = "0.0.2"
+current_version = "0.0.3"
 commit = true
 tag = true
 
 [[tool.bumpversion.files]]
 filename = "pyproject.toml"
 search = 'version = "{current_version}"'
 replace = 'version = "{new_version}"'
@@ -66,15 +66,15 @@
 commit_link = "https://github.com/NRWLDev/pytest-pogo/commit/::commit_hash::"
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 testpaths = ["tests"]
 addopts = "--random-order"
 env = [
-    "D:POSTGRES_DSN=postgres://unit:password@localhost:5435/unit",
+    "D:POSTGRES_DSN=postgres://unit:password@localhost:5436/unit",
 ]
 
 
 [tool.coverage.report]
 sort = "cover"
 fail_under = 99
 show_missing = true
```

### Comparing `pytest_pogo-0.0.2/PKG-INFO` & `pytest_pogo-0.0.3/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-pogo
-Version: 0.0.2
+Version: 0.0.3
 Summary: Pytest plugin for pogo-migrate
 Home-page: https://github.com/NRWLDev/pytest-pogo
 License: Apache
 Keywords: migrations,migrate,database,asyncpg,pytest
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Maintainer: Daniel Edgecombe
@@ -25,18 +25,21 @@
 Classifier: Topic :: Software Development
 Classifier: Topic :: Software Development :: Version Control
 Requires-Dist: pogo-migrate (>=0.0.8,<1.0.0)
 Requires-Dist: pytest (>=7,<9)
 Description-Content-Type: text/markdown
 
 # Pytest plugin for Pogo migrate - asyncpg migration tooling
-[![image](https://img.shields.io/pypi/v/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
-[![image](https://img.shields.io/pypi/l/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
-[![image](https://img.shields.io/pypi/pyversions/pytest-migrate.svg)](https://pypi.org/project/pytest-migrate/)
+[![image](https://img.shields.io/pypi/v/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
+[![image](https://img.shields.io/pypi/l/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
+[![image](https://img.shields.io/pypi/pyversions/pytest-pogo.svg)](https://pypi.org/project/pytest-pogo/)
 ![style](https://github.com/NRWLDev/pytest-pogo/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/pytest-pogo/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/pytest-pogo/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/pytest-pogo)
 
 
 Provides `pogo_engine` fixture which will apply local migrations at the start
 of the test session, and roll them back at the end.
 
+Additionally provides `pogo_engine_verbose` fixture, if migrations do not
+appear to be applying correctly, this will capture the verbose logs.
+
```

