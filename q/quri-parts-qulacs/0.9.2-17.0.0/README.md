# Comparing `tmp/quri_parts_qulacs-0.9.2.tar.gz` & `tmp/quri_parts_qulacs-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_qulacs-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_qulacs-17.0.0.tar", max compression
```

## Comparing `quri_parts_qulacs-0.9.2.tar` & `quri_parts_qulacs-17.0.0.tar`

### file list

```diff
@@ -1,15 +1,17 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_qulacs-0.9.2/LICENSE
--rw-r--r--   0        0        0      351 2023-03-29 07:37:19.874951 quri_parts_qulacs-0.9.2/README.md
--rw-r--r--   0        0        0     1183 2023-03-29 07:37:34.699027 quri_parts_qulacs-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:33.911022 quri_parts_qulacs-0.9.2/quri_parts/qulacs/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/__init__.py
--rw-r--r--   0        0        0     6974 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/__init__.py
--rw-r--r--   0        0        0      661 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/__init__.py
--rw-r--r--   0        0        0     5609 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/circuit_converter.py
--rw-r--r--   0        0        0     1689 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/gate_converter.py
--rw-r--r--   0        0        0    11867 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/estimator.py
--rw-r--r--   0        0        0     1881 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/operator/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/py.typed
--rw-r--r--   0        0        0     6384 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/sampler.py
--rw-r--r--   0        0        0     1811 2023-03-29 07:37:19.878951 quri_parts_qulacs-0.9.2/quri_parts/qulacs/simulator.py
--rw-r--r--   0        0        0     1275 1970-01-01 00:00:00.000000 quri_parts_qulacs-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/LICENSE
+-rw-r--r--   0        0        0      351 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/README.md
+-rw-r--r--   0        0        0     1184 2024-03-19 02:11:33.021988 quri_parts_qulacs-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:32.437991 quri_parts_qulacs-17.0.0/quri_parts/qulacs/NOTICE
+-rw-r--r--   0        0        0     1117 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/__init__.py
+-rw-r--r--   0        0        0     9212 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/__init__.py
+-rw-r--r--   0        0        0     4838 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/compiled_circuit.py
+-rw-r--r--   0        0        0      661 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/__init__.py
+-rw-r--r--   0        0        0     5667 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/circuit_converter.py
+-rw-r--r--   0        0        0     2269 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/gate_converter.py
+-rw-r--r--   0        0        0    13690 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/estimator.py
+-rw-r--r--   0        0        0     1901 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/operator/__init__.py
+-rw-r--r--   0        0        0     5068 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/overlap_estimator.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/py.typed
+-rw-r--r--   0        0        0     8410 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/sampler.py
+-rw-r--r--   0        0        0     5541 2024-03-19 02:11:01.302138 quri_parts_qulacs-17.0.0/quri_parts/qulacs/simulator.py
+-rw-r--r--   0        0        0     1276 1970-01-01 00:00:00.000000 quri_parts_qulacs-17.0.0/PKG-INFO
```

### Comparing `quri_parts_qulacs-0.9.2/LICENSE` & `quri_parts_qulacs-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_qulacs-0.9.2/pyproject.toml` & `quri_parts_qulacs-17.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-qulacs"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use Qulacs with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/__init__.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/__init__.py`

 * *Files 27% similar despite different names*

```diff
@@ -5,17 +5,18 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping, Sequence
-from typing import Callable, Type
+from typing import Callable, Union, cast
 
 import qulacs
+from numpy.typing import ArrayLike
 from typing_extensions import assert_never
 
 from quri_parts.circuit import (
     LinearMappedUnboundParametricQuantumCircuitBase,
     NonParametricQuantumCircuit,
     QuantumGate,
     UnboundParametricQuantumCircuitBase,
@@ -32,101 +33,159 @@
     is_parametric_gate_name,
     is_single_qubit_gate_name,
     is_three_qubit_gate_name,
     is_two_qubit_gate_name,
     is_unitary_matrix_gate_name,
 )
 
+from .. import cast_to_list
+from .compiled_circuit import compile_circuit, compile_parametric_circuit
+
 _single_qubit_gate_qulacs: Mapping[
-    SingleQubitGateNameType, Type[qulacs.QuantumGateBase]
+    SingleQubitGateNameType, Callable[[int], qulacs.QuantumGateBase]
 ] = {
     gate_names.Identity: qulacs.gate.Identity,
     gate_names.X: qulacs.gate.X,
     gate_names.Y: qulacs.gate.Y,
     gate_names.Z: qulacs.gate.Z,
     gate_names.H: qulacs.gate.H,
     gate_names.S: qulacs.gate.S,
     gate_names.Sdag: qulacs.gate.Sdag,
     gate_names.SqrtX: qulacs.gate.sqrtX,
     gate_names.SqrtXdag: qulacs.gate.sqrtXdag,
     gate_names.SqrtY: qulacs.gate.sqrtY,
     gate_names.SqrtYdag: qulacs.gate.sqrtYdag,
     gate_names.T: qulacs.gate.T,
     gate_names.Tdag: qulacs.gate.Tdag,
-    gate_names.U1: qulacs.gate.U1,
-    gate_names.U2: qulacs.gate.U2,
-    gate_names.U3: qulacs.gate.U3,
 }
 
+
+def _u1_gate_qulacs(gate: QuantumGate) -> qulacs.QuantumGateBase:
+    return cast(
+        qulacs.QuantumGateBase,
+        qulacs.gate.U1(*gate.target_indices, *gate.params),
+    )
+
+
+def _u2_gate_qulacs(gate: QuantumGate) -> qulacs.QuantumGateBase:
+    return cast(
+        qulacs.QuantumGateBase,
+        qulacs.gate.U2(*gate.target_indices, *gate.params),
+    )
+
+
+def _u3_gate_qulacs(gate: QuantumGate) -> qulacs.QuantumGateBase:
+    return cast(
+        qulacs.QuantumGateBase,
+        qulacs.gate.U3(*gate.target_indices, *gate.params),
+    )
+
+
 _single_qubit_reverse_rotation_gate_qulacs: Mapping[
-    SingleQubitGateNameType, Type[qulacs.QuantumGateBase]
+    SingleQubitGateNameType, Callable[[int, float], qulacs.QuantumGateBase]
 ] = {
     gate_names.RX: qulacs.gate.RX,
     gate_names.RY: qulacs.gate.RY,
     gate_names.RZ: qulacs.gate.RZ,
 }
 
-_two_qubit_gate_qulacs: Mapping[TwoQubitGateNameType, Type[qulacs.QuantumGateBase]] = {
+_two_qubit_gate_qulacs: Mapping[
+    TwoQubitGateNameType, Callable[[int, int], qulacs.QuantumGateBase]
+] = {
     gate_names.CNOT: qulacs.gate.CNOT,
     gate_names.CZ: qulacs.gate.CZ,
     gate_names.SWAP: qulacs.gate.SWAP,
 }
 
 _three_qubit_gate_qulacs: Mapping[
-    ThreeQubitGateNameType, Type[qulacs.QuantumGateBase]
+    ThreeQubitGateNameType, Callable[[int, int, int], qulacs.QuantumGateBase]
 ] = {
     gate_names.TOFFOLI: qulacs.gate.TOFFOLI,
 }
 
 _multi_pauli_gate_qulacs: Mapping[
-    MultiQubitGateNameType, Type[qulacs.QuantumGateBase]
+    MultiQubitGateNameType,
+    Callable[[list[int], list[int]], qulacs.QuantumGateBase],
 ] = {
     gate_names.Pauli: qulacs.gate.Pauli,
+}
+
+_multi_pauli_rotation_gate_qulacs: Mapping[
+    MultiQubitGateNameType,
+    Callable[[list[int], list[int], float], qulacs.QuantumGateBase],
+] = {
     gate_names.PauliRotation: qulacs.gate.PauliRotation,
 }
 
 _parametric_gate_qulacs = {
     gate_names.ParametricRX: qulacs.gate.ParametricRX,
     gate_names.ParametricRY: qulacs.gate.ParametricRY,
     gate_names.ParametricRZ: qulacs.gate.ParametricRZ,
     gate_names.ParametricPauliRotation: qulacs.gate.ParametricPauliRotation,
 }
 
 
+def _dense_matrix_gate_qulacs(
+    t: Union[int, Sequence[int]], unitary_matrix: ArrayLike
+) -> qulacs.QuantumGateBase:
+    # We need to disable type check due to an error in qulacs type annotation
+    # https://github.com/qulacs/qulacs/issues/537
+    return cast(
+        qulacs.QuantumGateBase,
+        qulacs.gate.DenseMatrix(t, unitary_matrix),  # type: ignore
+    )
+
+
 def convert_gate(
     gate: QuantumGate,
 ) -> qulacs.QuantumGateBase:
     if not is_gate_name(gate.name):
         raise ValueError(f"Unknown gate name: {gate.name}")
 
     if is_single_qubit_gate_name(gate.name):
         if gate.name in _single_qubit_gate_qulacs:
             return _single_qubit_gate_qulacs[gate.name](
                 *gate.target_indices, *gate.params
             )
+        elif gate.name == gate_names.U1:
+            return _u1_gate_qulacs(gate)
+        elif gate.name == gate_names.U2:
+            return _u2_gate_qulacs(gate)
+        elif gate.name == gate_names.U3:
+            return _u3_gate_qulacs(gate)
         elif gate.name in _single_qubit_reverse_rotation_gate_qulacs:
             neg_params = (-p for p in gate.params)
             return _single_qubit_reverse_rotation_gate_qulacs[gate.name](
                 *gate.target_indices, *neg_params
             )
+        else:
+            assert False, "Unreachable"
     elif is_two_qubit_gate_name(gate.name):
         return _two_qubit_gate_qulacs[gate.name](
             *gate.control_indices, *gate.target_indices
         )
     elif is_three_qubit_gate_name(gate.name):
         return _three_qubit_gate_qulacs[gate.name](
             *gate.control_indices, *gate.target_indices
         )
     elif is_multi_qubit_gate_name(gate.name):
-        neg_params = (-p for p in gate.params)
-        return _multi_pauli_gate_qulacs[gate.name](
-            gate.target_indices, gate.pauli_ids, *neg_params
-        )
+        # These cast are workaround for too strict type annotation of Qulacs
+        target_indices = cast_to_list(gate.target_indices)
+        pauli_ids = cast_to_list(gate.pauli_ids)
+        if gate.name in _multi_pauli_gate_qulacs:
+            return _multi_pauli_gate_qulacs[gate.name](target_indices, pauli_ids)
+        elif gate.name in _multi_pauli_rotation_gate_qulacs:
+            neg_params = (-p for p in gate.params)
+            return _multi_pauli_rotation_gate_qulacs[gate.name](
+                target_indices, pauli_ids, *neg_params
+            )
+        else:
+            assert False, "Unreachable"
     elif is_unitary_matrix_gate_name(gate.name):
-        return qulacs.gate.DenseMatrix(gate.target_indices, gate.unitary_matrix)
+        return _dense_matrix_gate_qulacs(gate.target_indices, gate.unitary_matrix)
     elif is_parametric_gate_name(gate.name):
         raise ValueError("Parametric gates are not supported")
     else:
         # It seems that currently assert_never does not work here
         # assert_never(gate.name)
         assert False, "Unreachable"
 
@@ -168,22 +227,31 @@
             if gate.name == gate_names.ParametricRX:
                 qulacs_circuit.add_parametric_RX_gate(gate.target_indices[0], 0)
             elif gate.name == gate_names.ParametricRY:
                 qulacs_circuit.add_parametric_RY_gate(gate.target_indices[0], 0)
             elif gate.name == gate_names.ParametricRZ:
                 qulacs_circuit.add_parametric_RZ_gate(gate.target_indices[0], 0)
             elif gate.name == gate_names.ParametricPauliRotation:
+                # These cast are workaround for too strict type annotation of Qulacs
+                target_indices = cast_to_list(gate.target_indices)
+                pauli_ids = cast_to_list(gate.pauli_ids)
                 qulacs_circuit.add_parametric_multi_Pauli_rotation_gate(
-                    gate.target_indices, gate.pauli_ids, 0
+                    target_indices, pauli_ids, 0
                 )
             else:
                 assert_never(gate.name)
         else:
             assert isinstance(
                 gate, QuantumGate
             ), f"gate should be a QuantumGate. actual={gate}"
             qulacs_circuit.add_gate(convert_gate(gate))
 
     return qulacs_circuit, param_mapper
 
 
-__all__ = ["convert_gate", "convert_circuit", "convert_parametric_circuit"]
+__all__ = [
+    "convert_gate",
+    "convert_circuit",
+    "convert_parametric_circuit",
+    "compile_circuit",
+    "compile_parametric_circuit",
+]
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/__init__.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/circuit_converter.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/circuit_converter.py`

 * *Files 2% similar despite different names*

```diff
@@ -142,16 +142,17 @@
             *[ci.noises_for_gate(gate, i, circuit) for ci in resolvers],
         )
         for qubits, gate_noise in noises:
             qulacs_circuit.add_gate(convert_noise_to_gate(qubits, gate_noise))
 
     # Circuit noises for depth at the end of the circuit.
     depth_noises = []
+    max_depth = max(depths.values()) if depths else 0
     for q in range(circuit.qubit_count):
         for ci in resolvers:
             depth_noises.extend(
-                ci.noises_for_depth(q, range(depths[q], depth + 1), circuit)
+                ci.noises_for_depth(q, range(depths[q], max_depth + 1), circuit)
             )
     for qubits, gate_noise in depth_noises:
         qulacs_circuit.add_gate(convert_noise_to_gate(qubits, gate_noise))
 
     return qulacs_circuit
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/circuit/noise/gate_converter.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/circuit/noise/gate_converter.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,40 +5,58 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Sequence
+from typing import cast
 
 from qulacs import QuantumGateBase
-from qulacs.gate import CPTP, DenseMatrix, Identity, Pauli, Probabilistic
+from qulacs.gate import CPTP, Identity, Pauli, Probabilistic
 
 from quri_parts.circuit.noise import AbstractKrausNoise, PauliNoise, ProbabilisticNoise
+from quri_parts.qulacs import cast_to_list
+from quri_parts.qulacs.circuit import _dense_matrix_gate_qulacs
 
 
 def create_kraus_gate(
     qubits: Sequence[int], noise: AbstractKrausNoise
 ) -> QuantumGateBase:
-    return CPTP([DenseMatrix(qubits, kraus) for kraus in noise.kraus_operators])
+    # This casting is for dealing with missing type of CPTP
+    return cast(
+        QuantumGateBase,
+        CPTP(
+            [
+                _dense_matrix_gate_qulacs(qubits, kraus)
+                for kraus in noise.kraus_operators
+            ]
+        ),
+    )
 
 
 def create_pauli_noise_gate(
     qubits: Sequence[int], noise: PauliNoise
 ) -> QuantumGateBase:
     qubits = noise.qubit_indices
     pauli_list, prob_list = noise.pauli_list, list(noise.prob_list)
 
-    pauli_gates = [Pauli(qubits, pauli) for pauli in pauli_list]
+    pauli_gates = [
+        Pauli(cast_to_list(qubits), cast_to_list(pauli)) for pauli in pauli_list
+    ]
     if sum(prob_list) < 1.0:
         pauli_gates.append(Identity(len(qubits)))
         prob_identity = 1.0 - sum(prob_list)
         prob_list.append(prob_identity)
 
-    return Probabilistic(prob_list, pauli_gates)
+    # This casting is for dealing with missing type of Probabilistic
+    return cast(QuantumGateBase, Probabilistic(cast_to_list(prob_list), pauli_gates))
 
 
 def create_probabilistic_gate(
     qubits: Sequence[int], noise: ProbabilisticNoise
 ) -> QuantumGateBase:
-    dense_matrices = [DenseMatrix(qubits, matrix) for matrix in noise.gate_matrices]
-    return Probabilistic(noise.prob_list, dense_matrices)
+    dense_matrices = [
+        _dense_matrix_gate_qulacs(qubits, matrix) for matrix in noise.gate_matrices
+    ]
+    # This casting is for dealing with missing type of Probabilistic
+    return cast(QuantumGateBase, Probabilistic(list(noise.prob_list), dense_matrices))
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/estimator.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/estimator.py`

 * *Files 19% similar despite different names*

```diff
@@ -8,72 +8,66 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Collection, Iterable, Sequence
 from typing import TYPE_CHECKING, Any, Callable, NamedTuple, Optional, Union
 
 import qulacs
-from typing_extensions import TypeAlias
 
 from quri_parts.circuit.noise import NoiseModel
 from quri_parts.core.estimator import (
     ConcurrentParametricQuantumEstimator,
     ConcurrentQuantumEstimator,
     Estimatable,
     Estimate,
+    GeneralQuantumEstimator,
     ParametricQuantumEstimator,
     QuantumEstimator,
     create_parametric_estimator,
 )
 from quri_parts.core.operator import zero
-from quri_parts.core.state import (
-    CircuitQuantumState,
-    ParametricCircuitQuantumState,
-    ParametricQuantumStateVector,
-    QuantumStateVector,
-)
+from quri_parts.core.state import ParametricQuantumStateVector, QuantumStateVector
 from quri_parts.core.utils.concurrent import execute_concurrently
+from quri_parts.qulacs import QulacsParametricStateT, QulacsStateT
+from quri_parts.qulacs.circuit.compiled_circuit import (
+    _QulacsCircuit,
+    _QulacsLinearMappedUnboundParametricCircuit,
+    _QulacsUnboundParametricCircuit,
+)
 
+from . import cast_to_list
 from .circuit import convert_circuit, convert_parametric_circuit
 from .circuit.noise import convert_circuit_with_noise_model
 from .operator import convert_operator
 
 if TYPE_CHECKING:
     from concurrent.futures import Executor
 
 
 class _Estimate(NamedTuple):
     value: complex
     error: float = 0.0
 
 
-#: A type alias for state classes supported by Qulacs estimators.
-#: Qulacs estimators support both of circuit states and state vectors.
-QulacsStateT: TypeAlias = Union[CircuitQuantumState, QuantumStateVector]
-
-#: A type alias for parametric state classes supported by Qulacs estimators.
-#: Qulacs estimators support both of circuit states and state vectors.
-QulacsParametricStateT: TypeAlias = Union[
-    ParametricCircuitQuantumState, ParametricQuantumStateVector
-]
-
-
 def _create_qulacs_initial_state(
     state: Union[QulacsStateT, QulacsParametricStateT]
 ) -> qulacs.QuantumState:
     qs_state = qulacs.QuantumState(state.qubit_count)
     if isinstance(state, (QuantumStateVector, ParametricQuantumStateVector)):
-        qs_state.load(state.vector)
+        qs_state.load(cast_to_list(state.vector))
     return qs_state
 
 
 def _estimate(operator: Estimatable, state: QulacsStateT) -> Estimate[complex]:
     if operator == zero():
         return _Estimate(value=0.0)
-    circuit = convert_circuit(state.circuit)
+    if isinstance(state.circuit, _QulacsCircuit):
+        circuit = state.circuit._qulacs_circuit
+    else:
+        circuit = convert_circuit(state.circuit)
     qs_state = _create_qulacs_initial_state(state)
     op = convert_operator(operator, state.qubit_count)
     circuit.update_quantum_state(qs_state)
     exp = op.get_expectation_value(qs_state)
     return _Estimate(value=exp)
 
 
@@ -89,15 +83,18 @@
 ) -> Sequence[Estimate[complex]]:
     return [_estimate(operator, state) for operator, state in op_state_tuples]
 
 
 def _sequential_estimate_single_state(
     state: QulacsStateT, operators: Sequence[Estimatable]
 ) -> Sequence[Estimate[complex]]:
-    circuit = convert_circuit(state.circuit)
+    if isinstance(state.circuit, _QulacsCircuit):
+        circuit = state.circuit._qulacs_circuit
+    else:
+        circuit = convert_circuit(state.circuit)
     n_qubits = state.qubit_count
     qs_state = _create_qulacs_initial_state(state)
     circuit.update_quantum_state(qs_state)
     results = []
     for op in operators:
         qs_op = convert_operator(op, n_qubits)
         results.append(_Estimate(value=qs_op.get_expectation_value(qs_state)))
@@ -173,15 +170,24 @@
     op_state: tuple[Estimatable, QulacsParametricStateT],
     params: Sequence[Sequence[float]],
 ) -> Sequence[Estimate[complex]]:
     operator, state = op_state
     n_qubits = state.qubit_count
     op = convert_operator(operator, n_qubits)
     parametric_circuit = state.parametric_circuit
-    qulacs_circuit, param_mapper = convert_parametric_circuit(parametric_circuit)
+    if isinstance(
+        parametric_circuit,
+        (_QulacsLinearMappedUnboundParametricCircuit, _QulacsUnboundParametricCircuit),
+    ):
+        qulacs_circuit, param_mapper = (
+            parametric_circuit.qulacs_circuit,
+            parametric_circuit.param_mapper,
+        )
+    else:
+        qulacs_circuit, param_mapper = convert_parametric_circuit(parametric_circuit)
 
     estimates = []
     for param in params:
         for i, v in enumerate(param_mapper(param)):
             qulacs_circuit.set_parameter(i, v)
         qs_state = _create_qulacs_initial_state(state)
         qulacs_circuit.update_quantum_state(qs_state)
@@ -232,15 +238,15 @@
         operator: Estimatable, state: QulacsStateT
     ) -> Estimate[complex]:
         if operator == zero():
             return _Estimate(value=0.0)
         circuit = convert_circuit_with_noise_model(state.circuit, model)
         qs_state = qulacs.DensityMatrix(state.qubit_count)
         if isinstance(state, QuantumStateVector):
-            qs_state.load(state.vector)
+            qs_state.load(cast_to_list(state.vector))
         op = convert_operator(operator, state.qubit_count)
         circuit.update_quantum_state(qs_state)
         exp = op.get_expectation_value(qs_state)
         return _Estimate(value=exp)
 
     return _estimate_with_noise
 
@@ -268,15 +274,15 @@
     def _estimate_single_state_sequentially(
         state: QulacsStateT, operators: Sequence[Estimatable]
     ) -> Sequence[Estimate[complex]]:
         circuit = convert_circuit_with_noise_model(state.circuit, model)
         qubit_count = state.qubit_count
         qs_state = qulacs.DensityMatrix(qubit_count)
         if isinstance(state, QuantumStateVector):
-            qs_state.load(state.vector)
+            qs_state.load(cast_to_list(state.vector))
         circuit.update_quantum_state(qs_state)
         results = []
         for op in operators:
             qs_op = convert_operator(op, qubit_count)
             results.append(_Estimate(value=qs_op.get_expectation_value(qs_state)))
         return results
 
@@ -314,15 +320,15 @@
 
         estimates = []
         for param in params:
             circuit = parametric_circuit.bind_parameters(param)
             qs_circuit = convert_circuit_with_noise_model(circuit, model)
             qs_state = qulacs.DensityMatrix(qubit_count)
             if isinstance(state, (QuantumStateVector, ParametricQuantumStateVector)):
-                qs_state.load(state.vector)
+                qs_state.load(cast_to_list(state.vector))
             qs_circuit.update_quantum_state(qs_state)
             exp = op.get_expectation_value(qs_state)
             estimates.append(_Estimate(value=exp))
 
         return estimates
 
     def estimator(
@@ -335,7 +341,43 @@
             (operator, state),
             params,
             executor,
             concurrency,
         )
 
     return estimator
+
+
+def create_qulacs_general_vector_estimator(
+    executor: Optional["Executor"] = None, concurrency: int = 1
+) -> GeneralQuantumEstimator[QulacsStateT, QulacsParametricStateT]:
+    """Creates a Qulacs general vector estimator."""
+    concurrent_param_estimator = create_qulacs_vector_concurrent_parametric_estimator(
+        executor, concurrency
+    )
+    return GeneralQuantumEstimator(
+        estimator=create_qulacs_vector_estimator(),
+        concurrent_estimator=create_qulacs_vector_concurrent_estimator(
+            executor, concurrency
+        ),
+        parametric_estimator=create_qulacs_vector_parametric_estimator(),
+        concurrent_parametric_estimator=concurrent_param_estimator,
+    )
+
+
+def create_qulacs_general_density_matrix_estimator(
+    model: NoiseModel, executor: Optional["Executor"] = None, concurrency: int = 1
+) -> GeneralQuantumEstimator[QulacsStateT, QulacsParametricStateT]:
+    """Creates a Qulacs general density estimator."""
+    # cp_estimator: abbreviation of concurrent parametric estimator
+    cp_estimator = create_qulacs_density_matrix_concurrent_parametric_estimator(
+        model, executor, concurrency
+    )
+
+    return GeneralQuantumEstimator(
+        estimator=create_qulacs_density_matrix_estimator(model),
+        concurrent_estimator=create_qulacs_density_matrix_concurrent_estimator(
+            model, executor, concurrency
+        ),
+        parametric_estimator=create_qulacs_density_matrix_parametric_estimator(model),
+        concurrent_parametric_estimator=cp_estimator,
+    )
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/operator/__init__.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/operator/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 def convert_operator(
     operator: Union[Operator, PauliLabel], n_qubits: int
 ) -> GeneralQuantumOperator:
     """Convert an :class:`~Operator` or a :class:`~PauliLabel` to a
     :class:`qulacs.GeneralQuantumOperator`."""
     op_key: _OperatorKey
     if isinstance(operator, PauliLabel):
-        op_key = operator
+        op_key = frozenset({(operator, 1.0)})
     else:
         op_key = frozenset(operator.items())
     if (op_key, n_qubits) in _operator_cache:
         return _operator_cache[(op_key, n_qubits)]
 
     op = GeneralQuantumOperator(n_qubits)
     paulis: Iterable[tuple[PauliLabel, complex]]
```

### Comparing `quri_parts_qulacs-0.9.2/quri_parts/qulacs/sampler.py` & `quri_parts_qulacs-17.0.0/quri_parts/qulacs/sampler.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,36 +15,46 @@
 import numpy as np
 import qulacs
 from numpy.random import default_rng
 
 from quri_parts.circuit import NonParametricQuantumCircuit
 from quri_parts.circuit.noise import NoiseModel
 from quri_parts.core.sampling import ConcurrentSampler, MeasurementCounts, Sampler
+from quri_parts.core.state import GeneralCircuitQuantumState
 from quri_parts.core.utils.concurrent import execute_concurrently
 
-from .circuit import convert_circuit
 from .circuit.noise import convert_circuit_with_noise_model
+from .simulator import (
+    create_qulacs_ideal_vector_state_sampler,
+    create_qulacs_vector_state_sampler,
+)
 
 if TYPE_CHECKING:
     from concurrent.futures import Executor
 
+_state_vector_sampler = create_qulacs_vector_state_sampler()
+_ideal_vector_sampler = create_qulacs_ideal_vector_state_sampler()
+
 
 def _sample(circuit: NonParametricQuantumCircuit, shots: int) -> MeasurementCounts:
-    qs_circuit = convert_circuit(circuit)
-    qs_state = qulacs.QuantumState(circuit.qubit_count)
-    qs_circuit.update_quantum_state(qs_state)
-
-    if shots > 2 ** max(qs_state.get_qubit_count(), 10):
-        # Use multinomial distribution for faster sampling
-        probs = np.abs(qs_state.get_vector()) ** 2
-        rng = default_rng()
-        counts = rng.multinomial(shots, probs)
-        return dict(((i, count) for i, count in enumerate(counts) if count > 0))
-    else:
-        return Counter(qs_state.sampling(shots))
+    state = GeneralCircuitQuantumState(circuit.qubit_count, circuit)
+    return _state_vector_sampler(state, shots)
+
+
+def _ideal_sample(
+    circuit: NonParametricQuantumCircuit, shots: int
+) -> MeasurementCounts:
+    state = GeneralCircuitQuantumState(circuit.qubit_count, circuit)
+    return _ideal_vector_sampler(state, shots)
+
+
+def create_qulacs_vector_ideal_sampler() -> Sampler:
+    """Returns a :class:`~Sampler` that uses Qulacs vector simulator for
+    returning the probabilities multiplied by the specific shot count."""
+    return _ideal_sample
 
 
 def create_qulacs_vector_sampler() -> Sampler:
     """Returns a :class:`~Sampler` that uses Qulacs vector simulator for
     sampling."""
     return _sample
 
@@ -120,14 +130,49 @@
             return dict((i, count) for i, count in enumerate(counts) if count > 0)
         else:
             return Counter(state.sampling(shots))
 
     return _sample_with_noise
 
 
+def create_qulacs_density_matrix_ideal_sampler(model: NoiseModel) -> Sampler:
+    """Returns a :class:`~Sampler` that uses Qulacs simulator using density
+    matrix with noise model and provides the exact probabilities multiplied
+    with the shot count."""
+
+    def _sample_with_noise(
+        circuit: NonParametricQuantumCircuit, shots: int
+    ) -> MeasurementCounts:
+        qubit_count = circuit.qubit_count
+        qs_circuit = convert_circuit_with_noise_model(circuit, model)
+        state = qulacs.DensityMatrix(qubit_count)
+        qs_circuit.update_quantum_state(state)
+
+        probs = list(np.abs(np.diag(state.get_matrix())))  # type: ignore
+        return {i: prob * shots for i, prob in enumerate(probs)}
+
+    return _sample_with_noise
+
+
+def create_qulacs_noisesimulator_sampler(model: NoiseModel) -> Sampler:
+    """Returns a :class:`~Sampler` that uses Qulacs NoiseSimulator."""
+
+    def _sample_with_noise(
+        circuit: NonParametricQuantumCircuit, shots: int
+    ) -> MeasurementCounts:
+        qubit_count = circuit.qubit_count
+        qs_circuit = convert_circuit_with_noise_model(circuit, model)
+        state = qulacs.QuantumState(qubit_count)
+        sim = qulacs.NoiseSimulator(qs_circuit, state)
+
+        return Counter(sim.execute(shots))
+
+    return _sample_with_noise
+
+
 def _create_qulacs_concurrent_sampler_with_noise_model(
     sampler_creator: Callable[[NoiseModel], Sampler],
     model: NoiseModel,
     executor: Optional["Executor"],
     concurrency: int,
 ) -> ConcurrentSampler:
     noise_sampler = sampler_creator(model)
@@ -175,7 +220,23 @@
 
     return _create_qulacs_concurrent_sampler_with_noise_model(
         create_qulacs_stochastic_state_vector_sampler,
         model,
         executor,
         concurrency,
     )
+
+
+def create_qulacs_noisesimulator_concurrent_sampler(
+    model: NoiseModel,
+    executor: Optional["Executor"] = None,
+    concurrency: int = 1,
+) -> ConcurrentSampler:
+    """Returns a :class:`~ConcurrentSampler` that uses Qulacs
+    NoiseSimulator."""
+
+    return _create_qulacs_concurrent_sampler_with_noise_model(
+        create_qulacs_noisesimulator_sampler,
+        model,
+        executor,
+        concurrency,
+    )
```

### Comparing `quri_parts_qulacs-0.9.2/PKG-INFO` & `quri_parts_qulacs-17.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-qulacs
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use Qulacs with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<4.0.0
```

