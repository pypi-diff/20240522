# Comparing `tmp/styxdefs-0.1.1.tar.gz` & `tmp/styxdefs-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "styxdefs-0.1.1.tar", max compression
+gzip compressed data, was "styxdefs-0.1.2.tar", max compression
```

## Comparing `styxdefs-0.1.1.tar` & `styxdefs-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1077 2024-05-21 21:29:50.928169 styxdefs-0.1.1/LICENSE
--rw-r--r--   0        0        0      870 2024-05-21 21:29:50.928169 styxdefs-0.1.1/README.md
--rw-r--r--   0        0        0     1564 2024-05-21 21:29:50.928169 styxdefs-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      418 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/__init__.py
--rw-r--r--   0        0        0     2720 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/runner.py
--rw-r--r--   0        0        0     2354 2024-05-21 21:29:50.928169 styxdefs-0.1.1/src/styxdefs/types.py
--rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 styxdefs-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-05-22 14:04:03.003202 styxdefs-0.1.2/LICENSE
+-rw-r--r--   0        0        0      870 2024-05-22 14:04:03.007202 styxdefs-0.1.2/README.md
+-rw-r--r--   0        0        0     1564 2024-05-22 14:04:03.007202 styxdefs-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      418 2024-05-22 14:04:03.007202 styxdefs-0.1.2/src/styxdefs/__init__.py
+-rw-r--r--   0        0        0     3670 2024-05-22 14:04:03.007202 styxdefs-0.1.2/src/styxdefs/runner.py
+-rw-r--r--   0        0        0     2354 2024-05-22 14:04:03.007202 styxdefs-0.1.2/src/styxdefs/types.py
+-rw-r--r--   0        0        0     1378 1970-01-01 00:00:00.000000 styxdefs-0.1.2/PKG-INFO
```

### Comparing `styxdefs-0.1.1/LICENSE` & `styxdefs-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.1/README.md` & `styxdefs-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.1/pyproject.toml` & `styxdefs-0.1.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "styxdefs"
-version = "0.1.1"
+version = "0.1.2"
 description = "Styx definitions and minimal runtime"
 authors = ["Florian Rupprecht <33600480+nx10@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 packages = [{include = "styxdefs", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `styxdefs-0.1.1/src/styxdefs/runner.py` & `styxdefs-0.1.2/src/styxdefs/runner.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,27 +1,75 @@
 """Default runner implementation."""
 
 import logging
+import os
+import pathlib
 from collections import deque
 from concurrent.futures import ThreadPoolExecutor
 from functools import partial
 from subprocess import PIPE, CalledProcessError, Popen
 
 from .types import Execution, InputPathType, Metadata, OutputPathType, Runner
 
 
-class DefaultRunner(Runner, Execution):
+class _DefaultExecution(Execution):
+    """Default execution implementation."""
+
+    def __init__(self, logger: logging.Logger, dir: pathlib.Path) -> None:
+        """Initialize the execution."""
+        self.logger: logging.Logger = logger
+        self.dir: pathlib.Path = dir
+
+    def input_file(self, host_file: InputPathType) -> str:
+        """Resolve host input files."""
+        return str(pathlib.Path(host_file).absolute())
+
+    def output_file(self, local_file: str, optional: bool = False) -> OutputPathType:
+        """Resolve local output files."""
+        return str(self.dir / local_file)
+
+    def run(self, cargs: list[str]) -> None:
+        """Run the command."""
+        self.last_cargs = cargs
+
+        def _stdout_handler(line: str) -> None:
+            self.logger.info(line)
+
+        def _stderr_handler(line: str) -> None:
+            self.logger.error(line)
+
+        while self.dir.exists():
+            self.logger.warning(
+                f"Execution directory {self.dir} already exists. Trying another."
+            )
+            self.dir = self.dir.with_name(f"{self.dir.name}_1")
+        self.dir.mkdir(parents=True, exist_ok=True)
+
+        with Popen(cargs, text=True, stdout=PIPE, stderr=PIPE, cwd=self.dir) as process:
+            with ThreadPoolExecutor(2) as pool:  # two threads to handle the streams
+                exhaust = partial(pool.submit, partial(deque, maxlen=0))
+                exhaust(_stdout_handler(line[:-1]) for line in process.stdout)  # type: ignore
+                exhaust(_stderr_handler(line[:-1]) for line in process.stderr)  # type: ignore
+        return_code = process.poll()
+        if return_code:
+            raise CalledProcessError(return_code, process.args)
+
+
+class DefaultRunner(Runner):
     """Default runner implementation."""
 
     logger_name = "styx_default_runner"
 
-    def __init__(self) -> None:
+    def __init__(self, data_dir: InputPathType | None = None) -> None:
         """Initialize the runner."""
         self.last_cargs: list[str] | None = None
         self.last_metadata: Metadata | None = None
+        self.data_dir = pathlib.Path(data_dir or "styx_tmp")
+        self.uid = os.urandom(8).hex()
+        self.execution_counter = 0
 
         # Configure logger
         self.logger = logging.getLogger(self.logger_name)
         if not self.logger.hasHandlers():
             self.logger.setLevel(logging.DEBUG)
             ch = logging.StreamHandler()
             ch.setLevel(logging.DEBUG)
@@ -30,42 +78,18 @@
             )
             ch.setFormatter(formatter)
             self.logger.addHandler(ch)
 
     def start_execution(self, metadata: Metadata) -> Execution:
         """Start a new execution."""
         self.last_metadata = metadata
-        return self
-
-    def input_file(self, host_file: InputPathType) -> str:
-        """Resolve host input files."""
-        return str(host_file)
-
-    def output_file(self, local_file: str, optional: bool = False) -> OutputPathType:
-        """Resolve local output files."""
-        return local_file
-
-    def run(self, cargs: list[str]) -> None:
-        """Run the command."""
-        self.last_cargs = cargs
-
-        def stdout_handler(line: str) -> None:
-            self.logger.info(line)
-
-        def stderr_handler(line: str) -> None:
-            self.logger.error(line)
-
-        with Popen(cargs, text=True, stdout=PIPE, stderr=PIPE) as process:
-            with ThreadPoolExecutor(2) as pool:  # two threads to handle the streams
-                exhaust = partial(pool.submit, partial(deque, maxlen=0))
-                exhaust(stdout_handler(line[:-1]) for line in process.stdout)  # type: ignore
-                exhaust(stderr_handler(line[:-1]) for line in process.stderr)  # type: ignore
-        return_code = process.poll()
-        if return_code:
-            raise CalledProcessError(return_code, process.args)
+        return _DefaultExecution(
+            logger=self.logger,
+            dir=self.data_dir / f"{self.uid}_{self.execution_counter}_{metadata.name}",
+        )
 
 
 _DEFAULT_RUNNER: DefaultRunner | None = None
 
 
 def get_global_runner() -> DefaultRunner:
     """Get the default runner."""
```

### Comparing `styxdefs-0.1.1/src/styxdefs/types.py` & `styxdefs-0.1.2/src/styxdefs/types.py`

 * *Files identical despite different names*

### Comparing `styxdefs-0.1.1/PKG-INFO` & `styxdefs-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: styxdefs
-Version: 0.1.1
+Version: 0.1.2
 Summary: Styx definitions and minimal runtime
 License: MIT
 Author: Florian Rupprecht
 Author-email: 33600480+nx10@users.noreply.github.com
 Requires-Python: >=3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

