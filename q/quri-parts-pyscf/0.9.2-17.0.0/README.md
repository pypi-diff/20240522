# Comparing `tmp/quri_parts_pyscf-0.9.2.tar.gz` & `tmp/quri_parts_pyscf-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_pyscf-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_pyscf-17.0.0.tar", max compression
```

## Comparing `quri_parts_pyscf-0.9.2.tar` & `quri_parts_pyscf-17.0.0.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/LICENSE
--rw-r--r--   0        0        0      256 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/README.md
--rw-r--r--   0        0        0     1240 2023-03-29 07:37:32.887017 quri_parts_pyscf-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:32.059012 quri_parts_pyscf-0.9.2/quri_parts/pyscf/NOTICE
--rw-r--r--   0        0        0      541 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/quri_parts/pyscf/__init__.py
--rw-r--r--   0        0        0      677 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/quri_parts/pyscf/mol/__init__.py
--rw-r--r--   0        0        0     1913 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/quri_parts/pyscf/mol/pyscf_interface.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_pyscf-0.9.2/quri_parts/pyscf/py.typed
--rw-r--r--   0        0        0     1206 1970-01-01 00:00:00.000000 quri_parts_pyscf-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/LICENSE
+-rw-r--r--   0        0        0      256 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/README.md
+-rw-r--r--   0        0        0     1241 2024-03-19 02:11:30.993999 quri_parts_pyscf-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:30.394002 quri_parts_pyscf-17.0.0/quri_parts/pyscf/NOTICE
+-rw-r--r--   0        0        0      541 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/quri_parts/pyscf/__init__.py
+-rw-r--r--   0        0        0     1466 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/quri_parts/pyscf/mol/__init__.py
+-rw-r--r--   0        0        0     2189 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/quri_parts/pyscf/mol/model.py
+-rw-r--r--   0        0        0    11090 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/quri_parts/pyscf/mol/non_relativistic.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_pyscf-17.0.0/quri_parts/pyscf/py.typed
+-rw-r--r--   0        0        0     1207 1970-01-01 00:00:00.000000 quri_parts_pyscf-17.0.0/PKG-INFO
```

### Comparing `quri_parts_pyscf-0.9.2/LICENSE` & `quri_parts_pyscf-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_pyscf-0.9.2/pyproject.toml` & `quri_parts_pyscf-17.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-pyscf"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use PySCF with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
@@ -24,15 +24,15 @@
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = "^3.9.8"
 typing-extensions = "^4.1.1"
 numpy = ">=1.22.0"
-pyscf = "^2.1.1"
+pyscf = "^2.3.0"
 quri-parts-core = "*"
 quri-parts-chem = "*"
 
 [tool.poetry.group.dev.dependencies]
 quri-parts-circuit = {path = "../circuit", develop = true}
 quri-parts-core = {path = "../core", develop = true}
 quri-parts-chem = {path = "../chem", develop = true}
```

### Comparing `quri_parts_pyscf-0.9.2/quri_parts/pyscf/__init__.py` & `quri_parts_pyscf-17.0.0/quri_parts/pyscf/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_pyscf-0.9.2/quri_parts/pyscf/mol/pyscf_interface.py` & `quri_parts_pyscf-17.0.0/quri_parts/pyscf/mol/model.py`

 * *Files 18% similar despite different names*

```diff
@@ -35,25 +35,34 @@
 
     @property
     def mol(self) -> Mole:
         """Returns :class:`Mole` the PySCF Mole object of the molecule."""
         return self._mol
 
     @property
+    def spin(self) -> int:
+        """Returns the total spin of the electrons."""
+        return int(self._mol.spin)
+
+    @property
     def n_electron(self) -> int:
         """Returns a number of electrons."""
         return cast(int, self._mol.nelectron)
 
     @property
+    def n_spatial_orb(self) -> int:
+        """Returns the number of spatial orbitals."""
+        return cast(int, self._mol.nao)
+
+    @property
     def mo_coeff(self) -> "npt.NDArray[np.complex128]":
         """Returns molecular orbital coefficients."""
         return self._mo_coeff
 
 
 def get_nuc_energy(mo: PySCFMolecularOrbitals) -> float:
     """Returns a nuclear repulsion energy of a given molecule.
 
     Args:
         mo: :class:`PySCFMolecularOrbitals` of the molecule.
     """
-
     return cast(float, mo.mol.energy_nuc())
```

### Comparing `quri_parts_pyscf-0.9.2/PKG-INFO` & `quri_parts_pyscf-17.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: quri-parts-pyscf
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use PySCF with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Dist: numpy (>=1.22.0)
-Requires-Dist: pyscf (>=2.1.1,<3.0.0)
+Requires-Dist: pyscf (>=2.3.0,<3.0.0)
 Requires-Dist: quri-parts-chem
 Requires-Dist: quri-parts-core
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Documentation, https://quri-parts.qunasys.com
 Project-URL: Repository, https://github.com/QunaSys/quri-parts
 Description-Content-Type: text/markdown
```

