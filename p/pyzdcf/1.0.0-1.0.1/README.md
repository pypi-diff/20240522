# Comparing `tmp/pyzdcf-1.0.0.tar.gz` & `tmp/pyzdcf-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyzdcf-1.0.0.tar", max compression
+gzip compressed data, was "pyzdcf-1.0.1.tar", max compression
```

## Comparing `pyzdcf-1.0.0.tar` & `pyzdcf-1.0.1.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-10-26 10:01:06.636430 pyzdcf-1.0.0/LICENSE
--rw-r--r--   0        0        0    11484 2022-10-26 12:20:18.743027 pyzdcf-1.0.0/README.md
--rw-r--r--   0        0        0      953 2022-10-26 13:37:46.350078 pyzdcf-1.0.0/pyproject.toml
--rw-r--r--   0        0        0       27 2022-10-17 10:15:29.543744 pyzdcf-1.0.0/pyzdcf/__init__.py
--rw-r--r--   0        0        0    32082 2022-10-26 10:26:17.572329 pyzdcf-1.0.0/pyzdcf/pyzdcf.py
--rw-r--r--   0        0        0    12654 2022-10-26 13:59:02.149977 pyzdcf-1.0.0/setup.py
--rw-r--r--   0        0        0    12545 2022-10-26 13:59:02.151532 pyzdcf-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-05-20 05:09:43.593445 pyzdcf-1.0.1/LICENSE
+-rw-r--r--   0        0        0    12615 2024-05-20 05:09:43.593445 pyzdcf-1.0.1/README.md
+-rw-r--r--   0        0        0      939 2024-05-22 05:04:53.718162 pyzdcf-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0       27 2024-05-20 05:09:43.597445 pyzdcf-1.0.1/pyzdcf/__init__.py
+-rw-r--r--   0        0        0    32082 2024-05-20 05:09:43.597445 pyzdcf-1.0.1/pyzdcf/pyzdcf.py
+-rw-r--r--   0        0        0    13764 1970-01-01 00:00:00.000000 pyzdcf-1.0.1/PKG-INFO
```

### Comparing `pyzdcf-1.0.0/LICENSE` & `pyzdcf-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyzdcf-1.0.0/README.md` & `pyzdcf-1.0.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,35 @@
 # pyZDCF
 
-## Description
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7253034.svg)](https://doi.org/10.5281/zenodo.7253034)
+[![pypi](https://img.shields.io/pypi/v/pyzdcf)](https://pypi.org/project/pyzdcf/)
+[![Documentation Status](https://readthedocs.org/projects/pyzdcf/badge/?version=latest)](https://pyzdcf.readthedocs.io/en/latest/?badge=latest)
+![](https://img.shields.io/pypi/pyversions/pyzdcf?color=gree)
 
 **pyZDCF** is a Python module that emulates a widely used Fortran program called ZDCF (Z-transformed Discrete Correlation Function, [Alexander 1997](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)). It is used for robust estimation of cross-correlation function of sparse and unevenly sampled astronomical time-series. This Python implementation also introduces sparse matrices in order to significantly reduce RAM usage when running the code on large time-series (> 3000 points).
 
 pyZDCF is based on the original Fortran code fully developed by 
 Prof. Tal Alexander from Weizmann Institute of Science, Israel 
-(see Acknowledgements and References for details and further reading).
+(see [Acknowledgements](#ackn) and [References](#ref) for details and further reading).
+
+Full docs with examples: [pyzdcf.readthedocs.io](https://pyzdcf.readthedocs.io/)
 
 ## Motivation
 
 Development of pyZDCF module was motivated by the long and successful usage of 
 the original ZDCF Fortran code in the analysis of light curves of active galactic
 nuclei by our research group (see [Kovacevic et al. 2014](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract), [Shapovalova et al. 2019](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract), and reference therein). One of the science cases we investigate is photometric reverberation mapping in the context of Legacy Survey of Space and Time (LSST) survey strategies (see [Jankov et al. 2022](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)). However, this module is **general** and is meant to be used for cross-correlation of spectroscopic or photometric light curves, same as the original Fortran version.
 
+## Installation
+
+pyZDCF can be installed using pip:
+
+```sh
+pip install pyzdcf
+```
 
 ### Dependencies
 >```
 >python = ">=3.8,<3.11"
 >numpy = ">=1.16.5,<1.23.0"
 >pandas = "^1.3"
 >scipy = "^1.7.3"
@@ -58,15 +70,15 @@
 - `uniform_sampling` - if ``True``, set flag to perform uniform sampling of the light curve.
 - `omit_zero_lags` - if True, omit zero lag points.
 - `minpts` - minimal number of points per bin.
 - `num_MC` - number of Monte Carlo simulations for error estimation.
 - `lc1_name` - Name of the first light curve file
 - `lc2_name` - Name of the second light curve file (required only if we do cross-correlation)
 
-For more information on the correct syntax, see "Running the code" subsection and the "API Documentation" section.
+For more information on the correct syntax, see "Running the code" subsection.
 
 
 ### Output
 
 The return value of the `pyzdcf` function is a `pandas.DataFrame` object displaying the results in 7 columns:
 
 ```
@@ -138,35 +150,37 @@
 - For more examples see [example notebook](https://github.com/LSST-sersag/pyzdcf/blob/main/notebooks/examples.ipynb).
 
 - Additionally, you can also check out code description of the original Fortran version because the majority of input parameters and all output files are the same as in pyZDCF. You can download the fortran source code [here](https://www.weizmann.ac.il/particle/tal/research-activities/software).
 
 
 ## Features
 
-* Added an option to use **sparse matrix implementation** for reduced RAM usage when working with long light curves (>3000 points);
+* **Sparse matrix implementation** for reduced RAM usage when working with long light curves (>3000 points);
 > The main benefit is that we can now run these demanding calculations on our own personal computers (8 GB of RAM is enough for
 > light curves containing up to 15000 points), making the usage of this algorithm more convinient than ever.
 > 
 > You can turn this on/off by specifying `sparse` keyword argument to `True` or `False`. Default value is `'auto'`, where sparse marices are utilized when there are more than 3000 points per light curve. Note that by reducing RAM usage, we pay in increased program running time.
 
 * **Interactive mode**: program specifically asks the user to provide necessary parameters (similar to original Fortran version);
 * **Manual mode**: user can provide all parameters in one dictionary.
+* **Fixed bugs** from original ZDCF (v2.3) written in Fortran 95.
 
+The module was tested (i.e., compared with original ZDCF v2.3 output, with fixed bugs) for various parameter combinations on a set of 100 AGN light curve candidates (*g* and *r* bands). The list of object ids and coordinates was taken from a combined catalogue of known AGNs ([Sánchez-Sáez et al. 2021](https://ui.adsabs.harvard.edu/abs/2021AJ....162..206S/abstract)).
 
 ## License
 
 Distributed under the MIT License.
 
 ## Contact
 
->**Isidora Jankov (main)** - isidora_jankov@matf.bg.ac.rs  
+>**Isidora Jankov (main)** - ijankov@proton.me  
 >Andjelka Kovačević - andjelka@matf.bg.ac.rs  
 >Dragana Ilić - dilic@matf.bg.ac.rs
 
-You can write to us:
+You are welcome to write to us:
 - if there are any problems running the code on your system;
 - suggestions for code improvements.
 
 If you want to report a bug, please open an Issue on GitHub: [https://github.com/LSST-sersag/pyzdcf](https://github.com/LSST-sersag/pyzdcf).
 
 
 ## Citation
@@ -189,22 +203,23 @@
   doi          = {10.5281/zenodo.7253034},
   url          = {https://doi.org/10.5281/zenodo.7253034}
 }
 ```
 
 For other citation formats see: [https://doi.org/10.5281/zenodo.7253034](https://doi.org/10.5281/zenodo.7253034)
 
-## Acknowledgments
+## <a name="ackn" />Acknowledgments
 
 * The pyZDCF module is based on the original Fortran code developed by Prof. Tal Alexander (Weizmann Institute of Science, Israel). Download Fortran version from professor's [page](https://www.weizmann.ac.il/particle/tal/research-activities/software).  
 * For theoretical details regarding the ZDCF algorithm see this publication: [Alexander, T. (1997)](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract).  
 * Huge thanks to my closest collegues and mentors Dr. Andjelka Kovačević and Dr. Dragana Ilić, as well as to Dr. Paula Sánchez-Sáez and Dr. Robert Nikutta for invaluable input during the development and testing of this python module.  
 * Many thanks to Prof. Eli Waxman, Amir Bar On and former students of Prof. Tal Alexander for their kind assistance regarding the development of pyZDCF module and its acknowledgment as part of the legacy behind late Prof. Alexander.
 
-## References
+## <a name="ref" />References
 * [Alexander, T. 1997, in: Astronomical Time Series, eds. D. Maoz, A. Sternberg, & E. M. Leibowitz, Vol. 218, Springer, Is AGN Variability Correlated with Other AGN Properties? ZDCF Analysis of Small Samples of Sparse Light Curves](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)
 * [Jankov, I.; Kovačević A. B.; Ilić, D.; et al. 2022, Astronomische Nachrichten, 343, e210090](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)
 * [Kovačević, A.; Popović, L. Č.; Shapovalova, A. I.; et al. 2014, Advances in Space Research, 54, 1414-1428](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract)
+* [Sánchez-Sáez, P.; Lira, H.; Martí, L.; et al. 2021,The Astronomical Journal, 162, id.206](https://ui.adsabs.harvard.edu/abs/2021AJ....162..206S/abstract)
 * [Shapovalova, A. I.; Popović, L. Č.; Afanasiev, V. L.; et al. 2019, MNRAS, 485, 4790-4803](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract)
```

### Comparing `pyzdcf-1.0.0/pyproject.toml` & `pyzdcf-1.0.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyzdcf"
-version = "1.0.0"
+version = "1.0.1"
 description = "Python module used for robust estimation of cross-corelation functions of sparse and unevenly sampled astronomical time-series. It emulates a Fortran program called ZDCF which is based on the Z-transformed Discrete Correlation Function algorithm (ZDCF, Alexander 1997)."
 authors = ["Isidora Jankov <isidora_jankov@matf.bg.ac.rs>"]
 readme = "README.md"
 license = "MIT"
 
 classifiers = [
 "License :: OSI Approved :: MIT License",
@@ -16,16 +16,16 @@
 include = [
 "LICENSE",
 ]
 
 repository = "https://github.com/LSST-sersag/pyzdcf"
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-numpy = ">=1.16.5,<1.23.0"
+python = ">=3.8"
+numpy = ">=1.16.5"
 pandas = "^1.3"
 scipy = "^1.7.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.0"
 
 [build-system]
```

### Comparing `pyzdcf-1.0.0/pyzdcf/pyzdcf.py` & `pyzdcf-1.0.1/pyzdcf/pyzdcf.py`

 * *Files identical despite different names*

### Comparing `pyzdcf-1.0.0/setup.py` & `pyzdcf-1.0.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,250 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pyzdcf
+Version: 1.0.1
+Summary: Python module used for robust estimation of cross-corelation functions of sparse and unevenly sampled astronomical time-series. It emulates a Fortran program called ZDCF which is based on the Z-transformed Discrete Correlation Function algorithm (ZDCF, Alexander 1997).
+Home-page: https://github.com/LSST-sersag/pyzdcf
+License: MIT
+Author: Isidora Jankov
+Author-email: isidora_jankov@matf.bg.ac.rs
+Requires-Python: >=3.8
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Topic :: Scientific/Engineering :: Astronomy
+Requires-Dist: numpy (>=1.16.5)
+Requires-Dist: pandas (>=1.3,<2.0)
+Requires-Dist: scipy (>=1.7.3,<2.0.0)
+Project-URL: Repository, https://github.com/LSST-sersag/pyzdcf
+Description-Content-Type: text/markdown
+
+# pyZDCF
+
+[![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7253034.svg)](https://doi.org/10.5281/zenodo.7253034)
+[![pypi](https://img.shields.io/pypi/v/pyzdcf)](https://pypi.org/project/pyzdcf/)
+[![Documentation Status](https://readthedocs.org/projects/pyzdcf/badge/?version=latest)](https://pyzdcf.readthedocs.io/en/latest/?badge=latest)
+![](https://img.shields.io/pypi/pyversions/pyzdcf?color=gree)
+
+**pyZDCF** is a Python module that emulates a widely used Fortran program called ZDCF (Z-transformed Discrete Correlation Function, [Alexander 1997](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)). It is used for robust estimation of cross-correlation function of sparse and unevenly sampled astronomical time-series. This Python implementation also introduces sparse matrices in order to significantly reduce RAM usage when running the code on large time-series (> 3000 points).
+
+pyZDCF is based on the original Fortran code fully developed by 
+Prof. Tal Alexander from Weizmann Institute of Science, Israel 
+(see [Acknowledgements](#ackn) and [References](#ref) for details and further reading).
+
+Full docs with examples: [pyzdcf.readthedocs.io](https://pyzdcf.readthedocs.io/)
+
+## Motivation
+
+Development of pyZDCF module was motivated by the long and successful usage of 
+the original ZDCF Fortran code in the analysis of light curves of active galactic
+nuclei by our research group (see [Kovacevic et al. 2014](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract), [Shapovalova et al. 2019](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract), and reference therein). One of the science cases we investigate is photometric reverberation mapping in the context of Legacy Survey of Space and Time (LSST) survey strategies (see [Jankov et al. 2022](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)). However, this module is **general** and is meant to be used for cross-correlation of spectroscopic or photometric light curves, same as the original Fortran version.
+
+## Installation
+
+pyZDCF can be installed using pip:
+
+```sh
+pip install pyzdcf
+```
+
+### Dependencies
+>```
+>python = ">=3.8,<3.11"
+>numpy = ">=1.16.5,<1.23.0"
+>pandas = "^1.3"
+>scipy = "^1.7.3"
+>```
+
+## How to use
+
+### Input files
+This code requires user-provided plain text files as input. CSV files are 
+accepted by default, but you can use any other delimited file, as long as you
+provide the `sep` keyword argument when calling `pyzdcf` function. The input
+light curve file should be in 3 columns: time (ordered), flux/magnitude and
+absolute error on flux/magnitude. Make sure to exclude the header (column
+names) from the input files.
+
+First few lines of the example input file accepted by default (CSV):
+
+```
+0.0,0.9594479339474323,0.0019188958678948648
+1.0,0.9588196871078336,0.0019176393742156672
+2.0,0.9637198686651904,0.0019274397373303808
+3.0,0.9622807967282166,0.0019245615934564328
+```
+
+**NOTE:** pyZDCF is tested only with input files having whole numbers (integers) for time column. If you have decimal numbers (e.g., you have a light curve with several measurments in the same night expressed as fractions of a day instead of minutes), just convert them into a time format with integer values (e.g., minutes instead of days). On the other hand, you could round the values from the same day (e.g. 5.6 --> 5, 5.8 --> 5, etc.) and the algorithm will take in the information and average the flux for that day. 
+
+### Input parameters
+
+If you use interactive mode (`intr = True`), then pyZDCF will ask you to
+enter all input parametars interactively, similarly to original ZDCF interface.
+There is also a manual mode (`intr = False`) where you can provide input
+parameters using a dictionary and passing it to `parameters` keyword argument.
+
+Available input parameters (keys in the `parameters` dictionary) are:
+
+- `autocf` - if ``True``, perform auto-correlation, otherwise do the cross-correlation.
+- `prefix` - provide a name for the output file.
+- `uniform_sampling` - if ``True``, set flag to perform uniform sampling of the light curve.
+- `omit_zero_lags` - if True, omit zero lag points.
+- `minpts` - minimal number of points per bin.
+- `num_MC` - number of Monte Carlo simulations for error estimation.
+- `lc1_name` - Name of the first light curve file
+- `lc2_name` - Name of the second light curve file (required only if we do cross-correlation)
+
+For more information on the correct syntax, see "Running the code" subsection.
+
+
+### Output
+
+The return value of the `pyzdcf` function is a `pandas.DataFrame` object displaying the results in 7 columns:
+
+```
++---+-------+-------------+-------------+--------------+-------------+-------------+------+
+|   |   tau |   -sig(tau) |   +sig(tau) |          dcf |   -err(dcf) |   +err(dcf) | #bin |
+|---+-------+-------------+-------------+--------------+-------------+-------------+------|
+| 0 |  -991 |           4 |           0 |  0.13598     |  0.361559   |  0.342224   |   10 |
+| 1 |  -988 |           2 |           0 | -0.217733    |  0.279988   |  0.301034   |   13 |
+| 2 |  -985 |           2 |           0 | -0.0614938   |  0.266546   |  0.27135    |   16 |
+| 3 |  -982 |           2 |           0 |  0.239601    |  0.237615   |  0.223317   |   19 |
+| 4 |  -979 |           2 |           0 |  0.331415    |  0.208171   |  0.192523   |   22 |
+```
+The columns are: time-lag, negative time-lag std, positive time-lag std, zdcf,
+negative zdcf sampling error, positive zdcf sampling error, number of points 
+per bin. For more information on how these values are calculated see 
+[Alexander 1997](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract).
+
+The code will also generate an output .dcf file file in a specified folder on your computer with same 7 columns containing the results. It is allowed to name these files however you want using the `prefix` parameter (see example in the next subsection).
+
+Optionally, by adding keyword argument `savelc = True`, `pyzdcf` can create and save light curve files used as input after averaging points with identical times. 
+
+
+### Running the code
+An example for calculating cross-correlation between two light curves:
+
+```python
+from pyzdcf import pyzdcf
+
+input = './input/'           # Path to the input data
+output = './output/'         # Path to the directory for saving the results
+
+# Light curve names
+lc1 = 'lc_name1'
+lc2 = 'lc_name2'
+
+# Parameters are passed to the pyZDCF as a dictionary
+
+params = dict(autocf            =  False, # Autocorrelation (T) or cross-correlation (F)
+              prefix            = 'ccf',  # Output files prefix
+              uniform_sampling  =  False, # Uniform sampling?
+              omit_zero_lags    =  True,  # Omit zero lag points?
+              minpts            =  0,     # Min. num. of points per bin (0 is a flag for default value of 11)
+              num_MC            =  100,   # Num. of Monte Carlo simulations for error estimation
+              lc1_name          =  lc1,   # Name of the first light curve file
+              lc2_name          =  lc2    # Name of the second light curve file (required only if we do CCF)
+             )
+
+# Here we use non-interactive mode (intr=False)
+dcf_df = pyzdcf(input_dir  = input, 
+                output_dir = output, 
+                intr       = False, 
+                parameters = params, 
+                sep        = ',', 
+                sparse     = 'auto', 
+                verbose    = True)
+
+# To run the program in interactive mode (like the original Fortran code):
+dcf_df = pyzdcf(input_dir  = input, 
+                output_dir = output, 
+                intr       = True, 
+                sep        = ',', 
+                sparse     = 'auto', 
+                verbose    = True
+                )
+```
+
+</br>
+
+- For more examples see [example notebook](https://github.com/LSST-sersag/pyzdcf/blob/main/notebooks/examples.ipynb).
+
+- Additionally, you can also check out code description of the original Fortran version because the majority of input parameters and all output files are the same as in pyZDCF. You can download the fortran source code [here](https://www.weizmann.ac.il/particle/tal/research-activities/software).
+
+
+## Features
+
+* **Sparse matrix implementation** for reduced RAM usage when working with long light curves (>3000 points);
+> The main benefit is that we can now run these demanding calculations on our own personal computers (8 GB of RAM is enough for
+> light curves containing up to 15000 points), making the usage of this algorithm more convinient than ever.
+> 
+> You can turn this on/off by specifying `sparse` keyword argument to `True` or `False`. Default value is `'auto'`, where sparse marices are utilized when there are more than 3000 points per light curve. Note that by reducing RAM usage, we pay in increased program running time.
+
+* **Interactive mode**: program specifically asks the user to provide necessary parameters (similar to original Fortran version);
+* **Manual mode**: user can provide all parameters in one dictionary.
+* **Fixed bugs** from original ZDCF (v2.3) written in Fortran 95.
+
+The module was tested (i.e., compared with original ZDCF v2.3 output, with fixed bugs) for various parameter combinations on a set of 100 AGN light curve candidates (*g* and *r* bands). The list of object ids and coordinates was taken from a combined catalogue of known AGNs ([Sánchez-Sáez et al. 2021](https://ui.adsabs.harvard.edu/abs/2021AJ....162..206S/abstract)).
+
+## License
+
+Distributed under the MIT License.
+
+## Contact
+
+>**Isidora Jankov (main)** - ijankov@proton.me  
+>Andjelka Kovačević - andjelka@matf.bg.ac.rs  
+>Dragana Ilić - dilic@matf.bg.ac.rs
+
+You are welcome to write to us:
+- if there are any problems running the code on your system;
+- suggestions for code improvements.
+
+If you want to report a bug, please open an Issue on GitHub: [https://github.com/LSST-sersag/pyzdcf](https://github.com/LSST-sersag/pyzdcf).
+
+
+## Citation
+
+If you use pyZDCF for scientific work leading to a publication, 
+please consider acknowledging it using the following citation (BibTeX):
+
+```
+@software{jankov_isidora_2022_7253034,
+  author       = {Jankov, Isidora and
+                  Kovačević, Andjelka B. and
+                  Ilić, Dragana and
+                  Sánchez-Sáez, Paula and
+                  Nikutta, Robert},
+  title        = {pyZDCF: Initial Release},
+  month        = oct,
+  year         = 2022,
+  publisher    = {Zenodo},
+  version      = {v1.0.0},
+  doi          = {10.5281/zenodo.7253034},
+  url          = {https://doi.org/10.5281/zenodo.7253034}
+}
+```
 
-packages = \
-['pyzdcf']
+For other citation formats see: [https://doi.org/10.5281/zenodo.7253034](https://doi.org/10.5281/zenodo.7253034)
+
+## <a name="ackn" />Acknowledgments
+
+* The pyZDCF module is based on the original Fortran code developed by Prof. Tal Alexander (Weizmann Institute of Science, Israel). Download Fortran version from professor's [page](https://www.weizmann.ac.il/particle/tal/research-activities/software).  
+* For theoretical details regarding the ZDCF algorithm see this publication: [Alexander, T. (1997)](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract).  
+* Huge thanks to my closest collegues and mentors Dr. Andjelka Kovačević and Dr. Dragana Ilić, as well as to Dr. Paula Sánchez-Sáez and Dr. Robert Nikutta for invaluable input during the development and testing of this python module.  
+* Many thanks to Prof. Eli Waxman, Amir Bar On and former students of Prof. Tal Alexander for their kind assistance regarding the development of pyZDCF module and its acknowledgment as part of the legacy behind late Prof. Alexander.
+
+## <a name="ref" />References
+* [Alexander, T. 1997, in: Astronomical Time Series, eds. D. Maoz, A. Sternberg, & E. M. Leibowitz, Vol. 218, Springer, Is AGN Variability Correlated with Other AGN Properties? ZDCF Analysis of Small Samples of Sparse Light Curves](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)
+* [Jankov, I.; Kovačević A. B.; Ilić, D.; et al. 2022, Astronomische Nachrichten, 343, e210090](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)
+* [Kovačević, A.; Popović, L. Č.; Shapovalova, A. I.; et al. 2014, Advances in Space Research, 54, 1414-1428](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract)
+* [Sánchez-Sáez, P.; Lira, H.; Martí, L.; et al. 2021,The Astronomical Journal, 162, id.206](https://ui.adsabs.harvard.edu/abs/2021AJ....162..206S/abstract)
+* [Shapovalova, A. I.; Popović, L. Č.; Afanasiev, V. L.; et al. 2019, MNRAS, 485, 4790-4803](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract)
 
-package_data = \
-{'': ['*']}
 
-install_requires = \
-['numpy>=1.16.5,<1.23.0', 'pandas>=1.3,<2.0', 'scipy>=1.7.3,<2.0.0']
-
-setup_kwargs = {
-    'name': 'pyzdcf',
-    'version': '1.0.0',
-    'description': 'Python module used for robust estimation of cross-corelation functions of sparse and unevenly sampled astronomical time-series. It emulates a Fortran program called ZDCF which is based on the Z-transformed Discrete Correlation Function algorithm (ZDCF, Alexander 1997).',
-    'long_description': '# pyZDCF\n\n## Description\n\n**pyZDCF** is a Python module that emulates a widely used Fortran program called ZDCF (Z-transformed Discrete Correlation Function, [Alexander 1997](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)). It is used for robust estimation of cross-correlation function of sparse and unevenly sampled astronomical time-series. This Python implementation also introduces sparse matrices in order to significantly reduce RAM usage when running the code on large time-series (> 3000 points).\n\npyZDCF is based on the original Fortran code fully developed by \nProf. Tal Alexander from Weizmann Institute of Science, Israel \n(see Acknowledgements and References for details and further reading).\n\n## Motivation\n\nDevelopment of pyZDCF module was motivated by the long and successful usage of \nthe original ZDCF Fortran code in the analysis of light curves of active galactic\nnuclei by our research group (see [Kovacevic et al. 2014](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract), [Shapovalova et al. 2019](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract), and reference therein). One of the science cases we investigate is photometric reverberation mapping in the context of Legacy Survey of Space and Time (LSST) survey strategies (see [Jankov et al. 2022](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)). However, this module is **general** and is meant to be used for cross-correlation of spectroscopic or photometric light curves, same as the original Fortran version.\n\n\n### Dependencies\n>```\n>python = ">=3.8,<3.11"\n>numpy = ">=1.16.5,<1.23.0"\n>pandas = "^1.3"\n>scipy = "^1.7.3"\n>```\n\n## How to use\n\n### Input files\nThis code requires user-provided plain text files as input. CSV files are \naccepted by default, but you can use any other delimited file, as long as you\nprovide the `sep` keyword argument when calling `pyzdcf` function. The input\nlight curve file should be in 3 columns: time (ordered), flux/magnitude and\nabsolute error on flux/magnitude. Make sure to exclude the header (column\nnames) from the input files.\n\nFirst few lines of the example input file accepted by default (CSV):\n\n```\n0.0,0.9594479339474323,0.0019188958678948648\n1.0,0.9588196871078336,0.0019176393742156672\n2.0,0.9637198686651904,0.0019274397373303808\n3.0,0.9622807967282166,0.0019245615934564328\n```\n\n**NOTE:** pyZDCF is tested only with input files having whole numbers (integers) for time column. If you have decimal numbers (e.g., you have a light curve with several measurments in the same night expressed as fractions of a day instead of minutes), just convert them into a time format with integer values (e.g., minutes instead of days). On the other hand, you could round the values from the same day (e.g. 5.6 --> 5, 5.8 --> 5, etc.) and the algorithm will take in the information and average the flux for that day. \n\n### Input parameters\n\nIf you use interactive mode (`intr = True`), then pyZDCF will ask you to\nenter all input parametars interactively, similarly to original ZDCF interface.\nThere is also a manual mode (`intr = False`) where you can provide input\nparameters using a dictionary and passing it to `parameters` keyword argument.\n\nAvailable input parameters (keys in the `parameters` dictionary) are:\n\n- `autocf` - if ``True``, perform auto-correlation, otherwise do the cross-correlation.\n- `prefix` - provide a name for the output file.\n- `uniform_sampling` - if ``True``, set flag to perform uniform sampling of the light curve.\n- `omit_zero_lags` - if True, omit zero lag points.\n- `minpts` - minimal number of points per bin.\n- `num_MC` - number of Monte Carlo simulations for error estimation.\n- `lc1_name` - Name of the first light curve file\n- `lc2_name` - Name of the second light curve file (required only if we do cross-correlation)\n\nFor more information on the correct syntax, see "Running the code" subsection and the "API Documentation" section.\n\n\n### Output\n\nThe return value of the `pyzdcf` function is a `pandas.DataFrame` object displaying the results in 7 columns:\n\n```\n+---+-------+-------------+-------------+--------------+-------------+-------------+------+\n|   |   tau |   -sig(tau) |   +sig(tau) |          dcf |   -err(dcf) |   +err(dcf) | #bin |\n|---+-------+-------------+-------------+--------------+-------------+-------------+------|\n| 0 |  -991 |           4 |           0 |  0.13598     |  0.361559   |  0.342224   |   10 |\n| 1 |  -988 |           2 |           0 | -0.217733    |  0.279988   |  0.301034   |   13 |\n| 2 |  -985 |           2 |           0 | -0.0614938   |  0.266546   |  0.27135    |   16 |\n| 3 |  -982 |           2 |           0 |  0.239601    |  0.237615   |  0.223317   |   19 |\n| 4 |  -979 |           2 |           0 |  0.331415    |  0.208171   |  0.192523   |   22 |\n```\nThe columns are: time-lag, negative time-lag std, positive time-lag std, zdcf,\nnegative zdcf sampling error, positive zdcf sampling error, number of points \nper bin. For more information on how these values are calculated see \n[Alexander 1997](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract).\n\nThe code will also generate an output .dcf file file in a specified folder on your computer with same 7 columns containing the results. It is allowed to name these files however you want using the `prefix` parameter (see example in the next subsection).\n\nOptionally, by adding keyword argument `savelc = True`, `pyzdcf` can create and save light curve files used as input after averaging points with identical times. \n\n\n### Running the code\nAn example for calculating cross-correlation between two light curves:\n\n```python\nfrom pyzdcf import pyzdcf\n\ninput = \'./input/\'           # Path to the input data\noutput = \'./output/\'         # Path to the directory for saving the results\n\n# Light curve names\nlc1 = \'lc_name1\'\nlc2 = \'lc_name2\'\n\n# Parameters are passed to the pyZDCF as a dictionary\n\nparams = dict(autocf            =  False, # Autocorrelation (T) or cross-correlation (F)\n              prefix            = \'ccf\',  # Output files prefix\n              uniform_sampling  =  False, # Uniform sampling?\n              omit_zero_lags    =  True,  # Omit zero lag points?\n              minpts            =  0,     # Min. num. of points per bin (0 is a flag for default value of 11)\n              num_MC            =  100,   # Num. of Monte Carlo simulations for error estimation\n              lc1_name          =  lc1,   # Name of the first light curve file\n              lc2_name          =  lc2    # Name of the second light curve file (required only if we do CCF)\n             )\n\n# Here we use non-interactive mode (intr=False)\ndcf_df = pyzdcf(input_dir  = input, \n                output_dir = output, \n                intr       = False, \n                parameters = params, \n                sep        = \',\', \n                sparse     = \'auto\', \n                verbose    = True)\n\n# To run the program in interactive mode (like the original Fortran code):\ndcf_df = pyzdcf(input_dir  = input, \n                output_dir = output, \n                intr       = True, \n                sep        = \',\', \n                sparse     = \'auto\', \n                verbose    = True\n                )\n```\n\n</br>\n\n- For more examples see [example notebook](https://github.com/LSST-sersag/pyzdcf/blob/main/notebooks/examples.ipynb).\n\n- Additionally, you can also check out code description of the original Fortran version because the majority of input parameters and all output files are the same as in pyZDCF. You can download the fortran source code [here](https://www.weizmann.ac.il/particle/tal/research-activities/software).\n\n\n## Features\n\n* Added an option to use **sparse matrix implementation** for reduced RAM usage when working with long light curves (>3000 points);\n> The main benefit is that we can now run these demanding calculations on our own personal computers (8 GB of RAM is enough for\n> light curves containing up to 15000 points), making the usage of this algorithm more convinient than ever.\n> \n> You can turn this on/off by specifying `sparse` keyword argument to `True` or `False`. Default value is `\'auto\'`, where sparse marices are utilized when there are more than 3000 points per light curve. Note that by reducing RAM usage, we pay in increased program running time.\n\n* **Interactive mode**: program specifically asks the user to provide necessary parameters (similar to original Fortran version);\n* **Manual mode**: user can provide all parameters in one dictionary.\n\n\n## License\n\nDistributed under the MIT License.\n\n## Contact\n\n>**Isidora Jankov (main)** - isidora_jankov@matf.bg.ac.rs  \n>Andjelka Kovačević - andjelka@matf.bg.ac.rs  \n>Dragana Ilić - dilic@matf.bg.ac.rs\n\nYou can write to us:\n- if there are any problems running the code on your system;\n- suggestions for code improvements.\n\nIf you want to report a bug, please open an Issue on GitHub: [https://github.com/LSST-sersag/pyzdcf](https://github.com/LSST-sersag/pyzdcf).\n\n\n## Citation\n\nIf you use pyZDCF for scientific work leading to a publication, \nplease consider acknowledging it using the following citation (BibTeX):\n\n```\n@software{jankov_isidora_2022_7253034,\n  author       = {Jankov, Isidora and\n                  Kovačević, Andjelka B. and\n                  Ilić, Dragana and\n                  Sánchez-Sáez, Paula and\n                  Nikutta, Robert},\n  title        = {pyZDCF: Initial Release},\n  month        = oct,\n  year         = 2022,\n  publisher    = {Zenodo},\n  version      = {v1.0.0},\n  doi          = {10.5281/zenodo.7253034},\n  url          = {https://doi.org/10.5281/zenodo.7253034}\n}\n```\n\nFor other citation formats see: [https://doi.org/10.5281/zenodo.7253034](https://doi.org/10.5281/zenodo.7253034)\n\n## Acknowledgments\n\n* The pyZDCF module is based on the original Fortran code developed by Prof. Tal Alexander (Weizmann Institute of Science, Israel). Download Fortran version from professor\'s [page](https://www.weizmann.ac.il/particle/tal/research-activities/software).  \n* For theoretical details regarding the ZDCF algorithm see this publication: [Alexander, T. (1997)](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract).  \n* Huge thanks to my closest collegues and mentors Dr. Andjelka Kovačević and Dr. Dragana Ilić, as well as to Dr. Paula Sánchez-Sáez and Dr. Robert Nikutta for invaluable input during the development and testing of this python module.  \n* Many thanks to Prof. Eli Waxman, Amir Bar On and former students of Prof. Tal Alexander for their kind assistance regarding the development of pyZDCF module and its acknowledgment as part of the legacy behind late Prof. Alexander.\n\n## References\n* [Alexander, T. 1997, in: Astronomical Time Series, eds. D. Maoz, A. Sternberg, & E. M. Leibowitz, Vol. 218, Springer, Is AGN Variability Correlated with Other AGN Properties? ZDCF Analysis of Small Samples of Sparse Light Curves](https://ui.adsabs.harvard.edu/abs/1997ASSL..218..163A/abstract)\n* [Jankov, I.; Kovačević A. B.; Ilić, D.; et al. 2022, Astronomische Nachrichten, 343, e210090](https://ui.adsabs.harvard.edu/abs/2022AN....34310090J/abstract)\n* [Kovačević, A.; Popović, L. Č.; Shapovalova, A. I.; et al. 2014, Advances in Space Research, 54, 1414-1428](https://ui.adsabs.harvard.edu/abs/2014AdSpR..54.1414K/abstract)\n* [Shapovalova, A. I.; Popović, L. Č.; Afanasiev, V. L.; et al. 2019, MNRAS, 485, 4790-4803](https://ui.adsabs.harvard.edu/abs/2019MNRAS.485.4790S/abstract)\n\n\n\n',
-    'author': 'Isidora Jankov',
-    'author_email': 'isidora_jankov@matf.bg.ac.rs',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/LSST-sersag/pyzdcf',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
 
 
-setup(**setup_kwargs)
```

