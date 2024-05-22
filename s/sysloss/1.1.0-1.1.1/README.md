# Comparing `tmp/sysloss-1.1.0.tar.gz` & `tmp/sysloss-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysloss-1.1.0.tar", max compression
+gzip compressed data, was "sysloss-1.1.1.tar", max compression
```

## Comparing `sysloss-1.1.0.tar` & `sysloss-1.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1070 2024-05-08 16:12:08.645780 sysloss-1.1.0/LICENSE
--rw-r--r--   0        0        0     2621 2024-05-08 16:12:08.645780 sysloss-1.1.0/README.md
--rw-r--r--   0        0        0     1620 2024-05-08 16:12:18.625846 sysloss-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       22 2024-05-08 16:12:18.625846 sysloss-1.1.0/src/sysloss/__init__.py
--rw-r--r--   0        0        0    29244 2024-05-08 16:12:08.653780 sysloss-1.1.0/src/sysloss/components.py
--rw-r--r--   0        0        0    51609 2024-05-08 16:12:08.653780 sysloss-1.1.0/src/sysloss/system.py
--rw-r--r--   0        0        0     3574 1970-01-01 00:00:00.000000 sysloss-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-22 15:06:08.168418 sysloss-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2673 2024-05-22 15:06:08.168418 sysloss-1.1.1/README.md
+-rw-r--r--   0        0        0     1613 2024-05-22 15:06:17.660491 sysloss-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-22 15:06:17.660491 sysloss-1.1.1/src/sysloss/__init__.py
+-rw-r--r--   0        0        0    29244 2024-05-22 15:06:08.176418 sysloss-1.1.1/src/sysloss/components.py
+-rw-r--r--   0        0        0    51545 2024-05-22 15:06:08.176418 sysloss-1.1.1/src/sysloss/system.py
+-rw-r--r--   0        0        0     3615 1970-01-01 00:00:00.000000 sysloss-1.1.1/PKG-INFO
```

### Comparing `sysloss-1.1.0/LICENSE` & `sysloss-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sysloss-1.1.0/README.md` & `sysloss-1.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,24 +3,28 @@
 
 <p align="center">
 <a href="https://github.com/geddy11/sysloss/actions"><img alt="Actions Status" src="https://github.com/geddy11/sysloss/actions/workflows/ci-cd.yml/badge.svg"></a>
 <a href="https://codecov.io/github/geddy11/sysloss"><img src="https://codecov.io/github/geddy11/sysloss/graph/badge.svg?token=9L1ZMN0UET"/></a>
 <a><img alt="PyPI" src="https://img.shields.io/pypi/v/sysloss"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://www.conventionalcommits.org"><img alt="Conv. commits" src="https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white"></a>
-<a href="https://doi.org/10.5281/zenodo.11086061"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086061.svg" alt="DOI"></a>
+<a href="https://doi.org/10.5281/zenodo.11086060"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086060.svg" alt="DOI"></a>
 </p>
 
 # sysLoss
 sysLoss is a tool for analyzing system power and losses. From the smallest IoT sensor to large industrial installations. The tool is efficient and easy to use, the analysis result provides a detailed report on voltages, currents, power and efficiency for every component defined in the system. Output format is Pandas DataFrame: Create charts, plots and export to Excel and other formats. 
 
 ## Installation
 ```bash
 $ pip install sysloss
 ```
+or
+```bash
+$ conda install conda-forge::sysloss
+```
 
 ## Usage
 ```python
 from sysloss.components import *
 from sysloss.system import System
 
 bts = System("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10))
```

#### html2text {}

```diff
@@ -2,24 +2,25 @@
        _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_g_e_d_d_y_1_1_/_s_y_s_l_o_s_s_/_g_r_a_p_h_/
    _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]_[_D_O_I_]
 # sysLoss sysLoss is a tool for analyzing system power and losses. From the
 smallest IoT sensor to large industrial installations. The tool is efficient
 and easy to use, the analysis result provides a detailed report on voltages,
 currents, power and efficiency for every component defined in the system.
 Output format is Pandas DataFrame: Create charts, plots and export to Excel and
-other formats. ## Installation ```bash $ pip install sysloss ``` ## Usage
-```python from sysloss.components import * from sysloss.system import System
-bts = System("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10)) bts.add_comp
-("CR2032", comp=Converter("Buck 1.8V", vo=1.8, eff=0.87)) bts.add_comp("Buck
-1.8V", comp=PLoad("MCU", pwr=13e-3)) bts.add_comp("CR2032", comp=Converter
-("Boost 5V", vo=5.0, eff=0.82)) bts.add_comp("Boost 5V", comp=RLoss("RC
-filter", rs=6.8)) bts.add_comp("RC filter", comp=ILoad("Sensor", ii=6e-3))
-bts.tree() ``` ``` Bluetooth sensor âââ CR2032 âââ Boost 5V â
-âââ RC filter â âââ Sensor âââ Buck 1.8V âââ MCU ```
-```python bts.solve() ``` ![result](https://github.com/geddy11/sysloss/raw/
-main/docs/bts.png) ## Documentation The [documentation](https://
-sysloss.readthedocs.io/en/latest/Getting%20started.html) includes tutorials in
-the form of Jupyter notebooks, located in docs/nb. ## Contributing Interested
-in contributing? Check out the contributing guidelines. Please note that this
-project is released with a Code of Conduct. By contributing to this project,
-you agree to abide by its terms. ## License `sysloss` was created by Geir
-Drange. It is licensed under the terms of the MIT license.
+other formats. ## Installation ```bash $ pip install sysloss ``` or ```bash $
+conda install conda-forge::sysloss ``` ## Usage ```python from
+sysloss.components import * from sysloss.system import System bts = System
+("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10)) bts.add_comp("CR2032",
+comp=Converter("Buck 1.8V", vo=1.8, eff=0.87)) bts.add_comp("Buck 1.8V",
+comp=PLoad("MCU", pwr=13e-3)) bts.add_comp("CR2032", comp=Converter("Boost 5V",
+vo=5.0, eff=0.82)) bts.add_comp("Boost 5V", comp=RLoss("RC filter", rs=6.8))
+bts.add_comp("RC filter", comp=ILoad("Sensor", ii=6e-3)) bts.tree() ``` ```
+Bluetooth sensor âââ CR2032 âââ Boost 5V â âââ RC filter
+â âââ Sensor âââ Buck 1.8V âââ MCU ``` ```python bts.solve
+() ``` ![result](https://github.com/geddy11/sysloss/raw/main/docs/bts.png) ##
+Documentation The [documentation](https://sysloss.readthedocs.io/en/latest/
+Getting%20started.html) includes tutorials in the form of Jupyter notebooks,
+located in docs/nb. ## Contributing Interested in contributing? Check out the
+contributing guidelines. Please note that this project is released with a Code
+of Conduct. By contributing to this project, you agree to abide by its terms.
+## License `sysloss` was created by Geir Drange. It is licensed under the terms
+of the MIT license.
```

### Comparing `sysloss-1.1.0/pyproject.toml` & `sysloss-1.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
 [tool.poetry]
 name = "sysloss"
-version = "1.1.0"
+version = "1.1.1"
 description = "Power analysis of circuits and systems."
 authors = ["Geir Drange"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/geddy11/sysloss"
 repository = "https://github.com/geddy11/sysloss"
 documentation = "https://sysloss.readthedocs.io/en/latest/Getting%20started.html#"
 keywords = ["system", "power" , "loss", "efficiency", "energy", "component"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
-scipy = "^1.9.0"
-pandas = "^2.0.0"
-rustworkx = "^0.13.0"
-rich = "^12.0.0"
-toml = "^0.10.2"
-matplotlib = "^3.0.0"
+scipy = "^1.9"
+pandas = "^2.0"
+rustworkx = ">=0.13"
+rich = ">=12.0"
+toml = ">=0.10.2"
+matplotlib = "^3.0"
+tqdm = ">=4.63"
 
 [tool.poetry.dev-dependencies]
-pytest = "^8.0.0"
-pytest-cov = "^4.0.0"
-matplotlib = "^3.0.0"
+pytest = "^8.0"
+pytest-cov = "^4.0"
+matplotlib = "^3.0"
 jupyter-book = "^1.0.0"
-toml = "^0.10.2"
-pandas = "^2.0.0"
-tqdm = "^4.63.0"
+toml = ">=0.10.2"
+pandas = "^2.0"
+tqdm = ">=4.63"
 
 [tool.poetry.group.docs]
 optional = true
 
 [tool.poetry.group.docs.dependencies]
-scipy = "^1.9.0"
-pandas = "^2.0.0"
-rustworkx = "^0.13.0"
-rich = "^12.0.0"
-toml = "^0.10.2"
-matplotlib = "^3.0.0"
-tqdm = "^4.63.0"
+scipy = "^1.9"
+pandas = "^2.0"
+rustworkx = ">=0.13"
+rich = ">=12.0"
+toml = ">=0.10.2"
+matplotlib = "^3.0"
+tqdm = ">=4.63"
 
 [tool.semantic_release]
 allow_zero_version = false
 version_toml = [
     "pyproject.toml:tool.poetry.version",
 ]                                                    # version location
 version_variables = [
```

### Comparing `sysloss-1.1.0/src/sysloss/components.py` & `sysloss-1.1.1/src/sysloss/components.py`

 * *Files identical despite different names*

### Comparing `sysloss-1.1.0/src/sysloss/system.py` & `sysloss-1.1.1/src/sysloss/system.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
 """:py:class:`~system.System` is the primary class for power analysis."""
 
 
 import rustworkx as rx
 import numpy as np
 from rich.tree import Tree
+from rich import print
 import json
 import pandas as pd
 import matplotlib
 import matplotlib.pyplot as plt
 from matplotlib.ticker import LinearLocator
 from scipy.interpolate import LinearNDInterpolator
 from typing import Callable
@@ -432,19 +433,14 @@
         The tree object is generated with `Rich <https://rich.readthedocs.io>`_.
 
         Parameters
         ----------
         name : str, optional
             Name of component to start with. If not given, print the entire system., by default ""
 
-        Returns
-        -------
-        rich.tree.Tree
-            System Tree class.
-
         Raises
         ------
         ValueError
             If the component name is invalid.
         """
         if not name == "":
             if not name in self._g.attrs["nodes"].keys():
@@ -460,15 +456,15 @@
             ndict = {}
             for i in adj:
                 c = []
                 for j in i[1]:
                     c += [j._params["name"]]
                 ndict[i[0]._params["name"]] = c
             t.add(self._make_rtree(ndict, n))
-        return t
+        print(t)
 
     def _set_phase_lkup(self):
         """Make lookup from node # to load phases"""
         self._phase_lkup = {}
         for c in self._g.attrs["phase_conf"].items():
             self._phase_lkup[self._get_index(c[0])] = c[1]
```

### Comparing `sysloss-1.1.0/PKG-INFO` & `sysloss-1.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,50 +1,55 @@
 Metadata-Version: 2.1
 Name: sysloss
-Version: 1.1.0
+Version: 1.1.1
 Summary: Power analysis of circuits and systems.
 Home-page: https://github.com/geddy11/sysloss
 License: MIT
 Keywords: system,power,loss,efficiency,energy,component
 Author: Geir Drange
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
-Requires-Dist: matplotlib (>=3.0.0,<4.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
-Requires-Dist: rich (>=12.0.0,<13.0.0)
-Requires-Dist: rustworkx (>=0.13.0,<0.14.0)
-Requires-Dist: scipy (>=1.9.0,<2.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
+Requires-Dist: matplotlib (>=3.0,<4.0)
+Requires-Dist: pandas (>=2.0,<3.0)
+Requires-Dist: rich (>=12.0)
+Requires-Dist: rustworkx (>=0.13)
+Requires-Dist: scipy (>=1.9,<2.0)
+Requires-Dist: toml (>=0.10.2)
+Requires-Dist: tqdm (>=4.63)
 Project-URL: Documentation, https://sysloss.readthedocs.io/en/latest/Getting%20started.html#
 Project-URL: Repository, https://github.com/geddy11/sysloss
 Description-Content-Type: text/markdown
 
 
 ![](https://github.com/geddy11/sysloss/raw/main/docs/sysloss.svg)
 
 <p align="center">
 <a href="https://github.com/geddy11/sysloss/actions"><img alt="Actions Status" src="https://github.com/geddy11/sysloss/actions/workflows/ci-cd.yml/badge.svg"></a>
 <a href="https://codecov.io/github/geddy11/sysloss"><img src="https://codecov.io/github/geddy11/sysloss/graph/badge.svg?token=9L1ZMN0UET"/></a>
 <a><img alt="PyPI" src="https://img.shields.io/pypi/v/sysloss"></a>
 <a href="https://github.com/psf/black"><img alt="Code style: black" src="https://img.shields.io/badge/code%20style-black-000000.svg"></a>
 <a href="https://www.conventionalcommits.org"><img alt="Conv. commits" src="https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white"></a>
-<a href="https://doi.org/10.5281/zenodo.11086061"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086061.svg" alt="DOI"></a>
+<a href="https://doi.org/10.5281/zenodo.11086060"><img src="https://zenodo.org/badge/DOI/10.5281/zenodo.11086060.svg" alt="DOI"></a>
 </p>
 
 # sysLoss
 sysLoss is a tool for analyzing system power and losses. From the smallest IoT sensor to large industrial installations. The tool is efficient and easy to use, the analysis result provides a detailed report on voltages, currents, power and efficiency for every component defined in the system. Output format is Pandas DataFrame: Create charts, plots and export to Excel and other formats. 
 
 ## Installation
 ```bash
 $ pip install sysloss
 ```
+or
+```bash
+$ conda install conda-forge::sysloss
+```
 
 ## Usage
 ```python
 from sysloss.components import *
 from sysloss.system import System
 
 bts = System("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10))
```

#### html2text {}

```diff
@@ -1,38 +1,38 @@
-Metadata-Version: 2.1 Name: sysloss Version: 1.1.0 Summary: Power analysis of
+Metadata-Version: 2.1 Name: sysloss Version: 1.1.1 Summary: Power analysis of
 circuits and systems. Home-page: https://github.com/geddy11/sysloss License:
 MIT Keywords: system,power,loss,efficiency,energy,component Author: Geir Drange
 Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
-(>=3.0.0,<4.0.0) Requires-Dist: pandas (>=2.0.0,<3.0.0) Requires-Dist: rich
-(>=12.0.0,<13.0.0) Requires-Dist: rustworkx (>=0.13.0,<0.14.0) Requires-Dist:
-scipy (>=1.9.0,<2.0.0) Requires-Dist: toml (>=0.10.2,<0.11.0) Project-URL:
-Documentation, https://sysloss.readthedocs.io/en/latest/Getting%20started.html#
-Project-URL: Repository, https://github.com/geddy11/sysloss Description-
-Content-Type: text/markdown ![](https://github.com/geddy11/sysloss/raw/main/
-docs/sysloss.svg)
+(>=3.0,<4.0) Requires-Dist: pandas (>=2.0,<3.0) Requires-Dist: rich (>=12.0)
+Requires-Dist: rustworkx (>=0.13) Requires-Dist: scipy (>=1.9,<2.0) Requires-
+Dist: toml (>=0.10.2) Requires-Dist: tqdm (>=4.63) Project-URL: Documentation,
+https://sysloss.readthedocs.io/en/latest/Getting%20started.html# Project-URL:
+Repository, https://github.com/geddy11/sysloss Description-Content-Type: text/
+markdown ![](https://github.com/geddy11/sysloss/raw/main/docs/sysloss.svg)
        _[_A_c_t_i_o_n_s_ _S_t_a_t_u_s_]_[_h_t_t_p_s_:_/_/_c_o_d_e_c_o_v_._i_o_/_g_i_t_h_u_b_/_g_e_d_d_y_1_1_/_s_y_s_l_o_s_s_/_g_r_a_p_h_/
    _b_a_d_g_e_._s_v_g_?_t_o_k_e_n_=_9_L_1_Z_M_N_0_U_E_T_][PyPI]_[_C_o_d_e_ _s_t_y_l_e_:_ _b_l_a_c_k_]_[_C_o_n_v_._ _c_o_m_m_i_t_s_]_[_D_O_I_]
 # sysLoss sysLoss is a tool for analyzing system power and losses. From the
 smallest IoT sensor to large industrial installations. The tool is efficient
 and easy to use, the analysis result provides a detailed report on voltages,
 currents, power and efficiency for every component defined in the system.
 Output format is Pandas DataFrame: Create charts, plots and export to Excel and
-other formats. ## Installation ```bash $ pip install sysloss ``` ## Usage
-```python from sysloss.components import * from sysloss.system import System
-bts = System("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10)) bts.add_comp
-("CR2032", comp=Converter("Buck 1.8V", vo=1.8, eff=0.87)) bts.add_comp("Buck
-1.8V", comp=PLoad("MCU", pwr=13e-3)) bts.add_comp("CR2032", comp=Converter
-("Boost 5V", vo=5.0, eff=0.82)) bts.add_comp("Boost 5V", comp=RLoss("RC
-filter", rs=6.8)) bts.add_comp("RC filter", comp=ILoad("Sensor", ii=6e-3))
-bts.tree() ``` ``` Bluetooth sensor âââ CR2032 âââ Boost 5V â
-âââ RC filter â âââ Sensor âââ Buck 1.8V âââ MCU ```
-```python bts.solve() ``` ![result](https://github.com/geddy11/sysloss/raw/
-main/docs/bts.png) ## Documentation The [documentation](https://
-sysloss.readthedocs.io/en/latest/Getting%20started.html) includes tutorials in
-the form of Jupyter notebooks, located in docs/nb. ## Contributing Interested
-in contributing? Check out the contributing guidelines. Please note that this
-project is released with a Code of Conduct. By contributing to this project,
-you agree to abide by its terms. ## License `sysloss` was created by Geir
-Drange. It is licensed under the terms of the MIT license.
+other formats. ## Installation ```bash $ pip install sysloss ``` or ```bash $
+conda install conda-forge::sysloss ``` ## Usage ```python from
+sysloss.components import * from sysloss.system import System bts = System
+("Bluetooth sensor", Source("CR2032", vo=3.0, rs=10)) bts.add_comp("CR2032",
+comp=Converter("Buck 1.8V", vo=1.8, eff=0.87)) bts.add_comp("Buck 1.8V",
+comp=PLoad("MCU", pwr=13e-3)) bts.add_comp("CR2032", comp=Converter("Boost 5V",
+vo=5.0, eff=0.82)) bts.add_comp("Boost 5V", comp=RLoss("RC filter", rs=6.8))
+bts.add_comp("RC filter", comp=ILoad("Sensor", ii=6e-3)) bts.tree() ``` ```
+Bluetooth sensor âââ CR2032 âââ Boost 5V â âââ RC filter
+â âââ Sensor âââ Buck 1.8V âââ MCU ``` ```python bts.solve
+() ``` ![result](https://github.com/geddy11/sysloss/raw/main/docs/bts.png) ##
+Documentation The [documentation](https://sysloss.readthedocs.io/en/latest/
+Getting%20started.html) includes tutorials in the form of Jupyter notebooks,
+located in docs/nb. ## Contributing Interested in contributing? Check out the
+contributing guidelines. Please note that this project is released with a Code
+of Conduct. By contributing to this project, you agree to abide by its terms.
+## License `sysloss` was created by Geir Drange. It is licensed under the terms
+of the MIT license.
```

