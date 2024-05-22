# Comparing `tmp/quri_parts_openfermion-0.9.2.tar.gz` & `tmp/quri_parts_openfermion-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_openfermion-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_openfermion-17.0.0.tar", max compression
```

## Comparing `quri_parts_openfermion-0.9.2.tar` & `quri_parts_openfermion-17.0.0.tar`

### file list

```diff
@@ -1,16 +1,19 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.870951 quri_parts_openfermion-0.9.2/LICENSE
--rw-r--r--   0        0        0      280 2023-03-29 07:37:19.870951 quri_parts_openfermion-0.9.2/README.md
--rw-r--r--   0        0        0     1315 2023-03-29 07:37:31.019006 quri_parts_openfermion-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      259 2023-03-29 07:37:30.195002 quri_parts_openfermion-0.9.2/quri_parts/openfermion/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/__init__.py
--rw-r--r--   0        0        0      659 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/__init__.py
--rw-r--r--   0        0        0     4333 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/kupccgsd.py
--rw-r--r--   0        0        0     3661 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/uccsd.py
--rw-r--r--   0        0        0      881 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/__init__.py
--rw-r--r--   0        0        0     1435 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/conversions.py
--rw-r--r--   0        0        0     2245 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/fermion_operator.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/py.typed
--rw-r--r--   0        0        0    11715 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/transforms/__init__.py
--rw-r--r--   0        0        0      720 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/__init__.py
--rw-r--r--   0        0        0     2915 2023-03-29 07:37:19.874951 quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py
--rw-r--r--   0        0        0     1227 1970-01-01 00:00:00.000000 quri_parts_openfermion-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/LICENSE
+-rw-r--r--   0        0        0      280 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/README.md
+-rw-r--r--   0        0        0     1316 2024-03-19 02:11:29.646006 quri_parts_openfermion-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0      259 2024-03-19 02:11:29.026009 quri_parts_openfermion-17.0.0/quri_parts/openfermion/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/__init__.py
+-rw-r--r--   0        0        0      645 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/ansatz/__init__.py
+-rw-r--r--   0        0        0     7905 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/ansatz/kupccgsd.py
+-rw-r--r--   0        0        0    12833 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/ansatz/uccsd.py
+-rw-r--r--   0        0        0      792 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/mol/__init__.py
+-rw-r--r--   0        0        0     2606 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/mol/hamiltonian.py
+-rw-r--r--   0        0        0      881 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/__init__.py
+-rw-r--r--   0        0        0     1435 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/conversions.py
+-rw-r--r--   0        0        0     2245 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/fermion_operator.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/py.typed
+-rw-r--r--   0        0        0    23660 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/transforms/__init__.py
+-rw-r--r--   0        0        0      829 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/utils/__init__.py
+-rw-r--r--   0        0        0     3565 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py
+-rw-r--r--   0        0        0     3368 2024-03-19 02:11:01.298138 quri_parts_openfermion-17.0.0/quri_parts/openfermion/utils/post_selection_filters.py
+-rw-r--r--   0        0        0     1228 1970-01-01 00:00:00.000000 quri_parts_openfermion-17.0.0/PKG-INFO
```

### Comparing `quri_parts_openfermion-0.9.2/LICENSE` & `quri_parts_openfermion-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.2/pyproject.toml` & `quri_parts_openfermion-17.0.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning", "setuptools"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry]
 name = "quri-parts-openfermion"
-version = "0.9.2"
+version = "17.0.0"
 description = "A support library for using OpenFermion with QURI Parts"
 license = "Apache-2.0"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
```

### Comparing `quri_parts_openfermion-0.9.2/quri_parts/openfermion/ansatz/__init__.py` & `quri_parts_openfermion-17.0.0/quri_parts/openfermion/ansatz/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,10 +5,10 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from .kupccgsd import KUpCCGSD
-from .uccsd import TrotterSingletUCCSD
+from .uccsd import TrotterUCCSD
 
-__all__ = ["KUpCCGSD", "TrotterSingletUCCSD"]
+__all__ = ["KUpCCGSD", "TrotterUCCSD"]
```

### Comparing `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/__init__.py` & `quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/__init__.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/conversions.py` & `quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/conversions.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.2/quri_parts/openfermion/operator/fermion_operator.py` & `quri_parts_openfermion-17.0.0/quri_parts/openfermion/operator/fermion_operator.py`

 * *Files identical despite different names*

### Comparing `quri_parts_openfermion-0.9.2/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py` & `quri_parts_openfermion-17.0.0/quri_parts/openfermion/utils/add_exp_excitation_gates_trotter_decomposition.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,50 +4,64 @@
 #      http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-from typing import Sequence, Union, cast
+from typing import Sequence, TypeVar, Union, cast
 
 from openfermion.ops import FermionOperator
 
 from quri_parts.chem.utils.excitations import DoubleExcitation, SingleExcitation
 from quri_parts.circuit import LinearMappedUnboundParametricQuantumCircuit, Parameter
+from quri_parts.core.operator import Operator
 
 from ..transforms import OpenFermionQubitOperatorMapper
 
+Excitation = TypeVar("Excitation", SingleExcitation, DoubleExcitation)
+
 
 def add_exp_excitation_gates_trotter_decomposition(
     circuit: LinearMappedUnboundParametricQuantumCircuit,
-    excitation_indices: Sequence[Union[SingleExcitation, DoubleExcitation]],
+    excitation_indices: Sequence[Excitation],
     params: Sequence[Parameter],
     operator_mapper: OpenFermionQubitOperatorMapper,
     coef: float,
 ) -> LinearMappedUnboundParametricQuantumCircuit:
     """Add parametric Pauli rotation gates as a product of the exponentials of
     the excitations to the given :attr:`circuit`."""
     for i, sorb_indices in enumerate(excitation_indices):
-        op = _create_operator(sorb_indices, operator_mapper)
+        op = create_anti_hermitian_sd_excitation_operator(sorb_indices, operator_mapper)
         for pauli, op_coef in op.items():
             pauli_index_list, pauli_id_list = zip(*pauli)
             op_coef = op_coef.imag
             circuit.add_ParametricPauliRotation_gate(
                 pauli_index_list,
                 pauli_id_list,
                 {params[i]: -2.0 * op_coef * coef},
             )
     return circuit
 
 
-def _create_operator(
+def create_anti_hermitian_sd_excitation_operator(
     excitation_indices: Union[SingleExcitation, DoubleExcitation],
     operator_mapper: OpenFermionQubitOperatorMapper,
-) -> FermionOperator:
+) -> Operator:
+    r"""Create an anti-hermitian :class:`~quri_parts.core.operator.Operator`
+    according to the assigned index.
+
+    - If there are 2 excitation indices (i, a), it creates the
+      :class:`~quri_parts.core.operator.Operator` for
+      :math:`c_a^{\dagger} c_i - c_i^{\dagger} c_a`.
+
+    - If there are 4 excitation indices (i, j, b, a), it creates the
+      :class:`~quri_parts.core.operator.Operator` for
+      :math:`c_a^{\dagger} c_b^{\dagger} c_j c_i - c_i^{\dagger}c_j^{\dagger} c_b c_a`.
+    """
     op = FermionOperator()
     if len(excitation_indices) == 2:
         op += FermionOperator(
             ((excitation_indices[1], 1), (excitation_indices[0], 0)), 1.0
         )
         op += FermionOperator(
             ((excitation_indices[0], 1), (excitation_indices[1], 0)), -1.0
```

### Comparing `quri_parts_openfermion-0.9.2/PKG-INFO` & `quri_parts_openfermion-17.0.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-openfermion
-Version: 0.9.2
+Version: 17.0.0
 Summary: A support library for using OpenFermion with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 License: Apache-2.0
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
```

