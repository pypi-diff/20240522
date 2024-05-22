# Comparing `tmp/packaging_demo_avr-0.0.8.tar.gz` & `tmp/packaging_demo_avr-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packaging_demo_avr-0.0.8.tar", last modified: Sat May 18 16:01:03 2024, max compression
+gzip compressed data, was "packaging_demo_avr-0.0.9.tar", last modified: Sat May 18 16:19:30 2024, max compression
```

## Comparing `packaging_demo_avr-0.0.8.tar` & `packaging_demo_avr-0.0.9.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:01:03.841466 packaging_demo_avr-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 16:01:03.841466 packaging_demo_avr-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    31246 2024-05-18 16:00:58.000000 packaging_demo_avr-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:01:03.837466 packaging_demo_avr-0.0.8/packaging_demo/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 16:00:58.000000 packaging_demo_avr-0.0.8/packaging_demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/cities.json
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/colorized_demo.py
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:01:03.837466 packaging_demo_avr-0.0.8/packaging_demo/my_folder/
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_folder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_folder/another-cities.json
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_folder/my_nested_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:01:03.837466 packaging_demo_avr-0.0.8/packaging_demo/my_folder/my_sub_package/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_folder/my_sub_package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_folder/my_sub_package/nested_module.py
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/my_other_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/packaging_demo/states_info.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:01:03.841466 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 16:01:03.000000 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-18 16:01:03.000000 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:01:03.000000 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-18 16:01:03.000000 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 16:01:03.000000 packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:01:03.841466 packaging_demo_avr-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 16:00:59.000000 packaging_demo_avr-0.0.8/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    31246 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:30.817358 packaging_demo_avr-0.0.9/packaging_demo/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/cities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/colorized_demo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/packaging_demo/my_folder/
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_folder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2282 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_folder/another-cities.json
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_folder/my_nested_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/packaging_demo/my_folder/my_sub_package/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_folder/my_sub_package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_folder/my_sub_package/nested_module.py
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/my_other_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/packaging_demo/states_info.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    32643 2024-05-18 16:19:30.000000 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-18 16:19:30.000000 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 16:19:30.000000 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-05-18 16:19:30.000000 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-18 16:19:30.000000 packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 16:19:30.821358 packaging_demo_avr-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-18 16:19:22.000000 packaging_demo_avr-0.0.9/version.txt
```

### Comparing `packaging_demo_avr-0.0.8/PKG-INFO` & `packaging_demo_avr-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/avr2002/python-packaging
 Project-URL: Documentation, https://github.com/avr2002/python-packaging/blob/main/README.md
 Keywords: python,bash,makefile,pypi,ci-cd,setuptools,wheels,package-development,github-actions,pypi-package,pre-commit-hooks,pyproject-toml,gitactions-workflow,github-actions-enabled,pre-commit-ci,pre-commit-config
 Classifier: Programming Language :: Python :: 3
```

### Comparing `packaging_demo_avr-0.0.8/README.md` & `packaging_demo_avr-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.8/packaging_demo/cities.json` & `packaging_demo_avr-0.0.9/packaging_demo/cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.8/packaging_demo/my_folder/another-cities.json` & `packaging_demo_avr-0.0.9/packaging_demo/my_folder/another-cities.json`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.8/packaging_demo/states_info.py` & `packaging_demo_avr-0.0.9/packaging_demo/states_info.py`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/PKG-INFO` & `packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packaging-demo-avr
-Version: 0.0.8
+Version: 0.0.9
 Summary: Demo for Python Packaging
 Author-email: Amit Vikram Raj <avr13405@gmail.com>
 License: MIT
 Project-URL: Repository, https://github.com/avr2002/python-packaging
 Project-URL: Documentation, https://github.com/avr2002/python-packaging/blob/main/README.md
 Keywords: python,bash,makefile,pypi,ci-cd,setuptools,wheels,package-development,github-actions,pypi-package,pre-commit-hooks,pyproject-toml,gitactions-workflow,github-actions-enabled,pre-commit-ci,pre-commit-config
 Classifier: Programming Language :: Python :: 3
```

### Comparing `packaging_demo_avr-0.0.8/packaging_demo_avr.egg-info/SOURCES.txt` & `packaging_demo_avr-0.0.9/packaging_demo_avr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `packaging_demo_avr-0.0.8/pyproject.toml` & `packaging_demo_avr-0.0.9/pyproject.toml`

 * *Files identical despite different names*

