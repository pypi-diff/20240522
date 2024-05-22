# Comparing `tmp/luxos-0.0.8b26.tar.gz` & `tmp/luxos-0.0.8b27.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "luxos-0.0.8b26.tar", last modified: Wed May 15 14:35:56 2024, max compression
+gzip compressed data, was "luxos-0.0.8b27.tar", last modified: Wed May 22 14:46:52 2024, max compression
```

## Comparing `luxos-0.0.8b26.tar` & `luxos-0.0.8b27.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-15 14:35:56.927947 luxos-0.0.8b26/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-15 14:35:24.000000 luxos-0.0.8b26/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-15 14:35:54.000000 luxos-0.0.8b26/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 14:35:56.927947 luxos-0.0.8b26/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.919947 luxos-0.0.8b26/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-15 14:35:54.000000 luxos-0.0.8b26/src/luxos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       75 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/api.json
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10357 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/asyncops.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8252 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/cli/v1.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.923947 luxos-0.0.8b26/src/luxos/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/async_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/health_checker.py
--rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/scripts/luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/text.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-05-15 14:35:24.000000 luxos-0.0.8b26/src/luxos/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/src/luxos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 14:35:56.000000 luxos-0.0.8b26/src/luxos.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 14:35:56.927947 luxos-0.0.8b26/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     6339 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_asyncops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_luxos.py
--rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_text.py
--rw-r--r--   0 runner    (1001) docker     (127)     3065 2024-05-15 14:35:24.000000 luxos-0.0.8b26/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-22 14:46:52.508378 luxos-0.0.8b27/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5343 2024-05-22 14:46:27.000000 luxos-0.0.8b27/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2107 2024-05-22 14:46:50.000000 luxos-0.0.8b27/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 14:46:52.508378 luxos-0.0.8b27/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.504378 luxos-0.0.8b27/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/src/luxos/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-22 14:46:50.000000 luxos-0.0.8b27/src/luxos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/api.json
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10342 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/asyncops.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/src/luxos/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8207 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/cli/v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/src/luxos/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1632 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/scripts/async_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30158 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/scripts/health_checker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12200 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/scripts/luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-22 14:46:27.000000 luxos-0.0.8b27/src/luxos/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/src/luxos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6175 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      715 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-22 14:46:52.000000 luxos-0.0.8b27/src/luxos.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 14:46:52.508378 luxos-0.0.8b27/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6324 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_asyncops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_luxos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      660 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3066 2024-05-22 14:46:27.000000 luxos-0.0.8b27/tests/test_utils.py
```

### Comparing `luxos-0.0.8b26/PKG-INFO` & `luxos-0.0.8b27/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.8b26
+Version: 0.0.8b27
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.8b26/README.md` & `luxos-0.0.8b27/README.md`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/pyproject.toml` & `luxos-0.0.8b27/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "luxos"
-version = "0.0.8b26"
+version = "0.0.8b27"
 description = "The all encompassing LuxOS python library."
 readme = "README.md"
 license = { text = "MIT" }  # TODO I don't think this is a MIT??
 requires-python = ">= 3.9"
 
 authors = [
   { name = "Antonio Cavallo", email = "antonio.cavallo@luxor.tech" },
@@ -45,28 +45,47 @@
 [tool.setuptools.package-data]
 'luxos' = ['*.json', 'py.typed']
 
 
 [tool.ruff]
 target-version = "py39"
 line-length = 88
-
+src = ["src/luxos"]
+exclude = [
+    "src/luxos/scripts/health_checker.py",
+    "src/luxos/scripts/luxos.py"
+]
 
 [tool.ruff.format]
 quote-style = "double"
 
+[tool.ruff.lint]
+ignore = []
+select = ["F", "E", "W", "Q", "I001"]
+
+[tool.ruff.lint.isort]
+known-first-party = ["luxos"]
+
+
 [tool.mypy]
 disallow_untyped_defs = false
 follow_imports = "normal"
 ignore_missing_imports = true
 pretty = true
 show_column_numbers = true
 show_error_codes = true
 warn_no_return = false
 warn_unused_ignores = true
+exclude = [
+    "^make\\.py",
+    "docs/conf\\.py",
+    "^docs/\\.*",
+    "^build/\\.*",
+    "^src/luxos/scripts/health_checker\\.py"
+]
 
 [tool.coverage.run]
 branch = true
 
 [tool.coverage.paths]
 source = [
   "src/",
```

### Comparing `luxos-0.0.8b26/src/luxos/api.json` & `luxos-0.0.8b27/src/luxos/api.json`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/src/luxos/api.py` & `luxos-0.0.8b27/src/luxos/api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 from __future__ import annotations
 
-import logging
-import json
 import importlib.resources
+import json
+import logging
 
 log = logging.getLogger(__name__)
 
 
-COMMANDS = json.loads(
-    (importlib.resources.files("luxos") / "api.json")
-    .read_text()
-)
+COMMANDS = json.loads((importlib.resources.files("luxos") / "api.json").read_text())
 
 
 def logon_required(cmd: str, commands_list=COMMANDS) -> bool | None:
     # Check if the command requires logon to LuxOS API
 
     if cmd not in COMMANDS:
-        log.info("%s command is not supported. "
-                 "Try again with a different command.", cmd)
+        log.info(
+            "%s command is not supported. " "Try again with a different command.", cmd
+        )
         return None
 
     return COMMANDS[cmd]["logon_required"]
 
 
 # TODO timeouts should be float | None
-def execute_command(host: str, port: int, timeout: int, cmd: str, params: list[str], verbose: bool):
+def execute_command(
+    host: str, port: int, timeout: int, cmd: str, params: list[str], verbose: bool
+):
     from .scripts import luxos
-    return luxos.execute_command(host, port, timeout, cmd, params, verbose)
-
 
+    return luxos.execute_command(host, port, timeout, cmd, params, verbose)
```

### Comparing `luxos-0.0.8b26/src/luxos/asyncops.py` & `luxos-0.0.8b27/src/luxos/asyncops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 from __future__ import annotations
 
-import functools
-import logging
 import asyncio
+import functools
 import json
-
+import logging
 from typing import Any
 
-from . import exceptions
-from . import api
-
+from . import api, exceptions
 
 log = logging.getLogger(__name__)
 
 TIMEOUT = 3.0  # default timeout for operations
 RETRY = 0  # default number (>1) of retry on a failed operation
 RETRY_DELAY = 1.0  # delay between retry
```

### Comparing `luxos-0.0.8b26/src/luxos/cli/v1.py` & `luxos-0.0.8b27/src/luxos/cli/v1.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,28 +86,28 @@
 
 ```
 
 """
 
 from __future__ import annotations
 
-import sys
+import argparse
 import contextlib
+import functools
 import inspect
 import logging
+import sys
 import time
 from pathlib import Path
-import functools
-import argparse
-from typing import Callable, Any
-
+from typing import Any, Callable
 
 # SPECIAL MODULE LEVEL VARIABLES
 MODULE_VARIABLES = {
-    "LOGGING_CONFIG": None,  # logging config dict (passed to logging.basicConfig(**LOGGING_CONFIG))
+    "LOGGING_CONFIG": None,  # logging config dict
+    # (passed to logging.basicConfig(**LOGGING_CONFIG))
     "CONFIGPATH": Path("config.yaml"),  # config default path
 }
 
 
 log = logging.getLogger(__name__)
 
 
@@ -156,34 +156,33 @@
         )
         self.add_argument("-q", "--quiet", action="count", help="report quiet logging")
 
         # we add the -c|--config flag to point to a config file
         configpath = (
             self.module_variables.get("CONFIGPATH") or MODULE_VARIABLES["CONFIGPATH"]
         )
-        configpath = Path(configpath).expanduser().absolute()
-        if configpath.is_relative_to(Path.cwd()):
-            configpath = configpath.relative_to(Path.cwd())
+        if configpath:
+            configpath = Path(configpath).expanduser().absolute()
+            if configpath.is_relative_to(Path.cwd()):
+                configpath = configpath.relative_to(Path.cwd())
 
         self.add_argument(
             "-c",
             "--config",
             default=configpath,
             type=Path,
             help="path to a config file",
         )
 
+    def error(self, message: str):
+        raise AbortWrongArgument(message)
+
     def parse_args(self, args=None, namespace=None):
         options = super().parse_args(args, namespace)
 
-        # we provide an error function to nicely bail out the script
-        def error(msg):
-            raise AbortWrongArgument(msg)
-
-        self.error = error
         options.error = self.error
 
         # setup the logging
         config = {}
         if value := self.module_variables.get("LOGGING_CONFIG"):
             config = value.copy()
```

### Comparing `luxos-0.0.8b26/src/luxos/exceptions.py` & `luxos-0.0.8b27/src/luxos/exceptions.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,16 +4,18 @@
 
 class MinerConnectionError(LuxosBaseException):
     def __init__(self, host: str, port: int, *args, **kwargs):
         super().__init__(host, port, *args, **kwargs)
         self.address = (host, port)
 
     def __str__(self):
-        return (f"<{self.address[0]}:{self.address[1]}>: {self.__class__.__name__}, "
-                f"{self.args[2] if self.args[2:] else 'unknown reason'}")
+        return (
+            f"<{self.address[0]}:{self.address[1]}>: {self.__class__.__name__}, "
+            f"{self.args[2] if self.args[2:] else 'unknown reason'}"
+        )
 
 
 class MinerCommandSessionAlreadyActive(MinerConnectionError):
     pass
 
 
 class MinerCommandTimeoutError(MinerConnectionError):
```

### Comparing `luxos-0.0.8b26/src/luxos/misc.py` & `luxos-0.0.8b27/src/luxos/misc.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # catch-all module (find later a better place)
 from __future__ import annotations
-import sys
-import itertools
+
 import ipaddress
+import itertools
+import sys
 from typing import Generator
 
 if sys.version_info >= (3, 12):
     batched = itertools.batched
 else:
 
     def batched(iterable, n):
```

### Comparing `luxos-0.0.8b26/src/luxos/scripts/async_luxos.py` & `luxos-0.0.8b27/src/luxos/scripts/async_luxos.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from __future__ import annotations
+
 import asyncio
 import json
 
-from .. import misc
-from .. import text
-from .. import asyncops
+from .. import asyncops, misc, text
 
 
 async def run(
     ipaddresses: list[str],
     port: int,
     cmd: str,
     params: list[str],
```

### Comparing `luxos-0.0.8b26/src/luxos/scripts/health_checker.py` & `luxos-0.0.8b27/src/luxos/scripts/health_checker.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/src/luxos/scripts/luxos.py` & `luxos-0.0.8b27/src/luxos/scripts/luxos.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/src/luxos/text.py` & `luxos-0.0.8b27/src/luxos/text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from __future__ import annotations
+
 import io
 
 
 def indent(txt: str, pre: str = " " * 2) -> str:
     """simple text indentation"""
 
     from textwrap import dedent
```

### Comparing `luxos-0.0.8b26/src/luxos/utils.py` & `luxos-0.0.8b27/src/luxos/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """user facing functions for normal use"""
 
 from __future__ import annotations
+
 import asyncio
 from pathlib import Path
 from typing import Any, Callable
 
-from luxos.asyncops import rexec  # noqa: F401
 import luxos.misc
+from luxos.asyncops import rexec  # noqa: F401
 
 
 def ip_ranges(txt: str, gsep: str = ":", rsep: str = "-") -> list[str]:
     """return a list of ips given a text expression.
 
     Eg.
         >>> for ip in ip_ranges("127.0.0.1"):
```

### Comparing `luxos-0.0.8b26/src/luxos.egg-info/PKG-INFO` & `luxos-0.0.8b27/src/luxos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: luxos
-Version: 0.0.8b26
+Version: 0.0.8b27
 Summary: The all encompassing LuxOS python library.
 Author-email: Antonio Cavallo <antonio.cavallo@luxor.tech>
 License: MIT
 Project-URL: Source, https://github.com/LuxorLabs/firmware-biz-tools
 Project-URL: Issues, https://github.com/LuxorLabs/firmware-biz-tools/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
```

### Comparing `luxos-0.0.8b26/src/luxos.egg-info/SOURCES.txt` & `luxos-0.0.8b27/src/luxos.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/tests/test_asyncops.py` & `luxos-0.0.8b27/tests/test_asyncops.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from __future__ import annotations
 
-import os
 import asyncio
+import os
+
 import pytest
+
 import luxos.asyncops as aapi
-from luxos import exceptions
-from luxos import misc
+from luxos import exceptions, misc
 
 ## NOTE ##
 # This tests spawn an underlying server, it might be better not run
 # unattended. Some also require a miner, we might not have it handy.
 pytestmark = pytest.mark.manual
 
 
@@ -155,16 +156,16 @@
     assert len(res["VERSION"]) == 1
     assert "API" in res["VERSION"][0]
 
 
 @pytest.mark.skipif(not getminer(), reason="need to set LUXOS_TEST_MINER")
 @pytest.mark.asyncio
 async def test_miner_profile_sets():
-    from string import ascii_lowercase
     from random import choices
+    from string import ascii_lowercase
 
     # random profile name
     profile = f"test-{''.join(choices(ascii_lowercase, k=5))}"
 
     # get the initial profile list
     host, port = getminer()
     profiles = (await aapi.rexec(host, port, "profiles"))["PROFILES"]
```

### Comparing `luxos-0.0.8b26/tests/test_cli.py` & `luxos-0.0.8b27/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/tests/test_misc.py` & `luxos-0.0.8b27/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `luxos-0.0.8b26/tests/test_text.py` & `luxos-0.0.8b27/tests/test_text.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+# ruff: noqa: W291, W293
 import pytest
 
 from luxos import text
 
 try:
     import rich
 except ModuleNotFoundError:
```

### Comparing `luxos-0.0.8b26/tests/test_utils.py` & `luxos-0.0.8b27/tests/test_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 ## NOTE ##
 # Some of these tests spawn an underlying server, it might be better not run
 # unattended. Some also require a miner, we might not have it handy.
 import asyncio
 
 import pytest
+
 import luxos.asyncops
 from luxos import utils
 
 
 @pytest.mark.manual
 @pytest.mark.asyncio
 async def test_basic_call(echopool):
```

