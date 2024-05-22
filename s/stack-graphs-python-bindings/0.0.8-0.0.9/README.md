# Comparing `tmp/stack_graphs_python_bindings-0.0.8.tar.gz` & `tmp/stack_graphs_python_bindings-0.0.9.tar.gz`

## Comparing `stack_graphs_python_bindings-0.0.8.tar` & `stack_graphs_python_bindings-0.0.9.tar`

### file list

```diff
@@ -1,17 +1,22 @@
--rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.8/Cargo.toml
--rw-r--r--   0     1001      127      840 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/.github/workflows/ci.yaml
--rw-r--r--   0     1001      127     4138 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/.github/workflows/release.yaml
--rw-r--r--   0     1001      127      739 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/.gitignore
--rw-r--r--   0     1001      127     1077 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/LICENSE
--rw-r--r--   0     1001      127     1708 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/Makefile
--rw-r--r--   0     1001      127      909 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/README.md
--rw-r--r--   0     1001      127     2101 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/src/classes.rs
--rw-r--r--   0     1001      127     1159 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/src/lib.rs
--rw-r--r--   0     1001      127     3547 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/src/stack_graphs_wrapper/mod.rs
--rw-r--r--   0     1001      127      456 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/stack_graphs_python.pyi
--rw-r--r--   0     1001      127       66 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/tests/js_sample/index.js
--rw-r--r--   0     1001      127       25 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/tests/js_sample/module.js
--rw-r--r--   0     1001      127      934 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/tests/test.py
--rw-r--r--   0     1001      127    50375 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/Cargo.lock
--rw-r--r--   0     1001      127      405 2024-05-13 15:03:12.000000 stack_graphs_python_bindings-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1279 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0      577 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.9/Cargo.toml
+-rw-r--r--   0     1001      127      525 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/.github/workflows/ci.yaml
+-rw-r--r--   0     1001      127     4138 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/.github/workflows/release.yaml
+-rw-r--r--   0     1001      127      739 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/.gitignore
+-rw-r--r--   0     1001      127     1077 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/LICENSE
+-rw-r--r--   0     1001      127     1716 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/Makefile
+-rw-r--r--   0     1001      127     1615 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/README.md
+-rw-r--r--   0     1001      127        0 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/py.typed
+-rw-r--r--   0     1001      127     2577 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/src/classes.rs
+-rw-r--r--   0     1001      127     1159 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/src/lib.rs
+-rw-r--r--   0     1001      127     3547 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/src/stack_graphs_wrapper/mod.rs
+-rw-r--r--   0     1001      127      575 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/stack_graphs_python.pyi
+-rw-r--r--   0     1001      127     1072 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/from_dir_test.py
+-rw-r--r--   0     1001      127     4166 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/helpers/virtual_files.py
+-rw-r--r--   0     1001      127     4815 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/helpers/virtual_files_test.py
+-rw-r--r--   0     1001      127      876 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/js_ok_test.py
+-rw-r--r--   0     1001      127       66 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/js_sample/index.js
+-rw-r--r--   0     1001      127       25 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/js_sample/module.js
+-rw-r--r--   0     1001      127      542 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/tests/position_test.py
+-rw-r--r--   0     1001      127    50375 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/Cargo.lock
+-rw-r--r--   0     1001      127      405 2024-05-21 19:15:23.000000 stack_graphs_python_bindings-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     1985 1970-01-01 00:00:00.000000 stack_graphs_python_bindings-0.0.9/PKG-INFO
```

### Comparing `stack_graphs_python_bindings-0.0.8/Cargo.toml` & `stack_graphs_python_bindings-0.0.9/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "stack-graphs-python-bindings"
-version = "0.0.8"
+version = "0.0.9"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "stack_graphs_python"
 crate-type = ["cdylib"]
```

### Comparing `stack_graphs_python_bindings-0.0.8/.github/workflows/release.yaml` & `stack_graphs_python_bindings-0.0.9/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.8/.gitignore` & `stack_graphs_python_bindings-0.0.9/.gitignore`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.8/LICENSE` & `stack_graphs_python_bindings-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.8/Makefile` & `stack_graphs_python_bindings-0.0.9/Makefile`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+# Run all commands in a single shell, so that the virtual environment is activated for all commands.
+.ONESHELL:
+
 .PHONY: setup
 setup:
-	pyenv virtualenvs | grep stack-graphs-python-bindings || pyenv virtualenv 3.11.9 stack-graphs-python-bindings
-	pyenv activate stack-graphs-python-bindings
+	python -m venv .venv
+	. .venv/bin/activate
 	pip install maturin
+	pip install pytest
 
 .PHONY: develop
 develop:
+	. .venv/bin/activate
 	maturin develop
 
-
 test: develop
-    ## TODO: Add actual tests with pytest
-	python tests/test.py
+	. .venv/bin/activate
+	pytest
 
 .PHONY: validate-tags release
 
 VERSION_PY := $(shell grep 'version = ' pyproject.toml | sed -e 's/version = "\(.*\)"/\1/')
 VERSION_RS := $(shell grep 'version =' Cargo.toml | sed -n 's/^version = "\(.*\)"/\1/p')
 
 # Usage: make validate-tags TAG=1.0.0
```

### Comparing `stack_graphs_python_bindings-0.0.8/src/classes.rs` & `stack_graphs_python_bindings-0.0.9/src/classes.rs`

 * *Files 16% similar despite different names*

```diff
@@ -26,23 +26,25 @@
     #[pyo3(get, set)]
     column: usize,
 }
 
 #[pyclass]
 pub struct Querier {
     db_reader: SQLiteReader,
+    db_path: String,
 }
 
 #[pymethods]
 impl Querier {
     #[new]
     pub fn new(db_path: String) -> Self {
         println!("Opening database: {}", db_path);
         Querier {
-            db_reader: SQLiteReader::open(db_path).unwrap(),
+            db_reader: SQLiteReader::open(db_path.clone()).unwrap(),
+            db_path: db_path,
         }
     }
 
     pub fn definitions(&mut self, reference: Position) -> PyResult<Vec<Position>> {
         let result = query_definition(reference.into(), &mut self.db_reader)?;
 
         let positions: Vec<Position> = result
@@ -50,24 +52,39 @@
             .map(|r| r.targets)
             .flatten()
             .map(|t| t.into())
             .collect();
 
         Ok(positions)
     }
+
+    fn __repr__(&self) -> String {
+        format!("Querier(db_path=\"{}\")", self.db_path)
+    }
 }
 
 // TODO(@nohehf): Indexer class
 
 #[pymethods]
 impl Position {
     #[new]
     fn new(path: String, line: usize, column: usize) -> Self {
         Position { path, line, column }
     }
+
+    fn __eq__(&self, other: &Position) -> bool {
+        self.path == other.path && self.line == other.line && self.column == other.column
+    }
+
+    fn __repr__(&self) -> String {
+        format!(
+            "Position(path=\"{}\", line={}, column={})",
+            self.path, self.line, self.column
+        )
+    }
 }
 
 impl Display for Position {
     fn fmt(&self, f: &mut std::fmt::Formatter<'_>) -> std::fmt::Result {
         write!(f, "{}:{}:{}", self.path, self.line, self.column)
     }
 }
```

### Comparing `stack_graphs_python_bindings-0.0.8/src/lib.rs` & `stack_graphs_python_bindings-0.0.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.8/src/stack_graphs_wrapper/mod.rs` & `stack_graphs_python_bindings-0.0.9/src/stack_graphs_wrapper/mod.rs`

 * *Files identical despite different names*

### Comparing `stack_graphs_python_bindings-0.0.8/tests/test.py` & `stack_graphs_python_bindings-0.0.9/tests/from_dir_test.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,36 @@
-# TODO(@nohehf): Make this a propper pytest test & run in CI
 import os
 from stack_graphs_python import index, Querier, Position, Language
 
-# index ./js_sample directory
 
-# convert ./js_sample directory to absolute path
-dir = os.path.abspath("./tests/js_sample")
-db_path = os.path.abspath("./db.sqlite")
+# index ./js_sample directory
+# This test is the same as the one in js_ok_test.py, without using the virtual file system helper
+def test_from_dir():
+    # convert ./js_sample directory to absolute path
+    dir = os.path.abspath("./tests/js_sample")
+    db_path = os.path.abspath("./db.sqlite")
 
-print("Indexing directory: ", dir)
-print("Database path: ", db_path)
+    print("Indexing directory: ", dir)
+    print("Database path: ", db_path)
 
-index([dir], db_path, language=Language.JavaScript)
+    index([dir], db_path, language=Language.JavaScript)
 
-source_reference = Position(path=dir + "/index.js", line=2, column=12)
+    source_reference = Position(path=dir + "/index.js", line=2, column=12)
 
-print("Querying definition for: ", source_reference.path)
+    print("Querying definition for: ", source_reference.path)
 
-querier = Querier(db_path)
+    querier = Querier(db_path)
 
-results = querier.definitions(source_reference)
+    results = querier.definitions(source_reference)
 
-print("Results: ", results)
+    print("Results: ", results)
 
-for result in results:
-    print("Path: ", result.path)
-    print("Line: ", result.line)
-    print("Column: ", result.column)
-    print("\n")
+    for result in results:
+        print("Path: ", result.path)
+        print("Line: ", result.line)
+        print("Column: ", result.column)
+        print("\n")
 
-assert len(results) == 2
-assert results[0].path.endswith("index.js")
-assert results[0].line == 0
-assert results[0].column == 9
+    assert len(results) == 2
+    assert results[0].path.endswith("index.js")
+    assert results[0].line == 0
+    assert results[0].column == 9
```

### Comparing `stack_graphs_python_bindings-0.0.8/Cargo.lock` & `stack_graphs_python_bindings-0.0.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1229,15 +1229,15 @@
  "serde_with",
  "smallvec",
  "thiserror",
 ]
 
 [[package]]
 name = "stack-graphs-python-bindings"
-version = "0.0.8"
+version = "0.0.9"
 dependencies = [
  "pyo3",
  "stack-graphs",
  "tree-sitter-stack-graphs",
  "tree-sitter-stack-graphs-java",
  "tree-sitter-stack-graphs-javascript",
  "tree-sitter-stack-graphs-python",
```

