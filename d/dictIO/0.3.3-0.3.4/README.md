# Comparing `tmp/dictIO-0.3.3.tar.gz` & `tmp/dictio-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dictIO-0.3.3.tar", last modified: Wed Feb 21 20:08:12 2024, max compression
+gzip compressed data, was "dictio-0.3.4.tar", last modified: Wed May 22 16:47:04 2024, max compression
```

## Comparing `dictIO-0.3.3.tar` & `dictio-0.3.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.965335 dictIO-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-02-21 20:07:59.000000 dictIO-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-02-21 20:07:59.000000 dictIO-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-02-21 20:08:12.965335 dictIO-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5338 2024-02-21 20:07:59.000000 dictIO-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     5316 2024-02-21 20:07:59.000000 dictIO-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 20:08:12.965335 dictIO-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.957334 dictIO-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.961334 dictIO-0.3.3/src/dictIO/
--rw-r--r--   0 runner    (1001) docker     (127)      941 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.961334 dictIO-0.3.3/src/dictIO/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/cli/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/cppDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/dictParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/dictReader.py
--rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/dictWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    43887 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    72847 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.961334 dictIO-0.3.3/src/dictIO/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/utils/counter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/utils/path.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-02-21 20:07:59.000000 dictIO-0.3.3/src/dictIO/utils/strings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.965335 dictIO-0.3.3/src/dictIO.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8087 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-02-21 20:08:12.000000 dictIO-0.3.3/src/dictIO.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 20:08:12.961334 dictIO-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_dict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_dictParser.py
--rw-r--r--   0 runner    (1001) docker     (127)    25623 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_dictReader.py
--rw-r--r--   0 runner    (1001) docker     (127)    14442 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_dictWriter.py
--rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (127)    60357 2024-02-21 20:07:59.000000 dictIO-0.3.3/tests/test_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.983461 dictio-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-22 16:46:54.000000 dictio-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-22 16:46:54.000000 dictio-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-22 16:47:04.983461 dictio-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5309 2024-05-22 16:46:54.000000 dictio-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5284 2024-05-22 16:46:54.000000 dictio-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:47:04.983461 dictio-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.975461 dictio-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.979461 dictio-0.3.4/src/dictIO/
+-rw-r--r--   0 runner    (1001) docker     (127)      941 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.979461 dictio-0.3.4/src/dictIO/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6699 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/cli/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23420 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/cppDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13285 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6892 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43887 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72847 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.979461 dictio-0.3.4/src/dictIO/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/utils/counter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2113 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/utils/path.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-22 16:46:54.000000 dictio-0.3.4/src/dictIO/utils/strings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.983461 dictio-0.3.4/src/dictIO.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8063 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 16:47:04.000000 dictio-0.3.4/src/dictIO.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:47:04.979461 dictio-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_dict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_dictParser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25581 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_dictReader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14426 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_dictWriter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22374 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60357 2024-05-22 16:46:54.000000 dictio-0.3.4/tests/test_parser.py
```

### Comparing `dictIO-0.3.3/LICENSE` & `dictio-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/PKG-INFO` & `dictio-0.3.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to read, write and manipulate dictionary text files. Supports dictIOs dict file format, as well as JSON, XML and OpenFOAM.
 Author-email: Frank Lumpitzsch <frank.lumpitzsch@dnv.com>, Claas Rostock <claas.rostock@dnv.com>
 Maintainer-email: Claas Rostock <claas.rostock@dnv.com>
 License: MIT License
         
         Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
         
@@ -44,17 +44,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=5.1
+Requires-Dist: lxml>=5.2
 Requires-Dist: jsonschema>=4.20
-Requires-Dist: numpy>=1.26
+Requires-Dist: numpy<2.0,>=1.26
 
 # dictIO
 dictIO is a Python package to read, write and manipulate dictionary text files.
 
 It was designed to leverage the versatility of text based dictionary files, or 'dict files' in short, while easing their use in Python through seamless support for Python dicts.
 
 dictIO supports
@@ -168,32 +168,32 @@
 
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
 
 [https://github.com/dnv-opensource/dictIO](https://github.com/dnv-opensource/dictIO)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/dictIO/fork>)
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

### Comparing `dictIO-0.3.3/README.md` & `dictio-0.3.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -114,32 +114,32 @@
 
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
 
 [https://github.com/dnv-opensource/dictIO](https://github.com/dnv-opensource/dictIO)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/dictIO/fork>)
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

### Comparing `dictIO-0.3.3/pyproject.toml` & `dictio-0.3.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 00000010: 7265 7175 6972 6573 203d 205b 2273 6574  requires = ["set
 00000020: 7570 746f 6f6c 7322 2c20 2277 6865 656c  uptools", "wheel
 00000030: 225d 0d0a 6275 696c 642d 6261 636b 656e  "]..build-backen
 00000040: 6420 3d20 2273 6574 7570 746f 6f6c 732e  d = "setuptools.
 00000050: 6275 696c 645f 6d65 7461 220d 0a0d 0a5b  build_meta"....[
 00000060: 7072 6f6a 6563 745d 0d0a 6e61 6d65 203d  project]..name =
 00000070: 2022 6469 6374 494f 220d 0a76 6572 7369   "dictIO"..versi
-00000080: 6f6e 203d 2022 302e 332e 3322 0d0a 6465  on = "0.3.3"..de
+00000080: 6f6e 203d 2022 302e 332e 3422 0d0a 6465  on = "0.3.4"..de
 00000090: 7363 7269 7074 696f 6e20 3d20 2250 7974  scription = "Pyt
 000000a0: 686f 6e20 7061 636b 6167 6520 746f 2072  hon package to r
 000000b0: 6561 642c 2077 7269 7465 2061 6e64 206d  ead, write and m
 000000c0: 616e 6970 756c 6174 6520 6469 6374 696f  anipulate dictio
 000000d0: 6e61 7279 2074 6578 7420 6669 6c65 732e  nary text files.
 000000e0: 2053 7570 706f 7274 7320 6469 6374 494f   Supports dictIO
 000000f0: 7320 6469 6374 2066 696c 6520 666f 726d  s dict file form
@@ -76,258 +76,256 @@
 000004b0: 696e 6565 7269 6e67 222c 0d0a 2020 2020  ineering",..    
 000004c0: 2254 6f70 6963 203a 3a20 536f 6674 7761  "Topic :: Softwa
 000004d0: 7265 2044 6576 656c 6f70 6d65 6e74 203a  re Development :
 000004e0: 3a20 4c69 6272 6172 6965 7320 3a3a 2050  : Libraries :: P
 000004f0: 7974 686f 6e20 4d6f 6475 6c65 7322 2c0d  ython Modules",.
 00000500: 0a5d 0d0a 6465 7065 6e64 656e 6369 6573  .]..dependencies
 00000510: 203d 205b 0d0a 2020 2020 226c 786d 6c3e   = [..    "lxml>
-00000520: 3d35 2e31 222c 0d0a 2020 2020 226a 736f  =5.1",..    "jso
+00000520: 3d35 2e32 222c 0d0a 2020 2020 226a 736f  =5.2",..    "jso
 00000530: 6e73 6368 656d 613e 3d34 2e32 3022 2c0d  nschema>=4.20",.
 00000540: 0a20 2020 2022 6e75 6d70 793e 3d31 2e32  .    "numpy>=1.2
-00000550: 3622 2c0d 0a5d 0d0a 0d0a 5b70 726f 6a65  6",..]....[proje
-00000560: 6374 2e75 726c 735d 0d0a 486f 6d65 7061  ct.urls]..Homepa
-00000570: 6765 203d 2022 6874 7470 733a 2f2f 6769  ge = "https://gi
-00000580: 7468 7562 2e63 6f6d 2f64 6e76 2d6f 7065  thub.com/dnv-ope
-00000590: 6e73 6f75 7263 652f 6469 6374 494f 220d  nsource/dictIO".
-000005a0: 0a44 6f63 756d 656e 7461 7469 6f6e 203d  .Documentation =
-000005b0: 2022 6874 7470 733a 2f2f 646e 762d 6f70   "https://dnv-op
-000005c0: 656e 736f 7572 6365 2e67 6974 6875 622e  ensource.github.
-000005d0: 696f 2f64 6963 7449 4f2f 5245 4144 4d45  io/dictIO/README
-000005e0: 2e68 746d 6c22 0d0a 5265 706f 7369 746f  .html"..Reposito
-000005f0: 7279 203d 2022 6874 7470 733a 2f2f 6769  ry = "https://gi
-00000600: 7468 7562 2e63 6f6d 2f64 6e76 2d6f 7065  thub.com/dnv-ope
-00000610: 6e73 6f75 7263 652f 6469 6374 494f 2e67  nsource/dictIO.g
-00000620: 6974 220d 0a49 7373 7565 7320 3d20 2268  it"..Issues = "h
-00000630: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
-00000640: 6d2f 646e 762d 6f70 656e 736f 7572 6365  m/dnv-opensource
-00000650: 2f64 6963 7449 4f2f 6973 7375 6573 220d  /dictIO/issues".
-00000660: 0a43 6861 6e67 656c 6f67 203d 2022 6874  .Changelog = "ht
-00000670: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
-00000680: 2f64 6e76 2d6f 7065 6e73 6f75 7263 652f  /dnv-opensource/
-00000690: 6469 6374 494f 2f62 6c6f 622f 6d61 696e  dictIO/blob/main
-000006a0: 2f43 4841 4e47 454c 4f47 2e6d 6422 0d0a  /CHANGELOG.md"..
-000006b0: 0d0a 5b70 726f 6a65 6374 2e73 6372 6970  ..[project.scrip
-000006c0: 7473 5d0d 0a64 6963 7450 6172 7365 7220  ts]..dictParser 
-000006d0: 3d20 2264 6963 7449 4f2e 636c 692e 6469  = "dictIO.cli.di
-000006e0: 6374 5061 7273 6572 3a6d 6169 6e22 0d0a  ctParser:main"..
-000006f0: 0d0a 5b74 6f6f 6c2e 7365 7475 7074 6f6f  ..[tool.setuptoo
-00000700: 6c73 2e70 6163 6b61 6765 732e 6669 6e64  ls.packages.find
-00000710: 5d0d 0a77 6865 7265 203d 205b 2273 7263  ]..where = ["src
-00000720: 225d 0d0a 6578 636c 7564 6520 3d20 5b22  "]..exclude = ["
-00000730: 7465 7374 2a22 5d0d 0a0d 0a5b 746f 6f6c  test*"]....[tool
-00000740: 2e62 6c61 636b 5d0d 0a6c 696e 652d 6c65  .black]..line-le
-00000750: 6e67 7468 203d 2031 3230 0d0a 7461 7267  ngth = 120..targ
-00000760: 6574 2d76 6572 7369 6f6e 203d 205b 2270  et-version = ["p
-00000770: 7933 3922 2c20 2270 7933 3130 222c 2022  y39", "py310", "
-00000780: 7079 3331 3122 2c20 2270 7933 3132 225d  py311", "py312"]
-00000790: 0d0a 0d0a 5b74 6f6f 6c2e 7275 6666 5d0d  ....[tool.ruff].
-000007a0: 0a65 7863 6c75 6465 203d 205b 0d0a 2020  .exclude = [..  
-000007b0: 2020 222e 6769 7422 2c0d 0a20 2020 2022    ".git",..    "
-000007c0: 2e76 656e 7622 2c0d 0a20 2020 2022 2e74  .venv",..    ".t
-000007d0: 6f78 222c 0d0a 2020 2020 2262 7569 6c64  ox",..    "build
-000007e0: 222c 0d0a 2020 2020 2264 6973 7422 2c0d  ",..    "dist",.
-000007f0: 0a20 2020 2022 5f5f 7079 6361 6368 655f  .    "__pycache_
-00000800: 5f22 2c0d 0a20 2020 2022 2e2f 646f 6373  _",..    "./docs
-00000810: 2f73 6f75 7263 652f 636f 6e66 2e70 7922  /source/conf.py"
-00000820: 2c0d 0a5d 0d0a 7372 6320 3d20 5b22 7372  ,..]..src = ["sr
-00000830: 6322 5d0d 0a6c 696e 652d 6c65 6e67 7468  c"]..line-length
-00000840: 203d 2031 3230 0d0a 7461 7267 6574 2d76   = 120..target-v
-00000850: 6572 7369 6f6e 203d 2022 7079 3339 220d  ersion = "py39".
-00000860: 0a0d 0a5b 746f 6f6c 2e72 7566 662e 6c69  ...[tool.ruff.li
-00000870: 6e74 5d0d 0a69 676e 6f72 6520 3d20 5b0d  nt]..ignore = [.
-00000880: 0a20 2020 2022 4535 3031 222c 2020 2320  .    "E501",  # 
-00000890: 4c69 6e65 206c 656e 6774 6820 746f 6f20  Line length too 
-000008a0: 6c6f 6e67 0d0a 2020 2020 2244 3130 3022  long..    "D100"
-000008b0: 2c20 2023 204d 6973 7369 6e67 2064 6f63  ,  # Missing doc
-000008c0: 7374 7269 6e67 2069 6e20 7075 626c 6963  string in public
-000008d0: 206d 6f64 756c 650d 0a20 2020 2022 4431   module..    "D1
-000008e0: 3034 222c 2020 2320 4d69 7373 696e 6720  04",  # Missing 
-000008f0: 646f 6373 7472 696e 6720 696e 2070 7562  docstring in pub
-00000900: 6c69 6320 7061 636b 6167 650d 0a20 2020  lic package..   
-00000910: 2022 4431 3035 222c 2020 2320 4d69 7373   "D105",  # Miss
-00000920: 696e 6720 646f 6373 7472 696e 6720 696e  ing docstring in
-00000930: 206d 6167 6963 206d 6574 686f 640d 0a20   magic method.. 
-00000940: 2020 2022 4431 3037 222c 2020 2320 4d69     "D107",  # Mi
-00000950: 7373 696e 6720 646f 6373 7472 696e 6720  ssing docstring 
-00000960: 696e 205f 5f69 6e69 745f 5f0d 0a20 2020  in __init__..   
-00000970: 2022 4432 3032 222c 2020 2320 4e6f 2062   "D202",  # No b
-00000980: 6c61 6e6b 206c 696e 6573 2061 6c6c 6f77  lank lines allow
-00000990: 6564 2061 6674 6572 2066 756e 6374 696f  ed after functio
-000009a0: 6e20 646f 6373 7472 696e 670d 0a20 2020  n docstring..   
-000009b0: 2022 4432 3033 222c 2020 2320 3120 626c   "D203",  # 1 bl
-000009c0: 616e 6b20 6c69 6e65 2072 6571 7569 7265  ank line require
-000009d0: 6420 6265 666f 7265 2063 6c61 7373 2064  d before class d
-000009e0: 6f63 7374 7269 6e67 0d0a 2020 2020 2244  ocstring..    "D
-000009f0: 3230 3522 2c20 2023 2031 2062 6c61 6e6b  205",  # 1 blank
-00000a00: 206c 696e 6520 7265 7175 6972 6564 2062   line required b
-00000a10: 6574 7765 656e 2073 756d 6d61 7279 206c  etween summary l
-00000a20: 696e 6520 616e 6420 6465 7363 7269 7074  ine and descript
-00000a30: 696f 6e0d 0a20 2020 2022 4432 3132 222c  ion..    "D212",
-00000a40: 2020 2320 4d75 6c74 692d 6c69 6e65 2064    # Multi-line d
-00000a50: 6f63 7374 7269 6e67 2073 756d 6d61 7279  ocstring summary
-00000a60: 2073 686f 756c 6420 7374 6172 7420 6174   should start at
-00000a70: 2074 6865 2066 6972 7374 206c 696e 650d   the first line.
-00000a80: 0a20 2020 2022 4432 3133 222c 2020 2320  .    "D213",  # 
-00000a90: 4d75 6c74 692d 6c69 6e65 2064 6f63 7374  Multi-line docst
-00000aa0: 7269 6e67 2073 756d 6d61 7279 2073 686f  ring summary sho
-00000ab0: 756c 6420 7374 6172 7420 6174 2074 6865  uld start at the
-00000ac0: 2073 6563 6f6e 6420 6c69 6e65 0d0a 2020   second line..  
-00000ad0: 2020 2320 224e 3830 3222 2c20 2023 2046    # "N802",  # F
-00000ae0: 756e 6374 696f 6e20 6e61 6d65 2073 686f  unction name sho
-00000af0: 756c 6420 6265 206c 6f77 6572 6361 7365  uld be lowercase
-00000b00: 2020 2875 6e63 6f6d 6d65 6e74 2069 6620    (uncomment if 
-00000b10: 796f 7520 7761 6e74 2074 6f20 616c 6c6f  you want to allo
-00000b20: 7720 5570 7065 7263 6173 6520 6675 6e63  w Uppercase func
-00000b30: 7469 6f6e 206e 616d 6573 290d 0a20 2020  tion names)..   
-00000b40: 2023 2022 4e38 3033 222c 2020 2320 4172   # "N803",  # Ar
-00000b50: 6775 6d65 6e74 206e 616d 6520 7368 6f75  gument name shou
-00000b60: 6c64 2062 6520 6c6f 7765 7263 6173 6520  ld be lowercase 
-00000b70: 2028 756e 636f 6d6d 656e 7420 6966 2079   (uncomment if y
-00000b80: 6f75 2077 616e 7420 746f 2061 6c6c 6f77  ou want to allow
-00000b90: 2055 7070 6572 6361 7365 2061 7267 756d   Uppercase argum
-00000ba0: 656e 7420 6e61 6d65 7329 0d0a 2020 2020  ent names)..    
-00000bb0: 224e 3830 3622 2c20 2023 2056 6172 6961  "N806",  # Varia
-00000bc0: 626c 6520 696e 2066 756e 6374 696f 6e20  ble in function 
-00000bd0: 7368 6f75 6c64 2062 6520 6c6f 7765 7263  should be lowerc
-00000be0: 6173 6520 2028 756e 636f 6d6d 656e 7420  ase  (uncomment 
-00000bf0: 6966 2079 6f75 2077 616e 7420 746f 2061  if you want to a
-00000c00: 6c6c 6f77 2055 7070 6572 6361 7365 2076  llow Uppercase v
-00000c10: 6172 6961 626c 6520 6e61 6d65 7320 696e  ariable names in
-00000c20: 2066 756e 6374 696f 6e73 290d 0a20 2020   functions)..   
-00000c30: 2023 2022 4e38 3135 222c 2020 2320 5661   # "N815",  # Va
-00000c40: 7269 6162 6c65 2069 6e20 636c 6173 7320  riable in class 
-00000c50: 7363 6f70 6520 7368 6f75 6c64 206e 6f74  scope should not
-00000c60: 2062 6520 6d69 7865 6443 6173 6520 2028   be mixedCase  (
-00000c70: 756e 636f 6d6d 656e 7420 6966 2079 6f75  uncomment if you
-00000c80: 2077 616e 7420 746f 2061 6c6c 6f77 206d   want to allow m
-00000c90: 6978 6564 4361 7365 2076 6172 6961 626c  ixedCase variabl
-00000ca0: 6520 6e61 6d65 7320 696e 2063 6c61 7373  e names in class
-00000cb0: 2073 636f 7065 290d 0a20 2020 2023 2022   scope)..    # "
-00000cc0: 4e38 3136 222c 2020 2320 5661 7269 6162  N816",  # Variab
-00000cd0: 6c65 2069 6e20 676c 6f62 616c 2073 636f  le in global sco
-00000ce0: 7065 2073 686f 756c 6420 6e6f 7420 6265  pe should not be
-00000cf0: 206d 6978 6564 4361 7365 2020 2875 6e63   mixedCase  (unc
-00000d00: 6f6d 6d65 6e74 2069 6620 796f 7520 7761  omment if you wa
-00000d10: 6e74 2074 6f20 616c 6c6f 7720 6d69 7865  nt to allow mixe
-00000d20: 6443 6173 6520 7661 7269 6162 6c65 206e  dCase variable n
-00000d30: 616d 6573 2069 6e20 676c 6f62 616c 2073  ames in global s
-00000d40: 636f 7065 290d 0a20 2020 2022 4e39 3939  cope)..    "N999
-00000d50: 222c 2020 2320 496e 7661 6c69 6420 6d6f  ",  # Invalid mo
-00000d60: 6475 6c65 206e 616d 650d 0a20 2020 205d  dule name..    ]
-00000d70: 0d0a 7365 6c65 6374 203d 205b 0d0a 2020  ..select = [..  
-00000d80: 2020 2245 222c 0d0a 2020 2020 2244 222c    "E",..    "D",
-00000d90: 0d0a 2020 2020 2246 222c 0d0a 2020 2020  ..    "F",..    
-00000da0: 224e 222c 0d0a 2020 2020 2257 222c 0d0a  "N",..    "W",..
-00000db0: 2020 2020 2249 222c 0d0a 2020 2020 2242      "I",..    "B
-00000dc0: 222c 0d0a 5d0d 0a0d 0a5b 746f 6f6c 2e72  ",..]....[tool.r
-00000dd0: 7566 662e 6c69 6e74 2e70 6570 382d 6e61  uff.lint.pep8-na
-00000de0: 6d69 6e67 5d0d 0a69 676e 6f72 652d 6e61  ming]..ignore-na
-00000df0: 6d65 7320 3d20 5b0d 0a20 2020 2022 7465  mes = [..    "te
-00000e00: 7374 5f2a 222c 0d0a 2020 2020 2273 6574  st_*",..    "set
-00000e10: 5570 222c 0d0a 2020 2020 2274 6561 7244  Up",..    "tearD
-00000e20: 6f77 6e22 2c0d 0a5d 0d0a 0d0a 5b74 6f6f  own",..]....[too
-00000e30: 6c2e 7275 6666 2e6c 696e 742e 7079 646f  l.ruff.lint.pydo
-00000e40: 6373 7479 6c65 5d0d 0a63 6f6e 7665 6e74  cstyle]..convent
-00000e50: 696f 6e20 3d20 226e 756d 7079 220d 0a0d  ion = "numpy"...
-00000e60: 0a5b 746f 6f6c 2e72 7566 662e 6c69 6e74  .[tool.ruff.lint
-00000e70: 2e70 6572 2d66 696c 652d 6967 6e6f 7265  .per-file-ignore
-00000e80: 735d 0d0a 225f 5f69 6e69 745f 5f2e 7079  s].."__init__.py
-00000e90: 2220 3d20 5b22 4930 3031 225d 0d0a 222e  " = ["I001"]..".
-00000ea0: 2f74 6573 7473 2f2a 2220 3d20 5b22 4422  /tests/*" = ["D"
-00000eb0: 5d0d 0a0d 0a5b 746f 6f6c 2e70 7972 6967  ]....[tool.pyrig
-00000ec0: 6874 5d0d 0a65 7863 6c75 6465 203d 205b  ht]..exclude = [
-00000ed0: 0d0a 2020 2020 222e 6769 7422 2c0d 0a20  ..    ".git",.. 
-00000ee0: 2020 2022 2e76 656e 7622 2c0d 0a20 2020     ".venv",..   
-00000ef0: 2022 2e74 6f78 222c 0d0a 2020 2020 2262   ".tox",..    "b
-00000f00: 7569 6c64 222c 0d0a 2020 2020 2264 6973  uild",..    "dis
-00000f10: 7422 2c0d 0a20 2020 2022 2a2a 2f5f 5f70  t",..    "**/__p
-00000f20: 7963 6163 6865 5f5f 222c 0d0a 2020 2020  ycache__",..    
-00000f30: 222e 2f64 6f63 732f 736f 7572 6365 2f63  "./docs/source/c
-00000f40: 6f6e 662e 7079 222c 0d0a 2020 2020 222e  onf.py",..    ".
-00000f50: 2f76 656e 7622 2c0d 0a5d 0d0a 6578 7472  /venv",..]..extr
-00000f60: 6150 6174 6873 203d 205b 222e 2f73 7263  aPaths = ["./src
-00000f70: 225d 0d0a 7479 7065 4368 6563 6b69 6e67  "]..typeChecking
-00000f80: 4d6f 6465 203d 2022 6261 7369 6322 0d0a  Mode = "basic"..
-00000f90: 7573 654c 6962 7261 7279 436f 6465 466f  useLibraryCodeFo
-00000fa0: 7254 7970 6573 203d 2074 7275 650d 0a72  rTypes = true..r
-00000fb0: 6570 6f72 744d 6973 7369 6e67 5061 7261  eportMissingPara
-00000fc0: 6d65 7465 7254 7970 6520 3d20 2265 7272  meterType = "err
-00000fd0: 6f72 220d 0a72 6570 6f72 7455 6e6b 6e6f  or"..reportUnkno
-00000fe0: 776e 5061 7261 6d65 7465 7254 7970 6520  wnParameterType 
-00000ff0: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
-00001000: 6f72 7455 6e6b 6e6f 776e 4d65 6d62 6572  ortUnknownMember
-00001010: 5479 7065 203d 2022 7761 726e 696e 6722  Type = "warning"
-00001020: 0d0a 7265 706f 7274 4d69 7373 696e 6754  ..reportMissingT
-00001030: 7970 6541 7267 756d 656e 7420 3d20 2265  ypeArgument = "e
-00001040: 7272 6f72 220d 0a72 6570 6f72 7450 726f  rror"..reportPro
-00001050: 7065 7274 7954 7970 654d 6973 6d61 7463  pertyTypeMismatc
-00001060: 6820 3d20 2265 7272 6f72 220d 0a72 6570  h = "error"..rep
-00001070: 6f72 7446 756e 6374 696f 6e4d 656d 6265  ortFunctionMembe
-00001080: 7241 6363 6573 7320 3d20 2277 6172 6e69  rAccess = "warni
-00001090: 6e67 220d 0a72 6570 6f72 7450 7269 7661  ng"..reportPriva
-000010a0: 7465 5573 6167 6520 3d20 2277 6172 6e69  teUsage = "warni
-000010b0: 6e67 220d 0a72 6570 6f72 7454 7970 6543  ng"..reportTypeC
-000010c0: 6f6d 6d65 6e74 5573 6167 6520 3d20 2277  ommentUsage = "w
-000010d0: 6172 6e69 6e67 220d 0a72 6570 6f72 7449  arning"..reportI
-000010e0: 6e63 6f6d 7061 7469 626c 654d 6574 686f  ncompatibleMetho
-000010f0: 644f 7665 7272 6964 6520 3d20 2277 6172  dOverride = "war
-00001100: 6e69 6e67 220d 0a72 6570 6f72 7449 6e63  ning"..reportInc
-00001110: 6f6d 7061 7469 626c 6556 6172 6961 626c  ompatibleVariabl
-00001120: 654f 7665 7272 6964 6520 3d20 2265 7272  eOverride = "err
-00001130: 6f72 220d 0a72 6570 6f72 7449 6e63 6f6e  or"..reportIncon
-00001140: 7369 7374 656e 7443 6f6e 7374 7275 6374  sistentConstruct
-00001150: 6f72 203d 2022 6572 726f 7222 0d0a 7265  or = "error"..re
-00001160: 706f 7274 4f76 6572 6c61 7070 696e 674f  portOverlappingO
-00001170: 7665 726c 6f61 6420 3d20 2277 6172 6e69  verload = "warni
-00001180: 6e67 220d 0a72 6570 6f72 7455 6e69 6e69  ng"..reportUnini
-00001190: 7469 616c 697a 6564 496e 7374 616e 6365  tializedInstance
-000011a0: 5661 7269 6162 6c65 203d 2022 7761 726e  Variable = "warn
-000011b0: 696e 6722 0d0a 7265 706f 7274 4361 6c6c  ing"..reportCall
-000011c0: 496e 4465 6661 756c 7449 6e69 7469 616c  InDefaultInitial
-000011d0: 697a 6572 203d 2022 7761 726e 696e 6722  izer = "warning"
-000011e0: 0d0a 7265 706f 7274 556e 6e65 6365 7373  ..reportUnnecess
-000011f0: 6172 7949 7349 6e73 7461 6e63 6520 3d20  aryIsInstance = 
-00001200: 2269 6e66 6f72 6d61 7469 6f6e 220d 0a72  "information"..r
-00001210: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
-00001220: 4361 7374 203d 2022 7761 726e 696e 6722  Cast = "warning"
-00001230: 0d0a 7265 706f 7274 556e 6e65 6365 7373  ..reportUnnecess
-00001240: 6172 7943 6f6d 7061 7269 736f 6e20 3d20  aryComparison = 
-00001250: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
-00001260: 7455 6e6e 6563 6573 7361 7279 436f 6e74  tUnnecessaryCont
-00001270: 6169 6e73 203d 2022 7761 726e 696e 6722  ains = "warning"
-00001280: 0d0a 7265 706f 7274 556e 7573 6564 4361  ..reportUnusedCa
-00001290: 6c6c 5265 7375 6c74 203d 2022 7761 726e  llResult = "warn
-000012a0: 696e 6722 0d0a 7265 706f 7274 556e 7573  ing"..reportUnus
-000012b0: 6564 4578 7072 6573 7369 6f6e 203d 2022  edExpression = "
-000012c0: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
-000012d0: 4d61 7463 684e 6f74 4578 6861 7573 7469  MatchNotExhausti
-000012e0: 7665 203d 2022 7761 726e 696e 6722 0d0a  ve = "warning"..
-000012f0: 7265 706f 7274 5368 6164 6f77 6564 496d  reportShadowedIm
-00001300: 706f 7274 7320 3d20 2277 6172 6e69 6e67  ports = "warning
-00001310: 220d 0a72 6570 6f72 7455 6e74 7970 6564  "..reportUntyped
-00001320: 4675 6e63 7469 6f6e 4465 636f 7261 746f  FunctionDecorato
-00001330: 7220 3d20 2277 6172 6e69 6e67 220d 0a72  r = "warning"..r
-00001340: 6570 6f72 7455 6e74 7970 6564 4261 7365  eportUntypedBase
-00001350: 436c 6173 7320 3d20 2265 7272 6f72 220d  Class = "error".
-00001360: 0a72 6570 6f72 7455 6e74 7970 6564 4e61  .reportUntypedNa
-00001370: 6d65 6454 7570 6c65 203d 2022 7761 726e  medTuple = "warn
-00001380: 696e 6722 0d0a 2320 4163 7469 7661 7465  ing"..# Activate
-00001390: 2074 6865 2066 6f6c 6c6f 7769 6e67 2072   the following r
-000013a0: 756c 6573 206f 6e6c 7920 6c6f 6361 6c6c  ules only locall
-000013b0: 7920 616e 6420 7465 6d70 6f72 6172 792c  y and temporary,
-000013c0: 2069 2e65 2e20 666f 7220 6120 5141 2073   i.e. for a QA s
-000013d0: 6573 7369 6f6e 2e0d 0a23 2028 466f 7220  ession...# (For 
-000013e0: 7365 7276 6572 2073 6964 6520 4349 2074  server side CI t
-000013f0: 6865 7920 6172 6520 636f 6e73 6964 6572  hey are consider
-00001400: 6564 2074 6f6f 2073 7472 6963 742e 290d  ed too strict.).
-00001410: 0a23 2072 6570 6f72 7443 6f6e 7374 616e  .# reportConstan
-00001420: 7452 6564 6566 696e 6974 696f 6e20 3d20  tRedefinition = 
-00001430: 2277 6172 6e69 6e67 220d 0a23 2072 6570  "warning"..# rep
-00001440: 6f72 7455 6e6e 6563 6573 7361 7279 5479  ortUnnecessaryTy
-00001450: 7065 4967 6e6f 7265 436f 6d6d 656e 7420  peIgnoreComment 
-00001460: 3d20 2269 6e66 6f72 6d61 7469 6f6e 220d  = "information".
-00001470: 0a23 2072 6570 6f72 7449 6d70 6f72 7443  .# reportImportC
-00001480: 7963 6c65 7320 3d20 2277 6172 6e69 6e67  ycles = "warning
-00001490: 220d 0a23 2072 6570 6f72 7449 6d70 6c69  "..# reportImpli
-000014a0: 6369 7453 7472 696e 6743 6f6e 6361 7465  citStringConcate
-000014b0: 6e61 7469 6f6e 203d 2022 7761 726e 696e  nation = "warnin
-000014c0: 6722 0d0a                                g"..
+00000550: 362c 3c32 2e30 222c 0d0a 5d0d 0a0d 0a5b  6,<2.0",..]....[
+00000560: 7072 6f6a 6563 742e 7572 6c73 5d0d 0a48  project.urls]..H
+00000570: 6f6d 6570 6167 6520 3d20 2268 7474 7073  omepage = "https
+00000580: 3a2f 2f67 6974 6875 622e 636f 6d2f 646e  ://github.com/dn
+00000590: 762d 6f70 656e 736f 7572 6365 2f64 6963  v-opensource/dic
+000005a0: 7449 4f22 0d0a 446f 6375 6d65 6e74 6174  tIO"..Documentat
+000005b0: 696f 6e20 3d20 2268 7474 7073 3a2f 2f64  ion = "https://d
+000005c0: 6e76 2d6f 7065 6e73 6f75 7263 652e 6769  nv-opensource.gi
+000005d0: 7468 7562 2e69 6f2f 6469 6374 494f 2f52  thub.io/dictIO/R
+000005e0: 4541 444d 452e 6874 6d6c 220d 0a52 6570  EADME.html"..Rep
+000005f0: 6f73 6974 6f72 7920 3d20 2268 7474 7073  ository = "https
+00000600: 3a2f 2f67 6974 6875 622e 636f 6d2f 646e  ://github.com/dn
+00000610: 762d 6f70 656e 736f 7572 6365 2f64 6963  v-opensource/dic
+00000620: 7449 4f2e 6769 7422 0d0a 4973 7375 6573  tIO.git"..Issues
+00000630: 203d 2022 6874 7470 733a 2f2f 6769 7468   = "https://gith
+00000640: 7562 2e63 6f6d 2f64 6e76 2d6f 7065 6e73  ub.com/dnv-opens
+00000650: 6f75 7263 652f 6469 6374 494f 2f69 7373  ource/dictIO/iss
+00000660: 7565 7322 0d0a 4368 616e 6765 6c6f 6720  ues"..Changelog 
+00000670: 3d20 2268 7474 7073 3a2f 2f67 6974 6875  = "https://githu
+00000680: 622e 636f 6d2f 646e 762d 6f70 656e 736f  b.com/dnv-openso
+00000690: 7572 6365 2f64 6963 7449 4f2f 626c 6f62  urce/dictIO/blob
+000006a0: 2f6d 6169 6e2f 4348 414e 4745 4c4f 472e  /main/CHANGELOG.
+000006b0: 6d64 220d 0a0d 0a5b 7072 6f6a 6563 742e  md"....[project.
+000006c0: 7363 7269 7074 735d 0d0a 6469 6374 5061  scripts]..dictPa
+000006d0: 7273 6572 203d 2022 6469 6374 494f 2e63  rser = "dictIO.c
+000006e0: 6c69 2e64 6963 7450 6172 7365 723a 6d61  li.dictParser:ma
+000006f0: 696e 220d 0a0d 0a5b 746f 6f6c 2e73 6574  in"....[tool.set
+00000700: 7570 746f 6f6c 732e 7061 636b 6167 6573  uptools.packages
+00000710: 2e66 696e 645d 0d0a 7768 6572 6520 3d20  .find]..where = 
+00000720: 5b22 7372 6322 5d0d 0a65 7863 6c75 6465  ["src"]..exclude
+00000730: 203d 205b 2274 6573 742a 225d 0d0a 0d0a   = ["test*"]....
+00000740: 5b74 6f6f 6c2e 7275 6666 5d0d 0a65 7863  [tool.ruff]..exc
+00000750: 6c75 6465 203d 205b 0d0a 2020 2020 222e  lude = [..    ".
+00000760: 6769 7422 2c0d 0a20 2020 2022 2e76 656e  git",..    ".ven
+00000770: 7622 2c0d 0a20 2020 2022 2e74 6f78 222c  v",..    ".tox",
+00000780: 0d0a 2020 2020 2262 7569 6c64 222c 0d0a  ..    "build",..
+00000790: 2020 2020 2264 6973 7422 2c0d 0a20 2020      "dist",..   
+000007a0: 2022 5f5f 7079 6361 6368 655f 5f22 2c0d   "__pycache__",.
+000007b0: 0a20 2020 2022 2e2f 646f 6373 2f73 6f75  .    "./docs/sou
+000007c0: 7263 652f 636f 6e66 2e70 7922 2c0d 0a5d  rce/conf.py",..]
+000007d0: 0d0a 7372 6320 3d20 5b22 7372 6322 5d0d  ..src = ["src"].
+000007e0: 0a6c 696e 652d 6c65 6e67 7468 203d 2031  .line-length = 1
+000007f0: 3230 0d0a 7461 7267 6574 2d76 6572 7369  20..target-versi
+00000800: 6f6e 203d 2022 7079 3339 220d 0a0d 0a5b  on = "py39"....[
+00000810: 746f 6f6c 2e72 7566 662e 6c69 6e74 5d0d  tool.ruff.lint].
+00000820: 0a69 676e 6f72 6520 3d20 5b0d 0a20 2020  .ignore = [..   
+00000830: 2022 4535 3031 222c 2020 2320 4c69 6e65   "E501",  # Line
+00000840: 206c 656e 6774 6820 746f 6f20 6c6f 6e67   length too long
+00000850: 0d0a 2020 2020 2244 3130 3022 2c20 2023  ..    "D100",  #
+00000860: 204d 6973 7369 6e67 2064 6f63 7374 7269   Missing docstri
+00000870: 6e67 2069 6e20 7075 626c 6963 206d 6f64  ng in public mod
+00000880: 756c 650d 0a20 2020 2022 4431 3034 222c  ule..    "D104",
+00000890: 2020 2320 4d69 7373 696e 6720 646f 6373    # Missing docs
+000008a0: 7472 696e 6720 696e 2070 7562 6c69 6320  tring in public 
+000008b0: 7061 636b 6167 650d 0a20 2020 2022 4431  package..    "D1
+000008c0: 3035 222c 2020 2320 4d69 7373 696e 6720  05",  # Missing 
+000008d0: 646f 6373 7472 696e 6720 696e 206d 6167  docstring in mag
+000008e0: 6963 206d 6574 686f 640d 0a20 2020 2022  ic method..    "
+000008f0: 4431 3037 222c 2020 2320 4d69 7373 696e  D107",  # Missin
+00000900: 6720 646f 6373 7472 696e 6720 696e 205f  g docstring in _
+00000910: 5f69 6e69 745f 5f0d 0a20 2020 2022 4432  _init__..    "D2
+00000920: 3032 222c 2020 2320 4e6f 2062 6c61 6e6b  02",  # No blank
+00000930: 206c 696e 6573 2061 6c6c 6f77 6564 2061   lines allowed a
+00000940: 6674 6572 2066 756e 6374 696f 6e20 646f  fter function do
+00000950: 6373 7472 696e 670d 0a20 2020 2022 4432  cstring..    "D2
+00000960: 3033 222c 2020 2320 3120 626c 616e 6b20  03",  # 1 blank 
+00000970: 6c69 6e65 2072 6571 7569 7265 6420 6265  line required be
+00000980: 666f 7265 2063 6c61 7373 2064 6f63 7374  fore class docst
+00000990: 7269 6e67 0d0a 2020 2020 2244 3230 3522  ring..    "D205"
+000009a0: 2c20 2023 2031 2062 6c61 6e6b 206c 696e  ,  # 1 blank lin
+000009b0: 6520 7265 7175 6972 6564 2062 6574 7765  e required betwe
+000009c0: 656e 2073 756d 6d61 7279 206c 696e 6520  en summary line 
+000009d0: 616e 6420 6465 7363 7269 7074 696f 6e0d  and description.
+000009e0: 0a20 2020 2022 4432 3132 222c 2020 2320  .    "D212",  # 
+000009f0: 4d75 6c74 692d 6c69 6e65 2064 6f63 7374  Multi-line docst
+00000a00: 7269 6e67 2073 756d 6d61 7279 2073 686f  ring summary sho
+00000a10: 756c 6420 7374 6172 7420 6174 2074 6865  uld start at the
+00000a20: 2066 6972 7374 206c 696e 650d 0a20 2020   first line..   
+00000a30: 2022 4432 3133 222c 2020 2320 4d75 6c74   "D213",  # Mult
+00000a40: 692d 6c69 6e65 2064 6f63 7374 7269 6e67  i-line docstring
+00000a50: 2073 756d 6d61 7279 2073 686f 756c 6420   summary should 
+00000a60: 7374 6172 7420 6174 2074 6865 2073 6563  start at the sec
+00000a70: 6f6e 6420 6c69 6e65 0d0a 2020 2020 2320  ond line..    # 
+00000a80: 224e 3830 3222 2c20 2023 2046 756e 6374  "N802",  # Funct
+00000a90: 696f 6e20 6e61 6d65 2073 686f 756c 6420  ion name should 
+00000aa0: 6265 206c 6f77 6572 6361 7365 2020 2875  be lowercase  (u
+00000ab0: 6e63 6f6d 6d65 6e74 2069 6620 796f 7520  ncomment if you 
+00000ac0: 7761 6e74 2074 6f20 616c 6c6f 7720 5570  want to allow Up
+00000ad0: 7065 7263 6173 6520 6675 6e63 7469 6f6e  percase function
+00000ae0: 206e 616d 6573 290d 0a20 2020 2023 2022   names)..    # "
+00000af0: 4e38 3033 222c 2020 2320 4172 6775 6d65  N803",  # Argume
+00000b00: 6e74 206e 616d 6520 7368 6f75 6c64 2062  nt name should b
+00000b10: 6520 6c6f 7765 7263 6173 6520 2028 756e  e lowercase  (un
+00000b20: 636f 6d6d 656e 7420 6966 2079 6f75 2077  comment if you w
+00000b30: 616e 7420 746f 2061 6c6c 6f77 2055 7070  ant to allow Upp
+00000b40: 6572 6361 7365 2061 7267 756d 656e 7420  ercase argument 
+00000b50: 6e61 6d65 7329 0d0a 2020 2020 224e 3830  names)..    "N80
+00000b60: 3622 2c20 2023 2056 6172 6961 626c 6520  6",  # Variable 
+00000b70: 696e 2066 756e 6374 696f 6e20 7368 6f75  in function shou
+00000b80: 6c64 2062 6520 6c6f 7765 7263 6173 6520  ld be lowercase 
+00000b90: 2028 756e 636f 6d6d 656e 7420 6966 2079   (uncomment if y
+00000ba0: 6f75 2077 616e 7420 746f 2061 6c6c 6f77  ou want to allow
+00000bb0: 2055 7070 6572 6361 7365 2076 6172 6961   Uppercase varia
+00000bc0: 626c 6520 6e61 6d65 7320 696e 2066 756e  ble names in fun
+00000bd0: 6374 696f 6e73 290d 0a20 2020 2023 2022  ctions)..    # "
+00000be0: 4e38 3135 222c 2020 2320 5661 7269 6162  N815",  # Variab
+00000bf0: 6c65 2069 6e20 636c 6173 7320 7363 6f70  le in class scop
+00000c00: 6520 7368 6f75 6c64 206e 6f74 2062 6520  e should not be 
+00000c10: 6d69 7865 6443 6173 6520 2028 756e 636f  mixedCase  (unco
+00000c20: 6d6d 656e 7420 6966 2079 6f75 2077 616e  mment if you wan
+00000c30: 7420 746f 2061 6c6c 6f77 206d 6978 6564  t to allow mixed
+00000c40: 4361 7365 2076 6172 6961 626c 6520 6e61  Case variable na
+00000c50: 6d65 7320 696e 2063 6c61 7373 2073 636f  mes in class sco
+00000c60: 7065 290d 0a20 2020 2023 2022 4e38 3136  pe)..    # "N816
+00000c70: 222c 2020 2320 5661 7269 6162 6c65 2069  ",  # Variable i
+00000c80: 6e20 676c 6f62 616c 2073 636f 7065 2073  n global scope s
+00000c90: 686f 756c 6420 6e6f 7420 6265 206d 6978  hould not be mix
+00000ca0: 6564 4361 7365 2020 2875 6e63 6f6d 6d65  edCase  (uncomme
+00000cb0: 6e74 2069 6620 796f 7520 7761 6e74 2074  nt if you want t
+00000cc0: 6f20 616c 6c6f 7720 6d69 7865 6443 6173  o allow mixedCas
+00000cd0: 6520 7661 7269 6162 6c65 206e 616d 6573  e variable names
+00000ce0: 2069 6e20 676c 6f62 616c 2073 636f 7065   in global scope
+00000cf0: 290d 0a20 2020 2022 4e39 3939 222c 2020  )..    "N999",  
+00000d00: 2320 496e 7661 6c69 6420 6d6f 6475 6c65  # Invalid module
+00000d10: 206e 616d 650d 0a20 2020 205d 0d0a 7365   name..    ]..se
+00000d20: 6c65 6374 203d 205b 0d0a 2020 2020 2245  lect = [..    "E
+00000d30: 222c 0d0a 2020 2020 2244 222c 0d0a 2020  ",..    "D",..  
+00000d40: 2020 2246 222c 0d0a 2020 2020 224e 222c    "F",..    "N",
+00000d50: 0d0a 2020 2020 2257 222c 0d0a 2020 2020  ..    "W",..    
+00000d60: 2249 222c 0d0a 2020 2020 2242 222c 0d0a  "I",..    "B",..
+00000d70: 5d0d 0a0d 0a5b 746f 6f6c 2e72 7566 662e  ]....[tool.ruff.
+00000d80: 6c69 6e74 2e70 6570 382d 6e61 6d69 6e67  lint.pep8-naming
+00000d90: 5d0d 0a69 676e 6f72 652d 6e61 6d65 7320  ]..ignore-names 
+00000da0: 3d20 5b0d 0a20 2020 2022 7465 7374 5f2a  = [..    "test_*
+00000db0: 222c 0d0a 2020 2020 2273 6574 5570 222c  ",..    "setUp",
+00000dc0: 0d0a 2020 2020 2274 6561 7244 6f77 6e22  ..    "tearDown"
+00000dd0: 2c0d 0a5d 0d0a 0d0a 5b74 6f6f 6c2e 7275  ,..]....[tool.ru
+00000de0: 6666 2e6c 696e 742e 7079 646f 6373 7479  ff.lint.pydocsty
+00000df0: 6c65 5d0d 0a63 6f6e 7665 6e74 696f 6e20  le]..convention 
+00000e00: 3d20 226e 756d 7079 220d 0a0d 0a5b 746f  = "numpy"....[to
+00000e10: 6f6c 2e72 7566 662e 6c69 6e74 2e70 6572  ol.ruff.lint.per
+00000e20: 2d66 696c 652d 6967 6e6f 7265 735d 0d0a  -file-ignores]..
+00000e30: 225f 5f69 6e69 745f 5f2e 7079 2220 3d20  "__init__.py" = 
+00000e40: 5b22 4930 3031 225d 0d0a 222e 2f74 6573  ["I001"].."./tes
+00000e50: 7473 2f2a 2220 3d20 5b22 4422 5d0d 0a0d  ts/*" = ["D"]...
+00000e60: 0a5b 746f 6f6c 2e72 7566 662e 666f 726d  .[tool.ruff.form
+00000e70: 6174 5d0d 0a64 6f63 7374 7269 6e67 2d63  at]..docstring-c
+00000e80: 6f64 652d 666f 726d 6174 203d 2074 7275  ode-format = tru
+00000e90: 650d 0a0d 0a5b 746f 6f6c 2e70 7972 6967  e....[tool.pyrig
+00000ea0: 6874 5d0d 0a65 7863 6c75 6465 203d 205b  ht]..exclude = [
+00000eb0: 0d0a 2020 2020 222e 6769 7422 2c0d 0a20  ..    ".git",.. 
+00000ec0: 2020 2022 2e76 656e 7622 2c0d 0a20 2020     ".venv",..   
+00000ed0: 2022 2e74 6f78 222c 0d0a 2020 2020 2262   ".tox",..    "b
+00000ee0: 7569 6c64 222c 0d0a 2020 2020 2264 6973  uild",..    "dis
+00000ef0: 7422 2c0d 0a20 2020 2022 2a2a 2f5f 5f70  t",..    "**/__p
+00000f00: 7963 6163 6865 5f5f 222c 0d0a 2020 2020  ycache__",..    
+00000f10: 222e 2f64 6f63 732f 736f 7572 6365 2f63  "./docs/source/c
+00000f20: 6f6e 662e 7079 222c 0d0a 2020 2020 222e  onf.py",..    ".
+00000f30: 2f76 656e 7622 2c0d 0a5d 0d0a 6578 7472  /venv",..]..extr
+00000f40: 6150 6174 6873 203d 205b 222e 2f73 7263  aPaths = ["./src
+00000f50: 225d 0d0a 7479 7065 4368 6563 6b69 6e67  "]..typeChecking
+00000f60: 4d6f 6465 203d 2022 6261 7369 6322 0d0a  Mode = "basic"..
+00000f70: 7573 654c 6962 7261 7279 436f 6465 466f  useLibraryCodeFo
+00000f80: 7254 7970 6573 203d 2074 7275 650d 0a72  rTypes = true..r
+00000f90: 6570 6f72 744d 6973 7369 6e67 5061 7261  eportMissingPara
+00000fa0: 6d65 7465 7254 7970 6520 3d20 2265 7272  meterType = "err
+00000fb0: 6f72 220d 0a72 6570 6f72 7455 6e6b 6e6f  or"..reportUnkno
+00000fc0: 776e 5061 7261 6d65 7465 7254 7970 6520  wnParameterType 
+00000fd0: 3d20 2277 6172 6e69 6e67 220d 0a72 6570  = "warning"..rep
+00000fe0: 6f72 7455 6e6b 6e6f 776e 4d65 6d62 6572  ortUnknownMember
+00000ff0: 5479 7065 203d 2022 7761 726e 696e 6722  Type = "warning"
+00001000: 0d0a 7265 706f 7274 4d69 7373 696e 6754  ..reportMissingT
+00001010: 7970 6541 7267 756d 656e 7420 3d20 2265  ypeArgument = "e
+00001020: 7272 6f72 220d 0a72 6570 6f72 7450 726f  rror"..reportPro
+00001030: 7065 7274 7954 7970 654d 6973 6d61 7463  pertyTypeMismatc
+00001040: 6820 3d20 2265 7272 6f72 220d 0a72 6570  h = "error"..rep
+00001050: 6f72 7446 756e 6374 696f 6e4d 656d 6265  ortFunctionMembe
+00001060: 7241 6363 6573 7320 3d20 2277 6172 6e69  rAccess = "warni
+00001070: 6e67 220d 0a72 6570 6f72 7450 7269 7661  ng"..reportPriva
+00001080: 7465 5573 6167 6520 3d20 2277 6172 6e69  teUsage = "warni
+00001090: 6e67 220d 0a72 6570 6f72 7454 7970 6543  ng"..reportTypeC
+000010a0: 6f6d 6d65 6e74 5573 6167 6520 3d20 2277  ommentUsage = "w
+000010b0: 6172 6e69 6e67 220d 0a72 6570 6f72 7449  arning"..reportI
+000010c0: 6e63 6f6d 7061 7469 626c 654d 6574 686f  ncompatibleMetho
+000010d0: 644f 7665 7272 6964 6520 3d20 2277 6172  dOverride = "war
+000010e0: 6e69 6e67 220d 0a72 6570 6f72 7449 6e63  ning"..reportInc
+000010f0: 6f6d 7061 7469 626c 6556 6172 6961 626c  ompatibleVariabl
+00001100: 654f 7665 7272 6964 6520 3d20 2265 7272  eOverride = "err
+00001110: 6f72 220d 0a72 6570 6f72 7449 6e63 6f6e  or"..reportIncon
+00001120: 7369 7374 656e 7443 6f6e 7374 7275 6374  sistentConstruct
+00001130: 6f72 203d 2022 6572 726f 7222 0d0a 7265  or = "error"..re
+00001140: 706f 7274 4f76 6572 6c61 7070 696e 674f  portOverlappingO
+00001150: 7665 726c 6f61 6420 3d20 2277 6172 6e69  verload = "warni
+00001160: 6e67 220d 0a72 6570 6f72 7455 6e69 6e69  ng"..reportUnini
+00001170: 7469 616c 697a 6564 496e 7374 616e 6365  tializedInstance
+00001180: 5661 7269 6162 6c65 203d 2022 7761 726e  Variable = "warn
+00001190: 696e 6722 0d0a 7265 706f 7274 4361 6c6c  ing"..reportCall
+000011a0: 496e 4465 6661 756c 7449 6e69 7469 616c  InDefaultInitial
+000011b0: 697a 6572 203d 2022 7761 726e 696e 6722  izer = "warning"
+000011c0: 0d0a 7265 706f 7274 556e 6e65 6365 7373  ..reportUnnecess
+000011d0: 6172 7949 7349 6e73 7461 6e63 6520 3d20  aryIsInstance = 
+000011e0: 2269 6e66 6f72 6d61 7469 6f6e 220d 0a72  "information"..r
+000011f0: 6570 6f72 7455 6e6e 6563 6573 7361 7279  eportUnnecessary
+00001200: 4361 7374 203d 2022 7761 726e 696e 6722  Cast = "warning"
+00001210: 0d0a 7265 706f 7274 556e 6e65 6365 7373  ..reportUnnecess
+00001220: 6172 7943 6f6d 7061 7269 736f 6e20 3d20  aryComparison = 
+00001230: 2277 6172 6e69 6e67 220d 0a72 6570 6f72  "warning"..repor
+00001240: 7455 6e6e 6563 6573 7361 7279 436f 6e74  tUnnecessaryCont
+00001250: 6169 6e73 203d 2022 7761 726e 696e 6722  ains = "warning"
+00001260: 0d0a 7265 706f 7274 556e 7573 6564 4361  ..reportUnusedCa
+00001270: 6c6c 5265 7375 6c74 203d 2022 7761 726e  llResult = "warn
+00001280: 696e 6722 0d0a 7265 706f 7274 556e 7573  ing"..reportUnus
+00001290: 6564 4578 7072 6573 7369 6f6e 203d 2022  edExpression = "
+000012a0: 7761 726e 696e 6722 0d0a 7265 706f 7274  warning"..report
+000012b0: 4d61 7463 684e 6f74 4578 6861 7573 7469  MatchNotExhausti
+000012c0: 7665 203d 2022 7761 726e 696e 6722 0d0a  ve = "warning"..
+000012d0: 7265 706f 7274 5368 6164 6f77 6564 496d  reportShadowedIm
+000012e0: 706f 7274 7320 3d20 2277 6172 6e69 6e67  ports = "warning
+000012f0: 220d 0a72 6570 6f72 7455 6e74 7970 6564  "..reportUntyped
+00001300: 4675 6e63 7469 6f6e 4465 636f 7261 746f  FunctionDecorato
+00001310: 7220 3d20 2277 6172 6e69 6e67 220d 0a72  r = "warning"..r
+00001320: 6570 6f72 7455 6e74 7970 6564 4261 7365  eportUntypedBase
+00001330: 436c 6173 7320 3d20 2265 7272 6f72 220d  Class = "error".
+00001340: 0a72 6570 6f72 7455 6e74 7970 6564 4e61  .reportUntypedNa
+00001350: 6d65 6454 7570 6c65 203d 2022 7761 726e  medTuple = "warn
+00001360: 696e 6722 0d0a 2320 4163 7469 7661 7465  ing"..# Activate
+00001370: 2074 6865 2066 6f6c 6c6f 7769 6e67 2072   the following r
+00001380: 756c 6573 206f 6e6c 7920 6c6f 6361 6c6c  ules only locall
+00001390: 7920 616e 6420 7465 6d70 6f72 6172 792c  y and temporary,
+000013a0: 2069 2e65 2e20 666f 7220 6120 5141 2073   i.e. for a QA s
+000013b0: 6573 7369 6f6e 2e0d 0a23 2028 466f 7220  ession...# (For 
+000013c0: 7365 7276 6572 2073 6964 6520 4349 2074  server side CI t
+000013d0: 6865 7920 6172 6520 636f 6e73 6964 6572  hey are consider
+000013e0: 6564 2074 6f6f 2073 7472 6963 742e 290d  ed too strict.).
+000013f0: 0a23 2072 6570 6f72 7443 6f6e 7374 616e  .# reportConstan
+00001400: 7452 6564 6566 696e 6974 696f 6e20 3d20  tRedefinition = 
+00001410: 2277 6172 6e69 6e67 220d 0a23 2072 6570  "warning"..# rep
+00001420: 6f72 7455 6e6e 6563 6573 7361 7279 5479  ortUnnecessaryTy
+00001430: 7065 4967 6e6f 7265 436f 6d6d 656e 7420  peIgnoreComment 
+00001440: 3d20 2269 6e66 6f72 6d61 7469 6f6e 220d  = "information".
+00001450: 0a23 2072 6570 6f72 7449 6d70 6f72 7443  .# reportImportC
+00001460: 7963 6c65 7320 3d20 2277 6172 6e69 6e67  ycles = "warning
+00001470: 220d 0a23 2072 6570 6f72 7449 6d70 6c69  "..# reportImpli
+00001480: 6369 7453 7472 696e 6743 6f6e 6361 7465  citStringConcate
+00001490: 6e61 7469 6f6e 203d 2022 7761 726e 696e  nation = "warnin
+000014a0: 6722 0d0a                                g"..
```

### Comparing `dictIO-0.3.3/src/dictIO/__init__.py` & `dictio-0.3.4/src/dictIO/__init__.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/cli/dictParser.py` & `dictio-0.3.4/src/dictIO/cli/dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/cppDict.py` & `dictio-0.3.4/src/dictIO/cppDict.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/dictParser.py` & `dictio-0.3.4/src/dictIO/dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/dictReader.py` & `dictio-0.3.4/src/dictIO/dictReader.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/dictWriter.py` & `dictio-0.3.4/src/dictIO/dictWriter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/formatter.py` & `dictio-0.3.4/src/dictIO/formatter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/parser.py` & `dictio-0.3.4/src/dictIO/parser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/utils/counter.py` & `dictio-0.3.4/src/dictIO/utils/counter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/utils/logging.py` & `dictio-0.3.4/src/dictIO/utils/logging.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/utils/path.py` & `dictio-0.3.4/src/dictIO/utils/path.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO/utils/strings.py` & `dictio-0.3.4/src/dictIO/utils/strings.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/src/dictIO.egg-info/PKG-INFO` & `dictio-0.3.4/src/dictIO.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dictIO
-Version: 0.3.3
+Version: 0.3.4
 Summary: Python package to read, write and manipulate dictionary text files. Supports dictIOs dict file format, as well as JSON, XML and OpenFOAM.
 Author-email: Frank Lumpitzsch <frank.lumpitzsch@dnv.com>, Claas Rostock <claas.rostock@dnv.com>
 Maintainer-email: Claas Rostock <claas.rostock@dnv.com>
 License: MIT License
         
         Copyright (c) 2024 [DNV](https://www.dnv.com) [open source](https://github.com/dnv-opensource)
         
@@ -44,17 +44,17 @@
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: lxml>=5.1
+Requires-Dist: lxml>=5.2
 Requires-Dist: jsonschema>=4.20
-Requires-Dist: numpy>=1.26
+Requires-Dist: numpy<2.0,>=1.26
 
 # dictIO
 dictIO is a Python package to read, write and manipulate dictionary text files.
 
 It was designed to leverage the versatility of text based dictionary files, or 'dict files' in short, while easing their use in Python through seamless support for Python dicts.
 
 dictIO supports
@@ -168,32 +168,32 @@
 
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
 
 [https://github.com/dnv-opensource/dictIO](https://github.com/dnv-opensource/dictIO)
 
 ## Contributing
 
 1. Fork it (<https://github.com/dnv-opensource/dictIO/fork>)
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

### Comparing `dictIO-0.3.3/src/dictIO.egg-info/SOURCES.txt` & `dictio-0.3.4/src/dictIO.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/tests/test_dict.py` & `dictio-0.3.4/tests/test_dict.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/tests/test_dictParser.py` & `dictio-0.3.4/tests/test_dictParser.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/tests/test_dictReader.py` & `dictio-0.3.4/tests/test_dictReader.py`

 * *Files 0% similar despite different names*

```diff
@@ -477,22 +477,22 @@
     # Prepare
     source_file = "subfolder/test_subfolder_dict_fsl"
     parsed_file = Path("subfolder/parsed.test_subfolder_dict_fsl")
     parsed_file_foam = Path("subfolder/parsed.test_subfolder_dict_fsl.foam")
     parsed_file.unlink(missing_ok=True)
     parsed_file_foam.unlink(missing_ok=True)
     # Execute
-    _ = os.system(f"python -m dictIO.cli.dictParser --quiet {source_file}")
+    _ = os.system(f"dictParser --quiet {source_file}")
     # Assert
     assert parsed_file.exists()
     assert not parsed_file_foam.exists()
     # Clean up
     parsed_file.unlink()
     # Execute
-    _ = os.system(f"python -m dictIO.cli.dictParser --quiet --output=foam {source_file}")
+    _ = os.system(f"dictParser --quiet --output=foam {source_file}")
     # Assert
     assert not parsed_file.exists()
     assert parsed_file_foam.exists()
     # Clean up
     parsed_file_foam.unlink()
```

### Comparing `dictIO-0.3.3/tests/test_dictWriter.py` & `dictio-0.3.4/tests/test_dictWriter.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,17 +26,15 @@
             "_is_leaf": False,
             "_condition": None,
             "_names": ["param1", "param2", "param3"],
             "_values": [-10.0, 0.0, 0.0],
             "_commands": {"ls": ["echo %PATH%", "dir"]},
         },
     }
-    test_str: str = (
-        r"/*---------------------------------*- C++ -*----------------------------------*\ filetype dictionary; coding utf-8; version 0.1; local --; purpose --; \*----------------------------------------------------------------------------*/ param1 -10.0; param2 0.0; param3 0.0; _case { _layer lhsvar; _level 1; _no_of_samples 108; _index 0; _path 'C:\Users\CLAROS\Documents\SystemSimulation\ModelVerification\tools\farn\test\cases\gp_0\lhsvar_000'; _key lhsvar_000; _is_leaf false; _condition NULL; _names ( param1 param2 param3 ); _values ( -10.0 0.0 0.0 ); _commands { ls ( 'echo %PATH%' dir ); } } "
-    )
+    test_str: str = r"/*---------------------------------*- C++ -*----------------------------------*\ filetype dictionary; coding utf-8; version 0.1; local --; purpose --; \*----------------------------------------------------------------------------*/ param1 -10.0; param2 0.0; param3 0.0; _case { _layer lhsvar; _level 1; _no_of_samples 108; _index 0; _path 'C:\Users\CLAROS\Documents\SystemSimulation\ModelVerification\tools\farn\test\cases\gp_0\lhsvar_000'; _key lhsvar_000; _is_leaf false; _condition NULL; _names ( param1 param2 param3 ); _values ( -10.0 0.0 0.0 ); _commands { ls ( 'echo %PATH%' dir ); } } "
     test_cpp_dict: CppDict = CppDict()
     test_cpp_dict.update(test_dict)
 
     # Execute 1.1: Write as CppDict completely new
     target_file.unlink(missing_ok=True)
     DictWriter.write(test_cpp_dict, target_file, mode="w")
     # Assert 1.1
```

### Comparing `dictIO-0.3.3/tests/test_formatter.py` & `dictio-0.3.4/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `dictIO-0.3.3/tests/test_parser.py` & `dictio-0.3.4/tests/test_parser.py`

 * *Files identical despite different names*

