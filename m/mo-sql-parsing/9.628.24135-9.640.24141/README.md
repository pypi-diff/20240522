# Comparing `tmp/mo_sql_parsing-9.628.24135.tar.gz` & `tmp/mo_sql_parsing-9.640.24141.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mo_sql_parsing-9.628.24135.tar", last modified: Tue May 14 02:14:25 2024, max compression
+gzip compressed data, was "mo_sql_parsing-9.640.24141.tar", last modified: Mon May 20 16:35:41 2024, max compression
```

## Comparing `mo_sql_parsing-9.628.24135.tar` & `mo_sql_parsing-9.640.24141.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2024-05-14 02:14:25.538254 mo_sql_parsing-9.628.24135/
--rw-rw-rw-   0        0        0    15922 2024-05-13 01:12:26.000000 mo_sql_parsing-9.628.24135/LICENSE
--rw-rw-rw-   0        0        0    10171 2024-05-14 02:14:25.537129 mo_sql_parsing-9.628.24135/PKG-INFO
--rw-rw-rw-   0        0        0     8521 2024-05-14 02:10:05.000000 mo_sql_parsing-9.628.24135/README.md
-drwxrwxrwx   0        0        0        0 2024-05-14 02:14:25.515867 mo_sql_parsing-9.628.24135/mo_sql_parsing/
--rw-rw-rw-   0        0        0     6723 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/__init__.py
--rw-rw-rw-   0        0        0    25509 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/formatting.py
--rw-rw-rw-   0        0        0    11503 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/keywords.py
--rw-rw-rw-   0        0        0    43041 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/sql_parser.py
--rw-rw-rw-   0        0        0     8811 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/types.py
--rw-rw-rw-   0        0        0    24893 2024-05-14 02:14:17.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/utils.py
--rw-rw-rw-   0        0        0     2949 2024-05-13 01:12:26.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing/windows.py
-drwxrwxrwx   0        0        0        0 2024-05-14 02:14:25.534837 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/
--rw-rw-rw-   0        0        0    10171 2024-05-14 02:14:25.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      434 2024-05-14 02:14:25.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-14 02:14:25.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2024-05-14 02:14:25.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2024-05-14 02:14:25.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/top_level.txt
--rw-rw-rw-   0        0        0        2 2024-04-03 00:09:26.000000 mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/zip-safe
--rw-rw-rw-   0        0        0       42 2024-05-14 02:14:25.538254 mo_sql_parsing-9.628.24135/setup.cfg
--rw-rw-rw-   0        0        0    10166 2024-05-14 02:14:20.000000 mo_sql_parsing-9.628.24135/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/
+-rw-rw-rw-   0        0        0    15922 2024-05-13 01:12:26.000000 mo_sql_parsing-9.640.24141/LICENSE
+-rw-rw-rw-   0        0        0    10151 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/PKG-INFO
+-rw-rw-rw-   0        0        0     8521 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/README.md
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.372149 mo_sql_parsing-9.640.24141/mo_sql_parsing/
+-rw-rw-rw-   0        0        0     6723 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/__init__.py
+-rw-rw-rw-   0        0        0    25509 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/formatting.py
+-rw-rw-rw-   0        0        0    11503 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/keywords.py
+-rw-rw-rw-   0        0        0    43041 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/sql_parser.py
+-rw-rw-rw-   0        0        0     8811 2024-05-14 02:14:17.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/types.py
+-rw-rw-rw-   0        0        0    24893 2024-05-20 16:33:51.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/utils.py
+-rw-rw-rw-   0        0        0     2949 2024-05-13 01:12:26.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing/windows.py
+drwxrwxrwx   0        0        0        0 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/
+-rw-rw-rw-   0        0        0    10151 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      434 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      214 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2024-05-20 16:35:41.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0        2 2024-04-03 00:09:26.000000 mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/zip-safe
+-rw-rw-rw-   0        0        0       42 2024-05-20 16:35:41.415918 mo_sql_parsing-9.640.24141/setup.cfg
+-rw-rw-rw-   0        0        0    10158 2024-05-20 16:35:35.000000 mo_sql_parsing-9.640.24141/setup.py
```

### Comparing `mo_sql_parsing-9.628.24135/LICENSE` & `mo_sql_parsing-9.640.24141/LICENSE`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/PKG-INFO` & `mo_sql_parsing-9.640.24141/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.628.24135
+Version: 9.640.24141
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -14,19 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.578.24081
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-imports==7.546.24057
-Requires-Dist: mo-parsing==8.581.24094
-Provides-Extra: dev
+Requires-Dist: mo-dots==10.632.24139
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-imports==7.584.24095
+Requires-Dist: mo-parsing==8.639.24140
 Provides-Extra: tests
 Requires-Dist: mo-testing==7.562.24075; extra == "tests"
 Requires-Dist: mo-threads==6.570.24076; extra == "tests"
 Requires-Dist: mo-files==6.570.24076; extra == "tests"
 Requires-Dist: mo-streams==1.570.24076; extra == "tests"
 Requires-Dist: zstandard>=0.22.0; extra == "tests"
```

### Comparing `mo_sql_parsing-9.628.24135/README.md` & `mo_sql_parsing-9.640.24141/README.md`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/__init__.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/__init__.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/formatting.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/formatting.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/keywords.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/keywords.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/sql_parser.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/sql_parser.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/types.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/types.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/utils.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/utils.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing/windows.py` & `mo_sql_parsing-9.640.24141/mo_sql_parsing/windows.py`

 * *Files identical despite different names*

### Comparing `mo_sql_parsing-9.628.24135/mo_sql_parsing.egg-info/PKG-INFO` & `mo_sql_parsing-9.640.24141/mo_sql_parsing.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mo-sql-parsing
-Version: 9.628.24135
+Version: 9.640.24141
 Summary: More SQL Parsing! Parse SQL into JSON parse tree
 Home-page: https://github.com/klahnakoski/mo-sql-parsing
 Author: Kyle Lahnakoski
 Author-email: kyle@lahnakoski.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Topic :: Software Development :: Libraries
@@ -14,19 +14,18 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: mo-dots==9.578.24081
-Requires-Dist: mo-future==7.546.24057
-Requires-Dist: mo-imports==7.546.24057
-Requires-Dist: mo-parsing==8.581.24094
-Provides-Extra: dev
+Requires-Dist: mo-dots==10.632.24139
+Requires-Dist: mo-future==7.584.24095
+Requires-Dist: mo-imports==7.584.24095
+Requires-Dist: mo-parsing==8.639.24140
 Provides-Extra: tests
 Requires-Dist: mo-testing==7.562.24075; extra == "tests"
 Requires-Dist: mo-threads==6.570.24076; extra == "tests"
 Requires-Dist: mo-files==6.570.24076; extra == "tests"
 Requires-Dist: mo-streams==1.570.24076; extra == "tests"
 Requires-Dist: zstandard>=0.22.0; extra == "tests"
```

### Comparing `mo_sql_parsing-9.628.24135/setup.py` & `mo_sql_parsing-9.640.24141/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 # THIS FILE IS AUTOGENERATED!
 from setuptools import setup
 setup(
     author='Kyle Lahnakoski',
     author_email='kyle@lahnakoski.com',
     classifiers=["Development Status :: 5 - Production/Stable","Topic :: Software Development :: Libraries","Topic :: Software Development :: Libraries :: Python Modules","Programming Language :: SQL","Programming Language :: Python :: 3.8","Programming Language :: Python :: 3.9","License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)","Programming Language :: Python :: 3.10","Programming Language :: Python :: 3.11","Programming Language :: Python :: 3.12"],
     description='More SQL Parsing! Parse SQL into JSON parse tree',
-    extras_require={"dev":[],"tests":["mo-testing==7.562.24075","mo-threads==6.570.24076","mo-files==6.570.24076","mo-streams==1.570.24076","zstandard>=0.22.0"]},
+    extras_require={"tests":["mo-testing==7.562.24075","mo-threads==6.570.24076","mo-files==6.570.24076","mo-streams==1.570.24076","zstandard>=0.22.0"]},
     include_package_data=True,
-    install_requires=["mo-dots==9.578.24081","mo-future==7.546.24057","mo-imports==7.546.24057","mo-parsing==8.581.24094"],
+    install_requires=["mo-dots==10.632.24139","mo-future==7.584.24095","mo-imports==7.584.24095","mo-parsing==8.639.24140"],
     license='MPL 2.0',
     long_description='# More SQL Parsing!\n\n[![PyPI Latest Release](https://img.shields.io/pypi/v/mo-sql-parsing.svg)](https://pypi.org/project/mo-sql-parsing/)\n[![Build Status](https://app.travis-ci.com/klahnakoski/mo-sql-parsing.svg?branch=master)](https://travis-ci.com/github/klahnakoski/mo-sql-parsing)\n[![Downloads](https://pepy.tech/badge/mo-sql-parsing/month)](https://pepy.tech/project/mo-sql-parsing)\n\n\nParse SQL into JSON so we can translate it for other datastores!\n\n[See changes](https://github.com/klahnakoski/mo-sql-parsing#version-changes-features)\n\n## Objective\n\nThe objective is to convert SQL queries to JSON-izable parse trees. This originally targeted MySQL, but has grown to include other database engines. *Please [paste some SQL into a new issue](https://github.com/klahnakoski/mo-sql-parsing/issues) if it does not work for you*\n\n\n## Project Status\n\nDecember 2023 -  I continue to resolve issues as they are raised. There are [over 1100 tests](https://app.travis-ci.com/github/klahnakoski/mo-sql-parsing), that cover most SQL for most databases, with limited DML and UDF support, including:\n\n  * inner queries, \n  * with clauses, \n  * window functions\n  * create/drop/alter tables and views\n  * insert/update/delete statements\n  * create procedure and function statements (MySQL only)\n\n\n## Install\n\n    pip install mo-sql-parsing\n\n## Parsing SQL\n\n    >>> from mo_sql_parsing import parse\n    >>> parse("select count(1) from jobs")\n    {\'select\': {\'value\': {\'count\': 1}}, \'from\': \'jobs\'}\n    \nEach SQL query is parsed to an object: Each clause is assigned to an object property of the same name. \n\n    >>> parse("select a as hello, b as world from jobs")\n    {\'select\': [{\'value\': \'a\', \'name\': \'hello\'}, {\'value\': \'b\', \'name\': \'world\'}], \'from\': \'jobs\'}\n\nThe `SELECT` clause is an array of objects containing `name` and `value` properties. \n\n\n### SQL Flavours \n\nThere are a few parsing modes you may be interested in:\n\n#### Double-quotes for literal strings\n\nMySQL uses both double quotes and single quotes to declare literal strings.  This is not ansi behaviour, but it is more forgiving for programmers coming from other languages. A specific parse function is provided: \n\n    result = parse_mysql(sql)\n\n#### SQLServer Identifiers (`[]`)\n\nSQLServer uses square brackets to delimit identifiers. For example\n\n    SELECT [Timestamp] FROM [table]\n    \nwhich conflicts with BigQuery array constructor (eg `[1, 2, 3, 4]`). You may use the SqlServer flavour with \n    \n    from mo_sql_parsing import parse_sqlserver as parse\n\n#### NULL is None\n\nThe default output for this parser is to emit a null function `{"null":{}}` wherever `NULL` is encountered in the SQL.  If you would like something different, you can replace nulls with `None` (or anything else for that matter):\n\n    result = parse(sql, null=None)\n    \nthis has been implemented with a post-parse rewriting of the parse tree.\n\n\n#### Normalized function call form\n\nThe default behaviour of the parser is to output function calls in `simple_op` format: The operator being a key in the object; `{op: params}`.  This form can be difficult to work with because the object must be scanned for known operators, or possible optional arguments, or at least distinguished from a query object.\n\nYou can have the parser emit function calls in `normal_op` format\n\n    >>> from mo_sql_parsing import parse, normal_op\n    >>> parse("select trim(\' \' from b+c)", calls=normal_op)\n    \nwhich produces calls in a normalized format\n\n    {"op": op, "args": args, "kwargs": kwargs}\n\nhere is the pretty-printed JSON from the example above:\n\n```\n{\'select\': {\'value\': {\n    \'op\': \'trim\', \n    \'args\': [{\'op\': \'add\', \'args\': [\'b\', \'c\']}], \n    \'kwargs\': {\'characters\': {\'literal\': \' \'}}\n}}}\n```\n\n\n## Generating SQL\n\nYou may also generate SQL from a given JSON document. This is done by the formatter, which is usually lagging the parser (Dec2023).\n\n    >>> from mo_sql_parsing import format\n    >>> format({"from":"test", "select":["a.b", "c"]})\n    \'SELECT a.b, c FROM test\'\n\n## Contributing\n\nIn the event that the parser is not working for you, you can help make this better but simply pasting your sql (or JSON) into a new issue. Extra points if you describe the problem. Even more points if you submit a PR with a test.  If you also submit a fix, then you also have my gratitude. \n\n\n### Run Tests\n\nSee [the tests directory](https://github.com/klahnakoski/mo-sql-parsing/tree/dev/tests) for instructions running tests, or writing new ones.\n\n## More about implementation\n\nSQL queries are translated to JSON objects: Each clause is assigned to an object property of the same name.\n\n    \n    # SELECT * FROM dual WHERE a>b ORDER BY a+b\n    {\n        "select": "*", \n        "from": "dual", \n        "where": {"gt": ["a", "b"]}, \n        "orderby": {"value": {"add": ["a", "b"]}}\n    }\n        \nExpressions are also objects, but with only one property: The name of the operation, and the value holding (an array of) parameters for that operation. \n\n    {op: parameters}\n\nand you can see this pattern in the previous example:\n\n    {"gt": ["a","b"]}\n    \n## Array Programming\n\nThe `mo-sql-parsing.scrub()` method is used liberally throughout the code, and it "simplifies" the JSON.  You may find this form a bit tedious to work with because the JSON property values can be values, lists of values, or missing.  Please consider converting everything to arrays: \n\n\n```\ndef listwrap(value):\n    if value is None:\n        return []\n    elif isinstance(value, list)\n        return value\n    else:\n        return [value]\n```  \n\nthen you may avoid all the is-it-a-list checks :\n\n```\nfor select in listwrap(parsed_result.get(\'select\')):\n    do_something(select)\n```\n\n## Version Changes, Features\n\n\n### Version 10\n\n*December 2023*\n\n`SELECT *` now emits an `all_columns` call instead of plain star (`*`).  \n\n```\n>>> from mo_sql_parsing import parse\n>>> parse("SELECT * FROM table")\n{\'select\': {\'all_columns\': {}}, \'from\': \'table\'}\n```\n\nThis works better with the `except` clause, and is more explicit when selecting all child properties.\n\n``` \n>>> parse("SELECT a.* EXCEPT b FROM table")\n>>> {"select": {"all_columns": "a", "except": "b"}, "from": "table"}\n```\n\nYou may get the original behaviour by staying with version 9, or by using `all_columns="*"`:\n\n```\n>>> parse("SELECT * FROM table", all_columns="*")\n{\'select\': "*", \'from\': \'table\'}\n```\n\n\n### Version 9\n\n*November 2022*\n\nOutput for `COUNT(DISTINCT x)` has changed from function composition\n\n    {"count": {"distinct": x}}\n\nto named parameters\n\n    {"count": x, "distinct": true}\n     \nThis was part of a bug fix [issue142](https://github.com/klahnakoski/mo-sql-parsing/issues/142) - realizing `distinct` is just one parameter of many in an aggregate function. Specifically, using the `calls=normal_op` for clarity:\n    \n    >>> from mo_sql_parsing import parse, normal_op\n    >>> parse("select count(distinct x)", calls=normal_op)\n    \n    {\'select\': {\'value\': {\n        \'op\': \'count\', \n        \'args\': [x], \n        \'kwargs\': {\'distinct\': True}\n    }}}\n\n### Version 8.200+\n\n*September 2022*\n\n* Added `ALTER TABLE` and `COPY` command parsing for Snowflake \n\n\n### Version 8\n \n*November 2021*\n\n* Prefer BigQuery `[]` (create array) over SQLServer `[]` (identity) \n* Added basic DML (`INSERT`/`UPDATE`/`DELETE`)              \n* flatter `CREATE TABLE` structures. The `option` list in column definition has been flattened:<br>\n    **Old column format**\n    \n        {"create table": {\n            "columns": {\n                "name": "name",\n                "type": {"decimal": [2, 3]},\n                "option": [\n                    "not null",\n                    "check": {"lt": [{"length": "name"}, 10]}\n                ]\n            }\n        }}\n        \n    **New column format**\n                \n        {"create table": {\n            "columns": {\n                "name": "name", \n                "type": {"decimal": [2, 3]}\n                "nullable": False,\n                "check": {"lt": [{"length": "name"}, 10]} \n            }\n        }}\n\n### Version 7 \n\n*October 2021*\n\n* changed error reporting; still terrible\n* upgraded mo-parsing library which forced version change\n\n### Version 6 \n\n*October 2021*\n\n* fixed `SELECT DISTINCT` parsing\n* added `DISTINCT ON` parsing\n\n### Version 5 \n\n*August 2021*\n\n* remove inline module `mo-parsing`\n* support `CREATE TABLE`, add SQL "flavours" emit `{null:{}}` for None\n\n### Version 4\n\n*November 2021*\n\n* changed parse result of `SELECT DISTINCT`\n* simpler `ORDER BY` clause in window functions\n',
     long_description_content_type='text/markdown',
     name='mo-sql-parsing',
     packages=["mo_sql_parsing"],
     url='https://github.com/klahnakoski/mo-sql-parsing',
-    version='9.628.24135',
+    version='9.640.24141',
     zip_safe=True
 )
```

