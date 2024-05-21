# Comparing `tmp/module_sdstate-0.1.3.tar.gz` & `tmp/module_sdstate-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "module_sdstate-0.1.3.tar", max compression
+gzip compressed data, was "module_sdstate-0.1.4.tar", max compression
```

## Comparing `module_sdstate-0.1.3.tar` & `module_sdstate-0.1.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.3/LICENSE
--rw-r--r--   0        0        0      680 2024-05-21 21:30:05.142896 module_sdstate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.3/README.md
--rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.3/src/module_sdstate/__init__.py
--rw-r--r--   0        0        0     6603 2024-05-06 20:37:26.351098 module_sdstate-0.1.3/src/module_sdstate/lanczos_utils.py
--rw-r--r--   0        0        0    10302 2024-05-21 21:27:44.095415 module_sdstate-0.1.3/src/module_sdstate/sdstate_utils.py
--rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1092 2024-02-23 19:52:24.045015 module_sdstate-0.1.4/LICENSE
+-rw-r--r--   0        0        0      680 2024-05-21 21:40:01.533381 module_sdstate-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1162 2024-02-26 20:26:54.627700 module_sdstate-0.1.4/README.md
+-rw-r--r--   0        0        0      118 2024-02-26 20:20:38.191958 module_sdstate-0.1.4/src/module_sdstate/__init__.py
+-rw-r--r--   0        0        0     6603 2024-05-06 20:37:26.351098 module_sdstate-0.1.4/src/module_sdstate/lanczos_utils.py
+-rw-r--r--   0        0        0    10301 2024-05-21 21:39:41.787603 module_sdstate-0.1.4/src/module_sdstate/sdstate_utils.py
+-rw-r--r--   0        0        0     2010 1970-01-01 00:00:00.000000 module_sdstate-0.1.4/PKG-INFO
```

### Comparing `module_sdstate-0.1.3/LICENSE` & `module_sdstate-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.3/pyproject.toml` & `module_sdstate-0.1.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "module_sdstate"
-version = "0.1.3"
+version = "0.1.4"
 description = "Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range."
 authors = ["Linjun Wang"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `module_sdstate-0.1.3/README.md` & `module_sdstate-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.3/src/module_sdstate/lanczos_utils.py` & `module_sdstate-0.1.4/src/module_sdstate/lanczos_utils.py`

 * *Files identical despite different names*

### Comparing `module_sdstate-0.1.3/src/module_sdstate/sdstate_utils.py` & `module_sdstate-0.1.4/src/module_sdstate/sdstate_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -193,15 +193,15 @@
     def process_batch(self,batch):
         partial_state = sdstate(n_qubit=self.n_qubit)
         for t, coeff in batch:
             if coeff != 0:
                 partial_state += self.op_state(t, coeff)
         return partial_state
     
-    def Hf_state(self, Hf: of.FermionOperator, multiprocessing = False):
+    def Hf_state(self, H: of.FermionOperator, multiprocessing = False):
         """Apply a Hamiltonian in FermionOperator on the current state. multiprocessing can be used
         to parallelize the process of applying each Excitation operator in the Hamiltonian. The general
         cost is given by O(N^4M), for N as the qubit dimension and M as the size of the current state.
         """
         re_state = sdstate(n_qubit = self.n_qubit)
         if multiprocessing:
             # Convert FermionOperator terms to a list of tuples for easy batch processing
```

### Comparing `module_sdstate-0.1.3/PKG-INFO` & `module_sdstate-0.1.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module_sdstate
-Version: 0.1.3
+Version: 0.1.4
 Summary: Implementation of Slater Determinant states as dictionaries of states and coefficient pairs. Each state is represented with an integar treated as binary, allowing applying of Excitation operators on the state efficiently. Memory-efficient implementation of Lanczos iteration for estimating Hamiltonian spectrum range.
 License: MIT
 Author: Linjun Wang
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

