# Comparing `tmp/quri_parts_braket-0.9.2.tar.gz` & `tmp/quri_parts_braket-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_braket-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_braket-17.0.0.tar", max compression
```

## Comparing `quri_parts_braket-0.9.2.tar` & `quri_parts_braket-17.0.0.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/LICENSE
--rw-r--r--   0        0        0      369 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/README.md
--rw-r--r--   0        0        0     1197 2023-03-29 07:37:23.482965 quri_parts_braket-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:22.614960 quri_parts_braket-0.9.2/quri_parts/braket/NOTICE
--rw-r--r--   0        0        0      541 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/__init__.py
--rw-r--r--   0        0        0      803 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/__init__.py
--rw-r--r--   0        0        0     1452 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/device.py
--rw-r--r--   0        0        0     7359 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/sampling.py
--rw-r--r--   0        0        0     1310 2023-03-29 07:37:19.854951 quri_parts_braket-0.9.2/quri_parts/braket/backend/transpiler.py
--rw-r--r--   0        0        0     6576 2023-03-29 07:37:19.858951 quri_parts_braket-0.9.2/quri_parts/braket/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.858951 quri_parts_braket-0.9.2/quri_parts/braket/py.typed
--rw-r--r--   0        0        0     1316 1970-01-01 00:00:00.000000 quri_parts_braket-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/LICENSE
+-rw-r--r--   0        0        0      369 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/README.md
+-rw-r--r--   0        0        0     1198 2024-03-19 02:11:24.774031 quri_parts_braket-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:24.154035 quri_parts_braket-17.0.0/quri_parts/braket/NOTICE
+-rw-r--r--   0        0        0      541 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/__init__.py
+-rw-r--r--   0        0        0      803 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/backend/__init__.py
+-rw-r--r--   0        0        0     1452 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/backend/device.py
+-rw-r--r--   0        0        0     7474 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/backend/sampling.py
+-rw-r--r--   0        0        0     1310 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/backend/transpiler.py
+-rw-r--r--   0        0        0     6154 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/circuit/__init__.py
+-rw-r--r--   0        0        0     4213 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/circuit/braket_circuit_converter.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.278138 quri_parts_braket-17.0.0/quri_parts/braket/py.typed
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 quri_parts_braket-17.0.0/PKG-INFO
```

### Comparing `quri_parts_braket-0.9.2/LICENSE` & `quri_parts_braket-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.2/pyproject.toml` & `quri_parts_braket-17.0.0/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-braket"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use Amazon Braket SDK with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/__init__.py` & `quri_parts_braket-17.0.0/quri_parts/braket/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/backend/__init__.py` & `quri_parts_braket-17.0.0/quri_parts/braket/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/backend/device.py` & `quri_parts_braket-17.0.0/quri_parts/braket/backend/device.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/backend/sampling.py` & `quri_parts_braket-17.0.0/quri_parts/braket/backend/sampling.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     SamplingCounts,
     SamplingJob,
     SamplingResult,
 )
 from quri_parts.backend.qubit_mapping import BackendQubitMapping, QubitMappedSamplingJob
 from quri_parts.braket.circuit import (
     BraketCircuitConverter,
-    BraketTranspiler,
+    BraketSetTranspiler,
     convert_circuit,
 )
 from quri_parts.circuit import NonParametricQuantumCircuit
 from quri_parts.circuit.transpile import CircuitTranspiler, SequentialTranspiler
 
 from .transpiler import AwsDeviceTranspiler
 
@@ -72,15 +72,15 @@
 
     Args:
         device: A Braket :class:`braket.devices.Device` for circuit execution.
         circuit_converter: A function converting \
             :class:`~quri_parts.circuit.NonParametricQuantumCircuit` to \
             a Braket :class:`braket.circuits.Circuit`.
         circuit_transpiler: A transpiler applied to the circuit before running it.
-            :class:`~BraketTranspiler` is used when not specified.
+            :class:`~BraketSetTranspiler` is used when not specified.
         enable_shots_roundup: If True, when a number of shots specified to \
             :meth:`~sample` is smaller than the minimum number of shots supported by \
             the device, it is rounded up to the minimum. In this case, it is possible \
             that shots more than specified are used. If it is strictly not allowed to \
             exceed the specified shot count, set this argument to False.
         qubit_mapping: If specified, indices of qubits in the circuit are remapped \
             before running it on the backend. It can be used when you want to use \
@@ -94,28 +94,28 @@
             :meth:`braket.devices.Device.run` method.
     """
 
     def __init__(
         self,
         device: Device,
         circuit_converter: BraketCircuitConverter = convert_circuit,
-        circuit_transpiler: Optional[CircuitTranspiler] = None,
+        circuit_transpiler: Optional[CircuitTranspiler] = BraketSetTranspiler(),
         enable_shots_roundup: bool = True,
         qubit_mapping: Optional[Mapping[int, int]] = None,
         run_kwargs: Mapping[str, Any] = {},
     ):
         self._device = device
         self._circuit_converter = circuit_converter
 
         self._qubit_mapping = None
         if qubit_mapping is not None:
             self._qubit_mapping = BackendQubitMapping(qubit_mapping)
 
         if circuit_transpiler is None:
-            circuit_transpiler = BraketTranspiler()
+            circuit_transpiler = BraketSetTranspiler()
         if isinstance(device, AwsDevice):
             circuit_transpiler = SequentialTranspiler(
                 [circuit_transpiler, AwsDeviceTranspiler(device)]
             )
         if self._qubit_mapping:
             circuit_transpiler = SequentialTranspiler(
                 [circuit_transpiler, self._qubit_mapping.circuit_transpiler]
@@ -136,16 +136,19 @@
 
     def sample(self, circuit: NonParametricQuantumCircuit, n_shots: int) -> SamplingJob:
         if not n_shots >= 1:
             raise ValueError("n_shots should be a positive integer.")
         if self._max_shots is not None and n_shots > self._max_shots:
             shot_dist = [self._max_shots] * (n_shots // self._max_shots)
             remaining = n_shots % self._max_shots
-            if remaining >= self._min_shots or self._enable_shots_roundup:
-                shot_dist.append(max(remaining, self._min_shots))
+            if remaining > 0:
+                if remaining >= self._min_shots:
+                    shot_dist.append(remaining)
+                elif self._enable_shots_roundup:
+                    shot_dist.append(self._min_shots)
         else:
             if n_shots >= self._min_shots or self._enable_shots_roundup:
                 shot_dist = [max(n_shots, self._min_shots)]
             else:
                 raise ValueError(
                     f"n_shots is smaller than minimum shot count ({self._min_shots}) "
                     "supported by the device. Try larger n_shots or use "
```

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/backend/transpiler.py` & `quri_parts_braket-17.0.0/quri_parts/braket/backend/transpiler.py`

 * *Files identical despite different names*

### Comparing `quri_parts_braket-0.9.2/quri_parts/braket/circuit/__init__.py` & `quri_parts_braket-17.0.0/quri_parts/braket/circuit/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -33,20 +33,22 @@
     CircuitTranspiler,
     IdentityInsertionTranspiler,
     PauliDecomposeTranspiler,
     PauliRotationDecomposeTranspiler,
     SequentialTranspiler,
 )
 
+from .braket_circuit_converter import circuit_from_braket, gate_from_braket
+
 BraketCircuitConverter: TypeAlias = Callable[
     [NonParametricQuantumCircuit, Optional[CircuitTranspiler]], Circuit
 ]
 
 
-class BraketTranspiler(SequentialTranspiler):
+class BraketSetTranspiler(SequentialTranspiler):
     """CircuitTranspiler to convert a circuit configuration suitable for
     Braket."""
 
     def __init__(self) -> None:
         transpilers = [
             PauliDecomposeTranspiler(),
             PauliRotationDecomposeTranspiler(),
@@ -61,14 +63,16 @@
     gate_names.Y: Gate.Y,
     gate_names.Z: Gate.Z,
     gate_names.H: Gate.H,
     gate_names.S: Gate.S,
     gate_names.Sdag: Gate.Si,
     gate_names.T: Gate.T,
     gate_names.Tdag: Gate.Ti,
+    gate_names.SqrtX: Gate.V,
+    gate_names.SqrtXdag: Gate.Vi,
 }
 
 _single_qubit_rotation_gate_braket: Mapping[SingleQubitGateNameType, Type[Gate]] = {
     gate_names.RX: Gate.Rx,
     gate_names.RY: Gate.Ry,
     gate_names.RZ: Gate.Rz,
 }
@@ -85,39 +89,24 @@
 
 _parametric_gate_braket: Mapping[ParametricGateNameType, Type[Gate]] = {
     gate_names.ParametricRX: Gate.Rx,
     gate_names.ParametricRY: Gate.Ry,
     gate_names.ParametricRZ: Gate.Rz,
 }
 
-_U_gate_matrix: Mapping[
-    SingleQubitGateNameType, Callable[[Sequence[float]], Sequence[Sequence[complex]]]
-] = {
-    gate_names.U1: lambda angle: [[1.0, 0.0], [0.0, np.exp(angle[0] * 1.0j)]],
-    gate_names.U2: lambda angle: [
-        [1.0 / np.sqrt(2.0), -np.exp(angle[1] * 1.0j) / np.sqrt(2.0)],
-        [
-            np.exp(angle[0] * 1.0j) / np.sqrt(2.0),
-            np.exp((angle[0] + angle[1]) * 1.0j) / np.sqrt(2.0),
-        ],
-    ],
-    gate_names.U3: lambda angle: [
-        [np.cos(angle[0] / 2.0), -np.exp(angle[2] * 1.0j) * np.sin(angle[0] / 2.0)],
-        [
-            np.exp(angle[1] * 1.0j) * np.sin(angle[0] / 2.0),
-            np.exp((angle[1] + angle[2]) * 1.0j) * np.cos(angle[0] / 2.0),
-        ],
-    ],
+# U2 gate is implemeted as a special case of U3.
+_U_gate_matrix: Mapping[SingleQubitGateNameType, Callable[[Sequence[float]], Gate]] = {
+    gate_names.U1: lambda angles: Gate.PhaseShift(*angles),
+    gate_names.U2: lambda angles: Gate.U(np.pi / 2, *angles),
+    gate_names.U3: lambda angles: Gate.U(*angles),
 }
 
 _special_named_gate_matrix: Mapping[
     SingleQubitGateNameType, Sequence[Sequence[complex]]
 ] = {
-    gate_names.SqrtX: [[0.5 + 0.5j, 0.5 - 0.5j], [0.5 - 0.5j, 0.5 + 0.5j]],
-    gate_names.SqrtXdag: [[0.5 - 0.5j, 0.5 + 0.5j], [0.5 + 0.5j, 0.5 - 0.5j]],
     gate_names.SqrtY: [[0.5 + 0.5j, -0.5 - 0.5j], [0.5 + 0.5j, 0.5 + 0.5j]],
     gate_names.SqrtYdag: [[0.5 - 0.5j, 0.5 - 0.5j], [-0.5 + 0.5j, 0.5 - 0.5j]],
 }
 
 
 def convert_gate(gate: QuantumGate) -> Instruction:
     if not is_gate_name(gate.name):
@@ -127,16 +116,15 @@
         if gate.name in _single_qubit_gate_braket:
             b_gate = _single_qubit_gate_braket[gate.name](*gate.params)
             return Instruction(b_gate, gate.target_indices)
         elif gate.name in _single_qubit_rotation_gate_braket:
             b_gate = _single_qubit_rotation_gate_braket[gate.name](*gate.params)
             return Instruction(b_gate, gate.target_indices)
         elif gate.name in _U_gate_matrix:
-            u_matrix = _U_gate_matrix[gate.name](gate.params)
-            b_gate = Gate.Unitary(np.array(u_matrix))
+            b_gate = _U_gate_matrix[gate.name](gate.params)
             return Instruction(b_gate, gate.target_indices)
         elif gate.name in _special_named_gate_matrix:
             s_matrix = _special_named_gate_matrix[gate.name]
             b_gate = Gate.Unitary(np.array(s_matrix))
             return Instruction(b_gate, gate.target_indices)
 
     elif is_two_qubit_gate_name(gate.name):
@@ -151,15 +139,15 @@
             b_gate = _three_qubit_gate_braket[gate.name](*gate.params)
             return Instruction(
                 b_gate, tuple(gate.control_indices) + tuple(gate.target_indices)
             )
 
     elif is_unitary_matrix_gate_name(gate.name):
         b_gate = Gate.Unitary(np.array(gate.unitary_matrix))
-        return Instruction(b_gate, gate.target_indices)
+        return Instruction(b_gate, reversed(gate.target_indices))
 
     elif is_parametric_gate_name(gate.name):
         raise ValueError("Parametric gates are not supported.")
     elif is_multi_qubit_gate_name(gate.name):
         pass
     else:
         assert False, "Unreachable"
@@ -167,24 +155,26 @@
     raise NotImplementedError(
         f"Conversion of {gate.name} to braket has not been implemented."
     )
 
 
 def convert_circuit(
     circuit: NonParametricQuantumCircuit,
-    transpiler: Optional[CircuitTranspiler] = BraketTranspiler(),
+    transpiler: Optional[CircuitTranspiler] = BraketSetTranspiler(),
 ) -> Circuit:
     if transpiler is not None:
         circuit = transpiler(circuit)
 
     braket_circuit = Circuit()
     for gate in circuit.gates:
         braket_circuit.add_instruction(convert_gate(gate))
     return braket_circuit
 
 
 __all__ = [
     "BraketCircuitConverter",
-    "BraketTranspiler",
+    "BraketSetTranspiler",
     "convert_gate",
     "convert_circuit",
+    "gate_from_braket",
+    "circuit_from_braket",
 ]
```

### Comparing `quri_parts_braket-0.9.2/PKG-INFO` & `quri_parts_braket-17.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-braket
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use Amazon Braket SDK with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

