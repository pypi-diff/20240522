# Comparing `tmp/pogo_migrate-0.0.8.tar.gz` & `tmp/pogo_migrate-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pogo_migrate-0.0.8.tar", max compression
+gzip compressed data, was "pogo_migrate-0.0.9.tar", max compression
```

## Comparing `pogo_migrate-0.0.8.tar` & `pogo_migrate-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      819 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/README.md
--rw-r--r--   0        0        0     4269 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/__init__.py
--rw-r--r--   0        0        0    17409 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/cli.py
--rw-r--r--   0        0        0     1705 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/config.py
--rw-r--r--   0        0        0       90 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/exceptions.py
--rw-r--r--   0        0        0     1887 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/migrate.py
--rw-r--r--   0        0        0     5251 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/migration.py
--rw-r--r--   0        0        0     2499 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/sql.py
--rw-r--r--   0        0        0      586 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/testing.py
--rw-r--r--   0        0        0     2987 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/topologicalsort.py
--rw-r--r--   0        0        0     1461 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/util.py
--rw-r--r--   0        0        0     1568 2024-03-10 17:14:03.598597 pogo_migrate-0.0.8/src/pogo_migrate/yoyo.py
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 pogo_migrate-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1261 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/README.md
+-rw-r--r--   0        0        0     4269 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/__init__.py
+-rw-r--r--   0        0        0    17409 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/cli.py
+-rw-r--r--   0        0        0     2054 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/config.py
+-rw-r--r--   0        0        0       90 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/exceptions.py
+-rw-r--r--   0        0        0     1887 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/migrate.py
+-rw-r--r--   0        0        0     5251 2024-03-12 16:35:19.422566 pogo_migrate-0.0.9/src/pogo_migrate/migration.py
+-rw-r--r--   0        0        0     2499 2024-03-12 16:35:19.426566 pogo_migrate-0.0.9/src/pogo_migrate/sql.py
+-rw-r--r--   0        0        0      544 2024-03-12 16:35:19.426566 pogo_migrate-0.0.9/src/pogo_migrate/testing.py
+-rw-r--r--   0        0        0     2987 2024-03-12 16:35:19.426566 pogo_migrate-0.0.9/src/pogo_migrate/topologicalsort.py
+-rw-r--r--   0        0        0     1461 2024-03-12 16:35:19.426566 pogo_migrate-0.0.9/src/pogo_migrate/util.py
+-rw-r--r--   0        0        0     1568 2024-03-12 16:35:19.426566 pogo_migrate-0.0.9/src/pogo_migrate/yoyo.py
+-rw-r--r--   0        0        0     2658 1970-01-01 00:00:00.000000 pogo_migrate-0.0.9/PKG-INFO
```

### Comparing `pogo_migrate-0.0.8/pyproject.toml` & `pogo_migrate-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pogo-migrate"
-version = "0.0.8"
+version = "0.0.9"
 description = "Database migration tool for asyncpg"
 readme = "README.md"
 homepage = "https://github.com/NRWLDev/pogo-migrate"
 authors = [
     "Daniel Edgecombe <daniel@nrwl.co>"
 ]
 maintainers = [
@@ -49,15 +49,15 @@
 
 # Release management
 changelog-gen = {version = "^0.9", extras = ["bump-my-version"]}
 pytest-asyncio = "^0.23.5"
 nest-asyncio = "^1.6.0"
 
 [tool.bumpversion]
-current_version = "0.0.8"
+current_version = "0.0.9"
 commit = true
 tag = true
 parse = '''(?x)
     (?P<major>0|[1-9]\d*)\.
     (?P<minor>0|[1-9]\d*)\.
     (?P<patch>0|[1-9]\d*)
     (?:
```

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/cli.py` & `pogo_migrate-0.0.9/src/pogo_migrate/cli.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/config.py` & `pogo_migrate-0.0.9/src/pogo_migrate/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,29 @@
 CONFIG_FILENAME = "pyproject.toml"
 
 
 @dataclasses.dataclass
 class Config:
     root_directory: Path
     migrations: Path
-    database_env_key: str
+    database_env_key: str | None = None
+    database_config: str | None = None
 
     @property
     def database_dsn(self: t.Self) -> str:
+        if self.database_env_key:
+            try:
+                return os.environ[self.database_env_key]
+            except KeyError as e:
+                msg = f"Configured database_env_key='{self.database_env_key}' not set."
+                raise exceptions.InvalidConfigurationError(msg) from e
         try:
-            return os.environ[self.database_env_key]
+            return self.database_config.format(**os.environ)
         except KeyError as e:
-            msg = f"Configured database_env_key='{self.database_env_key}' not set."
+            msg = f"Configured database_config env var {e!s} not set."
             raise exceptions.InvalidConfigurationError(msg) from e
 
     @classmethod
     def from_dict(cls: type[Config], data: dict, root_directory: Path) -> Config:
         data["root_directory"] = root_directory
         data["migrations"] = root_directory / data["migrations"]
         return cls(**data)
```

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/migrate.py` & `pogo_migrate-0.0.9/src/pogo_migrate/migrate.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/migration.py` & `pogo_migrate-0.0.9/src/pogo_migrate/migration.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/sql.py` & `pogo_migrate-0.0.9/src/pogo_migrate/sql.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/testing.py` & `pogo_migrate-0.0.9/src/pogo_migrate/testing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from __future__ import annotations
 
-import os
 import typing as t
 
 from pogo_migrate import config, migrate, sql
 
 if t.TYPE_CHECKING:
     import asyncpg
 
 
 async def apply(db: asyncpg.Connection | None = None) -> None:
     c = config.load_config()
     if db is None:
-        db = await sql.get_connection(os.environ[c.database_env_key])
+        db = await sql.get_connection(c.database_dsn)
     await migrate.apply(c, db)
 
 
 async def rollback(db: asyncpg.Connection | None = None) -> None:
     c = config.load_config()
     if db is None:
-        db = await sql.get_connection(os.environ[c.database_env_key])
+        db = await sql.get_connection(c.database_dsn)
     await migrate.rollback(c, db)
```

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/topologicalsort.py` & `pogo_migrate-0.0.9/src/pogo_migrate/topologicalsort.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/util.py` & `pogo_migrate-0.0.9/src/pogo_migrate/util.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/src/pogo_migrate/yoyo.py` & `pogo_migrate-0.0.9/src/pogo_migrate/yoyo.py`

 * *Files identical despite different names*

### Comparing `pogo_migrate-0.0.8/PKG-INFO` & `pogo_migrate-0.0.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pogo-migrate
-Version: 0.0.8
+Version: 0.0.9
 Summary: Database migration tool for asyncpg
 Home-page: https://github.com/NRWLDev/pogo-migrate
 License: Apache
 Keywords: migrations,migrate,database,asyncpg,yoyo
 Author: Daniel Edgecombe
 Author-email: daniel@nrwl.co
 Maintainer: Daniel Edgecombe
@@ -38,13 +38,32 @@
 [![image](https://img.shields.io/pypi/l/pogo_migrate.svg)](https://pypi.org/project/pogo_migrate/)
 [![image](https://img.shields.io/pypi/pyversions/pogo_migrate.svg)](https://pypi.org/project/pogo_migrate/)
 ![style](https://github.com/NRWLDev/pogo-migrate/actions/workflows/style.yml/badge.svg)
 ![tests](https://github.com/NRWLDev/pogo-migrate/actions/workflows/tests.yml/badge.svg)
 [![codecov](https://codecov.io/gh/NRWLDev/pogo-migrate/branch/main/graph/badge.svg)](https://codecov.io/gh/NRWLDev/pogo-migrate)
 
 
+## Configuration
+
+Add pogo to pyproject.toml
+
+```toml
+[tool.pogo]
+migrations_location = "./migrations"
+database_env_key = "POSTGRES_DSN"
+```
+
+If you have an existing environment with separate configuration values for
+postgres, you can build the DSN in config.
+
+```toml
+[tool.pogo]
+migrations_location = "./migrations"
+database_config = "postgres://{POSTGRES_USER}:{POSTGRES_PASSWORD}@{POSTGRES_HOST}:{POSTGRES_PORT}/{PORTGRES_DATABASE}"
+```
+
 ## Thanks and Credit
 
 Inspiration for this tool is drawn from
 [yoyo](https://ollycope.com/software/yoyo/latest/) and
 [dbmate](https://github.com/amacneil/dbmate).
```

