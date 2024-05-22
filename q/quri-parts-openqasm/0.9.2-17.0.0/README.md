# Comparing `tmp/quri_parts_openqasm-0.9.2.tar.gz` & `tmp/quri_parts_openqasm-17.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quri_parts_openqasm-0.9.2.tar", max compression
+gzip compressed data, was "quri_parts_openqasm-17.0.0.tar", max compression
```

## Comparing `quri_parts_openqasm-0.9.2.tar` & `quri_parts_openqasm-17.0.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11358 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/LICENSE
--rw-r--r--   0        0        0      351 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/README.md
--rw-r--r--   0        0        0     1015 2023-03-29 07:37:31.955011 quri_parts_openqasm-0.9.2/pyproject.toml
--rw-r--r--   0        0        0       34 2023-03-29 07:37:31.159007 quri_parts_openqasm-0.9.2/quri_parts/openqasm/NOTICE
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/__init__.py
--rw-r--r--   0        0        0     5518 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/circuit/__init__.py
--rw-r--r--   0        0        0        0 2023-03-29 07:37:19.874951 quri_parts_openqasm-0.9.2/quri_parts/openqasm/py.typed
--rw-r--r--   0        0        0     1089 1970-01-01 00:00:00.000000 quri_parts_openqasm-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    11358 2024-03-19 02:11:01.298138 quri_parts_openqasm-17.0.0/LICENSE
+-rw-r--r--   0        0        0      351 2024-03-19 02:11:01.298138 quri_parts_openqasm-17.0.0/README.md
+-rw-r--r--   0        0        0     1016 2024-03-19 02:11:30.310002 quri_parts_openqasm-17.0.0/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-19 02:11:29.746005 quri_parts_openqasm-17.0.0/quri_parts/openqasm/NOTICE
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_openqasm-17.0.0/quri_parts/openqasm/__init__.py
+-rw-r--r--   0        0        0     5848 2024-03-19 02:11:01.298138 quri_parts_openqasm-17.0.0/quri_parts/openqasm/circuit/__init__.py
+-rw-r--r--   0        0        0        0 2024-03-19 02:11:01.298138 quri_parts_openqasm-17.0.0/quri_parts/openqasm/py.typed
+-rw-r--r--   0        0        0     1090 1970-01-01 00:00:00.000000 quri_parts_openqasm-17.0.0/PKG-INFO
```

### Comparing `quri_parts_openqasm-0.9.2/LICENSE` & `quri_parts_openqasm-17.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quri_parts_openqasm-0.9.2/pyproject.toml` & `quri_parts_openqasm-17.0.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core>=1.0.0", "setuptools"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "quri-parts-openqasm"
-version = "0.9.2"
+version = "17.0.0"
 description = "A support library for using OpenQASM 3 with QURI Parts"
 authors = ["QURI Parts Authors <opensource@qunasys.com>"]
 readme = "README.md"
 repository = "https://github.com/QunaSys/quri-parts"
 documentation = "https://quri-parts.qunasys.com"
 keywords = ["quantum", "quantum computing"]
 classifiers = [
```

### Comparing `quri_parts_openqasm-0.9.2/quri_parts/openqasm/circuit/__init__.py` & `quri_parts_openqasm-17.0.0/quri_parts/openqasm/circuit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,47 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import io
-from typing import TYPE_CHECKING, Mapping
+from typing import TYPE_CHECKING, Callable, Mapping
 
 from quri_parts.circuit import gate_names
 from quri_parts.circuit.gate_names import (
     is_gate_name,
     is_multi_qubit_gate_name,
     is_parametric_gate_name,
     is_single_qubit_gate_name,
     is_three_qubit_gate_name,
     is_two_qubit_gate_name,
 )
+from quri_parts.circuit.transpile import (
+    CircuitTranspiler,
+    PauliDecomposeTranspiler,
+    PauliRotationDecomposeTranspiler,
+    SequentialTranspiler,
+)
 
 if TYPE_CHECKING:
     from quri_parts.circuit import NonParametricQuantumCircuit, QuantumGate
     from quri_parts.circuit.gate_names import (
         ParametricGateNameType,
         SingleQubitGateNameType,
         ThreeQubitGateNameType,
         TwoQubitGateNameType,
     )
 
+
+OpenQASMTranspiler: Callable[[], CircuitTranspiler] = lambda: SequentialTranspiler(
+    [PauliDecomposeTranspiler(), PauliRotationDecomposeTranspiler()]
+)
+
+
 _HEADER = """OPENQASM 3;
 include "stdgates.inc";"""
 _QUBIT_VAR_NAME = "q"
 
 # For information on "stdgates.inc", see https://arxiv.org/abs/2104.14722v2
 
 _single_qubit_gate_stdgates_symbol: Mapping["SingleQubitGateNameType", str] = {
```

### Comparing `quri_parts_openqasm-0.9.2/PKG-INFO` & `quri_parts_openqasm-17.0.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quri-parts-openqasm
-Version: 0.9.2
+Version: 17.0.0
 Summary: A support library for using OpenQASM 3 with QURI Parts
 Home-page: https://github.com/QunaSys/quri-parts
 Keywords: quantum,quantum computing
 Author: QURI Parts Authors
 Author-email: opensource@qunasys.com
 Requires-Python: >=3.9.8,<3.12
 Classifier: Programming Language :: Python :: 3
```

