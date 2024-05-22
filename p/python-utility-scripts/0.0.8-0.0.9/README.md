# Comparing `tmp/python_utility_scripts-0.0.8.tar.gz` & `tmp/python_utility_scripts-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_utility_scripts-0.0.8.tar", max compression
+gzip compressed data, was "python_utility_scripts-0.0.9.tar", max compression
```

## Comparing `python_utility_scripts-0.0.8.tar` & `python_utility_scripts-0.0.9.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0    11357 2024-03-20 23:44:15.613699 python_utility_scripts-0.0.8/LICENSE
--rw-r--r--   0        0        0     1297 2024-03-20 23:44:15.613699 python_utility_scripts-0.0.8/README.md
--rw-r--r--   0        0        0        0 2024-03-20 23:44:15.613699 python_utility_scripts-0.0.8/apps/__init__.py
--rw-r--r--   0        0        0     1021 2024-03-20 23:44:15.613699 python_utility_scripts-0.0.8/apps/unused_code/README.md
--rw-r--r--   0        0        0        0 2024-03-20 23:44:15.613699 python_utility_scripts-0.0.8/apps/unused_code/__init__.py
--rw-r--r--   0        0        0     3621 2024-03-20 23:44:15.614699 python_utility_scripts-0.0.8/apps/unused_code/unused_code.py
--rw-r--r--   0        0        0     2279 2024-03-20 23:44:15.614699 python_utility_scripts-0.0.8/apps/utils.py
--rw-r--r--   0        0        0     1363 2024-03-20 23:44:20.652678 python_utility_scripts-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 python_utility_scripts-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-03-25 19:10:31.485277 python_utility_scripts-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1297 2024-03-25 19:10:31.485277 python_utility_scripts-0.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-25 19:10:31.485277 python_utility_scripts-0.0.9/apps/__init__.py
+-rw-r--r--   0        0        0     1021 2024-03-25 19:10:31.485277 python_utility_scripts-0.0.9/apps/unused_code/README.md
+-rw-r--r--   0        0        0        0 2024-03-25 19:10:31.488277 python_utility_scripts-0.0.9/apps/unused_code/__init__.py
+-rw-r--r--   0        0        0     3621 2024-03-25 19:10:31.488277 python_utility_scripts-0.0.9/apps/unused_code/unused_code.py
+-rw-r--r--   0        0        0     2279 2024-03-25 19:10:31.488277 python_utility_scripts-0.0.9/apps/utils.py
+-rw-r--r--   0        0        0     1363 2024-03-25 19:10:35.522258 python_utility_scripts-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2298 1970-01-01 00:00:00.000000 python_utility_scripts-0.0.9/PKG-INFO
```

### Comparing `python_utility_scripts-0.0.8/LICENSE` & `python_utility_scripts-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `python_utility_scripts-0.0.8/README.md` & `python_utility_scripts-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `python_utility_scripts-0.0.8/apps/unused_code/README.md` & `python_utility_scripts-0.0.9/apps/unused_code/README.md`

 * *Files identical despite different names*

### Comparing `python_utility_scripts-0.0.8/apps/unused_code/unused_code.py` & `python_utility_scripts-0.0.9/apps/unused_code/unused_code.py`

 * *Files identical despite different names*

### Comparing `python_utility_scripts-0.0.8/apps/utils.py` & `python_utility_scripts-0.0.9/apps/utils.py`

 * *Files identical despite different names*

### Comparing `python_utility_scripts-0.0.8/pyproject.toml` & `python_utility_scripts-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "python-utility-scripts"
-version = "0.0.8"
+version = "0.0.9"
 description = "Python utility scripts"
 authors = ["dbasunag <dbasunag@redhat.com>"]
 license = "Apache License 2.0"
 readme = "README.md"
 repository = "https://github.com/RedHatQE/python-utility-scripts"
 homepage = "https://github.com/RedHatQE/python-utility-scripts"
 documentation = "https://github.com/RedHatQE/python-utility-scripts/blob/main/README.md"
```

### Comparing `python_utility_scripts-0.0.8/PKG-INFO` & `python_utility_scripts-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-utility-scripts
-Version: 0.0.8
+Version: 0.0.9
 Summary: Python utility scripts
 Home-page: https://github.com/RedHatQE/python-utility-scripts
 License: Apache-2.0
 Author: dbasunag
 Author-email: dbasunag@redhat.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

