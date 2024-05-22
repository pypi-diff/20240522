# Comparing `tmp/sillyorm-0.0.1.tar.gz` & `tmp/sillyorm-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sillyorm-0.0.1.tar", last modified: Mon May 20 23:46:45 2024, max compression
+gzip compressed data, was "sillyorm-0.1.0.tar", last modified: Wed May 22 21:40:53 2024, max compression
```

## Comparing `sillyorm-0.0.1.tar` & `sillyorm-0.1.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:46:45.659172 sillyorm-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-20 23:46:41.000000 sillyorm-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-05-20 23:46:45.659172 sillyorm-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-20 23:46:41.000000 sillyorm-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-20 23:46:41.000000 sillyorm-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 23:46:45.659172 sillyorm-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:46:45.659172 sillyorm-0.0.1/sillyORM.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10953 2024-05-20 23:46:45.000000 sillyorm-0.0.1/sillyORM.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-20 23:46:45.000000 sillyorm-0.0.1/sillyORM.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 23:46:45.000000 sillyorm-0.0.1/sillyORM.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-20 23:46:45.000000 sillyorm-0.0.1/sillyORM.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 23:46:45.000000 sillyorm-0.0.1/sillyORM.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:46:45.659172 sillyorm-0.0.1/sillyorm/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:46:45.659172 sillyorm-0.0.1/sillyorm/dbms/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/dbms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3799 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/dbms/postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/dbms/sqlite.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/environment.py
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     9917 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    22201 2024-05-20 23:46:41.000000 sillyorm-0.0.1/sillyorm/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 23:46:45.659172 sillyorm-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-20 23:46:41.000000 sillyorm-0.0.1/tests/test_add_constraint.py
--rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-20 23:46:41.000000 sillyorm-0.0.1/tests/test_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:40:53.652292 sillyorm-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7652 2024-05-22 21:40:49.000000 sillyorm-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-22 21:40:53.652292 sillyorm-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 21:40:49.000000 sillyorm-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-22 21:40:49.000000 sillyorm-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:40:53.652292 sillyorm-0.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:40:53.648292 sillyorm-0.1.0/sillyORM.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    11160 2024-05-22 21:40:53.000000 sillyorm-0.1.0/sillyORM.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      439 2024-05-22 21:40:53.000000 sillyorm-0.1.0/sillyORM.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:40:53.000000 sillyorm-0.1.0/sillyORM.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-05-22 21:40:53.000000 sillyorm-0.1.0/sillyORM.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-22 21:40:53.000000 sillyorm-0.1.0/sillyORM.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:40:53.648292 sillyorm-0.1.0/sillyorm/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:40:53.648292 sillyorm-0.1.0/sillyorm/dbms/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/dbms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/dbms/postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/dbms/sqlite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/environment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10873 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9050 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22326 2024-05-22 21:40:49.000000 sillyorm-0.1.0/sillyorm/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:40:53.648292 sillyorm-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-22 21:40:49.000000 sillyorm-0.1.0/tests/test_add_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12308 2024-05-22 21:40:49.000000 sillyorm-0.1.0/tests/test_model.py
```

### Comparing `sillyorm-0.0.1/LICENSE` & `sillyorm-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sillyorm-0.0.1/PKG-INFO` & `sillyorm-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sillyORM
-Version: 0.0.1
+Version: 0.1.0
 Summary: an ORM library
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -184,35 +184,35 @@
 Requires-Dist: types-psycopg2; extra == "dev"
 
 # sillyORM
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 ![CI: Python test](https://github.com/theverygaming/sillyORM/actions/workflows/test.yml/badge.svg)
 ![CI: Python mypy](https://github.com/theverygaming/sillyORM/actions/workflows/typecheck.yml/badge.svg)
-
+[![PyPI](https://img.shields.io/pypi/v/sillyorm.svg)](https://pypi.org/project/sillyORM/)
 
 simple ORM library written in Python
 
 Currently supports
 
 - SQLite
 - PostgreSQL
 
-<!-- ## Installation
-
-```bash
-pip install sillyorm
-``` -->
-
 > [!CAUTION]
 > :warning: **sillyORM is not ready for use in production environments**.
 > It is still **alpha software** and under development.
 > The API is unstable, and each release may introduce breaking changes.
 > There may even be **security vulnerabilities** present.
 
+## Installation
+
+```bash
+pip install sillyorm
+```
+
 ## Usage
 
 ```python
 import sillyorm
 from sillyorm.dbms import sqlite
 
 
@@ -236,7 +236,11 @@
 record = env["example"].create({"name": "Hello world!"})
 print(record.name)
 ```
 
 ## Documentation
 
 Read the docs [here](https://theverygaming.github.io/sillyORM/)
+
+> [!NOTE]
+> The docs are always for the _newest_ version.
+> If you need docs for another version you must build them yourself
```

### Comparing `sillyorm-0.0.1/README.md` & `sillyorm-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
 # sillyORM
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 ![CI: Python test](https://github.com/theverygaming/sillyORM/actions/workflows/test.yml/badge.svg)
 ![CI: Python mypy](https://github.com/theverygaming/sillyORM/actions/workflows/typecheck.yml/badge.svg)
-
+[![PyPI](https://img.shields.io/pypi/v/sillyorm.svg)](https://pypi.org/project/sillyORM/)
 
 simple ORM library written in Python
 
 Currently supports
 
 - SQLite
 - PostgreSQL
 
-<!-- ## Installation
-
-```bash
-pip install sillyorm
-``` -->
-
 > [!CAUTION]
 > :warning: **sillyORM is not ready for use in production environments**.
 > It is still **alpha software** and under development.
 > The API is unstable, and each release may introduce breaking changes.
 > There may even be **security vulnerabilities** present.
 
+## Installation
+
+```bash
+pip install sillyorm
+```
+
 ## Usage
 
 ```python
 import sillyorm
 from sillyorm.dbms import sqlite
 
 
@@ -51,7 +51,11 @@
 record = env["example"].create({"name": "Hello world!"})
 print(record.name)
 ```
 
 ## Documentation
 
 Read the docs [here](https://theverygaming.github.io/sillyORM/)
+
+> [!NOTE]
+> The docs are always for the _newest_ version.
+> If you need docs for another version you must build them yourself
```

### Comparing `sillyorm-0.0.1/sillyORM.egg-info/PKG-INFO` & `sillyorm-0.1.0/sillyORM.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sillyORM
-Version: 0.0.1
+Version: 0.1.0
 Summary: an ORM library
 License:                    GNU LESSER GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
          of this license document, but changing it is not allowed.
@@ -184,35 +184,35 @@
 Requires-Dist: types-psycopg2; extra == "dev"
 
 # sillyORM
 
 [![License: LGPL v3](https://img.shields.io/badge/License-LGPL_v3-blue.svg)](https://www.gnu.org/licenses/lgpl-3.0)
 ![CI: Python test](https://github.com/theverygaming/sillyORM/actions/workflows/test.yml/badge.svg)
 ![CI: Python mypy](https://github.com/theverygaming/sillyORM/actions/workflows/typecheck.yml/badge.svg)
-
+[![PyPI](https://img.shields.io/pypi/v/sillyorm.svg)](https://pypi.org/project/sillyORM/)
 
 simple ORM library written in Python
 
 Currently supports
 
 - SQLite
 - PostgreSQL
 
-<!-- ## Installation
-
-```bash
-pip install sillyorm
-``` -->
-
 > [!CAUTION]
 > :warning: **sillyORM is not ready for use in production environments**.
 > It is still **alpha software** and under development.
 > The API is unstable, and each release may introduce breaking changes.
 > There may even be **security vulnerabilities** present.
 
+## Installation
+
+```bash
+pip install sillyorm
+```
+
 ## Usage
 
 ```python
 import sillyorm
 from sillyorm.dbms import sqlite
 
 
@@ -236,7 +236,11 @@
 record = env["example"].create({"name": "Hello world!"})
 print(record.name)
 ```
 
 ## Documentation
 
 Read the docs [here](https://theverygaming.github.io/sillyORM/)
+
+> [!NOTE]
+> The docs are always for the _newest_ version.
+> If you need docs for another version you must build them yourself
```

### Comparing `sillyorm-0.0.1/sillyorm/dbms/postgresql.py` & `sillyorm-0.1.0/sillyorm/dbms/postgresql.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,14 +47,16 @@
         return cast(tuple[Any, ...], res)
 
     def get_table_column_info(self, name: str) -> list[sql.ColumnInfo]:
         def _str_type_to_sql_type(t: str, maxlen: int) -> sql.SqlType:
             match t:
                 case "character varying":
                     return sql.SqlType.varchar(maxlen)
+                case "text":
+                    return sql.SqlType.text()
                 case "integer":
                     return sql.SqlType.integer()
                 case "date":
                     return sql.SqlType.date()
                 case _:
                     raise SillyORMException(f"unknown pg type '{t}'")
```

### Comparing `sillyorm-0.0.1/sillyorm/dbms/sqlite.py` & `sillyorm-0.1.0/sillyorm/dbms/sqlite.py`

 * *Files identical despite different names*

### Comparing `sillyorm-0.0.1/sillyorm/environment.py` & `sillyorm-0.1.0/sillyorm/environment.py`

 * *Files identical despite different names*

### Comparing `sillyorm-0.0.1/sillyorm/fields.py` & `sillyorm-0.1.0/sillyorm/fields.py`

 * *Files 3% similar despite different names*

```diff
@@ -180,14 +180,53 @@
 
     def __set__(self, record: Model, value: str) -> None:
         if not isinstance(value, str):
             raise SillyORMException("String value must be str")
         super().__set__(record, value)
 
 
+class Text(Field):
+    """
+    Text field. Represents a large string of text
+
+    .. testcode:: models_fields
+
+       class ExampleModel(sillyorm.model.Model):
+           _name = "example_text"
+           field = sillyorm.fields.Text()
+
+       env.register_model(ExampleModel)
+
+       record = env["example_text"].create({"field": "hello"})
+       print(record.field)
+       record.field += " world!"
+       print(record.field)
+
+       largestring = "0123456789" * 100000 # 1MB of data
+       record.field = largestring
+       print(record.field == largestring)
+
+    .. testoutput:: models_fields
+
+       hello
+       hello world!
+       True
+
+    """
+
+    def __init__(self) -> None:
+        self.sql_type = sql.SqlType.text()
+        super().__init__()
+
+    def __set__(self, record: Model, value: str) -> None:
+        if not isinstance(value, str):
+            raise SillyORMException("Text value must be str")
+        super().__set__(record, value)
+
+
 class Date(Field):
     """
     Date field. Represents a python date object.
 
     .. testcode:: models_fields
 
        import datetime
```

### Comparing `sillyorm-0.0.1/sillyorm/model.py` & `sillyorm-0.1.0/sillyorm/model.py`

 * *Files identical despite different names*

### Comparing `sillyorm-0.0.1/sillyorm/sql.py` & `sillyorm-0.1.0/sillyorm/sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,14 +43,21 @@
 
         :param length: The maximum length
         :type length: int
         """
         return SqlType(f"VARCHAR({length})")
 
     @staticmethod
+    def text() -> SqlType:
+        """
+        `TEXT` SQL type
+        """
+        return SqlType("TEXT")
+
+    @staticmethod
     def date() -> SqlType:
         """
         `DATE` SQL type
 
         .. warning::
            some DBMS include a timestamp for DATE
         """
```

### Comparing `sillyorm-0.0.1/tests/test_add_constraint.py` & `sillyorm-0.1.0/tests/test_add_constraint.py`

 * *Files identical despite different names*

### Comparing `sillyorm-0.0.1/tests/test_model.py` & `sillyorm-0.1.0/tests/test_model.py`

 * *Files identical despite different names*

