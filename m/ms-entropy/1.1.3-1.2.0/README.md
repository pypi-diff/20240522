# Comparing `tmp/ms_entropy-1.1.3.tar.gz` & `tmp/ms_entropy-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_entropy-1.1.3.tar", last modified: Thu May  2 20:30:51 2024, max compression
+gzip compressed data, was "ms_entropy-1.2.0.tar", last modified: Wed May 22 01:14:00 2024, max compression
```

## Comparing `ms_entropy-1.1.3.tar` & `ms_entropy-1.2.0.tar`

### file list

```diff
@@ -1,54 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.610748 ms_entropy-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    20869 2024-05-02 20:30:51.610748 ms_entropy-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6772 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.598748 ms_entropy-1.1.3/ms_entropy/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.602748 ms_entropy-1.1.3/ms_entropy/entropy_search/
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)  1130374 2024-05-02 20:30:50.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    20960 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search.py
--rw-r--r--   0 runner    (1001) docker     (127)    30699 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    17630 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.602748 ms_entropy-1.1.3/ms_entropy/file_io/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/lbm2_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/mgf_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/msp_file.py
--rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/mzml_file.py
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/shared.py
--rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/file_io/spec_file.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.606748 ms_entropy-1.1.3/ms_entropy/pipe/
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/df.py
--rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/pandas.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/pipe/pipe.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.606748 ms_entropy-1.1.3/ms_entropy/spectra/
--rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/CleanSpectrum.c
--rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/CleanSpectrum.h
--rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/SpectralEntropy.c
--rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/SpectralEntropy.h
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)   516655 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy/spectra/entropy_cython.c
--rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/entropy_cython.pyx
--rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/entropy_numba.py
--rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/spectra/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/ms_entropy/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.606748 ms_entropy-1.1.3/ms_entropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    20869 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-02 20:30:51.000000 ms_entropy-1.1.3/ms_entropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-02 20:30:51.610748 ms_entropy-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:30:51.606748 ms_entropy-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/tests/test_entropy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5819 2024-05-02 20:30:42.000000 ms_entropy-1.1.3/tests/test_entropy_search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.873424 ms_entropy-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    20885 2024-05-22 01:14:00.873424 ms_entropy-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6788 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.861424 ms_entropy-1.2.0/ms_entropy/
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.865424 ms_entropy-1.2.0/ms_entropy/entropy_search/
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1130374 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    21277 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30699 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17716 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search_core_medium_memory.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.865424 ms_entropy-1.2.0/ms_entropy/file_io/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2047 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/lbm2_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/mgf_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/msp_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3916 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/mzml_file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/shared.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5722 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/file_io/spec_file.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.869424 ms_entropy-1.2.0/ms_entropy/pipe/
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/df.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4241 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1324 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/pipe/pipe.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.869424 ms_entropy-1.2.0/ms_entropy/spectra/
+-rw-r--r--   0 runner    (1001) docker     (127)    10932 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/CleanSpectrum.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3394 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/CleanSpectrum.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5571 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/SpectralEntropy.c
+-rw-r--r--   0 runner    (1001) docker     (127)     4812 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/SpectralEntropy.h
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10465 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)   516655 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy/spectra/entropy_cython.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11171 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/entropy_cython.pyx
+-rw-r--r--   0 runner    (1001) docker     (127)    11241 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/entropy_numba.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8756 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/spectra/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/ms_entropy/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.869424 ms_entropy-1.2.0/ms_entropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    20885 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2431 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       81 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 01:14:00.000000 ms_entropy-1.2.0/ms_entropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 01:14:00.873424 ms_entropy-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1868 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:14:00.869424 ms_entropy-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/tests/test_entropy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9011 2024-05-22 01:13:49.000000 ms_entropy-1.2.0/tests/test_entropy_search.py
```

### Comparing `ms_entropy-1.1.3/LICENSE` & `ms_entropy-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/PKG-INFO` & `ms_entropy-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_entropy
-Version: 1.1.3
+Version: 1.2.0
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Home-page: https://github.com/YuanyueLi/MSEntropy
 Author-email: Yuanyue Li <mail@yli.one>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,17 +230,17 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 [![Documentation Status](https://readthedocs.org/projects/msentropy/badge/?version=latest)](https://msentropy.readthedocs.io/en/latest/?badge=latest)
 
 
 If you have any questions, feel free to send me E-mails: mail@yli.one. If you find this package useful, please consider citing the following papers:
 
-> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
+> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ **20**, 1475-1478 (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
 > 
-> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524-1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ms_entropy-1.1.3/README.md` & `ms_entropy-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 [![Documentation Status](https://readthedocs.org/projects/msentropy/badge/?version=latest)](https://msentropy.readthedocs.io/en/latest/?badge=latest)
 
 
 If you have any questions, feel free to send me E-mails: mail@yli.one. If you find this package useful, please consider citing the following papers:
 
-> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
+> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ **20**, 1475-1478 (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
 > 
-> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524-1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search.py` & `ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c` & `ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx` & `ms_entropy-1.2.0/ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search.py` & `ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 #!/usr/bin/env python3
 import numpy as np
 import pickle
 from pathlib import Path
 from .flash_entropy_search_core import FlashEntropySearchCore
 from .flash_entropy_search_core_low_memory import FlashEntropySearchCoreLowMemory
+from .flash_entropy_search_core_medium_memory import FlashEntropySearchCoreMediumMemory
 from ..spectra import clean_spectrum
 
 
 class FlashEntropySearch:
     def __init__(self, max_ms2_tolerance_in_da=0.024, mz_index_step=0.0001, low_memory=False, path_data=None):
         self.precursor_mz_array = np.zeros(0, dtype=np.float32)
         self.low_memory = low_memory
-        if low_memory:
+        if low_memory==1:
             self.entropy_search = FlashEntropySearchCoreLowMemory(
                 path_data=path_data, max_ms2_tolerance_in_da=max_ms2_tolerance_in_da, mz_index_step=mz_index_step
             )
+        elif low_memory==2:
+            self.entropy_search = FlashEntropySearchCoreMediumMemory(
+                path_data=path_data, max_ms2_tolerance_in_da=max_ms2_tolerance_in_da, mz_index_step=mz_index_step
+            )
         else:
             self.entropy_search = FlashEntropySearchCore(path_data=path_data, max_ms2_tolerance_in_da=max_ms2_tolerance_in_da, mz_index_step=mz_index_step)
 
     def identity_search(self, precursor_mz, peaks, ms1_tolerance_in_da, ms2_tolerance_in_da, target="cpu", output_matched_peak_number=False, **kwargs):
         """
         Run the identity search, the query spectrum should be preprocessed by `clean_spectrum()` function before calling this function.
```

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search_core.py` & `ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search_core.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py` & `ms_entropy-1.2.0/ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 class FlashEntropySearchCoreLowMemory(FlashEntropySearchCore):
     def __init__(self, path_data, max_ms2_tolerance_in_da=0.024, mz_index_step=0.0001) -> None:
         super().__init__(max_ms2_tolerance_in_da=max_ms2_tolerance_in_da, mz_index_step=mz_index_step)
         self.path_data = Path(str(path_data))
         self.path_data.mkdir(parents=True, exist_ok=True)
         self.index_file = []
 
+    def __del__(self):
+        for file in self.index_file:
+            file.close()
+
     def _generate_index_from_peak_data(self, peak_data, max_indexed_mz, append):
         total_peaks_num = peak_data.shape[0]
 
         # Sort with precursor m/z.
         peak_data.sort(order="ion_mz")
 
         # Record the m/z, intensity, and spectrum index information for product ions.
```

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/lbm2_file.py` & `ms_entropy-1.2.0/ms_entropy/file_io/lbm2_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/mgf_file.py` & `ms_entropy-1.2.0/ms_entropy/file_io/mgf_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/msp_file.py` & `ms_entropy-1.2.0/ms_entropy/file_io/msp_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/mzml_file.py` & `ms_entropy-1.2.0/ms_entropy/file_io/mzml_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/shared.py` & `ms_entropy-1.2.0/ms_entropy/file_io/shared.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/file_io/spec_file.py` & `ms_entropy-1.2.0/ms_entropy/file_io/spec_file.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/pipe/entropy.py` & `ms_entropy-1.2.0/ms_entropy/pipe/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/pipe/functions.py` & `ms_entropy-1.2.0/ms_entropy/pipe/functions.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/pipe/pipe.py` & `ms_entropy-1.2.0/ms_entropy/pipe/pipe.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/CleanSpectrum.c` & `ms_entropy-1.2.0/ms_entropy/spectra/CleanSpectrum.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/CleanSpectrum.h` & `ms_entropy-1.2.0/ms_entropy/spectra/CleanSpectrum.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/SpectralEntropy.c` & `ms_entropy-1.2.0/ms_entropy/spectra/SpectralEntropy.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/SpectralEntropy.h` & `ms_entropy-1.2.0/ms_entropy/spectra/SpectralEntropy.h`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/entropy.py` & `ms_entropy-1.2.0/ms_entropy/spectra/entropy.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/entropy_cython.c` & `ms_entropy-1.2.0/ms_entropy/spectra/entropy_cython.c`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/entropy_cython.pyx` & `ms_entropy-1.2.0/ms_entropy/spectra/entropy_cython.pyx`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/entropy_numba.py` & `ms_entropy-1.2.0/ms_entropy/spectra/entropy_numba.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy/spectra/tools.py` & `ms_entropy-1.2.0/ms_entropy/spectra/tools.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/ms_entropy.egg-info/PKG-INFO` & `ms_entropy-1.2.0/ms_entropy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms_entropy
-Version: 1.1.3
+Version: 1.2.0
 Summary: This package provides a Python implementation of calculating spectral entropy, entropy similarity, and Flash entropy search for mass spectrometry data.
 Home-page: https://github.com/YuanyueLi/MSEntropy
 Author-email: Yuanyue Li <mail@yli.one>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -230,17 +230,17 @@
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.7972082.svg)](https://doi.org/10.5281/zenodo.7972082)
 [![Test MS Entropy package](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml/badge.svg?branch=main)](https://github.com/YuanyueLi/MSEntropy/actions/workflows/run_test.yml)
 [![Documentation Status](https://readthedocs.org/projects/msentropy/badge/?version=latest)](https://msentropy.readthedocs.io/en/latest/?badge=latest)
 
 
 If you have any questions, feel free to send me E-mails: mail@yli.one. If you find this package useful, please consider citing the following papers:
 
-> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
+> Li, Y., Fiehn, O. **Flash entropy search to query all mass spectral libraries in real time**, _Nat Methods_ **20**, 1475-1478 (2023). [https://doi.org/10.1038/s41592-023-02012-9](https://doi.org/10.1038/s41592-023-02012-9)
 > 
-> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524–1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
+> Li, Y., Kind, T., Folz, J. _et al._ **Spectral entropy outperforms MS/MS dot product similarity for small-molecule compound identification**, _Nat Methods_ **18**, 1524-1531 (2021). [https://doi.org/10.1038/s41592-021-01331-z](https://doi.org/10.1038/s41592-021-01331-z)
 
 # Theoritical Background
 
 `Spectral entropy` is an useful property to measure the complexity of a spectrum. It is inspried by the concept of Shannon entropy in information theory. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
 
 `Entropy similarity`, which measured spectral similarity based on spectral entropy, has been shown to outperform dot product similarity in compound identification. [(ref)](https://doi.org/10.1038/s41592-021-01331-z)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ms_entropy-1.1.3/ms_entropy.egg-info/SOURCES.txt` & `ms_entropy-1.2.0/ms_entropy.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 ./ms_entropy/__init__.py
 ./ms_entropy/version.py
 ./ms_entropy/entropy_search/__init__.py
 ./ms_entropy/entropy_search/fast_flash_entropy_search.py
 ./ms_entropy/entropy_search/flash_entropy_search.py
 ./ms_entropy/entropy_search/flash_entropy_search_core.py
 ./ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+./ms_entropy/entropy_search/flash_entropy_search_core_medium_memory.py
 ./ms_entropy/file_io/__init__.py
 ./ms_entropy/file_io/lbm2_file.py
 ./ms_entropy/file_io/mgf_file.py
 ./ms_entropy/file_io/msp_file.py
 ./ms_entropy/file_io/mzml_file.py
 ./ms_entropy/file_io/shared.py
 ./ms_entropy/file_io/spec_file.py
@@ -38,14 +39,15 @@
 ms_entropy/entropy_search/__init__.py
 ms_entropy/entropy_search/fast_flash_entropy_search.py
 ms_entropy/entropy_search/fast_flash_entropy_search_cpython.c
 ms_entropy/entropy_search/fast_flash_entropy_search_cpython.pyx
 ms_entropy/entropy_search/flash_entropy_search.py
 ms_entropy/entropy_search/flash_entropy_search_core.py
 ms_entropy/entropy_search/flash_entropy_search_core_low_memory.py
+ms_entropy/entropy_search/flash_entropy_search_core_medium_memory.py
 ms_entropy/file_io/__init__.py
 ms_entropy/file_io/lbm2_file.py
 ms_entropy/file_io/mgf_file.py
 ms_entropy/file_io/msp_file.py
 ms_entropy/file_io/mzml_file.py
 ms_entropy/file_io/shared.py
 ms_entropy/file_io/spec_file.py
```

### Comparing `ms_entropy-1.1.3/pyproject.toml` & `ms_entropy-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/setup.py` & `ms_entropy-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `ms_entropy-1.1.3/tests/test_entropy.py` & `ms_entropy-1.2.0/tests/test_entropy.py`

 * *Files identical despite different names*

