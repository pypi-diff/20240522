# Comparing `tmp/farn-0.3.6.tar.gz` & `tmp/farn-0.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "farn-0.3.6.tar", last modified: Wed Feb 21 20:27:47 2024, max compression
+gzip compressed data, was "farn-0.3.7.tar", last modified: Wed May 22 17:37:00 2024, max compression
```

## Comparing `farn-0.3.6.tar` & `farn-0.3.7.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.220320 farn-0.3.6/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-21 20:27:28.000000 farn-0.3.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-21 20:27:28.000000 farn-0.3.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-02-21 20:27:47.220320 farn-0.3.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5384 2024-02-21 20:27:28.000000 farn-0.3.6/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5489 2024-02-21 20:27:28.000000 farn-0.3.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 20:27:47.220320 farn-0.3.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.212320 farn-0.3.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.212320 farn-0.3.6/src/farn/
--rw-r--r--   0 runner    (1001) docker     (127)      423 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/cli/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9418 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/cli/farn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/core/
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14146 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/core/case.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/core/parameter.py
--rw-r--r--   0 runner    (1001) docker     (127)    30187 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/farn.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/run/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/batchProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/run/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/cli/batchProcess.py
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/subProcess.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/run/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/run/utils/threading.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/sampling/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/sampling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26732 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/sampling/sampling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/src/farn/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-02-21 20:27:28.000000 farn-0.3.6/src/farn/utils/os.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.220320 farn-0.3.6/src/farn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8319 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       90 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-02-21 20:27:47.000000 farn-0.3.6/src/farn.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:27:47.216320 farn-0.3.6/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-02-21 20:27:28.000000 farn-0.3.6/tests/test_cases.py
--rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-02-21 20:27:28.000000 farn-0.3.6/tests/test_farn.py
--rw-r--r--   0 runner    (1001) docker     (127)    37806 2024-02-21 20:27:28.000000 farn-0.3.6/tests/test_sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.286530 farn-0.3.7/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 17:36:49.000000 farn-0.3.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 17:36:49.000000 farn-0.3.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-22 17:37:00.286530 farn-0.3.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5355 2024-05-22 17:36:49.000000 farn-0.3.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5457 2024-05-22 17:36:49.000000 farn-0.3.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 17:37:00.286530 farn-0.3.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.278530 farn-0.3.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/cli/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9508 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/cli/farn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/core/
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/core/case.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/core/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31101 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/farn.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/run/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/batchProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/run/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3969 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/cli/batchProcess.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/subProcess.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/run/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1818 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/run/utils/threading.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.282530 farn-0.3.7/src/farn/sampling/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26620 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/sampling/sampling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.286530 farn-0.3.7/src/farn/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3258 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-05-22 17:36:49.000000 farn-0.3.7/src/farn/utils/os.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.286530 farn-0.3.7/src/farn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8295 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       90 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-05-22 17:37:00.000000 farn-0.3.7/src/farn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 17:37:00.286530 farn-0.3.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    13275 2024-05-22 17:36:49.000000 farn-0.3.7/tests/test_cases.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10279 2024-05-22 17:36:49.000000 farn-0.3.7/tests/test_farn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37806 2024-05-22 17:36:49.000000 farn-0.3.7/tests/test_sampling.py
```

### Comparing `farn-0.3.6/LICENSE` & `farn-0.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/PKG-INFO` & `farn-0.3.7/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python package to generate an n-dimensional case folder structure applying linear and spatial sampling strategies.
 Author-email: Frank Lumpitzsch <frank.lumpitzsch@dnv.com>, Claas Rostock <claas.rostock@dnv.com>
 Maintainer-email: Claas Rostock <claas.rostock@dnv.com>
 License: MIT License
         
         Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
         
@@ -44,25 +44,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=5.1
-Requires-Dist: numpy>=1.26
-Requires-Dist: scipy>=1.12
+Requires-Dist: lxml>=5.2
+Requires-Dist: numpy<2.0,>=1.26
+Requires-Dist: scipy>=1.13
 Requires-Dist: pandas>=2.2
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: Pillow>=10.2
+Requires-Dist: matplotlib>=3.9
+Requires-Dist: Pillow>=10.3
 Requires-Dist: pyDOE3>=1.0
 Requires-Dist: psutil>=5.9
 Requires-Dist: hilbertcurve>=2.0.5
-Requires-Dist: dictIO>=0.3.3
-Requires-Dist: ospx>=0.2.13
+Requires-Dist: dictIO>=0.3.4
+Requires-Dist: ospx>=0.2.14
 
 # farn
 [farn][farn_docs] is an n-dimensional case generator.
 
 Its primary design goal is to parameterize and execute simulation cases.
 However, at its core, farn is use-case agnostic and can support a wide spectrum of applications.
 
@@ -181,32 +181,32 @@
 
     ```sh
     (.venv) $ pytest .
     ```
 
 ## Meta
 
-Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2024 [DNV](https://www.dnv.com) SE. All rights reserved.
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
 
 Distributed under the MIT license. See [LICENSE](LICENSE.md) for more information.
 
 [https://github.com/dnv-opensource/farn](https://github.com/dnv-opensource/farn)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/farn/fork>)
-2. Create your branch (`git checkout -b myBranchName`)
-3. Commit your changes (e.g. `git commit -m 'place a descriptive commit message here'`)
-4. Push to the branch (e.g. `git push origin myBranchName`)
+2. Create your branch (`git checkout -b my-branch-name`)
+3. Commit your changes (`git commit -am 'place a descriptive commit message here'`)
+4. Push to the branch (`git push origin my-branch-name`)
 5. Create a new Pull Request in GitHub
 
 For your contribution, please make sure you follow the [STYLEGUIDE](STYLEGUIDE.md) before creating the Pull Request.
 
 <!-- Markdown link & img dfn's -->
 [dictIO_docs]: https://dnv-opensource.github.io/dictIO/README.html
 [ospx_docs]: https://dnv-opensource.github.io/ospx/README.html
```

### Comparing `farn-0.3.6/README.md` & `farn-0.3.7/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -119,32 +119,32 @@
 
     ```sh
     (.venv) $ pytest .
     ```
 
 ## Meta
 
-Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2024 [DNV](https://www.dnv.com) SE. All rights reserved.
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
 
 Distributed under the MIT license. See [LICENSE](LICENSE.md) for more information.
 
 [https://github.com/dnv-opensource/farn](https://github.com/dnv-opensource/farn)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/farn/fork>)
-2. Create your branch (`git checkout -b myBranchName`)
-3. Commit your changes (e.g. `git commit -m 'place a descriptive commit message here'`)
-4. Push to the branch (e.g. `git push origin myBranchName`)
+2. Create your branch (`git checkout -b my-branch-name`)
+3. Commit your changes (`git commit -am 'place a descriptive commit message here'`)
+4. Push to the branch (`git push origin my-branch-name`)
 5. Create a new Pull Request in GitHub
 
 For your contribution, please make sure you follow the [STYLEGUIDE](STYLEGUIDE.md) before creating the Pull Request.
 
 <!-- Markdown link & img dfn's -->
 [dictIO_docs]: https://dnv-opensource.github.io/dictIO/README.html
 [ospx_docs]: https://dnv-opensource.github.io/ospx/README.html
```

### Comparing `farn-0.3.6/pyproject.toml` & `farn-0.3.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6661 726e 220d 0a76 6572 7369 6f6e   "farn"..version
-00000080: 203d 2022 302e 332e 3622 0d0a 6465 7363   = "0.3.6"..desc
+00000080: 203d 2022 302e 332e 3722 0d0a 6465 7363   = "0.3.7"..desc
 00000090: 7269 7074 696f 6e20 3d20 2250 7974 686f  ription = "Pytho
 000000a0: 6e20 7061 636b 6167 6520 746f 2067 656e  n package to gen
 000000b0: 6572 6174 6520 616e 206e 2d64 696d 656e  erate an n-dimen
 000000c0: 7369 6f6e 616c 2063 6173 6520 666f 6c64  sional case fold
 000000d0: 6572 2073 7472 7563 7475 7265 2061 7070  er structure app
 000000e0: 6c79 696e 6720 6c69 6e65 6172 2061 6e64  lying linear and
 000000f0: 2073 7061 7469 616c 2073 616d 706c 696e   spatial samplin
@@ -74,271 +74,269 @@
 00000490: 6669 632f 456e 6769 6e65 6572 696e 6722  fic/Engineering"
 000004a0: 2c0d 0a20 2020 2022 546f 7069 6320 3a3a  ,..    "Topic ::
 000004b0: 2053 6f66 7477 6172 6520 4465 7665 6c6f   Software Develo
 000004c0: 706d 656e 7420 3a3a 204c 6962 7261 7269  pment :: Librari
 000004d0: 6573 203a 3a20 5079 7468 6f6e 204d 6f64  es :: Python Mod
 000004e0: 756c 6573 222c 0d0a 5d0d 0a64 6570 656e  ules",..]..depen
 000004f0: 6465 6e63 6965 7320 3d20 5b0d 0a20 2020  dencies = [..   
-00000500: 2022 6c78 6d6c 3e3d 352e 3122 2c0d 0a20   "lxml>=5.1",.. 
-00000510: 2020 2022 6e75 6d70 793e 3d31 2e32 3622     "numpy>=1.26"
-00000520: 2c0d 0a20 2020 2022 7363 6970 793e 3d31  ,..    "scipy>=1
-00000530: 2e31 3222 2c0d 0a20 2020 2022 7061 6e64  .12",..    "pand
-00000540: 6173 3e3d 322e 3222 2c0d 0a20 2020 2022  as>=2.2",..    "
-00000550: 6d61 7470 6c6f 746c 6962 3e3d 332e 3822  matplotlib>=3.8"
-00000560: 2c0d 0a20 2020 2022 5069 6c6c 6f77 3e3d  ,..    "Pillow>=
-00000570: 3130 2e32 222c 0d0a 2020 2020 2270 7944  10.2",..    "pyD
-00000580: 4f45 333e 3d31 2e30 222c 0d0a 2020 2020  OE3>=1.0",..    
-00000590: 2270 7375 7469 6c3e 3d35 2e39 222c 0d0a  "psutil>=5.9",..
-000005a0: 2020 2020 2268 696c 6265 7274 6375 7276      "hilbertcurv
-000005b0: 653e 3d32 2e30 2e35 222c 0d0a 2020 2020  e>=2.0.5",..    
-000005c0: 2264 6963 7449 4f3e 3d30 2e33 2e33 222c  "dictIO>=0.3.3",
-000005d0: 0d0a 2020 2020 226f 7370 783e 3d30 2e32  ..    "ospx>=0.2
-000005e0: 2e31 3322 2c0d 0a5d 0d0a 0d0a 5b70 726f  .13",..]....[pro
-000005f0: 6a65 6374 2e75 726c 735d 0d0a 486f 6d65  ject.urls]..Home
-00000600: 7061 6765 203d 2022 6874 7470 733a 2f2f  page = "https://
-00000610: 6769 7468 7562 2e63 6f6d 2f64 6e76 2d6f  github.com/dnv-o
-00000620: 7065 6e73 6f75 7263 652f 6661 726e 220d  pensource/farn".
-00000630: 0a44 6f63 756d 656e 7461 7469 6f6e 203d  .Documentation =
-00000640: 2022 6874 7470 733a 2f2f 646e 762d 6f70   "https://dnv-op
-00000650: 656e 736f 7572 6365 2e67 6974 6875 622e  ensource.github.
-00000660: 696f 2f66 6172 6e2f 5245 4144 4d45 2e68  io/farn/README.h
-00000670: 746d 6c22 0d0a 5265 706f 7369 746f 7279  tml"..Repository
-00000680: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
-00000690: 7562 2e63 6f6d 2f64 6e76 2d6f 7065 6e73  ub.com/dnv-opens
-000006a0: 6f75 7263 652f 6661 726e 2e67 6974 220d  ource/farn.git".
-000006b0: 0a49 7373 7565 7320 3d20 2268 7474 7073  .Issues = "https
-000006c0: 3a2f 2f67 6974 6875 622e 636f 6d2f 646e  ://github.com/dn
-000006d0: 762d 6f70 656e 736f 7572 6365 2f66 6172  v-opensource/far
-000006e0: 6e2f 6973 7375 6573 220d 0a43 6861 6e67  n/issues"..Chang
-000006f0: 656c 6f67 203d 2022 6874 7470 733a 2f2f  elog = "https://
-00000700: 6769 7468 7562 2e63 6f6d 2f64 6e76 2d6f  github.com/dnv-o
-00000710: 7065 6e73 6f75 7263 652f 6661 726e 2f62  pensource/farn/b
-00000720: 6c6f 622f 6d61 696e 2f43 4841 4e47 454c  lob/main/CHANGEL
-00000730: 4f47 2e6d 6422 0d0a 0d0a 5b70 726f 6a65  OG.md"....[proje
-00000740: 6374 2e73 6372 6970 7473 5d0d 0a66 6172  ct.scripts]..far
-00000750: 6e20 3d20 2266 6172 6e2e 636c 692e 6661  n = "farn.cli.fa
-00000760: 726e 3a6d 6169 6e22 0d0a 6261 7463 6850  rn:main"..batchP
-00000770: 726f 6365 7373 203d 2022 6661 726e 2e72  rocess = "farn.r
-00000780: 756e 2e63 6c69 2e62 6174 6368 5072 6f63  un.cli.batchProc
-00000790: 6573 733a 6d61 696e 220d 0a0d 0a5b 746f  ess:main"....[to
-000007a0: 6f6c 2e73 6574 7570 746f 6f6c 732e 7061  ol.setuptools.pa
-000007b0: 636b 6167 6573 2e66 696e 645d 0d0a 7768  ckages.find]..wh
-000007c0: 6572 6520 3d20 5b22 7372 6322 5d0d 0a65  ere = ["src"]..e
-000007d0: 7863 6c75 6465 203d 205b 2274 6573 742a  xclude = ["test*
-000007e0: 225d 0d0a 0d0a 5b74 6f6f 6c2e 626c 6163  "]....[tool.blac
-000007f0: 6b5d 0d0a 6c69 6e65 2d6c 656e 6774 6820  k]..line-length 
-00000800: 3d20 3132 300d 0a74 6172 6765 742d 7665  = 120..target-ve
-00000810: 7273 696f 6e20 3d20 5b22 7079 3339 222c  rsion = ["py39",
-00000820: 2022 7079 3331 3022 2c20 2270 7933 3131   "py310", "py311
-00000830: 222c 2022 7079 3331 3222 5d0d 0a0d 0a5b  ", "py312"]....[
-00000840: 746f 6f6c 2e72 7566 665d 0d0a 6578 636c  tool.ruff]..excl
-00000850: 7564 6520 3d20 5b0d 0a20 2020 2022 2e67  ude = [..    ".g
-00000860: 6974 222c 0d0a 2020 2020 222e 7665 6e76  it",..    ".venv
-00000870: 222c 0d0a 2020 2020 222e 746f 7822 2c0d  ",..    ".tox",.
-00000880: 0a20 2020 2022 6275 696c 6422 2c0d 0a20  .    "build",.. 
-00000890: 2020 2022 6469 7374 222c 0d0a 2020 2020     "dist",..    
-000008a0: 225f 5f70 7963 6163 6865 5f5f 222c 0d0a  "__pycache__",..
-000008b0: 2020 2020 222e 2f64 6f63 732f 736f 7572      "./docs/sour
-000008c0: 6365 2f63 6f6e 662e 7079 222c 0d0a 5d0d  ce/conf.py",..].
-000008d0: 0a73 7263 203d 205b 2273 7263 225d 0d0a  .src = ["src"]..
-000008e0: 6c69 6e65 2d6c 656e 6774 6820 3d20 3132  line-length = 12
-000008f0: 300d 0a74 6172 6765 742d 7665 7273 696f  0..target-versio
-00000900: 6e20 3d20 2270 7933 3922 0d0a 0d0a 5b74  n = "py39"....[t
-00000910: 6f6f 6c2e 7275 6666 2e6c 696e 745d 0d0a  ool.ruff.lint]..
-00000920: 6967 6e6f 7265 203d 205b 0d0a 2020 2020  ignore = [..    
-00000930: 2245 3530 3122 2c20 2023 204c 696e 6520  "E501",  # Line 
-00000940: 6c65 6e67 7468 2074 6f6f 206c 6f6e 670d  length too long.
-00000950: 0a20 2020 2022 4431 3030 222c 2020 2320  .    "D100",  # 
-00000960: 4d69 7373 696e 6720 646f 6373 7472 696e  Missing docstrin
-00000970: 6720 696e 2070 7562 6c69 6320 6d6f 6475  g in public modu
-00000980: 6c65 0d0a 2020 2020 2244 3130 3422 2c20  le..    "D104", 
-00000990: 2023 204d 6973 7369 6e67 2064 6f63 7374   # Missing docst
-000009a0: 7269 6e67 2069 6e20 7075 626c 6963 2070  ring in public p
-000009b0: 6163 6b61 6765 0d0a 2020 2020 2244 3130  ackage..    "D10
-000009c0: 3522 2c20 2023 204d 6973 7369 6e67 2064  5",  # Missing d
-000009d0: 6f63 7374 7269 6e67 2069 6e20 6d61 6769  ocstring in magi
-000009e0: 6320 6d65 7468 6f64 0d0a 2020 2020 2244  c method..    "D
-000009f0: 3130 3722 2c20 2023 204d 6973 7369 6e67  107",  # Missing
-00000a00: 2064 6f63 7374 7269 6e67 2069 6e20 5f5f   docstring in __
-00000a10: 696e 6974 5f5f 0d0a 2020 2020 2244 3230  init__..    "D20
-00000a20: 3222 2c20 2023 204e 6f20 626c 616e 6b20  2",  # No blank 
-00000a30: 6c69 6e65 7320 616c 6c6f 7765 6420 6166  lines allowed af
-00000a40: 7465 7220 6675 6e63 7469 6f6e 2064 6f63  ter function doc
-00000a50: 7374 7269 6e67 0d0a 2020 2020 2244 3230  string..    "D20
-00000a60: 3322 2c20 2023 2031 2062 6c61 6e6b 206c  3",  # 1 blank l
-00000a70: 696e 6520 7265 7175 6972 6564 2062 6566  ine required bef
-00000a80: 6f72 6520 636c 6173 7320 646f 6373 7472  ore class docstr
-00000a90: 696e 670d 0a20 2020 2022 4432 3035 222c  ing..    "D205",
-00000aa0: 2020 2320 3120 626c 616e 6b20 6c69 6e65    # 1 blank line
-00000ab0: 2072 6571 7569 7265 6420 6265 7477 6565   required betwee
-00000ac0: 6e20 7375 6d6d 6172 7920 6c69 6e65 2061  n summary line a
-00000ad0: 6e64 2064 6573 6372 6970 7469 6f6e 0d0a  nd description..
-00000ae0: 2020 2020 2244 3231 3222 2c20 2023 204d      "D212",  # M
-00000af0: 756c 7469 2d6c 696e 6520 646f 6373 7472  ulti-line docstr
-00000b00: 696e 6720 7375 6d6d 6172 7920 7368 6f75  ing summary shou
-00000b10: 6c64 2073 7461 7274 2061 7420 7468 6520  ld start at the 
-00000b20: 6669 7273 7420 6c69 6e65 0d0a 2020 2020  first line..    
-00000b30: 2244 3231 3322 2c20 2023 204d 756c 7469  "D213",  # Multi
-00000b40: 2d6c 696e 6520 646f 6373 7472 696e 6720  -line docstring 
-00000b50: 7375 6d6d 6172 7920 7368 6f75 6c64 2073  summary should s
-00000b60: 7461 7274 2061 7420 7468 6520 7365 636f  tart at the seco
-00000b70: 6e64 206c 696e 650d 0a20 2020 2023 2022  nd line..    # "
-00000b80: 4e38 3032 222c 2020 2320 4675 6e63 7469  N802",  # Functi
-00000b90: 6f6e 206e 616d 6520 7368 6f75 6c64 2062  on name should b
-00000ba0: 6520 6c6f 7765 7263 6173 6520 2028 756e  e lowercase  (un
-00000bb0: 636f 6d6d 656e 7420 6966 2079 6f75 2077  comment if you w
-00000bc0: 616e 7420 746f 2061 6c6c 6f77 2055 7070  ant to allow Upp
-00000bd0: 6572 6361 7365 2066 756e 6374 696f 6e20  ercase function 
-00000be0: 6e61 6d65 7329 0d0a 2020 2020 2320 224e  names)..    # "N
-00000bf0: 3830 3322 2c20 2023 2041 7267 756d 656e  803",  # Argumen
-00000c00: 7420 6e61 6d65 2073 686f 756c 6420 6265  t name should be
-00000c10: 206c 6f77 6572 6361 7365 2020 2875 6e63   lowercase  (unc
-00000c20: 6f6d 6d65 6e74 2069 6620 796f 7520 7761  omment if you wa
-00000c30: 6e74 2074 6f20 616c 6c6f 7720 5570 7065  nt to allow Uppe
-00000c40: 7263 6173 6520 6172 6775 6d65 6e74 206e  rcase argument n
-00000c50: 616d 6573 290d 0a20 2020 2022 4e38 3036  ames)..    "N806
-00000c60: 222c 2020 2320 5661 7269 6162 6c65 2069  ",  # Variable i
-00000c70: 6e20 6675 6e63 7469 6f6e 2073 686f 756c  n function shoul
-00000c80: 6420 6265 206c 6f77 6572 6361 7365 2020  d be lowercase  
-00000c90: 2875 6e63 6f6d 6d65 6e74 2069 6620 796f  (uncomment if yo
-00000ca0: 7520 7761 6e74 2074 6f20 616c 6c6f 7720  u want to allow 
-00000cb0: 5570 7065 7263 6173 6520 7661 7269 6162  Uppercase variab
-00000cc0: 6c65 206e 616d 6573 2069 6e20 6675 6e63  le names in func
-00000cd0: 7469 6f6e 7329 0d0a 2020 2020 2320 224e  tions)..    # "N
-00000ce0: 3831 3522 2c20 2023 2056 6172 6961 626c  815",  # Variabl
-00000cf0: 6520 696e 2063 6c61 7373 2073 636f 7065  e in class scope
-00000d00: 2073 686f 756c 6420 6e6f 7420 6265 206d   should not be m
-00000d10: 6978 6564 4361 7365 2020 2875 6e63 6f6d  ixedCase  (uncom
-00000d20: 6d65 6e74 2069 6620 796f 7520 7761 6e74  ment if you want
-00000d30: 2074 6f20 616c 6c6f 7720 6d69 7865 6443   to allow mixedC
-00000d40: 6173 6520 7661 7269 6162 6c65 206e 616d  ase variable nam
-00000d50: 6573 2069 6e20 636c 6173 7320 7363 6f70  es in class scop
-00000d60: 6529 0d0a 2020 2020 2320 224e 3831 3622  e)..    # "N816"
-00000d70: 2c20 2023 2056 6172 6961 626c 6520 696e  ,  # Variable in
-00000d80: 2067 6c6f 6261 6c20 7363 6f70 6520 7368   global scope sh
-00000d90: 6f75 6c64 206e 6f74 2062 6520 6d69 7865  ould not be mixe
-00000da0: 6443 6173 6520 2028 756e 636f 6d6d 656e  dCase  (uncommen
-00000db0: 7420 6966 2079 6f75 2077 616e 7420 746f  t if you want to
-00000dc0: 2061 6c6c 6f77 206d 6978 6564 4361 7365   allow mixedCase
-00000dd0: 2076 6172 6961 626c 6520 6e61 6d65 7320   variable names 
-00000de0: 696e 2067 6c6f 6261 6c20 7363 6f70 6529  in global scope)
-00000df0: 0d0a 2020 2020 224e 3939 3922 2c20 2023  ..    "N999",  #
-00000e00: 2049 6e76 616c 6964 206d 6f64 756c 6520   Invalid module 
-00000e10: 6e61 6d65 0d0a 2020 2020 5d0d 0a73 656c  name..    ]..sel
-00000e20: 6563 7420 3d20 5b0d 0a20 2020 2022 4522  ect = [..    "E"
-00000e30: 2c0d 0a20 2020 2022 4422 2c0d 0a20 2020  ,..    "D",..   
-00000e40: 2022 4622 2c0d 0a20 2020 2022 4e22 2c0d   "F",..    "N",.
-00000e50: 0a20 2020 2022 5722 2c0d 0a20 2020 2022  .    "W",..    "
-00000e60: 4922 2c0d 0a20 2020 2022 4222 2c0d 0a5d  I",..    "B",..]
-00000e70: 0d0a 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666  ......[tool.ruff
-00000e80: 2e6c 696e 742e 7065 7038 2d6e 616d 696e  .lint.pep8-namin
-00000e90: 675d 0d0a 6967 6e6f 7265 2d6e 616d 6573  g]..ignore-names
-00000ea0: 203d 205b 0d0a 2020 2020 2274 6573 745f   = [..    "test_
-00000eb0: 2a22 2c0d 0a20 2020 2022 7365 7455 7022  *",..    "setUp"
-00000ec0: 2c0d 0a20 2020 2022 7465 6172 446f 776e  ,..    "tearDown
-00000ed0: 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e72  ",..]....[tool.r
-00000ee0: 7566 662e 6c69 6e74 2e70 7964 6f63 7374  uff.lint.pydocst
-00000ef0: 796c 655d 0d0a 636f 6e76 656e 7469 6f6e  yle]..convention
-00000f00: 203d 2022 6e75 6d70 7922 0d0a 0d0a 5b74   = "numpy"....[t
-00000f10: 6f6f 6c2e 7275 6666 2e6c 696e 742e 7065  ool.ruff.lint.pe
-00000f20: 722d 6669 6c65 2d69 676e 6f72 6573 5d0d  r-file-ignores].
-00000f30: 0a22 5f5f 696e 6974 5f5f 2e70 7922 203d  ."__init__.py" =
-00000f40: 205b 2249 3030 3122 5d0d 0a22 2e2f 7465   ["I001"].."./te
-00000f50: 7374 732f 2a22 203d 205b 2244 225d 0d0a  sts/*" = ["D"]..
-00000f60: 0d0a 5b74 6f6f 6c2e 7079 7269 6768 745d  ..[tool.pyright]
-00000f70: 0d0a 6578 636c 7564 6520 3d20 5b0d 0a20  ..exclude = [.. 
-00000f80: 2020 2022 2e67 6974 222c 0d0a 2020 2020     ".git",..    
-00000f90: 222e 7665 6e76 222c 0d0a 2020 2020 222e  ".venv",..    ".
-00000fa0: 746f 7822 2c0d 0a20 2020 2022 6275 696c  tox",..    "buil
-00000fb0: 6422 2c0d 0a20 2020 2022 6469 7374 222c  d",..    "dist",
-00000fc0: 0d0a 2020 2020 222a 2a2f 5f5f 7079 6361  ..    "**/__pyca
-00000fd0: 6368 655f 5f22 2c0d 0a20 2020 2022 2e2f  che__",..    "./
-00000fe0: 646f 6373 2f73 6f75 7263 652f 636f 6e66  docs/source/conf
-00000ff0: 2e70 7922 2c0d 0a20 2020 2022 2e2f 7665  .py",..    "./ve
-00001000: 6e76 222c 0d0a 5d0d 0a65 7874 7261 5061  nv",..]..extraPa
-00001010: 7468 7320 3d20 5b22 2e2f 7372 6322 5d0d  ths = ["./src"].
-00001020: 0a74 7970 6543 6865 636b 696e 674d 6f64  .typeCheckingMod
-00001030: 6520 3d20 2262 6173 6963 220d 0a75 7365  e = "basic"..use
-00001040: 4c69 6272 6172 7943 6f64 6546 6f72 5479  LibraryCodeForTy
-00001050: 7065 7320 3d20 7472 7565 0d0a 7265 706f  pes = true..repo
-00001060: 7274 4d69 7373 696e 6750 6172 616d 6574  rtMissingParamet
-00001070: 6572 5479 7065 203d 2022 6572 726f 7222  erType = "error"
-00001080: 0d0a 7265 706f 7274 556e 6b6e 6f77 6e50  ..reportUnknownP
-00001090: 6172 616d 6574 6572 5479 7065 203d 2022  arameterType = "
-000010a0: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
-000010b0: 556e 6b6e 6f77 6e4d 656d 6265 7254 7970  UnknownMemberTyp
-000010c0: 6520 3d20 2277 6172 6e69 6e67 220d 0a72  e = "warning"..r
-000010d0: 6570 6f72 744d 6973 7369 6e67 5479 7065  eportMissingType
-000010e0: 4172 6775 6d65 6e74 203d 2022 6572 726f  Argument = "erro
-000010f0: 7222 0d0a 7265 706f 7274 5072 6f70 6572  r"..reportProper
-00001100: 7479 5479 7065 4d69 736d 6174 6368 203d  tyTypeMismatch =
-00001110: 2022 6572 726f 7222 0d0a 7265 706f 7274   "error"..report
-00001120: 4675 6e63 7469 6f6e 4d65 6d62 6572 4163  FunctionMemberAc
-00001130: 6365 7373 203d 2022 7761 726e 696e 6722  cess = "warning"
-00001140: 0d0a 7265 706f 7274 5072 6976 6174 6555  ..reportPrivateU
-00001150: 7361 6765 203d 2022 7761 726e 696e 6722  sage = "warning"
-00001160: 0d0a 7265 706f 7274 5479 7065 436f 6d6d  ..reportTypeComm
-00001170: 656e 7455 7361 6765 203d 2022 7761 726e  entUsage = "warn
-00001180: 696e 6722 0d0a 7265 706f 7274 496e 636f  ing"..reportInco
-00001190: 6d70 6174 6962 6c65 4d65 7468 6f64 4f76  mpatibleMethodOv
-000011a0: 6572 7269 6465 203d 2022 7761 726e 696e  erride = "warnin
-000011b0: 6722 0d0a 7265 706f 7274 496e 636f 6d70  g"..reportIncomp
-000011c0: 6174 6962 6c65 5661 7269 6162 6c65 4f76  atibleVariableOv
-000011d0: 6572 7269 6465 203d 2022 6572 726f 7222  erride = "error"
-000011e0: 0d0a 7265 706f 7274 496e 636f 6e73 6973  ..reportInconsis
-000011f0: 7465 6e74 436f 6e73 7472 7563 746f 7220  tentConstructor 
-00001200: 3d20 2265 7272 6f72 220d 0a72 6570 6f72  = "error"..repor
-00001210: 744f 7665 726c 6170 7069 6e67 4f76 6572  tOverlappingOver
-00001220: 6c6f 6164 203d 2022 7761 726e 696e 6722  load = "warning"
-00001230: 0d0a 7265 706f 7274 556e 696e 6974 6961  ..reportUninitia
-00001240: 6c69 7a65 6449 6e73 7461 6e63 6556 6172  lizedInstanceVar
-00001250: 6961 626c 6520 3d20 2277 6172 6e69 6e67  iable = "warning
-00001260: 220d 0a72 6570 6f72 7443 616c 6c49 6e44  "..reportCallInD
-00001270: 6566 6175 6c74 496e 6974 6961 6c69 7a65  efaultInitialize
-00001280: 7220 3d20 2277 6172 6e69 6e67 220d 0a72  r = "warning"..r
-00001290: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
-000012a0: 4973 496e 7374 616e 6365 203d 2022 696e  IsInstance = "in
-000012b0: 666f 726d 6174 696f 6e22 0d0a 7265 706f  formation"..repo
-000012c0: 7274 556e 6e65 6365 7373 6172 7943 6173  rtUnnecessaryCas
-000012d0: 7420 3d20 2277 6172 6e69 6e67 220d 0a72  t = "warning"..r
-000012e0: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
-000012f0: 436f 6d70 6172 6973 6f6e 203d 2022 7761  Comparison = "wa
-00001300: 726e 696e 6722 0d0a 7265 706f 7274 556e  rning"..reportUn
-00001310: 6e65 6365 7373 6172 7943 6f6e 7461 696e  necessaryContain
-00001320: 7320 3d20 2277 6172 6e69 6e67 220d 0a72  s = "warning"..r
-00001330: 6570 6f72 7455 6e75 7365 6443 616c 6c52  eportUnusedCallR
-00001340: 6573 756c 7420 3d20 2277 6172 6e69 6e67  esult = "warning
-00001350: 220d 0a72 6570 6f72 7455 6e75 7365 6445  "..reportUnusedE
-00001360: 7870 7265 7373 696f 6e20 3d20 2277 6172  xpression = "war
-00001370: 6e69 6e67 220d 0a72 6570 6f72 744d 6174  ning"..reportMat
-00001380: 6368 4e6f 7445 7868 6175 7374 6976 6520  chNotExhaustive 
-00001390: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-000013a0: 6f72 7453 6861 646f 7765 6449 6d70 6f72  ortShadowedImpor
-000013b0: 7473 203d 2022 7761 726e 696e 6722 0d0a  ts = "warning"..
-000013c0: 7265 706f 7274 556e 7479 7065 6446 756e  reportUntypedFun
-000013d0: 6374 696f 6e44 6563 6f72 6174 6f72 203d  ctionDecorator =
-000013e0: 2022 7761 726e 696e 6722 0d0a 7265 706f   "warning"..repo
-000013f0: 7274 556e 7479 7065 6442 6173 6543 6c61  rtUntypedBaseCla
-00001400: 7373 203d 2022 6572 726f 7222 0d0a 7265  ss = "error"..re
-00001410: 706f 7274 556e 7479 7065 644e 616d 6564  portUntypedNamed
-00001420: 5475 706c 6520 3d20 2277 6172 6e69 6e67  Tuple = "warning
-00001430: 220d 0a23 2041 6374 6976 6174 6520 7468  "..# Activate th
-00001440: 6520 666f 6c6c 6f77 696e 6720 7275 6c65  e following rule
-00001450: 7320 6f6e 6c79 206c 6f63 616c 6c79 2061  s only locally a
-00001460: 6e64 2074 656d 706f 7261 7279 2c20 692e  nd temporary, i.
-00001470: 652e 2066 6f72 2061 2051 4120 7365 7373  e. for a QA sess
-00001480: 696f 6e2e 0d0a 2320 2846 6f72 2073 6572  ion...# (For ser
-00001490: 7665 7220 7369 6465 2043 4920 7468 6579  ver side CI they
-000014a0: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
-000014b0: 746f 6f20 7374 7269 6374 2e29 0d0a 2320  too strict.)..# 
-000014c0: 7265 706f 7274 436f 6e73 7461 6e74 5265  reportConstantRe
-000014d0: 6465 6669 6e69 7469 6f6e 203d 2022 7761  definition = "wa
-000014e0: 726e 696e 6722 0d0a 2320 7265 706f 7274  rning"..# report
-000014f0: 556e 6e65 6365 7373 6172 7954 7970 6549  UnnecessaryTypeI
-00001500: 676e 6f72 6543 6f6d 6d65 6e74 203d 2022  gnoreComment = "
-00001510: 696e 666f 726d 6174 696f 6e22 0d0a 2320  information"..# 
-00001520: 7265 706f 7274 496d 706f 7274 4379 636c  reportImportCycl
-00001530: 6573 203d 2022 7761 726e 696e 6722 0d0a  es = "warning"..
-00001540: 2320 7265 706f 7274 496d 706c 6963 6974  # reportImplicit
-00001550: 5374 7269 6e67 436f 6e63 6174 656e 6174  StringConcatenat
-00001560: 696f 6e20 3d20 2277 6172 6e69 6e67 220d  ion = "warning".
-00001570: 0a                                       .
+00000500: 2022 6c78 6d6c 3e3d 352e 3222 2c0d 0a20   "lxml>=5.2",.. 
+00000510: 2020 2022 6e75 6d70 793e 3d31 2e32 362c     "numpy>=1.26,
+00000520: 3c32 2e30 222c 0d0a 2020 2020 2273 6369  <2.0",..    "sci
+00000530: 7079 3e3d 312e 3133 222c 0d0a 2020 2020  py>=1.13",..    
+00000540: 2270 616e 6461 733e 3d32 2e32 222c 0d0a  "pandas>=2.2",..
+00000550: 2020 2020 226d 6174 706c 6f74 6c69 623e      "matplotlib>
+00000560: 3d33 2e39 222c 0d0a 2020 2020 2250 696c  =3.9",..    "Pil
+00000570: 6c6f 773e 3d31 302e 3322 2c0d 0a20 2020  low>=10.3",..   
+00000580: 2022 7079 444f 4533 3e3d 312e 3022 2c0d   "pyDOE3>=1.0",.
+00000590: 0a20 2020 2022 7073 7574 696c 3e3d 352e  .    "psutil>=5.
+000005a0: 3922 2c0d 0a20 2020 2022 6869 6c62 6572  9",..    "hilber
+000005b0: 7463 7572 7665 3e3d 322e 302e 3522 2c0d  tcurve>=2.0.5",.
+000005c0: 0a20 2020 2022 6469 6374 494f 3e3d 302e  .    "dictIO>=0.
+000005d0: 332e 3422 2c0d 0a20 2020 2022 6f73 7078  3.4",..    "ospx
+000005e0: 3e3d 302e 322e 3134 222c 0d0a 5d0d 0a0d  >=0.2.14",..]...
+000005f0: 0a5b 7072 6f6a 6563 742e 7572 6c73 5d0d  .[project.urls].
+00000600: 0a48 6f6d 6570 6167 6520 3d20 2268 7474  .Homepage = "htt
+00000610: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000620: 646e 762d 6f70 656e 736f 7572 6365 2f66  dnv-opensource/f
+00000630: 6172 6e22 0d0a 446f 6375 6d65 6e74 6174  arn"..Documentat
+00000640: 696f 6e20 3d20 2268 7474 7073 3a2f 2f64  ion = "https://d
+00000650: 6e76 2d6f 7065 6e73 6f75 7263 652e 6769  nv-opensource.gi
+00000660: 7468 7562 2e69 6f2f 6661 726e 2f52 4541  thub.io/farn/REA
+00000670: 444d 452e 6874 6d6c 220d 0a52 6570 6f73  DME.html"..Repos
+00000680: 6974 6f72 7920 3d20 2268 7474 7073 3a2f  itory = "https:/
+00000690: 2f67 6974 6875 622e 636f 6d2f 646e 762d  /github.com/dnv-
+000006a0: 6f70 656e 736f 7572 6365 2f66 6172 6e2e  opensource/farn.
+000006b0: 6769 7422 0d0a 4973 7375 6573 203d 2022  git"..Issues = "
+000006c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
+000006d0: 6f6d 2f64 6e76 2d6f 7065 6e73 6f75 7263  om/dnv-opensourc
+000006e0: 652f 6661 726e 2f69 7373 7565 7322 0d0a  e/farn/issues"..
+000006f0: 4368 616e 6765 6c6f 6720 3d20 2268 7474  Changelog = "htt
+00000700: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000710: 646e 762d 6f70 656e 736f 7572 6365 2f66  dnv-opensource/f
+00000720: 6172 6e2f 626c 6f62 2f6d 6169 6e2f 4348  arn/blob/main/CH
+00000730: 414e 4745 4c4f 472e 6d64 220d 0a0d 0a5b  ANGELOG.md"....[
+00000740: 7072 6f6a 6563 742e 7363 7269 7074 735d  project.scripts]
+00000750: 0d0a 6661 726e 203d 2022 6661 726e 2e63  ..farn = "farn.c
+00000760: 6c69 2e66 6172 6e3a 6d61 696e 220d 0a62  li.farn:main"..b
+00000770: 6174 6368 5072 6f63 6573 7320 3d20 2266  atchProcess = "f
+00000780: 6172 6e2e 7275 6e2e 636c 692e 6261 7463  arn.run.cli.batc
+00000790: 6850 726f 6365 7373 3a6d 6169 6e22 0d0a  hProcess:main"..
+000007a0: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
+000007b0: 6c73 2e70 6163 6b61 6765 732e 6669 6e64  ls.packages.find
+000007c0: 5d0d 0a77 6865 7265 203d 205b 2273 7263  ]..where = ["src
+000007d0: 225d 0d0a 6578 636c 7564 6520 3d20 5b22  "]..exclude = ["
+000007e0: 7465 7374 2a22 5d0d 0a0d 0a5b 746f 6f6c  test*"]....[tool
+000007f0: 2e72 7566 665d 0d0a 6578 636c 7564 6520  .ruff]..exclude 
+00000800: 3d20 5b0d 0a20 2020 2022 2e67 6974 222c  = [..    ".git",
+00000810: 0d0a 2020 2020 222e 7665 6e76 222c 0d0a  ..    ".venv",..
+00000820: 2020 2020 222e 746f 7822 2c0d 0a20 2020      ".tox",..   
+00000830: 2022 6275 696c 6422 2c0d 0a20 2020 2022   "build",..    "
+00000840: 6469 7374 222c 0d0a 2020 2020 225f 5f70  dist",..    "__p
+00000850: 7963 6163 6865 5f5f 222c 0d0a 2020 2020  ycache__",..    
+00000860: 222e 2f64 6f63 732f 736f 7572 6365 2f63  "./docs/source/c
+00000870: 6f6e 662e 7079 222c 0d0a 5d0d 0a73 7263  onf.py",..]..src
+00000880: 203d 205b 2273 7263 225d 0d0a 6c69 6e65   = ["src"]..line
+00000890: 2d6c 656e 6774 6820 3d20 3132 300d 0a74  -length = 120..t
+000008a0: 6172 6765 742d 7665 7273 696f 6e20 3d20  arget-version = 
+000008b0: 2270 7933 3922 0d0a 0d0a 5b74 6f6f 6c2e  "py39"....[tool.
+000008c0: 7275 6666 2e6c 696e 745d 0d0a 6967 6e6f  ruff.lint]..igno
+000008d0: 7265 203d 205b 0d0a 2020 2020 2245 3530  re = [..    "E50
+000008e0: 3122 2c20 2023 204c 696e 6520 6c65 6e67  1",  # Line leng
+000008f0: 7468 2074 6f6f 206c 6f6e 670d 0a20 2020  th too long..   
+00000900: 2022 4431 3030 222c 2020 2320 4d69 7373   "D100",  # Miss
+00000910: 696e 6720 646f 6373 7472 696e 6720 696e  ing docstring in
+00000920: 2070 7562 6c69 6320 6d6f 6475 6c65 0d0a   public module..
+00000930: 2020 2020 2244 3130 3422 2c20 2023 204d      "D104",  # M
+00000940: 6973 7369 6e67 2064 6f63 7374 7269 6e67  issing docstring
+00000950: 2069 6e20 7075 626c 6963 2070 6163 6b61   in public packa
+00000960: 6765 0d0a 2020 2020 2244 3130 3522 2c20  ge..    "D105", 
+00000970: 2023 204d 6973 7369 6e67 2064 6f63 7374   # Missing docst
+00000980: 7269 6e67 2069 6e20 6d61 6769 6320 6d65  ring in magic me
+00000990: 7468 6f64 0d0a 2020 2020 2244 3130 3722  thod..    "D107"
+000009a0: 2c20 2023 204d 6973 7369 6e67 2064 6f63  ,  # Missing doc
+000009b0: 7374 7269 6e67 2069 6e20 5f5f 696e 6974  string in __init
+000009c0: 5f5f 0d0a 2020 2020 2244 3230 3222 2c20  __..    "D202", 
+000009d0: 2023 204e 6f20 626c 616e 6b20 6c69 6e65   # No blank line
+000009e0: 7320 616c 6c6f 7765 6420 6166 7465 7220  s allowed after 
+000009f0: 6675 6e63 7469 6f6e 2064 6f63 7374 7269  function docstri
+00000a00: 6e67 0d0a 2020 2020 2244 3230 3322 2c20  ng..    "D203", 
+00000a10: 2023 2031 2062 6c61 6e6b 206c 696e 6520   # 1 blank line 
+00000a20: 7265 7175 6972 6564 2062 6566 6f72 6520  required before 
+00000a30: 636c 6173 7320 646f 6373 7472 696e 670d  class docstring.
+00000a40: 0a20 2020 2022 4432 3035 222c 2020 2320  .    "D205",  # 
+00000a50: 3120 626c 616e 6b20 6c69 6e65 2072 6571  1 blank line req
+00000a60: 7569 7265 6420 6265 7477 6565 6e20 7375  uired between su
+00000a70: 6d6d 6172 7920 6c69 6e65 2061 6e64 2064  mmary line and d
+00000a80: 6573 6372 6970 7469 6f6e 0d0a 2020 2020  escription..    
+00000a90: 2244 3231 3222 2c20 2023 204d 756c 7469  "D212",  # Multi
+00000aa0: 2d6c 696e 6520 646f 6373 7472 696e 6720  -line docstring 
+00000ab0: 7375 6d6d 6172 7920 7368 6f75 6c64 2073  summary should s
+00000ac0: 7461 7274 2061 7420 7468 6520 6669 7273  tart at the firs
+00000ad0: 7420 6c69 6e65 0d0a 2020 2020 2244 3231  t line..    "D21
+00000ae0: 3322 2c20 2023 204d 756c 7469 2d6c 696e  3",  # Multi-lin
+00000af0: 6520 646f 6373 7472 696e 6720 7375 6d6d  e docstring summ
+00000b00: 6172 7920 7368 6f75 6c64 2073 7461 7274  ary should start
+00000b10: 2061 7420 7468 6520 7365 636f 6e64 206c   at the second l
+00000b20: 696e 650d 0a20 2020 2023 2022 4e38 3032  ine..    # "N802
+00000b30: 222c 2020 2320 4675 6e63 7469 6f6e 206e  ",  # Function n
+00000b40: 616d 6520 7368 6f75 6c64 2062 6520 6c6f  ame should be lo
+00000b50: 7765 7263 6173 6520 2028 756e 636f 6d6d  wercase  (uncomm
+00000b60: 656e 7420 6966 2079 6f75 2077 616e 7420  ent if you want 
+00000b70: 746f 2061 6c6c 6f77 2055 7070 6572 6361  to allow Upperca
+00000b80: 7365 2066 756e 6374 696f 6e20 6e61 6d65  se function name
+00000b90: 7329 0d0a 2020 2020 2320 224e 3830 3322  s)..    # "N803"
+00000ba0: 2c20 2023 2041 7267 756d 656e 7420 6e61  ,  # Argument na
+00000bb0: 6d65 2073 686f 756c 6420 6265 206c 6f77  me should be low
+00000bc0: 6572 6361 7365 2020 2875 6e63 6f6d 6d65  ercase  (uncomme
+00000bd0: 6e74 2069 6620 796f 7520 7761 6e74 2074  nt if you want t
+00000be0: 6f20 616c 6c6f 7720 5570 7065 7263 6173  o allow Uppercas
+00000bf0: 6520 6172 6775 6d65 6e74 206e 616d 6573  e argument names
+00000c00: 290d 0a20 2020 2022 4e38 3036 222c 2020  )..    "N806",  
+00000c10: 2320 5661 7269 6162 6c65 2069 6e20 6675  # Variable in fu
+00000c20: 6e63 7469 6f6e 2073 686f 756c 6420 6265  nction should be
+00000c30: 206c 6f77 6572 6361 7365 2020 2875 6e63   lowercase  (unc
+00000c40: 6f6d 6d65 6e74 2069 6620 796f 7520 7761  omment if you wa
+00000c50: 6e74 2074 6f20 616c 6c6f 7720 5570 7065  nt to allow Uppe
+00000c60: 7263 6173 6520 7661 7269 6162 6c65 206e  rcase variable n
+00000c70: 616d 6573 2069 6e20 6675 6e63 7469 6f6e  ames in function
+00000c80: 7329 0d0a 2020 2020 2320 224e 3831 3522  s)..    # "N815"
+00000c90: 2c20 2023 2056 6172 6961 626c 6520 696e  ,  # Variable in
+00000ca0: 2063 6c61 7373 2073 636f 7065 2073 686f   class scope sho
+00000cb0: 756c 6420 6e6f 7420 6265 206d 6978 6564  uld not be mixed
+00000cc0: 4361 7365 2020 2875 6e63 6f6d 6d65 6e74  Case  (uncomment
+00000cd0: 2069 6620 796f 7520 7761 6e74 2074 6f20   if you want to 
+00000ce0: 616c 6c6f 7720 6d69 7865 6443 6173 6520  allow mixedCase 
+00000cf0: 7661 7269 6162 6c65 206e 616d 6573 2069  variable names i
+00000d00: 6e20 636c 6173 7320 7363 6f70 6529 0d0a  n class scope)..
+00000d10: 2020 2020 2320 224e 3831 3622 2c20 2023      # "N816",  #
+00000d20: 2056 6172 6961 626c 6520 696e 2067 6c6f   Variable in glo
+00000d30: 6261 6c20 7363 6f70 6520 7368 6f75 6c64  bal scope should
+00000d40: 206e 6f74 2062 6520 6d69 7865 6443 6173   not be mixedCas
+00000d50: 6520 2028 756e 636f 6d6d 656e 7420 6966  e  (uncomment if
+00000d60: 2079 6f75 2077 616e 7420 746f 2061 6c6c   you want to all
+00000d70: 6f77 206d 6978 6564 4361 7365 2076 6172  ow mixedCase var
+00000d80: 6961 626c 6520 6e61 6d65 7320 696e 2067  iable names in g
+00000d90: 6c6f 6261 6c20 7363 6f70 6529 0d0a 2020  lobal scope)..  
+00000da0: 2020 224e 3939 3922 2c20 2023 2049 6e76    "N999",  # Inv
+00000db0: 616c 6964 206d 6f64 756c 6520 6e61 6d65  alid module name
+00000dc0: 0d0a 2020 2020 5d0d 0a73 656c 6563 7420  ..    ]..select 
+00000dd0: 3d20 5b0d 0a20 2020 2022 4522 2c0d 0a20  = [..    "E",.. 
+00000de0: 2020 2022 4422 2c0d 0a20 2020 2022 4622     "D",..    "F"
+00000df0: 2c0d 0a20 2020 2022 4e22 2c0d 0a20 2020  ,..    "N",..   
+00000e00: 2022 5722 2c0d 0a20 2020 2022 4922 2c0d   "W",..    "I",.
+00000e10: 0a20 2020 2022 4222 2c0d 0a5d 0d0a 0d0a  .    "B",..]....
+00000e20: 0d0a 5b74 6f6f 6c2e 7275 6666 2e6c 696e  ..[tool.ruff.lin
+00000e30: 742e 7065 7038 2d6e 616d 696e 675d 0d0a  t.pep8-naming]..
+00000e40: 6967 6e6f 7265 2d6e 616d 6573 203d 205b  ignore-names = [
+00000e50: 0d0a 2020 2020 2274 6573 745f 2a22 2c0d  ..    "test_*",.
+00000e60: 0a20 2020 2022 7365 7455 7022 2c0d 0a20  .    "setUp",.. 
+00000e70: 2020 2022 7465 6172 446f 776e 222c 0d0a     "tearDown",..
+00000e80: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+00000e90: 6c69 6e74 2e70 7964 6f63 7374 796c 655d  lint.pydocstyle]
+00000ea0: 0d0a 636f 6e76 656e 7469 6f6e 203d 2022  ..convention = "
+00000eb0: 6e75 6d70 7922 0d0a 0d0a 5b74 6f6f 6c2e  numpy"....[tool.
+00000ec0: 7275 6666 2e6c 696e 742e 7065 722d 6669  ruff.lint.per-fi
+00000ed0: 6c65 2d69 676e 6f72 6573 5d0d 0a22 5f5f  le-ignores].."__
+00000ee0: 696e 6974 5f5f 2e70 7922 203d 205b 2249  init__.py" = ["I
+00000ef0: 3030 3122 5d0d 0a22 2e2f 7465 7374 732f  001"].."./tests/
+00000f00: 2a22 203d 205b 2244 225d 0d0a 0d0a 5b74  *" = ["D"]....[t
+00000f10: 6f6f 6c2e 7275 6666 2e66 6f72 6d61 745d  ool.ruff.format]
+00000f20: 0d0a 646f 6373 7472 696e 672d 636f 6465  ..docstring-code
+00000f30: 2d66 6f72 6d61 7420 3d20 7472 7565 0d0a  -format = true..
+00000f40: 0d0a 5b74 6f6f 6c2e 7079 7269 6768 745d  ..[tool.pyright]
+00000f50: 0d0a 6578 636c 7564 6520 3d20 5b0d 0a20  ..exclude = [.. 
+00000f60: 2020 2022 2e67 6974 222c 0d0a 2020 2020     ".git",..    
+00000f70: 222e 7665 6e76 222c 0d0a 2020 2020 222e  ".venv",..    ".
+00000f80: 746f 7822 2c0d 0a20 2020 2022 6275 696c  tox",..    "buil
+00000f90: 6422 2c0d 0a20 2020 2022 6469 7374 222c  d",..    "dist",
+00000fa0: 0d0a 2020 2020 222a 2a2f 5f5f 7079 6361  ..    "**/__pyca
+00000fb0: 6368 655f 5f22 2c0d 0a20 2020 2022 2e2f  che__",..    "./
+00000fc0: 646f 6373 2f73 6f75 7263 652f 636f 6e66  docs/source/conf
+00000fd0: 2e70 7922 2c0d 0a20 2020 2022 2e2f 7665  .py",..    "./ve
+00000fe0: 6e76 222c 0d0a 5d0d 0a65 7874 7261 5061  nv",..]..extraPa
+00000ff0: 7468 7320 3d20 5b22 2e2f 7372 6322 5d0d  ths = ["./src"].
+00001000: 0a74 7970 6543 6865 636b 696e 674d 6f64  .typeCheckingMod
+00001010: 6520 3d20 2262 6173 6963 220d 0a75 7365  e = "basic"..use
+00001020: 4c69 6272 6172 7943 6f64 6546 6f72 5479  LibraryCodeForTy
+00001030: 7065 7320 3d20 7472 7565 0d0a 7265 706f  pes = true..repo
+00001040: 7274 4d69 7373 696e 6750 6172 616d 6574  rtMissingParamet
+00001050: 6572 5479 7065 203d 2022 6572 726f 7222  erType = "error"
+00001060: 0d0a 7265 706f 7274 556e 6b6e 6f77 6e50  ..reportUnknownP
+00001070: 6172 616d 6574 6572 5479 7065 203d 2022  arameterType = "
+00001080: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+00001090: 556e 6b6e 6f77 6e4d 656d 6265 7254 7970  UnknownMemberTyp
+000010a0: 6520 3d20 2277 6172 6e69 6e67 220d 0a72  e = "warning"..r
+000010b0: 6570 6f72 744d 6973 7369 6e67 5479 7065  eportMissingType
+000010c0: 4172 6775 6d65 6e74 203d 2022 6572 726f  Argument = "erro
+000010d0: 7222 0d0a 7265 706f 7274 5072 6f70 6572  r"..reportProper
+000010e0: 7479 5479 7065 4d69 736d 6174 6368 203d  tyTypeMismatch =
+000010f0: 2022 6572 726f 7222 0d0a 7265 706f 7274   "error"..report
+00001100: 4675 6e63 7469 6f6e 4d65 6d62 6572 4163  FunctionMemberAc
+00001110: 6365 7373 203d 2022 7761 726e 696e 6722  cess = "warning"
+00001120: 0d0a 7265 706f 7274 5072 6976 6174 6555  ..reportPrivateU
+00001130: 7361 6765 203d 2022 7761 726e 696e 6722  sage = "warning"
+00001140: 0d0a 7265 706f 7274 5479 7065 436f 6d6d  ..reportTypeComm
+00001150: 656e 7455 7361 6765 203d 2022 7761 726e  entUsage = "warn
+00001160: 696e 6722 0d0a 7265 706f 7274 496e 636f  ing"..reportInco
+00001170: 6d70 6174 6962 6c65 4d65 7468 6f64 4f76  mpatibleMethodOv
+00001180: 6572 7269 6465 203d 2022 7761 726e 696e  erride = "warnin
+00001190: 6722 0d0a 7265 706f 7274 496e 636f 6d70  g"..reportIncomp
+000011a0: 6174 6962 6c65 5661 7269 6162 6c65 4f76  atibleVariableOv
+000011b0: 6572 7269 6465 203d 2022 6572 726f 7222  erride = "error"
+000011c0: 0d0a 7265 706f 7274 496e 636f 6e73 6973  ..reportInconsis
+000011d0: 7465 6e74 436f 6e73 7472 7563 746f 7220  tentConstructor 
+000011e0: 3d20 2265 7272 6f72 220d 0a72 6570 6f72  = "error"..repor
+000011f0: 744f 7665 726c 6170 7069 6e67 4f76 6572  tOverlappingOver
+00001200: 6c6f 6164 203d 2022 7761 726e 696e 6722  load = "warning"
+00001210: 0d0a 7265 706f 7274 556e 696e 6974 6961  ..reportUninitia
+00001220: 6c69 7a65 6449 6e73 7461 6e63 6556 6172  lizedInstanceVar
+00001230: 6961 626c 6520 3d20 2277 6172 6e69 6e67  iable = "warning
+00001240: 220d 0a72 6570 6f72 7443 616c 6c49 6e44  "..reportCallInD
+00001250: 6566 6175 6c74 496e 6974 6961 6c69 7a65  efaultInitialize
+00001260: 7220 3d20 2277 6172 6e69 6e67 220d 0a72  r = "warning"..r
+00001270: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
+00001280: 4973 496e 7374 616e 6365 203d 2022 696e  IsInstance = "in
+00001290: 666f 726d 6174 696f 6e22 0d0a 7265 706f  formation"..repo
+000012a0: 7274 556e 6e65 6365 7373 6172 7943 6173  rtUnnecessaryCas
+000012b0: 7420 3d20 2277 6172 6e69 6e67 220d 0a72  t = "warning"..r
+000012c0: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
+000012d0: 436f 6d70 6172 6973 6f6e 203d 2022 7761  Comparison = "wa
+000012e0: 726e 696e 6722 0d0a 7265 706f 7274 556e  rning"..reportUn
+000012f0: 6e65 6365 7373 6172 7943 6f6e 7461 696e  necessaryContain
+00001300: 7320 3d20 2277 6172 6e69 6e67 220d 0a72  s = "warning"..r
+00001310: 6570 6f72 7455 6e75 7365 6443 616c 6c52  eportUnusedCallR
+00001320: 6573 756c 7420 3d20 2277 6172 6e69 6e67  esult = "warning
+00001330: 220d 0a72 6570 6f72 7455 6e75 7365 6445  "..reportUnusedE
+00001340: 7870 7265 7373 696f 6e20 3d20 2277 6172  xpression = "war
+00001350: 6e69 6e67 220d 0a72 6570 6f72 744d 6174  ning"..reportMat
+00001360: 6368 4e6f 7445 7868 6175 7374 6976 6520  chNotExhaustive 
+00001370: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00001380: 6f72 7453 6861 646f 7765 6449 6d70 6f72  ortShadowedImpor
+00001390: 7473 203d 2022 7761 726e 696e 6722 0d0a  ts = "warning"..
+000013a0: 7265 706f 7274 556e 7479 7065 6446 756e  reportUntypedFun
+000013b0: 6374 696f 6e44 6563 6f72 6174 6f72 203d  ctionDecorator =
+000013c0: 2022 7761 726e 696e 6722 0d0a 7265 706f   "warning"..repo
+000013d0: 7274 556e 7479 7065 6442 6173 6543 6c61  rtUntypedBaseCla
+000013e0: 7373 203d 2022 6572 726f 7222 0d0a 7265  ss = "error"..re
+000013f0: 706f 7274 556e 7479 7065 644e 616d 6564  portUntypedNamed
+00001400: 5475 706c 6520 3d20 2277 6172 6e69 6e67  Tuple = "warning
+00001410: 220d 0a23 2041 6374 6976 6174 6520 7468  "..# Activate th
+00001420: 6520 666f 6c6c 6f77 696e 6720 7275 6c65  e following rule
+00001430: 7320 6f6e 6c79 206c 6f63 616c 6c79 2061  s only locally a
+00001440: 6e64 2074 656d 706f 7261 7279 2c20 692e  nd temporary, i.
+00001450: 652e 2066 6f72 2061 2051 4120 7365 7373  e. for a QA sess
+00001460: 696f 6e2e 0d0a 2320 2846 6f72 2073 6572  ion...# (For ser
+00001470: 7665 7220 7369 6465 2043 4920 7468 6579  ver side CI they
+00001480: 2061 7265 2063 6f6e 7369 6465 7265 6420   are considered 
+00001490: 746f 6f20 7374 7269 6374 2e29 0d0a 2320  too strict.)..# 
+000014a0: 7265 706f 7274 436f 6e73 7461 6e74 5265  reportConstantRe
+000014b0: 6465 6669 6e69 7469 6f6e 203d 2022 7761  definition = "wa
+000014c0: 726e 696e 6722 0d0a 2320 7265 706f 7274  rning"..# report
+000014d0: 556e 6e65 6365 7373 6172 7954 7970 6549  UnnecessaryTypeI
+000014e0: 676e 6f72 6543 6f6d 6d65 6e74 203d 2022  gnoreComment = "
+000014f0: 696e 666f 726d 6174 696f 6e22 0d0a 2320  information"..# 
+00001500: 7265 706f 7274 496d 706f 7274 4379 636c  reportImportCycl
+00001510: 6573 203d 2022 7761 726e 696e 6722 0d0a  es = "warning"..
+00001520: 2320 7265 706f 7274 496d 706c 6963 6974  # reportImplicit
+00001530: 5374 7269 6e67 436f 6e63 6174 656e 6174  StringConcatenat
+00001540: 696f 6e20 3d20 2277 6172 6e69 6e67 220d  ion = "warning".
+00001550: 0a                                       .
```

### Comparing `farn-0.3.6/src/farn/cli/farn.py` & `farn-0.3.7/src/farn/cli/farn.py`

 * *Files 2% similar despite different names*

```diff
@@ -268,27 +268,27 @@
         elif rnd > (0.01 * rnd2) and rnd <= (0.86 * rnd2):
             p = t2(p)
         elif rnd > (0.86 * rnd2) and rnd <= (0.93 * rnd2):
             p = t3(p)
         else:
             p = t4(p)
         # ImageDraw.Draw(im,)
-        draw.point(
+        draw.point(  # pyright: ignore [reportUnknownMemberType]
             (p[0] * scale + x_offset, p[1] * scale),
             fill=(int(rgb[0] * rnd3[0]), int(rgb[1] * rnd3[1]), int(rgb[2] * rnd3[2])),
         )
 
         ii += 1
 
     del draw
 
     with tempfile.TemporaryDirectory() as temp_dir:
         # im.save(Path(os.getenv('HOME')) / 'splash.png')
         temp_file = Path(temp_dir) / "splash.png"
-        im.save(temp_file)
+        im.save(temp_file)  # pyright: ignore [reportUnknownMemberType]
 
         root = tk.Tk()
         root.overrideredirect(True)
         screen_width = root.winfo_screenwidth()
         screen_height = root.winfo_screenheight()
         root.geometry(
             "%dx%d+%d+%d"
```

### Comparing `farn-0.3.6/src/farn/core/case.py` & `farn-0.3.7/src/farn/core/case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 # pyright: reportUnknownMemberType=false
 import logging
 import re
 from copy import deepcopy
 from enum import IntEnum
 from pathlib import Path
-from typing import Any, Dict, List, MutableMapping, MutableSequence, Sequence, Set, Union
+from typing import (
+    Any,
+    Dict,
+    List,
+    MutableMapping,
+    MutableSequence,
+    Sequence,
+    Set,
+    Union,
+)
 
 import numpy as np
 from dictIO.utils.path import relative_path
 from numpy import ndarray
 from pandas import DataFrame, Series
 
 from farn.core import Parameter
@@ -204,14 +213,36 @@
                     f"\tAction '{action}' performed. Case {self.case} included."
                 )
                 return True
             return False
 
         return True
 
+    def add_parameters(
+        self,
+        parameters: Union[MutableSequence[Parameter], MutableMapping[str, str], None] = None,
+    ):
+        """Manually add extra parameters."""
+        if isinstance(parameters, MutableSequence):
+            self.parameters.extend(parameters)
+
+        elif isinstance(parameters, MutableMapping):
+            self.parameters.extend(
+                Parameter(parameter_name, parameter_value) for parameter_name, parameter_value in parameters.items()
+            )
+
+        else:
+            logger.error(
+                f"Layer {self.layer}, case {self.case} add_parameters failed:\n"
+                f"\tWrong input data format for additional parameters.\n"
+            )
+            exit(1)
+
+        return True
+
     def to_dict(self) -> Dict[str, Any]:
         """Return a dict with all case attributes.
 
         Returns
         -------
         Dict[str, Any]
             dict with all case attributes
@@ -242,14 +273,25 @@
 
     Inherits from List[Case] and can hence be transparently used as a Python list type.
     However, Cases extends its list base class by two convenience methods:
     to_pandas() and to_numpy(), which turn the list of Case objects
     into a pandas DataFrame or numpy ndarray, respectively.
     """
 
+    def add_parameters(
+        self,
+        parameters: Union[MutableSequence[Parameter], MutableMapping[str, str], None] = None,
+    ):
+        """Manually add extra parameters."""
+        _cases: List[Case] = deepcopy(self)
+        for case in _cases:
+            _ = case.add_parameters(parameters)
+
+        return False
+
     def to_pandas(
         self,
         use_path_as_index: bool = True,
         parameters_only: bool = False,
     ) -> DataFrame:
         """Return cases as a pandas Dataframe.
```

### Comparing `farn-0.3.6/src/farn/core/parameter.py` & `farn-0.3.7/src/farn/core/parameter.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn/farn.py` & `farn-0.3.7/src/farn/farn.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,767 +1,779 @@
-import logging
-import os
-import platform
-import re
-from copy import deepcopy
-from pathlib import Path
-from typing import Any, Dict, List, MutableMapping, MutableSequence, MutableSet, Sequence, Union
-
-from dictIO import CppDict, DictReader, DictWriter, create_target_file_name
-from dictIO.utils.strings import remove_quotes
-
-from farn.core import Case, Cases, Parameter
-from farn.run.batchProcess import AsyncBatchProcessor
-from farn.run.subProcess import execute_in_sub_process
-from farn.utils.logging import plural
-from farn.utils.os import append_system_variable
-
-__ALL__ = [
-    "run_farn",
-    "create_samples",
-    "create_cases",
-    "create_case_folders",
-    "create_param_dict_files",
-    "create_case_list_files",
-    "execute_command_set",
-]
-
-logger = logging.getLogger(__name__)
-
-
-def run_farn(
-    farn_dict_file: Union[str, os.PathLike[str]],
-    sample: bool = False,
-    generate: bool = False,
-    command: Union[str, None] = None,
-    batch: bool = False,
-    test: bool = False,
-) -> Cases:
-    """Run farn.
-
-    Runs the sampling for all layers as configured in farn dict,
-    generates the corresponding case folder structure and
-    executes user-defined shell command sets in all case folders.
-
-    Parameters
-    ----------
-    farn_dict_file : Union[str, os.PathLike[str]]
-        farnDict file. Contains the farn configuration.
-    sample : bool, optional
-        if True, runs the sampling defined for each layer and saves the sampled farnDict file with prefix sampled., by default False
-    generate : bool, optional
-        if True, generates the folder structure that spawns all layers and cases defined in farnDict, by default False
-    command : Union[str, None], optional
-        executes the given command set in all case folders. The command set must be defined in the commands section of the applicable layer in farnDict., by default None
-    batch : bool, optional
-        if True, executes the given command set in batch mode, i.e. asynchronously, by default False
-    test : bool, optional
-        if True, runs only first case and returns, by default False
-
-    Returns
-    -------
-    Cases
-        List containing all valid leaf cases.
-
-    Raises
-    ------
-    FileNotFoundError
-        if farn_dict_file does not exist
-    """
-
-    # Make sure farn_dict_file argument is of type Path. If not, cast it to Path type.
-    farn_dict_file = farn_dict_file if isinstance(farn_dict_file, Path) else Path(farn_dict_file)
-
-    # Check whether farn dict file exists
-    if not farn_dict_file.exists():
-        logger.error(f"run_farn: File {farn_dict_file} not found.")
-        raise FileNotFoundError(farn_dict_file)
-
-    # Set up farn environment
-    farn_dirs: Dict[str, Path] = _set_up_farn_environment(farn_dict_file)
-
-    # Read farn dict
-    farn_dict = DictReader.read(farn_dict_file, comments=False)
-
-    # Run sampling and create the samples for all layers in farn dict
-    if sample:
-        create_samples(farn_dict)  # run sampling
-        farn_dict.source_file = create_target_file_name(  # change filename to 'sampled.*'
-            farn_dict.source_file, prefix="sampled."  # type: ignore
-        )
-        logger.info(f"Save sampled farn dict {farn_dict.name}...")  # 1
-        DictWriter.write(farn_dict, mode="w")  # save sampled.* farn dict file
-        logger.info(f"Saved sampled farn dict in {farn_dict.source_file}.")  # 1
-
-    # Document CLI arguments of current farn call in the farn dict (for traceability)
-    farn_opts = {
-        "farnDict": farn_dict.name,
-        "sample": sample,
-        "generate": generate,
-        "execute": command,
-        "test": test,
-    }
-    farn_dict.update({"_farnOpts": farn_opts})
-
-    # Create all valid cases from the samples defined in farn dict.
-    cases = create_cases(
-        farn_dict=farn_dict,
-        case_dir=farn_dirs["CASEDIR"],
-        valid_only=True,
-    )
-
-    # Generate case folder structure
-    # and create a case-specific paramDict file in each case folder
-    if generate:
-        _ = create_case_folders(cases)
-        _ = create_param_dict_files(cases)
-        _ = create_case_list_files(
-            cases=cases,
-            target_dir=farn_dirs["ROOTDIR"],
-        )
-
-    # Execute a given command set in all case folders
-    if command:
-        _ = execute_command_set(
-            cases=cases,
-            command_set=command,
-            batch=batch,
-            test=test,
-        )
-
-    valid_leaf_cases: Cases = cases.filter(levels=-1, valid_only=True)
-
-    logger.info("Successfully finished farn.\n")
-
-    return valid_leaf_cases
-
-
-def create_samples(farn_dict: CppDict):
-    """Run sampling and create the samples inside all layers of the passed in farn dict.
-
-    Creates the _samples element in each layer and populates it with the discrete samples generated for the parameters defined and varied in the respective layer.
-    In case the _samples element already exists in a layer, it will be overwritten.
-
-    Parameters
-    ----------
-    farn_dict : CppDict
-        farn dict the samples shall be created in
-    """
-    from farn.sampling.sampling import DiscreteSampling
-
-    if "_layers" not in farn_dict:
-        logger.error(f"no '_layers' element in farn dict {farn_dict.name}. Sampling not possible.")
-        return
-
-    def create_samples_in_layer(
-        level: int,
-        layer_name: str,
-        layer: MutableMapping[str, Any],
-    ):
-        """Run sampling and generate the samples in the passed in layer."""
-        if "_sampling" not in layer:
-            logger.error("no '_sampling' element in layer")
-            return
-        if "_type" not in layer["_sampling"]:
-            logger.error("no '_type' element in sampling")
-            return
-
-        # instantiate and parameterize the sampling object
-        sampling = DiscreteSampling()
-        sampling.set_sampling_type(sampling_type=layer["_sampling"]["_type"])
-        sampling.set_sampling_parameters(
-            sampling_parameters=layer["_sampling"],
-            layer_name=layer_name,
-        )
-
-        # in case a _samples element already exists (e.g. from a former run) -> delete it
-        if "_samples" in layer:
-            del layer["_samples"]
-
-        # generate the samples and write them into the _samples element of the layer
-        samples: Dict[str, List[Any]] = sampling.generate_samples()
-        layer["_samples"] = samples
-
-        # if the layer does not have a _comment element yet: create a default comment
-        if "_comment" not in layer:
-            default_comment = f"level {level:2d}, layer {layer_name}"
-            layer["_comment"] = default_comment
-
-        return
-
-    logger.info(f"Run sampling of {farn_dict.name}...")
-
-    for index, (key, value) in enumerate(farn_dict["_layers"].items()):
-        create_samples_in_layer(
-            level=index,
-            layer_name=key,
-            layer=value,
-        )
-
-    logger.info(f"Successfully ran sampling of {farn_dict.name}.")
-
-    return
-
-
-def create_cases(
-    farn_dict: MutableMapping[Any, Any],
-    case_dir: Path,
-    valid_only: bool = False,
-) -> Cases:
-    """Create cases based on the layers, filter expressions and samples defined in the passed farn dict.
-
-    Creates case objects for all cases derived by recursive permutation of layers and the case specific samples defined per layer.
-    create_cases() creates one distinct case object for each case, holding all case attributes (parameters) set to their case specific values.
-
-    Optionally, only _valid_ cases can be returned, i.e. cases which fulfill the filter criteria configured for the respective layer.
-    Invalid cases then get excluded.
-
-    Note:
-    The corresponding case folder structure is not yet created by create_cases().
-    Creating the case folder structure is the responsibility of create_case_folder_structure().
-    However, the case_dir argument is passed in to allow create_cases() to already document in each case object
-    its _intended_ case folder path. This information is then read and used in create_case_folder_structure()
-    to actually create the case folders.
-
-    Parameters
-    ----------
-    farn_dict : MutableMapping
-        farn dict. The farn dict must be sampled, e.g. samples must have been generated for all layers defined in the farn dict.
-    case_dir : Path
-        directory the case folder structure is (intended) to be generated in.
-    valid_only: bool
-        whether or not only valid cases shall be returned, i.e. cases which fulfill the filter criteria configured for the respective layer., by default False
-
-    Returns
-    -------
-    Cases
-        list of case objects representing all created cases.
-    """
-    log_msg: str = "List all valid cases.." if valid_only else "List all cases.."
-    logger.info(log_msg)
-
-    # Check default distributions
-    default_distribution: Dict[str, Any] = {}
-
-    if "_always" in farn_dict:
-        default_distribution = farn_dict["_always"]
-
-    # Check arguments.
-    if "_layers" not in farn_dict:
-        logger.error("create_cases: No '_layers' element contained in farn dict.")
-        return Cases()
-
-    # Initialize cases list
-    cases: Cases = Cases()
-    number_of_invalid_cases: int = 0
-
-    # Create a local layers list that carries also the layers' name
-    # to ease sequential and indexed access to individual layers in create_next_level_cases()
-    layers: List[Dict[str, Any]] = []
-    for layer_name, layer in farn_dict["_layers"].items():
-        layer_copy: Dict[str, Any] = deepcopy(layer)
-        layer_copy["_name"] = layer_name
-        layers.append(layer_copy)
-
-    def create_next_level_cases(
-        level: int = 0,
-        base_case: Union[Case, None] = None,
-    ):
-        nonlocal cases
-        nonlocal number_of_invalid_cases
-        nonlocal layers
-
-        base_case = base_case or Case(path=Path.cwd())
-        base_case.parameters = base_case.parameters or []
-
-        current_layer: Dict[str, Any] = layers[level]
-        # validity checks for current layer
-        if "_samples" not in current_layer:
-            logger.warning(
-                f"No _samples element found in layer {current_layer['_name']}.\n"
-                f"Creation of cases for level {level:2d} aborted. "
-            )
-            return
-        if "_case_name" not in current_layer["_samples"]:
-            logger.warning(
-                f"The _samples element in layer {current_layer['_name']} is empty or does not have a _case_name element.\n"
-                f"Creation of cases for level {level:2d} aborted. "
-            )
-            return
-
-        current_layer_name: str = str(current_layer["_name"])
-        current_layer_is_leaf: bool = level == len(layers) - 1
-
-        no_of_samples_in_current_layer: int = len(current_layer["_samples"]["_case_name"])
-        samples_in_current_layer: MutableMapping[str, MutableSequence[float]] = {
-            param_name: param_values
-            for param_name, param_values in current_layer["_samples"].items()
-            if param_name != "_case_name"
-        }
-
-        parameter_names_used_in_preceeding_layers: MutableSet[str] = {
-            parameter.name for parameter in base_case.parameters if parameter.name
-        }
-
-        parameter_names_in_current_layer: MutableSequence[str] = []
-        for parameter_name in list(samples_in_current_layer.keys()):
-            if parameter_name in parameter_names_used_in_preceeding_layers:
-                logger.warning(
-                    f"The parameter {parameter_name} defined in layer {current_layer_name} had already been defined in a preceeding layer.\n"
-                    f"The preceeding definition prevails. The samples for parameter {parameter_name} defined in layer {current_layer_name} are skipped. "
-                )
-            else:
-                parameter_names_in_current_layer.append(parameter_name)
-
-        user_variables_in_current_layer: MutableSequence[Parameter] = []
-        for key, item in default_distribution.items():
-            if not key.startswith("_"):
-                default_variable = Parameter(name=key, value=item)
-                user_variables_in_current_layer.append(default_variable)
-
-        for key, item in current_layer.items():
-            if not key.startswith("_"):
-                user_variable = Parameter(name=key, value=item)
-                if user_variable.name in parameter_names_used_in_preceeding_layers:
-                    logger.warning(
-                        f"The user variable {user_variable.name} defined in layer {current_layer_name} matches a parameter that\n"
-                        f"had already been defined in a preceeding layer.\n"
-                        f"The preceeding definition prevails. The user variable {user_variable.name} defined in layer {current_layer_name} is skipped. "
-                    )
-                elif user_variable.name in parameter_names_in_current_layer:
-                    logger.warning(
-                        f"The user variable {user_variable.name} defined in layer {current_layer_name} matches a parameter name defined in the same layer.\n"
-                        f"The preceeding definition prevails. The user variable {user_variable.name} defined in layer {current_layer_name} is skipped. "
-                    )
-                else:
-                    user_variables_in_current_layer.append(user_variable)
-
-        condition_in_current_layer: Union[MutableMapping[str, str], None] = (
-            current_layer["_condition"] if "_condition" in current_layer else None
-        )
-        commands_in_current_layer: Union[MutableMapping[str, List[str]], None] = (
-            current_layer["_commands"] if "_commands" in current_layer else None
-        )
-
-        for index, case_name in enumerate(current_layer["_samples"]["_case_name"]):
-            case_name = remove_quotes(case_name)
-
-            case_parameters: MutableSequence[Parameter] = [
-                parameter for parameter in base_case.parameters if parameter.name
-            ]
-            case_parameters.extend(
-                Parameter(parameter_name, samples_in_current_layer[parameter_name][index])
-                for parameter_name in parameter_names_in_current_layer
-            )
-            case_parameters.extend(user_variables_in_current_layer)
-
-            case = Case(
-                case=case_name,
-                layer=current_layer_name,
-                level=level,
-                no_of_samples=no_of_samples_in_current_layer,
-                index=index,
-                path=base_case.path / case_name,
-                is_leaf=current_layer_is_leaf,
-                condition=condition_in_current_layer,
-                parameters=case_parameters,
-                command_sets=commands_in_current_layer,
-            )
-
-            if not valid_only or case.is_valid:
-                cases.append(case)
-                if not case.is_leaf:  # Recursion for next level cases
-                    create_next_level_cases(
-                        level=level + 1,
-                        base_case=case,
-                    )
-            else:
-                number_of_invalid_cases += 1
-
-        return
-
-    # Commence recursive collection of cases among all layers
-    base_case = Case(path=case_dir)
-    create_next_level_cases(level=0, base_case=base_case)
-
-    leaf_cases = [case for case in cases if case.is_leaf]
-
-    log_msg = ""
-    if valid_only:
-        log_msg = (
-            f"Successfully listed {len(leaf_cases)} valid case{plural(len(leaf_cases))}. "
-            f'{number_of_invalid_cases} invalid case{plural(number_of_invalid_cases)} {plural(number_of_invalid_cases, "were")} excluded.'
-        )
-    else:
-        log_msg = f"Successfully listed {len(leaf_cases)} case{plural(len(leaf_cases))}. "
-    logger.info(log_msg)
-
-    return cases
-
-
-def create_case_folders(cases: MutableSequence[Case]) -> int:
-    """Create the case folder structure for the passed in cases.
-
-    Parameters
-    ----------
-    cases : MutableSequence[Case]
-        cases the case folders shall be created for.
-
-    Returns
-    -------
-    int
-        number of case folders created.
-    """
-
-    logger.info("Create case folder structure...")
-    number_of_case_folders_created: int = 0
-
-    for case in cases:
-        logger.debug(f"creating case folder {case.path}")  # 1
-        case.path.mkdir(parents=True, exist_ok=True)
-        number_of_case_folders_created += 1
-
-    logger.info(f"Successfully created {number_of_case_folders_created} case folders.")
-
-    return number_of_case_folders_created
-
-
-def create_param_dict_files(cases: MutableSequence[Case]) -> int:
-    """Create the case specific paramDict files in the case folders of the passed in cases.
-
-    paramDict files contain the case specific parameters, meaning, via the paramDict files the case specific values
-    for all parameters get distributed to and persisted in the case folders.
-
-    Parameters
-    ----------
-    cases : MutableSequence[Case]
-        cases the paramDict file shall be created for
-
-    Returns
-    -------
-    int
-        number of paramDict files created
-    """
-
-    logger.info("Create case-specific paramDict files in all case folders...")
-    number_of_param_dicts_created: int = 0
-
-    for case in cases:
-        logger.debug(f"creating paramDict in {case.path}")  # 1
-        target_file = case.path / "paramDict"
-        param_dict = CppDict(target_file)
-
-        for parameter in case.parameters or []:
-            if parameter.name and not re.match("^_", parameter.name):
-                param_dict[parameter.name] = parameter.value
-
-        param_dict["_case"] = case.to_dict()
-
-        DictWriter.write(param_dict, target_file, mode="w")
-
-        if case.is_leaf:
-            number_of_param_dicts_created += 1
-
-    leaf_cases = [case for case in cases if case.is_leaf]
-
-    logger.info(
-        f"Successfully created {number_of_param_dicts_created} "
-        f"paramDict file{plural(number_of_param_dicts_created)} "
-        f"in {len(leaf_cases)} case folder{plural(len(leaf_cases))}."
-    )
-
-    return number_of_param_dicts_created
-
-
-def create_case_list_files(
-    cases: MutableSequence[Case],
-    target_dir: Union[Path, None] = None,
-    levels: Union[int, Sequence[int], None] = None,
-) -> list[Path]:
-    """Create case list files for the specified nest levels.
-
-    Case list files are simple text files containing a list of paths to all case folders that share a common nest level within the case folder structure.
-    I.e. a case list file created for level 0 contains the paths to all case folders on level 0.
-    A case list file for level 1 contains the paths to all case folders on level 1, and so on.
-
-    These lists can be used i.e. in a batchProcess to execute shell commands
-    in all case folders of a specific nest level inside the case folder structure.
-
-    Parameters
-    ----------
-    cases : MutableSequence[Case]
-        cases the case list files shall be created for
-    target_dir : Path, optional
-        directory in which the case list files shall be created. If None, current working directory will be used., by default None
-    levels : Union[int, Sequence[int], None], optional
-        list of integers indicating the nest levels for which case list files shall be created.
-        If missing, by default a case list file for the deepest nest level (the leaf level) will becreated., by default None
-
-    Returns
-    -------
-    list[Path]
-        The case list files that have been created (returned as a list of Path objects)
-    """
-
-    _remove_old_case_list_files()
-    target_dir = target_dir or Path.cwd()
-    case_list_file_all_levels = target_dir / "caseList"
-    logger.info(f"Create case list file '{case_list_file_all_levels}', containing all case folders.")
-
-    case_list_files_created: MutableSequence[Path] = []
-    max_level: int = 0
-    with case_list_file_all_levels.open(mode="w") as f:
-        for case in cases:
-            _ = f.write(f"{case.path.absolute()}\n")
-            max_level = max(max_level, case.level)
-    case_list_files_created.append(case_list_file_all_levels)
-
-    levels = levels or max_level
-    levels = [levels] if isinstance(levels, int) else levels
-
-    for level in levels:
-        case_list_file_for_level = target_dir / f"caseList_level_{level:02d}"
-        logger.info(
-            f"Create case list file '{case_list_file_for_level}', containing the case folders of level {level}."
-        )
-        with case_list_file_for_level.open(mode="w") as f:
-            for case in (case for case in cases if case.level == level):
-                _ = f.write(f"{case.path.absolute()}\n")
-        case_list_files_created.append(case_list_file_for_level)
-
-    case_list_files_created_log = "".join("\t" + path.name + "\n" for path in case_list_files_created)
-    case_list_files_created_log = case_list_files_created_log.removesuffix("\n")
-    logger.info(f"Successfully created following case list files:\n {case_list_files_created_log}")
-
-    return case_list_files_created
-
-
-def execute_command_set(
-    cases: MutableSequence[Case],
-    command_set: str,
-    batch: bool = True,
-    test: bool = False,
-) -> int:
-    """Execute the given command set in the case folders of the passed in cases.
-
-    Parameters
-    ----------
-    cases : MutableSequence[Case]
-        cases for which the specified command set shall be executed.
-    command_set : str
-        name of the command set to be executed, as defined in farnDict
-    batch : bool, optional
-        if True, executes the given command set in batch mode, i.e. asynchronously, by default False
-    test : bool, optional
-        if True, executes command set in only first case folder where command set is defined, by default False
-
-    Returns
-    -------
-    int
-        number of case folders in which the command set has been executed
-    """
-
-    logger.info(f"Execute command set '{command_set}' in all layers where '{command_set}' is defined...")
-
-    cases_registered: List[Case] = []
-    number_of_cases_registered: int = 0
-    reached_first_leaf: bool = False
-    if test:
-        logger.warning(
-            f"farn.py called with option --test: Only first case folder where command set '{command_set}' is defined will be executed."
-        )
-
-    for case in cases:
-        if not case.path.exists():
-            logger.warning(
-                f"Path {case.path} does not exist. "
-                f"This most commonly happens if a filter expression was changed in between generating the folder structure (option --generate) \n"
-                f"and executing a command set (option --execute). "
-                f"If so, first generate the missing cases by calling farn with option --generate once again \n"
-                f"and then retry to execute the command set with option --execute."
-            )
-            continue
-        if case.command_sets:
-            if command_set in case.command_sets:
-                cases_registered.append(case)
-                number_of_cases_registered += 1
-                if case.is_leaf:
-                    reached_first_leaf = True
-            else:
-                logger.debug(f"Command set '{command_set}' not defined in case {case.case}")
-        if test and reached_first_leaf:  # if test and at least one execution
-            break
-
-    number_of_cases_processed: int = 0
-
-    if batch:
-        cases_per_shell_command: Dict[str, List[Case]] = {}
-        for case in cases_registered:
-            if case.command_sets and command_set in case.command_sets:
-                shell_commands: List[str] = case.command_sets[command_set]
-                for shell_command in shell_commands:
-                    if shell_command in cases_per_shell_command:
-                        cases_per_shell_command[shell_command].append(case)
-                    else:
-                        cases_per_shell_command |= {shell_command: [case]}
-        for index, (shell_command, cases) in enumerate(cases_per_shell_command.items()):
-            case_list_file = Path.cwd() / f"caseList_for_command_{index}"
-            with case_list_file.open(mode="w") as f:
-                for case in cases:
-                    _ = f.write(f"{case.path.absolute()}\n")
-            batch_processor = AsyncBatchProcessor(case_list_file, shell_command)
-            batch_processor.run()
-    else:
-        for case in cases_registered:
-            if case.command_sets and command_set in case.command_sets:
-                shell_commands = case.command_sets[command_set]
-                # logger.debug(f"Execute command set '{command_set}' in {case.path}")                # commented out as a similar message gets logged in also subProcess
-                # Temporarily change cwd to case folder, to execute the shell commands from there
-                current_dir = Path.cwd()
-                os.chdir(case.path)
-                # Execute shell commands
-                _execute_shell_commands(shell_commands)
-                # Change back cwd to current folder
-                os.chdir(current_dir)
-                number_of_cases_processed += 1
-
-    # @TODO: This is only a temporary dummy.
-    #        To be replaced by a smarter algorithm.
-    #        CLAROS, 2022-08-16
-    number_of_cases_processed = number_of_cases_registered
-
-    if number_of_cases_processed > 0:
-        if test:
-            logger.info(
-                f"Test finished. Executed command set '{command_set}' in following case folder:\n"
-                f"\t {cases_registered[-1].path}"
-            )
-        else:
-            logger.info(
-                f"Successfully executed command set '{command_set}' "
-                f"in {number_of_cases_registered} case folder{plural(number_of_cases_registered)}."
-            )
-
-    return number_of_cases_registered
-
-
-def _set_up_farn_environment(farn_dict_file: Path) -> Dict[str, Path]:
-    """Read the '_environment' section from farn dict and sets up the farn environment accordingly.
-
-    Reads the '_environment' section from farnDict and sets up the farn environment directories as configured therein.
-    If the '_environment' section or certain entries therein are missing in farn dict, default values will be used.
-
-    Parameters
-    ----------
-    farn_dict_file : Path
-        farnDict file
-
-    Returns
-    -------
-    Dict[str, str]
-        dict containing the environment directories set up for farn (matching the _environment section in farnDict)
-    """
-
-    logger.info("Set up farn environment...")
-
-    # Set up farn environment.
-    # 1: Define default values for environment
-    # sourcery skip: merge-dict-assign
-    environment: Dict[str, str] = {}
-    environment["CASEDIR"] = "cases"
-    environment["DUMPDIR"] = "dump"
-    environment["LOGDIR"] = "logs"
-    environment["RESULTDIR"] = "results"
-    environment["TEMPLATEDIR"] = "template"
-    # 2: Overwrite default values with values defined in farn dict, if so
-    if environment_from_farn_dict := DictReader.read(farn_dict_file, scope=["_environment"]):
-        environment |= environment_from_farn_dict
-    else:
-        logger.warning(
-            f"Key '_environment' is missing in farn dict {farn_dict_file}. Using default values for farn environment."
-        )
-
-    # Read farn directories from environment
-    farn_dirs: Dict[str, Path]
-    farn_dirs = {k: Path.joinpath(Path.cwd(), v) for k, v in environment.items()}
-    farn_dirs["ROOTDIR"] = Path.cwd()
-    # Configure logging handler to write the farn log (use an additional handler, exclusively for farn)
-    _configure_additional_logging_handler_exclusively_for_farn(farn_dirs["LOGDIR"])
-
-    # Set up system environment variables for each farn directory
-    # This is necessary to enable shell commands defined in farnDict to point to them with i.e. %TEMPLATEDIR%
-    for key, item in farn_dirs.items():
-        append_system_variable(key, str(item))
-
-    logger.info("Successfully set up farn environment.")
-
-    return farn_dirs
-
-
-def _configure_additional_logging_handler_exclusively_for_farn(log_dir: Path):
-    """Create an additional logging handler exclusively for the farn log.
-
-    Parameters
-    ----------
-    log_dir : Path
-        folder in which the log file will be created
-    """
-    # Create log file
-    log_dir.mkdir(parents=True, exist_ok=True)
-    log_file = log_dir / "farn.log"
-    # Create logging file handler
-    file_handler = logging.FileHandler(str(log_file.absolute()), "a")
-    file_handler.name = str(log_file.absolute())
-    file_handler.setLevel(logging.INFO)
-    file_formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(message)s", "%Y-%m-%d %H:%M:%S")
-    file_handler.setFormatter(file_formatter)
-    # Register file handler at root logger
-    root_logger = logging.getLogger()
-    file_handler_already_exists: bool = any(handler.name == file_handler.name for handler in root_logger.handlers)
-    if not file_handler_already_exists:
-        root_logger.addHandler(file_handler)
-    return
-
-
-def _remove_old_case_list_files():  # sourcery skip: avoid-builtin-shadow
-    """Remove old case list files, if existing."""
-    logger.info("Remove old case list files...")
-
-    lists = [list for list in Path.cwd().rglob("*") if re.search("(path|queue)List", str(list))]
-
-    for list in lists:
-        list = Path(list)
-        list.unlink()
-
-    logger.info("Successfully removed old case list files.")
-
-    return
-
-
-def _sys_call(shell_commands: MutableSequence[str]):
-    """Fallback function until _execute_command is usable under linux."""
-
-    for shell_command in shell_commands:
-        _ = os.system(shell_command)
-
-    return
-
-
-def _execute_shell_commands(shell_commands: MutableSequence[str]):
-    """Execute a sequence of shell commands using subprocess.
-
-    Parameters
-    ----------
-    shell_commands : MutableSequence
-        list with shell commands to be executed
-    """
-
-    # @TODO: until the problem with vanishing '.'s on Linux systems is solved (e.g. in command "ln -s target ."),
-    #        reroute the function call to _sys_call instead, as a workaround.
-    if platform.system() == "Linux":
-        _sys_call(shell_commands)
-        return
-
-    for shell_command in shell_commands:
-        _ = execute_in_sub_process(shell_command)
-
-    return
+import logging
+import os
+import platform
+import re
+from copy import deepcopy
+from pathlib import Path
+from typing import (
+    Any,
+    Dict,
+    List,
+    MutableMapping,
+    MutableSequence,
+    MutableSet,
+    Sequence,
+    Union,
+)
+
+from dictIO import CppDict, DictReader, DictWriter, create_target_file_name
+from dictIO.utils.strings import remove_quotes
+
+from farn.core import Case, Cases, Parameter
+from farn.run.batchProcess import AsyncBatchProcessor
+from farn.run.subProcess import execute_in_sub_process
+from farn.utils.logging import plural
+from farn.utils.os import append_system_variable
+
+__ALL__ = [
+    "run_farn",
+    "create_samples",
+    "create_cases",
+    "create_case_folders",
+    "create_param_dict_files",
+    "create_case_list_files",
+    "execute_command_set",
+]
+
+logger = logging.getLogger(__name__)
+
+
+def run_farn(
+    farn_dict_file: Union[str, os.PathLike[str]],
+    sample: bool = False,
+    generate: bool = False,
+    command: Union[str, None] = None,
+    batch: bool = False,
+    test: bool = False,
+) -> Cases:
+    """Run farn.
+
+    Runs the sampling for all layers as configured in farn dict,
+    generates the corresponding case folder structure and
+    executes user-defined shell command sets in all case folders.
+
+    Parameters
+    ----------
+    farn_dict_file : Union[str, os.PathLike[str]]
+        farnDict file. Contains the farn configuration.
+    sample : bool, optional
+        if True, runs the sampling defined for each layer and saves the sampled farnDict file with prefix sampled., by default False
+    generate : bool, optional
+        if True, generates the folder structure that spawns all layers and cases defined in farnDict, by default False
+    command : Union[str, None], optional
+        executes the given command set in all case folders. The command set must be defined in the commands section of the applicable layer in farnDict., by default None
+    batch : bool, optional
+        if True, executes the given command set in batch mode, i.e. asynchronously, by default False
+    test : bool, optional
+        if True, runs only first case and returns, by default False
+
+    Returns
+    -------
+    Cases
+        List containing all valid leaf cases.
+
+    Raises
+    ------
+    FileNotFoundError
+        if farn_dict_file does not exist
+    """
+    # sourcery skip: extract-method
+
+    # Make sure farn_dict_file argument is of type Path. If not, cast it to Path type.
+    farn_dict_file = farn_dict_file if isinstance(farn_dict_file, Path) else Path(farn_dict_file)
+
+    # Check whether farn dict file exists
+    if not farn_dict_file.exists():
+        logger.error(f"run_farn: File {farn_dict_file} not found.")
+        raise FileNotFoundError(farn_dict_file)
+
+    # Set up farn environment
+    farn_dirs: Dict[str, Path] = _set_up_farn_environment(farn_dict_file)
+
+    # Read farn dict
+    farn_dict = DictReader.read(farn_dict_file, comments=False)
+
+    # Run sampling and create the samples for all layers in farn dict
+    if sample:
+        create_samples(farn_dict)  # run sampling
+        assert farn_dict.source_file is not None
+        farn_dict.source_file = create_target_file_name(  # change filename to 'sampled.*'
+            farn_dict.source_file,
+            prefix="sampled.",  # type: ignore
+        )
+        logger.info(f"Save sampled farn dict {farn_dict.name}...")  # 1
+        DictWriter.write(farn_dict, mode="w")  # save sampled.* farn dict file
+        logger.info(f"Saved sampled farn dict in {farn_dict.source_file}.")  # 1
+
+    # Document CLI arguments of current farn call in the farn dict (for traceability)
+    farn_opts = {
+        "farnDict": farn_dict.name,
+        "sample": sample,
+        "generate": generate,
+        "execute": command,
+        "test": test,
+    }
+    farn_dict.update({"_farnOpts": farn_opts})
+
+    # Create all valid cases from the samples defined in farn dict.
+    cases = create_cases(
+        farn_dict=farn_dict,
+        case_dir=farn_dirs["CASEDIR"],
+        valid_only=True,
+    )
+
+    # Generate case folder structure
+    # and create a case-specific paramDict file in each case folder
+    if generate:
+        _ = create_case_folders(cases)
+        _ = create_param_dict_files(cases)
+        _ = create_case_list_files(
+            cases=cases,
+            target_dir=farn_dirs["ROOTDIR"],
+        )
+
+    # Execute a given command set in all case folders
+    if command:
+        _ = execute_command_set(
+            cases=cases,
+            command_set=command,
+            batch=batch,
+            test=test,
+        )
+
+    valid_leaf_cases: Cases = cases.filter(levels=-1, valid_only=True)
+
+    logger.info("Successfully finished farn.\n")
+
+    return valid_leaf_cases
+
+
+def create_samples(farn_dict: CppDict):
+    """Run sampling and create the samples inside all layers of the passed in farn dict.
+
+    Creates the _samples element in each layer and populates it with the discrete samples generated for the parameters defined and varied in the respective layer.
+    In case the _samples element already exists in a layer, it will be overwritten.
+
+    Parameters
+    ----------
+    farn_dict : CppDict
+        farn dict the samples shall be created in
+    """
+    from farn.sampling.sampling import DiscreteSampling
+
+    if "_layers" not in farn_dict:
+        logger.error(f"no '_layers' element in farn dict {farn_dict.name}. Sampling not possible.")
+        return
+
+    def create_samples_in_layer(
+        level: int,
+        layer_name: str,
+        layer: MutableMapping[str, Any],
+    ):
+        """Run sampling and generate the samples in the passed in layer."""
+        if "_sampling" not in layer:
+            logger.error("no '_sampling' element in layer")
+            return
+        if "_type" not in layer["_sampling"]:
+            logger.error("no '_type' element in sampling")
+            return
+
+        # instantiate and parameterize the sampling object
+        sampling = DiscreteSampling()
+        sampling.set_sampling_type(sampling_type=layer["_sampling"]["_type"])
+        sampling.set_sampling_parameters(
+            sampling_parameters=layer["_sampling"],
+            layer_name=layer_name,
+        )
+
+        # in case a _samples element already exists (e.g. from a former run) -> delete it
+        if "_samples" in layer:
+            del layer["_samples"]
+
+        # generate the samples and write them into the _samples element of the layer
+        samples: Dict[str, List[Any]] = sampling.generate_samples()
+        layer["_samples"] = samples
+
+        # if the layer does not have a _comment element yet: create a default comment
+        if "_comment" not in layer:
+            default_comment = f"level {level:2d}, layer {layer_name}"
+            layer["_comment"] = default_comment
+
+        return
+
+    logger.info(f"Run sampling of {farn_dict.name}...")
+
+    for index, (key, value) in enumerate(farn_dict["_layers"].items()):
+        create_samples_in_layer(
+            level=index,
+            layer_name=key,
+            layer=value,
+        )
+
+    logger.info(f"Successfully ran sampling of {farn_dict.name}.")
+
+    return
+
+
+def create_cases(
+    farn_dict: MutableMapping[Any, Any],
+    case_dir: Path,
+    valid_only: bool = False,
+) -> Cases:
+    """Create cases based on the layers, filter expressions and samples defined in the passed farn dict.
+
+    Creates case objects for all cases derived by recursive permutation of layers and the case specific samples defined per layer.
+    create_cases() creates one distinct case object for each case, holding all case attributes (parameters) set to their case specific values.
+
+    Optionally, only _valid_ cases can be returned, i.e. cases which fulfill the filter criteria configured for the respective layer.
+    Invalid cases then get excluded.
+
+    Note:
+    The corresponding case folder structure is not yet created by create_cases().
+    Creating the case folder structure is the responsibility of create_case_folder_structure().
+    However, the case_dir argument is passed in to allow create_cases() to already document in each case object
+    its _intended_ case folder path. This information is then read and used in create_case_folder_structure()
+    to actually create the case folders.
+
+    Parameters
+    ----------
+    farn_dict : MutableMapping
+        farn dict. The farn dict must be sampled, e.g. samples must have been generated for all layers defined in the farn dict.
+    case_dir : Path
+        directory the case folder structure is (intended) to be generated in.
+    valid_only: bool
+        whether or not only valid cases shall be returned, i.e. cases which fulfill the filter criteria configured for the respective layer., by default False
+
+    Returns
+    -------
+    Cases
+        list of case objects representing all created cases.
+    """
+    log_msg: str = "List all valid cases.." if valid_only else "List all cases.."
+    logger.info(log_msg)
+
+    # Check default distributions
+    default_distribution: Dict[str, Any] = {}
+
+    if "_always" in farn_dict:
+        default_distribution = farn_dict["_always"]
+
+    # Check arguments.
+    if "_layers" not in farn_dict:
+        logger.error("create_cases: No '_layers' element contained in farn dict.")
+        return Cases()
+
+    # Initialize cases list
+    cases: Cases = Cases()
+    number_of_invalid_cases: int = 0
+
+    # Create a local layers list that carries also the layers' name
+    # to ease sequential and indexed access to individual layers in create_next_level_cases()
+    layers: List[Dict[str, Any]] = []
+    for layer_name, layer in farn_dict["_layers"].items():
+        layer_copy: Dict[str, Any] = deepcopy(layer)
+        layer_copy["_name"] = layer_name
+        layers.append(layer_copy)
+
+    def create_next_level_cases(
+        level: int = 0,
+        base_case: Union[Case, None] = None,
+    ):
+        nonlocal cases
+        nonlocal number_of_invalid_cases
+        nonlocal layers
+
+        base_case = base_case or Case(path=Path.cwd())
+        base_case.parameters = base_case.parameters or []
+
+        current_layer: Dict[str, Any] = layers[level]
+        # validity checks for current layer
+        if "_samples" not in current_layer:
+            logger.warning(
+                f"No _samples element found in layer {current_layer['_name']}.\n"
+                f"Creation of cases for level {level:2d} aborted. "
+            )
+            return
+        if "_case_name" not in current_layer["_samples"]:
+            logger.warning(
+                f"The _samples element in layer {current_layer['_name']} is empty or does not have a _case_name element.\n"
+                f"Creation of cases for level {level:2d} aborted. "
+            )
+            return
+
+        current_layer_name: str = str(current_layer["_name"])
+        current_layer_is_leaf: bool = level == len(layers) - 1
+
+        no_of_samples_in_current_layer: int = len(current_layer["_samples"]["_case_name"])
+        samples_in_current_layer: MutableMapping[str, MutableSequence[float]] = {
+            param_name: param_values
+            for param_name, param_values in current_layer["_samples"].items()
+            if param_name != "_case_name"
+        }
+
+        parameter_names_used_in_preceeding_layers: MutableSet[str] = {
+            parameter.name for parameter in base_case.parameters if parameter.name
+        }
+
+        parameter_names_in_current_layer: MutableSequence[str] = []
+        for parameter_name in list(samples_in_current_layer.keys()):
+            if parameter_name in parameter_names_used_in_preceeding_layers:
+                logger.warning(
+                    f"The parameter {parameter_name} defined in layer {current_layer_name} had already been defined in a preceeding layer.\n"
+                    f"The preceeding definition prevails. The samples for parameter {parameter_name} defined in layer {current_layer_name} are skipped. "
+                )
+            else:
+                parameter_names_in_current_layer.append(parameter_name)
+
+        user_variables_in_current_layer: MutableSequence[Parameter] = []
+        for key, item in default_distribution.items():
+            if not key.startswith("_"):
+                default_variable = Parameter(name=key, value=item)
+                user_variables_in_current_layer.append(default_variable)
+
+        for key, item in current_layer.items():
+            if not key.startswith("_"):
+                user_variable = Parameter(name=key, value=item)
+                if user_variable.name in parameter_names_used_in_preceeding_layers:
+                    logger.warning(
+                        f"The user variable {user_variable.name} defined in layer {current_layer_name} matches a parameter that\n"
+                        f"had already been defined in a preceeding layer.\n"
+                        f"The preceeding definition prevails. The user variable {user_variable.name} defined in layer {current_layer_name} is skipped. "
+                    )
+                elif user_variable.name in parameter_names_in_current_layer:
+                    logger.warning(
+                        f"The user variable {user_variable.name} defined in layer {current_layer_name} matches a parameter name defined in the same layer.\n"
+                        f"The preceeding definition prevails. The user variable {user_variable.name} defined in layer {current_layer_name} is skipped. "
+                    )
+                else:
+                    user_variables_in_current_layer.append(user_variable)
+
+        condition_in_current_layer: Union[MutableMapping[str, str], None] = (
+            current_layer["_condition"] if "_condition" in current_layer else None
+        )
+        commands_in_current_layer: Union[MutableMapping[str, List[str]], None] = (
+            current_layer["_commands"] if "_commands" in current_layer else None
+        )
+
+        for index, case_name in enumerate(current_layer["_samples"]["_case_name"]):
+            case_name = remove_quotes(case_name)
+
+            case_parameters: MutableSequence[Parameter] = [
+                parameter for parameter in base_case.parameters if parameter.name
+            ]
+            case_parameters.extend(
+                Parameter(parameter_name, samples_in_current_layer[parameter_name][index])
+                for parameter_name in parameter_names_in_current_layer
+            )
+            case_parameters.extend(user_variables_in_current_layer)
+
+            case = Case(
+                case=case_name,
+                layer=current_layer_name,
+                level=level,
+                no_of_samples=no_of_samples_in_current_layer,
+                index=index,
+                path=base_case.path / case_name,
+                is_leaf=current_layer_is_leaf,
+                condition=condition_in_current_layer,
+                parameters=case_parameters,
+                command_sets=commands_in_current_layer,
+            )
+
+            if not valid_only or case.is_valid:
+                cases.append(case)
+                if not case.is_leaf:  # Recursion for next level cases
+                    create_next_level_cases(
+                        level=level + 1,
+                        base_case=case,
+                    )
+            else:
+                number_of_invalid_cases += 1
+
+        return
+
+    # Commence recursive collection of cases among all layers
+    base_case = Case(path=case_dir)
+    create_next_level_cases(level=0, base_case=base_case)
+
+    leaf_cases = [case for case in cases if case.is_leaf]
+
+    log_msg = ""
+    if valid_only:
+        log_msg = (
+            f"Successfully listed {len(leaf_cases)} valid case{plural(len(leaf_cases))}. "
+            f'{number_of_invalid_cases} invalid case{plural(number_of_invalid_cases)} {plural(number_of_invalid_cases, "were")} excluded.'
+        )
+    else:
+        log_msg = f"Successfully listed {len(leaf_cases)} case{plural(len(leaf_cases))}. "
+    logger.info(log_msg)
+
+    return cases
+
+
+def create_case_folders(cases: MutableSequence[Case]) -> int:
+    """Create the case folder structure for the passed in cases.
+
+    Parameters
+    ----------
+    cases : MutableSequence[Case]
+        cases the case folders shall be created for.
+
+    Returns
+    -------
+    int
+        number of case folders created.
+    """
+
+    logger.info("Create case folder structure...")
+    number_of_case_folders_created: int = 0
+
+    for case in cases:
+        logger.debug(f"creating case folder {case.path}")  # 1
+        case.path.mkdir(parents=True, exist_ok=True)
+        number_of_case_folders_created += 1
+
+    logger.info(f"Successfully created {number_of_case_folders_created} case folders.")
+
+    return number_of_case_folders_created
+
+
+def create_param_dict_files(cases: MutableSequence[Case]) -> int:
+    """Create the case specific paramDict files in the case folders of the passed in cases.
+
+    paramDict files contain the case specific parameters, meaning, via the paramDict files the case specific values
+    for all parameters get distributed to and persisted in the case folders.
+
+    Parameters
+    ----------
+    cases : MutableSequence[Case]
+        cases the paramDict file shall be created for
+
+    Returns
+    -------
+    int
+        number of paramDict files created
+    """
+
+    logger.info("Create case-specific paramDict files in all case folders...")
+    number_of_param_dicts_created: int = 0
+
+    for case in cases:
+        logger.debug(f"creating paramDict in {case.path}")  # 1
+        target_file = case.path / "paramDict"
+        param_dict = CppDict(target_file)
+
+        for parameter in case.parameters or []:
+            if parameter.name and not re.match("^_", parameter.name):
+                param_dict[parameter.name] = parameter.value
+
+        param_dict["_case"] = case.to_dict()
+
+        DictWriter.write(param_dict, target_file, mode="w")
+
+        if case.is_leaf:
+            number_of_param_dicts_created += 1
+
+    leaf_cases = [case for case in cases if case.is_leaf]
+
+    logger.info(
+        f"Successfully created {number_of_param_dicts_created} "
+        f"paramDict file{plural(number_of_param_dicts_created)} "
+        f"in {len(leaf_cases)} case folder{plural(len(leaf_cases))}."
+    )
+
+    return number_of_param_dicts_created
+
+
+def create_case_list_files(
+    cases: MutableSequence[Case],
+    target_dir: Union[Path, None] = None,
+    levels: Union[int, Sequence[int], None] = None,
+) -> list[Path]:
+    """Create case list files for the specified nest levels.
+
+    Case list files are simple text files containing a list of paths to all case folders that share a common nest level within the case folder structure.
+    I.e. a case list file created for level 0 contains the paths to all case folders on level 0.
+    A case list file for level 1 contains the paths to all case folders on level 1, and so on.
+
+    These lists can be used i.e. in a batchProcess to execute shell commands
+    in all case folders of a specific nest level inside the case folder structure.
+
+    Parameters
+    ----------
+    cases : MutableSequence[Case]
+        cases the case list files shall be created for
+    target_dir : Path, optional
+        directory in which the case list files shall be created. If None, current working directory will be used., by default None
+    levels : Union[int, Sequence[int], None], optional
+        list of integers indicating the nest levels for which case list files shall be created.
+        If missing, by default a case list file for the deepest nest level (the leaf level) will becreated., by default None
+
+    Returns
+    -------
+    list[Path]
+        The case list files that have been created (returned as a list of Path objects)
+    """
+
+    _remove_old_case_list_files()
+    target_dir = target_dir or Path.cwd()
+    case_list_file_all_levels = target_dir / "caseList"
+    logger.info(f"Create case list file '{case_list_file_all_levels}', containing all case folders.")
+
+    case_list_files_created: MutableSequence[Path] = []
+    max_level: int = 0
+    with case_list_file_all_levels.open(mode="w") as f:
+        for case in cases:
+            _ = f.write(f"{case.path.absolute()}\n")
+            max_level = max(max_level, case.level)
+    case_list_files_created.append(case_list_file_all_levels)
+
+    levels = levels or max_level
+    levels = [levels] if isinstance(levels, int) else levels
+
+    for level in levels:
+        case_list_file_for_level = target_dir / f"caseList_level_{level:02d}"
+        logger.info(
+            f"Create case list file '{case_list_file_for_level}', containing the case folders of level {level}."
+        )
+        with case_list_file_for_level.open(mode="w") as f:
+            for case in (case for case in cases if case.level == level):
+                _ = f.write(f"{case.path.absolute()}\n")
+        case_list_files_created.append(case_list_file_for_level)
+
+    case_list_files_created_log = "".join("\t" + path.name + "\n" for path in case_list_files_created)
+    case_list_files_created_log = case_list_files_created_log.removesuffix("\n")
+    logger.info(f"Successfully created following case list files:\n {case_list_files_created_log}")
+
+    return case_list_files_created
+
+
+def execute_command_set(
+    cases: MutableSequence[Case],
+    command_set: str,
+    batch: bool = True,
+    test: bool = False,
+) -> int:
+    """Execute the given command set in the case folders of the passed in cases.
+
+    Parameters
+    ----------
+    cases : MutableSequence[Case]
+        cases for which the specified command set shall be executed.
+    command_set : str
+        name of the command set to be executed, as defined in farnDict
+    batch : bool, optional
+        if True, executes the given command set in batch mode, i.e. asynchronously, by default False
+    test : bool, optional
+        if True, executes command set in only first case folder where command set is defined, by default False
+
+    Returns
+    -------
+    int
+        number of case folders in which the command set has been executed
+    """
+
+    logger.info(f"Execute command set '{command_set}' in all layers where '{command_set}' is defined...")
+
+    cases_registered: List[Case] = []
+    number_of_cases_registered: int = 0
+    reached_first_leaf: bool = False
+    if test:
+        logger.warning(
+            f"farn.py called with option --test: Only first case folder where command set '{command_set}' is defined will be executed."
+        )
+
+    for case in cases:
+        if not case.path.exists():
+            logger.warning(
+                f"Path {case.path} does not exist. "
+                f"This most commonly happens if a filter expression was changed in between generating the folder structure (option --generate) \n"
+                f"and executing a command set (option --execute). "
+                f"If so, first generate the missing cases by calling farn with option --generate once again \n"
+                f"and then retry to execute the command set with option --execute."
+            )
+            continue
+        if case.command_sets:
+            if command_set in case.command_sets:
+                cases_registered.append(case)
+                number_of_cases_registered += 1
+                if case.is_leaf:
+                    reached_first_leaf = True
+            else:
+                logger.debug(f"Command set '{command_set}' not defined in case {case.case}")
+        if test and reached_first_leaf:  # if test and at least one execution
+            break
+
+    number_of_cases_processed: int = 0
+
+    if batch:
+        cases_per_shell_command: Dict[str, List[Case]] = {}
+        for case in cases_registered:
+            if case.command_sets and command_set in case.command_sets:
+                shell_commands: List[str] = case.command_sets[command_set]
+                for shell_command in shell_commands:
+                    if shell_command in cases_per_shell_command:
+                        cases_per_shell_command[shell_command].append(case)
+                    else:
+                        cases_per_shell_command |= {shell_command: [case]}
+        for index, (shell_command, cases) in enumerate(cases_per_shell_command.items()):
+            case_list_file = Path.cwd() / f"caseList_for_command_{index}"
+            with case_list_file.open(mode="w") as f:
+                for case in cases:
+                    _ = f.write(f"{case.path.absolute()}\n")
+            batch_processor = AsyncBatchProcessor(case_list_file, shell_command)
+            batch_processor.run()
+    else:
+        for case in cases_registered:
+            if case.command_sets and command_set in case.command_sets:
+                shell_commands = case.command_sets[command_set]
+                # logger.debug(f"Execute command set '{command_set}' in {case.path}")                # commented out as a similar message gets logged in also subProcess
+                # Temporarily change cwd to case folder, to execute the shell commands from there
+                current_dir = Path.cwd()
+                os.chdir(case.path)
+                # Execute shell commands
+                _execute_shell_commands(shell_commands)
+                # Change back cwd to current folder
+                os.chdir(current_dir)
+                number_of_cases_processed += 1
+
+    # @TODO: This is only a temporary dummy.
+    #        To be replaced by a smarter algorithm.
+    #        CLAROS, 2022-08-16
+    number_of_cases_processed = number_of_cases_registered
+
+    if number_of_cases_processed > 0:
+        if test:
+            logger.info(
+                f"Test finished. Executed command set '{command_set}' in following case folder:\n"
+                f"\t {cases_registered[-1].path}"
+            )
+        else:
+            logger.info(
+                f"Successfully executed command set '{command_set}' "
+                f"in {number_of_cases_registered} case folder{plural(number_of_cases_registered)}."
+            )
+
+    return number_of_cases_registered
+
+
+def _set_up_farn_environment(farn_dict_file: Path) -> Dict[str, Path]:
+    """Read the '_environment' section from farn dict and sets up the farn environment accordingly.
+
+    Reads the '_environment' section from farnDict and sets up the farn environment directories as configured therein.
+    If the '_environment' section or certain entries therein are missing in farn dict, default values will be used.
+
+    Parameters
+    ----------
+    farn_dict_file : Path
+        farnDict file
+
+    Returns
+    -------
+    Dict[str, str]
+        dict containing the environment directories set up for farn (matching the _environment section in farnDict)
+    """
+
+    logger.info("Set up farn environment...")
+
+    # Set up farn environment.
+    # 1: Define default values for environment
+    # sourcery skip: merge-dict-assign
+    environment: Dict[str, str] = {}
+    environment["CASEDIR"] = "cases"
+    environment["DUMPDIR"] = "dump"
+    environment["LOGDIR"] = "logs"
+    environment["RESULTDIR"] = "results"
+    environment["TEMPLATEDIR"] = "template"
+    # 2: Overwrite default values with values defined in farn dict, if so
+    if environment_from_farn_dict := DictReader.read(farn_dict_file, scope=["_environment"]):
+        environment |= environment_from_farn_dict
+    else:
+        logger.warning(
+            f"Key '_environment' is missing in farn dict {farn_dict_file}. Using default values for farn environment."
+        )
+
+    # Read farn directories from environment
+    farn_dirs: Dict[str, Path]
+    farn_dirs = {k: Path.joinpath(Path.cwd(), v) for k, v in environment.items()}
+    farn_dirs["ROOTDIR"] = Path.cwd()
+    # Configure logging handler to write the farn log (use an additional handler, exclusively for farn)
+    _configure_additional_logging_handler_exclusively_for_farn(farn_dirs["LOGDIR"])
+
+    # Set up system environment variables for each farn directory
+    # This is necessary to enable shell commands defined in farnDict to point to them with i.e. %TEMPLATEDIR%
+    for key, item in farn_dirs.items():
+        append_system_variable(key, str(item))
+
+    logger.info("Successfully set up farn environment.")
+
+    return farn_dirs
+
+
+def _configure_additional_logging_handler_exclusively_for_farn(log_dir: Path):
+    """Create an additional logging handler exclusively for the farn log.
+
+    Parameters
+    ----------
+    log_dir : Path
+        folder in which the log file will be created
+    """
+    # Create log file
+    log_dir.mkdir(parents=True, exist_ok=True)
+    log_file = log_dir / "farn.log"
+    # Create logging file handler
+    file_handler = logging.FileHandler(str(log_file.absolute()), "a")
+    file_handler.name = str(log_file.absolute())
+    file_handler.setLevel(logging.INFO)
+    file_formatter = logging.Formatter("%(asctime)s %(levelname)-8s %(message)s", "%Y-%m-%d %H:%M:%S")
+    file_handler.setFormatter(file_formatter)
+    # Register file handler at root logger
+    root_logger = logging.getLogger()
+    file_handler_already_exists: bool = any(handler.name == file_handler.name for handler in root_logger.handlers)
+    if not file_handler_already_exists:
+        root_logger.addHandler(file_handler)
+    return
+
+
+def _remove_old_case_list_files():  # sourcery skip: avoid-builtin-shadow
+    """Remove old case list files, if existing."""
+    logger.info("Remove old case list files...")
+
+    lists = [list for list in Path.cwd().rglob("*") if re.search("(path|queue)List", str(list))]
+
+    for list in lists:
+        list = Path(list)
+        list.unlink()
+
+    logger.info("Successfully removed old case list files.")
+
+    return
+
+
+def _sys_call(shell_commands: MutableSequence[str]):
+    """Fallback function until _execute_command is usable under linux."""
+
+    for shell_command in shell_commands:
+        _ = os.system(shell_command)
+
+    return
+
+
+def _execute_shell_commands(shell_commands: MutableSequence[str]):
+    """Execute a sequence of shell commands using subprocess.
+
+    Parameters
+    ----------
+    shell_commands : MutableSequence
+        list with shell commands to be executed
+    """
+
+    # @TODO: until the problem with vanishing '.'s on Linux systems is solved (e.g. in command "ln -s target ."),
+    #        reroute the function call to _sys_call instead, as a workaround.
+    if platform.system() == "Linux":
+        _sys_call(shell_commands)
+        return
+
+    for shell_command in shell_commands:
+        _ = execute_in_sub_process(shell_command)
+
+    return
```

### Comparing `farn-0.3.6/src/farn/run/batchProcess.py` & `farn-0.3.7/src/farn/run/batchProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn/run/cli/batchProcess.py` & `farn-0.3.7/src/farn/run/cli/batchProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn/run/subProcess.py` & `farn-0.3.7/src/farn/run/subProcess.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn/run/utils/threading.py` & `farn-0.3.7/src/farn/run/utils/threading.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn/sampling/sampling.py` & `farn-0.3.7/src/farn/sampling/sampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,17 +237,15 @@
         # Assert that the number of values per parameter is the same for all parameters
         number_of_values_per_parameter: List[int] = [len(item) for item in self.sampling_parameters["_values"]]
         all_parameters_have_same_number_of_values: bool = all(
             number_of_values == number_of_values_per_parameter[0]  # (breakline)
             for number_of_values in number_of_values_per_parameter
         )
         if not all_parameters_have_same_number_of_values:
-            msg: str = (
-                "_values: The number of values per parameter need to be the same for all parameters. However, they are different."
-            )
+            msg: str = "_values: The number of values per parameter need to be the same for all parameters. However, they are different."
             logger.error(msg)
             raise ValueError(msg)
 
         self.number_of_samples = number_of_values_per_parameter[0]
         self.leading_zeros = int(math.log10(self.number_of_samples) - 1.0e-06) + 1
         self._generate_case_names(samples)
 
@@ -480,23 +478,19 @@
 
         if "_iterationDepth" in self.sampling_parameters.keys():
             if not isinstance(self.sampling_parameters["_iterationDepth"], int):
                 msg: str = f'_iterationDepth was not given as integer: {self.sampling_parameters["_iterationDepth"]}.'
                 logger.error(msg)
                 raise ValueError(msg)
             if self.sampling_parameters["_iterationDepth"] > self.maxIterationDepth:
-                msg: str = (
-                    f'_iterationDepth {self.sampling_parameters["_iterationDepth"]} given in farnDict is beyond the limit of {self.maxIterationDepth}...\n\t\tsetting to {self.maxIterationDepth}'
-                )
+                msg: str = f'_iterationDepth {self.sampling_parameters["_iterationDepth"]} given in farnDict is beyond the limit of {self.maxIterationDepth}...\n\t\tsetting to {self.maxIterationDepth}'
                 logger.warning(msg)
                 self.iteration_depth = self.maxIterationDepth
             elif self.sampling_parameters["_iterationDepth"] < self.minIterationDepth:
-                msg: str = (
-                    f'_iterationDepth {self.sampling_parameters["_iterationDepth"]} given in farnDict is below the limit of {self.minIterationDepth}...\n\t\tsetting to {self.minIterationDepth}'
-                )
+                msg: str = f'_iterationDepth {self.sampling_parameters["_iterationDepth"]} given in farnDict is below the limit of {self.minIterationDepth}...\n\t\tsetting to {self.minIterationDepth}'
                 logger.warning(msg)
                 self.iteration_depth = self.minIterationDepth
             else:
                 self.iteration_depth = self.sampling_parameters["_iterationDepth"]
         else:
             self.iteration_depth = 10
```

### Comparing `farn-0.3.6/src/farn/utils/logging.py` & `farn-0.3.7/src/farn/utils/logging.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/src/farn.egg-info/PKG-INFO` & `farn-0.3.7/src/farn.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: farn
-Version: 0.3.6
+Version: 0.3.7
 Summary: Python package to generate an n-dimensional case folder structure applying linear and spatial sampling strategies.
 Author-email: Frank Lumpitzsch <frank.lumpitzsch@dnv.com>, Claas Rostock <claas.rostock@dnv.com>
 Maintainer-email: Claas Rostock <claas.rostock@dnv.com>
 License: MIT License
         
         Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
         
@@ -44,25 +44,25 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=5.1
-Requires-Dist: numpy>=1.26
-Requires-Dist: scipy>=1.12
+Requires-Dist: lxml>=5.2
+Requires-Dist: numpy<2.0,>=1.26
+Requires-Dist: scipy>=1.13
 Requires-Dist: pandas>=2.2
-Requires-Dist: matplotlib>=3.8
-Requires-Dist: Pillow>=10.2
+Requires-Dist: matplotlib>=3.9
+Requires-Dist: Pillow>=10.3
 Requires-Dist: pyDOE3>=1.0
 Requires-Dist: psutil>=5.9
 Requires-Dist: hilbertcurve>=2.0.5
-Requires-Dist: dictIO>=0.3.3
-Requires-Dist: ospx>=0.2.13
+Requires-Dist: dictIO>=0.3.4
+Requires-Dist: ospx>=0.2.14
 
 # farn
 [farn][farn_docs] is an n-dimensional case generator.
 
 Its primary design goal is to parameterize and execute simulation cases.
 However, at its core, farn is use-case agnostic and can support a wide spectrum of applications.
 
@@ -181,32 +181,32 @@
 
     ```sh
     (.venv) $ pytest .
     ```
 
 ## Meta
 
-Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
+Copyright (c) 2024 [DNV](https://www.dnv.com) SE. All rights reserved.
 
 Frank Lumpitzsch – [@LinkedIn](https://www.linkedin.com/in/frank-lumpitzsch-23013196/) – frank.lumpitzsch@dnv.com
 
 Claas Rostock – [@LinkedIn](https://www.linkedin.com/in/claasrostock/?locale=en_US) – claas.rostock@dnv.com
 
 Seunghyeon Yoo – [@LinkedIn](https://www.linkedin.com/in/seunghyeon-yoo-3625173b/) – seunghyeon.yoo@dnv.com
 
 Distributed under the MIT license. See [LICENSE](LICENSE.md) for more information.
 
 [https://github.com/dnv-opensource/farn](https://github.com/dnv-opensource/farn)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/farn/fork>)
-2. Create your branch (`git checkout -b myBranchName`)
-3. Commit your changes (e.g. `git commit -m 'place a descriptive commit message here'`)
-4. Push to the branch (e.g. `git push origin myBranchName`)
+2. Create your branch (`git checkout -b my-branch-name`)
+3. Commit your changes (`git commit -am 'place a descriptive commit message here'`)
+4. Push to the branch (`git push origin my-branch-name`)
 5. Create a new Pull Request in GitHub
 
 For your contribution, please make sure you follow the [STYLEGUIDE](STYLEGUIDE.md) before creating the Pull Request.
 
 <!-- Markdown link & img dfn's -->
 [dictIO_docs]: https://dnv-opensource.github.io/dictIO/README.html
 [ospx_docs]: https://dnv-opensource.github.io/ospx/README.html
```

### Comparing `farn-0.3.6/src/farn.egg-info/SOURCES.txt` & `farn-0.3.7/src/farn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/tests/test_cases.py` & `farn-0.3.7/tests/test_cases.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/tests/test_farn.py` & `farn-0.3.7/tests/test_farn.py`

 * *Files identical despite different names*

### Comparing `farn-0.3.6/tests/test_sampling.py` & `farn-0.3.7/tests/test_sampling.py`

 * *Files identical despite different names*

