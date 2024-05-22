# Comparing `tmp/ignoro-1.2.1.tar.gz` & `tmp/ignoro-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ignoro-1.2.1.tar", last modified: Wed Dec  6 12:18:45 2023, max compression
+gzip compressed data, was "ignoro-1.2.2.tar", last modified: Wed May 22 21:45:13 2024, max compression
```

## Comparing `ignoro-1.2.1.tar` & `ignoro-1.2.2.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1073 2023-12-06 12:18:32.635884 ignoro-1.2.1/LICENSE
--rw-r--r--   0        0        0     5910 2023-12-06 12:18:32.635884 ignoro-1.2.1/README.md
--rw-r--r--   0        0        0      149 2023-12-06 12:18:32.635884 ignoro-1.2.1/ignoro/__init__.py
--rw-r--r--   0        0        0    13148 2023-12-06 12:18:32.635884 ignoro-1.2.1/ignoro/api.py
--rw-r--r--   0        0        0    12450 2023-12-06 12:18:32.635884 ignoro-1.2.1/ignoro/cli.py
--rw-r--r--   0        0        0      174 2023-12-06 12:18:32.635884 ignoro-1.2.1/ignoro/exceptions.py
--rw-r--r--   0        0        0     1556 2023-12-06 12:18:45.111781 ignoro-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     3735 2023-12-06 12:18:32.635884 ignoro-1.2.1/tests/conftest.py
--rw-r--r--   0        0        0    17984 2023-12-06 12:18:32.635884 ignoro-1.2.1/tests/test_api.py
--rw-r--r--   0        0        0    33153 2023-12-06 12:18:32.635884 ignoro-1.2.1/tests/test_cli.py
--rw-r--r--   0        0        0     6972 1970-01-01 00:00:00.000000 ignoro-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-22 21:45:02.569871 ignoro-1.2.2/LICENSE
+-rw-r--r--   0        0        0     6219 2024-05-22 21:45:02.569871 ignoro-1.2.2/README.md
+-rw-r--r--   0        0        0      149 2024-05-22 21:45:02.569871 ignoro-1.2.2/ignoro/__init__.py
+-rw-r--r--   0        0        0    13148 2024-05-22 21:45:02.569871 ignoro-1.2.2/ignoro/api.py
+-rw-r--r--   0        0        0    12450 2024-05-22 21:45:02.569871 ignoro-1.2.2/ignoro/cli.py
+-rw-r--r--   0        0        0      174 2024-05-22 21:45:02.569871 ignoro-1.2.2/ignoro/exceptions.py
+-rw-r--r--   0        0        0     1556 2024-05-22 21:45:13.929925 ignoro-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     3735 2024-05-22 21:45:02.569871 ignoro-1.2.2/tests/conftest.py
+-rw-r--r--   0        0        0    17984 2024-05-22 21:45:02.569871 ignoro-1.2.2/tests/test_api.py
+-rw-r--r--   0        0        0    33153 2024-05-22 21:45:02.569871 ignoro-1.2.2/tests/test_cli.py
+-rw-r--r--   0        0        0     7281 1970-01-01 00:00:00.000000 ignoro-1.2.2/PKG-INFO
```

### Comparing `ignoro-1.2.1/LICENSE` & `ignoro-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/README.md` & `ignoro-1.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,14 @@
-<div align="center"><img src="https://raw.githubusercontent.com/solbero/ignoro/main/logo.png" alt="Logo" /></div>
+<div align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solbero/ignoro/main/logo-dark.png">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/solbero/ignoro/main/logo-light.png">
+    <img src="https://raw.githubusercontent.com/solbero/ignoro/main/logo-light.png" alt="Ignoro project logo" />
+  </picture>
+</div>
 <p align="center"><em>Create .gitignore files with ease from your command line!</em></p>
 <p align="center">
   <a href="https://github.com/solbero/ignoro/actions/workflows/test.yml">
     <img alt="Tests" src="https://img.shields.io/github/actions/workflow/status/solbero/ignoro/test.yml?label=tests"/>
   </a>
   <a href="https://codecov.io/gh/solbero/ignoro">
     <img alt="Coverage" src="https://img.shields.io/codecov/c/github/solbero/ignoro"/>
@@ -202,8 +208,8 @@
 ```sh
 pdm run ruff format .
 pdm run ruff check .
 ```
 
 ## License
 
-Ignoro is licensed under the [MIT License](https://opensource.org/license/mit/).
+Ignoro is licensed under the [MIT License](https://opensource.org/license/mit/).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-                                    [Logo]
+                             [Ignoro project logo]
            CCrreeaattee ..ggiittiiggnnoorree ffiilleess wwiitthh eeaassee ffrroomm yyoouurr ccoommmmaanndd lliinnee!!
        _[_T_e_s_t_s_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]
 ## About Ignoro is a command line interface designed to help you quickly create
 and modify `.gitignore` files for your projects. The CLI uses one or more of
 the 550+ templates supplied by [gitignore.io](https://www.toptal.com/
 developers/gitignore) to craft the perfect `.gitignore` for your project. ##
 Features * [x] Search for templates at [gitignore.io](https://www.toptal.com/
```

### Comparing `ignoro-1.2.1/ignoro/api.py` & `ignoro-1.2.2/ignoro/api.py`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/ignoro/cli.py` & `ignoro-1.2.2/ignoro/cli.py`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/pyproject.toml` & `ignoro-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ignoro"
-version = "1.2.1"
+version = "1.2.2"
 description = "A CLI for creating and modifying .gitignore files based on templates from gitignore.io"
 authors = [
     { name = "solbero", email = "njosol@pm.me" },
 ]
 maintainers = [
     { name = "solbero", email = "njosol@pm.me" },
 ]
```

### Comparing `ignoro-1.2.1/tests/conftest.py` & `ignoro-1.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/tests/test_api.py` & `ignoro-1.2.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/tests/test_cli.py` & `ignoro-1.2.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ignoro-1.2.1/PKG-INFO` & `ignoro-1.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: ignoro
-Version: 1.2.1
+Version: 1.2.2
 Summary: A CLI for creating and modifying .gitignore files based on templates from gitignore.io
-Keywords: gitignore gitignore.io cli python typer
+Keywords: gitignore,gitignore.io,cli,python,typer
 Author-Email: solbero <njosol@pm.me>
 Maintainer-Email: solbero <njosol@pm.me>
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,21 @@
 Project-URL: Repository, https://github.com/solbero/ignoro
 Project-URL: Changelog, https://github.com/solbero/ignoro/blob/main/CHANGELOG.md
 Requires-Python: >=3.10
 Requires-Dist: requests>=2.31.0
 Requires-Dist: typer[all]>=0.9.0
 Description-Content-Type: text/markdown
 
-<div align="center"><img src="https://raw.githubusercontent.com/solbero/ignoro/main/logo.png" alt="Logo" /></div>
+<div align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solbero/ignoro/main/logo-dark.png">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/solbero/ignoro/main/logo-light.png">
+    <img src="https://raw.githubusercontent.com/solbero/ignoro/main/logo-light.png" alt="Ignoro project logo" />
+  </picture>
+</div>
 <p align="center"><em>Create .gitignore files with ease from your command line!</em></p>
 <p align="center">
   <a href="https://github.com/solbero/ignoro/actions/workflows/test.yml">
     <img alt="Tests" src="https://img.shields.io/github/actions/workflow/status/solbero/ignoro/test.yml?label=tests"/>
   </a>
   <a href="https://codecov.io/gh/solbero/ignoro">
     <img alt="Coverage" src="https://img.shields.io/codecov/c/github/solbero/ignoro"/>
@@ -228,8 +234,8 @@
 ```sh
 pdm run ruff format .
 pdm run ruff check .
 ```
 
 ## License
 
-Ignoro is licensed under the [MIT License](https://opensource.org/license/mit/).
+Ignoro is licensed under the [MIT License](https://opensource.org/license/mit/).
```

#### html2text {}

```diff
@@ -1,23 +1,23 @@
-Metadata-Version: 2.1 Name: ignoro Version: 1.2.1 Summary: A CLI for creating
+Metadata-Version: 2.1 Name: ignoro Version: 1.2.2 Summary: A CLI for creating
 and modifying .gitignore files based on templates from gitignore.io Keywords:
-gitignore gitignore.io cli python typer Author-Email: solbero
+gitignore,gitignore.io,cli,python,typer Author-Email: solbero
 pm.me> Maintainer-Email: solbero
 pm.me> License: MIT Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Utilities Project-
 URL: Repository, https://github.com/solbero/ignoro Project-URL: Changelog,
 https://github.com/solbero/ignoro/blob/main/CHANGELOG.md Requires-Python:
 >=3.10 Requires-Dist: requests>=2.31.0 Requires-Dist: typer[all]>=0.9.0
 Description-Content-Type: text/markdown
-                                    [Logo]
+                             [Ignoro project logo]
            CCrreeaattee ..ggiittiiggnnoorree ffiilleess wwiitthh eeaassee ffrroomm yyoouurr ccoommmmaanndd lliinnee!!
        _[_T_e_s_t_s_]_[_C_o_v_e_r_a_g_e_]_[_P_y_P_I_ _-_ _V_e_r_s_i_o_n_]_[_P_y_P_I_ _-_ _P_y_t_h_o_n_ _V_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]
 ## About Ignoro is a command line interface designed to help you quickly create
 and modify `.gitignore` files for your projects. The CLI uses one or more of
 the 550+ templates supplied by [gitignore.io](https://www.toptal.com/
 developers/gitignore) to craft the perfect `.gitignore` for your project. ##
 Features * [x] Search for templates at [gitignore.io](https://www.toptal.com/
```

