# Comparing `tmp/quri_parts_cirq-0.9.2.tar.gz` & `tmp/quri_parts_cirq-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_cirq-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_cirq-17.0.0.tar", max compression
```

## Comparing `quri_parts_cirq-0.9.2.tar` & `quri_parts_cirq-17.0.0.tar`

### file list

```diff
@@ -1,8 +1,11 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.862951 quri_parts_cirq-0.9.2/LICENSE
--rw-r--r--   0        0        0      252 2023-03-29 07:37:19.862951 quri_parts_cirq-0.9.2/README.md
--rw-r--r--   0        0        0     1088 2023-03-29 07:37:26.266980 quri_parts_cirq-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:25.486976 quri_parts_cirq-0.9.2/quri_parts/cirq/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.862951 quri_parts_cirq-0.9.2/quri_parts/cirq/__init__.py
--rw-r--r--   0        0        0     6617 2023-03-29 07:37:19.866951 quri_parts_cirq-0.9.2/quri_parts/cirq/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_cirq-0.9.2/quri_parts/cirq/py.typed
--rw-r--r--   0        0        0     1126 1970-01-01 00:00:00.000000 quri_parts_cirq-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/LICENSE
+-rw-r--r--   0        0        0      252 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/README.md
+-rw-r--r--   0        0        0     1089 2024-03-19 02:11:26.826021 quri_parts_cirq-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:26.254024 quri_parts_cirq-17.0.0/quri_parts/cirq/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/__init__.py
+-rw-r--r--   0        0        0      784 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/circuit/__init__.py
+-rw-r--r--   0        0        0     6728 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/circuit/circuit_converter.py
+-rw-r--r--   0        0        0     4102 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/circuit/cirq_circuit_converter.py
+-rw-r--r--   0        0        0     1467 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/operator/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.286138 quri_parts_cirq-17.0.0/quri_parts/cirq/py.typed
+-rw-r--r--   0        0        0     1127 1970-01-01 00:00:00.000000 quri_parts_cirq-17.0.0/PKG-INFO
```

### Comparing `quri_parts_cirq-0.9.2/LICENSE` & `quri_parts_cirq-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_cirq-0.9.2/pyproject.toml` & `quri_parts_cirq-17.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-cirq"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use Cirq with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_cirq-0.9.2/quri_parts/cirq/circuit/__init__.py` & `quri_parts_cirq-17.0.0/quri_parts/cirq/circuit/circuit_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     CircuitTranspiler,
     PauliDecomposeTranspiler,
     PauliRotationDecomposeTranspiler,
     SequentialTranspiler,
 )
 
 #: CircuitTranspiler to convert a circit configuration suitable for Cirq.
-CirqTranspiler: Callable[[], CircuitTranspiler] = lambda: SequentialTranspiler(
+CirqSetTranspiler: Callable[[], CircuitTranspiler] = lambda: SequentialTranspiler(
     [PauliDecomposeTranspiler(), PauliRotationDecomposeTranspiler()]
 )
 
 
 # Implementation is follwed from Qiskit (lambda → psi)
 class U1(Gate):
     """Define a cirq U1 gate."""
@@ -165,14 +165,16 @@
     gate_names.TOFFOLI: TOFFOLI,
 }
 
 
 def convert_gate(
     gate: QuantumGate,
 ) -> Operation:
+    """Converts a :class:`~QuantumGate` to
+    :class:`cirq.Operation`."""
     if is_single_qubit_gate_name(gate.name):
         if gate.name in _single_qubit_gate_cirq:
             return _single_qubit_gate_cirq[gate.name].on(
                 LineQubit(*gate.target_indices)
             )
         else:
             return _single_qubit_rotation_gate_cirq[gate.name](*gate.params).on(
@@ -194,26 +196,25 @@
     elif is_three_qubit_gate_name(gate.name):
         return _three_qubit_gate_cirq[gate.name].on(
             *(LineQubit(q) for q in (*gate.control_indices, *gate.target_indices))
         )
 
     elif is_unitary_matrix_gate_name(gate.name):
         return MatrixGate(np.array(gate.unitary_matrix)).on(
-            *[LineQubit(i) for i in gate.target_indices]
+            *[LineQubit(i) for i in reversed(gate.target_indices)]
         )
 
     elif is_parametric_gate_name(gate.name):
         raise ValueError("Parametric gates are not supported")
     else:
         raise NotImplementedError(
             f"{gate.name} conversion to Cirq gate not implemented"
         )
 
 
 def convert_circuit(circuit: NonParametricQuantumCircuit) -> Circuit:
+    """Converts a :class:`~NonParametricQuantumCircuit` to
+    :class:`cirq.Circuit`."""
     cirq_circuit = Circuit()
     for gate in circuit.gates:
         cirq_circuit.append(convert_gate(gate))
     return cirq_circuit
-
-
-__all__ = ["convert_gate", "convert_circuit", "CirqTranspiler"]
```

### Comparing `quri_parts_cirq-0.9.2/PKG-INFO` & `quri_parts_cirq-17.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-cirq
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use Cirq with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

