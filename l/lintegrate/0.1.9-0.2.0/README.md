# Comparing `tmp/lintegrate-0.1.9.tar.gz` & `tmp/lintegrate-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/lintegrate-0.1.9.tar", last modified: Fri Dec 10 16:47:59 2021, max compression
+gzip compressed data, was "lintegrate-0.2.0.tar", last modified: Wed May 22 13:57:11 2024, max compression
```

## Comparing `lintegrate-0.1.9.tar` & `lintegrate-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/
--rw-r--r--   0 runner    (1001) docker     (121)    35078 2021-12-10 16:47:49.000000 lintegrate-0.1.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      208 2021-12-10 16:47:49.000000 lintegrate-0.1.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2021-12-10 16:47:59.000000 lintegrate-0.1.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7204 2021-12-10 16:47:49.000000 lintegrate-0.1.9/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     2948 2021-12-10 16:47:49.000000 lintegrate-0.1.9/SConstruct
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/example/
--rw-r--r--   0 runner    (1001) docker     (121)      417 2021-12-10 16:47:49.000000 lintegrate-0.1.9/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)     2393 2021-12-10 16:47:49.000000 lintegrate-0.1.9/example/example.c
--rw-r--r--   0 runner    (1001) docker     (121)     2014 2021-12-10 16:47:49.000000 lintegrate-0.1.9/example/example_flat.c
--rw-r--r--   0 runner    (1001) docker     (121)     2187 2021-12-10 16:47:49.000000 lintegrate-0.1.9/example/example_split.c
--rw-r--r--   0 runner    (1001) docker     (121)      546 2021-12-10 16:47:49.000000 lintegrate-0.1.9/gsl-config.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/lintegrate/
--rw-r--r--   0 runner    (1001) docker     (121)       13 2021-12-10 16:47:49.000000 lintegrate-0.1.9/lintegrate/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)       49 2021-12-10 16:47:49.000000 lintegrate-0.1.9/lintegrate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)   526634 2021-12-10 16:47:58.000000 lintegrate-0.1.9/lintegrate/lintegrate.c
--rw-r--r--   0 runner    (1001) docker     (121)    19533 2021-12-10 16:47:49.000000 lintegrate-0.1.9/lintegrate/lintegrate.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/lintegrate.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     9662 2021-12-10 16:47:58.000000 lintegrate-0.1.9/lintegrate.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      659 2021-12-10 16:47:59.000000 lintegrate-0.1.9/lintegrate.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-12-10 16:47:58.000000 lintegrate-0.1.9/lintegrate.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2021-12-10 16:47:58.000000 lintegrate-0.1.9/lintegrate.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       11 2021-12-10 16:47:58.000000 lintegrate-0.1.9/lintegrate.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      175 2021-12-10 16:47:49.000000 lintegrate-0.1.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       16 2021-12-10 16:47:49.000000 lintegrate-0.1.9/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      123 2021-12-10 16:47:59.000000 lintegrate-0.1.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2021-12-10 16:47:49.000000 lintegrate-0.1.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/src/
--rw-r--r--   0 runner    (1001) docker     (121)    77504 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/cquad_const.c
--rw-r--r--   0 runner    (1001) docker     (121)     1568 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/err.c
--rw-r--r--   0 runner    (1001) docker     (121)     6882 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/lintegrate.h
--rw-r--r--   0 runner    (1001) docker     (121)    17711 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/lintegrate_cquad.c
--rw-r--r--   0 runner    (1001) docker     (121)    18051 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/lintegrate_qag.c
--rw-r--r--   0 runner    (1001) docker     (121)     6371 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/lintegrate_qng.c
--rw-r--r--   0 runner    (1001) docker     (121)     4534 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/lintegrate_split.c
--rw-r--r--   0 runner    (1001) docker     (121)     1458 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/logadd.c
--rw-r--r--   0 runner    (1001) docker     (121)     1418 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/logsub.c
--rw-r--r--   0 runner    (1001) docker     (121)    18380 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/qkrules.c
--rw-r--r--   0 runner    (1001) docker     (121)     6941 2021-12-10 16:47:49.000000 lintegrate-0.1.9/src/qng.h
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-12-10 16:47:59.000000 lintegrate-0.1.9/test/
--rw-r--r--   0 runner    (1001) docker     (121)     4226 2021-12-10 16:47:49.000000 lintegrate-0.1.9/test/test_lintegrate.py
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.488434 lintegrate-0.2.0/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      527 2023-08-31 15:59:16.000000 lintegrate-0.2.0/.readthedocs.yaml
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      274 2023-08-31 15:59:16.000000 lintegrate-0.2.0/CONTRIBUTING.md
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    35078 2023-08-31 15:59:16.000000 lintegrate-0.2.0/LICENSE
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      191 2024-05-22 13:46:46.000000 lintegrate-0.2.0/MANIFEST.in
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     9394 2024-05-22 13:57:11.482953 lintegrate-0.2.0/PKG-INFO
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     8179 2023-09-04 11:01:16.000000 lintegrate-0.2.0/README.md
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2948 2024-05-21 10:23:28.000000 lintegrate-0.2.0/SConstruct
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.076250 lintegrate-0.2.0/docs/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      634 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/Makefile
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     4873 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/capi.rst
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2510 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/conf.py
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     3071 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/examples.rst
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2099 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/index.rst
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2661 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/installation.rst
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     7167 2023-08-31 15:59:16.000000 lintegrate-0.2.0/docs/pythonapi.rst
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.177296 lintegrate-0.2.0/example/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      417 2023-08-31 15:59:16.000000 lintegrate-0.2.0/example/Makefile
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2393 2023-08-31 15:59:16.000000 lintegrate-0.2.0/example/example.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2014 2023-08-31 15:59:16.000000 lintegrate-0.2.0/example/example_flat.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     2187 2023-08-31 15:59:16.000000 lintegrate-0.2.0/example/example_split.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      546 2023-08-31 15:59:16.000000 lintegrate-0.2.0/gsl-config.bat
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     1443 2024-05-22 13:46:46.000000 lintegrate-0.2.0/pyproject.toml
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)       38 2024-05-22 13:57:11.489443 lintegrate-0.2.0/setup.cfg
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     1841 2024-05-22 13:46:46.000000 lintegrate-0.2.0/setup.py
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.315231 lintegrate-0.2.0/src/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)       25 2024-05-22 13:46:46.000000 lintegrate-0.2.0/src/.gitignore
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    77504 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/cquad_const.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     1568 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/err.c
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.352893 lintegrate-0.2.0/src/lintegrate/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      442 2024-05-22 13:46:46.000000 lintegrate-0.2.0/src/lintegrate/__init__.py
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      411 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate/_version.py
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    19798 2024-05-22 13:46:46.000000 lintegrate-0.2.0/src/lintegrate/lintegrate.pyx
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.474935 lintegrate-0.2.0/src/lintegrate.egg-info/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     9394 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate.egg-info/PKG-INFO
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      805 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate.egg-info/SOURCES.txt
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)        1 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate.egg-info/dependency_links.txt
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)      122 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate.egg-info/requires.txt
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)       11 2024-05-22 13:57:10.000000 lintegrate-0.2.0/src/lintegrate.egg-info/top_level.txt
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     6882 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/lintegrate.h
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    17711 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/lintegrate_cquad.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    18051 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/lintegrate_qag.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     6371 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/lintegrate_qng.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     4534 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/lintegrate_split.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     1458 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/logadd.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     1418 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/logsub.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)    18380 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/qkrules.c
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     6941 2023-08-31 15:59:16.000000 lintegrate-0.2.0/src/qng.h
+drwxrwxrwx   0 matthew   (1000) matthew   (1000)        0 2024-05-22 13:57:11.452854 lintegrate-0.2.0/test/
+-rwxrwxrwx   0 matthew   (1000) matthew   (1000)     4226 2023-08-31 15:59:16.000000 lintegrate-0.2.0/test/test_lintegrate.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `lintegrate-0.1.9/LICENSE` & `lintegrate-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/README.md` & `lintegrate-0.2.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,14 +14,16 @@
  * [`gsl_integration_qng`](https://www.gnu.org/software/gsl/doc/html/integration.html#qng-non-adaptive-gauss-kronrod-integration)
  * [`gsl_integration_cquad`](https://www.gnu.org/software/gsl/doc/html/integration.html#cquad-doubly-adaptive-integration)
 
 respectively. These can be useful when, e.g., you can calculate the natural logarithm of a Gaussian likelihood function (in cases where the exponentiation of the Gaussian function would lead to zeros or infinities) and you want to numerically find the integral of the Gaussian function itself.
 
 The functions `lintegrate_qag`, `lintegrate_qng`, and `lintegrate_cquad`, all have wrappers functions (with `_split` appended to their names) that allow the user to specify a set of intervals that the integrals will be split into when performing the calculation. The intervals could, for example, be spaced evenly in log-space, for cases where the integral function has a very pronounced peak as it approaches zero.
 
+The full API documentation and examples can be found [here](https://lintegrate.readthedocs.io/).
+
 ## Example
 
 An [example](example/example.c) of the use the functions is:
 
 ```C
 /* example using lintegrate functionality */
 
@@ -113,19 +115,19 @@
 The library can be built using [scons](http://scons.org) by just typing `sudo scons` in the base directory. To install
 the library system-wide (in `/usr/local/lib` by default) run:
 ```
 sudo scons
 sudo scons install
 ```
 
-A Python module containing wrappers to the functions can be built by running, e.g.:
-```
-sudo python setup.py install
+A Python module containing wrappers to the functions can be built and installed from source for the user by running, e.g.:
+```bash
+pip install .
 ```
-for a system-wide install (add `--user` and remove `sudo` if just wanting to install for a single user, and using `--prefix=INSTALLPATH` if wanting to specify this install location).
+from within the repository directory.
 
 The Python module can also be installed from [PyPI](https://pypi.org/project/lintegrate/) using pip with:
 ```bash
 pip install lintegrate
 ```
 
 or in a Conda environment with:
@@ -185,13 +187,36 @@
 mu <- 0
 sig <- 1
 mmin <- -10
 mmax <- 10
 lint$lqag(py_func(integrand), r_to_py(mmin), r_to_py(mmax), c(mu, sig))
 ```
 
-[![DOI](https://zenodo.org/badge/93165960.svg)](https://zenodo.org/badge/latestdoi/93165960)
+## Citation
+
+If using `lintegrate` in your research, I would be grateful if you cite the associated [JOSS paper](https://joss.theoj.org/papers/10.21105/joss.04231) for the software. The following BibTeX citation can be used:
+
+```bibtex
+@article{Pitkin2022,
+  doi = {10.21105/joss.04231},
+  url = {https://doi.org/10.21105/joss.04231},
+  year = {2022},
+  publisher = {The Open Journal},
+  volume = {7},
+  number = {73},
+  pages = {4231},
+  author = {Matthew Pitkin},
+  title = {lintegrate: A C/Python numerical integration library for working in log-space},
+  journal = {Journal of Open Source Software}
+}
+```
+
+You may also want to cite the [GSL](https://www.gnu.org/software/gsl/) reference "_M. Galassi et al, GNU Scientific Library Reference Manual (3rd Ed.), ISBN 0954612078_" and the URL http://www.gnu.org/software/gsl/.
+
+
+[![DOI](https://joss.theoj.org/papers/10.21105/joss.04231/status.svg)](https://doi.org/10.21105/joss.04231)
 [![Build Status](https://github.com/mattpitkin/lintegrate/workflows/build/badge.svg)](https://github.com/mattpitkin/lintegrate/actions?query=workflow%3Abuild)
 [![PyPI version](https://badge.fury.io/py/lintegrate.svg)](https://badge.fury.io/py/lintegrate)
 [![Anaconda-Server Badge](https://anaconda.org/conda-forge/lintegrate/badges/version.svg)](https://anaconda.org/conda-forge/lintegrate)
+[![Documentation Status](https://readthedocs.org/projects/lintegrate/badge/?version=latest)](http://lintegrate.readthedocs.io/en/latest/?badge=latest)
 
 &copy; 2017 Matthew Pitkin
```

### Comparing `lintegrate-0.1.9/SConstruct` & `lintegrate-0.2.0/SConstruct`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/example/example.c` & `lintegrate-0.2.0/example/example.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/example/example_flat.c` & `lintegrate-0.2.0/example/example_flat.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/example/example_split.c` & `lintegrate-0.2.0/example/example_split.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/gsl-config.bat` & `lintegrate-0.2.0/gsl-config.bat`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/lintegrate/lintegrate.pyx` & `lintegrate-0.2.0/src/lintegrate/lintegrate.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -16,40 +16,46 @@
 # along with this program; if not, write to the Free Software
 # Foundation, Inc., 51 Franklin Street, Fifth Floor, Boston, MA 02110-1301, USA.
 
 import numpy as np
 cimport numpy as np
 
 from numpy.math cimport LOGE2, INFINITY
-
 from libc.math cimport exp, sqrt, log, log10, isinf, fabs
 
+
 cdef extern from "gsl/gsl_integration.h":
     void gsl_integration_workspace_free (gsl_integration_workspace * w)
     ctypedef struct gsl_integration_workspace
     gsl_integration_workspace * gsl_integration_workspace_alloc (size_t n)
     void gsl_integration_cquad_workspace_free (gsl_integration_cquad_workspace * w)
     ctypedef struct gsl_integration_cquad_workspace
     gsl_integration_cquad_workspace * gsl_integration_cquad_workspace_alloc (size_t n)
 
+
 cdef extern from "gsl/gsl_sf_log.h":
     double gsl_sf_log_1plusx(double x)
 
+
 cdef extern from "lintegrate.h":
     ctypedef double (*pylintfunc)(double x, void *funcdata, void *args)
     int lintegration_qng (pylintfunc f, void *funcdata, void *args, double a, double b, double epsabs, double epsrel, double *result, double *abserr, size_t *neval)
     int lintegration_qag (pylintfunc f, void *funcdata, void *args, double a, double b, double epsabs, double epsrel, size_t limit, int key, gsl_integration_workspace * workspace, double * result, double * abserr)
     int lintegration_cquad (pylintfunc f, void *funcdata, void *args, double a, double b, double epsabs, double epsrel, gsl_integration_cquad_workspace * ws, double *result, double *abserr, size_t * nevals)
 
 
 DTYPE = np.float64
 ctypedef np.float64_t DTYPE_t
 
+# call import_array() https://cython.readthedocs.io/en/latest/src/tutorial/numpy.html#adding-types
+np.import_array()
+
 GSL_DBL_EPSILON = 2.2204460492503131e-16
 
+
 cdef double logtrapzC(np.ndarray[DTYPE_t, ndim=1] lx, np.ndarray[DTYPE_t, ndim=1] t):
     assert len(lx) == len(t) or len(t) == 1, "Function and function evaluation points must be the same length, or there must be a single evaluation point spacing given"
 
     cdef double B = -INFINITY
 
     cdef int i = 0
     cdef double z
@@ -66,15 +72,15 @@
 
     if len(t) > 1:
         return B
     else:
         return B + log(t[0])
 
 
-cdef logplus(double x, double y):
+cdef double logplus(double x, double y):
     """
     Calculate :math:`\log{(e^x + e^y)}` in a way that preserves numerical precision.
 
     .. note:: This is faster than using the :func:`numpy.logaddexp` function
 
     Parameters
     ----------
@@ -133,47 +139,47 @@
         if isinstance(x, np.ndarray) or isinstance(x, list):
             # check arrays are the same length
             if not disable_checks:
                 assert len(f) == len(x) and len(x) > 1, "Function and function evaluation points are not the same length"
 
             if not disable_checks:
                 # make sure x values are in ascending order (keeping f values associated to their x evaluation points)
-                zp = np.array(sorted(zip(x, f)))
+                zp = np.array(sorted(zip(x, f)), dtype=np.float64)
 
                 # perform trapezium rule (internal logtrapzC function is faster than using scipy logsumexp)
                 return logtrapzC(zp[:,1], zp[:,0])
             else:
-                return logtrapzC(np.array(f), np.array(x))
+                return logtrapzC(np.array(f, dtype=np.float64), np.array(x, dtype=np.float64))
         elif isinstance(x, float):
             assert x > 0., "Evaluation spacings must be positive"
 
             # perform trapezium rule
-            return logtrapzC(f, np.array([x]))
+            return logtrapzC(f.astype(np.float64), np.array([x]))
         else:
             raise TypeError('Error... value of "x" must be a numpy array or a float')
     elif callable(f): # f is a function
         if isinstance(x, np.ndarray) or isinstance(x, list):
             if not disable_checks:
                 assert len(x) > 1, "Function must be evaluated at more than one point"
 
             try:
                 if not isinstance(args, tuple):
                     args = (args,)
-                vs = f(np.array(x), args) # make sure x is an array when passed to function
+                vs = f(np.array(x, dtype=np.float64), args) # make sure x is an array when passed to function
             except Exception as e:
                 raise RuntimeError('Error... could not evaluate function "f": {}'.format(e))
 
             if not disable_checks:
                 # make sure x values are in ascending order (keeping f values associated to their x evaluation points)
-                zp = np.array(sorted(zip(x, vs)))
+                zp = np.array(sorted(zip(x, vs)), dtype=np.float64)
 
                 # perform trapezium rule (internal logtrapzC function is faster than using scipy logsumexp)
                 return logtrapzC(zp[:,1], zp[:,0])
             else:
-                return logtrapzC(vs, np.array(x))
+                return logtrapzC(vs, np.array(x, dtype=np.float64))
         else:
             raise TypeError('Error... "x" must be a numpy array or list')
     else:
         raise RuntimeError('Error... "f" must be a numpy array, list, or callable function')
 
 
 def lqng(func, a=0., b=0., args=(), epsabs=1.49e-8, epsrel=1.49e-8, intervals=None, nintervals=0, intervaltype='linear'):
@@ -216,15 +222,15 @@
     epsrel : float, optional
         The relative error tolerance for the integral
     intervals : :class:`numpy.ndarray`, list, optional
         An array of values bounding intervals into which the integral will be split (this could be
         used, for example, if you have a very tightly peaked function and require small intervals
         around the peak).
     nintervals : int, optional
-        If `intervals` is not given then split the range between `a` and `b` into `nintervals'
+        If `intervals` is not given then split the range between `a` and `b` into `nintervals`
         intervals
     intervaltype : string, optional
         If splitting into `nintervals` intervals then choose whether to split the range in equal
         intervals in 'linear', 'log', or 'log10' space
     """
 
     if not callable(func):
@@ -311,15 +317,15 @@
         A key given the integration rule following those for the `gsl_integration_qag` function. This can be
         1, 2, 3, 4, 5, or 6, corresponding to the 15, 21, 31, 41, 51 and 61 point Gauss-Kronrod rules respectively.
     intervals : :class:`numpy.ndarray`, list, optional
         An array of values bounding intervals into which the integral will be split (this could be
         used, for example, if you have a very tightly peaked function and require small intervals
         around the peak).
     nintervals : int, optional
-        If `intervals` is not given then split the range between `a` and `b` into `nintervals'
+        If `intervals` is not given then split the range between `a` and `b` into `nintervals`
         intervals
     intervaltype : string, optional
         If splitting into `nintervals` intervals then choose whether to split the range in equal
         intervals in 'linear', 'log', or 'log10' space
     """
 
     if not callable(func):
@@ -415,15 +421,15 @@
     wsintervals : int, optional
         A sufficient number of subintervals for the integration (if the workspace is full the smallest intervals will be discarded)
     intervals : :class:`numpy.ndarray`, list, optional
         An array of values bounding intervals into which the integral will be split (this could be
         used, for example, if you have a very tightly peaked function and require small intervals
         around the peak).
     nintervals : int, optional
-        If `intervals` is not given then split the range between `a` and `b` into `nintervals'
+        If `intervals` is not given then split the range between `a` and `b` into `nintervals`
         intervals
     intervaltype : string, optional
         If splitting into `nintervals` intervals then choose whether to split the range in equal
         intervals in 'linear', 'log', or 'log10' space
     """
 
     if not callable(func):
@@ -473,9 +479,10 @@
     gsl_integration_cquad_workspace_free(w)
 
     return (result, abserr, neval)
 
 
 # callback function to allow python functions to be passed to C lintegration functions
 # (see e.g. https://github.com/cython/cython/tree/master/Demos/callback)
-cdef double lintegrate_callback(double x, void *f, void *args):
+cdef double lintegrate_callback(double x, void *f, void *args) noexcept:
     return (<object>f)(x, <object>args)
+
```

### Comparing `lintegrate-0.1.9/src/cquad_const.c` & `lintegrate-0.2.0/src/cquad_const.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/err.c` & `lintegrate-0.2.0/src/err.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/lintegrate.h` & `lintegrate-0.2.0/src/lintegrate.h`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/lintegrate_cquad.c` & `lintegrate-0.2.0/src/lintegrate_cquad.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/lintegrate_qag.c` & `lintegrate-0.2.0/src/lintegrate_qag.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/lintegrate_qng.c` & `lintegrate-0.2.0/src/lintegrate_qng.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/lintegrate_split.c` & `lintegrate-0.2.0/src/lintegrate_split.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/logadd.c` & `lintegrate-0.2.0/src/logadd.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/logsub.c` & `lintegrate-0.2.0/src/logsub.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/qkrules.c` & `lintegrate-0.2.0/src/qkrules.c`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/src/qng.h` & `lintegrate-0.2.0/src/qng.h`

 * *Files identical despite different names*

### Comparing `lintegrate-0.1.9/test/test_lintegrate.py` & `lintegrate-0.2.0/test/test_lintegrate.py`

 * *Files identical despite different names*

