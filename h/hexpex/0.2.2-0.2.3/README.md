# Comparing `tmp/hexpex-0.2.2.tar.gz` & `tmp/hexpex-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hexpex-0.2.2.tar", max compression
+gzip compressed data, was "hexpex-0.2.3.tar", max compression
```

## Comparing `hexpex-0.2.2.tar` & `hexpex-0.2.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    35149 2023-08-26 08:08:02.171520 hexpex-0.2.2/LICENSE
--rw-r--r--   0        0        0     6848 2023-08-26 08:08:02.171520 hexpex-0.2.2/README.md
--rw-r--r--   0        0        0      745 2023-08-26 08:08:02.171520 hexpex-0.2.2/hexpex/__init__.py
--rw-r--r--   0        0        0    13507 2023-08-26 08:08:02.171520 hexpex-0.2.2/hexpex/hex.py
--rw-r--r--   0        0        0      997 2023-08-26 08:08:02.171520 hexpex-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     7479 1970-01-01 00:00:00.000000 hexpex-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 21:43:38.370163 hexpex-0.2.3/LICENSE
+-rw-r--r--   0        0        0     7143 2024-05-22 21:43:38.370163 hexpex-0.2.3/README.md
+-rw-r--r--   0        0        0      745 2024-05-22 21:43:38.370163 hexpex-0.2.3/hexpex/__init__.py
+-rw-r--r--   0        0        0    13507 2024-05-22 21:43:38.370163 hexpex-0.2.3/hexpex/hex.py
+-rw-r--r--   0        0        0      997 2024-05-22 21:43:38.374163 hexpex-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     7774 1970-01-01 00:00:00.000000 hexpex-0.2.3/PKG-INFO
```

### Comparing `hexpex-0.2.2/LICENSE` & `hexpex-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hexpex-0.2.2/README.md` & `hexpex-0.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 <!-- PROJECT TITLE -->
-<p align="center"><img src="https://raw.githubusercontent.com/solbero/hexpex/main/logo.png" /></p>
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solbero/hexpex/main/logo-dark.png">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/solbero/hexpex/main/logo-light.png">
+    <img src="https://raw.githubusercontent.com/solbero/hexpex/main/logo-light.png" alt="Hexpex project logo" />
+  </picture>
+</p>
 
 <!-- PROJECT BLURB -->
 <p align="center">
   <em>A type-hinted, object-oriented Python implementation for working with hex grids</em>
 </p>
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
-  <a href="https://github.com/solbero/hexpex/actions/workflows/build.yaml/" target="_blank">
-    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/build.yaml?branch=main&label=build" alt="Build action">
+  <a href="https://github.com/solbero/hexpex/actions/workflows/build.yaml" target="_blank">
+    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/build.yaml?label=build" alt="Build action">
   </a>
-  <a href="https://github.com/solbero/hexpex/actions/workflows/publish.yaml/" target="_blank">
-    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/publish.yaml?branch=main&label=publish" alt="Publish action">
+  <a href="https://github.com/solbero/hexpex/actions/workflows/publish.yaml" target="_blank">
+    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/publish.yaml?label=publish" alt="Publish action" >
+
   </a>
   <a href="https://app.codecov.io/gh/solbero/hexpex" target="_blank">
     <img src="https://img.shields.io/codecov/c/github/solbero/hexpex" alt="Code coverage">
   </a>
   <a href="https://pypi.org/project/hexpex/" target="_blank">
     <img src="https://img.shields.io/pypi/v/hexpex" alt="Package version">
   </a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-       [https://raw.githubusercontent.com/solbero/hexpex/main/logo.png]
+                             [Hexpex project logo]
 AA ttyyppee--hhiinntteedd,, oobbjjeecctt--oorriieenntteedd PPyytthhoonn iimmpplleemmeennttaattiioonn ffoorr wwoorrkkiinngg wwiitthh hheexx ggrriiddss
 _[_B_u_i_l_d_ _a_c_t_i_o_n_]_[_P_u_b_l_i_s_h_ _a_c_t_i_o_n_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
                               _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 ## About the Project This is a type-hinted, object-oriented implementation in
 Python of [hexagonal grids](https://www.redblobgames.com/grids/hexagons/) as
 described on [Red Blob Games](https://www.redblobgames.com/). This package
 allows you to easily work with hexagonal grids in Python. All of its classes,
```

### Comparing `hexpex-0.2.2/hexpex/__init__.py` & `hexpex-0.2.3/hexpex/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 from hexpex.hex import Axial as Axial
 from hexpex.hex import AxialFlatAdjacentDirection as AxialFlatAdjacentDirection
 from hexpex.hex import AxialFlatDiagonalDirection as AxialFlatDiagonalDirection
 from hexpex.hex import AxialPointyAdjacentDirection as AxialPointyAdjacentDirection
 from hexpex.hex import AxialPointyDiagonalDirection as AxialPointyDiagonalDirection
 from hexpex.hex import Cube as Cube
```

### Comparing `hexpex-0.2.2/hexpex/hex.py` & `hexpex-0.2.3/hexpex/hex.py`

 * *Files identical despite different names*

### Comparing `hexpex-0.2.2/pyproject.toml` & `hexpex-0.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hexpex"
-version = "0.2.2"
+version = "0.2.3"
 description = "A type-hinted, object-oriented Python implementation for working with hex grids"
 authors = ["solbero <njord.solberg@gmail.com>"]
 license = "GPLv3"
 readme = "README.md"
 repository = "https://github.com/solbero/hexpex"
 
 [tool.poetry.dependencies]
```

### Comparing `hexpex-0.2.2/PKG-INFO` & `hexpex-0.2.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hexpex
-Version: 0.2.2
+Version: 0.2.3
 Summary: A type-hinted, object-oriented Python implementation for working with hex grids
 Home-page: https://github.com/solbero/hexpex
 License: GPLv3
 Author: solbero
 Author-email: njord.solberg@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
@@ -12,28 +12,35 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/solbero/hexpex
 Description-Content-Type: text/markdown
 
 <!-- PROJECT TITLE -->
-<p align="center"><img src="https://raw.githubusercontent.com/solbero/hexpex/main/logo.png" /></p>
+<p align="center">
+  <picture>
+    <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/solbero/hexpex/main/logo-dark.png">
+    <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/solbero/hexpex/main/logo-light.png">
+    <img src="https://raw.githubusercontent.com/solbero/hexpex/main/logo-light.png" alt="Hexpex project logo" />
+  </picture>
+</p>
 
 <!-- PROJECT BLURB -->
 <p align="center">
   <em>A type-hinted, object-oriented Python implementation for working with hex grids</em>
 </p>
 
 <!-- PROJECT SHIELDS -->
 <div align="center">
-  <a href="https://github.com/solbero/hexpex/actions/workflows/build.yaml/" target="_blank">
-    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/build.yaml?branch=main&label=build" alt="Build action">
+  <a href="https://github.com/solbero/hexpex/actions/workflows/build.yaml" target="_blank">
+    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/build.yaml?label=build" alt="Build action">
   </a>
-  <a href="https://github.com/solbero/hexpex/actions/workflows/publish.yaml/" target="_blank">
-    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/publish.yaml?branch=main&label=publish" alt="Publish action">
+  <a href="https://github.com/solbero/hexpex/actions/workflows/publish.yaml" target="_blank">
+    <img src="https://img.shields.io/github/actions/workflow/status/solbero/hexpex/publish.yaml?label=publish" alt="Publish action" >
+
   </a>
   <a href="https://app.codecov.io/gh/solbero/hexpex" target="_blank">
     <img src="https://img.shields.io/codecov/c/github/solbero/hexpex" alt="Code coverage">
   </a>
   <a href="https://pypi.org/project/hexpex/" target="_blank">
     <img src="https://img.shields.io/pypi/v/hexpex" alt="Package version">
   </a>
```

#### html2text {}

```diff
@@ -1,17 +1,17 @@
-Metadata-Version: 2.1 Name: hexpex Version: 0.2.2 Summary: A type-hinted,
+Metadata-Version: 2.1 Name: hexpex Version: 0.2.3 Summary: A type-hinted,
 object-oriented Python implementation for working with hex grids Home-page:
 https://github.com/solbero/hexpex License: GPLv3 Author: solbero Author-email:
 njord.solberg@gmail.com Requires-Python: >=3.9,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Project-URL: Repository, https://github.com/solbero/hexpex Description-Content-
 Type: text/markdown
-       [https://raw.githubusercontent.com/solbero/hexpex/main/logo.png]
+                             [Hexpex project logo]
 AA ttyyppee--hhiinntteedd,, oobbjjeecctt--oorriieenntteedd PPyytthhoonn iimmpplleemmeennttaattiioonn ffoorr wwoorrkkiinngg wwiitthh hheexx ggrriiddss
 _[_B_u_i_l_d_ _a_c_t_i_o_n_]_[_P_u_b_l_i_s_h_ _a_c_t_i_o_n_]_[_C_o_d_e_ _c_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_[_S_u_p_p_o_r_t_e_d_ _P_y_t_h_o_n
                               _v_e_r_s_i_o_n_s_]_[_L_i_c_e_n_s_e_]
 ## About the Project This is a type-hinted, object-oriented implementation in
 Python of [hexagonal grids](https://www.redblobgames.com/grids/hexagons/) as
 described on [Red Blob Games](https://www.redblobgames.com/). This package
 allows you to easily work with hexagonal grids in Python. All of its classes,
```

