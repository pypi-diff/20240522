# Comparing `tmp/quri_parts-0.9.2.tar.gz` & `tmp/quri_parts-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts-17.0.0.tar", max compression
```

## Comparing `quri_parts-0.9.2.tar` & `quri_parts-17.0.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.850951 quri_parts-0.9.2/LICENSE
--rw-r--r--   0        0        0     4539 2023-03-29 07:37:19.850951 quri_parts-0.9.2/README.md
--rw-r--r--   0        0        0     3144 2023-03-29 07:37:21.486956 quri_parts-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:19.930951 quri_parts-0.9.2/quri_parts/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.882951 quri_parts-0.9.2/quri_parts/_quri_parts_meta.py
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 quri_parts-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.274138 quri_parts-17.0.0/LICENSE
+-rw-r--r--   0        0        0     4795 2024-03-19 02:11:01.274138 quri_parts-17.0.0/README.md
+-rw-r--r--   0        0        0     3712 2024-03-19 02:11:23.134040 quri_parts-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:22.274045 quri_parts-17.0.0/quri_parts/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.310138 quri_parts-17.0.0/quri_parts/_quri_parts_meta.py
+-rw-r--r--   0        0        0     6614 1970-01-01 00:00:00.000000 quri_parts-17.0.0/PKG-INFO
```

### Comparing `quri_parts-0.9.2/LICENSE` & `quri_parts-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts-0.9.2/README.md` & `quri_parts-17.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,29 @@
   - `quri-parts-core`: General components
       - Operator, state, estimator, sampler etc.
 - Platform (device/simulator) support
   - Quantum circuit simulators
       - `quri-parts-qulacs`: [Qulacs](https://github.com/qulacs/qulacs)
       - `quri-parts-stim`: [Stim](https://github.com/quantumlib/Stim)
       - `quri-parts-itensor`: [ITensor](https://github.com/ITensor/ITensors.jl)
+      - `quri-parts-tket`: [TKet](https://www.quantinuum.com/developers/tket)
   - Quantum platforms/SDKs
       - `quri-parts-braket`: [Amazon Braket SDK](https://github.com/aws/amazon-braket-sdk-python)
-      - `quri-parts-cirq`: [Cirq](https://quantumai.google/cirq) (Only circuit conversion is supported yet)
-      - `quri-parts-qiskit`: [Qiskit](https://qiskit.org/) (Circuit conversion and execution are not supported yet)
+      - `quri-parts-cirq`: [Cirq](https://quantumai.google/cirq) (Only circuit and operator conversion is supported yet)
+      - `quri-parts-qiskit`: [Qiskit](https://qiskit.org/)
+      - `quri-parts-quantinuum`: [Quantinuum](https://www.quantinuum.com/hardware/)
+      - `quri-parts-ionq`: [IONQ](https://ionq.com/docs/)
 - Intermediate representation support
   - `quri-parts-openqasm`: [OpenQASM 3.0](https://openqasm.com/)
 - `quri-parts-algo`: Algorithms
   - Ansatz, optimizer, error mitigation etc.
 - Chemistry
   - `quri-parts-chem`: General concepts
-      - Fermion-qubit mapping etc.
+      - Fermion-qubit mapping, electron integrals, ansatz etc.
+  - `quri-parts-pyscf`: [PySCF](https://pyscf.org/)
   - Library support
       - `quri-parts-openfermion`: [OpenFermion](https://quantumai.google/openfermion)
 
 
 ## Installation
 
 QURI Parts requires Python 3.9.8 or later.
```

### Comparing `quri_parts-0.9.2/PKG-INFO` & `quri_parts-17.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts
-Version: 0.9.2
+Version: 17.0.0
 Summary: Platform-independent quantum computing library
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
@@ -12,38 +12,40 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Provides-Extra: braket
 Provides-Extra: cirq
-Provides-Extra: honeywell
 Provides-Extra: ionq
 Provides-Extra: itensor
 Provides-Extra: openfermion
 Provides-Extra: openqasm
 Provides-Extra: pyscf
 Provides-Extra: qiskit
+Provides-Extra: quantinuum
 Provides-Extra: qulacs
 Provides-Extra: stim
+Provides-Extra: tket
 Requires-Dist: quri-parts-algo
 Requires-Dist: quri-parts-braket ; extra == "braket"
 Requires-Dist: quri-parts-chem
 Requires-Dist: quri-parts-circuit
 Requires-Dist: quri-parts-cirq ; extra == "cirq"
 Requires-Dist: quri-parts-core
-Requires-Dist: quri-parts-honeywell ; extra == "honeywell"
 Requires-Dist: quri-parts-ionq ; extra == "ionq"
 Requires-Dist: quri-parts-itensor ; extra == "itensor"
 Requires-Dist: quri-parts-openfermion ; extra == "openfermion"
 Requires-Dist: quri-parts-openqasm ; extra == "openqasm"
 Requires-Dist: quri-parts-pyscf ; extra == "pyscf"
 Requires-Dist: quri-parts-qiskit ; extra == "qiskit"
+Requires-Dist: quri-parts-quantinuum ; extra == "quantinuum"
 Requires-Dist: quri-parts-qulacs ; extra == "qulacs"
 Requires-Dist: quri-parts-stim ; extra == "stim"
+Requires-Dist: quri-parts-tket ; extra == "tket"
 Project-URL: Documentation, https://quri-parts.qunasys.com
 Project-URL: Repository, https://github.com/QunaSys/quri-parts
 Description-Content-Type: text/markdown
 
 # QURI Parts
 
 
@@ -66,25 +68,29 @@
   - `quri-parts-core`: General components
       - Operator, state, estimator, sampler etc.
 - Platform (device/simulator) support
   - Quantum circuit simulators
       - `quri-parts-qulacs`: [Qulacs](https://github.com/qulacs/qulacs)
       - `quri-parts-stim`: [Stim](https://github.com/quantumlib/Stim)
       - `quri-parts-itensor`: [ITensor](https://github.com/ITensor/ITensors.jl)
+      - `quri-parts-tket`: [TKet](https://www.quantinuum.com/developers/tket)
   - Quantum platforms/SDKs
       - `quri-parts-braket`: [Amazon Braket SDK](https://github.com/aws/amazon-braket-sdk-python)
-      - `quri-parts-cirq`: [Cirq](https://quantumai.google/cirq) (Only circuit conversion is supported yet)
-      - `quri-parts-qiskit`: [Qiskit](https://qiskit.org/) (Circuit conversion and execution are not supported yet)
+      - `quri-parts-cirq`: [Cirq](https://quantumai.google/cirq) (Only circuit and operator conversion is supported yet)
+      - `quri-parts-qiskit`: [Qiskit](https://qiskit.org/)
+      - `quri-parts-quantinuum`: [Quantinuum](https://www.quantinuum.com/hardware/)
+      - `quri-parts-ionq`: [IONQ](https://ionq.com/docs/)
 - Intermediate representation support
   - `quri-parts-openqasm`: [OpenQASM 3.0](https://openqasm.com/)
 - `quri-parts-algo`: Algorithms
   - Ansatz, optimizer, error mitigation etc.
 - Chemistry
   - `quri-parts-chem`: General concepts
-      - Fermion-qubit mapping etc.
+      - Fermion-qubit mapping, electron integrals, ansatz etc.
+  - `quri-parts-pyscf`: [PySCF](https://pyscf.org/)
   - Library support
       - `quri-parts-openfermion`: [OpenFermion](https://quantumai.google/openfermion)
 
 
 ## Installation
 
 QURI Parts requires Python 3.9.8 or later.
```

