# Comparing `tmp/pyodide-build-0.26.0a4.tar.gz` & `tmp/pyodide_build-0.26.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyodide-build-0.26.0a4.tar", last modified: Thu Mar 14 11:06:34 2024, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pyodide-build-0.26.0a4.tar` & `pyodide_build-0.26.0a5.tar`

### file list

```diff
@@ -1,56 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.233253 pyodide-build-0.26.0a4/
--rw-r--r--   0 runner    (1001) docker     (127)    16725 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-14 11:06:34.233253 pyodide-build-0.26.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    21297 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/_f2c_fixes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11749 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/_py_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     3681 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/bash_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)    10467 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/build_env.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    31123 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/buildall.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    23861 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/buildpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10069 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     8893 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/build_recipes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/create_zipfile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1486 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/py_compile.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/skeleton.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/cli/xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (127)    11963 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/create_pypa_index.py
--rw-r--r--   0 runner    (1001) docker     (127)     4580 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/create_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     4292 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/install_xbuildenv.py
--rw-r--r--   0 runner    (1001) docker     (127)     7577 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     3850 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/logger.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8707 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/mkpkg.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/out_of_tree/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/out_of_tree/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/out_of_tree/build.py
--rw-r--r--   0 runner    (1001) docker     (127)    15500 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/out_of_tree/pypi.py
--rw-r--r--   0 runner    (1001) docker     (127)     8849 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/out_of_tree/venv.py
--rw-r--r--   0 runner    (1001) docker     (127)     9773 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/pypabuild.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    19544 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/pywasmcross.py
--rw-r--r--   0 runner    (1001) docker     (127)     4836 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/pyzip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/recipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/tools/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.225253 pyodide-build-0.26.0a4/pyodide_build/tools/cmake/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.225253 pyodide-build-0.26.0a4/pyodide_build/tools/cmake/Modules/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/tools/cmake/Modules/Platform/
--rw-r--r--   0 runner    (1001) docker     (127)     6189 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/tools/emscripten.meson.cross
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/tools/pyo3_config.ini
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.229253 pyodide-build-0.26.0a4/pyodide_build/vendor/
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyodide_build/vendor/_pypabuild.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 11:06:34.233253 pyodide-build-0.26.0a4/pyodide_build.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      300 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-03-14 11:06:34.000000 pyodide-build-0.26.0a4/pyodide_build.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2024-03-14 11:06:24.000000 pyodide-build-0.26.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 11:06:34.233253 pyodide-build-0.26.0a4/setup.cfg
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/__init__.py
+-rw-r--r--   0        0        0    21297 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/_f2c_fixes.py
+-rw-r--r--   0        0        0    11764 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/_py_compile.py
+-rw-r--r--   0        0        0     3693 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/bash_runner.py
+-rw-r--r--   0        0        0     8181 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/build_env.py
+-rwxr-xr-x   0        0        0    30967 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/buildall.py
+-rwxr-xr-x   0        0        0    24052 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/buildpkg.py
+-rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/common.py
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/config.py
+-rw-r--r--   0        0        0     2928 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/create_package_index.py
+-rw-r--r--   0        0        0     4580 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/create_xbuildenv.py
+-rw-r--r--   0        0        0     7273 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/io.py
+-rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/logger.py
+-rwxr-xr-x   0        0        0     8707 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/mkpkg.py
+-rw-r--r--   0        0        0     9904 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pypabuild.py
+-rwxr-xr-x   0        0        0    19753 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pywasmcross.py
+-rw-r--r--   0        0        0     4476 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/pyzip.py
+-rw-r--r--   0        0        0     3412 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/recipe.py
+-rw-r--r--   0        0        0    11605 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/xbuildenv.py
+-rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/xbuildenv_releases.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/__init__.py
+-rw-r--r--   0        0        0    10069 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/build.py
+-rw-r--r--   0        0        0     8879 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/build_recipes.py
+-rw-r--r--   0        0        0     1632 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/config.py
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/create_zipfile.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/py_compile.py
+-rw-r--r--   0        0        0     2316 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/skeleton.py
+-rw-r--r--   0        0        0      343 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/venv.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/cli/xbuildenv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/__init__.py
+-rw-r--r--   0        0        0     1422 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/build.py
+-rw-r--r--   0        0        0    15500 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/pypi.py
+-rw-r--r--   0        0        0     9604 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/out_of_tree/venv.py
+-rw-r--r--   0        0        0      363 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/emscripten.meson.cross
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/pyo3_config.ini
+-rw-r--r--   0        0        0     6189 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyodide_build/vendor/_pypabuild.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/.gitignore
+-rw-r--r--   0        0        0    16725 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/LICENSE
+-rw-r--r--   0        0        0      257 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/README.md
+-rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/pyproject.toml
+-rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pyodide_build-0.26.0a5/PKG-INFO
```

### Comparing `pyodide-build-0.26.0a4/LICENSE` & `pyodide_build-0.26.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/PKG-INFO` & `pyodide_build-0.26.0a5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,47 +1,48 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: pyodide-build
-Version: 0.26.0a4
+Version: 0.26.0a5
 Summary: "Tools for building Pyodide"
-Author: Pyodide developers
-License: MPL-2.0
 Project-URL: Homepage, https://github.com/pyodide/pyodide
 Project-URL: Bug Tracker, https://github.com/pyodide/pyodide/issues
 Project-URL: Documentation, https://pyodide.org/en/stable/
-Classifier: Programming Language :: Python :: 3
+Author: Pyodide developers
+License: MPL-2.0
+License-File: LICENSE
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.12
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyyaml
-Requires-Dist: ruamel.yaml
+Requires-Dist: auditwheel-emscripten~=0.0.9
+Requires-Dist: build~=1.2.0
+Requires-Dist: cmake>=3.24
+Requires-Dist: loky
 Requires-Dist: packaging
-Requires-Dist: wheel
-Requires-Dist: build>=1.0.0
-Requires-Dist: virtualenv
-Requires-Dist: pydantic<2,>=1.10.2
+Requires-Dist: pydantic<3,>=2
 Requires-Dist: pyodide-cli~=0.2.1
-Requires-Dist: cmake>=3.24
-Requires-Dist: unearth~=0.6
+Requires-Dist: pyodide-lock==0.1.0a6
+Requires-Dist: pyyaml
 Requires-Dist: requests
-Requires-Dist: types-requests
-Requires-Dist: typer
-Requires-Dist: auditwheel-emscripten~=0.0.9
-Requires-Dist: pyodide-lock==0.1.0a4
 Requires-Dist: resolvelib
 Requires-Dist: rich
-Requires-Dist: loky
-Provides-Extra: test
-Requires-Dist: pytest<8.0.0; extra == "test"
-Requires-Dist: pytest-pyodide==0.56.2; extra == "test"
-Requires-Dist: packaging; extra == "test"
+Requires-Dist: ruamel-yaml
+Requires-Dist: typer
+Requires-Dist: types-requests
+Requires-Dist: unearth~=0.6
+Requires-Dist: virtualenv
+Requires-Dist: wheel
 Provides-Extra: deploy
-Requires-Dist: boto3; extra == "deploy"
-Requires-Dist: moto; extra == "deploy"
+Requires-Dist: boto3; extra == 'deploy'
+Requires-Dist: moto; extra == 'deploy'
+Provides-Extra: test
+Requires-Dist: packaging; extra == 'test'
+Requires-Dist: pytest-httpserver; extra == 'test'
+Requires-Dist: pytest-pyodide==0.57.0; extra == 'test'
+Requires-Dist: pytest<8.0.0; extra == 'test'
+Description-Content-Type: text/markdown
 
 # pyodide-build
 
 Tools for building Pyodide.
 
 See [http://github.com/pyodide/pyodide](http://github.com/pyodide/pyodide) for
 more information.
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/_f2c_fixes.py` & `pyodide_build-0.26.0a5/pyodide_build/_f2c_fixes.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/_py_compile.py` & `pyodide_build-0.26.0a5/pyodide_build/_py_compile.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,17 +118,18 @@
         logger.debug(f"Running py-compile on {input_path} to {output_path}")
 
         if compression_level > 0:
             compression = zipfile.ZIP_DEFLATED
         else:
             compression = zipfile.ZIP_STORED
 
-        with zipfile.ZipFile(
-            input_path
-        ) as fh_zip_in, TemporaryDirectory() as temp_dir_str:
+        with (
+            zipfile.ZipFile(input_path) as fh_zip_in,
+            TemporaryDirectory() as temp_dir_str,
+        ):
             temp_dir = Path(temp_dir_str)
             output_path_tmp = temp_dir / output_name
             with zipfile.ZipFile(
                 output_path_tmp,
                 mode="w",
                 compression=compression,
                 compresslevel=compression_level,
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/bash_runner.py` & `pyodide_build-0.26.0a5/pyodide_build/bash_runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
 
 @contextmanager
 def get_bash_runner(
     extra_envs: dict[str, str],
 ) -> Iterator[BashRunnerWithSharedEnvironment]:
     pyodide_root = get_pyodide_root()
-    env = get_build_environment_vars()
+    env = get_build_environment_vars(pyodide_root)
     env.update(extra_envs)
 
     with BashRunnerWithSharedEnvironment(env=env) as b:
         # Working in-tree, add emscripten toolchain into PATH and set ccache
         if Path(pyodide_root, "pyodide_env.sh").exists():
             b.run(
                 f"source {pyodide_root}/pyodide_env.sh",
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/build_env.py` & `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/venv.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,356 +1,281 @@
-# This file contains functions for managing the Pyodide build environment.
-
-import dataclasses
-import functools
-import os
-import re
+import shutil
 import subprocess
-import tomllib
-from collections.abc import Iterator
-from contextlib import nullcontext, redirect_stdout
-from io import StringIO
+import sys
+import textwrap
 from pathlib import Path
+from typing import Any
 
-from packaging.tags import Tag, compatible_tags, cpython_tags
+from ..build_env import get_build_flag, get_pyodide_root, in_xbuildenv
+from ..common import exit_with_stdio
+from ..logger import logger
 
-from .common import exit_with_stdio, xbuildenv_dirname
-from .logger import logger
-from .recipe import load_all_recipes
-
-RUST_BUILD_PRELUDE = """
-rustup toolchain install ${RUST_TOOLCHAIN} && rustup default ${RUST_TOOLCHAIN}
-rustup target add wasm32-unknown-emscripten --toolchain ${RUST_TOOLCHAIN}
-"""
-
-
-BUILD_VARS: set[str] = {
-    "CARGO_BUILD_TARGET",
-    "CARGO_TARGET_WASM32_UNKNOWN_EMSCRIPTEN_LINKER",
-    "HOME",
-    "HOSTINSTALLDIR",
-    "HOSTSITEPACKAGES",
-    "NUMPY_LIB",
-    "PATH",
-    "PLATFORM_TRIPLET",
-    "PIP_CONSTRAINT",
-    "PYMAJOR",
-    "PYMICRO",
-    "PYMINOR",
-    "PYO3_CROSS_INCLUDE_DIR",
-    "PYO3_CROSS_LIB_DIR",
-    "PYODIDE_EMSCRIPTEN_VERSION",
-    "PYODIDE_JOBS",
-    "PYODIDE_PACKAGE_ABI",
-    "PYODIDE_ROOT",
-    "PYTHON_ARCHIVE_SHA256",
-    "PYTHON_ARCHIVE_URL",
-    "PYTHONINCLUDE",
-    "PYTHONPATH",
-    "PYVERSION",
-    "RUSTFLAGS",
-    "RUST_TOOLCHAIN",
-    "SIDE_MODULE_CFLAGS",
-    "SIDE_MODULE_CXXFLAGS",
-    "SIDE_MODULE_LDFLAGS",
-    "STDLIB_MODULE_CFLAGS",
-    "SYSCONFIGDATA_DIR",
-    "SYSCONFIG_NAME",
-    "TARGETINSTALLDIR",
-    "WASM_LIBRARY_DIR",
-    "CMAKE_TOOLCHAIN_FILE",
-    "PYO3_CONFIG_FILE",
-    "MESON_CROSS_FILE",
-    "PKG_CONFIG_LIBDIR",
-}
 
+def check_result(result: subprocess.CompletedProcess[str], msg: str) -> None:
+    """Abort if the process returns a nonzero error code"""
+    if result.returncode != 0:
+        logger.error(msg)
+        exit_with_stdio(result)
 
-@dataclasses.dataclass(eq=False, order=False, kw_only=True)
-class BuildArgs:
-    """
-    Common arguments for building a package.
-    """
 
-    pkgname: str = ""
-    cflags: str = ""
-    cxxflags: str = ""
-    ldflags: str = ""
-    target_install_dir: str = ""  # The path to the target Python installation
-    host_install_dir: str = ""  # Directory for installing built host packages.
-    builddir: str = ""  # The path to run pypa/build
+def dedent(s: str) -> str:
+    return textwrap.dedent(s).strip() + "\n"
 
 
-def init_environment(*, quiet: bool = False) -> None:
-    """
-    Initialize Pyodide build environment.
-    This function needs to be called before any other Pyodide build functions.
+def get_pyversion() -> str:
+    return f"{sys.version_info.major}.{sys.version_info.minor}"
 
-    Parameters
-    ----------
-    quiet
-        If True, do not print any messages
-    """
 
-    # Already initialized
-    if "PYODIDE_ROOT" in os.environ:
+def check_host_python_version(session: Any) -> None:
+    pyodide_version = session.interpreter.version.partition(" ")[0].split(".")[:2]
+    sys_version = [str(sys.version_info.major), str(sys.version_info.minor)]
+    if pyodide_version == sys_version:
         return
+    pyodide_version_fmt = ".".join(pyodide_version)
+    sys_version_fmt = ".".join(sys_version)
+    logger.stderr(
+        f"Expected host Python version to be {pyodide_version_fmt} but got version {sys_version_fmt}"
+    )
+    sys.exit(1)
 
-    root = search_pyodide_root(Path.cwd())
-    if not root:  # Not in Pyodide tree
-        root = _init_xbuild_env(quiet=quiet)
 
-    os.environ["PYODIDE_ROOT"] = str(root)
+def pyodide_dist_dir() -> Path:
+    return get_pyodide_root() / "dist"
 
 
-def _init_xbuild_env(*, quiet: bool = False) -> Path:
-    """
-    Initialize the build environment for out-of-tree builds.
+def create_pip_conf(venv_root: Path) -> None:
+    """Create pip.conf file in venv root
 
-    Parameters
-    ----------
-    quiet
-        If True, do not print any messages
-
-    Returns
-    -------
-        The path to the Pyodide root directory inside the xbuild environment
+    This file adds a few options that will always be used by pip install.
     """
-    from . import install_xbuildenv  # avoid circular import
-
-    # TODO: Do not hardcode the path
-    xbuildenv_path = Path(xbuildenv_dirname()).resolve()
-
-    context = redirect_stdout(StringIO()) if quiet else nullcontext()
-    with context:
-        return install_xbuildenv.install(xbuildenv_path, download=True)
-
+    if in_xbuildenv():
+        # In the xbuildenv, we don't have the packages locally. We will include
+        # in the xbuildenv a PEP 503 index for the vendored Pyodide packages
+        # https://peps.python.org/pep-0503/
+        repo = f'extra-index-url=file:{get_pyodide_root()/"package_index"}'
+    else:
+        # In the Pyodide development environment, the Pyodide dist directory
+        # should contain the needed wheels. find-links
+        repo = f"find-links={pyodide_dist_dir()}"
+
+    # Prevent attempts to install binary wheels from source.
+    # Maybe some day we can convince pip to invoke `pyodide build` as the build
+    # front end for wheels...
+    (venv_root / "pip.conf").write_text(
+        dedent(
+            f"""
+            [install]
+            only-binary=:all:
+            {repo}
+            """
+        )
+    )
 
-@functools.cache
-def get_pyodide_root() -> Path:
-    init_environment()
-    return Path(os.environ["PYODIDE_ROOT"])
 
+def get_pip_monkeypatch(venv_bin: Path) -> str:
+    """Monkey patch pip's environment to show info about Pyodide's environment.
 
-def search_pyodide_root(curdir: str | Path, *, max_depth: int = 10) -> Path | None:
+    The code returned is injected at the beginning of the pip script.
     """
-    Recursively search for the root of the Pyodide repository,
-    by looking for the pyproject.toml file in the parent directories
-    which contains [tool.pyodide] section.
-    """
-
-    # We want to include "curdir" in parent_dirs, so add a garbage suffix
-    parent_dirs = (Path(curdir) / "garbage").parents[:max_depth]
-
-    for base in parent_dirs:
-        pyproject_file = base / "pyproject.toml"
-
-        if not pyproject_file.is_file():
-            continue
-
-        try:
-            with pyproject_file.open("rb") as f:
-                configs = tomllib.load(f)
-        except tomllib.TOMLDecodeError as e:
-            raise ValueError(f"Could not parse {pyproject_file}.") from e
-
-        if "tool" in configs and "pyodide" in configs["tool"]:
-            return base
-
-    return None
-
-
-def in_xbuildenv() -> bool:
-    pyodide_root = get_pyodide_root()
-    return pyodide_root.name == "pyodide-root"
-
+    result = subprocess.run(
+        [
+            venv_bin / "python",
+            "-c",
+            dedent(
+                """
+                import os, sys, sysconfig, platform
+                print([
+                    os.name,
+                    sys.platform,
+                    sys.implementation._multiarch,
+                    sysconfig.get_platform()
+                ])
+                """
+            ),
+        ],
+        capture_output=True,
+        encoding="utf8",
+    )
+    check_result(result, "ERROR: failed to invoke Pyodide")
+    platform_data = result.stdout
+    sysconfigdata_dir = Path(get_build_flag("TARGETINSTALLDIR")) / "sysconfigdata"
+    return dedent(
+        """\
+        import os
+        import platform
+        import sys
+        """
+        # when pip installs an executable it uses sys.executable to create the
+        # shebang for the installed executable. The shebang for pip points to
+        # python-host but we want the shebang of the executable that we install
+        # to point to Pyodide python. We monkeypatch distlib.scripts.get_executable
+        # to return the value with the host suffix removed.
+        """
+        from pip._vendor.distlib import scripts
+        def get_executable():
+            return sys.executable.removesuffix("-host")
+
+        scripts.get_executable = get_executable
+
+        from pip._vendor.packaging import tags
+        orig_platform_tags = tags.platform_tags
+        """
+        # TODO: Remove the following monkeypatch when we merge and pull in
+        # https://github.com/pypa/packaging/pull/804
+        """
+        def _emscripten_platforms():
+            pyodide_abi_version = sysconfig.get_config_var("PYODIDE_ABI_VERSION")
+            if pyodide_abi_version:
+                yield f"pyodide_{pyodide_abi_version}_wasm32"
+            yield from tags._generic_platforms()
+
+        def platform_tags():
+            if platform.system() == "emscripten":
+                yield from _emscripten_platforms()
+                return
+            return orig_platform_tags()
+
+        tags.platform_tags = platform_tags
+        """
+        f"""
+        os_name, sys_platform, multiarch, host_platform = {platform_data}
+        os.name = os_name
+        orig_platform = sys.platform
+        sys.platform = sys_platform
+        sys.implementation._multiarch = multiarch
+        platform.system = lambda: sys_platform
+        platform.machine = lambda: "wasm32"
+        os.environ["_PYTHON_HOST_PLATFORM"] = host_platform
+        os.environ["_PYTHON_SYSCONFIGDATA_NAME"] = f'_sysconfigdata_{{sys.abiflags}}_{{sys.platform}}_{{sys.implementation._multiarch}}'
+        sys.path.append("{sysconfigdata_dir}")
+        import sysconfig
+        sysconfig.get_config_vars()
+        del os.environ["_PYTHON_SYSCONFIGDATA_NAME"]
+        sys.platform = orig_platform
+        """
+    )
 
-@functools.cache
-def get_build_environment_vars() -> dict[str, str]:
-    """
-    Get common environment variables for the in-tree and out-of-tree build.
-    """
-    env = _get_make_environment_vars().copy()
 
-    # Allow users to overwrite the build environment variables by setting
-    # host environment variables.
-    # TODO: Add modifiable configuration file instead.
-    # (https://github.com/pyodide/pyodide/pull/3737/files#r1161247201)
-    env.update({key: os.environ[key] for key in BUILD_VARS if key in os.environ})
-    env["PYODIDE"] = "1"
-
-    tools_dir = Path(__file__).parent / "tools"
-
-    if "CMAKE_TOOLCHAIN_FILE" not in env:
-        env["CMAKE_TOOLCHAIN_FILE"] = str(
-            tools_dir / "cmake/Modules/Platform/Emscripten.cmake"
+def create_pip_script(venv_bin):
+    """Create pip and write it into the virtualenv bin folder."""
+    # pip needs to run in the host Python not in Pyodide, so we'll use the host
+    # Python in the shebang. Use whichever Python was used to invoke
+    # pyodide venv.
+    host_python_path = venv_bin / f"python{get_pyversion()}-host"
+    host_python_path.symlink_to(sys.executable)
+    # in case someone needs a Python-version-agnostic way to refer to python-host
+    (venv_bin / "python-host").symlink_to(sys.executable)
+
+    (venv_bin / "pip").write_text(
+        # Other than the shebang and the monkey patch, this is exactly what
+        # normal pip looks like.
+        f"#!{host_python_path} -s\n"
+        + get_pip_monkeypatch(venv_bin)
+        + dedent(
+            """
+            import re
+            import sys
+            from pip._internal.cli.main import main
+            if __name__ == '__main__':
+                sys.argv[0] = re.sub(r'(-script\\.pyw|\\.exe)?$', '', sys.argv[0])
+                sys.exit(main())
+            """
         )
+    )
+    (venv_bin / "pip").chmod(0o777)
 
-    if "PYO3_CONFIG_FILE" not in env:
-        env["PYO3_CONFIG_FILE"] = str(tools_dir / "pyo3_config.ini")
-
-    if "MESON_CROSS_FILE" not in env:
-        env["MESON_CROSS_FILE"] = str(tools_dir / "emscripten.meson.cross")
-
-    hostsitepackages = env["HOSTSITEPACKAGES"]
-    pythonpath = [
-        hostsitepackages,
+    pyversion = get_pyversion()
+    other_pips = [
+        venv_bin / "pip3",
+        venv_bin / f"pip{pyversion}",
+        venv_bin / f"pip-{pyversion}",
     ]
-    env["PYTHONPATH"] = ":".join(pythonpath)
-
-    return env
 
+    for pip in other_pips:
+        pip.unlink()
+        pip.symlink_to(venv_bin / "pip")
+
+
+def create_pyodide_script(venv_bin: Path) -> None:
+    """Write pyodide cli script into the virtualenv bin folder"""
+    import os
+
+    # Temporarily restore us to the environment that 'pyodide venv' was
+    # invoked in
+    PATH = os.environ["PATH"]
+    PYODIDE_ROOT = os.environ["PYODIDE_ROOT"]
+
+    original_pyodide_cli = shutil.which("pyodide")
+    if original_pyodide_cli is None:
+        raise RuntimeError("ERROR: pyodide cli not found")
+
+    pyodide_path = venv_bin / "pyodide"
+    pyodide_path.write_text(
+        dedent(
+            f"""
+            #!/usr/bin/env bash
+            PATH="{PATH}:$PATH" PYODIDE_ROOT='{PYODIDE_ROOT}' exec {original_pyodide_cli} "$@"
+            """
+        )
+    )
+    pyodide_path.chmod(0o777)
 
-def _get_make_environment_vars(*, pyodide_root: Path | None = None) -> dict[str, str]:
-    """Load environment variables from Makefile.envs
 
-    This allows us to set all build vars in one place
+def install_stdlib(venv_bin: Path) -> None:
+    """Install micropip and all unvendored stdlib modules"""
+    # Micropip we could install with pip hypothetically, but because we use
+    # `--extra-index-url` it would install the pypi version which we don't want.
 
-    Parameters
-    ----------
-    pyodide_root
-        The root directory of the Pyodide repository. If None, this will be inferred.
-    """
-
-    PYODIDE_ROOT = get_pyodide_root() if pyodide_root is None else pyodide_root
-    environment = {}
+    # Other stuff we need to load with loadPackage
+    # TODO: Also load all shared libs.
+    to_load = ["micropip"]
     result = subprocess.run(
-        ["make", "-f", str(PYODIDE_ROOT / "Makefile.envs"), ".output_vars"],
+        [
+            venv_bin / "python",
+            "-c",
+            dedent(
+                f"""
+                from pyodide_js import loadPackage
+                from pyodide_js._api import lockfile_packages
+                from pyodide_js._api import lockfile_unvendored_stdlibs_and_test
+                shared_libs = [pkgname for (pkgname,pkg) in lockfile_packages.object_entries() if getattr(pkg, "shared_library", False)]
+
+                to_load = [*lockfile_unvendored_stdlibs_and_test, *shared_libs, *{to_load!r}]
+                loadPackage(to_load);
+                """
+            ),
+        ],
         capture_output=True,
-        text=True,
-        env={"PYODIDE_ROOT": str(PYODIDE_ROOT)},
+        encoding="utf8",
     )
+    check_result(result, "ERROR: failed to install unvendored stdlib modules")
 
-    if result.returncode != 0:
-        logger.error("ERROR: Failed to load environment variables from Makefile.envs")
-        exit_with_stdio(result)
-
-    for line in result.stdout.splitlines():
-        equalPos = line.find("=")
-        if equalPos != -1:
-            varname = line[0:equalPos]
-
-            if varname not in BUILD_VARS:
-                continue
-
-            value = line[equalPos + 1 :]
-            value = value.strip("'").strip()
-            environment[varname] = value
-    return environment
-
-
-def get_build_flag(name: str) -> str:
-    """
-    Get a value of a build flag.
-    """
-    build_vars = get_build_environment_vars()
-    if name not in build_vars:
-        raise ValueError(f"Unknown build flag: {name}")
-
-    return build_vars[name]
-
-
-def get_pyversion_major() -> str:
-    return get_build_flag("PYMAJOR")
-
-
-def get_pyversion_minor() -> str:
-    return get_build_flag("PYMINOR")
-
-
-def get_pyversion_major_minor() -> str:
-    return f"{get_pyversion_major()}.{get_pyversion_minor()}"
-
-
-def get_pyversion() -> str:
-    return f"python{get_pyversion_major_minor()}"
-
-
-def get_hostsitepackages() -> str:
-    return get_build_flag("HOSTSITEPACKAGES")
 
+def create_pyodide_venv(dest: Path) -> None:
+    """Create a Pyodide virtualenv and store it into dest"""
+    logger.info(f"Creating Pyodide virtualenv at {dest}")
+    from virtualenv import session_via_cli
 
-@functools.cache
-def get_unisolated_packages() -> list[str]:
-    PYODIDE_ROOT = get_pyodide_root()
-
-    unisolated_file = PYODIDE_ROOT / "unisolated.txt"
-    if unisolated_file.exists():
-        # in xbuild env, read from file
-        unisolated_packages = unisolated_file.read_text().splitlines()
-    else:
-        unisolated_packages = []
-        recipe_dir = PYODIDE_ROOT / "packages"
-        recipes = load_all_recipes(recipe_dir)
-        for name, config in recipes.items():
-            if config.build.cross_build_env:
-                unisolated_packages.append(name)
-
-    return unisolated_packages
-
-
-def platform() -> str:
-    emscripten_version = get_build_flag("PYODIDE_EMSCRIPTEN_VERSION")
-    version = emscripten_version.replace(".", "_")
-    return f"emscripten_{version}_wasm32"
-
-
-def pyodide_tags() -> Iterator[Tag]:
-    """
-    Returns the sequence of tag triples for the Pyodide interpreter.
-
-    The sequence is ordered in decreasing specificity.
-    """
-    PYMAJOR = get_pyversion_major()
-    PYMINOR = get_pyversion_minor()
-    PLATFORM = platform()
-    python_version = (int(PYMAJOR), int(PYMINOR))
-    yield from cpython_tags(platforms=[PLATFORM], python_version=python_version)
-    yield from compatible_tags(platforms=[PLATFORM], python_version=python_version)
-    # Following line can be removed once packaging 22.0 is released and we update to it.
-    yield Tag(interpreter=f"cp{PYMAJOR}{PYMINOR}", abi="none", platform="any")
+    if dest.exists():
+        logger.error(f"ERROR: dest directory '{dest}' already exists")
+        sys.exit(1)
 
+    interp_path = pyodide_dist_dir() / "python"
+    session = session_via_cli(["--no-wheel", "-p", str(interp_path), str(dest)])
+    check_host_python_version(session)
 
-def replace_so_abi_tags(wheel_dir: Path) -> None:
-    """Replace native abi tag with emscripten abi tag in .so file names"""
-    import sysconfig
-
-    build_soabi = sysconfig.get_config_var("SOABI")
-    assert build_soabi
-    ext_suffix = sysconfig.get_config_var("EXT_SUFFIX")
-    assert ext_suffix
-    build_triplet = "-".join(build_soabi.split("-")[2:])
-    host_triplet = get_build_flag("PLATFORM_TRIPLET")
-    for file in wheel_dir.glob(f"**/*{ext_suffix}"):
-        file.rename(file.with_name(file.name.replace(build_triplet, host_triplet)))
-
-
-def emscripten_version() -> str:
-    return get_build_flag("PYODIDE_EMSCRIPTEN_VERSION")
-
-
-def get_emscripten_version_info() -> str:
-    """Extracted for testing purposes."""
-    return subprocess.run(["emcc", "-v"], capture_output=True, encoding="utf8").stderr
-
-
-def check_emscripten_version() -> None:
-    needed_version = emscripten_version()
-    try:
-        version_info = get_emscripten_version_info()
-    except FileNotFoundError:
-        raise RuntimeError(
-            f"No Emscripten compiler found. Need Emscripten version {needed_version}"
-        ) from None
-    installed_version = None
     try:
-        for x in reversed(version_info.partition("\n")[0].split(" ")):
-            if re.match(r"[0-9]+\.[0-9]+\.[0-9]+", x):
-                installed_version = x
-                break
-    except Exception:
-        raise RuntimeError("Failed to determine Emscripten version.") from None
-    if installed_version is None:
-        raise RuntimeError("Failed to determine Emscripten version.")
-    if installed_version != needed_version:
-        raise RuntimeError(
-            f"Incorrect Emscripten version {installed_version}. Need Emscripten version {needed_version}"
-        )
+        session.run()
+        venv_root = Path(session.creator.dest).absolute()
+        venv_bin = venv_root / "bin"
+
+        logger.info("... Configuring virtualenv")
+        create_pip_conf(venv_root)
+        create_pip_script(venv_bin)
+        create_pyodide_script(venv_bin)
+        logger.info("... Installing standard library")
+        install_stdlib(venv_bin)
+    except (Exception, KeyboardInterrupt, SystemExit):
+        shutil.rmtree(session.creator.dest)
+        raise
+
+    logger.success("Successfully created Pyodide virtual environment!")
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/buildall.py` & `pyodide_build-0.26.0a5/pyodide_build/buildall.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return None
 
 
 @dataclasses.dataclass
 class Package(BasePackage):
     def __init__(self, pkgdir: Path, config: MetaConfig):
         self.pkgdir = pkgdir
-        self.meta = config.copy(deep=True)
+        self.meta = config.model_copy(deep=True)
 
         self.name = self.meta.package.name
         self.version = self.meta.package.version
         self.disabled = self.meta.package.disabled
         self.package_type = self.meta.build.package_type
 
         assert self.name == pkgdir.name, f"{self.name} != {pkgdir.name}"
@@ -768,24 +768,22 @@
 
 
 def generate_lockfile(
     output_dir: Path, pkg_map: dict[str, BasePackage]
 ) -> PyodideLockSpec:
     """Generate the package.json file"""
 
-    from . import __version__
-
     # Build package.json data.
     [platform, _, arch] = build_env.platform().rpartition("_")
     info = {
         "arch": arch,
         "platform": platform,
-        # This assumes that pyodide-build version == pyodide version.
-        "version": __version__,
+        "version": build_env.get_build_flag("PYODIDE_VERSION"),
         "python": sys.version.partition(" ")[0],
+        "abi_version": build_env.get_build_flag("PYODIDE_ABI_VERSION"),
     }
     packages = generate_packagedata(output_dir, pkg_map)
     lock_spec = PyodideLockSpec(info=info, packages=packages)
     lock_spec.check_wheel_filenames()
     return lock_spec
 
 
@@ -871,15 +869,15 @@
     output_dir: Path,
     compression_level: int = 6,
     metadata_files: bool = False,
 ) -> None:
     """
     Install packages into the output directory.
     - copies build artifacts (wheel, zip, ...) to the output directory
-    - create pyodide_lock.json
+    - create pyodide-lock.json
 
 
     pkg_map
         package map created from build_packages
 
     output_dir
         output directory to install packages into
@@ -901,19 +899,19 @@
     package_data = generate_lockfile(output_dir, pkg_map)
     package_data.to_json(lockfile_path)
 
 
 def set_default_build_args(build_args: BuildArgs) -> BuildArgs:
     args = dataclasses.replace(build_args)
 
-    if args.cflags is None:
-        args.cflags = build_env.get_build_flag("SIDE_MODULE_CFLAGS")  # type: ignore[unreachable]
-    if args.cxxflags is None:
-        args.cxxflags = build_env.get_build_flag("SIDE_MODULE_CXXFLAGS")  # type: ignore[unreachable]
-    if args.ldflags is None:
-        args.ldflags = build_env.get_build_flag("SIDE_MODULE_LDFLAGS")  # type: ignore[unreachable]
-    if args.target_install_dir is None:
-        args.target_install_dir = build_env.get_build_flag("TARGETINSTALLDIR")  # type: ignore[unreachable]
-    if args.host_install_dir is None:
-        args.host_install_dir = build_env.get_build_flag("HOSTINSTALLDIR")  # type: ignore[unreachable]
+    if not args.cflags:
+        args.cflags = build_env.get_build_flag("SIDE_MODULE_CFLAGS")
+    if not args.cxxflags:
+        args.cxxflags = build_env.get_build_flag("SIDE_MODULE_CXXFLAGS")
+    if not args.ldflags:
+        args.ldflags = build_env.get_build_flag("SIDE_MODULE_LDFLAGS")
+    if not args.target_install_dir:
+        args.target_install_dir = build_env.get_build_flag("TARGETINSTALLDIR")
+    if not args.host_install_dir:
+        args.host_install_dir = build_env.get_build_flag("HOSTINSTALLDIR")
 
     return args
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/buildpkg.py` & `pyodide_build-0.26.0a5/pyodide_build/buildpkg.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 #!/usr/bin/env python3
 
 """
 Builds a Pyodide package.
 """
 
-import cgi
 import fnmatch
 import os
+import re
 import shutil
 import subprocess
 import sys
-import urllib
 from collections.abc import Iterator
 from datetime import datetime
 from pathlib import Path
 from typing import Any, cast
-from urllib import request
+
+import requests
 
 from . import common, pypabuild
 from .bash_runner import BashRunnerWithSharedEnvironment, get_bash_runner
 from .build_env import (
     RUST_BUILD_PRELUDE,
     BuildArgs,
     get_build_environment_vars,
+    get_pyodide_root,
     pyodide_tags,
     replace_so_abi_tags,
+    wheel_platform,
 )
 from .common import (
     _environment_substitute_str,
     _get_sha256_checksum,
     chdir,
     exit_with_stdio,
     find_matching_wheels,
     make_zip_archive,
     modify_wheel,
+    retag_wheel,
 )
 from .io import MetaConfig, _SourceSpec
 from .logger import logger
 
 
 def _make_whlfile(
     *args: Any, owner: int | None = None, group: int | None = None, **kwargs: Any
@@ -162,17 +165,18 @@
 
         self._redirect_stdout_stderr_to_logfile()
 
         if not self.continue_:
             self._prepare_source()
             self._patch()
 
-        with chdir(self.pkg_root), get_bash_runner(
-            self._get_helper_vars()
-        ) as bash_runner:
+        with (
+            chdir(self.pkg_root),
+            get_bash_runner(self._get_helper_vars()) as bash_runner,
+        ):
             if self.recipe.is_rust_package():
                 bash_runner.run(
                     RUST_BUILD_PRELUDE,
                     script_name="rust build prelude",
                     cwd=self.src_extract_dir,
                 )
 
@@ -289,45 +293,45 @@
         self.src_dist_dir.mkdir(parents=True, exist_ok=True)
 
     def _download_and_extract(self) -> None:
         """
         Download the source from specified in the package metadata,
         then checksum it, then extract the archive into the build directory.
         """
-
-        build_env = get_build_environment_vars()
+        build_env = get_build_environment_vars(get_pyodide_root())
         url = cast(str, self.source_metadata.url)  # we know it's not None
         url = _environment_substitute_str(url, build_env)
 
         max_retry = 3
         for retry_cnt in range(max_retry):
             try:
-                response = request.urlopen(url)
-            except urllib.error.URLError as e:
+                response = requests.get(url)
+                response.raise_for_status()
+            except requests.HTTPError as e:
                 if retry_cnt == max_retry - 1:
                     raise RuntimeError(
                         f"Failed to download {url} after {max_retry} trials"
                     ) from e
 
                 continue
 
             break
 
-        # TODO: replace cgi with something else (will be removed in Python 3.13)
-        _, parameters = cgi.parse_header(
-            response.headers.get("Content-Disposition", "")
-        )
-        if "filename" in parameters:
-            tarballname = parameters["filename"]
-        else:
-            tarballname = Path(response.geturl()).name
-
         self.build_dir.mkdir(parents=True, exist_ok=True)
+
+        tarballname = url.split("/")[-1]
+        if "Content-Disposition" in response.headers:
+            filenames = re.findall(
+                "filename=(.+)", response.headers["Content-Disposition"]
+            )
+            if filenames:
+                tarballname = filenames[0]
+
         tarballpath = self.build_dir / tarballname
-        tarballpath.write_bytes(response.read())
+        tarballpath.write_bytes(response.content)
 
         checksum = self.source_metadata.sha256
         if checksum is not None:
             try:
                 checksum = _environment_substitute_str(checksum, build_env)
                 check_checksum(tarballpath, checksum)
             except Exception:
@@ -417,14 +421,18 @@
             self.src_dist_dir.glob("*.whl"), pyodide_tags()
         )
         if rest:
             raise Exception(
                 f"Unexpected number of wheels {len(rest) + 1} when building {self.name}"
             )
 
+        if "emscripten" in wheel.name:
+            # Retag platformed wheels to pyodide
+            wheel = retag_wheel(wheel, wheel_platform())
+
         logger.info(f"Unpacking wheel to {str(wheel)}")
 
         name, ver, _ = wheel.name.split("-", 2)
 
         with modify_wheel(wheel) as wheel_dir:
             # update so abi tags after build is complete but before running post script
             # to maximize sanity.
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/build.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/build.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/build_recipes.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/build_recipes.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,28 +63,28 @@
     build_dir: str = typer.Option(
         None,
         envvar="PYODIDE_RECIPE_BUILD_DIR",
         help="The directory where build directories for packages are created. "
         "Default: recipe_dir.",
     ),
     cflags: str = typer.Option(
-        None, help="Extra compiling flags. Default: SIDE_MODULE_CFLAGS"
+        "", help="Extra compiling flags. Default: SIDE_MODULE_CFLAGS"
     ),
     cxxflags: str = typer.Option(
-        None, help="Extra compiling flags. Default: SIDE_MODULE_CXXFLAGS"
+        "", help="Extra compiling flags. Default: SIDE_MODULE_CXXFLAGS"
     ),
     ldflags: str = typer.Option(
-        None, help="Extra linking flags. Default: SIDE_MODULE_LDFLAGS"
+        "", help="Extra linking flags. Default: SIDE_MODULE_LDFLAGS"
     ),
     target_install_dir: str = typer.Option(
-        None,
+        "",
         help="The path to the target Python installation. Default: TARGETINSTALLDIR",
     ),
     host_install_dir: str = typer.Option(
-        None,
+        "",
         help="Directory for installing built host packages. Default: HOSTINSTALLDIR",
     ),
     force_rebuild: bool = typer.Option(
         False,
         help="Force rebuild of all packages regardless of whether they appear to have been updated",
     ),
     continue_: bool = typer.Option(
@@ -174,19 +174,19 @@
     cxxflags: str = typer.Option(
         None, help="Extra compiling flags. Default: SIDE_MODULE_CXXFLAGS"
     ),
     ldflags: str = typer.Option(
         None, help="Extra linking flags. Default: SIDE_MODULE_LDFLAGS"
     ),
     target_install_dir: str = typer.Option(
-        None,
+        "",
         help="The path to the target Python installation. Default: TARGETINSTALLDIR",
     ),
     host_install_dir: str = typer.Option(
-        None,
+        "",
         help="Directory for installing built host packages. Default: HOSTINSTALLDIR",
     ),
     log_dir: str = typer.Option(None, help="Directory to place log files"),
     force_rebuild: bool = typer.Option(
         False,
         help="Force rebuild of all packages regardless of whether they appear to have been updated",
     ),
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/config.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/config.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
 
-from ..build_env import get_build_environment_vars, init_environment
+from ..build_env import get_build_environment_vars, get_pyodide_root, init_environment
 
 app = typer.Typer(help="Manage config variables used in pyodide")
 
 
 # A dictionary of config variables {key: env_var_in_makefile}
 PYODIDE_CONFIGS = {
     "emscripten_version": "PYODIDE_EMSCRIPTEN_VERSION",
@@ -24,15 +24,15 @@
 def callback() -> None:
     return
 
 
 def _get_configs() -> dict[str, str]:
     init_environment(quiet=True)
 
-    configs: dict[str, str] = get_build_environment_vars()
+    configs: dict[str, str] = get_build_environment_vars(get_pyodide_root())
 
     configs_filtered = {k: configs[v] for k, v in PYODIDE_CONFIGS.items()}
     return configs_filtered
 
 
 @app.command("list")
 def list_config():
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/create_zipfile.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/create_zipfile.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,52 @@
+import re
 from pathlib import Path
 
 import typer
 
 from ..pyzip import create_zipfile
 
 
 def main(
     libdir: list[Path] = typer.Argument(
         ...,
         help="List of paths to the directory containing the Python standard library or extra packages.",
     ),
+    exclude: str = typer.Option(
+        "",
+        help="List of files to exclude from the zip file. Defaults to no files.",
+    ),
+    stub: str = typer.Option(
+        "",
+        help="List of files that are replaced by JS implementations. Defaults to no files.",
+    ),
     pycompile: bool = typer.Option(
         False, help="Whether to compile the .py files into .pyc."
     ),
     output: Path = typer.Option(
         "python.zip", help="Path to the output zip file. Defaults to python.zip."
     ),
     compression_level: int = typer.Option(
         6, help="Compression level to use for the created zip file"
     ),
 ) -> None:
     """
     Bundle Python standard libraries into a zip file.
     """
+
+    # Convert the comma / space separated strings to lists
+    excludes = [
+        item.strip() for item in re.split(r",|\s", exclude) if item.strip() != ""
+    ]
+    stubs = [item.strip() for item in re.split(r",|\s", stub) if item.strip() != ""]
+
     create_zipfile(
         libdir,
+        excludes,
+        stubs,
         output,
         pycompile=pycompile,
         filterfunc=None,
         compression_level=compression_level,
     )
     typer.echo(f"Zip file created at {output.resolve()}")
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/py_compile.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/py_compile.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/cli/skeleton.py` & `pyodide_build-0.26.0a5/pyodide_build/cli/skeleton.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/common.py` & `pyodide_build-0.26.0a5/pyodide_build/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,15 +103,17 @@
             f"WARNING: failed to parse top level import name from {whlfile}."
         )
         return None
 
     return top_level_imports
 
 
-def _environment_substitute_str(string: str, env: dict[str, str] | None = None) -> str:
+def _environment_substitute_str(
+    string: str, env: Mapping[str, str] | None = None
+) -> str:
     """
     Substitute $(VAR) in string with the value of the environment variable VAR.
 
     Parameters
     ----------
     string
         A string
@@ -240,17 +242,23 @@
         compression = zipfile.ZIP_DEFLATED
     else:
         compression = zipfile.ZIP_STORED
 
     with TemporaryDirectory() as temp_dir:
         input_path = Path(temp_dir) / archive_path.name
         shutil.move(archive_path, input_path)
-        with zipfile.ZipFile(input_path) as fh_zip_in, zipfile.ZipFile(
-            archive_path, "w", compression=compression, compresslevel=compression_level
-        ) as fh_zip_out:
+        with (
+            zipfile.ZipFile(input_path) as fh_zip_in,
+            zipfile.ZipFile(
+                archive_path,
+                "w",
+                compression=compression,
+                compresslevel=compression_level,
+            ) as fh_zip_out,
+        ):
             for name in fh_zip_in.namelist():
                 fh_zip_out.writestr(name, fh_zip_in.read(name))
 
 
 def _get_sha256_checksum(archive: Path) -> str:
     """Compute the sha256 checksum of a file
 
@@ -318,14 +326,36 @@
         wheel_dir_name = f"{name}-{ver}"
         wheel_dir = Path(temp_dir) / wheel_dir_name
         yield wheel_dir
         wheel.unlink()
         pack_wheel(wheel_dir, wheel.parent)
 
 
+def retag_wheel(wheel_path: Path, platform: str) -> Path:
+    result = subprocess.run(
+        [
+            sys.executable,
+            "-m",
+            "wheel",
+            "tags",
+            wheel_path,
+            "--platform-tag",
+            platform,
+            "--remove",
+        ],
+        check=False,
+        encoding="utf-8",
+        capture_output=True,
+    )
+    if result.returncode != 0:
+        logger.error(f"ERROR: Retagging wheel {wheel_path} to {platform} failed")
+        exit_with_stdio(result)
+    return wheel_path.parent / result.stdout.strip()
+
+
 def extract_wheel_metadata_file(wheel_path: Path, output_path: Path) -> None:
     """Extracts the METADATA file from the given wheel and writes it to the
     output path.
 
     Raises a RuntimeError if the METADATA file does not exist.
 
     For a wheel called "NAME-VERSION-...", the METADATA file is expected to be
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/create_xbuildenv.py` & `pyodide_build-0.26.0a5/pyodide_build/create_xbuildenv.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/io.py` & `pyodide_build-0.26.0a5/pyodide_build/io.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,82 +1,76 @@
 from pathlib import Path
-from typing import Any, Literal
+from typing import Literal, Self
 
 import pydantic
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 
 class _PackageSpec(BaseModel):
     name: str
     version: str
     top_level: list[str] = Field([], alias="top-level")
     tag: list[str] = Field([])
     disabled: bool = Field(False, alias="_disabled")
-
-    class Config:
-        extra = pydantic.Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class _SourceSpec(BaseModel):
     url: str | None = None
     extract_dir: str | None = None
     path: Path | None = None
     sha256: str | None = None
     patches: list[str] = []
     extras: list[tuple[str, str]] = []
+    model_config = ConfigDict(extra="forbid")
 
-    class Config:
-        extra = pydantic.Extra.forbid
-
-    @pydantic.root_validator
-    def _check_url_has_hash(cls, values: dict[str, Any]) -> dict[str, Any]:
-        if values["url"] is not None and values["sha256"] is None:
+    @pydantic.model_validator(mode="after")
+    def _check_url_has_hash(self) -> Self:
+        if self.url is not None and self.sha256 is None:
             raise ValueError(
                 "If source is downloaded from url, it must have a 'source/sha256' hash."
             )
-        return values
 
-    @pydantic.root_validator
-    def _check_in_tree_url(cls, values: dict[str, Any]) -> dict[str, Any]:
-        in_tree = values["path"] is not None
-        from_url = values["url"] is not None
+        return self
+
+    @pydantic.model_validator(mode="after")
+    def _check_in_tree_url(self) -> Self:
+        in_tree = self.path is not None
+        from_url = self.url is not None
 
         # cpython_modules is a special case, it is not in the tree
         # TODO: just copy the file into the tree?
         # if not (in_tree or from_url):
         #     raise ValueError("Source section should have a 'url' or 'path' key")
 
         if in_tree and from_url:
             raise ValueError(
                 "Source section should not have both a 'url' and a 'path' key"
             )
-        return values
 
-    @pydantic.root_validator
-    def _check_patches_extra(cls, values: dict[str, Any]) -> dict[str, Any]:
-        patches = values["patches"]
-        extras = values["extras"]
-        in_tree = values["path"] is not None
-        from_url = values["url"] is not None
+        return self
 
-        url_is_wheel = from_url and values["url"].endswith(".whl")
+    @pydantic.model_validator(mode="after")
+    def _check_patches_extra(self) -> Self:
+        in_tree = self.path is not None
+        url_is_wheel = self.url and self.url.endswith(".whl")
 
-        if in_tree and (patches or extras):
+        if in_tree and (self.patches or self.extras):
             raise ValueError(
                 "If source is in tree, 'source/patches' and 'source/extras' keys "
                 "are not allowed"
             )
 
-        if url_is_wheel and (patches or extras):
+        if url_is_wheel and (self.patches or self.extras):
             raise ValueError(
                 "If source is a wheel, 'source/patches' and 'source/extras' "
                 "keys are not allowed"
             )
 
-        return values
+        return self
 
 
 _ExportTypes = Literal["pyinit", "requested", "whole_archive"]
 _BuildSpecExports = _ExportTypes | list[str]
 _BuildSpecTypes = Literal[
     "package", "static_library", "shared_library", "cpython_module"
 ]
@@ -93,84 +87,75 @@
     script: str | None = None
     post: str | None = None
     unvendor_tests: bool = Field(True, alias="unvendor-tests")
     retain_test_patterns: list[str] = Field([], alias="_retain-test-patterns")
     vendor_sharedlib: bool = Field(False, alias="vendor-sharedlib")
     cross_build_env: bool = Field(False, alias="cross-build-env")
     cross_build_files: list[str] = Field([], alias="cross-build-files")
+    model_config = ConfigDict(extra="forbid")
 
-    class Config:
-        extra = pydantic.Extra.forbid
-
-    @pydantic.root_validator
-    def _check_config(cls, values: dict[str, Any]) -> dict[str, Any]:
-        static_library = values["package_type"] == "static_library"
-        shared_library = values["package_type"] == "shared_library"
-        cpython_module = values["package_type"] == "cpython_module"
+    @pydantic.model_validator(mode="after")
+    def _check_config(self) -> Self:
+        static_library = self.package_type == "static_library"
+        shared_library = self.package_type == "shared_library"
+        cpython_module = self.package_type == "cpython_module"
 
         if not (static_library or shared_library or cpython_module):
-            return values
+            return self
 
         allowed_keys = {
             "package_type",
             "script",
             "exports",
             "unvendor_tests",
         }
 
-        typ = values["package_type"]
-        for key, val in values.items():
-            if val and key not in allowed_keys:
+        typ = self.package_type
+        for key in self.model_fields_set:
+            if key not in allowed_keys:
                 raise ValueError(
                     f"If building a {typ}, 'build/{key}' key is not allowed."
                 )
-        return values
+
+        return self
 
 
 class _RequirementsSpec(BaseModel):
     run: list[str] = []
     host: list[str] = []
     executable: list[str] = []
-
-    class Config:
-        extra = pydantic.Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class _TestSpec(BaseModel):
     imports: list[str] = []
-
-    class Config:
-        extra = pydantic.Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class _AboutSpec(BaseModel):
     home: str | None = None
     PyPI: str | None = None
     summary: str | None = None
     license: str | None = None
-
-    class Config:
-        extra = pydantic.Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
 
 class _ExtraSpec(BaseModel):
     recipe_maintainers: list[str] = Field([], alias="recipe-maintainers")
 
 
 class MetaConfig(BaseModel):
     package: _PackageSpec
     source: _SourceSpec = _SourceSpec()
     build: _BuildSpec = _BuildSpec()
     requirements: _RequirementsSpec = _RequirementsSpec()
     test: _TestSpec = _TestSpec()
     about: _AboutSpec = _AboutSpec()
     extra: _ExtraSpec = _ExtraSpec()
-
-    class Config:
-        extra = pydantic.Extra.forbid
+    model_config = ConfigDict(extra="forbid")
 
     @classmethod
     def from_yaml(cls, path: Path) -> "MetaConfig":
         """Load the meta.yaml from a path
 
         Parameters
         ----------
@@ -194,26 +179,26 @@
         ----------
         path
             path to the meta.yaml file
         """
         import yaml
 
         with open(path, "w") as f:
-            yaml.dump(self.dict(by_alias=True, exclude_unset=True), f)
+            yaml.dump(self.model_dump(by_alias=True, exclude_unset=True), f)
 
-    @pydantic.root_validator
-    def _check_wheel_host_requirements(cls, values: dict[str, Any]) -> dict[str, Any]:
+    @pydantic.model_validator(mode="after")
+    def _check_wheel_host_requirements(self) -> Self:
         """Check that if sources is a wheel it shouldn't have host dependencies."""
-        if "source" not in values:
+        if self.source.path is None and self.source.url is None:
             raise ValueError(
                 'either "path" or "url" must be provided in the "source" section'
             )
 
-        source_url = values["source"].url
-        requirements_host = values["requirements"].host
+        source_url = self.source.url
+        requirements_host = self.requirements.host
 
         if source_url is not None and source_url.endswith(".whl"):
             if len(requirements_host):
                 raise ValueError(
                     f"When source -> url is a wheel ({source_url}) the package cannot have host "
                     f"dependencies. Found {requirements_host}"
                 )
@@ -224,20 +209,21 @@
                 # Note here names are with "_", after alias conversion
                 "cross_build_env",
                 "cross_build_files",
                 "exports",
                 "unvendor_tests",
                 "package_type",
             }
-            for key, val in values["build"].dict().items():
-                if val and key not in allowed_keys:
+            for key in self.build.model_fields_set:
+                if key not in allowed_keys:
                     raise ValueError(
                         f"If source is a wheel, 'build/{key}' key is not allowed"
                     )
-        return values
+
+        return self
 
     def is_rust_package(self) -> bool:
         """
         Check if a package requires rust toolchain to build.
         """
         return any(
             q in self.requirements.executable for q in ("rustc", "cargo", "rustup")
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/logger.py` & `pyodide_build-0.26.0a5/pyodide_build/logger.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/mkpkg.py` & `pyodide_build-0.26.0a5/pyodide_build/mkpkg.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/out_of_tree/build.py` & `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/build.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 from pathlib import Path
 
 from build import ConfigSettingsType
 
 from .. import build_env, common, pypabuild
+from ..build_env import get_pyodide_root
 from ..io import _BuildSpecExports
 
 
 def run(
     srcdir: Path,
     outdir: Path,
     exports: _BuildSpecExports,
@@ -20,15 +21,15 @@
     cxxflags += f" {os.environ.get('CXXFLAGS', '')}"
     ldflags = build_env.get_build_flag("SIDE_MODULE_LDFLAGS")
     ldflags += f" {os.environ.get('LDFLAGS', '')}"
     target_install_dir = os.environ.get(
         "TARGETINSTALLDIR", build_env.get_build_flag("TARGETINSTALLDIR")
     )
     env = os.environ.copy()
-    env.update(build_env.get_build_environment_vars())
+    env.update(build_env.get_build_environment_vars(get_pyodide_root()))
 
     build_env_ctx = pypabuild.get_build_env(
         env=env,
         pkgname="",
         cflags=cflags,
         cxxflags=cxxflags,
         ldflags=ldflags,
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/out_of_tree/pypi.py` & `pyodide_build-0.26.0a5/pyodide_build/out_of_tree/pypi.py`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/pypabuild.py` & `pyodide_build-0.26.0a5/pyodide_build/pypabuild.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import sys
 import traceback
 from collections.abc import Callable, Iterator, Mapping, Sequence
 from contextlib import contextmanager
 from itertools import chain
 from pathlib import Path
 from tempfile import TemporaryDirectory
+from typing import Literal, cast
 
 from build import BuildBackendException, ConfigSettingsType
 from build.env import DefaultIsolatedEnv
 from packaging.requirements import Requirement
 
 from . import common, pywasmcross
 from .build_env import (
@@ -52,15 +53,15 @@
     "strip": "STRIP",
     "gfortran": "FC",  # https://mesonbuild.com/Reference-tables.html#compiler-and-linker-selection-variables
 }
 
 
 def _gen_runner(
     cross_build_env: Mapping[str, str],
-    isolated_build_env: DefaultIsolatedEnv,
+    isolated_build_env: _DefaultIsolatedEnv,
 ) -> Callable[[Sequence[str], str | None, Mapping[str, str] | None], None]:
     """
     This returns a slightly modified version of default subprocess runner that pypa/build uses.
     pypa/build prepends the virtual environment's bin directory to the PATH environment variable.
     This is problematic because it shadows the pywasmcross compiler wrappers for cmake, meson, etc.
 
     This function prepends the compiler wrapper directory to the PATH again so that our compiler wrappers
@@ -77,15 +78,15 @@
     def _runner(cmd, cwd=None, extra_environ=None):
         env = os.environ.copy()
         if extra_environ:
             env.update(extra_environ)
 
         # Some build dependencies like cmake, meson installs binaries to this directory
         # and we should add it to the PATH so that they can be found.
-        env["BUILD_ENV_SCRIPTS_DIR"] = isolated_build_env._scripts_dir
+        env["BUILD_ENV_SCRIPTS_DIR"] = isolated_build_env.scripts_dir
         env["PATH"] = f"{cross_build_env['COMPILER_WRAPPER_DIR']}:{env['PATH']}"
         # For debugging: Uncomment the following line to print the build command
         # print("Build backend call:", " ".join(str(x) for x in cmd), file=sys.stderr)
         sp.check_call(cmd, cwd=cwd, env=env)
 
     return _runner
 
@@ -131,22 +132,23 @@
     )
 
 
 def _build_in_isolated_env(
     build_env: Mapping[str, str],
     srcdir: Path,
     outdir: str,
-    distribution: str,
+    distribution: Literal["sdist", "wheel"],
     config_settings: ConfigSettingsType,
 ) -> str:
     # For debugging: The following line disables removal of the isolated venv.
     # It will be left in the /tmp folder and can be inspected or entered as
     # needed.
     # _DefaultIsolatedEnv.__exit__ = lambda *args: None
     with _DefaultIsolatedEnv() as env:
+        env = cast(_DefaultIsolatedEnv, env)
         builder = _ProjectBuilder.from_isolated_env(
             env,
             srcdir,
             runner=_gen_runner(build_env, env),
         )
 
         # first install the build dependencies
@@ -167,15 +169,19 @@
             if not installed_requires_for_build:
                 build_reqs = builder.get_requires_for_build(
                     distribution,
                     config_settings,
                 )
                 install_reqs(env, build_reqs)
 
-            return builder.build(distribution, outdir, config_settings)
+            return builder.build(
+                distribution,
+                outdir,
+                config_settings,
+            )
 
 
 def parse_backend_flags(backend_flags: str | list[str]) -> ConfigSettingsType:
     config_settings: dict[str, str | list[str]] = {}
 
     if isinstance(backend_flags, str):
         backend_flags = backend_flags.split()
@@ -282,19 +288,18 @@
 
 def build(
     srcdir: Path,
     outdir: Path,
     build_env: Mapping[str, str],
     config_settings: ConfigSettingsType,
 ) -> str:
-    distribution = "wheel"
     try:
         with _handle_build_error():
             built = _build_in_isolated_env(
-                build_env, srcdir, str(outdir), distribution, config_settings
+                build_env, srcdir, str(outdir), "wheel", config_settings
             )
             print("{bold}{green}Successfully built {}{reset}".format(built, **_STYLES))
             return built
     except Exception as e:  # pragma: no cover
         tb = traceback.format_exc().strip("\n")
         print("\n{dim}{}{reset}\n".format(tb, **_STYLES))
         _error(str(e))
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/pywasmcross.py` & `pyodide_build-0.26.0a5/pyodide_build/pywasmcross.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 Python has never had a proper cross-compilation story. This is a hack, which
 miraculously works, to get around that.
 The gist is we compile the package replacing calls to the compiler and linker
 with wrappers that adjusting include paths and flags as necessary for
 cross-compiling and then pass the command long to emscripten.
 """
+
 import json
 import os
 import sys
 from pathlib import Path
 
 from __main__ import __file__ as INVOKED_PATH_STR
 
@@ -422,16 +423,24 @@
     if exports == "whole_archive":
         return
     yield "-sSIDE_MODULE=2"
     if isinstance(exports, str):
         export_list = calculate_exports(line, exports == "requested")
     else:
         export_list = exports
+
     prefixed_exports = ["_" + x for x in export_list]
-    yield f"-sEXPORTED_FUNCTIONS={prefixed_exports!r}"
+
+    import tempfile
+
+    with tempfile.NamedTemporaryFile(mode="w", delete=False) as f:
+        # Use a response file to avoid command line length limits
+        f.write(json.dumps(prefixed_exports))
+
+    yield f"-sEXPORTED_FUNCTIONS=@{f.name}"
 
 
 def handle_command_generate_args(  # noqa: C901
     line: list[str], build_args: CrossCompileArgs
 ) -> list[str]:
     """
     A helper command for `handle_command` that generates the new arguments for
@@ -474,15 +483,15 @@
         if any(arg.endswith((".cpp", ".cc")) for arg in line):
             new_args = ["em++"]
     elif cmd == "ar":
         line[0] = "emar"
         return line
     elif cmd == "cmake":
         # If it is a build/install command, or running a script, we don't do anything.
-        if "--build" in line or "--install" in line or "-P" in line:
+        if "--build" in line or "--install" in line or "-P" in line or "-E" in line:
             return line
 
         flags = get_cmake_compiler_flags()
         line[:1] = [
             "emcmake",
             "cmake",
             *flags,
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/pyzip.py` & `pyodide_build-0.26.0a5/pyodide_build/pyzip.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,49 +2,17 @@
 from collections.abc import Callable
 from pathlib import Path
 from tempfile import TemporaryDirectory
 
 from ._py_compile import _compile
 from .common import make_zip_archive
 
-# These files are removed from the stdlib
-REMOVED_FILES = (
-    # package management
-    "ensurepip/",
-    "venv/",
-    # build system
-    "lib2to3/",
-    # other platforms
-    "_osx_support.py",
-    "_aix_support.py",
-    # Not supported by browser
-    "curses/",
-    "dbm/",
-    "idlelib/",
-    "tkinter/",
-    "turtle.py",
-    "turtledemo",
-)
-
-# These files are unvendored from the stdlib and can be loaded with `loadPackage`
-UNVENDORED_FILES = (
-    "test/",
-    "sqlite3",
-    "ssl.py",
-    "lzma.py",
-    "_pydecimal.py",
-    "pydoc_data",
-)
-
-# We have JS implementations of these modules
-JS_STUB_FILES = ("webbrowser.py",)
-
 
 def default_filterfunc(
-    root: Path, verbose: bool = False
+    root: Path, excludes: list[str], stubs: list[str], verbose: bool = False
 ) -> Callable[[str, list[str]], set[str]]:
     """
     The default filter function used by `create_zipfile`.
 
     This function filters out several modules that are:
 
     - not supported in Pyodide due to browser limitations (e.g. `tkinter`)
@@ -71,23 +39,21 @@
 
         if path.is_file() and name.endswith(("pyi", "toml", "cfg", "md", "rst")):
             return True
 
         return False
 
     def filterfunc(path: Path | str, names: list[str]) -> set[str]:
-        filtered_files = {
-            (root / f).resolve() for f in REMOVED_FILES + UNVENDORED_FILES
-        }
+        filtered_files = {(root / f).resolve() for f in excludes}
 
         # We have JS implementations of these modules, so we don't need to
         # include the Python ones. Checking the name of the root directory
         # is a bit of a hack, but it works...
         if root.name.startswith("python3"):
-            filtered_files.update({root / f for f in JS_STUB_FILES})
+            filtered_files.update({root / f for f in stubs})
 
         path = Path(path).resolve()
 
         if _should_skip(path):
             return set(names)
 
         _names = []
@@ -103,14 +69,16 @@
         return set(_names)
 
     return filterfunc
 
 
 def create_zipfile(
     libdirs: list[Path],
+    excludes: list[str] | None = None,
+    stubs: list[str] | None = None,
     output: Path | str = "python",
     pycompile: bool = False,
     filterfunc: Callable[[str, list[str]], set[str]] | None = None,
     compression_level: int = 6,
 ) -> None:
     """
     Bundle Python standard libraries into a zip file.
@@ -126,14 +94,20 @@
     hence this function.
 
     Parameters
     ----------
     libdirs
         List of paths to the directory containing the Python standard library or extra packages.
 
+    excludes
+        List of files to exclude from the zip file.
+
+    stubs
+        List of files that are replaced by JS implementations.
+
     output
         Path to the output zip file. Defaults to python.zip.
 
     pycompile
         Whether to compile the .py files into .pyc, by default False
 
     filterfunc
@@ -148,23 +122,25 @@
     Returns
     -------
     BytesIO
         A BytesIO object containing the zip file.
     """
 
     archive = Path(output)
+    excludes = excludes or []
+    stubs = stubs or []
 
     with TemporaryDirectory() as temp_dir_str:
         temp_dir = Path(temp_dir_str)
 
         for libdir in libdirs:
             libdir = Path(libdir)
 
             if filterfunc is None:
-                _filterfunc = default_filterfunc(libdir)
+                _filterfunc = default_filterfunc(libdir, excludes, stubs)
 
             shutil.copytree(libdir, temp_dir, ignore=_filterfunc, dirs_exist_ok=True)
 
         make_zip_archive(
             archive,
             temp_dir,
             compression_level=compression_level,
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/recipe.py` & `pyodide_build-0.26.0a5/pyodide_build/recipe.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,45 +59,45 @@
             tagged_recipes.setdefault(_tag, []).append(recipe)
 
     recipes: dict[str, MetaConfig] = {}
 
     for name_or_tag in names_or_tags:
         # 1. package name
         if name_or_tag in available_recipes:
-            recipes[name_or_tag] = available_recipes[name_or_tag].copy(deep=True)
+            recipes[name_or_tag] = available_recipes[name_or_tag].model_copy(deep=True)
 
         # 2. tag
         elif (
             name_or_tag.startswith("tag:")
             and (tag := name_or_tag.removeprefix("tag:")) in tagged_recipes
         ):
             for recipe in tagged_recipes[tag]:
-                recipes[recipe.package.name] = recipe.copy(deep=True)
+                recipes[recipe.package.name] = recipe.model_copy(deep=True)
 
         # 3. meta packages
         elif name_or_tag == "*":  # all packages
             recipes.update(
                 {
-                    name: package.copy(deep=True)
+                    name: package.model_copy(deep=True)
                     for name, package in available_recipes.items()
                 }
             )
         elif name_or_tag == "no-numpy-dependents":
             # This is a meta package and will be handled outside of this function
             recipes["no-numpy-dependents"] = None  # type: ignore[assignment]
 
         elif name_or_tag in ("core", "min-scipy-stack"):
             logger.warning(
                 f"Using meta package without the 'tag:' prefix is deprecated,"
                 f" use 'tag:{name_or_tag}' instead."
             )
             for recipe in tagged_recipes[name_or_tag]:
-                recipes[recipe.package.name] = recipe.copy(deep=True)
+                recipes[recipe.package.name] = recipe.model_copy(deep=True)
         else:
             raise ValueError(f"Unknown package name or tag: {name_or_tag}")
 
     if load_always_tag:
         always_recipes = tagged_recipes.get("always", [])
         for recipe in always_recipes:
-            recipes[recipe.package.name] = recipe.copy(deep=True)
+            recipes[recipe.package.name] = recipe.model_copy(deep=True)
 
     return recipes
```

### Comparing `pyodide-build-0.26.0a4/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake` & `pyodide_build-0.26.0a5/pyodide_build/tools/cmake/Modules/Platform/Emscripten.cmake`

 * *Files identical despite different names*

### Comparing `pyodide-build-0.26.0a4/pyodide_build/vendor/_pypabuild.py` & `pyodide_build-0.26.0a5/pyodide_build/vendor/_pypabuild.py`

 * *Files 8% similar despite different names*

```diff
@@ -87,14 +87,23 @@
 
 
 class _DefaultIsolatedEnv(DefaultIsolatedEnv):
     @staticmethod
     def log(message: str) -> None:
         _cprint("{bold}* {}{reset}", message)
 
+    @property
+    def scripts_dir(self) -> str:
+        if hasattr(self, "_env_backend"):  # pypabuild >= 1.2.0
+            return self._env_backend.scripts_dir
+        elif hasattr(self, "_scripts_dir"):
+            return self._scripts_dir
+        else:
+            raise AttributeError("No attribute '_env_backend' or '_scripts_dir' found")
+
 
 @contextlib.contextmanager
 def _handle_build_error() -> Iterator[None]:
     try:
         yield
     except (BuildException, FailedProcessError) as e:
         _error(str(e))
```

### Comparing `pyodide-build-0.26.0a4/pyproject.toml` & `pyodide_build-0.26.0a5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [build-system]
-requires = ["setuptools>=61.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "pyodide-build"
 authors = [{name = "Pyodide developers"}]
 description = '"Tools for building Pyodide"'
 classifiers = [
     "Programming Language :: Python :: 3",
@@ -14,25 +14,25 @@
 license = {text = "MPL-2.0"}
 requires-python = ">=3.12"
 dependencies = [
     "pyyaml",
     "ruamel.yaml",
     "packaging",
     "wheel",
-    "build>=1.0.0",
+    "build~=1.2.0",
     "virtualenv",
-    "pydantic>=1.10.2,<2",
+    "pydantic>=2,<3",
     "pyodide-cli~=0.2.1",
     "cmake>=3.24",
     "unearth~=0.6",
     "requests",
     "types-requests",
     "typer",
     "auditwheel-emscripten~=0.0.9",
-    "pyodide-lock==0.1.0a4",
+    "pyodide-lock==0.1.0a6",
     "resolvelib",
     "rich",
     "loky",
 ]
 dynamic = ["version"]
 
 [project.readme]
@@ -40,14 +40,17 @@
 content-type = "text/markdown"
 
 [project.urls]
 Homepage = "https://github.com/pyodide/pyodide"
 "Bug Tracker" = "https://github.com/pyodide/pyodide/issues"
 Documentation = "https://pyodide.org/en/stable/"
 
+[project.entry-points."pipx.run"]
+pyodide = "pyodide_cli.__main__:main"
+
 [project.entry-points."pyodide.cli"]
 build = "pyodide_build.cli.build:main"
 build-recipes = "pyodide_build.cli.build_recipes:build_recipes"
 build-recipes-no-deps = "pyodide_build.cli.build_recipes:build_recipes_no_deps"
 venv = "pyodide_build.cli.venv:main"
 skeleton = "pyodide_build.cli.skeleton:app"
 py-compile = "pyodide_build.cli.py_compile:main"
@@ -55,31 +58,23 @@
 create-zipfile = "pyodide_build.cli.create_zipfile:main"
 xbuildenv = "pyodide_build.cli.xbuildenv:app"
 
 [project.optional-dependencies]
 test = [
     # (FIXME: 2024/01/28) The latest pytest-asyncio 0.23.3 is not compatible with pytest 8.0.0
     "pytest<8.0.0",
-    "pytest-pyodide==0.56.2",
+    "pytest-pyodide==0.57.0",
+    "pytest-httpserver",
     "packaging",
 ]
 deploy = [
     "boto3",
     "moto",
 ]
 
-[tool.setuptools]
-package-dir = {"" = "."}
-license-files = ["LICENSE"]
-include-package-data = false
-
-[tool.setuptools.packages.find]
-where = ["."]
-exclude = ["pyodide_build.tests*"]
-namespaces = true
-
-[tool.setuptools.package-data]
-"pyodide_build.tools" = ["*.ini", "*.cross"]
-"pyodide_build.tools.cmake.Modules.Platform" = ["*.cmake"]
+[tool.hatch]
+version.path = "pyodide_build/__init__.py"
 
-[tool.setuptools.dynamic]
-version = {attr = "pyodide_build.__version__"}
+[tool.hatch.build.targets.sdist]
+exclude = [
+    "/pyodide_build/tests",
+]
```

