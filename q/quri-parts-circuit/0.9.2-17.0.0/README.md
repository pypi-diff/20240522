# Comparing `tmp/quri_parts_circuit-0.9.2.tar.gz` & `tmp/quri_parts_circuit-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_circuit-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_circuit-17.0.0.tar", max compression
```

## Comparing `quri_parts_circuit-0.9.2.tar` & `quri_parts_circuit-17.0.0.tar`

### file list

```diff
@@ -1,32 +1,34 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/LICENSE
--rw-r--r--   0        0        0      259 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/README.md
--rw-r--r--   0        0        0     1022 2023-03-29 07:37:25.310975 quri_parts_circuit-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      201 2023-03-29 07:37:24.538971 quri_parts_circuit-0.9.2/quri_parts/circuit/NOTICE
--rw-r--r--   0        0        0     3636 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/__init__.py
--rw-r--r--   0        0        0    11742 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit.py
--rw-r--r--   0        0        0     9067 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_linear_mapped.py
--rw-r--r--   0        0        0    14569 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_parametric.py
--rw-r--r--   0        0        0     2324 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/clifford_gate.py
--rw-r--r--   0        0        0     1496 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/gate.py
--rw-r--r--   0        0        0     5263 2023-03-29 07:37:19.858951 quri_parts_circuit-0.9.2/quri_parts/circuit/gate_names.py
--rw-r--r--   0        0        0    14467 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/gates.py
--rw-r--r--   0        0        0     2167 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/inverse_gate.py
--rw-r--r--   0        0        0     1880 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/__init__.py
--rw-r--r--   0        0        0    35663 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_instruction.py
--rw-r--r--   0        0        0    14041 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_model.py
--rw-r--r--   0        0        0     1250 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter.py
--rw-r--r--   0        0        0    11601 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_mapping.py
--rw-r--r--   0        0        0     5514 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_shift.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/py.typed
--rw-r--r--   0        0        0      702 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/topology/__init__.py
--rw-r--r--   0        0        0     5227 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/topology/square_lattice.py
--rw-r--r--   0        0        0     5759 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/__init__.py
--rw-r--r--   0        0        0     3289 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/clifford_approximation.py
--rw-r--r--   0        0        0    16837 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/gate_kind_decomposer.py
--rw-r--r--   0        0        0     1518 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/identity_insertion.py
--rw-r--r--   0        0        0     2845 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/multi_pauli_decomposer.py
--rw-r--r--   0        0        0     2358 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/qubit_remapping.py
--rw-r--r--   0        0        0     5221 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/transpiler.py
--rw-r--r--   0        0        0     3835 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/unitary_matrix_decomposer.py
--rw-r--r--   0        0        0     2387 2023-03-29 07:37:19.862951 quri_parts_circuit-0.9.2/quri_parts/circuit/utils/controlled_rotations.py
--rw-r--r--   0        0        0     1118 1970-01-01 00:00:00.000000 quri_parts_circuit-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/LICENSE
+-rw-r--r--   0        0        0      259 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/README.md
+-rw-r--r--   0        0        0     1031 2024-03-19 02:11:26.126024 quri_parts_circuit-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0      201 2024-03-19 02:11:25.562027 quri_parts_circuit-17.0.0/quri_parts/circuit/NOTICE
+-rw-r--r--   0        0        0     3707 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/__init__.py
+-rw-r--r--   0        0        0    13630 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/circuit.py
+-rw-r--r--   0        0        0    10614 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/circuit_linear_mapped.py
+-rw-r--r--   0        0        0    16844 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/circuit_parametric.py
+-rw-r--r--   0        0        0     2323 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/clifford_gate.py
+-rw-r--r--   0        0        0     2989 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/gate.py
+-rw-r--r--   0        0        0     5315 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/gate_names.py
+-rw-r--r--   0        0        0    15149 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/gates.py
+-rw-r--r--   0        0        0     3021 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/inverse.py
+-rw-r--r--   0        0        0     1880 2024-03-19 02:11:01.282138 quri_parts_circuit-17.0.0/quri_parts/circuit/noise/__init__.py
+-rw-r--r--   0        0        0    35663 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/noise/noise_instruction.py
+-rw-r--r--   0        0        0    15035 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/noise/noise_model.py
+-rw-r--r--   0        0        0     1250 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/parameter.py
+-rw-r--r--   0        0        0    11601 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/parameter_mapping.py
+-rw-r--r--   0        0        0     5514 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/parameter_shift.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/py.typed
+-rw-r--r--   0        0        0      702 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/topology/__init__.py
+-rw-r--r--   0        0        0     5227 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/topology/square_lattice.py
+-rw-r--r--   0        0        0     8441 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     3289 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/clifford_approximation.py
+-rw-r--r--   0        0        0     8889 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/fuse.py
+-rw-r--r--   0        0        0    16837 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/gate_kind_decomposer.py
+-rw-r--r--   0        0        0     2005 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/identity_manipulation.py
+-rw-r--r--   0        0        0     2855 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/multi_pauli_decomposer.py
+-rw-r--r--   0        0        0     2358 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/qubit_remapping.py
+-rw-r--r--   0        0        0     5283 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/transpiler.py
+-rw-r--r--   0        0        0    11369 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/unitary_matrix_decomposer.py
+-rw-r--r--   0        0        0    13947 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/utils/circuit_drawer.py
+-rw-r--r--   0        0        0     2387 2024-03-19 02:11:01.286138 quri_parts_circuit-17.0.0/quri_parts/circuit/utils/controlled_rotations.py
+-rw-r--r--   0        0        0     1119 1970-01-01 00:00:00.000000 quri_parts_circuit-17.0.0/PKG-INFO
```

### Comparing `quri_parts_circuit-0.9.2/LICENSE` & `quri_parts_circuit-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/pyproject.toml` & `quri_parts_circuit-17.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-circuit"
-version = "0.9.2"
+version = "17.0.0"
 description = "Platform-independent quantum circuit library"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
@@ -27,15 +27,15 @@
 [tool.poetry.dependencies]
 python = "^3.9.8"
 typing-extensions = "^4.1.1"
 numpy = ">=1.22.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.0.1"
-flake8 = "^4.0.1"
+flake8 = ">=4.0.1,<7.0.0"
 mypy = ">=0.950"
 docformatter = "^1.4"
 isort = "^5.10.1"
 black = "^23.1.0"
 
 [tool.black]
 line-length = 88
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/__init__.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     SWAP,
     TOFFOLI,
     U1,
     U2,
     U3,
     H,
     Identity,
+    Measurement,
     ParametricPauliRotation,
     ParametricRX,
     ParametricRY,
     ParametricRZ,
     Pauli,
     PauliRotation,
     S,
@@ -61,15 +62,15 @@
     Tdag,
     TwoQubitUnitaryMatrix,
     UnitaryMatrix,
     X,
     Y,
     Z,
 )
-from .inverse_gate import inverse_gate
+from .inverse import inverse_circuit, inverse_gate
 from .parameter import CONST, Parameter
 from .parameter_mapping import (
     LinearParameterFunction,
     LinearParameterMapping,
     ParameterMapping,
     ParameterOrLinearFunction,
 )
@@ -114,14 +115,15 @@
     "TOFFOLI",
     "Pauli",
     "PauliRotation",
     "ParametricRX",
     "ParametricRY",
     "ParametricRZ",
     "ParametricPauliRotation",
+    "Measurement",
     "QuantumCircuitProtocol",
     "MutableQuantumCircuitProtocol",
     "GateSequence",
     "NonParametricQuantumCircuit",
     "QuantumCircuit",
     "ImmutableQuantumCircuit",
     "Parameter",
@@ -136,9 +138,10 @@
     "ImmutableBoundParametricQuantumCircuit",
     "LinearParameterFunction",
     "LinearParameterMapping",
     "LinearMappedUnboundParametricQuantumCircuitBase",
     "LinearMappedUnboundParametricQuantumCircuit",
     "ImmutableLinearMappedUnboundParametricQuantumCircuit",
     "inverse_gate",
+    "inverse_circuit",
     "is_clifford",
 ]
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/circuit.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import warnings
 from abc import ABC, abstractmethod, abstractproperty
 from collections.abc import Sequence
 from typing import Optional, Protocol, Union
 
-from typing_extensions import TypeAlias
+from typing_extensions import TypeAlias, TypeGuard
 
 from .gate import ParametricQuantumGate, QuantumGate
 from .gates import (
     CNOT,
     CZ,
     RX,
     RY,
@@ -24,14 +25,15 @@
     SWAP,
     TOFFOLI,
     U1,
     U2,
     U3,
     H,
     Identity,
+    Measurement,
     Pauli,
     PauliRotation,
     S,
     Sdag,
     SingleQubitUnitaryMatrix,
     SqrtX,
     SqrtXdag,
@@ -45,14 +47,20 @@
     Y,
     Z,
 )
 
 GateSequence: TypeAlias = Union["NonParametricQuantumCircuit", Sequence[QuantumGate]]
 
 
+def is_gate_sequence(
+    gates: Union["QuantumCircuitProtocol", GateSequence]
+) -> TypeGuard[GateSequence]:
+    return isinstance(gates, (NonParametricQuantumCircuit, Sequence))
+
+
 class QuantumCircuitProtocol(Protocol):
     """Interface protocol for a quantum circuit.
 
     This interface covers all quantum circuit classes, including:
 
     * Non-parametric circuit, parametric circuit and linearly mapped parametric circuit
     * Mutable and immutable circuit classes
@@ -60,14 +68,19 @@
 
     @abstractproperty
     def qubit_count(self) -> int:
         """Number of qubits involved in the circuit."""
         ...
 
     @abstractproperty
+    def cbit_count(self) -> int:
+        """Number of classical bits involved in the circuit."""
+        ...
+
+    @abstractproperty
     def depth(self) -> int:
         """Returns circuit depth."""
         ...
 
 
 class MutableQuantumCircuitProtocol(QuantumCircuitProtocol, Protocol):
     r"""Interface protocol for a mutable quantum circuit.
@@ -221,14 +234,27 @@
         target_qubits: Sequence[int],
         pauli_id_list: Sequence[int],
         angle: float,
     ) -> None:
         """Add a Pauli rotation gate to the circuit."""
         self.add_gate(PauliRotation(target_qubits, pauli_id_list, angle))
 
+    def measure(
+        self,
+        qubit_indices: Union[int, Sequence[int]],
+        classical_indices: Union[int, Sequence[int]],
+    ) -> None:
+        """Adds measurement gate at selected qubits."""
+        if isinstance(qubit_indices, int):
+            qubit_indices = [qubit_indices]
+        if isinstance(classical_indices, int):
+            classical_indices = [classical_indices]
+
+        self.add_gate(Measurement(qubit_indices, classical_indices))
+
 
 class NonParametricQuantumCircuit(QuantumCircuitProtocol, ABC):
     """A base class for quantum circuits having only non-parametric gates.
 
     This class support ``+`` operator with ``GateSequence``.
     """
 
@@ -269,53 +295,78 @@
 
         Use this method when you want to get a new circuit based on an
         existing circuit but don't want to modify it.
         """
         ...
 
     def __add__(self, gates: GateSequence) -> "QuantumCircuit":
+        if not is_gate_sequence(gates):
+            return NotImplemented
         return self.combine(gates)
 
 
 class QuantumCircuit(NonParametricQuantumCircuit, MutableQuantumCircuitProtocol):
     """A mutable quantum circuit having only non-parametric gates."""
 
     def __init__(
         self,
         qubit_count: int,
+        cbit_count: int = 0,
         gates: Sequence[QuantumGate] = [],
     ):
         self._qubit_count = qubit_count
-        self._gates = list(gates)
+        if isinstance(cbit_count, Sequence):
+            warnings.warn(
+                "QuantumCircuit initialization takes cbit_count before gates.",
+                DeprecationWarning,
+            )
+            self._gates = list(cbit_count)
+            self._cbit_count = 0
+        else:
+            self._cbit_count = cbit_count
+            self._gates = list(gates)
 
     @property
     def qubit_count(self) -> int:
         return self._qubit_count
 
     @property
+    def cbit_count(self) -> int:
+        return self._cbit_count
+
+    @property
     def gates(self) -> Sequence[QuantumGate]:
         return tuple(self._gates)
 
     def freeze(self) -> "ImmutableQuantumCircuit":
         return ImmutableQuantumCircuit(self)
 
     def get_mutable_copy(self) -> "QuantumCircuit":
-        circuit = QuantumCircuit(self.qubit_count, self._gates)
+        circuit = QuantumCircuit(self.qubit_count, self.cbit_count, self._gates)
         return circuit
 
     def add_gate(self, gate: QuantumGate, gate_index: Optional[int] = None) -> None:
         if isinstance(gate, ParametricQuantumGate):
             raise ValueError(
                 "QuantumCircuit only accepts QuantumGate, not ParametricQuantumGate."
             )
         if max([*gate.control_indices, *gate.target_indices]) >= self.qubit_count:
             raise ValueError(
                 "The indices of the gate applied must be smaller than qubit_count"
             )
-        if gate_index:
+        if (
+            len(gate.classical_indices) > 0
+            and max(gate.classical_indices) >= self.cbit_count
+        ):
+            raise ValueError(
+                "The classical indices of the gate applied must be smaller",
+                "than cbit_count",
+            )
+
+        if gate_index is not None:
             self._gates.insert(gate_index, gate)
         else:
             self._gates.append(gate)
 
     def extend(self, gates: GateSequence) -> None:
         if isinstance(gates, NonParametricQuantumCircuit):
             gates = gates.gates
@@ -324,37 +375,44 @@
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, NonParametricQuantumCircuit):
             return False
         return self.freeze() == other.freeze()
 
     def __iadd__(self, gates: GateSequence) -> "QuantumCircuit":
+        if not is_gate_sequence(gates):
+            return NotImplemented
         self.extend(gates)
         return self
 
 
 class ImmutableQuantumCircuit(NonParametricQuantumCircuit):
     """An immutable quantum circuit having only non-parametric gates."""
 
-    def __init__(self, circuit: QuantumCircuit):
+    def __init__(self, circuit: NonParametricQuantumCircuit):
         self._qubit_count = circuit.qubit_count
+        self._cbit_count = circuit.cbit_count
         self._gates = circuit.gates
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, NonParametricQuantumCircuit):
             return False
         f = other.freeze()
         return (self.qubit_count, self.gates) == (f.qubit_count, f.gates)
 
     @property
     def qubit_count(self) -> int:
         return self._qubit_count
 
     @property
+    def cbit_count(self) -> int:
+        return self._cbit_count
+
+    @property
     def gates(self) -> Sequence[QuantumGate]:
         return self._gates
 
     def freeze(self) -> "ImmutableQuantumCircuit":
         return self
 
     def get_mutable_copy(self) -> QuantumCircuit:
-        return QuantumCircuit(self.qubit_count, self.gates)
+        return QuantumCircuit(self.qubit_count, self.cbit_count, self.gates)
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_linear_mapped.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/circuit_linear_mapped.py`

 * *Files 5% similar despite different names*

```diff
@@ -36,14 +36,18 @@
     _circuit: UnboundParametricQuantumCircuitBase
 
     @property
     def qubit_count(self) -> int:
         return self._circuit.qubit_count
 
     @property
+    def cbit_count(self) -> int:
+        return self._circuit.cbit_count
+
+    @property
     def parameter_count(self) -> int:
         return len(self._param_mapping.in_params)
 
     @property
     def depth(self) -> int:
         return self._circuit.depth
 
@@ -59,33 +63,54 @@
     def param_mapping(self) -> LinearParameterMapping:
         return self._param_mapping
 
     def primitive_circuit(self) -> ImmutableUnboundParametricQuantumCircuit:
         return self._circuit.freeze()
 
     def get_mutable_copy(self) -> "LinearMappedUnboundParametricQuantumCircuit":
-        circuit = LinearMappedUnboundParametricQuantumCircuit(self.qubit_count)
+        circuit = LinearMappedUnboundParametricQuantumCircuit(
+            self.qubit_count, self.cbit_count
+        )
         circuit._param_mapping = self._param_mapping
         circuit._circuit = self._circuit.get_mutable_copy()
         return circuit
 
     def combine(
         self,
-        gates: Union[GateSequence, "LinearMappedUnboundParametricQuantumCircuitBase"],
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
     ) -> "LinearMappedUnboundParametricQuantumCircuit":
-        circuit = LinearMappedUnboundParametricQuantumCircuit(self.qubit_count)
-        circuit.extend(self)
-        circuit.extend(gates)
+        circuit = LinearMappedUnboundParametricQuantumCircuit(
+            self.qubit_count, self.cbit_count
+        )
+        try:
+            circuit.extend(self)
+            circuit.extend(gates)
+        except ValueError:
+            return NotImplemented
         return circuit
 
     def __add__(
         self,
-        gates: Union[GateSequence, "LinearMappedUnboundParametricQuantumCircuitBase"],
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
+    ) -> "LinearMappedUnboundParametricQuantumCircuit":
+        try:
+            return self.combine(gates)
+        except ValueError:
+            return NotImplemented
+
+    def __radd__(
+        self, gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol]
     ) -> "LinearMappedUnboundParametricQuantumCircuit":
-        return self.combine(gates)
+        combined_circuit = LinearMappedUnboundParametricQuantumCircuit(self.qubit_count)
+        try:
+            combined_circuit.extend(gates)
+            combined_circuit.extend(self)
+        except ValueError:
+            return NotImplemented
+        return combined_circuit
 
     def bind_parameters(
         self, params: Sequence[float]
     ) -> ImmutableBoundParametricQuantumCircuit:
         raw_param_vars = self._param_mapping.mapper(
             dict(zip(self._param_mapping.in_params, params))
         )
@@ -95,18 +120,18 @@
 class LinearMappedUnboundParametricQuantumCircuit(
     LinearMappedUnboundParametricQuantumCircuitBase,
     MutableUnboundParametricQuantumCircuitProtocol,
 ):
     """A mutable parametric quantum circuit where parameters of parametric
     gates are given by linear functions of circuit parameters."""
 
-    def __init__(self, qubit_count: int):
+    def __init__(self, qubit_count: int, cbit_count: int = 0):
         self._param_mapping = LinearParameterMapping()
         self._circuit: UnboundParametricQuantumCircuit = (
-            UnboundParametricQuantumCircuit(qubit_count)
+            UnboundParametricQuantumCircuit(qubit_count, cbit_count)
         )
 
     def add_parameters(self, *names: str) -> Sequence[Parameter]:
         """Add new parameters for the circuit.
 
         Newly created parameters are returned as a sequence. Before
         adding a parametric gate to the circuit, all used parameters
@@ -185,46 +210,66 @@
         param = self._circuit.add_ParametricPauliRotation_gate(qubit_indices, pauli_ids)
         self._param_mapping = self._param_mapping.with_data_updated(
             out_params_addition=(param,), mapping_update={param: angle}
         )
 
     def extend(
         self,
-        gates: Union[GateSequence, LinearMappedUnboundParametricQuantumCircuitBase],
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
     ) -> None:
         """Extend the parametric circuit with given gates or a linear mapped
         unbound parametric circuit.
 
         If the two linear mapped parametric circuit share the same
         parameters, they are treated as the same parameters, in contrast
         to the case of :class:`~UnboundParametricQuantumCircuit`.
         """
-        if isinstance(gates, LinearMappedUnboundParametricQuantumCircuitBase):
+        if isinstance(gates, UnboundParametricQuantumCircuitProtocol):
             if self.qubit_count != gates.qubit_count:
                 raise ValueError(
                     f"Qubit count not match (self={self.qubit_count}, "
                     f"other={gates.qubit_count})."
                 )
-            self._param_mapping = self._param_mapping.combine(gates._param_mapping)
-            self._circuit.extend(gates._circuit)
+            if isinstance(gates.param_mapping, LinearParameterMapping):
+                self._param_mapping = self._param_mapping.combine(gates.param_mapping)
+            else:
+                raise ValueError(
+                    f"Unsupported parameter mapping type: {type(gates.param_mapping)}"
+                )
+            self._circuit.extend(gates.primitive_circuit())
         else:
             if isinstance(gates, NonParametricQuantumCircuit):
+                if self.qubit_count != gates.qubit_count:
+                    raise ValueError(
+                        f"Qubit count not match (self={self.qubit_count}, "
+                        f"other={gates.qubit_count})."
+                    )
                 gates = gates.gates
             for gate in gates:
                 self.add_gate(gate)
 
+    def __iadd__(
+        self,
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
+    ) -> "LinearMappedUnboundParametricQuantumCircuit":
+        try:
+            self.extend(gates)
+        except ValueError:
+            return NotImplemented
+        return self
+
     def freeze(self) -> "ImmutableLinearMappedUnboundParametricQuantumCircuit":
         return ImmutableLinearMappedUnboundParametricQuantumCircuit(self)
 
 
 class ImmutableLinearMappedUnboundParametricQuantumCircuit(
     LinearMappedUnboundParametricQuantumCircuitBase
 ):
     """An immutable parametric quantum circuit where parameters of parametric
     gates are given by linear functions of circuit parameters."""
 
-    def __init__(self, circuit: LinearMappedUnboundParametricQuantumCircuit):
+    def __init__(self, circuit: LinearMappedUnboundParametricQuantumCircuitBase):
         self._param_mapping = circuit._param_mapping
         self._circuit = circuit._circuit.freeze()
 
     def freeze(self) -> "ImmutableLinearMappedUnboundParametricQuantumCircuit":
         return self
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/circuit_parametric.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/circuit_parametric.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,25 +7,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import ABC, abstractmethod, abstractproperty
 from collections.abc import Mapping, Sequence
 from functools import cached_property
-from typing import Optional, Protocol, Union
+from typing import Optional, Protocol, Union, runtime_checkable
 
 from quri_parts.circuit import gate_names
 
 from .circuit import (
     GateSequence,
     ImmutableQuantumCircuit,
     MutableQuantumCircuitProtocol,
     NonParametricQuantumCircuit,
     QuantumCircuit,
     QuantumCircuitProtocol,
+    is_gate_sequence,
 )
 from .gate import ParametricQuantumGate, QuantumGate
 from .gates import (
     RX,
     RY,
     RZ,
     ParametricPauliRotation,
@@ -34,14 +35,15 @@
     ParametricRZ,
     PauliRotation,
 )
 from .parameter import Parameter
 from .parameter_mapping import LinearParameterMapping, ParameterMapping
 
 
+@runtime_checkable
 class UnboundParametricQuantumCircuitProtocol(QuantumCircuitProtocol, Protocol):
     """Interface protocol for a quantum circuit containing unbound (i.e. not
     assigned values) parameters.
 
     For circuit execution, the parameters need to be assigned concrete
     values by :meth:`~bind_parameters` method.
     """
@@ -72,15 +74,15 @@
 
         Use this method when you want to get a new circuit based on an
         existing circuit but don't want to modify it.
         """
         ...
 
     @abstractmethod
-    def primitive_circuit(self) -> "UnboundParametricQuantumCircuitProtocol":
+    def primitive_circuit(self) -> "ImmutableUnboundParametricQuantumCircuit":
         r"""Returns the parametric circuit where each gate has an independent
         parameter.
 
         Note that some parametric circuit,
         e.g. :class:`LinearMappedUnboundParametricQuantumCircuit`, can have non-trivial
         mapping of the parameters. In this "primitive circuit", however,
         gate parameters are treated as independent,
@@ -124,14 +126,26 @@
         ...
 
     @abstractproperty
     def param_mapping(self) -> ParameterMapping:
         """Returns the parameter mapping of the circuit."""
         ...
 
+    def __add__(
+        self, gates: Union[GateSequence, "UnboundParametricQuantumCircuitProtocol"]
+    ) -> "UnboundParametricQuantumCircuitProtocol":
+        """Returns a new combined circuit with the given gates added."""
+        ...
+
+    def __radd__(
+        self, gates: Union[GateSequence, "UnboundParametricQuantumCircuitProtocol"]
+    ) -> "UnboundParametricQuantumCircuitProtocol":
+        """Returns a new combined circuit with the given gates added."""
+        ...
+
 
 class MutableUnboundParametricQuantumCircuitProtocol(
     UnboundParametricQuantumCircuitProtocol, MutableQuantumCircuitProtocol, Protocol
 ):
     ...
 
 
@@ -178,33 +192,33 @@
 
     @property
     def param_mapping(self) -> LinearParameterMapping:
         return LinearParameterMapping(
             self._params, self._params, dict(zip(self._params, self._params))
         )
 
-    def primitive_circuit(self) -> "UnboundParametricQuantumCircuitProtocol":
+    def primitive_circuit(self) -> "ImmutableUnboundParametricQuantumCircuit":
         return self.freeze()
 
     def get_mutable_copy(self) -> "UnboundParametricQuantumCircuit":
-        circuit = UnboundParametricQuantumCircuit(self.qubit_count)
+        circuit = UnboundParametricQuantumCircuit(self.qubit_count, self.cbit_count)
         circuit._gates = list(self._gates)
         return circuit
 
     def combine(
         self, gates: Union[GateSequence, "UnboundParametricQuantumCircuitBase"]
     ) -> "UnboundParametricQuantumCircuit":
         """Create a new parametric circuit with itself and the given gates or
         an unbound parametric circuit combined.
 
         All parameters in self and the other are treated as different
         ones. I.e. even if those two share the same instance of a
         parameter, it is copied into two independent parameters.
         """
-        circuit = UnboundParametricQuantumCircuit(self.qubit_count)
+        circuit = UnboundParametricQuantumCircuit(self.qubit_count, self.cbit_count)
         circuit.extend(self)
         circuit.extend(gates)
         return circuit
 
     @abstractmethod
     def freeze(self) -> "ImmutableUnboundParametricQuantumCircuit":
         ...
@@ -226,48 +240,78 @@
     def _params(self) -> Sequence[Parameter]:
         return [p for _, p in self._gates if p is not None]
 
     @property
     def parameter_count(self) -> int:
         return len(self._params)
 
+    def __add__(
+        self,
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
+    ) -> "UnboundParametricQuantumCircuit":
+        if isinstance(gates, UnboundParametricQuantumCircuitBase):
+            return self.combine(gates)
+        elif is_gate_sequence(gates):
+            return self.combine(gates)
+        else:
+            return NotImplemented
+
+    def __radd__(
+        self,
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
+    ) -> "UnboundParametricQuantumCircuit":
+        if isinstance(gates, UnboundParametricQuantumCircuitBase) or is_gate_sequence(
+            gates
+        ):
+            combined_circuit = UnboundParametricQuantumCircuit(self.qubit_count)
+            combined_circuit.extend(gates)
+            combined_circuit.extend(self)
+            return combined_circuit
+        else:
+            return NotImplemented
+
 
 class UnboundParametricQuantumCircuit(
     UnboundParametricQuantumCircuitBase,
     MutableUnboundParametricQuantumCircuitProtocol,
 ):
     """A mutable unbound parametric quantum circuit.
 
     This class is for parametric circuits where all parametric gates have independent
     parameters, i.e., no two parametric gates share the same parameter. If you want to
     make dependency between parameters, see
     :class:`~LinearMappedUnboundParametricQuantumCircuit`.
     """
 
-    def __init__(self, qubit_count: int):
+    def __init__(self, qubit_count: int, cbit_count: int = 0):
         self._qubit_count = qubit_count
         self._gates: list[
             Union[tuple[QuantumGate, None], tuple[ParametricQuantumGate, Parameter]]
         ] = []
+        self._cbit_count = cbit_count
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, UnboundParametricQuantumCircuitBase):
             return False
         return self.freeze() == other.freeze()
 
     @property
     def qubit_count(self) -> int:
         return self._qubit_count
 
+    @property
+    def cbit_count(self) -> int:
+        return self._cbit_count
+
     def add_gate(self, gate: QuantumGate, gate_index: Optional[int] = None) -> None:
         if max([*gate.control_indices, *gate.target_indices]) >= self.qubit_count:
             raise ValueError(
                 "The indices of the gate applied must be smaller than qubit_count"
             )
-        if gate_index:
+        if gate_index is not None:
             self._gates.insert(gate_index, (gate, None))
         else:
             self._gates.append((gate, None))
 
     def add_ParametricRX_gate(self, qubit_index: int) -> Parameter:
         """Add a parametric RX gate to the circuit."""
         if qubit_index >= self.qubit_count:
@@ -324,55 +368,77 @@
             self._gates.extend(gates._gates)
         else:
             if isinstance(gates, NonParametricQuantumCircuit):
                 gates = gates.gates
             for g in gates:
                 self.add_gate(g)
 
+    def __iadd__(
+        self,
+        gates: Union[GateSequence, UnboundParametricQuantumCircuitProtocol],
+    ) -> "UnboundParametricQuantumCircuit":
+        if isinstance(gates, UnboundParametricQuantumCircuitBase):
+            self.extend(gates)
+            return self
+        elif is_gate_sequence(gates):
+            self.extend(gates)
+            return self
+        else:
+            return NotImplemented
+
     def freeze(self) -> "ImmutableUnboundParametricQuantumCircuit":
         return ImmutableUnboundParametricQuantumCircuit(self)
 
 
 class ImmutableUnboundParametricQuantumCircuit(UnboundParametricQuantumCircuitBase):
     """An immutable unbound parametric quantum circuit.
 
     This class is for parametric circuits where all parametric gates have independent
     parameters, i.e., no two parametric gates share the same parameter. If you want to
     make dependency between parameters, see
     :class:`~ImmutableLinearMappedUnboundParametricQuantumCircuit`.
     """
 
-    def __init__(self, circuit: UnboundParametricQuantumCircuit):
+    def __init__(self, circuit: UnboundParametricQuantumCircuitBase):
         self._qubit_count = circuit.qubit_count
         self._gates = tuple(circuit._gates)
+        self._cbit_count = circuit.cbit_count
 
     def __eq__(self, other: object) -> bool:
         if not isinstance(other, UnboundParametricQuantumCircuitBase):
             return False
         f = other.freeze()
-        return (self.qubit_count, self._gates) == (f.qubit_count, f._gates)
+        return (self.qubit_count, self.cbit_count, self._gates) == (
+            f.qubit_count,
+            f.cbit_count,
+            f._gates,
+        )
 
     @property
     def qubit_count(self) -> int:
         return self._qubit_count
 
+    @property
+    def cbit_count(self) -> int:
+        return self._cbit_count
+
     def freeze(self) -> "ImmutableUnboundParametricQuantumCircuit":
         return self
 
 
 class ImmutableBoundParametricQuantumCircuit(ImmutableQuantumCircuit):
     """An immutable \"bound\" parametric quantum circuit, i.e. a parametric
     circuit with its parameters assigned concrete values."""
 
     def __init__(
         self,
         circuit: UnboundParametricQuantumCircuitBase,
         parameter_map: Mapping[Parameter, float],
     ):
-        super().__init__(QuantumCircuit(circuit.qubit_count))
+        super().__init__(QuantumCircuit(circuit.qubit_count, circuit.cbit_count))
         self.unbound_param_circuit = circuit.freeze()
         self.parameter_map = dict(parameter_map)
 
     @cached_property
     def gates(self) -> Sequence[QuantumGate]:
         def map_param_gate(
             gate: Union[QuantumGate, ParametricQuantumGate], param: Optional[Parameter]
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/clifford_gate.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/clifford_gate.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     Args:
         gate: A gate to be checked whether Clifford or not.
         rtol: The relative tolerance parameter determines how close the angle of
             rotation is to the angle in the Clifford angle set.
         atol: The absolute tolerance parameter determines how close the angle of
             rotation is to the angle in the Clifford angle set.
     """
-
     if gate.name in CLIFFORD_GATE_NAMES:
         return True
 
     elif gate.name in {"T", "Tdag"}:
         return False
 
     elif gate.name in {"RX", "RY", "RZ", "U1", "U2", "U3", "PauliRotation"}:
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/gate_names.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/gate_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
 Tdag: Literal["Tdag"] = "Tdag"
 RX: Literal["RX"] = "RX"
 RY: Literal["RY"] = "RY"
 RZ: Literal["RZ"] = "RZ"
 U1: Literal["U1"] = "U1"
 U2: Literal["U2"] = "U2"
 U3: Literal["U3"] = "U3"
+Measurement: Literal["Measurement"] = "Measurement"
 
 SINGLE_QUBIT_GATE_NAMES: set[SingleQubitGateNameType] = {
     Identity,
     X,
     Y,
     Z,
     H,
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/gates.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/gates.py`

 * *Files 4% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         )
 
 
 U2 = U2Factory()
 r"""U2 gate is a single-qubit rotation about X + Z axis:
 
 :math:`U_2(\phi, \lambda) = R_Z(\phi)R_Y(\pi/2)R_Z(\lambda)`.
-Represented by matrix :math:`\frac{1}{\sqrt{2}}\begin{pmatrix} 1 & e^{-i\lambda} \\
+Represented by matrix :math:`\frac{1}{\sqrt{2}}\begin{pmatrix} 1 & -e^{i\lambda} \\
 e^{i\phi} & e^{i(\phi+\lambda)} \end{pmatrix}`
 """
 
 
 class U3Factory:
     name: Literal["U3"] = gate_names.U3
 
@@ -271,17 +271,18 @@
         return QuantumGate(
             name=self.name, target_indices=(target_index,), params=(theta, phi, lmd)
         )
 
 
 U3 = U3Factory()
 r"""U3 gate is a generic single-qubit rotation gate with 3 Euler angles.
+
 Represented by matrix
 :math:`\begin{pmatrix}
-\cos\frac{\theta}{2} & -e^{-i\lambda}\sin\frac{\theta}{2} \\
+\cos\frac{\theta}{2} & -e^{i\lambda}\sin\frac{\theta}{2} \\
 e^{i\phi}\sin\frac{\theta}{2} & e^{i(\phi+\lambda)}\cos\frac{\theta}{2}
 \end{pmatrix}`
 """
 
 
 class CNOTFactory:
     name: Literal["CNOT"] = gate_names.CNOT
@@ -500,7 +501,29 @@
 ParametricPauliRotation = ParametricPauliRotationFactory()
 """Parametric Pauli rotation gate.
 
 Note that the instance of this class doesn't contain parameter values.
 Every parametric gate is carried with it's parameter
 (:class:`~Parameter`) such as (ParametricPauliRotation, Parameter).
 """
+
+
+class MeasurementFactory:
+    name: Literal["Measurement"] = gate_names.Measurement
+
+    def __call__(
+        self, target_indices: Sequence[int], classical_indices: Sequence[int]
+    ) -> QuantumGate:
+        if len(target_indices) != len(classical_indices):
+            raise ValueError(
+                "Number of qubits and classical bits must be same for measurement."
+            )
+        return QuantumGate(
+            name=self.name,
+            target_indices=tuple(target_indices),
+            classical_indices=tuple(classical_indices),
+        )
+
+
+Measurement = MeasurementFactory()
+r"""Measurement gate that transfers the measurement result to a classical
+bit."""
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/inverse_gate.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/inverse.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,15 +7,22 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping
 from typing import Callable, Union
 
-from quri_parts.circuit import gate_names, gates
+import numpy as np
+
+from quri_parts.circuit import (
+    NonParametricQuantumCircuit,
+    QuantumCircuit,
+    gate_names,
+    gates,
+)
 
 from .gate import QuantumGate
 from .gate_names import SingleQubitGateNameType, is_single_qubit_gate_name
 
 _single_qubit_gate_dagger: Mapping[
     SingleQubitGateNameType, Callable[[int], QuantumGate]
 ] = {
@@ -53,10 +60,32 @@
             inverse_gate = _single_qubit_gate_dagger[gate.name](*target_indices)
         elif gate.name in _rotation_gate_dagger:
             param = gate.params
             inv_param = tuple((-1 * i for i in param))
             inverse_gate = _rotation_gate_dagger[gate.name](*target_indices, *inv_param)
         else:
             inverse_gate = gate
+    elif gate.name == gate_names.PauliRotation:
+        pauli_ids = gate.pauli_ids
+        angle = gate.params[0]
+        neg_angle = -angle
+        inverse_gate = gates.PauliRotation(target_indices, pauli_ids, neg_angle)
+    elif gate.name == gate_names.UnitaryMatrix:
+        unitary = gate.unitary_matrix
+        inverse_unitary = np.array(unitary, dtype=np.complex128).conj().T
+        inverse_gate = gates.UnitaryMatrix(target_indices, inverse_unitary.tolist())
     else:
         inverse_gate = gate
     return inverse_gate
+
+
+def inverse_circuit(
+    circuit: NonParametricQuantumCircuit,
+) -> QuantumCircuit:
+    qubit_count = circuit.qubit_count
+
+    gates_inv = []
+    for gate in circuit.gates:
+        gates_inv.append(inverse_gate(gate))
+    gates_inv.reverse()
+
+    return QuantumCircuit(qubit_count, gates=gates_inv)
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/__init__.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_instruction.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/noise/noise_instruction.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/noise/noise_model.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/noise/noise_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import itertools as it
 from collections import defaultdict
 from collections.abc import Iterable, MutableMapping, MutableSequence, Sequence
+from typing import Callable, Optional
 
 from quri_parts.circuit import QuantumGate
 
 from .noise_instruction import (
     CircuitNoiseInstruction,
     GateNoiseInstruction,
     NoiseInstruction,
@@ -98,14 +99,18 @@
         noises: Sequence of :class:`NoiseInstruction`.
     """
 
     def __init__(self, noises: Sequence[NoiseInstruction] = []):
         self._id_to_index: MutableMapping[int, int] = {}
         self._index = 0
 
+        self._custom_gate_filters: MutableMapping[
+            int, Callable[[QuantumGate], bool]
+        ] = {}
+
         self._gate_noises_for_specified: MutableMapping[
             tuple[str, QubitIndices], MutableSequence[GateNoiseInstruction]
         ] = defaultdict(list)
         self._gate_noises_for_all_gates_specified_qubits: MutableMapping[
             QubitIndices, MutableSequence[GateNoiseInstruction]
         ] = defaultdict(list)
         self._gate_noises_for_all_qubits_specified_gates: MutableMapping[
@@ -211,24 +216,34 @@
         that match the given gate conditions in this noise model. The order of
         the list is the order in which :class:`NoiseInstructions` are added to
         the noise model.
 
         Args:
            gate: :class:`QuantumGate` to which noises are applied.
         """
-        return sorted(
-            it.chain(
-                self._get_gate_noises_for_all(gate, self._gate_noises_for_all),
-                self._get_gate_noises_for_all_qubits_specified_gates(gate),
-                self._get_gate_noises_for_all_gates_specified_qubits(gate),
-                self._get_gate_noises_for_specified(gate),
-            ),
-            key=lambda x: self._id_to_index[id(x[1])],
+        cpairs = it.chain(
+            self._get_gate_noises_for_all(gate, self._gate_noises_for_all),
+            self._get_gate_noises_for_all_qubits_specified_gates(gate),
+            self._get_gate_noises_for_all_gates_specified_qubits(gate),
+            self._get_gate_noises_for_specified(gate),
         )
 
+        if self._custom_gate_filters:
+            pairs = tuple(
+                filter(
+                    lambda pair: id(pair[1]) not in self._custom_gate_filters
+                    or self._custom_gate_filters[id(pair[1])](gate),
+                    cpairs,
+                )
+            )
+        else:
+            pairs = tuple(cpairs)
+
+        return sorted(pairs, key=lambda x: self._id_to_index[id(x[1])])
+
     def noises_for_circuit(self) -> Sequence[CircuitNoiseInstruction]:
         """Returns sequence of :class:`CircuitNoiseInstruction` in the
         model."""
         return self._circuit_noises
 
     def _add_gate_noise_for_all_gates_specified_qubits(
         self, noise: GateNoiseInstruction
@@ -281,20 +296,33 @@
                 self._gate_noises_for_specified[(gate, qubits)].append(noise)
 
     def _add_circuit_noise(self, noise: CircuitNoiseInstruction) -> None:
         """Add :class:`CircuitNoiseInstruction` to the internal data
         structure."""
         self._circuit_noises.append(noise)
 
-    def add_noise(self, noise: NoiseInstruction) -> None:
+    def add_noise(
+        self,
+        noise: NoiseInstruction,
+        custom_gate_filter: Optional[Callable[[QuantumGate], bool]] = None,
+    ) -> None:
         """Add single :class:`NoiseInstruction` to the model and update the
-        state of the model."""
+        state of the model.
+
+        Args:
+            noise: :class:`NoiseInstruction` to be added to the model.
+            custom_gate_filter: (If specified) Additional condition to determine
+                if the noise is applied to the target gate.
+        """
 
         self._id_to_index[id(noise)] = self._issue_index()
 
+        if custom_gate_filter is not None:
+            self._custom_gate_filters[id(noise)] = custom_gate_filter
+
         if isinstance(noise, GateNoiseInstruction):
             if (not noise.qubit_indices) and (not noise.target_gates):
                 self._add_gate_noise_for_all(noise)
             elif not noise.qubit_indices:
                 self._add_gate_noise_for_all_qubits_specified_gates(noise)
             elif not noise.target_gates:
                 self._add_gate_noise_for_all_gates_specified_qubits(noise)
@@ -326,16 +354,18 @@
             self._gate_noises_for_specified,
             self._gate_noises_for_all_gates_specified_qubits,
             self._gate_noises_for_all_qubits_specified_gates,
             self._gate_noises_for_all,
             self._circuit_noises,
             self._index,
             self._id_to_index,
+            self._custom_gate_filters,
         ) == (
             other._gate_noises_for_specified,
             other._gate_noises_for_all_gates_specified_qubits,
             other._gate_noises_for_all_qubits_specified_gates,
             other._gate_noises_for_all,
             other._circuit_noises,
             other._index,
             other._id_to_index,
+            other._custom_gate_filters,
         )
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/parameter.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_mapping.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/parameter_shift.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/parameter_shift.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/topology/__init__.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/topology/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/topology/square_lattice.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/topology/square_lattice.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/clifford_approximation.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/clifford_approximation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/gate_kind_decomposer.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/gate_kind_decomposer.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/identity_insertion.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/identity_manipulation.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,15 +4,20 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from quri_parts.circuit import NonParametricQuantumCircuit, QuantumCircuit, gates
+from quri_parts.circuit import (
+    NonParametricQuantumCircuit,
+    QuantumCircuit,
+    gate_names,
+    gates,
+)
 
 from .transpiler import CircuitTranspilerProtocol
 
 
 class IdentityInsertionTranspiler(CircuitTranspilerProtocol):
     """If there are qubits to which any gate has not been applied, Identity
     gates are added for those qubits.
@@ -32,7 +37,21 @@
                 return circuit
 
         cc = QuantumCircuit(circuit.qubit_count)
         cc.extend(circuit.gates)
         for q in non_applied:
             cc.add_gate(gates.Identity(q))
         return cc
+
+
+class IdentityEliminationTranspiler(CircuitTranspilerProtocol):
+    """Generate a new circuit by removing all Identity gates from the given
+    circuit."""
+
+    def __call__(
+        self, circuit: NonParametricQuantumCircuit
+    ) -> NonParametricQuantumCircuit:
+        ret = QuantumCircuit(circuit.qubit_count)
+        for gate in circuit.gates:
+            if gate.name != gate_names.Identity:
+                ret.add_gate(gate)
+        return ret
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/multi_pauli_decomposer.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/multi_pauli_decomposer.py`

 * *Files 0% similar despite different names*

```diff
@@ -67,15 +67,15 @@
                 elif pauli == 3:
                     pass
                 else:
                     raise ValueError("Pauli id must be either 1, 2, or 3.")
             return rc
 
         ret.extend(rot_gates(1))
-        for i in range(1, len(indices)):
+        for i in reversed(range(1, len(indices))):
             ret.append(gates.CNOT(indices[i], indices[0]))
         ret.append(gates.RZ(indices[0], angle))
         for i in range(1, len(indices)):
             ret.append(gates.CNOT(indices[i], indices[0]))
         ret.extend(rot_gates(-1))
 
         return ret
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/qubit_remapping.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/qubit_remapping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/transpile/transpiler.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/transpile/transpiler.py`

 * *Files 8% similar despite different names*

```diff
@@ -95,15 +95,16 @@
         cg: list[QuantumGate] = []
         for gate in circuit.gates:
             if self.is_target_gate(gate):
                 cg.extend(self.decompose(gate))
             else:
                 cg.append(gate)
 
-        cc = QuantumCircuit(circuit.qubit_count)
+        cc = QuantumCircuit(circuit.qubit_count, cbit_count=circuit.cbit_count)
+
         cc.extend(cg)
         return cc
 
 
 class GateKindDecomposer(GateDecomposer, ABC):
     """Abstract class that represents CircuitTranspiler, such that each gate is
     identified by its gate name and the target gate is replaced by a sequence
@@ -112,15 +113,15 @@
     Classes inheriting from this class can be used for
     ParallelDecomposer.
     """
 
     @property
     @abstractmethod
     def target_gate_names(self) -> Sequence[str]:
-        """Returns the set of gate names to be decomposed."."""
+        """Returns the set of gate names to be decomposed."""
         ...
 
     def is_target_gate(self, gate: QuantumGate) -> bool:
         return gate.name in self.target_gate_names
 
 
 class ParallelDecomposer(CircuitTranspilerProtocol):
@@ -149,10 +150,11 @@
         cg: list[QuantumGate] = []
         for gate in circuit.gates:
             if gate.name in self._decomposer_map:
                 cg.extend(self._decomposer_map[gate.name].decompose(gate))
             else:
                 cg.append(gate)
 
-        cc = QuantumCircuit(circuit.qubit_count)
+        cc = QuantumCircuit(circuit.qubit_count, cbit_count=circuit.cbit_count)
+
         cc.extend(cg)
         return cc
```

### Comparing `quri_parts_circuit-0.9.2/quri_parts/circuit/utils/controlled_rotations.py` & `quri_parts_circuit-17.0.0/quri_parts/circuit/utils/controlled_rotations.py`

 * *Files identical despite different names*

### Comparing `quri_parts_circuit-0.9.2/PKG-INFO` & `quri_parts_circuit-17.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-circuit
-Version: 0.9.2
+Version: 17.0.0
 Summary: Platform-independent quantum circuit library
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

