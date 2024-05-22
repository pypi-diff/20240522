# Comparing `tmp/rra_tools-1.0.7.tar.gz` & `tmp/rra_tools-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rra_tools-1.0.7.tar", max compression
+gzip compressed data, was "rra_tools-1.0.8.tar", max compression
```

## Comparing `rra_tools-1.0.7.tar` & `rra_tools-1.0.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1517 2024-05-15 05:29:59.404272 rra_tools-1.0.7/LICENSE
--rw-r--r--   0        0        0    12799 2024-05-15 05:29:59.404272 rra_tools-1.0.7/README.md
--rw-r--r--   0        0        0     3749 2024-05-15 05:29:59.404272 rra_tools-1.0.7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-15 05:29:59.404272 rra_tools-1.0.7/src/rra_tools/__init__.py
--rw-r--r--   0        0        0      745 2024-05-15 05:29:59.404272 rra_tools-1.0.7/src/rra_tools/cli_tools/__init__.py
--rw-r--r--   0        0        0      983 2024-05-15 05:29:59.404272 rra_tools-1.0.7/src/rra_tools/cli_tools/exceptions.py
--rw-r--r--   0        0        0      410 2024-05-15 05:29:59.404272 rra_tools-1.0.7/src/rra_tools/cli_tools/importers.py
--rw-r--r--   0        0        0     5439 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/cli_tools/options.py
--rw-r--r--   0        0        0     4694 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/jobmon.py
--rw-r--r--   0        0        0      415 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/logging/__init__.py
--rw-r--r--   0        0        0     2235 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/logging/config.py
--rw-r--r--   0        0        0     3981 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/logging/performance.py
--rw-r--r--   0        0        0      605 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/logging/protocol.py
--rw-r--r--   0        0        0     3082 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/parallel.py
--rw-r--r--   0        0        0        0 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/py.typed
--rw-r--r--   0        0        0     3031 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/shell_tools.py
--rw-r--r--   0        0        0     2466 2024-05-15 05:29:59.408272 rra_tools-1.0.7/src/rra_tools/translate.py
--rw-r--r--   0        0        0    13990 1970-01-01 00:00:00.000000 rra_tools-1.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1517 2024-05-22 04:20:07.505825 rra_tools-1.0.8/LICENSE
+-rw-r--r--   0        0        0    12799 2024-05-22 04:20:07.505825 rra_tools-1.0.8/README.md
+-rw-r--r--   0        0        0     3770 2024-05-22 04:20:07.509825 rra_tools-1.0.8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/__init__.py
+-rw-r--r--   0        0        0      745 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/__init__.py
+-rw-r--r--   0        0        0      983 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/exceptions.py
+-rw-r--r--   0        0        0      410 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/importers.py
+-rw-r--r--   0        0        0     5439 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/cli_tools/options.py
+-rw-r--r--   0        0        0    10244 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/jobmon.py
+-rw-r--r--   0        0        0      415 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/__init__.py
+-rw-r--r--   0        0        0     2235 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/config.py
+-rw-r--r--   0        0        0     3981 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/performance.py
+-rw-r--r--   0        0        0      605 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/logging/protocol.py
+-rw-r--r--   0        0        0     3082 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/parallel.py
+-rw-r--r--   0        0        0        0 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/py.typed
+-rw-r--r--   0        0        0     3031 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/shell_tools.py
+-rw-r--r--   0        0        0     2466 2024-05-22 04:20:07.509825 rra_tools-1.0.8/src/rra_tools/translate.py
+-rw-r--r--   0        0        0    14032 1970-01-01 00:00:00.000000 rra_tools-1.0.8/PKG-INFO
```

### Comparing `rra_tools-1.0.7/LICENSE` & `rra_tools-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/README.md` & `rra_tools-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/pyproject.toml` & `rra_tools-1.0.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rra-tools"
-version = "1.0.7"
+version = "1.0.8"
 description = "Common utilities for IHME Rapid Response team pipelines."
 authors = [
     "James Collins <collijk@uw.edu>",
 ]
 license = "BSD-3-Clause"
 readme = "README.md"
 
@@ -33,14 +33,15 @@
 python = ">=3.10, <4.0"
 click = "*"
 pandas = "^2.2.2"
 deep-translator = "^1.11.4"
 tqdm = "^4.66.4"
 pathos = "^0.3.2"
 loguru = "^0.7.2"
+requests = "^2.32.2"
 
 [tool.poetry.group.dev.dependencies]
 mkdocstrings = {version = ">=0.23", extras = ["python"]}
 mkdocs-material = "*"
 mkdocs-table-reader-plugin = "*"
 mypy = "*"
 pre-commit = "*"
```

### Comparing `rra_tools-1.0.7/src/rra_tools/cli_tools/__init__.py` & `rra_tools-1.0.8/src/rra_tools/cli_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/cli_tools/exceptions.py` & `rra_tools-1.0.8/src/rra_tools/cli_tools/exceptions.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/cli_tools/options.py` & `rra_tools-1.0.8/src/rra_tools/cli_tools/options.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/logging/config.py` & `rra_tools-1.0.8/src/rra_tools/logging/config.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/logging/performance.py` & `rra_tools-1.0.8/src/rra_tools/logging/performance.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/logging/protocol.py` & `rra_tools-1.0.8/src/rra_tools/logging/protocol.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/parallel.py` & `rra_tools-1.0.8/src/rra_tools/parallel.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/shell_tools.py` & `rra_tools-1.0.8/src/rra_tools/shell_tools.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/src/rra_tools/translate.py` & `rra_tools-1.0.8/src/rra_tools/translate.py`

 * *Files identical despite different names*

### Comparing `rra_tools-1.0.7/PKG-INFO` & `rra_tools-1.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rra-tools
-Version: 1.0.7
+Version: 1.0.8
 Summary: Common utilities for IHME Rapid Response team pipelines.
 Home-page: https://collijk.github.io/rra-tools
 License: BSD-3-Clause
 Author: James Collins
 Author-email: collijk@uw.edu
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,14 +19,15 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Typing :: Typed
 Requires-Dist: click
 Requires-Dist: deep-translator (>=1.11.4,<2.0.0)
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
 Requires-Dist: pandas (>=2.2.2,<3.0.0)
 Requires-Dist: pathos (>=0.3.2,<0.4.0)
+Requires-Dist: requests (>=2.32.2,<3.0.0)
 Requires-Dist: tqdm (>=4.66.4,<5.0.0)
 Project-URL: Documentation, https://collijk.github.io/rra-tools
 Project-URL: Repository, https://github.com/collijk/rra-tools
 Description-Content-Type: text/markdown
 
 # RRA Tools
```

