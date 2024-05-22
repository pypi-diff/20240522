# Comparing `tmp/amep-1.0.1.tar.gz` & `tmp/amep-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amep-1.0.1.tar", last modified: Mon Apr 22 13:12:38 2024, max compression
+gzip compressed data, was "amep-1.0.2.tar", last modified: Wed May 22 12:17:48 2024, max compression
```

## Comparing `amep-1.0.1.tar` & `amep-1.0.2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.631772 amep-1.0.1/
--rw-rw-rw-   0        0        0      810 2024-03-21 11:20:52.000000 amep-1.0.1/AUTHORS
--rw-rw-rw-   0        0        0    35823 2023-12-19 10:42:45.000000 amep-1.0.1/LICENSE
--rw-rw-rw-   0        0        0     2277 2023-12-19 10:42:45.000000 amep-1.0.1/LICENSES.third-party
--rw-rw-rw-   0        0        0       42 2024-03-21 11:20:52.000000 amep-1.0.1/MANIFEST.in
--rw-rw-rw-   0        0        0    56892 2024-04-22 13:12:38.627445 amep-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    13851 2024-04-22 12:32:20.000000 amep-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.527495 amep-1.0.1/amep/
--rw-rw-rw-   0        0        0     2479 2024-03-11 15:50:56.000000 amep-1.0.1/amep/__init__.py
--rw-rw-rw-   0        0        0     1021 2024-04-22 12:32:20.000000 amep-1.0.1/amep/_version.py
--rw-rw-rw-   0        0        0    73256 2024-04-22 12:32:20.000000 amep-1.0.1/amep/base.py
--rw-rw-rw-   0        0        0    39715 2024-03-14 12:47:14.000000 amep-1.0.1/amep/cluster.py
--rw-rw-rw-   0        0        0    30285 2024-04-22 12:32:20.000000 amep-1.0.1/amep/continuum.py
--rw-rw-rw-   0        0        0   151395 2024-04-22 12:32:20.000000 amep-1.0.1/amep/evaluate.py
--rw-rw-rw-   0        0        0    26422 2024-03-14 12:47:14.000000 amep-1.0.1/amep/functions.py
--rw-rw-rw-   0        0        0    13073 2024-04-17 12:38:54.000000 amep-1.0.1/amep/load.py
--rw-rw-rw-   0        0        0    58441 2024-03-14 12:47:14.000000 amep-1.0.1/amep/order.py
--rw-rw-rw-   0        0        0    41852 2024-03-14 12:47:14.000000 amep-1.0.1/amep/pbc.py
--rw-rw-rw-   0        0        0    66438 2024-04-22 12:32:20.000000 amep-1.0.1/amep/plot.py
--rw-rw-rw-   0        0        0    47910 2024-04-22 12:32:20.000000 amep-1.0.1/amep/reader.py
--rw-rw-rw-   0        0        0    62236 2024-04-22 12:32:20.000000 amep-1.0.1/amep/spatialcor.py
--rw-rw-rw-   0        0        0    12917 2024-03-14 12:47:14.000000 amep-1.0.1/amep/statistics.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.531184 amep-1.0.1/amep/styles/
--rw-rw-rw-   0        0        0     1730 2024-02-15 19:00:52.000000 amep-1.0.1/amep/styles/amep_latex.mplstyle
--rw-rw-rw-   0        0        0     2437 2024-02-15 19:00:52.000000 amep-1.0.1/amep/styles/amep_standard.mplstyle
--rw-rw-rw-   0        0        0     7425 2024-03-14 12:47:14.000000 amep-1.0.1/amep/thermo.py
--rw-rw-rw-   0        0        0     4302 2024-03-11 15:50:56.000000 amep-1.0.1/amep/timecor.py
--rw-rw-rw-   0        0        0    16421 2024-03-14 12:47:14.000000 amep-1.0.1/amep/trajectory.py
--rw-rw-rw-   0        0        0    64120 2024-03-14 12:47:14.000000 amep-1.0.1/amep/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.625007 amep-1.0.1/amep.egg-info/
--rw-rw-rw-   0        0        0      518 2024-04-22 13:12:38.000000 amep-1.0.1/amep.egg-info/SOURCES.txt
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.579767 amep-1.0.1/examples/
--rw-rw-rw-   0        0        0     2439 2024-03-15 12:08:10.000000 amep-1.0.1/examples/continuum-example.py
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.408500 amep-1.0.1/examples/data/
-drwxrwxrwx   0        0        0        0 2024-04-22 13:12:38.604843 amep-1.0.1/examples/data/continuum/
--rw-rw-rw-   0        0        0     6298 2024-02-15 16:04:47.000000 amep-1.0.1/examples/data/continuum/solver.py
--rw-rw-rw-   0        0        0     3709 2024-03-15 12:08:10.000000 amep-1.0.1/examples/particle-example.py
--rw-rw-rw-   0        0        0     2027 2024-04-22 12:32:20.000000 amep-1.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-22 13:12:38.631772 amep-1.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.835806 amep-1.0.2/
+-rw-rw-rw-   0        0        0      810 2024-03-21 11:20:52.000000 amep-1.0.2/AUTHORS
+-rw-rw-rw-   0        0        0    35823 2023-12-19 10:42:45.000000 amep-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0     2277 2023-12-19 10:42:45.000000 amep-1.0.2/LICENSES.third-party
+-rw-rw-rw-   0        0        0       42 2024-03-21 11:20:52.000000 amep-1.0.2/MANIFEST.in
+-rw-rw-rw-   0        0        0    58256 2024-05-22 12:17:48.832724 amep-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0    15215 2024-05-22 12:01:39.000000 amep-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.692187 amep-1.0.2/amep/
+-rw-rw-rw-   0        0        0     2479 2024-03-11 15:50:56.000000 amep-1.0.2/amep/__init__.py
+-rw-rw-rw-   0        0        0     1021 2024-05-22 12:01:39.000000 amep-1.0.2/amep/_version.py
+-rw-rw-rw-   0        0        0    73256 2024-04-22 12:32:20.000000 amep-1.0.2/amep/base.py
+-rw-rw-rw-   0        0        0    39715 2024-03-14 12:47:14.000000 amep-1.0.2/amep/cluster.py
+-rw-rw-rw-   0        0        0    30285 2024-04-22 12:32:20.000000 amep-1.0.2/amep/continuum.py
+-rw-rw-rw-   0        0        0   151385 2024-05-22 12:01:39.000000 amep-1.0.2/amep/evaluate.py
+-rw-rw-rw-   0        0        0    26422 2024-03-14 12:47:14.000000 amep-1.0.2/amep/functions.py
+-rw-rw-rw-   0        0        0    13073 2024-04-17 12:38:54.000000 amep-1.0.2/amep/load.py
+-rw-rw-rw-   0        0        0    58441 2024-03-14 12:47:14.000000 amep-1.0.2/amep/order.py
+-rw-rw-rw-   0        0        0    41852 2024-03-14 12:47:14.000000 amep-1.0.2/amep/pbc.py
+-rw-rw-rw-   0        0        0    66565 2024-05-22 12:01:39.000000 amep-1.0.2/amep/plot.py
+-rw-rw-rw-   0        0        0    47910 2024-04-22 12:32:20.000000 amep-1.0.2/amep/reader.py
+-rw-rw-rw-   0        0        0    62236 2024-04-22 12:32:20.000000 amep-1.0.2/amep/spatialcor.py
+-rw-rw-rw-   0        0        0    12917 2024-03-14 12:47:14.000000 amep-1.0.2/amep/statistics.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.697173 amep-1.0.2/amep/styles/
+-rw-rw-rw-   0        0        0     1730 2024-02-15 19:00:52.000000 amep-1.0.2/amep/styles/amep_latex.mplstyle
+-rw-rw-rw-   0        0        0     2437 2024-02-15 19:00:52.000000 amep-1.0.2/amep/styles/amep_standard.mplstyle
+-rw-rw-rw-   0        0        0     7425 2024-03-14 12:47:14.000000 amep-1.0.2/amep/thermo.py
+-rw-rw-rw-   0        0        0     4302 2024-03-11 15:50:56.000000 amep-1.0.2/amep/timecor.py
+-rw-rw-rw-   0        0        0    16421 2024-03-14 12:47:14.000000 amep-1.0.2/amep/trajectory.py
+-rw-rw-rw-   0        0        0    64120 2024-03-14 12:47:14.000000 amep-1.0.2/amep/utils.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.829729 amep-1.0.2/amep.egg-info/
+-rw-rw-rw-   0        0        0      518 2024-05-22 12:17:48.000000 amep-1.0.2/amep.egg-info/SOURCES.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.717014 amep-1.0.2/examples/
+-rw-rw-rw-   0        0        0     2439 2024-03-15 12:08:10.000000 amep-1.0.2/examples/continuum-example.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.542218 amep-1.0.2/examples/data/
+drwxrwxrwx   0        0        0        0 2024-05-22 12:17:48.732433 amep-1.0.2/examples/data/continuum/
+-rw-rw-rw-   0        0        0     6298 2024-02-15 16:04:47.000000 amep-1.0.2/examples/data/continuum/solver.py
+-rw-rw-rw-   0        0        0     3709 2024-03-15 12:08:10.000000 amep-1.0.2/examples/particle-example.py
+-rw-rw-rw-   0        0        0     2078 2024-05-22 12:01:39.000000 amep-1.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:17:48.835806 amep-1.0.2/setup.cfg
```

### Comparing `amep-1.0.1/AUTHORS` & `amep-1.0.2/AUTHORS`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/LICENSE` & `amep-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/LICENSES.third-party` & `amep-1.0.2/LICENSES.third-party`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/PKG-INFO` & `amep-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amep
-Version: 1.0.1
+Version: 1.0.2
 Summary: Active Matter Evaluation Package for data analysis of active matter simulations
 Author-email: Lukas Hecht <lukas.hecht@pkm.tu-darmstadt.de>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -716,14 +716,16 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![GitHub Discussions](https://img.shields.io/github/discussions/amepproject/amep)](https://github.com/amepproject/amep/discussions)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Famepproject%2Famep%2Fmain%2Fpyproject.toml)
 [![Static Badge](https://img.shields.io/badge/documentation-amepproject.de-blue)](https://amepproject.de)
 [![Pepy Total Downlods](https://img.shields.io/pepy/dt/amep?label=pypi%7Cdownloads)](https://pypi.org/project/amep/)
 [![Conda Downloads](https://img.shields.io/conda/d/conda-forge/amep)](https://anaconda.org/conda-forge/amep)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/amepproject/amep/test.yml?label=pipeline)](https://github.com/amepproject/amep/actions)
+[![Static Badge](https://img.shields.io/badge/arXiv-2404.16533-brown)](https://doi.org/10.48550/arXiv.2404.16533)
+
 
 <center><img src="https://raw.githubusercontent.com/amepproject/amep/main/doc/source/_static/images/amep-logo_v2.png" alt="amep logo" width="200" height="200"/></center>
 
 The **AMEP** (**A**ctive **M**atter **E**valuation **P**ackage) Python library 
 is a powerful tool for analyzing data from molecular-dynamics (MD), 
 Brownian-dynamics (BD), and continuum simulations. It comprises various 
 methods to analyze structural and dynamical properties of condensed matter 
@@ -855,14 +857,48 @@
 **AMEP** provides the possibility to animate plots and trajectories. 
 **To enable all animation features, FFmpeg must be installed on the device on** 
 **which you run AMEP**. FFmpeg is not automatically installed when you install 
 **AMEP**. Please visit [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html) 
 to download FFmpeg and to get further information on how to install FFmpeg on your machine.
 
 
+# Citation
+
+If you use **AMEP** for a project that leads to a scientific publication, please acknowledge 
+the use of **AMEP** within the body of your publication for example by copying or adapting 
+the following formulation:
+
+*Data analysis for this publication utilized the AMEP library [1].*
+
+> [1] L. Hecht, K.-R. Dormann, K. L. Spanheimer, M. Ebrahimi, M. Cordts, S. Mandal, 
+>     A. K. Mukhopadhyay, and B. Liebchen, AMEP: The Active Matter Evaluation Package for Python, 
+>     *arXiv [Cond-Mat.Soft]* (2024). Available at: http://arxiv.org/abs/2404.16533.
+
+The pre-print is freely available on [arXiv](https://arxiv.org/abs/2404.16533). To cite this reference, 
+you can use the following BibTeX entry:
+
+```bibtex
+@misc{hecht2024amep,
+    title = {AMEP: The Active Matter Evaluation Package for Python}, 
+    author = {Lukas Hecht and 
+              Kay-Robert Dormann and 
+              Kai Luca Spanheimer and 
+              Mahdieh Ebrahimi and 
+              Malte Cordts and 
+              Suvendu Mandal and 
+              Aritra K. Mukhopadhyay and 
+              Benno Liebchen},
+    year = {2024},
+    eprint = {2404.16533},
+    archivePrefix = {arXiv},
+    primaryClass = {cond-mat.soft}
+}
+```
+
+
 # Getting started
 
 The following example briefly demonstrates the **AMEP** workflow. A typical 
 task is to calculate the average of an observable over several frames of the 
 simulation (time average). In the example below, we first load LAMMPS 
 simulation data stored as individual `dump*.txt` files for each frame, and 
 second, we calculate and plot the time-averaged radial pair distribution
```

### Comparing `amep-1.0.1/README.md` & `amep-1.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
 [![GitHub Discussions](https://img.shields.io/github/discussions/amepproject/amep)](https://github.com/amepproject/amep/discussions)
 ![Python Version from PEP 621 TOML](https://img.shields.io/python/required-version-toml?tomlFilePath=https%3A%2F%2Fraw.githubusercontent.com%2Famepproject%2Famep%2Fmain%2Fpyproject.toml)
 [![Static Badge](https://img.shields.io/badge/documentation-amepproject.de-blue)](https://amepproject.de)
 [![Pepy Total Downlods](https://img.shields.io/pepy/dt/amep?label=pypi%7Cdownloads)](https://pypi.org/project/amep/)
 [![Conda Downloads](https://img.shields.io/conda/d/conda-forge/amep)](https://anaconda.org/conda-forge/amep)
 [![GitHub Actions Workflow Status](https://img.shields.io/github/actions/workflow/status/amepproject/amep/test.yml?label=pipeline)](https://github.com/amepproject/amep/actions)
+[![Static Badge](https://img.shields.io/badge/arXiv-2404.16533-brown)](https://doi.org/10.48550/arXiv.2404.16533)
+
 
 <center><img src="https://raw.githubusercontent.com/amepproject/amep/main/doc/source/_static/images/amep-logo_v2.png" alt="amep logo" width="200" height="200"/></center>
 
 The **AMEP** (**A**ctive **M**atter **E**valuation **P**ackage) Python library 
 is a powerful tool for analyzing data from molecular-dynamics (MD), 
 Brownian-dynamics (BD), and continuum simulations. It comprises various 
 methods to analyze structural and dynamical properties of condensed matter 
@@ -140,14 +142,48 @@
 **AMEP** provides the possibility to animate plots and trajectories. 
 **To enable all animation features, FFmpeg must be installed on the device on** 
 **which you run AMEP**. FFmpeg is not automatically installed when you install 
 **AMEP**. Please visit [https://ffmpeg.org/download.html](https://ffmpeg.org/download.html) 
 to download FFmpeg and to get further information on how to install FFmpeg on your machine.
 
 
+# Citation
+
+If you use **AMEP** for a project that leads to a scientific publication, please acknowledge 
+the use of **AMEP** within the body of your publication for example by copying or adapting 
+the following formulation:
+
+*Data analysis for this publication utilized the AMEP library [1].*
+
+> [1] L. Hecht, K.-R. Dormann, K. L. Spanheimer, M. Ebrahimi, M. Cordts, S. Mandal, 
+>     A. K. Mukhopadhyay, and B. Liebchen, AMEP: The Active Matter Evaluation Package for Python, 
+>     *arXiv [Cond-Mat.Soft]* (2024). Available at: http://arxiv.org/abs/2404.16533.
+
+The pre-print is freely available on [arXiv](https://arxiv.org/abs/2404.16533). To cite this reference, 
+you can use the following BibTeX entry:
+
+```bibtex
+@misc{hecht2024amep,
+    title = {AMEP: The Active Matter Evaluation Package for Python}, 
+    author = {Lukas Hecht and 
+              Kay-Robert Dormann and 
+              Kai Luca Spanheimer and 
+              Mahdieh Ebrahimi and 
+              Malte Cordts and 
+              Suvendu Mandal and 
+              Aritra K. Mukhopadhyay and 
+              Benno Liebchen},
+    year = {2024},
+    eprint = {2404.16533},
+    archivePrefix = {arXiv},
+    primaryClass = {cond-mat.soft}
+}
+```
+
+
 # Getting started
 
 The following example briefly demonstrates the **AMEP** workflow. A typical 
 task is to calculate the average of an observable over several frames of the 
 simulation (time average). In the example below, we first load LAMMPS 
 simulation data stored as individual `dump*.txt` files for each frame, and 
 second, we calculate and plot the time-averaged radial pair distribution
```

### Comparing `amep-1.0.1/amep/__init__.py` & `amep-1.0.2/amep/__init__.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/_version.py` & `amep-1.0.2/amep/_version.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,8 +16,8 @@
 # along with this program.  If not, see <https://www.gnu.org/licenses/>.
 #
 # Contact: Lukas Hecht (lukas.hecht@pkm.tu-darmstadt.de)
 # =============================================================================
 """
 AMEP version number.
 """
-__version__ = "1.0.1"
+__version__ = "1.0.2"
```

### Comparing `amep-1.0.1/amep/base.py` & `amep-1.0.2/amep/base.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/cluster.py` & `amep-1.0.2/amep/cluster.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/continuum.py` & `amep-1.0.2/amep/continuum.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/evaluate.py` & `amep-1.0.2/amep/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -3798,43 +3798,49 @@
         self.__use_nojump = use_nojump
         
         if self.__nav is None:
             self.__nav = self.__traj.nframes
             
         # get reference frame at time t0:
         self.__frame0 = self.__traj[self.__nskip]
-
+        
         # check data availability
-        if self.__use_nojump and self.__traj[0].nojump_coords() is None:
-            raise ValueError(
-                'No nojump coordinates available. Call traj.nojump() '\
-                'to calculate the nojump coordinates.'
-            )
-        elif self.__pbc and self.__traj[0].unwrapped_coords() is None\
-        and self.__traj[0].nojump_coords() is None:
-            raise ValueError(
-                'Neither unwrapped nor nojump coordinates are available. '\
-                'Call traj.nojump() to calculate the nojump coordinates or '\
-                'do not apply periodic boundary conditions.'
-            )
-        else:
-            # get mode
-            if self.__use_nojump or\
-            (self.__pbc and self.__traj[0].unwrapped_coords() is None):
-                self.__mode = 'nojump'
-            elif self.__pbc and self.__traj[0].unwrapped_coords() is not None:
-                self.__mode = 'unwrapped'
+        if self.__pbc:
+            if self.__use_nojump:
+                try:
+                    a = self.__traj[0].nojump_coords()
+                except:
+                    raise ValueError(
+                        'No nojump coordinates available. Call traj.nojump() '\
+                        'to calculate the nojump coordinates.'
+                    )
             else:
-                self.__mode = 'normal'
-            # calculation
-            self.__frames, self.__avg, self.__indices = average_func(
-                self.__compute, self.__traj, skip=self.__skip,
-                nr=self.__nav, indices=True
-            )
-            self.__times = self.__traj.times[self.__indices]
+                try:
+                    a = self.__traj[0].unwrapped_coords()
+                except:
+                    raise ValueError(
+                        'There are no unwrapped coordinates available. '\
+                        'Please set use_nojump=True to use nojump coordinates '\
+                        'instead or do not apply periodic boundary conditions.'
+                    )
+        # get mode
+        if self.__pbc and self.__use_nojump:
+            self.__mode = 'nojump'
+        elif self.__pbc:
+            self.__mode = 'unwrapped'
+        else:
+            self.__mode = 'normal'
+
+        # calculation
+        self.__frames, self.__avg, self.__indices = average_func(
+            self.__compute, self.__traj, skip=self.__skip,
+            nr=self.__nav, indices=True
+        )
+        self.__times = self.__traj.times[self.__indices]
+
 
     def __compute(self, frame):
         r'''
         Calculation for a single frame.
 
         Parameters
         ----------
```

### Comparing `amep-1.0.1/amep/functions.py` & `amep-1.0.2/amep/functions.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/load.py` & `amep-1.0.2/amep/load.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/order.py` & `amep-1.0.2/amep/order.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/pbc.py` & `amep-1.0.2/amep/pbc.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/plot.py` & `amep-1.0.2/amep/plot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1422,15 +1422,15 @@
         trajectory: FieldTrajectory | ParticleTrajectory,
         outfile: Path | str, ptype: int | None = None,
         ftype: str | None = None, xlabel: str = '', ylabel: str = '',
         cbar_label: str = '', cbar: bool = True,
         formatter: Callable[[mpl.axes.Axes,], None] | None = None,
         painter: object | None = None,
         title: str = '', figsize: tuple[float, float] | None = None,
-        start: float = 0.0, stop: float = 1.0, nth: int = 1,
+        start: float = 0.0, stop: float = 1.0, nth: int = 1, fps: int = 10,
         verbose: bool = False, **kwargs) -> None:
     r'''Create a video from a trajectory.
 
     Quick video writeout. Just takes a trajectory and animates it.
     For further customization of videos, check the `amep.plot.create_video`
     method.
 
@@ -1486,14 +1486,16 @@
         Fraction of the trajectory at which to start animate the data. Must be
         smaller than `stop`. The default is 0.0.
     stop : float, optional
         Fraction of the trajectory at which to stop animate the data. Must be
         larger than `start`. The default is 1.0.
     nth : int, optional
         Use each nth frame to make the animate. The default is 1.
+    fps: int, optional
+        The frames per second of the video. The default is 10.
     verbose : bool, optional
         If True, runtime information is printed. The default is False.
     **kwargs
         All additional keyword arguments are forwared to `amep.plot.particles`
         if a ParticleTrajectory is provided and to `amep.plot.field` if a
         FieldTrajectory is provided.
 
@@ -1664,14 +1666,15 @@
         int(stop*trajectory.nframes),
         nth
     )
     anim = FuncAnimation(fig, animate, frames = indices)
     with tqdm(total = len(indices)) as pbar:
         anim.save(
             outfile,
+            fps = fps,
             progress_callback = lambda frameindex, nframes: pbar.update()
         )
     plt.close(fig)
 
 
 def create_video(
         fig: mpl.figure.Figure, update_frame_func: object,
```

### Comparing `amep-1.0.1/amep/reader.py` & `amep-1.0.2/amep/reader.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/spatialcor.py` & `amep-1.0.2/amep/spatialcor.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/statistics.py` & `amep-1.0.2/amep/statistics.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/styles/amep_latex.mplstyle` & `amep-1.0.2/amep/styles/amep_latex.mplstyle`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/styles/amep_standard.mplstyle` & `amep-1.0.2/amep/styles/amep_standard.mplstyle`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/thermo.py` & `amep-1.0.2/amep/thermo.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/timecor.py` & `amep-1.0.2/amep/timecor.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/trajectory.py` & `amep-1.0.2/amep/trajectory.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep/utils.py` & `amep-1.0.2/amep/utils.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/amep.egg-info/SOURCES.txt` & `amep-1.0.2/amep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/examples/continuum-example.py` & `amep-1.0.2/examples/continuum-example.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/examples/data/continuum/solver.py` & `amep-1.0.2/examples/data/continuum/solver.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/examples/particle-example.py` & `amep-1.0.2/examples/particle-example.py`

 * *Files identical despite different names*

### Comparing `amep-1.0.1/pyproject.toml` & `amep-1.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,46 +1,46 @@
 [project]
 name = "amep"
-version = "1.0.1"
+version = "1.0.2"
 license = {file="LICENSE"}
 authors = [
-	{name = "Lukas Hecht", email = "lukas.hecht@pkm.tu-darmstadt.de"},
+    {name = "Lukas Hecht", email = "lukas.hecht@pkm.tu-darmstadt.de"},
 ]
 description = "Active Matter Evaluation Package for data analysis of active matter simulations"
 readme = "README.md"
 requires-python = ">=3.10"
 keywords = [
     "active matter",
     "soft matter",
     "physics",
     "data analysis",
     "computational physics",
 ]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
-	"Intended Audience :: Science/Research",
-	"Intended Audience :: Education",
-	"License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
-	"Natural Language :: English",
-	"Operating System :: OS Independent",
-	"Programming Language :: Python :: 3",
-	"Programming Language :: Python :: 3.10",
+    "Intended Audience :: Science/Research",
+    "Intended Audience :: Education",
+    "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
-	"Topic :: Scientific/Engineering :: Physics",
-	"Topic :: Scientific/Engineering :: Visualization",
+    "Topic :: Scientific/Engineering :: Physics",
+    "Topic :: Scientific/Engineering :: Visualization",
 ]
 dependencies = [
-	"h5py >= 3.7.0",
-	"matplotlib >= 3.6.2",
-	"numba >= 0.56.4",
-	"numpy >= 1.21.6",
-	"scipy >= 1.10.0",
-	"scikit-image >= 0.20.0",
-	"tqdm >= 4.65.0"
+    "h5py >= 3.7.0",
+    "matplotlib >= 3.6.2",
+    "numba >= 0.56.4",
+    "numpy >= 1.21.6",
+    "scipy >= 1.10.0",
+    "scikit-image >= 0.20.0",
+    "tqdm >= 4.65.0"
 ]
 
 [project.urls]
 "Homepage" = "https://amepproject.de/"
 "Issues" = "https://github.com/amepproject/amep/issues"
 "Repository" = "https://github.com/amepproject/amep"
 "Documentation" = "https://amepproject.de/"
```

