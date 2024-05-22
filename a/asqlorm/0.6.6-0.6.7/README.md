# Comparing `tmp/asqlorm-0.6.6.tar.gz` & `tmp/asqlorm-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asqlorm-0.6.6.tar", max compression
+gzip compressed data, was "asqlorm-0.6.7.tar", max compression
```

## Comparing `asqlorm-0.6.6.tar` & `asqlorm-0.6.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.6/README.md
--rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.6/asqlorm/__init__.py
--rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.6/asqlorm/generator/main.py
--rw-r--r--   0        0        0    44663 2024-05-22 16:32:21.189717 asqlorm-0.6.6/asqlorm/models.py
--rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.6/asqlorm/sql/sql_alchemy.py
--rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.6/asqlorm/utils.py
--rw-r--r--   0        0        0      652 2024-05-22 16:39:17.381231 asqlorm-0.6.6/pyproject.toml
--rw-r--r--   0        0        0      633 1970-01-01 00:00:00.000000 asqlorm-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0        7 2024-02-20 21:09:44.192439 asqlorm-0.6.7/README.md
+-rw-r--r--   0        0        0        0 2024-02-06 21:46:57.101551 asqlorm-0.6.7/asqlorm/__init__.py
+-rw-r--r--   0        0        0    30525 2024-05-08 17:40:16.365136 asqlorm-0.6.7/asqlorm/generator/main.py
+-rw-r--r--   0        0        0    44663 2024-05-22 16:32:21.189717 asqlorm-0.6.7/asqlorm/models.py
+-rw-r--r--   0        0        0     8402 2024-04-24 23:09:35.099688 asqlorm-0.6.7/asqlorm/sql/sql_alchemy.py
+-rw-r--r--   0        0        0     1753 2024-02-24 00:45:59.861298 asqlorm-0.6.7/asqlorm/utils.py
+-rw-r--r--   0        0        0      649 2024-05-22 16:40:35.432712 asqlorm-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0      620 1970-01-01 00:00:00.000000 asqlorm-0.6.7/PKG-INFO
```

### Comparing `asqlorm-0.6.6/asqlorm/generator/main.py` & `asqlorm-0.6.7/asqlorm/generator/main.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.6/asqlorm/models.py` & `asqlorm-0.6.7/asqlorm/models.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.6/asqlorm/sql/sql_alchemy.py` & `asqlorm-0.6.7/asqlorm/sql/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.6/asqlorm/utils.py` & `asqlorm-0.6.7/asqlorm/utils.py`

 * *Files identical despite different names*

### Comparing `asqlorm-0.6.6/pyproject.toml` & `asqlorm-0.6.7/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asqlorm"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = ["Jeremy Berman <jerber@sas.upenn.edu>"]
 readme = "README.md"
 packages = [{ include = 'asqlorm' }]
 exclude = ["tests/**/*"]
 
 
@@ -13,15 +13,15 @@
 pydantic = "^2.7"
 fastgql = "*"
 devtools = "*"
 sqlparse = "*"
 black = "*"
 psycopg = {extras = ["binary"], version = "*"}
 sqlalchemy = "^2.0.29"
-sentry-sdk = {extras = ["sqlalchemy"], version = "^2.1"}
+sentry-sdk = {extras = ["sqlalchemy"], version = "*"}
 greenlet = "^3.0.3"
 asyncpg = "^0.29.0"
 
 [tool.poetry.dev-dependencies]
 mypy = '^1.8'
 ruff = '*'
 doppler-env = '^0.3.1'
```

### Comparing `asqlorm-0.6.6/PKG-INFO` & `asqlorm-0.6.7/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: asqlorm
-Version: 0.6.6
+Version: 0.6.7
 Summary: 
 Author: Jeremy Berman
 Author-email: jerber@sas.upenn.edu
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncpg (>=0.29.0,<0.30.0)
 Requires-Dist: black
 Requires-Dist: devtools
 Requires-Dist: fastgql
 Requires-Dist: greenlet (>=3.0.3,<4.0.0)
 Requires-Dist: psycopg[binary]
 Requires-Dist: pydantic (>=2.7,<3.0)
-Requires-Dist: sentry-sdk[sqlalchemy] (>=2.1,<3.0)
+Requires-Dist: sentry-sdk[sqlalchemy]
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlparse
 Description-Content-Type: text/markdown
 
 sqlorm!
```

