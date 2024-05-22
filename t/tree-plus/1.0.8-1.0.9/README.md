# Comparing `tmp/tree_plus-1.0.8.tar.gz` & `tmp/tree_plus-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tree_plus-1.0.8.tar", last modified: Mon Dec 25 01:41:28 2023, max compression
+gzip compressed data, was "tree_plus-1.0.9.tar", last modified: Mon Dec 25 20:57:36 2023, max compression
```

## Comparing `tree_plus-1.0.8.tar` & `tree_plus-1.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 01:41:28.535864 tree_plus-1.0.8/
--rw-r--r--   0 bion      (1000) bion      (1000)    10984 2023-05-27 13:13:27.000000 tree_plus-1.0.8/LICENSE
--rw-r--r--   0 bion      (1000) bion      (1000)    42042 2023-12-25 01:41:28.535864 tree_plus-1.0.8/PKG-INFO
--rw-r--r--   0 bion      (1000) bion      (1000)    40936 2023-12-25 01:40:52.000000 tree_plus-1.0.8/README.md
--rw-r--r--   0 bion      (1000) bion      (1000)     1208 2023-12-25 01:41:21.000000 tree_plus-1.0.8/pyproject.toml
--rw-r--r--   0 bion      (1000) bion      (1000)       38 2023-12-25 01:41:28.535864 tree_plus-1.0.8/setup.cfg
-drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 01:41:28.535864 tree_plus-1.0.8/tests/
--rw-r--r--   0 bion      (1000) bion      (1000)        1 2023-05-22 22:37:03.000000 tree_plus-1.0.8/tests/__init__.py
--rw-r--r--   0 bion      (1000) bion      (1000)     3710 2023-12-24 17:47:30.000000 tree_plus-1.0.8/tests/test_cli.py
--rw-r--r--   0 bion      (1000) bion      (1000)      197 2023-12-24 23:15:30.000000 tree_plus-1.0.8/tests/test_dotenv.py
--rw-r--r--   0 bion      (1000) bion      (1000)     5986 2023-12-24 20:50:53.000000 tree_plus-1.0.8/tests/test_e2e.py
--rw-r--r--   0 bion      (1000) bion      (1000)    28987 2023-12-25 00:56:09.000000 tree_plus-1.0.8/tests/test_more_language_units.py
--rw-r--r--   0 bion      (1000) bion      (1000)     3129 2023-12-24 16:03:23.000000 tree_plus-1.0.8/tests/test_units.py
-drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 01:41:28.535864 tree_plus-1.0.8/tree_plus.egg-info/
--rw-r--r--   0 bion      (1000) bion      (1000)    42042 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/PKG-INFO
--rw-r--r--   0 bion      (1000) bion      (1000)      551 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/SOURCES.txt
--rw-r--r--   0 bion      (1000) bion      (1000)        1 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/dependency_links.txt
--rw-r--r--   0 bion      (1000) bion      (1000)       49 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/entry_points.txt
--rw-r--r--   0 bion      (1000) bion      (1000)       55 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/requires.txt
--rw-r--r--   0 bion      (1000) bion      (1000)       28 2023-12-25 01:41:28.000000 tree_plus-1.0.8/tree_plus.egg-info/top_level.txt
--rw-r--r--   0 bion      (1000) bion      (1000)    15175 2023-12-24 20:59:14.000000 tree_plus-1.0.8/tree_plus_cli.py
-drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 01:41:28.535864 tree_plus-1.0.8/tree_plus_src/
--rw-r--r--   0 bion      (1000) bion      (1000)      453 2023-12-24 18:22:17.000000 tree_plus-1.0.8/tree_plus_src/__init__.py
--rw-r--r--   0 bion      (1000) bion      (1000)     2598 2023-12-22 14:25:20.000000 tree_plus-1.0.8/tree_plus_src/count_tokens_lines.py
--rw-r--r--   0 bion      (1000) bion      (1000)      349 2023-12-24 15:20:07.000000 tree_plus-1.0.8/tree_plus_src/debug.py
--rw-r--r--   0 bion      (1000) bion      (1000)     3499 2023-12-24 19:42:28.000000 tree_plus-1.0.8/tree_plus_src/ignore.py
--rw-r--r--   0 bion      (1000) bion      (1000)    51565 2023-12-25 00:51:29.000000 tree_plus-1.0.8/tree_plus_src/parse_file.py
--rw-r--r--   0 bion      (1000) bion      (1000)     1922 2023-12-24 20:08:58.000000 tree_plus-1.0.8/tree_plus_src/traverse_directory.py
+drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 20:57:36.148551 tree_plus-1.0.9/
+-rw-r--r--   0 bion      (1000) bion      (1000)    10984 2023-05-27 13:13:27.000000 tree_plus-1.0.9/LICENSE
+-rw-r--r--   0 bion      (1000) bion      (1000)    42063 2023-12-25 20:57:36.148551 tree_plus-1.0.9/PKG-INFO
+-rw-r--r--   0 bion      (1000) bion      (1000)    40936 2023-12-25 01:40:52.000000 tree_plus-1.0.9/README.md
+-rw-r--r--   0 bion      (1000) bion      (1000)     1217 2023-12-25 20:57:27.000000 tree_plus-1.0.9/pyproject.toml
+-rw-r--r--   0 bion      (1000) bion      (1000)       38 2023-12-25 20:57:36.148551 tree_plus-1.0.9/setup.cfg
+drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 20:57:36.148551 tree_plus-1.0.9/tests/
+-rw-r--r--   0 bion      (1000) bion      (1000)        1 2023-05-22 22:37:03.000000 tree_plus-1.0.9/tests/__init__.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     3710 2023-12-24 17:47:30.000000 tree_plus-1.0.9/tests/test_cli.py
+-rw-r--r--   0 bion      (1000) bion      (1000)      197 2023-12-24 23:15:30.000000 tree_plus-1.0.9/tests/test_dotenv.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     5948 2023-12-25 12:09:05.000000 tree_plus-1.0.9/tests/test_e2e.py
+-rw-r--r--   0 bion      (1000) bion      (1000)    39711 2023-12-25 20:07:28.000000 tree_plus-1.0.9/tests/test_more_language_units.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     3129 2023-12-24 16:03:23.000000 tree_plus-1.0.9/tests/test_units.py
+drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 20:57:36.148551 tree_plus-1.0.9/tree_plus.egg-info/
+-rw-r--r--   0 bion      (1000) bion      (1000)    42063 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/PKG-INFO
+-rw-r--r--   0 bion      (1000) bion      (1000)      551 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/SOURCES.txt
+-rw-r--r--   0 bion      (1000) bion      (1000)        1 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/dependency_links.txt
+-rw-r--r--   0 bion      (1000) bion      (1000)       49 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/entry_points.txt
+-rw-r--r--   0 bion      (1000) bion      (1000)       61 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/requires.txt
+-rw-r--r--   0 bion      (1000) bion      (1000)       28 2023-12-25 20:57:36.000000 tree_plus-1.0.9/tree_plus.egg-info/top_level.txt
+-rw-r--r--   0 bion      (1000) bion      (1000)    15175 2023-12-24 20:59:14.000000 tree_plus-1.0.9/tree_plus_cli.py
+drwxr-xr-x   0 bion      (1000) bion      (1000)        0 2023-12-25 20:57:36.148551 tree_plus-1.0.9/tree_plus_src/
+-rw-r--r--   0 bion      (1000) bion      (1000)      453 2023-12-24 18:22:17.000000 tree_plus-1.0.9/tree_plus_src/__init__.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     2598 2023-12-22 14:25:20.000000 tree_plus-1.0.9/tree_plus_src/count_tokens_lines.py
+-rw-r--r--   0 bion      (1000) bion      (1000)      349 2023-12-24 15:20:07.000000 tree_plus-1.0.9/tree_plus_src/debug.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     3499 2023-12-24 19:42:28.000000 tree_plus-1.0.9/tree_plus_src/ignore.py
+-rw-r--r--   0 bion      (1000) bion      (1000)    65770 2023-12-25 20:31:05.000000 tree_plus-1.0.9/tree_plus_src/parse_file.py
+-rw-r--r--   0 bion      (1000) bion      (1000)     1922 2023-12-24 20:08:58.000000 tree_plus-1.0.9/tree_plus_src/traverse_directory.py
```

### Comparing `tree_plus-1.0.8/LICENSE` & `tree_plus-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/PKG-INFO` & `tree_plus-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree_plus
-Version: 1.0.8
+Version: 1.0.9
 Summary: A `tree` util enhanced with tokens, lines, and components.
 Author-email: Bion Howard <bion@atomiclogic.com>
 Project-URL: Homepage, https://github.com/bionicles/tree_plus
 Project-URL: Issues, https://github.com/bionicles/tree_plus/issues
 Project-URL: repository, https://www.github.com/bionicles/tree_plus
 Project-URL: documentation, https://www.github.com/bionicles/tree_plus/README.md
 Keywords: tree,util,cli
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken
 Requires-Dist: PyYAML
 Requires-Dist: click
 Requires-Dist: rich
+Requires-Dist: tomli
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-dotenv; extra == "dev"
 
 # Tree Plus
 
 **A `tree` util enhanced with tokens, lines, and components.**
```

### Comparing `tree_plus-1.0.8/README.md` & `tree_plus-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/pyproject.toml` & `tree_plus-1.0.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [project]
 name = "tree_plus"
-version = "1.0.8"
+version = "1.0.9"
 authors = [{ name = "Bion Howard", email = "bion@atomiclogic.com" }]
 description = "A `tree` util enhanced with tokens, lines, and components."
 readme = "README.md"
 requires-python = ">=3.8"
 keywords=["tree", "util", "cli"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: Apache Software License",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Intended Audience :: Developers",
     "Topic :: Utilities",
 ]
-dependencies = ["tiktoken", "PyYAML", "click", "rich"]
+dependencies = ["tiktoken", "PyYAML", "click", "rich", "tomli"]
 
 [project.optional-dependencies]
 dev = ["pytest", "pytest-dotenv"]
 
 [project.urls]
 Homepage = "https://github.com/bionicles/tree_plus"
 Issues = "https://github.com/bionicles/tree_plus/issues"
```

### Comparing `tree_plus-1.0.8/tests/test_cli.py` & `tree_plus-1.0.9/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tests/test_e2e.py` & `tree_plus-1.0.9/tests/test_e2e.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,14 @@
     assert ".ts" in result_str
     assert ".hs" in result_str
     assert ".cs" in result_str
     assert ".exs" in result_str
     assert ".java" not in result_str
     assert "group1" not in result_str
     assert "group2" not in result_str
-    assert "group3" not in result_str
     assert "group4" in result_str
     assert "group5" in result_str
     assert "group_todo" in result_str
 
 
 # Test ignore parameter
 def test_e2e_ignore_parameter_filetype():
```

### Comparing `tree_plus-1.0.8/tests/test_more_language_units.py` & `tree_plus-1.0.9/tests/test_more_language_units.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,53 @@
 # tests/test_more_language_units.py
 from typing import List
 import pytest
 import os
 
 from rich import print
+import sqlite3
 
 from tree_plus_src import parse_file
 
+SQLITE_PATH = "tests/more_languages/group3/test.sqlite"
+
+# Define the SQL commands for table creation
+create_students_table = """
+CREATE TABLE IF NOT EXISTS students (
+    id INTEGER PRIMARY KEY,
+    name TEXT NOT NULL,
+    age INTEGER NOT NULL
+);
+"""
+
+create_courses_table = """
+CREATE TABLE IF NOT EXISTS courses (
+    id INTEGER PRIMARY KEY,
+    title TEXT NOT NULL,
+    credits INTEGER NOT NULL
+);
+"""
+
+SQLITE_TEST_QUERIES = (create_students_table, create_courses_table)
+
+
+def create_sqlite_test_db(
+    db_path: str = SQLITE_PATH,
+    test_queries: tuple = SQLITE_TEST_QUERIES,
+    force: bool = False,
+):
+    if os.path.exists(db_path) and force:
+        os.remove(db_path)
+    conn = sqlite3.connect(db_path)
+    cursor = conn.cursor()
+    for query in test_queries:
+        cursor.execute(query)
+    conn.commit()
+    conn.close()
+
 
 @pytest.mark.parametrize(
     "file,expected",
     [
         (
             "tests/more_languages/group1/COBOL_TEST.CBL",
             [
@@ -39,21 +76,14 @@
             "tests/more_languages/group1/KotlinTest.kt",
             [
                 "data class Person(val name: String)",
                 "fun greet(person: Person)",
             ],
         ),
         (
-            "tests/more_languages/group1/LispTest.lisp",
-            [
-                "defstruct person",
-                "defun greet",
-            ],
-        ),
-        (
             "tests/more_languages/group1/LuaTest.lua",
             [
                 "function HelloWorld.new",
                 "function HelloWorld.greet",
                 "function say_hello",
             ],
         ),
@@ -320,18 +350,208 @@
                 "section ConstructiveApproach",
                 "lemma finite_group_order (G : Type*) [Group G] [Fintype G]",
                 """lemma complex_lemma {X Y : Type*} [SomeClass X] [AnotherClass Y]
   (f : X → Y) (g : Y → X)""",
                 "end ConstructiveApproach",
             ],
         ),
+        (
+            "tests/more_languages/group3/csharp_test.cs",
+            [
+                "public interface IExcelTemplate",
+                "    void LoadTemplate",
+                "    void LoadData",
+                "    void ModifyCell",
+                "    void SaveToFile",
+                "public interface IGreet",
+                "    void Greet",
+                "public enum WeekDays",
+                "public delegate void DisplayMessage",
+                "public struct Address",
+                "public static class HelperFunctions",
+                "    public static void PrintMessage",
+                "    public static int AddNumbers",
+                "namespace HelloWorldApp",
+                "    class Person : IGreet",
+                "        public Person",
+                "        public void Greet",
+                "    class HelloWorld",
+                "        static void Main",
+                "namespace TemplateToExcelServer.Template",
+                "    public interface ITemplateObject",
+                "        string[,] GetContent",
+                "        string[] GetContentArray",
+                "        string[] GetFormat",
+                "        int? GetFormatLength",
+                "        TemplateObject SetContent",
+                "        TemplateObject SetContentArray",
+                "        TemplateObject SetFormat",
+                "        TemplateObject SetNameOfReport",
+                "        TemplateObject SetSheetName",
+                "public class BankAccount",
+                "    public override string ToString: =>",
+                "var IncrementBy: =>",
+                "Func<int, int, int> add: =>",
+                "button.Click +=: =>",
+                "public Func<int, int> GetMultiplier: =>",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test.sqlite",
+            [
+                "students table:",
+                "   id integer primary key",
+                "   name text not null",
+                "   age integer not null",
+                "courses table:",
+                "   id integer primary key",
+                "   title text not null",
+                "   credits integer not null",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test_pyproject.toml",
+            [
+                "name: tree_plus",
+                "version: 1.0.8",
+                "description: A `tree` util enhanced with tokens, lines, and components.",
+                "License :: OSI Approved :: Apache Software License",
+                "License :: OSI Approved :: MIT License",
+                "dependencies:",
+                "    tiktoken",
+                "    PyYAML",
+                "    click",
+                "    rich",
+                "    tomli",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test_Cargo.toml",
+            [
+                "name: test_cargo",
+                "version: 0.1.0",
+                "description: A test Cargo.toml",
+                "license: MIT OR Apache-2.0",
+                "dependencies:",
+                "  clap 4.4",
+                "  sqlx 0.7 (features: runtime-tokio, tls-rustls)",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test_openapi.yaml",
+            [
+                "openapi: 3.0.1",
+                "    title: TODO Plugin",
+                "    description: A plugin that allows the user to create and manage a TODO list using ChatGPT.",
+                "    version: v1",
+                "servers:",
+                "    - url: PLUGIN_HOSTNAME",
+                "paths:",
+                "    '/todos/{username}':",
+                "        GET (getTodos): Get the list of todos",
+                "        POST (addTodo): Add a todo to the list",
+                "        DELETE (deleteTodo): Delete a todo from the list",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test.graphql",
+            [
+                "type Query",
+                "    getBooks: [Book]",
+                "    getAuthors: [Author]",
+                "type Mutation",
+                "    addBook(title: String, author: String): Book",
+                "    removeBook(id: ID): Book",
+                "type Book",
+                "    id: ID",
+                "    title: String",
+                "    author: Author",
+                "type Author",
+                "    id: ID",
+                "    name: String",
+                "    books: [Book]",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test_openrpc.json",
+            [
+                "openrpc: 1.2.1",
+                "info:",
+                "    title: Demo Petstore",
+                "    version: 1.0.0",
+                "methods:",
+                "    listPets: List all pets",
+                "        params:",
+                "            - limit: integer",
+                "        result: pets = An array of pets",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test_json_rpc_2_0.json",
+            [
+                "jsonrpc: 2.0",
+                "method: subtract",
+                "params:",
+                "    minuend: 42",
+                "    subtrahend: 23",
+                "id: 1",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test.capnp",
+            [
+                "struct Employee",
+                "  id @0 :Int32",
+                "  name @1 :Text",
+                "  role @2 :Text",
+                "  skills @3 :List(Skill)",
+                "  struct Skill",
+                "    name @0 :Text",
+                "    level @1 :Level",
+                "    enum Level",
+                "      beginner @0",
+                "      intermediate @1",
+                "      expert @2",
+                "  status :union",
+                "    active @4 :Void",
+                "    onLeave @5 :Void",
+                "    retired @6 :Void",
+                "struct Company",
+                "  employees @0 :List(Employee)",
+            ],
+        ),
+        (
+            "tests/more_languages/group3/test.proto",
+            [
+                'syntax = "proto3"',
+                "service EmployeeService",
+                "    rpc GetEmployee(EmployeeId) returns (EmployeeInfo)",
+                "    rpc AddEmployee(EmployeeData) returns (EmployeeInfo)",
+                "    rpc UpdateEmployee(EmployeeUpdate) returns (EmployeeInfo)",
+                "message EmployeeId",
+                "    int32 id = 1",
+                "message EmployeeInfo",
+                "    int32 id = 1",
+                "    string name = 2",
+                "    string role = 3",
+                "message EmployeeData",
+                "    string name = 1",
+                "    string role = 2",
+                "message EmployeeUpdate",
+                "    int32 id = 1",
+                "    string name = 2",
+                "    string role = 3",
+            ],
+        ),
     ],
 )
 def test_more_languages_group3(file: str, expected: List[str]):
     print(f"{file=}")
+    if file.endswith("test.sqlite"):
+        create_sqlite_test_db()
     os.environ.get("DEBUG_TREE_PLUS") == "1"
     result = parse_file(file)
     print(f"{result=}")
     print(f"{expected=}")
     assert result == expected
 
 
@@ -393,14 +613,74 @@
                 'data "aws_ami" "ubuntu"',
                 'variable "instance_type"',
                 'output "instance_public_ip"',
                 "locals",
                 'module "vpc"',
             ],
         ),
+        (
+            "tests/more_languages/group4/haskell_test.hs",
+            [
+                "data Person",
+                "greet :: Person -> String",
+                """resolveVariables ::
+  forall m fragments.
+  (MonadError QErr m, Traversable fragments) =>
+  Options.BackwardsCompatibleNullInNonNullableVariables ->
+  [G.VariableDefinition] ->
+  GH.VariableValues ->
+  [G.Directive G.Name] ->
+  G.SelectionSet fragments G.Name ->
+  m
+    ( [G.Directive Variable],
+      G.SelectionSet fragments Variable
+    )""",
+            ],
+        ),
+        (
+            "tests/more_languages/group4/mathematica_test.nb",
+            [
+                "person[name_]",
+                "sayHello[]",
+                "sumList[list_List]",
+            ],
+        ),
+        (
+            "tests/more_languages/group4/test.zig",
+            [
+                "pub fn add(a: i32, b: i32) i32",
+                'test "add function"',
+                "const BunBuildOptions = struct",
+                "    pub fn updateRuntime(this: *BunBuildOptions) anyerror!void",
+                "    pub fn step(this: BunBuildOptions, b: anytype) *std.build.OptionsStep",
+                """pub fn sgemv(
+    order: Order,
+    trans: Trans,
+    m: usize,
+    n: usize,
+    alpha: f32,
+    a: []const f32,
+    lda: usize,
+    x: []const f32,
+    x_add: usize,
+    beta: f32,
+    y: []f32,
+    y_add: usize,
+) void""",
+            ],
+        ),
+        (
+            "tests/more_languages/group4/RTest.R",
+            [
+                "class(person)",
+                "greet.Person <- function",
+                "ensure_between = function",
+                "run_intermediate_annealing_process = function",
+            ],
+        ),
     ],
 )
 def test_more_languages_group4(
     file: str,
     expected: List[str],
 ):
     print(f"{file=}")
@@ -693,14 +973,67 @@
     print(f"{file=}")
     result = parse_file(file)
     print(f"{result=}")
     print(f"{expected=}")
     assert result == expected
 
 
+@pytest.mark.parametrize(
+    "file,expected",
+    [
+        (
+            "tests/more_languages/group_lisp/LispTest.lisp",
+            [
+                "defstruct person",
+                "defun greet",
+            ],
+        ),
+        (
+            "tests/more_languages/group_lisp/clojure_test.clj",
+            [
+                "defprotocol P",
+                "defrecord Person",
+                "defn -main",
+                "ns bion.likes_trees",
+                "def repo-url",
+                "defn config",
+                "defmacro with-os",
+                "defrecord SetFullElement",
+            ],
+        ),
+        (
+            "tests/more_languages/group_lisp/test_scheme.scm",
+            [
+                "define topological-sort",
+                "  define table",
+                "  define queue",
+                "  define result",
+                "  define set-up",
+                "  define traverse",
+            ],
+        ),
+        (
+            "tests/more_languages/group_lisp/racket_struct.rkt",
+            [
+                "struct point",
+            ],
+        ),
+    ],
+)
+def test_more_languages_group_lisp(
+    file: str,
+    expected: List[str],
+):
+    print(f"{file=}")
+    result = parse_file(file)
+    print(f"{result=}")
+    print(f"{expected=}")
+    assert result == expected
+
+
 # TODO:
 # @pytest.mark.parametrize(
 #     "file,expected",
 #     [
 #         (
 #             "tests/more_languages/group3/crystal_test.cr",
 #             ["class Person -> def greet", "def say_hello"],
@@ -746,18 +1079,15 @@
 # ),
 
 # (
 #     "tests/more_languages/group4/fsharp_test.fs",
 #     ["type Person -> member this.SayHello", "let person"],
 # ),
 
-# (
-#     "tests/more_languages/group4/haskell_test.hs",
-#     ["data Person", "greet :: Person -> String"],
-# ),
+
 # (
 #     "tests/more_languages/group4/mathematica_test.nb",
 #     [
 #         "person[name_]",
 #         'BeginPackage["TestModule"] -> sayHello::usage',
 #         'BeginPackage["TestModule"] -> sumList::usage',
 #     ],
```

### Comparing `tree_plus-1.0.8/tests/test_units.py` & `tree_plus-1.0.9/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tree_plus.egg-info/PKG-INFO` & `tree_plus-1.0.9/tree_plus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tree_plus
-Version: 1.0.8
+Version: 1.0.9
 Summary: A `tree` util enhanced with tokens, lines, and components.
 Author-email: Bion Howard <bion@atomiclogic.com>
 Project-URL: Homepage, https://github.com/bionicles/tree_plus
 Project-URL: Issues, https://github.com/bionicles/tree_plus/issues
 Project-URL: repository, https://www.github.com/bionicles/tree_plus
 Project-URL: documentation, https://www.github.com/bionicles/tree_plus/README.md
 Keywords: tree,util,cli
@@ -18,14 +18,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: tiktoken
 Requires-Dist: PyYAML
 Requires-Dist: click
 Requires-Dist: rich
+Requires-Dist: tomli
 Provides-Extra: dev
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-dotenv; extra == "dev"
 
 # Tree Plus
 
 **A `tree` util enhanced with tokens, lines, and components.**
```

### Comparing `tree_plus-1.0.8/tree_plus.egg-info/SOURCES.txt` & `tree_plus-1.0.9/tree_plus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tree_plus_cli.py` & `tree_plus-1.0.9/tree_plus_cli.py`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tree_plus_src/count_tokens_lines.py` & `tree_plus-1.0.9/tree_plus_src/count_tokens_lines.py`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tree_plus_src/ignore.py` & `tree_plus-1.0.9/tree_plus_src/ignore.py`

 * *Files identical despite different names*

### Comparing `tree_plus-1.0.8/tree_plus_src/parse_file.py` & `tree_plus-1.0.9/tree_plus_src/parse_file.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,39 @@
 # tree_plus_src/parse_file.py
-from typing import List
+from typing import List, Tuple
 import collections
 import builtins
 import sqlite3
 import typing
 import yaml
 import ast
 import os
 import re
 import json
 
+import tomli
+
 from tree_plus_src.ignore import is_binary
 from tree_plus_src.debug import debug_print
 
 
+LISP_EXTENSIONS = {".lisp", ".clj", ".scm", ".el", ".rkt"}
+
+
+def extract_groups(match: re.Match) -> dict:
+    "filter and debug print non-None match groups"
+    numbered_groups = {}
+    for i in range(len(match.groups())):
+        group = match.group(i)
+        if group:
+            numbered_groups[i] = group
+    debug_print(numbered_groups)
+    return numbered_groups
+
+
 def parse_file(file_path: str) -> List[str]:
     """
     Parse a file and return a List[str] of its major components.
     """
     base_file_path, file_extension = os.path.splitext(file_path)
     file_name = os.path.basename(base_file_path)
     file_extension = file_extension.lower()
@@ -50,14 +66,22 @@
             # print(f"SyntaxError @ {file_path}: {components}")
             components = [f"SyntaxError: {components}"]
     elif file_extension == ".json":
         if "package.json" in file_path.lower():
             components = parse_package_json(contents)
         elif "$schema" in contents:  # not great!
             components = parse_json_schema(contents)
+        elif 'jsonrpc": "2' in contents:
+            components = parse_json_rpc(contents)
+        elif 'openrpc": "' in contents:
+            components = parse_openrpc_json(contents)
+    elif file_path.endswith("Cargo.toml"):
+        components = parse_cargo_toml(contents)
+    elif file_path.endswith("pyproject.toml"):
+        components = parse_pyproject_toml(contents)
     elif file_extension in [".js", ".jsx"]:
         components = parse_ts(contents)
     elif file_path.endswith(".d.ts"):
         components = parse_d_dot_ts(contents)
     elif file_extension in {".ts", ".tsx"}:
         components = parse_ts(contents)
         if "app-routing.module" in file_path:
@@ -68,88 +92,388 @@
         #     components = parse_angular_component_ts(contents) + components
         elif "environment" == file_name or "environment." in file_name:  # paranoid
             components = parse_environment_ts(contents)
         elif "spec.ts" in file_path:
             components = parse_angular_spec(contents) + components
     elif file_extension == ".md":
         components = parse_md(contents)
+    elif file_extension in (".yml", ".yaml"):
+        components = parse_yml(contents)
     elif file_extension == ".c":
         components = parse_c(contents)
     elif file_extension in {".cpp", ".cc"}:
         components = parse_cpp(contents)
     elif file_extension == ".h":
         # harrumph!
         # components = parse_c(contents)
         components = parse_cpp(contents)
     elif file_extension == ".rs":
         components = parse_rs(contents)
+    elif file_extension == ".zig":
+        components = parse_zig(contents)
     elif file_extension == ".swift":
         components = parse_swift(contents)
     elif file_extension == ".go":
         components = parse_go(contents)
     elif file_extension == ".sh":
         components = parse_bash(contents)
     elif file_extension == ".rb":
         components = parse_rb(contents)
     elif file_extension == ".env":
         components = parse_dot_env(contents)
     elif file_extension == ".sql":
         components = parse_sql(contents)
+    elif file_name == "Makefile":
+        components = parse_makefile(contents)
     elif file_extension == ".txt":
         if "requirements" in file_name:
             components = parse_requirements_txt(contents)
         else:
             components = parse_txt(contents)
-    elif file_extension == ".tex":
-        components = parse_tex(contents)
-    elif file_extension == ".lean":
-        components = parse_lean(contents)
-    elif file_extension == ".cbl":
-        components = parse_cobol(contents)
+    elif file_extension == ".graphql":
+        components = parse_graphql(contents)
+    elif file_extension == ".cs":
+        components = parse_cs(contents)
+    elif file_extension == ".kt":
+        components = parse_kotlin(contents)
     elif file_extension == ".java":
         components = parse_java(contents)
+    elif file_extension == ".hs":
+        components = parse_hs(contents)
     elif file_extension == ".jl":
         components = parse_julia(contents)
-    elif file_extension == ".kt":
-        components = parse_kotlin(contents)
-    elif file_extension == ".lisp":
+    elif file_extension == ".scala":
+        components = parse_scala(contents)
+    elif file_extension in LISP_EXTENSIONS:
         components = parse_lisp(contents)
+    elif file_extension == ".capnp":
+        components = parse_capnp(contents)
+    elif file_extension == ".proto":
+        components = parse_grpc(contents)
+    elif file_extension == ".tex":
+        components = parse_tex(contents)
+    elif file_extension == ".lean":
+        components = parse_lean(contents)
+    elif file_extension == ".tf":
+        components = parse_tf(contents)
     elif file_extension == ".lua":
         components = parse_lua(contents)
+    elif file_extension == ".php":
+        components = parse_php(contents)
     elif file_extension == ".m":
         if "@interface" in contents or "@implementation" in contents:
             components = parse_objective_c(contents)
         elif "classdef" in contents or "methods" in contents:
             components = parse_matlab(contents)
+    elif file_extension.lower() == ".r":
+        components = parse_r(contents)
+    elif file_extension.lower() == ".nb":
+        components = parse_mathematica(contents)
     elif file_extension == ".matlab":
         components = parse_matlab(contents)
     elif file_extension == ".ml":
         components = parse_ocaml(contents)
+    elif file_extension == ".cbl":
+        components = parse_cobol(contents)
     elif file_extension == ".apl":
         components = parse_apl(contents)
     elif file_extension == ".pl":
         components = parse_perl(contents)
-    elif file_extension == ".php":
-        components = parse_php(contents)
     elif file_extension == ".ps1":
         components = parse_powershell(contents)
-    elif file_extension == ".scala":
-        components = parse_scala(contents)
-    elif file_extension == ".tf":
-        components = parse_tf(contents)
-    elif file_extension in (".yml", ".yaml"):
-        components = parse_yml(contents)
-    elif file_name == "Makefile":
-        components = parse_makefile(contents)
 
     bugs_todos_and_notes = parse_markers(contents)
     total_components = bugs_todos_and_notes + components
     return total_components
 
 
+def parse_mathematica(contents: str) -> List[str]:
+    combined_pattern = re.compile(
+        r"((\w+\[.*?\]))\s*:=.*?(?=\n\n|\Z)",
+    )
+
+    components = []
+
+    for match_number, match in enumerate(combined_pattern.finditer(contents)):
+        debug_print(f"parse_mathematica match_number: {match_number}")
+        groups = extract_groups(match)
+        component = groups[1]
+        components.append(component)
+
+    return components
+
+
+def parse_r(contents: str) -> List[str]:
+    combined_pattern = re.compile(
+        # class and whatever's inside
+        r"class\(.*\)|"
+        # arrow or equals function
+        r".* ((<\-)|=) (function)\(",
+    )
+
+    components = []
+
+    for match_number, match in enumerate(combined_pattern.finditer(contents)):
+        debug_print(f"parse_r match_number: {match_number}")
+        groups = extract_groups(match)
+        component = match.group().strip().rstrip("(")
+        components.append(component)
+
+    return components
+
+
+def parse_zig(contents: str) -> List[str]:
+    combined_pattern = re.compile(
+        r"\n( *(pub )?fn \w+\([^)]*\) [^{]*) |"
+        r"const\s+\w+\s*=\s*struct|"
+        r"test\s+\"[^\"]+\"",
+        re.DOTALL,
+    )
+
+    components = []
+
+    for match_number, match in enumerate(combined_pattern.finditer(contents)):
+        debug_print(f"parse_zig match_number: {match_number}")
+        groups = extract_groups(match)  # this debug prints the matches
+        if 1 in groups:
+            component = groups[1]
+        else:
+            component = match.group().rstrip()
+        components.append(component)
+
+    return components
+
+
+def parse_hs(contents: str) -> List[str]:
+    components = []
+
+    # Combined regex pattern for Haskell components
+    combined_pattern = re.compile(
+        # Data type declarations
+        r"^data\s+([^\s]+)|"
+        # Function type signatures
+        r"^([\w']+\s*::(?:.|\n)*?)(?=\n\w|\n\n|\Z)",
+        re.MULTILINE,
+    )
+
+    for match_number, match in enumerate(combined_pattern.finditer(contents)):
+        debug_print(f"parse_hs match_number: {match_number}")
+        groups = extract_groups(match)
+        if groups:
+            component = groups[0].strip()
+            debug_print(component)
+            components.append(component)
+
+    return components
+
+
+def parse_lisp(content: str) -> List[str]:
+    components = []
+
+    # Combined regex pattern for various Lisp components
+    combined_pattern = re.compile(
+        # Common Lisp struct
+        # r"\(defstruct\s+(\w+)|"
+        # Common Lisp function
+        # r"\(defun\s+(\w+)|"
+        # Clojure protocol
+        # r"\(defprotocol\s+(\w+)|"
+        # Clojure record
+        # r"\(defrecord\s+(\w+)|"
+        # defn, means something other than def, clearly
+        # r"\(defn\s+-?\s*(\w+)|"
+        # just "def"
+        # r"\(def\s+-?\s*(\w+)|"
+        # Clojure namespace
+        # Scheme define
+        # r"\(define\s+\((\w+)|"
+        # Macros
+        # r"\(defmacro\s+(\w+)",
+        # namespace
+        r"\(ns\s+([^\s\(\)]+)|"
+        # def(______)?
+        r"( *\(def\w* \(?[\w_-]+)|"
+        # racket has a struct
+        r"\((struct \(?[\w_-]+)",
+        re.DOTALL,
+    )
+
+    for match_number, match in enumerate(combined_pattern.finditer(content)):
+        debug_print(f"parse_lisp match_number: {match_number}")
+        groups = extract_groups(match)
+        if groups:
+            components.append(groups[0].replace("(", ""))
+
+    return components
+
+
+def parse_capnp(contents: str) -> List[str]:
+    lines = contents.split("\n")
+    components = []
+
+    for line in lines:
+        line_stripped = line.strip()
+        leading_spaces = len(line) - len(line.lstrip())
+
+        if (
+            line_stripped.startswith("struct")
+            or line_stripped.startswith("enum")
+            or ":union" in line
+        ):
+            components.append(" " * leading_spaces + line_stripped.rstrip("{ "))
+        elif "@" in line:
+            field_info = " ".join(line_stripped.split()[:3]).rstrip(";")
+            components.append(" " * leading_spaces + field_info)
+
+    return components
+
+
+def parse_grpc(contents: str) -> List[str]:
+    lines = contents.split("\n")
+    components = []
+
+    for line in lines:
+        line_stripped = line.strip()
+        if line_stripped.startswith("syntax"):
+            components.append(line_stripped.rstrip(";"))
+        elif line_stripped.startswith("service") or line_stripped.startswith("message"):
+            components.append(line_stripped.rstrip("{ "))
+        elif line_stripped.startswith("rpc"):
+            components.append("    " + line_stripped.rstrip(" {}"))
+        elif (
+            line_stripped
+            and not line_stripped.startswith("//")
+            and "=" in line_stripped
+        ):
+            field_info = line_stripped.split(";")[0]  # Retain field numbers
+            components.append("    " + field_info)
+
+    return components
+
+
+def parse_openrpc_json(contents: str) -> List[str]:
+    data = json.loads(contents)
+    components = []
+
+    components.append(f"openrpc: {data.get('openrpc', 'N/A')}")
+    info = data.get("info", {})
+    components.append("info:")
+    components.append(f"    title: {info.get('title', 'N/A')}")
+    components.append(f"    version: {info.get('version', 'N/A')}")
+
+    methods = data.get("methods", [])
+    components.append("methods:")
+    for method in methods:
+        method_name = method.get("name")
+        method_desc = method.get("description", "No description")
+        components.append(f"    {method_name}: {method_desc}")
+        params = method.get("params", [])
+        components.append("        params:")
+        for param in params:
+            param_type = param.get("schema", {}).get("type", "N/A")
+            components.append(f"            - {param.get('name')}: {param_type}")
+        result = method.get("result", {}).get("name", "N/A")
+        result_desc = method.get("result", {}).get("description", "No description")
+        components.append(f"        result: {result} = {result_desc}")
+
+    return components
+
+
+def parse_json_rpc(contents: str) -> List[str]:
+    data = json.loads(contents)
+    components = []
+
+    components.append(f"jsonrpc: {data.get('jsonrpc', 'N/A')}")
+    components.append(f"method: {data.get('method', 'N/A')}")
+    components.append("params:")
+    for param, value in data.get("params", {}).items():
+        components.append(f"    {param}: {value}")
+    components.append(f"id: {data.get('id', 'N/A')}")
+
+    return components
+
+
+def parse_graphql(contents: str) -> List[str]:
+    components = []
+    for line in contents.splitlines():
+        line = line.strip()
+        if line == "}":  # Skip lines that only contain a closing brace
+            continue
+        if line.startswith("type") or line.startswith("enum"):
+            components.append(line.rstrip(" {"))  # Remove trailing '{'
+        elif line and not line.startswith("#"):
+            components.append("    " + line)
+    return components
+
+
+def format_dependency(name, details):
+    if isinstance(details, str):
+        return f"  {name} {details}"
+    elif isinstance(details, dict):
+        # Handle complex dependencies with additional properties
+        version = details.get("version", "")
+        features = ", ".join(details.get("features", []))
+        return (
+            f"  {name} {version} (features: {features})"
+            if features
+            else f"  {name} {version}"
+        )
+    return f"  {name}"
+
+
+def parse_cargo_toml(contents: str) -> List[str]:
+    data = tomli.loads(contents)
+    components = []
+
+    if "package" in data:
+        package_info = data["package"]
+        components.append(f"name: {package_info.get('name', 'N/A')}")
+        components.append(f"version: {package_info.get('version', 'N/A')}")
+        components.append(f"description: {package_info.get('description', 'N/A')}")
+        components.append(f"license: {package_info.get('license', 'N/A')}")
+
+    if "dependencies" in data:
+        dependencies = data["dependencies"]
+        components.append("dependencies:")
+        for dep, details in dependencies.items():
+            components.append(format_dependency(dep, details))
+
+    return components
+
+
+def parse_pyproject_toml(contents: str) -> List[str]:
+    data = tomli.loads(contents)
+    debug_print("parse_pyproject_toml data:", data)
+    components = []
+
+    if "project" in data:
+        project_info = data["project"]
+        debug_print("parse_pyproject_toml project_info:", project_info)
+        components.append(f"name: {project_info.get('name', 'N/A')}")
+        components.append(f"version: {project_info.get('version', 'N/A')}")
+        project_description = project_info.get("description", "N/A")
+
+        debug_print("parse_pyproject_toml project_description:", project_description)
+        components.append(f"description: {project_description}")
+
+        if "classifiers" in project_info:
+            classifiers = project_info["classifiers"]
+            for classifier in classifiers:
+                if "License ::" in classifier:
+                    components.append(classifier)
+
+    if "dependencies" in project_info:
+        dependencies = project_info["dependencies"]
+        components.append("dependencies:")
+        for dep in dependencies:
+            components.append(f"    {dep}")
+
+    return components
+
+
 def parse_lean(lean_content: str) -> List[str]:
     debug_print("parse_lean")
     components = []
 
     # Regex for title, sections, lemmas, theorems, and axioms
     title_re = r"\/-!\n(# [^\n]+)"
 
@@ -175,14 +499,62 @@
         debug_print(component)
         component = match.group(0).rstrip(" :\n")
         components.append(component)
 
     return components
 
 
+def parse_cs(contents: str) -> List[str]:
+    # Combined regex pattern to match all components
+    combined_pattern = re.compile(
+        # Interfaces, Enums, Delegates, Structs, Classes
+        r"\n( *(public )?(static )?(interface|enum|delegate|struct|class)\s+(\w+)( \w+)?( : \w+)?)|"
+        # Methods in Interfaces and Classes, capturing indentation
+        r"\n( *(public)?\s+(static\s+)?[\w<>\[\],]+\??\s+(\w+))\([^)]*\)|"
+        # Namespaces
+        r"\b(namespace\s+([\w\.]+))|"
+        # Method Arrow functions
+        r"\n( *(public\s+override\s+)?[\w<>\[\]]+\s+(\w+)\s*)\([^)]*\)\s*=>|"
+        # Arrow functions
+        # r"\n( *var\s+(\w+))\s*=\s*\([^)]*\)\s*=>|"
+        # Func<...> Lambda Expressions
+        # r"( *Func<[\w<>, ]+\s+\w+)\s*=\s*\([^)]*\)\s*=>|"
+        # Combined var and Func Lambda Expressions
+        r"\n( *(var|Func<[\w<>, ]+)\s+(\w+))\s*=\s*\([^)]*\)\s*=>|"
+        # Methods returning Lambda Expressions
+        r"\n( *(public\s+)?Func<[\w<>,\s]+\s+\w+)\([^)]*\)\s*\{|"
+        # Event Handler Arrow Functions
+        r"\n( *\w+(\.\w+)?\s*\+=)\s*\([^)]*\)\s*=>",
+        re.DOTALL,
+    )
+
+    components = []
+    for match_number, match in enumerate(combined_pattern.finditer(contents)):
+        groups = extract_groups(match)
+        if 1 in groups:
+            component = groups[1]
+        elif 8 in groups:
+            component = groups[8].lstrip("\n")
+        elif 14 in groups:  # Method Lambda
+            component = groups[14] + ": =>"
+        elif 17 in groups:  # var / Func Lambda
+            component = groups[17] + ": =>"
+        elif 20 in groups:  # Method returning Lambda
+            component = groups[20] + ": =>"
+        elif 22 in groups:
+            component = groups[22] + ": =>"
+        else:
+            component = match.group().strip()
+        debug_print(f"parse_cs: {match_number=} {component=}")
+        if component:
+            components.append(component)
+
+    return components
+
+
 def parse_tex(tex_content: str) -> List[str]:
     debug_print("parse_tex")
 
     # Regex for title, author, and date
     title_re = r"\\title\{([^\}]+)\}"
     author_re = r"\\author\{((?:[^{}]+|\{[^\}]*\})*)\}"
     date_re = r"\\date\{([^\}]+)\}"
@@ -192,24 +564,19 @@
     author = re.search(author_re, tex_content)
     date = re.search(date_re, tex_content)
 
     components = []
     if title:
         components.append(title.group(1))
 
-    # Handling multiple authors
-
+    # Handle multiple authors
     if author:
         author = author.group(1)
         debug_print(f"parse_tex: {author=}")
         is_multi_author = author.count("\\and") > 0
-        # Remove emails
-        # author = re.sub(r"\\texttt\{[^\}]+\}", "", author)
-        # debug_print(f"parse_tex: Removed emails {author=}")
-        # (no change observed from this substitution)
         # Remove LaTeX commands
         author = re.sub(r"\\.*", "", author).strip()
         debug_print(f"parse_tex: Removed LaTeX commands {author=}")
         if is_multi_author:
             debug_print(f"parse_tex: multi {author=}")
             author = author.splitlines()[0]
             first_author = author.split("\\and")[0]
@@ -222,15 +589,14 @@
     # Regex for sections and subsections
     section_re = r"\\(sub)?section\{([^\}]+)\}"
 
     # Extract sections and subsections
     outline = []
     section_count = 0
     subsection_count = 0
-    # TODO: format hierarchical numbered outline
     for match in re.finditer(section_re, tex_content):
         if match.group(1):  # Subsection
             subsection_count += 1
             outline.append(f"  {section_count}.{subsection_count} {match.group(2)}")
         else:
             section_count += 1
             subsection_count = 0  # Reset
@@ -594,24 +960,14 @@
 
     # Remove private closures (not effective)
     # contents = re.sub(r"private\s+.*?\{.*?\}", "", contents, flags=re.DOTALL)
 
     return contents
 
 
-def extract_groups(match) -> dict:
-    numbered_groups = {}
-    for i in range(len(match.groups())):
-        group = match.group(i)
-        if group:
-            numbered_groups[i] = group
-    debug_print(numbered_groups)
-    return numbered_groups
-
-
 def parse_ts(contents: str) -> List[str]:
     contents = remove_ts_comments_and_private_blocks(contents)
     # Combined regex pattern to match all components and title pattern
     combined_pattern = re.compile(
         # Types
         r"\btype\s+(\w+)|"
         # Interfaces
@@ -697,82 +1053,130 @@
         lines = table_body.strip().split("\n")
         lines = [line.strip() for line in lines]
         # Add each line to the output, with an indent
         output.extend([f"   {line}" for line in lines])
     return output
 
 
-def is_k8s_yml(contents: str) -> bool:
-    for doc in yaml.safe_load_all(contents):
-        if "apiVersion" in doc and "kind" in doc and "metadata" in doc:
-            return True
+def is_openapi_yml(ymls: Tuple[dict]) -> bool:
+    yml = ymls[0]
+    return "openapi" in yml or "swagger" in yml
+
+
+def is_k8s_yml(ymls: Tuple[dict]) -> bool:
+    yml = ymls[0]
+    debug_print("is_k8s_yml yml:", yml)
+    if "apiVersion" in yml and "kind" in yml and "metadata" in yml:
+        return True
     return False
 
 
-def is_ansible_yml(contents: str) -> bool:
-    try:
-        docs = list(yaml.safe_load_all(contents))
-        if isinstance(docs[0], list) and any(
-            isinstance(item, dict) and "name" in item for item in docs[0]
-        ):
-            return True
-    except Exception as e:
-        debug_print("Exception in is_ansible_yml: ", e)
-        return False
+def is_ansible_yml(ymls: Tuple[dict]) -> bool:
+    yml = ymls[0]
+    if isinstance(yml, list) and any(
+        isinstance(item, dict) and "name" in item for item in yml
+    ):
+        return True
     return False
 
 
-def is_github_yml(contents: str) -> bool:
-    try:
-        doc = yaml.safe_load(contents)  # load YAML from string
-        if "name" in doc and "jobs" in doc:
-            return True
-    except Exception as e:
-        debug_print("Exception in is_github_yml: ", e)
+def is_github_yml(ymls: Tuple[dict]) -> bool:
+    yml = ymls[0]
+    if "name" in yml and "jobs" in yml:
+        return True
     return False
 
 
-def parse_github_yml(contents: str) -> List[str]:
+def parse_github_yml(ymls: Tuple[dict]) -> List[str]:
     result = []
-    try:
-        doc = yaml.safe_load(contents)  # load YAML from string
-        if is_github_yml(contents):
-            result.append(doc["name"])
-            for job in doc["jobs"]:
-                result.append(f"  job: {job}")
-                if "steps" in doc["jobs"][job]:
-                    for step in doc["jobs"][job]["steps"]:
-                        if "name" in step:
-                            result.append(f"    - {step['name']}")
-    except Exception as e:
-        print("Exception in parse_github_yml: ", e)
+    yml = ymls[0]
+    result.append(yml["name"])
+    for job in yml["jobs"]:
+        result.append(f"  job: {job}")
+        if "steps" in yml["jobs"][job]:
+            for step in yml["jobs"][job]["steps"]:
+                if "name" in step:
+                    result.append(f"    - {step['name']}")
     return result
 
 
-def parse_k8s(contents: str) -> List[str]:
+def parse_k8s(ymls: Tuple[dict]) -> List[str]:
     result = []
-    for doc in yaml.safe_load_all(contents):
-        result.append(f"{doc['apiVersion']}.{doc['kind']} -> {doc['metadata']['name']}")
+    for yml in ymls:
+        result.append(f"{yml['apiVersion']}.{yml['kind']} -> {yml['metadata']['name']}")
     return result
 
 
-def parse_ansible(contents: str) -> List[str]:
+def parse_ansible(ymls: Tuple[dict]) -> List[str]:
     result = []
-    for doc in yaml.safe_load_all(contents):
-        result.extend(item.get("name", "") for item in doc if isinstance(item, dict))
+    for yml in ymls:
+        result.extend(item.get("name", "") for item in yml if isinstance(item, dict))
     return result
 
 
+def parse_openapi_yml(ymls: Tuple[dict]) -> List[str]:
+    components = []
+    yml = ymls[0]
+    # Extract OpenAPI version and info
+    components.append(f"openapi: {yml.get('openapi', yml.get('swagger', 'N/A'))}")
+    info = yml.get("info", {})
+    components.append(f"    title: {info.get('title', 'N/A')}")
+    description = info.get("description", "")
+    first_sentence = (
+        re.split(r"\.\s|\.\n", description, maxsplit=1)[0] + "."
+        if description
+        else "N/A"
+    )
+    components.append(f"    description: {first_sentence}")
+    components.append(f"    version: {info.get('version', 'N/A')}")
+
+    # Extracting servers
+    servers = yml.get("servers", [])
+    if servers:
+        components.append("servers:")
+        for server in servers:
+            components.append(f"    - url: {server.get('url', 'N/A')}")
+
+    # Extracting paths
+    paths = yml.get("paths", {})
+    if paths:
+        components.append("paths:")
+        for path, methods in paths.items():
+            components.append(f"    '{path}':")
+            for method, details in methods.items():
+                operation_id = details.get("operationId", "N/A")
+                summary = details.get("summary", "N/A")
+                components.append(
+                    f"        {method.upper()} ({operation_id}): {summary}"
+                )
+
+    return components
+
+
 def parse_yml(contents: str) -> List[str]:
-    if is_k8s_yml(contents):
-        return parse_k8s(contents)
-    elif is_ansible_yml(contents):
-        return parse_ansible(contents)
-    elif is_github_yml(contents):
-        return parse_github_yml(contents)
+    try:
+        ymls = tuple(yaml.safe_load_all(contents))
+    except Exception as e:
+        debug_print("parse_yml yaml.safe_load Exception:", e)
+        debug_print("parse_yml contents:", contents)
+        raise
+    debug_print("parse_yml loaded yml:", ymls)
+    if not ymls:
+        return []
+    try:
+        if is_k8s_yml(ymls):
+            return parse_k8s(ymls)
+        elif is_ansible_yml(ymls):
+            return parse_ansible(ymls)
+        elif is_github_yml(ymls):
+            return parse_github_yml(ymls)
+        elif is_openapi_yml(ymls):
+            return parse_openapi_yml(ymls)
+    except Exception as e:
+        debug_print("parse_yml transform Exception: ", e)
     return ["Unsupported YAML Category"]
 
 
 def extract_nodes(node, node_type, parent=None):
     result = []
     if isinstance(node, node_type):
         result.append((parent, node))
@@ -850,24 +1254,46 @@
     # Return only the formatted names
     return [item[1] for item in sorted_items]
 
 
 def parse_db(db_path: str) -> List[str]:
     # Connect to the SQLite database
     conn = sqlite3.connect(db_path)
-    # Create a cursor object
     cursor = conn.cursor()
-    # Execute the query that retrieves all table names
+
+    # Get the list of table names
     cursor.execute("SELECT name FROM sqlite_master WHERE type='table';")
-    # Fetch all results of the query
     tables = cursor.fetchall()
+
+    components = []
+
+    # For each table, get the column details
+    for table in tables:
+        table_name = table[0]
+        components.append(f"{table_name} table:")
+
+        cursor.execute(f"PRAGMA table_info({table_name});")
+        columns = cursor.fetchall()
+        debug_print("parse_db columns:", columns)
+
+        for column in columns:
+            column_name = column[1]
+            column_type = column[2].lower()
+            is_primary_key = column[5] == 1
+            not_null = column[3] == 1
+            column_desc = f"   {column_name} {column_type}"
+            if is_primary_key:
+                column_desc += " primary key"
+            if not_null and not is_primary_key:
+                column_desc += " not null"
+            components.append(column_desc)
     # Close the connection
     conn.close()
-    # Extract the table names from the tuples and return them
-    return [f"CREATE TABLE {table[0]}" for table in tables]
+
+    return components
 
 
 def parse_cobol(content: str) -> List[str]:
     division_patterns = [
         (
             r"IDENTIFICATION DIVISION.*\n.*PROGRAM-ID. (\w+)",
             "IDENTIFICATION DIVISION -> PROGRAM-ID. ",
@@ -971,32 +1397,32 @@
         function_name = function_match[0]
         parameters = function_match[1]
         components.append(f"fun {function_name}({parameters})")
 
     return components
 
 
-def parse_lisp(content: str) -> List[str]:
-    components = []
+# def parse_lisp(content: str) -> List[str]:
+#     components = []
 
-    # Find struct declarations
-    struct_pattern = r"\(defstruct\s+(\w+)"
-    struct_matches = re.findall(struct_pattern, content)
+#     # Find struct declarations
+#     struct_pattern = r"\(defstruct\s+(\w+)"
+#     struct_matches = re.findall(struct_pattern, content)
 
-    for struct_match in struct_matches:
-        components.append(f"defstruct {struct_match}")
+#     for struct_match in struct_matches:
+#         components.append(f"defstruct {struct_match}")
 
-    # Find function declarations
-    function_pattern = r"\(defun\s+(\w+)"
-    function_matches = re.findall(function_pattern, content)
+#     # Find function declarations
+#     function_pattern = r"\(defun\s+(\w+)"
+#     function_matches = re.findall(function_pattern, content)
 
-    for function_match in function_matches:
-        components.append(f"defun {function_match}")
+#     for function_match in function_matches:
+#         components.append(f"defun {function_match}")
 
-    return components
+#     return components
 
 
 def parse_lua(content: str) -> List[str]:
     components = []
 
     # Find function declarations, but ignore arguments
     function_pattern = r"\bfunction\s+([\w.]+)\s*\("
```

### Comparing `tree_plus-1.0.8/tree_plus_src/traverse_directory.py` & `tree_plus-1.0.9/tree_plus_src/traverse_directory.py`

 * *Files identical despite different names*

