# Comparing `tmp/rosa_python_client-1.0.93.tar.gz` & `tmp/rosa_python_client-1.0.94.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rosa_python_client-1.0.93.tar", max compression
+gzip compressed data, was "rosa_python_client-1.0.94.tar", max compression
```

## Comparing `rosa_python_client-1.0.93.tar` & `rosa_python_client-1.0.94.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      865 2024-05-21 06:40:55.343979 rosa_python_client-1.0.93/README.md
--rw-r--r--   0        0        0     1412 2024-05-21 06:41:00.161940 rosa_python_client-1.0.93/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-21 06:40:55.344979 rosa_python_client-1.0.93/rosa/__init__.py
--rw-r--r--   0        0        0    11119 2024-05-21 06:40:55.344979 rosa_python_client-1.0.93/rosa/cli.py
--rw-r--r--   0        0        0        0 2024-05-21 06:40:55.344979 rosa_python_client-1.0.93/rosa/tests/__init__.py
--rw-r--r--   0        0        0      843 2024-05-21 06:40:55.345979 rosa_python_client-1.0.93/rosa/tests/conftest.py
--rw-r--r--   0        0        0       30 2024-05-21 06:40:55.345979 rosa_python_client-1.0.93/rosa/tests/const.py
--rw-r--r--   0        0        0     1031 2024-05-21 06:40:55.345979 rosa_python_client-1.0.93/rosa/tests/test_parse_command.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.93/PKG-INFO
+-rw-r--r--   0        0        0      865 2024-05-22 09:45:27.168975 rosa_python_client-1.0.94/README.md
+-rw-r--r--   0        0        0     1412 2024-05-22 09:45:31.853938 rosa_python_client-1.0.94/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-22 09:45:27.169975 rosa_python_client-1.0.94/rosa/__init__.py
+-rw-r--r--   0        0        0    11119 2024-05-22 09:45:27.169975 rosa_python_client-1.0.94/rosa/cli.py
+-rw-r--r--   0        0        0        0 2024-05-22 09:45:27.169975 rosa_python_client-1.0.94/rosa/tests/__init__.py
+-rw-r--r--   0        0        0      843 2024-05-22 09:45:27.170975 rosa_python_client-1.0.94/rosa/tests/conftest.py
+-rw-r--r--   0        0        0       30 2024-05-22 09:45:27.170975 rosa_python_client-1.0.94/rosa/tests/const.py
+-rw-r--r--   0        0        0     1031 2024-05-22 09:45:27.170975 rosa_python_client-1.0.94/rosa/tests/test_parse_command.py
+-rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 rosa_python_client-1.0.94/PKG-INFO
```

### Comparing `rosa_python_client-1.0.93/README.md` & `rosa_python_client-1.0.94/README.md`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.93/pyproject.toml` & `rosa_python_client-1.0.94/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "rosa-python-client"
-version = "1.0.93"
+version = "1.0.94"
 description = "Wrapper for rosa cli"
 authors = ["Meni Yakove <myakove@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "rosa" }]
 license = "Apache-2.0"
 homepage = "https://github.com/RedHatQE/rosa-python-client"
 documentation = "https://github.com/RedHatQE/rosa-python-client/blob/main/README.md"
```

### Comparing `rosa_python_client-1.0.93/rosa/cli.py` & `rosa_python_client-1.0.94/rosa/cli.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.93/rosa/tests/conftest.py` & `rosa_python_client-1.0.94/rosa/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.93/rosa/tests/test_parse_command.py` & `rosa_python_client-1.0.94/rosa/tests/test_parse_command.py`

 * *Files identical despite different names*

### Comparing `rosa_python_client-1.0.93/PKG-INFO` & `rosa_python_client-1.0.94/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rosa-python-client
-Version: 1.0.93
+Version: 1.0.94
 Summary: Wrapper for rosa cli
 Home-page: https://github.com/RedHatQE/rosa-python-client
 License: Apache-2.0
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

