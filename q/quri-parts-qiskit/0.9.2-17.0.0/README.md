# Comparing `tmp/quri_parts_qiskit-0.9.2.tar.gz` & `tmp/quri_parts_qiskit-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_qiskit-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_qiskit-17.0.0.tar", max compression
```

## Comparing `quri_parts_qiskit-0.9.2.tar` & `quri_parts_qiskit-17.0.0.tar`

### file list

```diff
@@ -1,10 +1,19 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/LICENSE
--rw-r--r--   0        0        0      260 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/README.md
--rw-r--r--   0        0        0     1090 2023-03-29 07:37:33.795022 quri_parts_qiskit-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:33.011017 quri_parts_qiskit-0.9.2/quri_parts/qiskit/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/__init__.py
--rw-r--r--   0        0        0      724 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/__init__.py
--rw-r--r--   0        0        0     7241 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/sampling.py
--rw-r--r--   0        0        0     6341 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_qiskit-0.9.2/quri_parts/qiskit/py.typed
--rw-r--r--   0        0        0     1137 1970-01-01 00:00:00.000000 quri_parts_qiskit-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.298138 quri_parts_qiskit-17.0.0/LICENSE
+-rw-r--r--   0        0        0      260 2024-03-19 02:11:01.298138 quri_parts_qiskit-17.0.0/README.md
+-rw-r--r--   0        0        0     1243 2024-03-19 02:11:31.665995 quri_parts_qiskit-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0      251 2024-03-19 02:11:31.081998 quri_parts_qiskit-17.0.0/quri_parts/qiskit/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/__init__.py
+-rw-r--r--   0        0        0     1759 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/__init__.py
+-rw-r--r--   0        0        0      973 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/connectivity.py
+-rw-r--r--   0        0        0    17114 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/primitive.py
+-rw-r--r--   0        0        0     7789 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/sampling.py
+-rw-r--r--   0        0        0    10338 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/saved_sampling.py
+-rw-r--r--   0        0        0     2881 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/tracker.py
+-rw-r--r--   0        0        0     5992 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/utils.py
+-rw-r--r--   0        0        0      869 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/circuit/__init__.py
+-rw-r--r--   0        0        0     6578 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/circuit/circuit_converter.py
+-rw-r--r--   0        0        0     4456 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/circuit/qiskit_circuit_converter.py
+-rw-r--r--   0        0        0     3331 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/circuit/transpile/__init__.py
+-rw-r--r--   0        0        0     1923 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/operator/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.302138 quri_parts_qiskit-17.0.0/quri_parts/qiskit/py.typed
+-rw-r--r--   0        0        0     1272 1970-01-01 00:00:00.000000 quri_parts_qiskit-17.0.0/PKG-INFO
```

### Comparing `quri_parts_qiskit-0.9.2/LICENSE` & `quri_parts_qiskit-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_qiskit-0.9.2/pyproject.toml` & `quri_parts_qiskit-17.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-qiskit"
-version = "0.9.2"
+version = "17.0.0"
 description = "A plugin to use Qiskit with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
@@ -24,18 +24,23 @@
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
 python = "^3.9.8"
 numpy = ">=1.22.0"
 quri-parts-circuit = "*"
-qiskit = "^0.39.4"
+quri-parts-core = "*"
+qiskit = ">=0.41.1,<1"
+qiskit-ibm-runtime = ">=0.9.0,<1"
+pydantic = ">=1.9,<2.0"
+networkx = "*"
 
 [tool.poetry.group.dev.dependencies]
 quri-parts-circuit = {path = "../circuit", develop = true}
+quri-parts-core = {path = "../core", develop = true}
 
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
 mypy = ">=0.950"
 docformatter = "^1.4"
 isort = "^5.10.1"
 black = "^23.1.0"
```

### Comparing `quri_parts_qiskit-0.9.2/quri_parts/qiskit/backend/sampling.py` & `quri_parts_qiskit-17.0.0/quri_parts/qiskit/backend/sampling.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,55 +4,59 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from collections.abc import Mapping, MutableMapping
-from typing import Any, Optional
+from collections.abc import Mapping
+from typing import Any, Optional, Sequence
 
 import qiskit
 from qiskit.providers import Job
-from qiskit.providers.backend import Backend, BackendV1, BackendV2
+from qiskit.providers.backend import Backend
 from qiskit.result import Result
 
 from quri_parts.backend import (
     BackendError,
     CompositeSamplingJob,
     SamplingBackend,
     SamplingCounts,
     SamplingJob,
     SamplingResult,
 )
-from quri_parts.backend.qubit_mapping import BackendQubitMapping, QubitMappedSamplingJob
 from quri_parts.circuit import NonParametricQuantumCircuit
-from quri_parts.circuit.transpile import CircuitTranspiler, SequentialTranspiler
-from quri_parts.qiskit.circuit import (
-    QiskitCircuitConverter,
-    QiskitTranspiler,
-    convert_circuit,
+from quri_parts.circuit.transpile import CircuitTranspiler
+from quri_parts.qiskit.circuit import QiskitCircuitConverter, convert_circuit
+
+from .saved_sampling import (
+    QiskitSavedDataSamplingJob,
+    QiskitSavedDataSamplingResult,
+    encode_saved_data_job_sequence_to_json,
+)
+from .utils import (
+    convert_qiskit_sampling_count_to_qp_sampling_count,
+    distribute_backend_shots,
+    get_backend_min_max_shot,
+    get_job_mapper_and_circuit_transpiler,
 )
 
 
 class QiskitSamplingResult(SamplingResult):
     """A result of a Qiskit sampling job."""
 
     def __init__(self, qiskit_result: Result):
         if not isinstance(qiskit_result, Result):
             raise ValueError("Only qiskit.result.Result is supported")
         self._qiskit_result = qiskit_result
 
     @property
     def counts(self) -> SamplingCounts:
         qiskit_counts = self._qiskit_result.get_counts()
-        measurements: MutableMapping[int, int] = {}
-        for result in qiskit_counts:
-            measurements[int(result, 2)] = qiskit_counts[result]
-        return measurements
+        return convert_qiskit_sampling_count_to_qp_sampling_count(qiskit_counts)
 
 
 class QiskitSamplingJob(SamplingJob):
     """A job for a Qiskit sampling measurement."""
 
     def __init__(self, qiskit_job: Job):
         self._qiskit_job = qiskit_job
@@ -68,15 +72,15 @@
     Args:
         backend: A Qiskit :class:`qiskit.providers.backend.Backend`
             for circuit execution.
         circuit_converter: A function converting
             :class:`~quri_parts.circuit.NonParametricQuantumCircuit` to
             a Qiskit :class:`qiskit.circuit.QuantumCircuit`.
         circuit_transpiler: A transpiler applied to the circuit before running it.
-            :class:`~QiskitTranspiler` is used when not specified.
+            :class:`~QiskitSetTranspiler` is used when not specified.
         enable_shots_roundup: If True, when a number of shots specified to
             :meth:`~sample` is smaller than the minimum number of shots supported by
             the device, it is rounded up to the minimum. In this case, it is possible
             that shots more than specified are used. If it is strictly not allowed to
             exceed the specified shot count, set this argument to False.
         qubit_mapping: If specified, indices of qubits in the circuit are remapped
             before running it on the backend. It can be used when you want to use
@@ -84,92 +88,109 @@
             The mapping should be specified with "from" qubit
             indices as keys and "to" qubit indices as values. For example, if
             you want to map qubits 0, 1, 2, 3 to backend qubits as 0 → 4, 1 → 2,
             2 → 5, 3 → 0, then the ``qubit_mapping`` should be
             ``{0: 4, 1: 2, 2: 5, 3: 0}``.
         run_kwargs: Additional keyword arguments for
             :meth:`qiskit.providers.backend.Backend.run` method.
+        save_data_while_sampling: If True, the circuit, n_shots and the
+            sampling counts will be saved. Please use the `.jobs` or `.jobs_json`
+            to access the saved data.
     """
 
     def __init__(
         self,
         backend: Backend,
         circuit_converter: QiskitCircuitConverter = convert_circuit,
         circuit_transpiler: Optional[CircuitTranspiler] = None,
         enable_shots_roundup: bool = True,
         qubit_mapping: Optional[Mapping[int, int]] = None,
         run_kwargs: Mapping[str, Any] = {},
+        save_data_while_sampling: bool = False,
     ):
         self._backend = backend
+
+        # circuit related
         self._circuit_converter = circuit_converter
 
-        self._qubit_mapping = None
-        if qubit_mapping is not None:
-            self._qubit_mapping = BackendQubitMapping(qubit_mapping)
-
-        if circuit_transpiler is None:
-            circuit_transpiler = QiskitTranspiler()
-        if self._qubit_mapping:
-            circuit_transpiler = SequentialTranspiler(
-                [circuit_transpiler, self._qubit_mapping.circuit_transpiler]
-            )
-        self._circuit_transpiler = circuit_transpiler
+        (
+            self._job_mapper,
+            self._circuit_transpiler,
+        ) = get_job_mapper_and_circuit_transpiler(qubit_mapping, circuit_transpiler)
 
+        # shots related
         self._enable_shots_roundup = enable_shots_roundup
-        self._run_kwargs = run_kwargs
+        self._min_shots, self._max_shots = get_backend_min_max_shot(backend)
 
-        self._min_shots = 1
-        self._max_shots: Optional[int] = None
-        if isinstance(backend, BackendV1):
-            max_shots = backend.configuration().max_shots
-            if max_shots > 0:
-                self._max_shots = max_shots
+        # other kwargs
+        self._run_kwargs = run_kwargs
 
-        if not isinstance(backend, (BackendV1, BackendV2)):
-            raise BackendError("Backend not supported.")
+        # saving mode
+        self._save_data_while_sampling = save_data_while_sampling
+        self._saved_data: list[tuple[str, int, QiskitSamplingJob]] = []
 
     def sample(self, circuit: NonParametricQuantumCircuit, n_shots: int) -> SamplingJob:
         if not n_shots >= 1:
             raise ValueError("n_shots should be a positive integer.")
-        if self._max_shots is not None and n_shots > self._max_shots:
-            shot_dist = [self._max_shots] * (n_shots // self._max_shots)
-            remaining = n_shots % self._max_shots
-            if remaining >= self._min_shots or self._enable_shots_roundup:
-                shot_dist.append(max(remaining, self._min_shots))
-        else:
-            if n_shots >= self._min_shots or self._enable_shots_roundup:
-                shot_dist = [max(n_shots, self._min_shots)]
-            else:
-                raise ValueError(
-                    f"n_shots is smaller than minimum shot count ({self._min_shots}) "
-                    "supported by the device. Try larger n_shots or use "
-                    "enable_shots_roundup=True when creating the backend."
-                )
+
+        shot_dist = distribute_backend_shots(
+            n_shots, self._min_shots, self._max_shots, self._enable_shots_roundup
+        )
 
         qiskit_circuit = self._circuit_converter(circuit, self._circuit_transpiler)
         qiskit_circuit.measure_all()
-        qiskit_jobs = []
+        transpiled_circuit = qiskit.transpile(qiskit_circuit, self._backend)
+        circuit_qasm_str = transpiled_circuit.qasm()
+
+        jobs: list[QiskitSamplingJob] = []
         try:
             for s in shot_dist:
-                qiskit_jobs.append(
-                    self._backend.run(
-                        qiskit.transpile(qiskit_circuit, self._backend),
-                        shots=s,
-                        **self._run_kwargs,
-                    )
+                qiskit_job = self._backend.run(
+                    transpiled_circuit,
+                    shots=s,
+                    **self._run_kwargs,
                 )
+                qiskit_sampling_job = QiskitSamplingJob(qiskit_job)
+                # Saving mode
+                if self._save_data_while_sampling:
+                    self._saved_data.append((circuit_qasm_str, s, qiskit_sampling_job))
+                jobs.append(qiskit_sampling_job)
+
         except Exception as e:
-            for j in qiskit_jobs:
+            for qiskit_sampling_job in jobs:
                 try:
-                    j.cancel()
+                    qiskit_sampling_job._qiskit_job.cancel()
                 except Exception:
                     # Ignore cancel errors
                     pass
             raise BackendError("Qiskit Device.run failed.") from e
 
-        jobs: list[SamplingJob] = [QiskitSamplingJob(j) for j in qiskit_jobs]
-        if self._qubit_mapping is not None:
-            jobs = [QubitMappedSamplingJob(job, self._qubit_mapping) for job in jobs]
-        if len(jobs) == 1:
-            return jobs[0]
-        else:
-            return CompositeSamplingJob(jobs)
+        qubit_mapped_jobs = [self._job_mapper(job) for job in jobs]
+        return (
+            qubit_mapped_jobs[0]
+            if len(qubit_mapped_jobs) == 1
+            else CompositeSamplingJob(qubit_mapped_jobs)
+        )
+
+    @property
+    def jobs(self) -> Sequence[QiskitSavedDataSamplingJob]:
+        """Convert saved data to a list of QiskitSavedDataSamplingJob
+        objects."""
+        job_list = []
+        for circuit_qasm_str, n_shots, qiskit_sampling_job in self._saved_data:
+            raw_measurement_cnt = qiskit_sampling_job._qiskit_job.result().get_counts()
+            saved_sampling_result = QiskitSavedDataSamplingResult(
+                raw_data=raw_measurement_cnt
+            )
+            saved_sampling_job = QiskitSavedDataSamplingJob(
+                circuit_qasm=circuit_qasm_str,
+                n_shots=n_shots,
+                saved_result=saved_sampling_result,
+            )
+            job_list.append(saved_sampling_job)
+        return job_list
+
+    @property
+    def jobs_json(self) -> str:
+        """Encodes the list of QiskitSavedDataSamplingJob objects to a json
+        string."""
+        return encode_saved_data_job_sequence_to_json(self.jobs)
```

### Comparing `quri_parts_qiskit-0.9.2/quri_parts/qiskit/circuit/__init__.py` & `quri_parts_qiskit-17.0.0/quri_parts/qiskit/circuit/circuit_converter.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from qiskit.circuit.gate import Gate
 from qiskit.extensions import UnitaryGate
 from qiskit.opflow import X, Y, Z
 from typing_extensions import TypeAlias
 
 from quri_parts.circuit import NonParametricQuantumCircuit, QuantumGate, gate_names
 from quri_parts.circuit.gate_names import (
+    Measurement,
     MultiQubitGateNameType,
     ParametricGateNameType,
     SingleQubitGateNameType,
     ThreeQubitGateNameType,
     TwoQubitGateNameType,
     is_gate_name,
     is_multi_qubit_gate_name,
@@ -42,15 +43,15 @@
 )
 
 QiskitCircuitConverter: TypeAlias = Callable[
     [NonParametricQuantumCircuit, Optional[CircuitTranspiler]], QuantumCircuit
 ]
 
 #: CircuitTranspiler to convert a circuit configuration suitable for Qiskit.
-QiskitTranspiler: Callable[[], CircuitTranspiler] = lambda: SequentialTranspiler(
+QiskitSetTranspiler: Callable[[], CircuitTranspiler] = lambda: SequentialTranspiler(
     [PauliDecomposeTranspiler(), PauliRotationDecomposeTranspiler()]
 )
 
 
 _single_qubit_gate_qiskit: Mapping[SingleQubitGateNameType, Type[Gate]] = {
     gate_names.Identity: qgate.IGate,
     gate_names.X: qgate.XGate,
@@ -98,14 +99,16 @@
 ] = {
     gate_names.SqrtY: [[0.5 + 0.5j, -0.5 - 0.5j], [0.5 + 0.5j, 0.5 + 0.5j]],
     gate_names.SqrtYdag: [[0.5 - 0.5j, 0.5 - 0.5j], [-0.5 + 0.5j, 0.5 - 0.5j]],
 }
 
 
 def convert_gate(gate: QuantumGate) -> Gate:
+    """Converts a :class:`QuantumGate` to
+    :class:`qiskit.Gate`."""
     if not is_gate_name(gate.name):
         raise ValueError(f"Unknown gate name: {gate.name}")
 
     if is_single_qubit_gate_name(gate.name):
         if gate.name in _single_qubit_gate_qiskit:
             return _single_qubit_gate_qiskit[gate.name]()
         elif gate.name in _single_qubit_rotation_gate_qiskit:
@@ -155,25 +158,23 @@
     raise NotImplementedError(
         f"Conversion of {gate.name} to qiskit has not been implemented."
     )
 
 
 def convert_circuit(
     circuit: NonParametricQuantumCircuit,
-    transpiler: Optional[CircuitTranspiler] = QiskitTranspiler(),
+    transpiler: Optional[CircuitTranspiler] = QiskitSetTranspiler(),
 ) -> QuantumCircuit:
+    """Converts a :class:`NonParametricQuantumCircuit` to
+    :class:`qiskit.QuantumCircuit`."""
     if transpiler is not None:
         circuit = transpiler(circuit)
 
-    qiskit_circuit = QuantumCircuit(circuit.qubit_count)
+    qiskit_circuit = QuantumCircuit(circuit.qubit_count, circuit.cbit_count)
     for gate in circuit.gates:
+        if gate.name == Measurement:
+            qiskit_circuit.measure(gate.target_indices, gate.classical_indices)
+            continue
+
         indices = (*gate.control_indices, *gate.target_indices)
         qiskit_circuit.append(convert_gate(gate), qargs=indices)
     return qiskit_circuit
-
-
-__all__ = [
-    "QiskitCircuitConverter",
-    "QiskitTranspiler",
-    "convert_gate",
-    "convert_circuit",
-]
```

### Comparing `quri_parts_qiskit-0.9.2/PKG-INFO` & `quri_parts_qiskit-17.0.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,30 @@
 Metadata-Version: 2.1
 Name: quri-parts-qiskit
-Version: 0.9.2
+Version: 17.0.0
 Summary: A plugin to use Qiskit with QURI Parts
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
+Requires-Dist: networkx
 Requires-Dist: numpy (>=1.22.0)
-Requires-Dist: qiskit (>=0.39.4,<0.40.0)
+Requires-Dist: pydantic (>=1.9,<2.0)
+Requires-Dist: qiskit (>=0.41.1,<1)
+Requires-Dist: qiskit-ibm-runtime (>=0.9.0,<1)
 Requires-Dist: quri-parts-circuit
+Requires-Dist: quri-parts-core
 Project-URL: Documentation, https://quri-parts.qunasys.com
 Project-URL: Repository, https://github.com/QunaSys/quri-parts
 Description-Content-Type: text/markdown
 
 # QURI Parts Qiskit
 
 QURI Parts Qiskit is a support library for using Qiskit with QURI Parts.
```

