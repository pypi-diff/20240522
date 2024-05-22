# Comparing `tmp/stockwell-1.1.tar.gz` & `tmp/stockwell-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stockwell-1.1.tar", last modified: Mon Jun  5 13:44:01 2023, max compression
+gzip compressed data, was "stockwell-1.1.1.tar", last modified: Tue May 21 16:23:15 2024, max compression
```

## Comparing `stockwell-1.1.tar` & `stockwell-1.1.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-05 13:43:54.000000 stockwell-1.1/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-06-05 13:43:54.000000 stockwell-1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-06-05 13:43:54.000000 stockwell-1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-05 13:44:01.197198 stockwell-1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-05 13:43:54.000000 stockwell-1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-05 13:43:54.000000 stockwell-1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-05 13:44:01.197198 stockwell-1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-06-05 13:43:54.000000 stockwell-1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/c_libs/
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/sine.c
--rw-r--r--   0 runner    (1001) docker     (123)     9003 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/st.c
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/c_libs/st_types.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/lib_path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/sine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/st.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-06-05 13:43:54.000000 stockwell-1.1/stockwell/tests/test_stockwell.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-05 13:44:01.197198 stockwell-1.1/stockwell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6350 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-05 13:44:01.000000 stockwell-1.1/stockwell.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    70144 2023-06-05 13:43:54.000000 stockwell-1.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.918045 stockwell-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-21 16:23:10.000000 stockwell-1.1.1/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-21 16:23:10.000000 stockwell-1.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-05-21 16:23:10.000000 stockwell-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-21 16:23:15.918045 stockwell-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4316 2024-05-21 16:23:10.000000 stockwell-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-05-21 16:23:10.000000 stockwell-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-05-21 16:23:15.918045 stockwell-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3415 2024-05-21 16:23:10.000000 stockwell-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.918045 stockwell-1.1.1/stockwell/
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-05-21 16:23:15.918045 stockwell-1.1.1/stockwell/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.914045 stockwell-1.1.1/stockwell/c_libs/
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/c_libs/sine.c
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/c_libs/st.c
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/c_libs/st_types.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.914045 stockwell-1.1.1/stockwell/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/lib_path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/sine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/st.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.918045 stockwell-1.1.1/stockwell/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-05-21 16:23:10.000000 stockwell-1.1.1/stockwell/tests/test_stockwell.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 16:23:15.914045 stockwell-1.1.1/stockwell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6885 2024-05-21 16:23:15.000000 stockwell-1.1.1/stockwell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-21 16:23:15.000000 stockwell-1.1.1/stockwell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 16:23:15.000000 stockwell-1.1.1/stockwell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-21 16:23:15.000000 stockwell-1.1.1/stockwell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-21 16:23:15.000000 stockwell-1.1.1/stockwell.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    70144 2024-05-21 16:23:10.000000 stockwell-1.1.1/versioneer.py
```

### Comparing `stockwell-1.1/LICENSE.txt` & `stockwell-1.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `stockwell-1.1/PKG-INFO` & `stockwell-1.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: stockwell
-Version: 1.1
+Version: 1.1.1
 Summary: Time-frequency analysis through Stockwell transform
 Home-page: https://github.com/claudiodsf/stockwell
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
-License: CeCILL Free Software License Agreement, Version 2.1
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: Homepage, https://github.com/claudiodsf/stockwell
+Project-URL: Source, https://github.com/claudiodsf/stockwell
 Description: # Stockwell
         
         Python package for time-frequency analysis through Stockwell transform.
         
         Based on original code from [NIMH MEG Core Facility].
         
+        [![changelog-badge]][changelog-link]
         [![cf-badge]][cf-link]
         [![PyPI-badge]][PyPI-link]
         [![license-badge]][license-link]
         
         ## Installation
         
         ### Using Anaconda
@@ -60,25 +63,30 @@
         On Windows, install the [Microsoft C++ Build Tools].
         
         #### FFTW
         
         To compile Stockwell, you will need to have [FFTW]
         installed.
         
-        If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
+        On Linux and macOS, you can download and compile FFTW from source using
+        the script `get_fftw3.sh`
         
-            conda install fftw
+        Alternatively, you can install FFTW using your package manager:
         
-        If you use Homebrew (macOS)
+        - If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
         
-            brew install fftw
+              conda install fftw
         
-        If you use `apt` (Debian or Ubuntu)
+        - If you use Homebrew (macOS)
         
-            sudo apt install libfftw3-dev
+              brew install fftw
+        
+        - If you use `apt` (Debian or Ubuntu)
+        
+              sudo apt install libfftw3-dev
         
         #### Install the Python package from source
         
         Finally, install this Python package using pip:
         
             pip install .
         
@@ -141,14 +149,16 @@
         spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
         doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
         
         [S transform on Wikipedia].
         
         [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
         
+        [changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+        [changelog-link]: https://github.com/claudiodsf/stockwell/blob/main/CHANGELOG.md
         [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
         [cf-link]: https://anaconda.org/conda-forge/stockwell
         [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
         [PyPI-link]: https://pypi.python.org/pypi/stockwell
         [license-badge]: https://img.shields.io/badge/license-GPLv3-green
         [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
         [releases-link]: https://github.com/claudiodsf/stockwell/releases
@@ -158,19 +168,19 @@
         https://visualstudio.microsoft.com/visual-cpp-build-tools
         [FFTW]: http://www.fftw.org
         [S transform on Wikipedia]: https://en.wikipedia.org/wiki/S_transform
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `stockwell-1.1/README.md` & `stockwell-1.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Stockwell
 
 Python package for time-frequency analysis through Stockwell transform.
 
 Based on original code from [NIMH MEG Core Facility].
 
+[![changelog-badge]][changelog-link]
 [![cf-badge]][cf-link]
 [![PyPI-badge]][PyPI-link]
 [![license-badge]][license-link]
 
 ## Installation
 
 ### Using Anaconda
@@ -52,25 +53,30 @@
 On Windows, install the [Microsoft C++ Build Tools].
 
 #### FFTW
 
 To compile Stockwell, you will need to have [FFTW]
 installed.
 
-If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
+On Linux and macOS, you can download and compile FFTW from source using
+the script `get_fftw3.sh`
 
-    conda install fftw
+Alternatively, you can install FFTW using your package manager:
 
-If you use Homebrew (macOS)
+- If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
 
-    brew install fftw
+      conda install fftw
 
-If you use `apt` (Debian or Ubuntu)
+- If you use Homebrew (macOS)
 
-    sudo apt install libfftw3-dev
+      brew install fftw
+
+- If you use `apt` (Debian or Ubuntu)
+
+      sudo apt install libfftw3-dev
 
 #### Install the Python package from source
 
 Finally, install this Python package using pip:
 
     pip install .
 
@@ -133,14 +139,16 @@
 spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
 doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
 
 [S transform on Wikipedia].
 
 [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
 
+[changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+[changelog-link]: https://github.com/claudiodsf/stockwell/blob/main/CHANGELOG.md
 [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
 [cf-link]: https://anaconda.org/conda-forge/stockwell
 [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
 [PyPI-link]: https://pypi.python.org/pypi/stockwell
 [license-badge]: https://img.shields.io/badge/license-GPLv3-green
 [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
 [releases-link]: https://github.com/claudiodsf/stockwell/releases
```

### Comparing `stockwell-1.1/pyproject.toml` & `stockwell-1.1.1/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -2,28 +2,28 @@
 requires = [
   'wheel',
   'setuptools',
   'numpy>=1.18'
 ]
 
 [tool.cibuildwheel]
-build = ['cp36-*', 'cp37-*', 'cp38-*', 'cp39-*', 'cp310-*']
+build = ['cp38-*', 'cp39-*', 'cp310-*', 'cp311-*', 'cp312-*']
 skip = '*-win32'
 test-requires = 'pytest'
 test-command = 'pytest --pyargs stockwell'
 
 [tool.cibuildwheel.linux]
 before-all = 'yum install -y fftw-devel'
 
 [[tool.cibuildwheel.overrides]]
 select = "*-musllinux*"
 before-all = "apk add fftw-dev"
 
 [tool.cibuildwheel.macos]
-before-all = 'brew install fftw'
+before-build = './get_fftw3.sh'
 
 [tool.cibuildwheel.windows]
 before-all = '%CONDA%\Scripts\conda.exe install fftw'
 before-build = 'pip install delvewheel'
 repair-wheel-command = 'delvewheel repair --add-path %CONDA%\Library\bin -w {dest_dir} {wheel}'
 test-requires = ''
 test-command = 'python -m stockwell.tests.test_stockwell'
```

### Comparing `stockwell-1.1/setup.py` & `stockwell-1.1.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,37 +1,53 @@
 # -*- coding: utf-8 -*-
 """setup.py: setuptools control."""
 import os
-from setuptools import setup
-from distutils.core import Extension
+from setuptools import setup, Extension
 import versioneer
 
 with open('README.md', 'rb') as f:
     long_descr = f.read().decode('utf-8').replace(
         '(stockwell.png)',
         '(https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/stockwell.png)'
     ).replace(
         '(inv_stockwell.png)',
         '(https://cdn.jsdelivr.net/gh/claudiodsf/stockwell/inv_stockwell.png)'
     )
 
+project_urls = {
+    'Homepage': 'https://github.com/claudiodsf/stockwell',
+    'Source': 'https://github.com/claudiodsf/stockwell',
+}
+
 include_dirs_st = []
 library_dirs_st = []
-# This seems necessary only for Windows
-if 'CONDA_PREFIX' in os.environ:
-    include_dirs_st.append(
-        os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'include'))
-    library_dirs_st.append(
-        os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'lib'))
-# This is needed for Miniconda on GitHub-hosted Windows runner
-if 'CONDA' in os.environ:
-    include_dirs_st.append(
-        os.path.join(os.environ['CONDA'], 'Library', 'include'))
-    library_dirs_st.append(
-        os.path.join(os.environ['CONDA'], 'Library', 'lib'))
+# First search for fftw3 in the current directory
+# (i.e., installed using the script "get_fftw3.sh")
+if os.path.exists('fftw3'):
+    include_dirs_st.append('fftw3/include')
+    library_dirs_st.append('fftw3/lib')
+else:
+    # Search Homebrew fftw3 on macOS
+    if 'HOMEBREW_PREFIX' in os.environ:
+        include_dirs_st.append(
+            os.path.join(os.environ['HOMEBREW_PREFIX'], 'include'))
+        library_dirs_st.append(
+            os.path.join(os.environ['HOMEBREW_PREFIX'], 'lib'))
+    # Search for a version of fftw3 provided by Conda
+    if 'CONDA_PREFIX' in os.environ:
+        include_dirs_st.append(
+            os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'include'))
+        library_dirs_st.append(
+            os.path.join(os.environ['CONDA_PREFIX'], 'Library', 'lib'))
+    # This is needed for Miniconda on GitHub-hosted Windows runner
+    if 'CONDA' in os.environ:
+        include_dirs_st.append(
+            os.path.join(os.environ['CONDA'], 'Library', 'include'))
+        library_dirs_st.append(
+            os.path.join(os.environ['CONDA'], 'Library', 'lib'))
 
 ext_modules = [
     Extension(
         'st',
         sources=['stockwell/c_libs/st.c'],
         include_dirs=include_dirs_st,
         library_dirs=library_dirs_st,
@@ -52,28 +68,29 @@
     ext_package='stockwell.lib',
     ext_modules=ext_modules,
     description='Time-frequency analysis through Stockwell transform',
     long_description=long_descr,
     long_description_content_type='text/markdown',
     author='Claudio Satriano',
     author_email='satriano@ipgp.fr',
-    url='https://github.com/claudiodsf/stockwell',
-    license='CeCILL Free Software License Agreement, Version 2.1',
+    url=project_urls['Homepage'],
+    project_urls=project_urls,
+    license='GNU General Public License v3 or later (GPLv3+)',
     platforms='OS Independent',
     classifiers=[
         'Development Status :: 5 - Production/Stable',
         'Environment :: Console',
         'Intended Audience :: Science/Research',
-        'License :: OSI Approved :: CEA CNRS Inria Logiciel Libre '
-            'License, version 2.1 (CeCILL-2.1)',
+        'License :: OSI Approved :: '
+            'GNU General Public License v3 or later (GPLv3+)',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering',
         'Topic :: Scientific/Engineering :: Physics'],
     install_requires=['numpy>=1.18']
     )
```

### Comparing `stockwell-1.1/stockwell/c_libs/sine.c` & `stockwell-1.1.1/stockwell/c_libs/sine.c`

 * *Files identical despite different names*

### Comparing `stockwell-1.1/stockwell/c_libs/st.c` & `stockwell-1.1.1/stockwell/c_libs/st.c`

 * *Files identical despite different names*

### Comparing `stockwell-1.1/stockwell/sine.py` & `stockwell-1.1.1/stockwell/sine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 """
 sine.py
 
 This file is part of the Stockwell project.
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>
 
 :license:
     GNU General Public License v3.0 or later.
     (https://www.gnu.org/licenses/gpl-3.0.html)
 """
-import numpy as np
 from ctypes import CDLL, POINTER, c_int, c_double, c_void_p
+import numpy as np
 from .lib_path import get_lib_path
 
 lib_sine = CDLL(get_lib_path('sine'))
 lib_sine.sine_taper.argtypes = [
     c_int,  # K
     c_int,  # N
     POINTER(c_double)  # d
```

### Comparing `stockwell-1.1/stockwell/st.py` & `stockwell-1.1.1/stockwell/st.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 """
 st.py
 
 This file is part of the Stockwell project.
 
 :copyright:
-    2023 Claudio Satriano <satriano@ipgp.fr>
+    2023-2024 Claudio Satriano <satriano@ipgp.fr>
 
 :license:
     GNU General Public License v3.0 or later.
     (https://www.gnu.org/licenses/gpl-3.0.html)
 """
-import numpy as np
 from ctypes import CDLL, POINTER, c_int, c_uint, c_double, c_void_p
+import numpy as np
 from .lib_path import get_lib_path
 
 lib_st = CDLL(get_lib_path('st'))
 lib_st.st.argtypes = [
     c_int,  # len
     c_int,  # lo
     c_int,  # hi
```

### Comparing `stockwell-1.1/stockwell.egg-info/PKG-INFO` & `stockwell-1.1.1/stockwell.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 Metadata-Version: 2.1
 Name: stockwell
-Version: 1.1
+Version: 1.1.1
 Summary: Time-frequency analysis through Stockwell transform
 Home-page: https://github.com/claudiodsf/stockwell
 Author: Claudio Satriano
 Author-email: satriano@ipgp.fr
-License: CeCILL Free Software License Agreement, Version 2.1
+License: GNU General Public License v3 or later (GPLv3+)
+Project-URL: Homepage, https://github.com/claudiodsf/stockwell
+Project-URL: Source, https://github.com/claudiodsf/stockwell
 Description: # Stockwell
         
         Python package for time-frequency analysis through Stockwell transform.
         
         Based on original code from [NIMH MEG Core Facility].
         
+        [![changelog-badge]][changelog-link]
         [![cf-badge]][cf-link]
         [![PyPI-badge]][PyPI-link]
         [![license-badge]][license-link]
         
         ## Installation
         
         ### Using Anaconda
@@ -60,25 +63,30 @@
         On Windows, install the [Microsoft C++ Build Tools].
         
         #### FFTW
         
         To compile Stockwell, you will need to have [FFTW]
         installed.
         
-        If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
+        On Linux and macOS, you can download and compile FFTW from source using
+        the script `get_fftw3.sh`
         
-            conda install fftw
+        Alternatively, you can install FFTW using your package manager:
         
-        If you use Homebrew (macOS)
+        - If you use [Anaconda]&nbsp;(Linux, macOS, Windows):
         
-            brew install fftw
+              conda install fftw
         
-        If you use `apt` (Debian or Ubuntu)
+        - If you use Homebrew (macOS)
         
-            sudo apt install libfftw3-dev
+              brew install fftw
+        
+        - If you use `apt` (Debian or Ubuntu)
+        
+              sudo apt install libfftw3-dev
         
         #### Install the Python package from source
         
         Finally, install this Python package using pip:
         
             pip install .
         
@@ -141,14 +149,16 @@
         spectrum: the S transform, IEEE Trans. Signal Process., 44(4), 998–1001,
         doi:[10.1109/78.492555](https://doi.org/10.1109/78.492555)
         
         [S transform on Wikipedia].
         
         [NIMH MEG Core Facility]: https://kurage.nimh.nih.gov/meglab/Meg/Stockwell
         
+        [changelog-badge]: https://img.shields.io/badge/Changelog-136CB6.svg
+        [changelog-link]: https://github.com/claudiodsf/stockwell/blob/main/CHANGELOG.md
         [cf-badge]: http://img.shields.io/conda/vn/conda-forge/stockwell.svg
         [cf-link]: https://anaconda.org/conda-forge/stockwell
         [PyPI-badge]: http://img.shields.io/pypi/v/stockwell.svg
         [PyPI-link]: https://pypi.python.org/pypi/stockwell
         [license-badge]: https://img.shields.io/badge/license-GPLv3-green
         [license-link]: https://www.gnu.org/licenses/gpl-3.0.html
         [releases-link]: https://github.com/claudiodsf/stockwell/releases
@@ -158,19 +168,19 @@
         https://visualstudio.microsoft.com/visual-cpp-build-tools
         [FFTW]: http://www.fftw.org
         [S transform on Wikipedia]: https://en.wikipedia.org/wiki/S_transform
 Platform: OS Independent
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: CEA CNRS Inria Logiciel Libre License, version 2.1 (CeCILL-2.1)
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Description-Content-Type: text/markdown
```

### Comparing `stockwell-1.1/stockwell.egg-info/SOURCES.txt` & `stockwell-1.1.1/stockwell.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `stockwell-1.1/versioneer.py` & `stockwell-1.1.1/versioneer.py`

 * *Files identical despite different names*

