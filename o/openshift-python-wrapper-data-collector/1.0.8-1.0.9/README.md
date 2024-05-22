# Comparing `tmp/openshift_python_wrapper_data_collector-1.0.8.tar.gz` & `tmp/openshift_python_wrapper_data_collector-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openshift_python_wrapper_data_collector-1.0.8.tar", max compression
+gzip compressed data, was "openshift_python_wrapper_data_collector-1.0.9.tar", max compression
```

## Comparing `openshift_python_wrapper_data_collector-1.0.8.tar` & `openshift_python_wrapper_data_collector-1.0.9.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11357 2024-01-28 09:51:56.695312 openshift_python_wrapper_data_collector-1.0.8/LICENSE
--rw-r--r--   0        0        0     1017 2024-01-28 09:51:56.695312 openshift_python_wrapper_data_collector-1.0.8/README.md
--rw-r--r--   0        0        0        0 2024-01-28 09:51:56.696312 openshift_python_wrapper_data_collector-1.0.8/ocp_wrapper_data_collector/__init__.py
--rw-r--r--   0        0        0    10965 2024-01-28 09:51:56.696312 openshift_python_wrapper_data_collector-1.0.8/ocp_wrapper_data_collector/data_collector.py
--rw-r--r--   0        0        0     1648 2024-01-28 09:52:01.375267 openshift_python_wrapper_data_collector-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 openshift_python_wrapper_data_collector-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-01-28 13:56:39.807278 openshift_python_wrapper_data_collector-1.0.9/LICENSE
+-rw-r--r--   0        0        0     1017 2024-01-28 13:56:39.807278 openshift_python_wrapper_data_collector-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-01-28 13:56:39.807278 openshift_python_wrapper_data_collector-1.0.9/ocp_wrapper_data_collector/__init__.py
+-rw-r--r--   0        0        0    10965 2024-01-28 13:56:39.807278 openshift_python_wrapper_data_collector-1.0.9/ocp_wrapper_data_collector/data_collector.py
+-rw-r--r--   0        0        0     1648 2024-01-28 13:56:44.421234 openshift_python_wrapper_data_collector-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2300 1970-01-01 00:00:00.000000 openshift_python_wrapper_data_collector-1.0.9/PKG-INFO
```

### Comparing `openshift_python_wrapper_data_collector-1.0.8/LICENSE` & `openshift_python_wrapper_data_collector-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openshift_python_wrapper_data_collector-1.0.8/README.md` & `openshift_python_wrapper_data_collector-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `openshift_python_wrapper_data_collector-1.0.8/ocp_wrapper_data_collector/data_collector.py` & `openshift_python_wrapper_data_collector-1.0.9/ocp_wrapper_data_collector/data_collector.py`

 * *Files identical despite different names*

### Comparing `openshift_python_wrapper_data_collector-1.0.8/pyproject.toml` & `openshift_python_wrapper_data_collector-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 output-format = "grouped"
 
 [tool.ruff.format]
 exclude = [".git", ".venv", ".mypy_cache", ".tox", "__pycache__"]
 
 [tool.poetry]
 name = "openshift-python-wrapper-data-collector"
-version = "1.0.8"
+version = "1.0.9"
 description = "Data collector for https://github.com/openshift/openshift-python-wrapper when running with PyTest"
 authors = ["Meni Yakove <myakove@gmail.com>", "Ruth Netser <rnetser@gmail.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://github.com/RedHatQE/openshift-python-wrapper-data-collector"
 documentation = "https://github.com/RedHatQE/openshift-python-wrapper-data-collector/blob/main/README.md"
 keywords = ["Openshift", "OCP"]
```

### Comparing `openshift_python_wrapper_data_collector-1.0.8/PKG-INFO` & `openshift_python_wrapper_data_collector-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openshift-python-wrapper-data-collector
-Version: 1.0.8
+Version: 1.0.9
 Summary: Data collector for https://github.com/openshift/openshift-python-wrapper when running with PyTest
 Home-page: https://github.com/RedHatQE/openshift-python-wrapper-data-collector
 License: Apache-2.0
 Keywords: Openshift,OCP
 Author: Meni Yakove
 Author-email: myakove@gmail.com
 Requires-Python: >=3.8,<4.0
```

