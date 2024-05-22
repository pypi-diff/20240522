# Comparing `tmp/pynenv-0.2.4.tar.gz` & `tmp/pynenv-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynenv-0.2.4.tar", max compression
+gzip compressed data, was "pynenv-0.2.5.tar", max compression
```

## Comparing `pynenv-0.2.4.tar` & `pynenv-0.2.5.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.4/LICENSE
--rw-r--r--   0        0        0      384 2024-05-22 17:40:28.797496 pynenv-0.2.4/README.md
--rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.4/pynenv/__init__.py
--rw-r--r--   0        0        0      916 2024-05-22 18:04:54.800029 pynenv-0.2.4/pynenv/environment.py
--rw-r--r--   0        0        0      362 2024-05-22 18:05:33.663786 pynenv-0.2.4/pyproject.toml
--rw-r--r--   0        0        0      829 1970-01-01 00:00:00.000000 pynenv-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-05-21 06:38:02.002239 pynenv-0.2.5/LICENSE
+-rw-r--r--   0        0        0      443 2024-05-22 18:07:00.388244 pynenv-0.2.5/README.md
+-rw-r--r--   0        0        0        0 2024-05-21 06:49:05.377202 pynenv-0.2.5/pynenv/__init__.py
+-rw-r--r--   0        0        0      916 2024-05-22 18:04:54.800029 pynenv-0.2.5/pynenv/environment.py
+-rw-r--r--   0        0        0      362 2024-05-22 18:07:43.630974 pynenv-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0      888 1970-01-01 00:00:00.000000 pynenv-0.2.5/PKG-INFO
```

### Comparing `pynenv-0.2.4/LICENSE` & `pynenv-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pynenv-0.2.4/pynenv/environment.py` & `pynenv-0.2.5/pynenv/environment.py`

 * *Files identical despite different names*

### Comparing `pynenv-0.2.4/PKG-INFO` & `pynenv-0.2.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pynenv
-Version: 0.2.4
+Version: 0.2.5
 Summary: General helper functions for environments
 Author: Nik Sheridan
 Author-email: niksheridan@duck.com
 Requires-Python: >=3.12,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: loguru (>=0.7.2,<0.8.0)
@@ -21,18 +21,19 @@
 ```bash
 pip install pynenv
 ```
 
 ## Example Useage
 
 ```python
-from pynenv.environment import get_environment_variable, json2file, yaml2file
+from pynenv.environment import get_environment_variable, json2dict, yaml2dict
 
-my_env_var = get_environment_variable('SOME_VAR')
-json_dict = json
+my_env_var = get_environment_variable('HOME')
+json_dict = json2dict('test_json.json')
+yaml_dict = yaml2dict('test_yaml.yaml')
 ```
 
 ## Build
 
 * Adjust version in ```pyproject.toml```
 * Run ```poetry build```
 * Run ```poetry publish```
```

