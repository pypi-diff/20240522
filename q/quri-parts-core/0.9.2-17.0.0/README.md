# Comparing `tmp/quri_parts_core-0.9.2.tar.gz` & `tmp/quri_parts_core-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_core-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_core-17.0.0.tar", max compression
```

## Comparing `quri_parts_core-0.9.2.tar` & `quri_parts_core-17.0.0.tar`

### file list

```diff
@@ -1,43 +1,53 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/LICENSE
--rw-r--r--   0        0        0      288 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/README.md
--rw-r--r--   0        0        0     1169 2023-03-29 07:37:27.166985 quri_parts_core-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     2691 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/py.typed
--rw-r--r--   0        0        0     3382 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/backend/qubit_mapping.py
--rw-r--r--   0        0        0       34 2023-03-29 07:37:26.378981 quri_parts_core-0.9.2/quri_parts/core/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/__init__.py
--rw-r--r--   0        0        0     1215 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/circuit/exp_single_pauli_gate.py
--rw-r--r--   0        0        0     7710 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/__init__.py
--rw-r--r--   0        0        0     6657 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/gradient.py
--rw-r--r--   0        0        0     2343 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/__init__.py
--rw-r--r--   0        0        0     9705 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/estimator.py
--rw-r--r--   0        0        0     6287 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/pauli.py
--rw-r--r--   0        0        0     2228 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/__init__.py
--rw-r--r--   0        0        0     4929 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/bitwise_commuting_pauli.py
--rw-r--r--   0        0        0     2818 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/measurement/interface.py
--rw-r--r--   0        0        0     1329 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/__init__.py
--rw-r--r--   0        0        0     7257 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/conjugation.py
--rw-r--r--   0        0        0     1312 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/grouping/__init__.py
--rw-r--r--   0        0        0     5551 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/grouping/pauli_grouping.py
--rw-r--r--   0        0        0     5683 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/operator.py
--rw-r--r--   0        0        0    10528 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/pauli.py
--rw-r--r--   0        0        0     2325 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/representation/__init__.py
--rw-r--r--   0        0        0     1545 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/representation/bsf.py
--rw-r--r--   0        0        0     3597 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/operator/trotter_suzuki.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/py.typed
--rw-r--r--   0        0        0     3424 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/sampling/__init__.py
--rw-r--r--   0        0        0     6076 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/sampling/shots_allocator.py
--rw-r--r--   0        0        0     2617 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/__init__.py
--rw-r--r--   0        0        0     7057 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/comp_basis.py
--rw-r--r--   0        0        0     3399 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state.py
--rw-r--r--   0        0        0     3604 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_parametric.py
--rw-r--r--   0        0        0     2927 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_vector.py
--rw-r--r--   0        0        0     3380 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/state/state_vector_parametric.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/__init__.py
--rw-r--r--   0        0        0     1142 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/array.py
--rw-r--r--   0        0        0     8991 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/binary_field.py
--rw-r--r--   0        0        0     1403 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/bit.py
--rw-r--r--   0        0        0     1936 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/concurrent.py
--rw-r--r--   0        0        0     6161 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/differentiation.py
--rw-r--r--   0        0        0     1458 2023-03-29 07:37:19.866951 quri_parts_core-0.9.2/quri_parts/core/utils/statistics.py
--rw-r--r--   0        0        0     1186 1970-01-01 00:00:00.000000 quri_parts_core-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.286138 quri_parts_core-17.0.0/LICENSE
+-rw-r--r--   0        0        0      288 2024-03-19 02:11:01.286138 quri_parts_core-17.0.0/README.md
+-rw-r--r--   0        0        0     1195 2024-03-19 02:11:27.494017 quri_parts_core-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0     2769 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/backend/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/backend/py.typed
+-rw-r--r--   0        0        0     3421 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/backend/qubit_mapping.py
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:26.910020 quri_parts_core-17.0.0/quri_parts/core/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/__init__.py
+-rw-r--r--   0        0        0      787 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/circuit/__init__.py
+-rw-r--r--   0        0        0     1998 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/circuit/exp_commuting_paulis_gate.py
+-rw-r--r--   0        0        0     1214 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/circuit/exp_single_pauli_gate.py
+-rw-r--r--   0        0        0    24987 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/__init__.py
+-rw-r--r--   0        0        0     6888 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/gradient.py
+-rw-r--r--   0        0        0     4236 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/hessian.py
+-rw-r--r--   0        0        0     3256 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/__init__.py
+-rw-r--r--   0        0        0    11968 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/estimator.py
+-rw-r--r--   0        0        0     3577 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/estimator_helpers.py
+-rw-r--r--   0        0        0     6905 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/overlap_estimator.py
+-rw-r--r--   0        0        0     6287 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/pauli.py
+-rw-r--r--   0        0        0     1406 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/estimator/utils.py
+-rw-r--r--   0        0        0     3956 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/measurement/__init__.py
+-rw-r--r--   0        0        0     4929 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/measurement/bitwise_commuting_pauli.py
+-rw-r--r--   0        0        0     2818 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/measurement/interface.py
+-rw-r--r--   0        0        0     1486 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/__init__.py
+-rw-r--r--   0        0        0     7257 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/conjugation.py
+-rw-r--r--   0        0        0     1312 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/grouping/__init__.py
+-rw-r--r--   0        0        0     5551 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/grouping/pauli_grouping.py
+-rw-r--r--   0        0        0     7098 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/operator.py
+-rw-r--r--   0        0        0    10967 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/pauli.py
+-rw-r--r--   0        0        0     2325 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/representation/__init__.py
+-rw-r--r--   0        0        0     1545 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/representation/bsf.py
+-rw-r--r--   0        0        0     5156 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/sparse.py
+-rw-r--r--   0        0        0     3597 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/operator/trotter_suzuki.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/py.typed
+-rw-r--r--   0        0        0     5849 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/sampling/__init__.py
+-rw-r--r--   0        0        0     6076 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/sampling/shots_allocator.py
+-rw-r--r--   0        0        0     4347 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/sampling/weighted_shots_allocator.py
+-rw-r--r--   0        0        0     2714 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/__init__.py
+-rw-r--r--   0        0        0     7057 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/comp_basis.py
+-rw-r--r--   0        0        0     3399 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/state.py
+-rw-r--r--   0        0        0     6513 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/state_helper.py
+-rw-r--r--   0        0        0     3604 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/state_parametric.py
+-rw-r--r--   0        0        0     2927 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/state_vector.py
+-rw-r--r--   0        0        0     3380 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/state/state_vector_parametric.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/__init__.py
+-rw-r--r--   0        0        0     1142 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/array.py
+-rw-r--r--   0        0        0     8991 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/binary_field.py
+-rw-r--r--   0        0        0     1613 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/bit.py
+-rw-r--r--   0        0        0     1936 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/concurrent.py
+-rw-r--r--   0        0        0     9439 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/differentiation.py
+-rw-r--r--   0        0        0    11947 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/recording.py
+-rw-r--r--   0        0        0     1458 2024-03-19 02:11:01.290138 quri_parts_core-17.0.0/quri_parts/core/utils/statistics.py
+-rw-r--r--   0        0        0     1225 1970-01-01 00:00:00.000000 quri_parts_core-17.0.0/PKG-INFO
```

### Comparing `quri_parts_core-0.9.2/LICENSE` & `quri_parts_core-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/pyproject.toml` & `quri_parts_core-17.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-core"
-version = "0.9.2"
+version = "17.0.0"
 description = "A platform-independent library for quantum computing"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
@@ -21,18 +21,19 @@
 ]
 
 [tool.poetry-dynamic-versioning]
 enable = false
 style = "pep440"
 
 [tool.poetry.dependencies]
-python = "^3.9.8"
+python = ">=3.9.8,<3.13"
 typing-extensions = "^4.1.1"
 numpy = ">=1.22.0"
 quri-parts-circuit = "*"
+scipy = "^1.11.3"
 
 [tool.poetry.group.dev.dependencies]
 quri-parts-circuit = {path = "../circuit", develop = true}
 
 quri-parts-qulacs = {path = "../qulacs", develop = true}
 pytest = "^7.0.1"
 flake8 = "^4.0.1"
```

### Comparing `quri_parts_core-0.9.2/quri_parts/backend/__init__.py` & `quri_parts_core-17.0.0/quri_parts/backend/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,25 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from abc import abstractmethod, abstractproperty
 from collections import Counter
 from collections.abc import Collection, Mapping
 from dataclasses import dataclass
-from typing import Protocol
+from typing import Protocol, Union
 
 from typing_extensions import TypeAlias
 
 from quri_parts.circuit import NonParametricQuantumCircuit
 
-#: SamplingCounts represents count statistics of repeated sampling of a quantum
-#: circuit. Keys are observed bit patterns encoded in integers and values are counts
-#: of observation of the corresponding bit patterns.
-SamplingCounts: TypeAlias = Mapping[int, int]
+#: SamplingCounts represents count statistics of repeated sampling or the
+#: measurement probabilities of a quantum circuit. Keys are observed bit
+#: patterns encoded in integers and values are counts of observation or the
+#: probabilities of the corresponding bit patterns.
+SamplingCounts: TypeAlias = Mapping[int, Union[float, int]]
 
 
 class SamplingResult(Protocol):
     """A result of a sampling job."""
 
     @abstractproperty
     def counts(self) -> SamplingCounts:
```

### Comparing `quri_parts_core-0.9.2/quri_parts/backend/qubit_mapping.py` & `quri_parts_core-17.0.0/quri_parts/backend/qubit_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Mapping
 from dataclasses import dataclass
 from functools import cached_property
+from typing import Union
 
 from quri_parts.circuit.transpile import QubitRemappingTranspiler
 
 from . import SamplingCounts, SamplingJob, SamplingResult
 
 
 def _create_reverse_map(qubit_mapping: Mapping[int, int]) -> Mapping[int, int]:
@@ -28,15 +29,15 @@
             result += original_bits
     return result
 
 
 def _reverse_map_counts(
     m: SamplingCounts, reverse_bit_map: Mapping[int, int]
 ) -> SamplingCounts:
-    d: dict[int, int] = {}
+    d: dict[int, Union[float, int]] = {}
     for b, count in m.items():
         reversed_bits = _reverse_map_bits(b, reverse_bit_map)
         d[reversed_bits] = d.get(reversed_bits, 0) + count
     return d
 
 
 @dataclass(frozen=True)
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/circuit/exp_single_pauli_gate.py` & `quri_parts_core-17.0.0/quri_parts/core/circuit/exp_single_pauli_gate.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,11 +17,10 @@
     PauliRotation gate, where :math:`a` is a real number coefficient and
     :math:`P` is a product of the Pauli.
 
     Args:
         pauli: :class:`PauliLabel` for the exponentiated single Pauli.
         coef: A real number that is a coefficient of an exponentiated single Pauli.
     """
-
     target_indices, pauli_ids = zip(*pauli)
     c = -1 * coef
     return PauliRotation(target_indices, pauli_ids, 2 * c)
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/estimator/gradient.py` & `quri_parts_core-17.0.0/quri_parts/core/estimator/gradient.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Sequence
 from dataclasses import dataclass
 from typing import Optional, TypeVar, Union, cast
 
+import numpy as np
+
 from quri_parts.circuit.parameter_mapping import LinearParameterMapping
 from quri_parts.circuit.parameter_shift import ShiftedParameters
 from quri_parts.core.estimator import (
     ConcurrentParametricQuantumEstimator,
     Estimatable,
     Estimates,
     GradientEstimator,
@@ -57,35 +59,36 @@
         params: Parameter values for which the gradient is estimated.
         estimator: An estimator that estimates expectation values
             of the operator for the parametric states.
         delta: Step size for numerical differentiation.
 
     Returns:
         The estimated values (can be accessed with :attr:`.values`) with errors
-        of estimation (can be accessed with :attr:`.error_matrix`). Currently,
-        :attr:`.error_matrix` returns `None`.
+        of estimation (can be accessed with :attr:`.error_matrix`).
     """
 
     v = []
     for i in range(len(params)):
         a = list(params)
         a[i] = params[i] + (delta * 0.5)
         v.append(a)
         a = list(params)
         a[i] = params[i] - (delta * 0.5)
         v.append(a)
 
     estimates = list(estimator(op, state, v))
 
     grad = []
+    err_diag = []
     for i in range(len(params)):
         d = estimates[2 * i].value - estimates[2 * i + 1].value
         grad.append(d / delta)
-
-    return _Estimates(grad, None)
+        var = (estimates[2 * i].error ** 2) + (estimates[2 * i + 1].error ** 2)
+        err_diag.append(np.sqrt(var) / delta)
+    return _Estimates(grad, np.diag(err_diag).tolist())
 
 
 def create_numerical_gradient_estimator(
     parametric_estimator: ConcurrentParametricQuantumEstimator[_ParametricStateT],
     delta: float,
 ) -> GradientEstimator[_ParametricStateT]:
     """Create a :class:`GradientEstimator` that estimates gradient values.
@@ -130,16 +133,15 @@
             expectation is evaluated.
         params: Parameter values for which the gradient is estimated.
         estimator: An estimator that estimates expectation values
             of the operator for the parametric states.
 
     Returns:
         The estimated values (can be accessed with :attr:`.values`) with errors
-        of estimation (can be accessed with :attr:`.error_matrix`). Currently,
-        :attr:`.error_matrix` returns `None`.
+        of estimation (can be accessed with :attr:`.error_matrix`).
     """
     param_mapping = cast(LinearParameterMapping, state.parametric_circuit.param_mapping)
     parameter_shift = ShiftedParameters(param_mapping)
     derivatives = parameter_shift.get_derivatives()
     shifted_params_and_coefs = [
         d.get_shifted_parameters_and_coef(params) for d in derivatives
     ]
@@ -167,21 +169,25 @@
 
     estimates = estimator(
         op, cast(_ParametricStateT, raw_param_state), gate_params_list
     )
     estimates_dict = dict(zip(gate_params_list, estimates))
 
     grad = []
+    err_diag = []
     for params_and_coefs in shifted_params_and_coefs:
         g = 0.0 + 0.0j
+        var = 0.0
         for p, c in params_and_coefs:
             g += estimates_dict[p].value * c
+            var += (estimates_dict[p].error ** 2) * abs(c) ** 2
         grad.append(g)
+        err_diag.append(np.sqrt(var))
 
-    return _Estimates(grad, None)
+    return _Estimates(grad, np.diag(err_diag).tolist())
 
 
 def create_parameter_shift_gradient_estimator(
     parametric_estimator: ConcurrentParametricQuantumEstimator[_ParametricStateT],
 ) -> GradientEstimator[_ParametricStateT]:
     def estimator(
         operator: Estimatable, state: _ParametricStateT, params: Sequence[float]
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/estimator.py` & `quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/estimator.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,31 +13,41 @@
 from functools import cached_property
 from math import sqrt
 
 from quri_parts.core.estimator import (
     ConcurrentQuantumEstimator,
     Estimatable,
     Estimate,
+    GeneralQuantumEstimator,
     QuantumEstimator,
+    create_general_estimator_from_estimator,
 )
 from quri_parts.core.estimator.sampling.pauli import (
     general_pauli_sum_expectation_estimator,
     general_pauli_sum_sample_variance,
 )
+from quri_parts.core.estimator.utils import is_estimatable
 from quri_parts.core.measurement import (
+    CommutablePauliSetMeasurement,
     CommutablePauliSetMeasurementFactory,
     PauliReconstructorFactory,
 )
 from quri_parts.core.operator import PAULI_IDENTITY, CommutablePauliSet, Operator
 from quri_parts.core.sampling import (
     ConcurrentSampler,
     MeasurementCounts,
     PauliSamplingShotsAllocator,
 )
-from quri_parts.core.state import CircuitQuantumState
+from quri_parts.core.state import CircuitQuantumState, ParametricCircuitQuantumState
+
+from .estimator_helpers import (
+    CircuitShotPairPreparationFunction,
+    distribute_shots_among_pauli_sets,
+    get_sampling_circuits_and_shots,
+)
 
 
 class _Estimate:
     def __init__(
         self,
         op: Operator,
         const: complex,
@@ -78,21 +88,35 @@
 
 @dataclass
 class _ConstEstimate:
     value: complex
     error: float = 0.0
 
 
+def get_estimate_from_sampling_result(
+    op: Operator,
+    measurement_groups: Iterable[CommutablePauliSetMeasurement],
+    const: complex,
+    sampling_counts: Iterable[MeasurementCounts],
+) -> Estimate[complex]:
+    """Converts sampling counts into the estimation of the operator's
+    expectation value."""
+    pauli_sets = tuple(m.pauli_set for m in measurement_groups)
+    pauli_recs = tuple(m.pauli_reconstructor_factory for m in measurement_groups)
+    return _Estimate(op, const, pauli_sets, pauli_recs, tuple(sampling_counts))
+
+
 def sampling_estimate(
     op: Estimatable,
     state: CircuitQuantumState,
     total_shots: int,
     sampler: ConcurrentSampler,
     measurement_factory: CommutablePauliSetMeasurementFactory,
     shots_allocator: PauliSamplingShotsAllocator,
+    circuit_shot_pair_prep_fn: CircuitShotPairPreparationFunction = get_sampling_circuits_and_shots,  # noqa: E501
 ) -> Estimate[complex]:
     """Estimate expectation value of a given operator with a given state by
     sampling measurement.
 
     The sampling measurements are configured with arguments as follows.
 
     Args:
@@ -100,58 +124,45 @@
         state: A quantum state on which the operator expectation is evaluated.
         total_shots: Total number of shots available for sampling measurements.
         sampler: A Sampler that actually performs the sampling measurements.
         measurement_factory: A function that performs Pauli grouping and returns
             a measurement scheme for Pauli operators constituting the original operator.
         shots_allocator: A function that allocates the total shots to Pauli groups to
             be measured.
-
+        circuit_shot_pair_prep_fn: A :class:`~CircuitShotPairPreparationFunction` that
+            prepares the set of circuits to perform measurement with. It is default to
+            a function that concatenates the measurement circuits after the state
+            preparation circuit.
     Returns:
         The estimated value (can be accessed with :attr:`.value`) with standard error
             of estimation (can be accessed with :attr:`.error`).
     """
+    assert is_estimatable(
+        op, state
+    ), "Number of qubits of the operator is too large to estimate."
+
     if not isinstance(op, Operator):
         op = Operator({op: 1.0})
 
     if len(op) == 0:
         return _ConstEstimate(0.0)
 
     if len(op) == 1 and PAULI_IDENTITY in op:
         return _ConstEstimate(op[PAULI_IDENTITY])
 
-    # If there is a standalone Identity group then eliminate, else set const 0.
-    const: complex = 0.0
-    measurements = []
-    for m in measurement_factory(op):
-        if m.pauli_set == {PAULI_IDENTITY}:
-            const = op[PAULI_IDENTITY]
-        else:
-            measurements.append(m)
-
-    pauli_sets = tuple(m.pauli_set for m in measurements)
-    shot_allocs = shots_allocator(op, pauli_sets, total_shots)
-    shots_map = {pauli_set: n_shots for pauli_set, n_shots in shot_allocs}
-
-    # Eliminate pauli sets which are allocated no shots
-    measurement_circuit_shots = [
-        (m, state.circuit + m.measurement_circuit, shots_map[m.pauli_set])
-        for m in measurements
-        if shots_map[m.pauli_set] > 0
-    ]
+    const = op.constant
+    measurements = measurement_factory(op)
+    measurements = [m for m in measurements if m.pauli_set != {PAULI_IDENTITY}]
 
-    circuit_and_shots = [
-        (circuit, shots) for _, circuit, shots in measurement_circuit_shots
-    ]
-    sampling_counts = sampler(circuit_and_shots)
-
-    pauli_sets = tuple(m.pauli_set for m, _, _ in measurement_circuit_shots)
-    pauli_recs = tuple(
-        m.pauli_reconstructor_factory for m, _, _ in measurement_circuit_shots
+    shots_map = distribute_shots_among_pauli_sets(
+        op, measurements, shots_allocator, total_shots
     )
-    return _Estimate(op, const, pauli_sets, pauli_recs, tuple(sampling_counts))
+    circuit_and_shots = circuit_shot_pair_prep_fn(state, measurements, shots_map)
+    sampling_counts = sampler(circuit_and_shots)
+    return get_estimate_from_sampling_result(op, measurements, const, sampling_counts)
 
 
 def create_sampling_estimator(
     total_shots: int,
     sampler: ConcurrentSampler,
     measurement_factory: CommutablePauliSetMeasurementFactory,
     shots_allocator: PauliSamplingShotsAllocator,
@@ -181,14 +192,15 @@
 def concurrent_sampling_estimate(
     operators: Collection[Estimatable],
     states: Collection[CircuitQuantumState],
     total_shots: int,
     sampler: ConcurrentSampler,
     measurement_factory: CommutablePauliSetMeasurementFactory,
     shots_allocator: PauliSamplingShotsAllocator,
+    circuit_shot_pair_prep_fn: CircuitShotPairPreparationFunction = get_sampling_circuits_and_shots,  # noqa: E501
 ) -> Iterable[Estimate[complex]]:
     """Estimate expectation value of given operators with given states by
     sampling measurement.
 
     The sampling measurements are configured with arguments as follows.
 
     Args:
@@ -196,15 +208,18 @@
         states: Quantum states on which the operator expectation is evaluated.
         total_shots: Total number of shots available for sampling measurements.
         sampler: A Sampler that actually performs the sampling measurements.
         measurement_factory: A function that performs Pauli grouping and returns
             a measurement scheme for Pauli operators constituting the original operator.
         shots_allocator: A function that allocates the total shots to Pauli groups to
             be measured.
-
+        circuit_shot_pair_prep_fn: A :class:`~CircuitShotPairPreparationFunction` that
+            prepares the set of circuits to perform measurement with. It is default to
+            a function that concatenates the measurement circuits after the state
+            preparation circuit.
     Returns:
         The estimated values (can be accessed with :attr:`.value`) with standard errors
             of estimation (can be accessed with :attr:`.error`).
     """
     num_ops = len(operators)
     num_states = len(states)
 
@@ -220,17 +235,24 @@
             f"number of states ({num_states})."
         )
 
     if num_states == 1:
         states = [next(iter(states))] * num_ops
     if num_ops == 1:
         operators = [next(iter(operators))] * num_states
+
     return [
         sampling_estimate(
-            op, state, total_shots, sampler, measurement_factory, shots_allocator
+            op,
+            state,
+            total_shots,
+            sampler,
+            measurement_factory,
+            shots_allocator,
+            circuit_shot_pair_prep_fn,
         )
         for op, state in zip(operators, states)
     ]
 
 
 def create_sampling_concurrent_estimator(
     total_shots: int,
@@ -262,7 +284,30 @@
             total_shots,
             sampler,
             measurement_factory,
             shots_allocator,
         )
 
     return estimator
+
+
+def create_general_sampling_estimator(
+    total_shots: int,
+    sampler: ConcurrentSampler,
+    measurement_factory: CommutablePauliSetMeasurementFactory,
+    shots_allocator: PauliSamplingShotsAllocator,
+) -> GeneralQuantumEstimator[CircuitQuantumState, ParametricCircuitQuantumState]:
+    """Creates a :class:`GeneralQuantumEstimator` that performs sampling
+    estimation.
+
+    Args:
+        total_shots: Total number of shots available for sampling measurements.
+        sampler: A Sampler that actually performs the sampling measurements.
+        measurement_factory: A function that performs Pauli grouping and returns
+            a measurement scheme for Pauli operators constituting the original operator.
+        shots_allocator: A function that allocates the total shots to Pauli groups to
+            be measured.
+    """
+    sampling_estimator = create_sampling_estimator(
+        total_shots, sampler, measurement_factory, shots_allocator
+    )
+    return create_general_estimator_from_estimator(sampling_estimator)
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/estimator/sampling/pauli.py` & `quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/pauli.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/measurement/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/measurement/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,14 +4,18 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Iterable, Union
+
+from quri_parts.core.operator import Operator, PauliLabel
+
 from .bitwise_commuting_pauli import (
     bitwise_commuting_pauli_measurement,
     bitwise_commuting_pauli_measurement_circuit,
     bitwise_pauli_reconstructor_factory,
     individual_pauli_measurement,
 )
 from .interface import (
@@ -35,19 +39,72 @@
 #: a :class:`~PauliReconstructor` for a given Pauli operator.
 PauliReconstructorFactory = PauliReconstructorFactory
 
 #: Represents a function that performs grouping of Pauli operators into groups of
 #: commutable Pauli operators and returns measurement schemes for them.
 CommutablePauliSetMeasurementFactory = CommutablePauliSetMeasurementFactory
 
+
+class CachedMeasurementFactory:
+    """A class decorator that converts a
+    :class:`CommutablePauliSetMeasurementFactory` to a new
+    :class:`CommutablePauliSetMeasurementFactory` runs the same grouping
+    algorithm but caches grouping result for later usage.
+
+    Example:
+    >>> cached_measurement_factory = CachedMeasuremetFactory(
+    ...    bitwise_commuting_pauli_measurement
+    ... )
+    >>> operator = Operator({
+    ...    pauli_label("X0 Y1"): 1,
+    ...    pauli_label("X0 Z2"): 2,
+    ...    pauli_label("Y0 Z2"): 3,
+    ...    PAULI_IDENTITY: 4
+    ... })
+    >>> cached_measurement_factory(operator)
+    """
+
+    def __init__(
+        self, measurement_factory: CommutablePauliSetMeasurementFactory
+    ) -> None:
+        self._measurement_factory = measurement_factory
+        self._cache: dict[
+            frozenset[tuple[PauliLabel, complex]],
+            Iterable[CommutablePauliSetMeasurement],
+        ] = {}
+
+    def __call__(
+        self, paulis: Union[Operator, Iterable[PauliLabel]]
+    ) -> Iterable[CommutablePauliSetMeasurement]:
+        if not isinstance(paulis, Operator):
+            paulis = Operator({p: 1 + 0j for p in paulis})
+
+        op_key = frozenset(paulis.items())
+        if op_key in self._cache:
+            return self._cache[op_key]
+        groups = self._measurement_factory(paulis)
+        self._cache[op_key] = groups
+        return groups
+
+    @property
+    def cached_groups(
+        self,
+    ) -> dict[
+        frozenset[tuple[PauliLabel, complex]],
+        Iterable[CommutablePauliSetMeasurement],
+    ]:
+        return self._cache.copy()
+
+
 __all__ = [
     "PauliMeasurementCircuitGeneration",
     "PauliReconstructor",
     "PauliReconstructorFactory",
     "CommutablePauliSetMeasurement",
     "CommutablePauliSetMeasurementTuple",
     "CommutablePauliSetMeasurementFactory",
     "bitwise_commuting_pauli_measurement_circuit",
     "bitwise_pauli_reconstructor_factory",
     "bitwise_commuting_pauli_measurement",
     "individual_pauli_measurement",
+    "CachedMeasuremetFactory",
 ]
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/measurement/bitwise_commuting_pauli.py` & `quri_parts_core-17.0.0/quri_parts/core/measurement/bitwise_commuting_pauli.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/measurement/interface.py` & `quri_parts_core-17.0.0/quri_parts/core/measurement/interface.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -4,41 +4,46 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from .operator import Operator, commutator, zero
+from .operator import Operator, commutator, is_hermitian, is_ops_close, truncate, zero
 from .pauli import (
     PAULI_IDENTITY,
     CommutablePauliSet,
     PauliLabel,
     SinglePauli,
     pauli_label,
     pauli_name,
     pauli_product,
 )
 from .representation import transition_amp_comp_basis, transition_amp_representation
+from .sparse import get_sparse_matrix
 from .trotter_suzuki import trotter_suzuki_decomposition
 
 PAULI_IDENTITY = PAULI_IDENTITY
 """PauliLabel used as an identity."""
 
 #: CommutablePauliSet
 CommutablePauliSet = CommutablePauliSet
 
 __all__ = [
     "CommutablePauliSet",
     "commutator",
+    "truncate",
+    "is_hermitian",
+    "is_ops_close",
     "PAULI_IDENTITY",
     "pauli_label",
     "pauli_name",
     "pauli_product",
     "PauliLabel",
     "Operator",
     "SinglePauli",
     "transition_amp_comp_basis",
     "transition_amp_representation",
     "zero",
     "trotter_suzuki_decomposition",
+    "get_sparse_matrix",
 ]
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/conjugation.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/conjugation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/grouping/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/grouping/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/grouping/pauli_grouping.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/grouping/pauli_grouping.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/operator.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/operator.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+import cmath
+
 from .pauli import PAULI_IDENTITY, PauliLabel, pauli_product
 
 
 class Operator(dict[PauliLabel, complex]):
     """Operator represents the set of single-term operators as a
     dict[PauliLabel, coefficient].
 
@@ -104,14 +106,28 @@
             return NotImplemented
 
     def __rmul__(self, other: object) -> "Operator":
         if not isinstance(other, (int, float, complex)):
             return NotImplemented
         return self * other
 
+    def __truediv__(self, other: object) -> "Operator":
+        if not isinstance(other, (int, float, complex)):
+            return NotImplemented
+        copied = self.copy()
+        copied /= other
+        return copied
+
+    def __itruediv__(self, other: object) -> "Operator":
+        if not isinstance(other, (int, float, complex)):
+            return NotImplemented
+        for pauli, coef in self.items():
+            self[pauli] = coef / other
+        return self
+
     def add_term(self, pauli_label: PauliLabel, coef: complex) -> None:
         """Method for adding single-term operator."""
         if coef == 0:
             return
         c = self.get(pauli_label, 0)
         new_coef = c + coef
         if new_coef == 0 and pauli_label in self:
@@ -159,7 +175,36 @@
 def commutator(op1: Operator, op2: Operator) -> Operator:
     """Returns the commutator of op1 and op2 :math:`[\\text{op1},
 
     \\text{op2}]`.
     """
     op_res = op1 * op2 - op2 * op1
     return op_res
+
+
+def is_ops_close(
+    op1: Operator, op2: Operator, rtol: float = 1e-9, atol: float = 0.0
+) -> bool:
+    """Returns ``True`` if two operators are close to each other."""
+    uniq_p_labels = set(op1) | set(op2)
+
+    for pauli in uniq_p_labels:
+        op1_coeff = op1.get(pauli, 0.0)
+        op2_coeff = op2.get(pauli, 0.0)
+        if not cmath.isclose(op1_coeff, op2_coeff, rel_tol=rtol, abs_tol=atol):
+            return False
+    return True
+
+
+def truncate(op: Operator, atol: float = 1e-8) -> Operator:
+    """Returns truncated operator by eliminating terms whose coefficients are
+    smaller than ``atol``."""
+    _op = Operator()
+    for pauli, coef in op.items():
+        if abs(coef) >= atol:
+            _op[pauli] = coef
+    return _op
+
+
+def is_hermitian(op: Operator, atol: float = 1e-8) -> bool:
+    """Returns ``True`` if given operator is hermitian."""
+    return is_ops_close(op, op.hermitian_conjugated(), atol)
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/pauli.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/pauli.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # limitations under the License.
 
 import re
 from abc import abstractmethod
 from collections.abc import Collection, Iterable, Mapping, Sequence, Set
 from enum import IntEnum
 from typing import Optional, Protocol, Union, cast, runtime_checkable
+from weakref import WeakValueDictionary
 
 from typing_extensions import TypeAlias
 
 
 class SinglePauli(IntEnum):
     """An integer enumeration representing Pauli matrices X, Y, Z acting on a
     single qubit."""
@@ -36,14 +37,16 @@
     (SinglePauli.Y, SinglePauli.Y): None,
     (SinglePauli.Y, SinglePauli.Z): (SinglePauli.X, 1.0j),
     (SinglePauli.Z, SinglePauli.X): (SinglePauli.Y, 1.0j),
     (SinglePauli.Z, SinglePauli.Y): (SinglePauli.X, -1.0j),
     (SinglePauli.Z, SinglePauli.Z): None,
 }
 
+_pauli_cache: WeakValueDictionary[str, "PauliLabel"] = WeakValueDictionary()
+
 
 def pauli_name(p: int) -> str:
     """Returns the name of Pauli matrix for a SinglePauli (int)"""
     # Using a predefined lookup dict for performance (faster than SinglePauli(p).name)
     return _pauli_name_map[p]
 
 
@@ -175,16 +178,25 @@
     >>> for i, p in label:
     ...     # Do something with p
 
     .. _Hashable:
         https://docs.python.org/3/library/collections.abc.html#collections.abc.Hashable
     """
 
+    def __new__(cls, arg: Iterable[tuple[int, int]] = ()) -> "PauliLabel":
+        instance = super().__new__(cls, arg)  # type: ignore
+        pl_str = str(instance)
+        if pl_str in _pauli_cache:
+            return _pauli_cache[pl_str]
+        else:
+            _pauli_cache[pl_str] = instance
+            return instance
+
     def __str__(self) -> str:
-        if self == PAULI_IDENTITY:
+        if len(self) == 0:
             return "I"
         return " ".join(
             [SinglePauli(o).name + str(i) for i, o in sorted(self, key=lambda t: t[0])]
         )
 
     def qubit_indices(self) -> Collection[int]:
         """Returns a Collection of qubit indices on which Pauli matrices act.
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/representation/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/representation/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/representation/bsf.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/representation/bsf.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/operator/trotter_suzuki.py` & `quri_parts_core-17.0.0/quri_parts/core/operator/trotter_suzuki.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/sampling/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/estimator/sampling/estimator_helpers.py`

 * *Files 25% similar despite different names*

```diff
@@ -4,91 +4,79 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Callable, Collection, Iterable, Mapping, NamedTuple, Union
+from collections.abc import Iterable
+from typing import Callable
 
 from typing_extensions import TypeAlias
 
-from quri_parts.backend import SamplingBackend
 from quri_parts.circuit import NonParametricQuantumCircuit
+from quri_parts.core.measurement import CommutablePauliSetMeasurement
 from quri_parts.core.operator import CommutablePauliSet, Operator
+from quri_parts.core.sampling import PauliSamplingShotsAllocator
+from quri_parts.core.state import CircuitQuantumState
 
-#: MeasurementCounts represents count statistics of repeated measurements of a quantum
-#: circuit. Keys are observed bit patterns encoded in integers and values are counts
-#: of observation of the corresponding bit patterns.
-MeasurementCounts: TypeAlias = Mapping[int, Union[int, float]]
-
-#: Sampler represents a function that samples a specified (non-parametric) circuit by
-#: a specified times and returns the count statistics.
-Sampler: TypeAlias = Callable[[NonParametricQuantumCircuit, int], MeasurementCounts]
-
-#: ConcurrentSampler represents a function that samples specified (non-parametric)
-#: circuits concurrently.
-ConcurrentSampler: TypeAlias = Callable[
-    [Iterable[tuple[NonParametricQuantumCircuit, int]]], Iterable[MeasurementCounts]
+#: A function that returns the sequence of (circuit, shot) pairs for performing
+#: sampling estimation on the given state. The default operation is that
+#: it concatenates the measurement circuits determined by the grouping scheme
+#: to the circuit that prepares the state. This is done with the
+#: `circuit_shot_pairs_preparation_fn` below. Users may customize this function if
+#: additional circuit operations needs to be done other than simple concatenation.
+CircuitShotPairPreparationFunction: TypeAlias = Callable[
+    [
+        CircuitQuantumState,
+        Iterable[CommutablePauliSetMeasurement],
+        dict[CommutablePauliSet, int],
+    ],
+    Iterable[tuple[NonParametricQuantumCircuit, int]],
 ]
 
 
-def create_sampler_from_sampling_backend(backend: SamplingBackend) -> Sampler:
-    """Create a simple :class:`~Sampler` using a :class:`~SamplingBackend`."""
-
-    def sampler(
-        circuit: NonParametricQuantumCircuit, n_shots: int
-    ) -> MeasurementCounts:
-        job = backend.sample(circuit, n_shots)
-        return job.result().counts
-
-    return sampler
-
-
-def create_concurrent_sampler_from_sampling_backend(
-    backend: SamplingBackend,
-) -> ConcurrentSampler:
-    """Create a simple :class:`~ConcurrentSampler` using a
-    :class:`~SamplingBackend`."""
-
-    def sampler(
-        shot_circuit_pairs: Iterable[tuple[NonParametricQuantumCircuit, int]]
-    ) -> Iterable[MeasurementCounts]:
-        jobs = [
-            backend.sample(circuit, n_shots) for circuit, n_shots in shot_circuit_pairs
-        ]
-        return map(lambda j: j.result().counts, jobs)
-
-    return sampler
-
-
-def create_sampler_from_concurrent_sampler(
-    concurrent_sampler: ConcurrentSampler,
-) -> Sampler:
-    def sampler(circuit: NonParametricQuantumCircuit, shots: int) -> MeasurementCounts:
-        return next(iter(concurrent_sampler([(circuit, shots)])))
-
-    return sampler
-
-
-class PauliSamplingSetting(NamedTuple):
-    pauli_set: CommutablePauliSet
-    n_shots: int
-
-
-#: PauliSamplingShotsAllocator represents a function that distributes
-#: a given number of sampling shots to each :class:`~CommutablePauliSet`.
-PauliSamplingShotsAllocator: TypeAlias = Callable[
-    [Operator, Collection[CommutablePauliSet], int], Collection[PauliSamplingSetting]
-]
-
-
-__all__ = [
-    "MeasurementCounts",
-    "Sampler",
-    "ConcurrentSampler",
-    "create_sampler_from_sampling_backend",
-    "create_concurrent_sampler_from_sampling_backend",
-    "create_sampler_from_concurrent_sampler",
-    "PauliSamplingSetting",
-    "PauliSamplingShotsAllocator",
-]
+def distribute_shots_among_pauli_sets(
+    operator: Operator,
+    measurement_groups: Iterable[CommutablePauliSetMeasurement],
+    shots_allocator: PauliSamplingShotsAllocator,
+    total_shots: int,
+) -> dict[CommutablePauliSet, int]:
+    """Distribute shots to each commuting pauli sets.
+
+    Args:
+        operator: The operator to be measured.
+        measurement_groups: Sequence of :class:`~CommutablePauliSetMeasurement` that
+            corresponds to the grouping result of the operator.
+        shot_allocator: A function that allocates the total shots to Pauli groups to
+            be measured.
+        total_shots: Total number of shots available for sampling measurements.
+    """
+    pauli_sets = {m.pauli_set for m in measurement_groups}
+    shot_allocs = shots_allocator(operator, pauli_sets, total_shots)
+    return {pauli_set: n_shots for pauli_set, n_shots in shot_allocs}
+
+
+def get_sampling_circuits_and_shots(
+    state: CircuitQuantumState,
+    measurement_groups: Iterable[CommutablePauliSetMeasurement],
+    shots_map: dict[CommutablePauliSet, int],
+) -> Iterable[tuple[NonParametricQuantumCircuit, int]]:
+    """Sets up the (circuit, shot) pairs for performing sampling estimation.
+    The circuit is given by the measurement circuit concatenated after the
+    circuit held inside the state.
+
+    Args:
+        state: The state on which the expectation value is estimated.
+        measurement_groups: Sequence of :class:`~CommutablePauliSetMeasurement` that
+            corresponds to the grouping result of the operator.
+        shots_map: A dictionary whose key is the commuting pauli set and the value is
+            the shot count assigned to the commuting pauli set.
+    """
+    return [
+        (
+            state.circuit + m.measurement_circuit,
+            n_shots,
+        )
+        for m in measurement_groups
+        if (n_shots := shots_map[m.pauli_set]) > 0
+    ]
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/sampling/shots_allocator.py` & `quri_parts_core-17.0.0/quri_parts/core/sampling/shots_allocator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/__init__.py` & `quri_parts_core-17.0.0/quri_parts/core/state/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 # limitations under the License.
 
 """Interfaces and classes representing quantum states."""
 from typing import Sequence, TypeVar
 
 from .comp_basis import ComputationalBasisState, comp_basis_superposition
 from .state import CircuitQuantumState, GeneralCircuitQuantumState, QuantumState
+from .state_helper import apply_circuit, quantum_state
 from .state_parametric import ParametricCircuitQuantumState
 from .state_vector import QuantumStateVector, StateVectorType
 from .state_vector_parametric import ParametricQuantumStateVector
 
 #: A type alias representing a numerical state vector,
 #: equivalent to np.ndarray of complex floats.
 StateVectorType = StateVectorType
@@ -55,8 +56,10 @@
     "comp_basis_superposition",
     "ComputationalBasisSuperposition",
     "StateVectorType",
     "QuantumStateVector",
     "ParametricQuantumStateVector",
     "QuantumStateT",
     "ParametricQuantumStateT",
+    "quantum_state",
+    "apply_circuit",
 ]
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/comp_basis.py` & `quri_parts_core-17.0.0/quri_parts/core/state/comp_basis.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/state.py` & `quri_parts_core-17.0.0/quri_parts/core/state/state.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/state_parametric.py` & `quri_parts_core-17.0.0/quri_parts/core/state/state_parametric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/state_vector.py` & `quri_parts_core-17.0.0/quri_parts/core/state/state_vector.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/state/state_vector_parametric.py` & `quri_parts_core-17.0.0/quri_parts/core/state/state_vector_parametric.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/utils/array.py` & `quri_parts_core-17.0.0/quri_parts/core/utils/array.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/utils/binary_field.py` & `quri_parts_core-17.0.0/quri_parts/core/utils/binary_field.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/utils/bit.py` & `quri_parts_core-17.0.0/quri_parts/core/utils/bit.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
+from typing import Union
+
+import numpy as np
+
+
+def bit_length(bits: Union[int, np.int8, np.int16, np.int32, np.int64]) -> int:
+    """Computes the bit length of an integer."""
+    return int(bits).bit_length()
+
 
 def get_bit(x: int, index: int) -> bool:
     """Returns if the bit at 'index' is set or not."""
     mask = 1 << index
     return (x & mask) != 0
 
 
@@ -30,12 +39,12 @@
             return i
     raise ValueError("Given integer is too large.")
 
 
 def parity_sign_of_bits(bits: int) -> int:
     """Returns a sign corresponding to parity of bits (even=1, odd=-1)."""
     sign = 1
-    for _ in range(bits.bit_length()):
+    for _ in range(bit_length(bits)):
         if bits & 1 == 1:
             sign *= -1
         bits = bits >> 1
     return sign
```

### Comparing `quri_parts_core-0.9.2/quri_parts/core/utils/concurrent.py` & `quri_parts_core-17.0.0/quri_parts/core/utils/concurrent.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/quri_parts/core/utils/statistics.py` & `quri_parts_core-17.0.0/quri_parts/core/utils/statistics.py`

 * *Files identical despite different names*

### Comparing `quri_parts_core-0.9.2/PKG-INFO` & `quri_parts_core-17.0.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: quri-parts-core
-Version: 0.9.2
+Version: 17.0.0
 Summary: A platform-independent library for quantum computing
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
-Requires-Python: >=3.9.8,<4.0.0
+Requires-Python: >=3.9.8,<3.13
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Typing :: Typed
 Requires-Dist: numpy (>=1.22.0)
 Requires-Dist: quri-parts-circuit
+Requires-Dist: scipy (>=1.11.3,<2.0.0)
 Requires-Dist: typing-extensions (>=4.1.1,<5.0.0)
 Project-URL: Documentation, https://quri-parts.qunasys.com
 Project-URL: Repository, https://github.com/QunaSys/quri-parts
 Description-Content-Type: text/markdown
 
 # QURI Parts Core
```

