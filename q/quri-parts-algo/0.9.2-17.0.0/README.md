# Comparing `tmp/quri_parts_algo-0.9.2.tar.gz` & `tmp/quri_parts_algo-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_algo-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_algo-17.0.0.tar", max compression
```

## Comparing `quri_parts_algo-0.9.2.tar` & `quri_parts_algo-17.0.0.tar`

### file list

```diff
@@ -1,27 +1,29 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.850951 quri_parts_algo-0.9.2/LICENSE
--rw-r--r--   0        0        0      276 2023-03-29 07:37:19.850951 quri_parts_algo-0.9.2/README.md
--rw-r--r--   0        0        0     1229 2023-03-29 07:37:22.450959 quri_parts_algo-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:21.634956 quri_parts_algo-0.9.2/quri_parts/algo/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/__init__.py
--rw-r--r--   0        0        0     1333 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/__init__.py
--rw-r--r--   0        0        0     5711 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/hardware_efficient.py
--rw-r--r--   0        0        0     4236 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/symmetry_preserving.py
--rw-r--r--   0        0        0     8908 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/ansatz/two_local.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/__init__.py
--rw-r--r--   0        0        0     1000 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/__init__.py
--rw-r--r--   0        0        0    11773 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/cdr.py
--rw-r--r--   0        0        0      879 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/__init__.py
--rw-r--r--   0        0        0     4348 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py
--rw-r--r--   0        0        0     1234 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/__init__.py
--rw-r--r--   0        0        0    12086 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/zne.py
--rw-r--r--   0        0        0     1272 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/__init__.py
--rw-r--r--   0        0        0     6547 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/adam.py
--rw-r--r--   0        0        0     2563 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/interface.py
--rw-r--r--   0        0        0    10573 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/lbfgs.py
--rw-r--r--   0        0        0     8689 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/nft.py
--rw-r--r--   0        0        0     6270 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/spsa.py
--rw-r--r--   0        0        0     1495 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/optimizer/tolerance.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/py.typed
--rw-r--r--   0        0        0      792 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/utils/__init__.py
--rw-r--r--   0        0        0     6380 2023-03-29 07:37:19.854951 quri_parts_algo-0.9.2/quri_parts/algo/utils/fitting.py
--rw-r--r--   0        0        0     1190 1970-01-01 00:00:00.000000 quri_parts_algo-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/LICENSE
+-rw-r--r--   0        0        0      276 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/README.md
+-rw-r--r--   0        0        0     1230 2024-03-19 02:11:24.034035 quri_parts_algo-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:23.274039 quri_parts_algo-17.0.0/quri_parts/algo/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/__init__.py
+-rw-r--r--   0        0        0     1333 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/ansatz/__init__.py
+-rw-r--r--   0        0        0     5711 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/ansatz/hardware_efficient.py
+-rw-r--r--   0        0        0     4236 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/ansatz/symmetry_preserving.py
+-rw-r--r--   0        0        0     8908 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/ansatz/two_local.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/__init__.py
+-rw-r--r--   0        0        0     1000 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/cdr/__init__.py
+-rw-r--r--   0        0        0    11781 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/cdr/cdr.py
+-rw-r--r--   0        0        0      745 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/post_selection/__init__.py
+-rw-r--r--   0        0        0     2662 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/post_selection/post_selection.py
+-rw-r--r--   0        0        0      879 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/readout_mitigation/__init__.py
+-rw-r--r--   0        0        0     4348 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py
+-rw-r--r--   0        0        0     1234 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/zne/__init__.py
+-rw-r--r--   0        0        0    12088 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/mitigation/zne/zne.py
+-rw-r--r--   0        0        0     1272 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/__init__.py
+-rw-r--r--   0        0        0     6656 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/adam.py
+-rw-r--r--   0        0        0     2563 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/interface.py
+-rw-r--r--   0        0        0    10814 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/lbfgs.py
+-rw-r--r--   0        0        0     8712 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/nft.py
+-rw-r--r--   0        0        0     6287 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/spsa.py
+-rw-r--r--   0        0        0     1495 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/optimizer/tolerance.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/py.typed
+-rw-r--r--   0        0        0      792 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/utils/__init__.py
+-rw-r--r--   0        0        0     6380 2024-03-19 02:11:01.278138 quri_parts_algo-17.0.0/quri_parts/algo/utils/fitting.py
+-rw-r--r--   0        0        0     1191 1970-01-01 00:00:00.000000 quri_parts_algo-17.0.0/PKG-INFO
```

### Comparing `quri_parts_algo-0.9.2/LICENSE` & `quri_parts_algo-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/pyproject.toml` & `quri_parts_algo-17.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-algo"
-version = "0.9.2"
+version = "17.0.0"
 description = "Algorithms for quantum computers"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/ansatz/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/hardware_efficient.py` & `quri_parts_algo-17.0.0/quri_parts/algo/ansatz/hardware_efficient.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/symmetry_preserving.py` & `quri_parts_algo-17.0.0/quri_parts/algo/ansatz/symmetry_preserving.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/ansatz/two_local.py` & `quri_parts_algo-17.0.0/quri_parts/algo/ansatz/two_local.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/cdr/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/cdr/cdr.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/cdr/cdr.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 from quri_parts.circuit.transpile import CliffordApproximationTranspiler
 from quri_parts.core.estimator import (
     ConcurrentQuantumEstimator,
     Estimatable,
     Estimate,
     QuantumEstimator,
 )
-from quri_parts.core.operator import Operator
+from quri_parts.core.operator import Operator, is_hermitian
 from quri_parts.core.state import GeneralCircuitQuantumState
 
 
 class _Estimate(NamedTuple):
     value: complex
     error: float = np.nan  # The error of cdr has been not implemented yet.
 
@@ -92,15 +92,15 @@
         for index, gate in enumerate(circuit.gates):
             if index in indices_rep:
                 transpiler = CliffordApproximationTranspiler()
                 transpiled_gates = transpiler.decompose(gate)
                 new_gates += transpiled_gates
             else:
                 new_gates.append(gate)
-        training_circuits.append(QuantumCircuit(circuit.qubit_count, new_gates))
+        training_circuits.append(QuantumCircuit(circuit.qubit_count, gates=new_gates))
 
     return training_circuits
 
 
 def create_polynomial_regression(order: int) -> RegressionMethod:
     """Returns a :class:`RegressionMethod` that gives a value which is
     evaluated by using the polynomial regression.
@@ -221,15 +221,15 @@
         num_training_circuits: A number of training circuits to be used for CDR.
         fraction_of_replacement: Fraction of the number of non-Clifford gates that are
             to be replaced by Clifford gates.
         seed: Seed to choose which gates to replace with Clifford ones.
     """
 
     if isinstance(obs, Operator):
-        if obs != obs.hermitian_conjugated():
+        if not is_hermitian(obs):
             raise NotImplementedError(
                 "Only the case that obs is a Hermitian has been implemented."
             )
     if fraction_of_replacement < 0 or 1 <= fraction_of_replacement:
         raise ValueError(
             "fraction_of_replacement must be larger than 0 and less than 1."
         )
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/readout_mitigation/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/readout_mitigation/readout_mitigation.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/zne/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/mitigation/zne/zne.py` & `quri_parts_algo-17.0.0/quri_parts/algo/mitigation/zne/zne.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 from quri_parts.circuit import NonParametricQuantumCircuit, QuantumCircuit, inverse_gate
 from quri_parts.core.estimator import (
     ConcurrentQuantumEstimator,
     Estimatable,
     Estimate,
     QuantumEstimator,
 )
-from quri_parts.core.operator import Operator
+from quri_parts.core.operator import Operator, is_hermitian
 from quri_parts.core.state import GeneralCircuitQuantumState
 
 
 class _Estimate(NamedTuple):
     value: float
     error: float = np.nan  # The error of zne has been not implemented yet.
 
@@ -264,15 +264,15 @@
         scale_factors: Factor to scale the circuit. An real number that satisfies >= 1.
         extrapolate_method: :class:`ZeroExtrapolationMethod` that determine the
             method of extrapolation.
         folding_method: :class:`FoldingMethod` that determines the method of folding.
     """
 
     if isinstance(obs, Operator):
-        if obs != obs.hermitian_conjugated():
+        if not is_hermitian(obs):
             raise NotImplementedError(
                 "Only the case that obs is a Hermitian has been implemented."
             )
 
     exp_values: Iterable[float] = []
     circuit_states = []
     for i in scale_factors:
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/adam.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/adam.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from collections.abc import Sequence
-from dataclasses import dataclass
+from dataclasses import dataclass, field
 from typing import Callable, Optional
 
 import numpy as np
 
 from quri_parts.core.utils.array import readonly_array
 
 from .interface import (
@@ -22,23 +22,25 @@
     Optimizer,
     OptimizerState,
     OptimizerStatus,
     Params,
 )
 from .tolerance import ftol as create_ftol
 
-_const_zero_array: Params = readonly_array(np.zeros(0, dtype=float))
+
+def _const_zero_array_factory() -> Params:
+    return readonly_array(np.zeros(0, dtype=float))
 
 
 @dataclass(frozen=True)
 class OptimizerStateAdam(OptimizerState):
     """Optimizer state for Adam."""
 
-    m: Params = _const_zero_array
-    v: Params = _const_zero_array
+    m: Params = field(default_factory=_const_zero_array_factory)
+    v: Params = field(default_factory=_const_zero_array_factory)
 
 
 def _adam_grad_square_moving_average(
     v_prev: Params, grad: Params, m: Params, beta2: float, eps: float
 ) -> Params:
     return beta2 * v_prev + (1 - beta2) * grad**2
 
@@ -92,15 +94,15 @@
         if ftol is not None:
             if not 0.0 < ftol:
                 raise ValueError("ftol must be a positive float.")
             self._ftol = create_ftol(ftol)
 
     def get_init_state(self, init_params: Params) -> OptimizerStateAdam:
         # Defensively copy init_params by np.array
-        params = readonly_array(np.array(init_params))
+        params = readonly_array(np.array(init_params, dtype=float))
         zeros = readonly_array(np.zeros(len(params), dtype=float))
         return OptimizerStateAdam(
             params=params,
             m=zeros,
             v=zeros,
         )
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/interface.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/interface.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/lbfgs.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/lbfgs.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import warnings
-from dataclasses import dataclass, replace
+from dataclasses import dataclass, field, replace
 from typing import TYPE_CHECKING, Callable, Optional, cast
 
 import numpy as np
 
 if TYPE_CHECKING:
     import numpy.typing as npt  # noqa: F401
 
@@ -31,31 +31,33 @@
     Optimizer,
     OptimizerState,
     OptimizerStatus,
     Params,
 )
 from .tolerance import gtol as create_gtol
 
-_const_zero_array: Params = readonly_array(np.zeros(0, dtype=float))
+
+def _const_zero_array_factory() -> Params:
+    return readonly_array(np.zeros(0, dtype=float))
 
 
 @dataclass(frozen=True)
 class OptimizerStateLBFGS(OptimizerState):
     """Optimizer state for LBFGS."""
 
-    grad: Params = _const_zero_array
+    grad: Params = field(default_factory=_const_zero_array_factory)
 
-    p: Params = _const_zero_array
-    s: Params = _const_zero_array
-    y: Params = _const_zero_array
-    rho: Params = _const_zero_array
+    p: Params = field(default_factory=_const_zero_array_factory)
+    s: Params = field(default_factory=_const_zero_array_factory)
+    y: Params = field(default_factory=_const_zero_array_factory)
+    rho: Params = field(default_factory=_const_zero_array_factory)
 
-    cost_prev: float = 0
+    cost_prev: float = 0.0
     ind: int = 0
-    a: Params = _const_zero_array
+    a: Params = field(default_factory=_const_zero_array_factory)
 
 
 class LBFGS(Optimizer):
     r"""L-BFGS (Limited memory Bryden-Fletcher-Goldfarb-Shanno) optimizer.
     Partially inspired by SciPy implementation of BFGS optimizer [1]. For the
     details of algorithm, see [2].
 
@@ -121,25 +123,25 @@
         self._gtol: Optional[Callable[["npt.NDArray[np.float_]"], bool]] = None
         if gtol is not None:
             if not 0.0 < gtol:
                 raise ValueError("ftol must be a positive float.")
             self._gtol = create_gtol(gtol)
 
     def get_init_state(self, init_params: Params) -> OptimizerStateLBFGS:
-        params = readonly_array(np.array(init_params))
+        params = readonly_array(np.array(init_params, dtype=float))
         zeros2d = readonly_array(np.zeros((self._m, len(params)), dtype=float))
         zeros = readonly_array(np.zeros(self._m, dtype=float))
         return OptimizerStateLBFGS(
             params=params,
             grad=zeros,
             p=zeros,
             s=zeros2d,
             y=zeros2d,
             rho=zeros,
-            cost_prev=0,
+            cost_prev=0.0,
             ind=0,
             a=zeros,
         )
 
     def step(
         self,
         state: OptimizerState,
@@ -164,15 +166,15 @@
 
         if niter == 1:
             cost = cost_function(params)
             funcalls += 1
 
             grad = grad_function(params)
             gradcalls += 1
-            cost_prev = cost + cast(float, np.linalg.norm(grad)) / 2
+            cost_prev = cost + cast(float, np.linalg.norm(grad)) / 2.0
 
             p = -grad
 
         funcalls, gradcalls, alpha, cost, cost_prev, grad_next = self._linesearch12(
             funcalls=funcalls,
             gradcalls=gradcalls,
             cost_function=cost_function,
@@ -223,15 +225,15 @@
         ind = state.ind
         a = state.a.copy()
 
         s[ind] = alpha * p
         y[ind] = grad_next - grad
 
         rho_inv = np.dot(s[ind], y[ind])
-        rho[ind] = self._rho_const if rho_inv == 0.0 else 1 / rho_inv
+        rho[ind] = self._rho_const if rho_inv == 0.0 else 1.0 / rho_inv
 
         grad = grad_next
 
         q = grad.copy()
         for i in reversed(range(ind + 1)):
             a[i] = np.dot(s[i], q) * rho[i]
             q -= a[i] * y[i]
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/nft.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/nft.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         self._ftol: Optional[Callable[[float, float], bool]] = None
         if ftol is not None:
             if not 0.0 < ftol:
                 raise ValueError("ftol must be a positive float.")
             self._ftol = create_ftol(ftol)
 
     def get_init_state(self, init_params: Params) -> OptimizerStateNFT:
-        params = readonly_array(np.array(init_params))
+        params = readonly_array(np.array(init_params, dtype=float))
         return OptimizerStateNFT(
             params=params,
         )
 
     def step(
         self,
         state: OptimizerState,
@@ -170,26 +170,26 @@
             ):
                 z0 = cost_function(params)
                 funcalls += 1
             else:
                 z0 = cost
 
             p = params.copy()
-            p[idx] = params[idx] + np.pi / 2
+            p[idx] = params[idx] + np.pi / 2.0
             z1 = cost_function(p)
             funcalls += 1
 
             p = params.copy()
-            p[idx] = params[idx] - np.pi / 2
+            p[idx] = params[idx] - np.pi / 2.0
             z3 = cost_function(p)
             funcalls += 1
 
             z2 = z1 + z3 - z0
-            c = (z1 + z3) / 2
-            a = np.sqrt((z0 - z2) ** 2 + (z1 - z3) ** 2) / 2
+            c = (z1 + z3) / 2.0
+            a = np.sqrt((z0 - z2) ** 2 + (z1 - z3) ** 2) / 2.0
             b = (
                 np.arctan((z1 - z3) / ((z0 - z2) + self._eps * (z0 == z2)))
                 + params[idx]
             )
             b += 0.5 * np.pi + 0.5 * np.pi * np.sign((z0 - z2) + self._eps * (z0 == z2))
 
             params[idx] = b
@@ -247,15 +247,15 @@
                 y_data[i] = cost_function(params)
                 funcalls += 1
             # fit function: `A * cos(x-B) + C`
             # If `A > 0`, it is minimized at `x = B+pi`,
             # while if `A < 0` minimum at `x=b`
             fit_result, _ = curve_fit(_fit_func, x_data, y_data)
             a, b, _ = fit_result
-            params[idx] = b + np.pi if a > 0 else b
+            params[idx] = b + np.pi if a > 0.0 else b
 
         cost = cost_function(params)
         funcalls += 1
 
         return params, cost, funcalls
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/spsa.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/spsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             for stochastic optimization,"
             in IEEE Transactions on Aerospace and Electronic Systems, vol. 34,
             no. 3, pp. 817-823, July 1998, doi: 10.1109/7.705889.
     """
 
     def __init__(
         self,
-        a: float = 2 * np.pi / 10,
+        a: float = 2.0 * np.pi / 10.0,
         c: float = 0.1,
         alpha: float = 0.602,
         gamma: float = 0.101,
         A: float = 0.0,
         ftol: Optional[float] = 1e-5,
         rng_seed: Optional[int] = None,
     ):
@@ -104,15 +104,15 @@
         self._ftol: Optional[Callable[[float, float], bool]] = None
         if ftol is not None:
             if not 0.0 < ftol:
                 raise ValueError("ftol must be a positive float.")
             self._ftol = create_ftol(ftol)
 
     def get_init_state(self, init_params: Params) -> OptimizerStateSPSA:
-        params = readonly_array(np.array(init_params))
+        params = readonly_array(np.array(init_params, dtype=float))
         rng = np.random.default_rng(seed=self._rng_seed)
         return OptimizerStateSPSA(
             params=params,
             rng=rng,
         )
 
     def step(
```

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/optimizer/tolerance.py` & `quri_parts_algo-17.0.0/quri_parts/algo/optimizer/tolerance.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/utils/__init__.py` & `quri_parts_algo-17.0.0/quri_parts/algo/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_algo-0.9.2/quri_parts/algo/utils/fitting.py` & `quri_parts_algo-17.0.0/quri_parts/algo/utils/fitting.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,17 +91,17 @@
 def exp_fitting_with_const(
     x_data: Iterable[float],
     y_data: Iterable[float],
     order: int,
     constant: float,
     point: float,
 ) -> FittedResult:
-    """Curve fitting with an exponential ansatz f(x) = constant + b exp(p(x)), where p(x)
-    is a polynomial of a given order and constant is a known parameter (obtained as the
-    infinite limit f(x->inf) when f(x) converges to a finite asymptotic value).
+    """Curve fitting with an exponential ansatz f(x) = constant + b exp(p(x)), where
+    p(x) is a polynomial of a given order and constant is a known parameter (obtained
+    as the infinite limit f(x->inf) when f(x) converges to a finite asymptotic value).
 
     Args:
         x_data : x-coordinates for fitting.
         y_data : y-coordinates for fitting.
         order: Order of the polynomial on the exponential used for fitting.
         constant: A constant deduced from asymptotic behavior f(x->inf).
         point: A point at which the fitted function to be evaluated.
```

### Comparing `quri_parts_algo-0.9.2/PKG-INFO` & `quri_parts_algo-17.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-algo
-Version: 0.9.2
+Version: 17.0.0
 Summary: Algorithms for quantum computers
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
```

