# Comparing `tmp/spyral_utils-0.3.0.tar.gz` & `tmp/spyral_utils-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spyral_utils-0.3.0.tar", last modified: Fri Mar  8 16:39:25 2024, max compression
+gzip compressed data, was "spyral_utils-1.0.0.tar", last modified: Wed May 22 13:50:19 2024, max compression
```

## Comparing `spyral_utils-0.3.0.tar` & `spyral_utils-1.0.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/LICENSE.txt
--rw-r--r--   0        0        0     3984 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/README.md
--rw-r--r--   0        0        0      767 2024-03-08 16:39:25.033353 spyral_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      253 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/__init__.py
--rw-r--r--   0        0        0     1470 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/constants.py
--rw-r--r--   0        0        0      374 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/nuclear/__init__.py
--rw-r--r--   0        0        0    58326 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/nuclear/amdc_2020.txt
--rw-r--r--   0        0        0     4229 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/nuclear/nuclear_map.py
--rw-r--r--   0        0        0     2226 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/nuclear/particle_id.py
--rw-r--r--   0        0        0    14570 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/nuclear/target.py
--rw-r--r--   0        0        0      276 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/plot/__init__.py
--rw-r--r--   0        0        0     8350 2024-03-08 16:39:13.413240 spyral_utils-0.3.0/src/spyral_utils/plot/cut.py
--rw-r--r--   0        0        0    15447 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/src/spyral_utils/plot/histogram.py
--rw-r--r--   0        0        0        0 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0      150 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/cut.json
--rw-r--r--   0        0        0      106 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/gas_target.json
--rw-r--r--   0        0        0      345 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/pid.json
--rw-r--r--   0        0        0      106 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/solid_target.json
--rw-r--r--   0        0        0      594 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/test_cut.py
--rw-r--r--   0        0        0      187 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/test_nuclear_map.py
--rw-r--r--   0        0        0      546 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/test_pid.py
--rw-r--r--   0        0        0     1309 2024-03-08 16:39:13.417240 spyral_utils-0.3.0/tests/test_target.py
--rw-r--r--   0        0        0     4468 1970-01-01 00:00:00.000000 spyral_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-05-22 13:50:03.684432 spyral_utils-1.0.0/LICENSE.txt
+-rw-r--r--   0        0        0     3906 2024-05-22 13:50:03.684432 spyral_utils-1.0.0/README.md
+-rw-r--r--   0        0        0      767 2024-05-22 13:50:19.052601 spyral_utils-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0      253 2024-05-22 13:50:03.684432 spyral_utils-1.0.0/src/spyral_utils/__init__.py
+-rw-r--r--   0        0        0     1470 2024-05-22 13:50:03.684432 spyral_utils-1.0.0/src/spyral_utils/constants.py
+-rw-r--r--   0        0        0      526 2024-05-22 13:50:03.684432 spyral_utils-1.0.0/src/spyral_utils/nuclear/__init__.py
+-rw-r--r--   0        0        0    58326 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/nuclear/amdc_2020.txt
+-rw-r--r--   0        0        0     4435 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/nuclear/nuclear_map.py
+-rw-r--r--   0        0        0     2226 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/nuclear/particle_id.py
+-rw-r--r--   0        0        0    14570 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/nuclear/target.py
+-rw-r--r--   0        0        0      276 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/plot/__init__.py
+-rw-r--r--   0        0        0     8350 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/plot/cut.py
+-rw-r--r--   0        0        0    15563 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/src/spyral_utils/plot/histogram.py
+-rw-r--r--   0        0        0        0 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0      150 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/cut.json
+-rw-r--r--   0        0        0      106 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/gas_target.json
+-rw-r--r--   0        0        0      345 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/pid.json
+-rw-r--r--   0        0        0      106 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/solid_target.json
+-rw-r--r--   0        0        0      594 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/test_cut.py
+-rw-r--r--   0        0        0      187 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/test_nuclear_map.py
+-rw-r--r--   0        0        0      482 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/test_pid.py
+-rw-r--r--   0        0        0     1270 2024-05-22 13:50:03.688432 spyral_utils-1.0.0/tests/test_target.py
+-rw-r--r--   0        0        0     4390 1970-01-01 00:00:00.000000 spyral_utils-1.0.0/PKG-INFO
```

### Comparing `spyral_utils-0.3.0/LICENSE.txt` & `spyral_utils-1.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/README.md` & `spyral_utils-1.0.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 # spyral-utils
 
-![testing workflow](https://github.com/gwm17/spyral-utils/actions/workflows/test-actions.yml/badge.svg)
+![testing workflow](https://github.com/ATTPC/spyral-utils/actions/workflows/test-actions.yml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/spyral-utils.svg)](https://pypi.python.org/pypi/spyral-utils/)
 [![PyPI license](https://img.shields.io/pypi/l/spyral-utils.svg)](https://pypi.python.org/pypi/spyral-utils/)
 
-spyral-utils is a utility library that contains some of the  core functionality of [Spyral](https://github.com/turinath/Spyral.git). These utilities were found to be useful not just within Spyral but also continuing analysis after using Spyral. Some key utilities include:
+spyral-utils is a utility library that contains some of the  core functionality of [Spyral](https://github.com/ATTPC/Spyral.git). These utilities were found to be useful not just within Spyral but also continuing analysis after using Spyral. Some key utilities include:
 
 - Nuclear masses from the AMDC AME 2020 masses
 - Some histogramming and gating/cuting tools that are plotting backend agnostic
 - Energy loss analysis for gas and solid targets using pycatima
 - 4-vector analysis through the vector package
 
-spyral-utils is still in very early development, so all mileage may vary!
-
-See the [documentation](https://gwm17.github.io/spyral-utils/) for more details.
+See the [documentation](https://attpc.github.io/spyral-utils/) for more details.
 
 ## Installation
 
 spyral-utils can be installed using `pip install spyral-utils`
 
 ## System requirements
 
 spyral-utils requires Python >= 3.10 and  < 3.13
 
-spyral-utils is cross-platform and tested for MacOS 13, Windows 11, and Ubuntu 22.04.
+spyral-utils is cross-platform and tested for MacOS 14, Windows 11, and Ubuntu 22.04.
 
 ## Formats
 
 Several parts of the utilities allow for saving and creating objects from JSON. Below is an outline of the expected formats for each of these
 
 ### Targets
```

### Comparing `spyral_utils-0.3.0/pyproject.toml` & `spyral_utils-1.0.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "spyral-utils"
-version = "0.3.0"
+version = "1.0.0"
 description = "A collection of useful utilities for the Spyral analysis framework"
 authors = [
     { name = "Gordon McCann", email = "mccann@frib.msu.edu" },
     { name = "Nathan Turi", email = "turi@frib.msu.edu" },
 ]
 dependencies = [
     "numpy>=1.26.0, <2.0",
```

### Comparing `spyral_utils-0.3.0/src/spyral_utils/constants.py` & `spyral_utils-1.0.0/src/spyral_utils/constants.py`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/src/spyral_utils/nuclear/amdc_2020.txt` & `spyral_utils-1.0.0/src/spyral_utils/nuclear/amdc_2020.txt`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/src/spyral_utils/nuclear/nuclear_map.py` & `spyral_utils-1.0.0/src/spyral_utils/nuclear/nuclear_map.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,17 +11,19 @@
 
 Functions
 ---------
 generate_nucleus_id(z: int, a: int) -> int:
     get a unqiue nucleus id
 """
 
-from dataclasses import dataclass
 from ..constants import AMU_2_MEV, ELECTRON_MASS_U
+
+from dataclasses import dataclass
 from pathlib import Path
+from importlib.resources import files, as_file
 
 DATA_PATH: Path = Path(__file__).parent.resolve() / "amdc_2020.txt"
 
 
 @dataclass
 class NucleusData:
     """Nucleus data from AME dataclass
@@ -117,29 +119,32 @@
     get_data(z: int, a: int) -> NucleusData
         retrieve the mass data for a given nucleus
     """
 
     def __init__(self):
         self.map = {}
 
-        with open(DATA_PATH) as data_file:
+        data_handle = files("spyral_utils.nuclear").joinpath("amdc_2020.txt")
+        with as_file(data_handle) as data_path:
+            data_file = open(data_path, "r")
             data_file.readline()  # Header
             for line in data_file:
                 entries = line.split()
                 data = NucleusData()
                 data.Z = int(entries[0])  # Column 1: Z
                 data.A = int(entries[1])  # Column 2: A
                 data.element_symbol = entries[2]  # Column 3: Element
                 data.atomic_mass = float(entries[3])
                 data.mass = (
                     float(entries[3]) - float(data.Z) * ELECTRON_MASS_U
                 ) * AMU_2_MEV  # Remove electron masses to obtain nuclear masses, Column 4
                 data.isotopic_symbol = f"{data.A}{entries[2]}"
                 data.pretty_iso_symbol = f"<sup>{data.A}</sup>{entries[2]}"
                 self.map[generate_nucleus_id(data.Z, data.A)] = data
+            data_file.close()
 
     def get_data(self, z: int, a: int) -> NucleusData:
         """retrieve the mass data for a given nucleus
 
         Parameters
         ----------
         z: int
```

### Comparing `spyral_utils-0.3.0/src/spyral_utils/nuclear/particle_id.py` & `spyral_utils-1.0.0/src/spyral_utils/nuclear/particle_id.py`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/src/spyral_utils/nuclear/target.py` & `spyral_utils-1.0.0/src/spyral_utils/nuclear/target.py`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/src/spyral_utils/plot/cut.py` & `spyral_utils-1.0.0/src/spyral_utils/plot/cut.py`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/src/spyral_utils/plot/histogram.py` & `spyral_utils-1.0.0/src/spyral_utils/plot/histogram.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 Classes
 -------
 Hist1D
     A 1-D histogram dataclass. Should not be instantiated directly
 Hist2D
     A 2-D histogram dataclass. Should not be instantiated directly
 Histogrammer
-    A parent object used to create, manage, draw histograms
+    A parent object used to create, manage histograms
 """
 
 import numpy as np
 from numpy.typing import NDArray
 from dataclasses import dataclass
 from math import floor
 
@@ -108,15 +108,15 @@
         mean = np.average(
             self.bins[bin_min:bin_max], weights=self.counts[bin_min:bin_max]
         )
         variance = np.average(
             (self.bins[bin_min:bin_max] - mean) ** 2.0,
             weights=self.counts[bin_min:bin_max],
         )
-        return (integral, mean, np.sqrt(variance))
+        return (integral, mean, np.sqrt(variance))  # type: ignore
 
     def get_subrange(
         self, xrange: tuple[float, float]
     ) -> tuple[np.ndarray, np.ndarray]:
         """Get a subrange of the histogram
 
         Parameters
@@ -125,15 +125,15 @@
             the subrange of the histogram (min, max) in x-coordinates
 
         Returns
         -------
         tuple[ndarray, ndarray]
             the subrange (bin edges, counts)
         """
-        mask = np.logical_and(self.bins > xrange[0], self.bins < xrange[1])
+        mask = np.logical_and(self.bins >= xrange[0], self.bins < xrange[1])
         return (self.bins[mask], self.counts[mask[:-1]])
 
 
 @dataclass
 class Hist2D:
     """Dataclass wrapping a numpy array used to store two-dimensional histogram data and retrieve histogram statistics
 
@@ -212,14 +212,16 @@
             Returns a tuple of (integral, x mean, y mean, x std. dev., y std. dev.) for the subrange, or None if the subrange is not within the histogram bounds
 
         """
         clamped_x_range = clamp_range(xrange, (self.x_bins.min(), self.x_bins.max()))
         clamped_y_range = clamp_range(yrange, (self.y_bins.min(), self.y_bins.max()))
         bin_min = self.get_bin((clamped_x_range[0], clamped_y_range[0]))
         bin_max = self.get_bin((clamped_x_range[1], clamped_y_range[1]))
+        if bin_min == None or bin_max == None:
+            return None
 
         x_bin_range = np.arange(start=bin_min[0], stop=bin_max[0], step=1)
         y_bin_range = np.arange(start=bin_min[1], stop=bin_max[1], step=1)
         bin_mesh = np.ix_(y_bin_range, x_bin_range)
 
         integral = np.sum(self.counts[bin_mesh])
         mean_x = np.average(
@@ -234,15 +236,15 @@
             (self.x_bins[bin_min[0] : bin_max[0]] - mean_x) ** 2.0,
             weights=np.sum(self.counts.T[bin_min[0] : bin_max[0]], 1),
         )
         var_y = np.average(
             (self.y_bins[bin_min[1] : bin_max[1]] - mean_y) ** 2.0,
             weights=np.sum(self.counts[bin_min[1] : bin_max[1]], 1),
         )
-        return (integral, mean_x, mean_y, np.sqrt(var_x), np.sqrt(var_y))
+        return (integral, mean_x, mean_y, np.sqrt(var_x), np.sqrt(var_y))  # type: ignore
 
     def get_subrange(
         self, xrange: tuple[float, float], yrange: tuple[float, float]
     ) -> tuple[np.ndarray, np.ndarray, np.ndarray]:
         """Get a subrange of the histogram
 
         Parameters
@@ -253,16 +255,16 @@
             the subrange of the histogram (min, max) in y-coordinates
 
         Returns
         -------
         tuple[ndarray, ndarray, ndarray]
             the subrange (x bin edges, y bin edges, counts)
         """
-        x_mask = np.logical_and(self.x_bins > xrange[0], self.x_bins < xrange[1])
-        y_mask = np.logical_and(self.y_bins > yrange[0], self.y_bins < yrange[1])
+        x_mask = np.logical_and(self.x_bins >= xrange[0], self.x_bins < xrange[1])
+        y_mask = np.logical_and(self.y_bins >= yrange[0], self.y_bins < yrange[1])
         bin_mesh = np.ix_(y_mask, x_mask)
         return (self.x_bins[x_mask], self.y_bins[y_mask], self.counts[bin_mesh])
 
 
 class Histogrammer:
     """Histogrammer is a wrapper around a dictionary of str->Hist1D|Hist2D that interfaces with matplotlib
 
@@ -400,15 +402,15 @@
         if name not in self.histograms:
             return False
 
         hist = self.histograms[name]
         if type(hist) is not Hist2D:
             return False
         counts, _, _ = np.histogram2d(
-            x_data.flatten(), y_data.flatten(), bins=(hist.x_bins, hist.y_bins)
+            x_data.flatten(), y_data.flatten(), bins=(hist.x_bins, hist.y_bins)  # type: ignore
         )
         hist.counts += counts.T
         return True
 
     def get_hist1d(self, name: str) -> Hist1D | None:
         """Retrieve a Hist1D by name
```

### Comparing `spyral_utils-0.3.0/tests/test_cut.py` & `spyral_utils-1.0.0/tests/test_cut.py`

 * *Files identical despite different names*

### Comparing `spyral_utils-0.3.0/tests/test_target.py` & `spyral_utils-1.0.0/tests/test_target.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,8 @@
-from spyral_utils.nuclear.target import load_target, GasTarget, SolidTarget
-from spyral_utils.nuclear import NuclearDataMap
+from spyral_utils.nuclear import load_target, GasTarget, SolidTarget, NuclearDataMap
 from pathlib import Path
 import numpy as np
 
 GAS_TARGET_PATH: Path = Path(__file__).parent.resolve() / "gas_target.json"
 SOLID_TARGET_PATH: Path = Path(__file__).parent.resolve() / "solid_target.json"
 PROJ_Z: int = 1
 PROJ_A: int = 1
```

### Comparing `spyral_utils-0.3.0/PKG-INFO` & `spyral_utils-1.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 Metadata-Version: 2.1
 Name: spyral-utils
-Version: 0.3.0
+Version: 1.0.0
 Summary: A collection of useful utilities for the Spyral analysis framework
 Author-Email: Gordon McCann <mccann@frib.msu.edu>, Nathan Turi <turi@frib.msu.edu>
 License: GPLv3
 Requires-Python: <3.13,>=3.10
 Requires-Dist: numpy<2.0,>=1.26.0
 Requires-Dist: scipy>=1.11.3
 Requires-Dist: polars>=0.19.12
 Requires-Dist: pycatima>=1.90
 Requires-Dist: shapely>=2.0.2
 Requires-Dist: vector>=1.3.0
 Description-Content-Type: text/markdown
 
 # spyral-utils
 
-![testing workflow](https://github.com/gwm17/spyral-utils/actions/workflows/test-actions.yml/badge.svg)
+![testing workflow](https://github.com/ATTPC/spyral-utils/actions/workflows/test-actions.yml/badge.svg)
 [![PyPI version shields.io](https://img.shields.io/pypi/v/spyral-utils.svg)](https://pypi.python.org/pypi/spyral-utils/)
 [![PyPI license](https://img.shields.io/pypi/l/spyral-utils.svg)](https://pypi.python.org/pypi/spyral-utils/)
 
-spyral-utils is a utility library that contains some of the  core functionality of [Spyral](https://github.com/turinath/Spyral.git). These utilities were found to be useful not just within Spyral but also continuing analysis after using Spyral. Some key utilities include:
+spyral-utils is a utility library that contains some of the  core functionality of [Spyral](https://github.com/ATTPC/Spyral.git). These utilities were found to be useful not just within Spyral but also continuing analysis after using Spyral. Some key utilities include:
 
 - Nuclear masses from the AMDC AME 2020 masses
 - Some histogramming and gating/cuting tools that are plotting backend agnostic
 - Energy loss analysis for gas and solid targets using pycatima
 - 4-vector analysis through the vector package
 
-spyral-utils is still in very early development, so all mileage may vary!
-
-See the [documentation](https://gwm17.github.io/spyral-utils/) for more details.
+See the [documentation](https://attpc.github.io/spyral-utils/) for more details.
 
 ## Installation
 
 spyral-utils can be installed using `pip install spyral-utils`
 
 ## System requirements
 
 spyral-utils requires Python >= 3.10 and  < 3.13
 
-spyral-utils is cross-platform and tested for MacOS 13, Windows 11, and Ubuntu 22.04.
+spyral-utils is cross-platform and tested for MacOS 14, Windows 11, and Ubuntu 22.04.
 
 ## Formats
 
 Several parts of the utilities allow for saving and creating objects from JSON. Below is an outline of the expected formats for each of these
 
 ### Targets
```

