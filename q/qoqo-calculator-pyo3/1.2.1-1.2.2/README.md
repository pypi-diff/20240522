# Comparing `tmp/qoqo_calculator_pyo3-1.2.1.tar.gz` & `tmp/qoqo_calculator_pyo3-1.2.2.tar.gz`

## Comparing `qoqo_calculator_pyo3-1.2.1.tar` & `qoqo_calculator_pyo3-1.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0     1001      127      812 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/Cargo.toml
--rw-r--r--   0     1001      127    11358 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/LICENSE
--rw-r--r--   0     1001      127     1555 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/README.md
--rw-r--r--   0     1001      127    52301 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator.rs
--rw-r--r--   0     1001      127    26250 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator_complex.rs
--rw-r--r--   0     1001      127    65682 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator_float.rs
--rw-r--r--   0     1001      127     7219 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/lib.rs
--rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/Cargo.toml
--rw-r--r--   0     1001      127    11358 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/LICENSE
--rw-r--r--   0     1001      127     3171 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/README.md
--rw-r--r--   0     1001      127     1468 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/BSD_LICENSE
--rw-r--r--   0     1001      127   544169 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/DEPENDENCIES
--rw-r--r--   0     1001      127    11881 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      127     1064 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/MIT_LICENSE
--rw-r--r--   0     1001      127        0 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/NOTICE
--rw-r--r--   0     1001      127     2404 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/PYTHON_LICENSE
--rw-r--r--   0     1001      127      762 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/__init__.py
--rw-r--r--   0     1001      127     3432 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator.rs
--rw-r--r--   0     1001      127    21313 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator_complex.rs
--rw-r--r--   0     1001      127    21506 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator_float.rs
--rw-r--r--   0     1001      127     2124 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/lib.rs
--rw-r--r--   0     1001      127    11634 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/Cargo.lock
--rw-r--r--   0        0        0      153 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.1/Cargo.toml
--rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.1/pyproject.toml
--rw-r--r--   0     1001      127     1064 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/MIT_LICENSE
--rw-r--r--   0     1001      127      762 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/__init__.py
--rw-r--r--   0     1001      127    11881 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION
--rw-r--r--   0     1001      127     2404 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/PYTHON_LICENSE
--rw-r--r--   0     1001      127     1468 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/BSD_LICENSE
--rw-r--r--   0     1001      127        0 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/NOTICE
--rw-r--r--   0     1001      127   544169 2024-05-03 07:55:56.000000 qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/DEPENDENCIES
--rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.1/PKG-INFO
+-rw-r--r--   0     1001      127      812 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/Cargo.toml
+-rw-r--r--   0     1001      127    11358 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/LICENSE
+-rw-r--r--   0     1001      127     1555 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/README.md
+-rw-r--r--   0     1001      127    52301 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator.rs
+-rw-r--r--   0     1001      127    26250 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator_complex.rs
+-rw-r--r--   0     1001      127    65682 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator_float.rs
+-rw-r--r--   0     1001      127     7219 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/lib.rs
+-rw-r--r--   0        0        0      938 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/Cargo.toml
+-rw-r--r--   0     1001      127    11358 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/LICENSE
+-rw-r--r--   0     1001      127     3171 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/README.md
+-rw-r--r--   0     1001      127     1468 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/BSD_LICENSE
+-rw-r--r--   0     1001      127   544169 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/DEPENDENCIES
+-rw-r--r--   0     1001      127    11881 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      127     1064 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/MIT_LICENSE
+-rw-r--r--   0     1001      127        0 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/NOTICE
+-rw-r--r--   0     1001      127     2404 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/PYTHON_LICENSE
+-rw-r--r--   0     1001      127      762 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/__init__.py
+-rw-r--r--   0     1001      127     3432 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator.rs
+-rw-r--r--   0     1001      127    21191 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator_complex.rs
+-rw-r--r--   0     1001      127    21386 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator_float.rs
+-rw-r--r--   0     1001      127     2124 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/lib.rs
+-rw-r--r--   0     1001      127    11634 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/Cargo.lock
+-rw-r--r--   0        0        0      153 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.2/Cargo.toml
+-rw-r--r--   0        0        0      721 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.2/pyproject.toml
+-rw-r--r--   0     1001      127     1064 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/MIT_LICENSE
+-rw-r--r--   0     1001      127      762 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/__init__.py
+-rw-r--r--   0     1001      127    11881 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION
+-rw-r--r--   0     1001      127     2404 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/PYTHON_LICENSE
+-rw-r--r--   0     1001      127     1468 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/BSD_LICENSE
+-rw-r--r--   0     1001      127        0 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/NOTICE
+-rw-r--r--   0     1001      127   544169 2024-05-07 06:58:10.000000 qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/DEPENDENCIES
+-rw-r--r--   0        0        0     4230 1970-01-01 00:00:00.000000 qoqo_calculator_pyo3-1.2.2/PKG-INFO
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/Cargo.toml` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo_calculator"
-version = "1.2.1"
+version = "1.2.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 categories = ["science", "simulation"]
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_calculator"
 description = "qoqo-calculator is the calculator backend of the qoqo quantum computing toolkit by HQS Quantum Simulations"
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/README.md` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator_complex.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator_complex.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/calculator_float.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/calculator_float.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator/src/lib.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/Cargo.toml` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "qoqo_calculator_pyo3"
-version = "1.2.1"
+version = "1.2.2"
 authors = ["HQS Quantum Simulations <info@quantumsimulations.de>"]
 license = "Apache-2.0"
 edition = "2021"
 readme = "README.md"
 repository = "https://github.com/HQSquantumsimulations/qoqo_calculator_pyo3"
 description = "Python interface to qoqo calculator, the calculator backend of the qoqo quantum computing toolkit by HQS Quantum Simulations"
 include = [
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/README.md` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/README.md`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/BSD_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/BSD_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/DEPENDENCIES` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000030: 3d3d 3d3d 0a61 7574 6f63 6667 2031 2e32  ====.autocfg 1.2
+00000030: 3d3d 3d3d 0a61 7574 6f63 6667 2031 2e33  ====.autocfg 1.3
 00000040: 2e30 0a68 7474 7073 3a2f 2f67 6974 6875  .0.https://githu
 00000050: 622e 636f 6d2f 6375 7669 7065 722f 6175  b.com/cuviper/au
 00000060: 746f 6366 670a 6279 204a 6f73 6820 5374  tocfg.by Josh St
 00000070: 6f6e 6520 3c63 7576 6970 6572 4067 6d61  one <cuviper@gma
 00000080: 696c 2e63 6f6d 3e0a 4175 746f 6d61 7469  il.com>.Automati
 00000090: 6320 6366 6720 666f 7220 5275 7374 2063  c cfg for Rust c
 000000a0: 6f6d 7069 6c65 7220 6665 6174 7572 6573  ompiler features
@@ -6773,15 +6773,15 @@
 0001a740: 7369 6f6e 7320 616e 640a 6c69 6d69 7461  sions and.limita
 0001a750: 7469 6f6e 7320 756e 6465 7220 7468 6520  tions under the 
 0001a760: 4c69 6365 6e73 652e 0a0a 0a3d 3d3d 3d3d  License....=====
 0001a770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001a780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001a790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
 0001a7a0: 6e75 6d2d 7472 6169 7473 2030 2e32 2e31  num-traits 0.2.1
-0001a7b0: 380a 6874 7470 733a 2f2f 6769 7468 7562  8.https://github
+0001a7b0: 390a 6874 7470 733a 2f2f 6769 7468 7562  9.https://github
 0001a7c0: 2e63 6f6d 2f72 7573 742d 6e75 6d2f 6e75  .com/rust-num/nu
 0001a7d0: 6d2d 7472 6169 7473 0a62 7920 5468 6520  m-traits.by The 
 0001a7e0: 5275 7374 2050 726f 6a65 6374 2044 6576  Rust Project Dev
 0001a7f0: 656c 6f70 6572 730a 4e75 6d65 7269 6320  elopers.Numeric 
 0001a800: 7472 6169 7473 2066 6f72 2067 656e 6572  traits for gener
 0001a810: 6963 206d 6174 6865 6d61 7469 6373 0a4c  ic mathematics.L
 0001a820: 6963 656e 7365 3a20 4d49 5420 4f52 2041  icense: MIT OR A
@@ -15097,15 +15097,15 @@
 0003af80: 6368 2077 6172 7261 6e74 7920 6f72 2061  ch warranty or a
 0003af90: 6464 6974 696f 6e61 6c20 6c69 6162 696c  dditional liabil
 0003afa0: 6974 792e 0a0a 0a3d 3d3d 3d3d 3d3d 3d3d  ity....=========
 0003afb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003afc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003afd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 716f 716f  ===========.qoqo
 0003afe0: 5f63 616c 6375 6c61 746f 7220 312e 322e  _calculator 1.2.
-0003aff0: 310a 6874 7470 733a 2f2f 6769 7468 7562  1.https://github
+0003aff0: 320a 6874 7470 733a 2f2f 6769 7468 7562  2.https://github
 0003b000: 2e63 6f6d 2f48 5153 7175 616e 7475 6d73  .com/HQSquantums
 0003b010: 696d 756c 6174 696f 6e73 2f71 6f71 6f5f  imulations/qoqo_
 0003b020: 6361 6c63 756c 6174 6f72 0a62 7920 4851  calculator.by HQ
 0003b030: 5320 5175 616e 7475 6d20 5369 6d75 6c61  S Quantum Simula
 0003b040: 7469 6f6e 7320 3c69 6e66 6f40 7175 616e  tions <info@quan
 0003b050: 7475 6d73 696d 756c 6174 696f 6e73 2e64  tumsimulations.d
 0003b060: 653e 0a71 6f71 6f2d 6361 6c63 756c 6174  e>.qoqo-calculat
@@ -15830,15 +15830,15 @@
 0003dd50: 6d69 7373 696f 6e73 2061 6e64 0a20 2020  missions and.   
 0003dd60: 6c69 6d69 7461 7469 6f6e 7320 756e 6465  limitations unde
 0003dd70: 7220 7468 6520 4c69 6365 6e73 652e 0a0a  r the License...
 0003dd80: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
 0003dd90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003dda0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003ddb0: 3d3d 3d3d 3d0a 716f 716f 5f63 616c 6375  =====.qoqo_calcu
-0003ddc0: 6c61 746f 725f 7079 6f33 2031 2e32 2e31  lator_pyo3 1.2.1
+0003ddc0: 6c61 746f 725f 7079 6f33 2031 2e32 2e32  lator_pyo3 1.2.2
 0003ddd0: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
 0003dde0: 636f 6d2f 4851 5371 7561 6e74 756d 7369  com/HQSquantumsi
 0003ddf0: 6d75 6c61 7469 6f6e 732f 716f 716f 5f63  mulations/qoqo_c
 0003de00: 616c 6375 6c61 746f 725f 7079 6f33 0a62  alculator_pyo3.b
 0003de10: 7920 4851 5320 5175 616e 7475 6d20 5369  y HQS Quantum Si
 0003de20: 6d75 6c61 7469 6f6e 7320 3c69 6e66 6f40  mulations <info@
 0003de30: 7175 616e 7475 6d73 696d 756c 6174 696f  quantumsimulatio
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/MIT_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/MIT_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/PYTHON_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/qoqo_calculator_pyo3/__init__.py` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/qoqo_calculator_pyo3/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator_complex.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator_complex.rs`

 * *Files 0% similar despite different names*

```diff
@@ -572,16 +572,13 @@
         Ok(CalculatorComplexWrapper {
             internal: self.internal.recip(),
         })
     }
 }
 
 impl CalculatorComplexWrapper {
-    pub fn from_pyany(input: Py<PyAny>) -> PyResult<CalculatorComplex> {
-        Python::with_gil(|py| -> PyResult<CalculatorComplex> {
-            let input = input.bind(py);
-            convert_into_calculator_complex(input).map_err(|err| {
-                PyValueError::new_err(format!("Error in convert_to_calculator_complex: {err:?}"))
-            })
+    pub fn from_pyany(input: &Bound<PyAny>) -> PyResult<CalculatorComplex> {
+        convert_into_calculator_complex(input).map_err(|err| {
+            PyValueError::new_err(format!("Error in convert_to_calculator_complex: {err:?}"))
         })
     }
 }
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/calculator_float.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/calculator_float.rs`

 * *Files 0% similar despite different names*

```diff
@@ -588,16 +588,13 @@
                 "Symbolic Value can not be cast to float.",
             )),
         }
     }
 }
 
 impl CalculatorFloatWrapper {
-    pub fn from_pyany(input: Py<PyAny>) -> PyResult<CalculatorFloat> {
-        Python::with_gil(|py| -> PyResult<CalculatorFloat> {
-            let input = input.bind(py);
-            convert_into_calculator_float(input).map_err(|err| {
-                PyValueError::new_err(format!("Error in convert_to_calculator_float: {err:?}"))
-            })
+    pub fn from_pyany(input: &Bound<PyAny>) -> PyResult<CalculatorFloat> {
+        convert_into_calculator_float(input).map_err(|err| {
+            PyValueError::new_err(format!("Error in convert_to_calculator_float: {err:?}"))
         })
     }
 }
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/src/lib.rs` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/Cargo.lock` & `qoqo_calculator_pyo3-1.2.2/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "autocfg"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
+checksum = "0c4b4d0bd25bd0b74681c0ad21497610ce1b7c91b1022cd21c80c6fbdd9476b0"
 
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
@@ -77,17 +77,17 @@
 dependencies = [
  "num-traits",
  "serde",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.18"
+version = "0.2.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
+checksum = "071dfc062690e90b734c0b2273ce72ad0ffa95f0c74596bc250dcfd960262841"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
 version = "1.19.0"
@@ -194,27 +194,27 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "qoqo_calculator"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
  "num-complex",
  "schemars",
  "serde",
  "serde_json",
  "serde_test",
  "thiserror",
 ]
 
 [[package]]
 name = "qoqo_calculator_pyo3"
-version = "1.2.1"
+version = "1.2.2"
 dependencies = [
  "num-complex",
  "pyo3",
  "pyo3-build-config",
  "qoqo_calculator",
  "serde",
  "thiserror",
```

### Comparing `qoqo_calculator_pyo3-1.2.1/pyproject.toml` & `qoqo_calculator_pyo3-1.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "qoqo_calculator_pyo3"
-version = "1.2.1"
+version = "1.2.2"
 license = { text = "Apache-2.0 AND Apache-2.0 with LLVM-exception AND MIT AND Unicode-DFS-2016" }
 maintainers = [
     { name = "HQS Quantum Simulations GmbH", email = "info@quantumsimulations.de" },
 ]
 requires-python = ">=3.8"
 
 [build-system]
```

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/MIT_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/MIT_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/__init__.py` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/__init__.py`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/LICENSE_FOR_BINARY_DISTRIBUTION`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/PYTHON_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/PYTHON_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/BSD_LICENSE` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/BSD_LICENSE`

 * *Files identical despite different names*

### Comparing `qoqo_calculator_pyo3-1.2.1/qoqo_calculator_pyo3/DEPENDENCIES` & `qoqo_calculator_pyo3-1.2.2/qoqo_calculator_pyo3/DEPENDENCIES`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000010: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 00000020: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
-00000030: 3d3d 3d3d 0a61 7574 6f63 6667 2031 2e32  ====.autocfg 1.2
+00000030: 3d3d 3d3d 0a61 7574 6f63 6667 2031 2e33  ====.autocfg 1.3
 00000040: 2e30 0a68 7474 7073 3a2f 2f67 6974 6875  .0.https://githu
 00000050: 622e 636f 6d2f 6375 7669 7065 722f 6175  b.com/cuviper/au
 00000060: 746f 6366 670a 6279 204a 6f73 6820 5374  tocfg.by Josh St
 00000070: 6f6e 6520 3c63 7576 6970 6572 4067 6d61  one <cuviper@gma
 00000080: 696c 2e63 6f6d 3e0a 4175 746f 6d61 7469  il.com>.Automati
 00000090: 6320 6366 6720 666f 7220 5275 7374 2063  c cfg for Rust c
 000000a0: 6f6d 7069 6c65 7220 6665 6174 7572 6573  ompiler features
@@ -6773,15 +6773,15 @@
 0001a740: 7369 6f6e 7320 616e 640a 6c69 6d69 7461  sions and.limita
 0001a750: 7469 6f6e 7320 756e 6465 7220 7468 6520  tions under the 
 0001a760: 4c69 6365 6e73 652e 0a0a 0a3d 3d3d 3d3d  License....=====
 0001a770: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001a780: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0001a790: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a  ===============.
 0001a7a0: 6e75 6d2d 7472 6169 7473 2030 2e32 2e31  num-traits 0.2.1
-0001a7b0: 380a 6874 7470 733a 2f2f 6769 7468 7562  8.https://github
+0001a7b0: 390a 6874 7470 733a 2f2f 6769 7468 7562  9.https://github
 0001a7c0: 2e63 6f6d 2f72 7573 742d 6e75 6d2f 6e75  .com/rust-num/nu
 0001a7d0: 6d2d 7472 6169 7473 0a62 7920 5468 6520  m-traits.by The 
 0001a7e0: 5275 7374 2050 726f 6a65 6374 2044 6576  Rust Project Dev
 0001a7f0: 656c 6f70 6572 730a 4e75 6d65 7269 6320  elopers.Numeric 
 0001a800: 7472 6169 7473 2066 6f72 2067 656e 6572  traits for gener
 0001a810: 6963 206d 6174 6865 6d61 7469 6373 0a4c  ic mathematics.L
 0001a820: 6963 656e 7365 3a20 4d49 5420 4f52 2041  icense: MIT OR A
@@ -15097,15 +15097,15 @@
 0003af80: 6368 2077 6172 7261 6e74 7920 6f72 2061  ch warranty or a
 0003af90: 6464 6974 696f 6e61 6c20 6c69 6162 696c  dditional liabil
 0003afa0: 6974 792e 0a0a 0a3d 3d3d 3d3d 3d3d 3d3d  ity....=========
 0003afb0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003afc0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003afd0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d0a 716f 716f  ===========.qoqo
 0003afe0: 5f63 616c 6375 6c61 746f 7220 312e 322e  _calculator 1.2.
-0003aff0: 310a 6874 7470 733a 2f2f 6769 7468 7562  1.https://github
+0003aff0: 320a 6874 7470 733a 2f2f 6769 7468 7562  2.https://github
 0003b000: 2e63 6f6d 2f48 5153 7175 616e 7475 6d73  .com/HQSquantums
 0003b010: 696d 756c 6174 696f 6e73 2f71 6f71 6f5f  imulations/qoqo_
 0003b020: 6361 6c63 756c 6174 6f72 0a62 7920 4851  calculator.by HQ
 0003b030: 5320 5175 616e 7475 6d20 5369 6d75 6c61  S Quantum Simula
 0003b040: 7469 6f6e 7320 3c69 6e66 6f40 7175 616e  tions <info@quan
 0003b050: 7475 6d73 696d 756c 6174 696f 6e73 2e64  tumsimulations.d
 0003b060: 653e 0a71 6f71 6f2d 6361 6c63 756c 6174  e>.qoqo-calculat
@@ -15830,15 +15830,15 @@
 0003dd50: 6d69 7373 696f 6e73 2061 6e64 0a20 2020  missions and.   
 0003dd60: 6c69 6d69 7461 7469 6f6e 7320 756e 6465  limitations unde
 0003dd70: 7220 7468 6520 4c69 6365 6e73 652e 0a0a  r the License...
 0003dd80: 0a3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  .===============
 0003dd90: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003dda0: 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d 3d3d  ================
 0003ddb0: 3d3d 3d3d 3d0a 716f 716f 5f63 616c 6375  =====.qoqo_calcu
-0003ddc0: 6c61 746f 725f 7079 6f33 2031 2e32 2e31  lator_pyo3 1.2.1
+0003ddc0: 6c61 746f 725f 7079 6f33 2031 2e32 2e32  lator_pyo3 1.2.2
 0003ddd0: 0a68 7474 7073 3a2f 2f67 6974 6875 622e  .https://github.
 0003dde0: 636f 6d2f 4851 5371 7561 6e74 756d 7369  com/HQSquantumsi
 0003ddf0: 6d75 6c61 7469 6f6e 732f 716f 716f 5f63  mulations/qoqo_c
 0003de00: 616c 6375 6c61 746f 725f 7079 6f33 0a62  alculator_pyo3.b
 0003de10: 7920 4851 5320 5175 616e 7475 6d20 5369  y HQS Quantum Si
 0003de20: 6d75 6c61 7469 6f6e 7320 3c69 6e66 6f40  mulations <info@
 0003de30: 7175 616e 7475 6d73 696d 756c 6174 696f  quantumsimulatio
```

### Comparing `qoqo_calculator_pyo3-1.2.1/PKG-INFO` & `qoqo_calculator_pyo3-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: qoqo_calculator_pyo3
-Version: 1.2.1
+Version: 1.2.2
 Requires-Dist: sphinx >=2.1 ; extra == 'docs'
 Requires-Dist: nbsphinx ; extra == 'docs'
 Requires-Dist: pygments ; extra == 'docs'
 Requires-Dist: recommonmark ; extra == 'docs'
 Requires-Dist: myst-parser ; extra == 'docs'
 Requires-Dist: sphinx-rtd-theme ; extra == 'docs'
 Requires-Dist: tomli ; extra == 'docs'
```

