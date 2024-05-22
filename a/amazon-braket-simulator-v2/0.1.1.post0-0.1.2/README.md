# Comparing `tmp/amazon_braket_simulator_v2-0.1.1.post0.tar.gz` & `tmp/amazon_braket_simulator_v2-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "amazon_braket_simulator_v2-0.1.1.post0.tar", last modified: Wed May 15 16:13:08 2024, max compression
+gzip compressed data, was "amazon_braket_simulator_v2-0.1.2.tar", last modified: Wed May 22 16:14:39 2024, max compression
```

## Comparing `amazon_braket_simulator_v2-0.1.1.post0.tar` & `amazon_braket_simulator_v2-0.1.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:13:08.365182 amazon_braket_simulator_v2-0.1.1.post0/
--rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-05-15 16:13:08.365182 amazon_braket_simulator_v2-0.1.1.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-15 16:13:08.365182 amazon_braket_simulator_v2-0.1.1.post0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:13:08.361183 amazon_braket_simulator_v2-0.1.1.post0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:13:08.365182 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16023 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-15 16:13:08.000000 amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:13:08.361183 amazon_braket_simulator_v2-0.1.1.post0/src/braket/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/juliapkg.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 16:13:08.361183 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/base_simulator_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/density_matrix_simulator_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     4436 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/julia_import.py
--rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-15 16:12:58.000000 amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/state_vector_simulator_v2.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:39.776382 amazon_braket_simulator_v2-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    10142 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-22 16:14:39.776382 amazon_braket_simulator_v2-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1474 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-22 16:14:39.776382 amazon_braket_simulator_v2-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:39.768382 amazon_braket_simulator_v2-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:39.772382 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16017 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-22 16:14:39.000000 amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:39.772382 amazon_braket_simulator_v2-0.1.2/src/braket/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/juliapkg.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:14:39.772382 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6346 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/base_simulator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11042 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/density_matrix_simulator_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/julia_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10748 2024-05-22 16:14:29.000000 amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/state_vector_simulator_v2.py
```

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/LICENSE` & `amazon_braket_simulator_v2-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/PKG-INFO` & `amazon_braket_simulator_v2-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-simulator-v2
-Version: 0.1.1.post0
+Version: 0.1.2
 Summary: Local simulation of quantum circuits
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/README.md` & `amazon_braket_simulator_v2-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/pyproject.toml` & `amazon_braket_simulator_v2-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/PKG-INFO` & `amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: amazon-braket-simulator-v2
-Version: 0.1.1.post0
+Version: 0.1.2
 Summary: Local simulation of quantum circuits
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt` & `amazon_braket_simulator_v2-0.1.2/src/amazon_braket_simulator_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/base_simulator_v2.py` & `amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/base_simulator_v2.py`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/density_matrix_simulator_v2.py` & `amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/density_matrix_simulator_v2.py`

 * *Files identical despite different names*

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/julia_import.py` & `amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/julia_import.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     )
 else:
     # Required to avoid segfaults (https://juliapy.github.io/PythonCall.jl/dev/faq/)
     if os.environ.get("PYTHON_JULIACALL_HANDLE_SIGNALS", "yes") != "yes":
         warnings.warn(
             "`PYTHON_JULIACALL_HANDLE_SIGNALS` environment variable "
             + "is set to something other than 'yes' or ''. "
-            + +"You will experience segfaults if running with Julia multithreading."
+            + "You will experience segfaults if running with Julia multithreading."
         )
 
     if os.environ.get("PYTHON_JULIACALL_THREADS", "auto") != "auto":
         warnings.warn(
             "`PYTHON_JULIACALL_THREADS` environment variable is set to "
             + "something other than `auto`, so `amazon-braket-simulator-v2` "
             + "was not able to set it."
@@ -32,92 +32,102 @@
         ("PYTHON_JULIACALL_THREADS", "auto"),
         ("PYTHON_JULIACALL_OPTLEVEL", "3"),
         # let the user's Conda/Pip handle installing things
         ("JULIA_CONDAPKG_BACKEND", "Null"),
     ):
         os.environ[k] = os.environ.get(k, default)
 
-import braket.default_simulator.gate_operations as gates
-import braket.default_simulator.noise_operations as noises
-from braket.default_simulator.openqasm.circuit import Circuit
 import juliacall
 
 jl = juliacall.Base.Module()
 
 jl.seval("using PythonCall, BraketSimulator")
 jl.seval("using PythonCall: Py, pyconvert")
 jlBraketSimulator = jl.BraketSimulator
 
-# at init run many commonly used gates and noises to force compilation
-# for this Python session
-# must be done at init because each new Python session has a separate handle and
-# seems to invalidate old methods
-
-circuit = Circuit()
-for instruction in (
-    gates.Hadamard(targets=[0]),
-    gates.RotX(targets=[0], angle=0.1),
-    gates.RotY(targets=[1], angle=0.2),
-    gates.RotZ(targets=[0], angle=0.1),
-    gates.PhaseShift(targets=[0], angle=0.1),
-    gates.PRx(targets=[0], angle_1=0.1, angle_2=0.2),
-    gates.GPi(targets=[0], angle=0.1),
-    gates.GPi2(targets=[0], angle=0.1),
-    gates.PauliX(targets=[0]),
-    gates.PauliY(targets=[1]),
-    gates.PauliZ(targets=[0]),
-    gates.V(targets=[0]),
-    gates.Vi(targets=[1]),
-    gates.S(targets=[0]),
-    gates.Si(targets=[1]),
-    gates.T(targets=[0]),
-    gates.Ti(targets=[1]),
-    gates.Identity(targets=[1]),
-    gates.Swap(targets=[0, 1]),
-    gates.ISwap(targets=[0, 1]),
-    gates.PSwap(targets=[0, 1], angle=0.1),
-    gates.ECR(targets=[0, 1]),
-    gates.CX(targets=[0, 1]),
-    gates.CY(targets=[0, 1]),
-    gates.CZ(targets=[0, 1]),
-    gates.CV(targets=[0, 1]),
-    gates.MS(targets=[0, 1], angle_1=0.1, angle_2=0.2, angle_3=0.3),
-    gates.XX(targets=[0, 1], angle=0.1),
-    gates.XY(targets=[0, 1], angle=0.1),
-    gates.YY(targets=[0, 1], angle=0.1),
-    gates.ZZ(targets=[0, 1], angle=0.1),
-    gates.CPhaseShift(targets=[0, 1], angle=0.1),
-    gates.CPhaseShift00(targets=[0, 1], angle=0.1),
-    gates.CPhaseShift10(targets=[0, 1], angle=0.1),
-    gates.CPhaseShift01(targets=[0, 1], angle=0.1),
-    gates.CCNot(targets=[0, 1, 2]),
-    gates.CSwap(targets=[0, 1, 2]),
-):
-    circuit.add_instruction(instruction)
-
-jl.simulate(
-    jlBraketSimulator.StateVectorSimulator(0, 0), [circuit], 3, 100, measured_qubits=[]
-)
-
-circuit = Circuit()
-for instruction in (
-    gates.Hadamard(targets=[0]),
-    gates.CX(targets=[0, 1]),
-    noises.BitFlip(targets=[0], probability=0.1),
-    noises.PhaseFlip(targets=[0], probability=0.1),
-    noises.PauliChannel(targets=[0], probX=0.1, probY=0.2, probZ=0.3),
-    noises.Depolarizing(targets=[0], probability=0.1),
-    noises.TwoQubitDepolarizing(targets=[0, 1], probability=0.1),
-    noises.TwoQubitDephasing(targets=[0, 1], probability=0.1),
-    noises.AmplitudeDamping(targets=[0], gamma=0.1),
-    noises.PhaseDamping(targets=[0], gamma=0.1),
-    noises.GeneralizedAmplitudeDamping(targets=[0], gamma=0.1, probability=0.2),
-):
-    circuit.add_instruction(instruction)
-
-jl.simulate(
-    jlBraketSimulator.DensityMatrixSimulator(0, 0),
-    [circuit],
-    3,
-    100,
-    measured_qubits=[],
-)
+
+def precompile():
+    # at init run many commonly used gates and noises to force compilation
+    # for this Python session
+    # must be done at init because each new Python session has a separate handle and
+    # seems to invalidate old methods
+    import braket.default_simulator.gate_operations as gates
+    import braket.default_simulator.noise_operations as noises
+    from braket.default_simulator.openqasm.circuit import Circuit
+
+    circuit = Circuit()
+    for instruction in (
+        gates.Hadamard(targets=[0]),
+        gates.RotX(targets=[0], angle=0.1),
+        gates.RotY(targets=[1], angle=0.2),
+        gates.RotZ(targets=[0], angle=0.1),
+        gates.PhaseShift(targets=[0], angle=0.1),
+        gates.PRx(targets=[0], angle_1=0.1, angle_2=0.2),
+        gates.GPi(targets=[0], angle=0.1),
+        gates.GPi2(targets=[0], angle=0.1),
+        gates.PauliX(targets=[0]),
+        gates.PauliY(targets=[1]),
+        gates.PauliZ(targets=[0]),
+        gates.V(targets=[0]),
+        gates.Vi(targets=[1]),
+        gates.S(targets=[0]),
+        gates.Si(targets=[1]),
+        gates.T(targets=[0]),
+        gates.Ti(targets=[1]),
+        gates.Identity(targets=[1]),
+        gates.Swap(targets=[0, 1]),
+        gates.ISwap(targets=[0, 1]),
+        gates.PSwap(targets=[0, 1], angle=0.1),
+        gates.ECR(targets=[0, 1]),
+        gates.CX(targets=[0, 1]),
+        gates.CY(targets=[0, 1]),
+        gates.CZ(targets=[0, 1]),
+        gates.CV(targets=[0, 1]),
+        gates.MS(targets=[0, 1], angle_1=0.1, angle_2=0.2, angle_3=0.3),
+        gates.XX(targets=[0, 1], angle=0.1),
+        gates.XY(targets=[0, 1], angle=0.1),
+        gates.YY(targets=[0, 1], angle=0.1),
+        gates.ZZ(targets=[0, 1], angle=0.1),
+        gates.CPhaseShift(targets=[0, 1], angle=0.1),
+        gates.CPhaseShift00(targets=[0, 1], angle=0.1),
+        gates.CPhaseShift10(targets=[0, 1], angle=0.1),
+        gates.CPhaseShift01(targets=[0, 1], angle=0.1),
+        gates.CCNot(targets=[0, 1, 2]),
+        gates.CSwap(targets=[0, 1, 2]),
+    ):
+        circuit.add_instruction(instruction)
+
+    jl.simulate(
+        jlBraketSimulator.StateVectorSimulator(0, 0),
+        [circuit],
+        3,
+        100,
+        measured_qubits=[],
+    )
+
+    circuit = Circuit()
+    for instruction in (
+        gates.Hadamard(targets=[0]),
+        gates.CX(targets=[0, 1]),
+        noises.BitFlip(targets=[0], probability=0.1),
+        noises.PhaseFlip(targets=[0], probability=0.1),
+        noises.PauliChannel(targets=[0], probX=0.1, probY=0.2, probZ=0.3),
+        noises.Depolarizing(targets=[0], probability=0.1),
+        noises.TwoQubitDepolarizing(targets=[0, 1], probability=0.1),
+        noises.TwoQubitDephasing(targets=[0, 1], probability=0.1),
+        noises.AmplitudeDamping(targets=[0], gamma=0.1),
+        noises.PhaseDamping(targets=[0], gamma=0.1),
+        noises.GeneralizedAmplitudeDamping(targets=[0], gamma=0.1, probability=0.2),
+    ):
+        circuit.add_instruction(instruction)
+
+    jl.simulate(
+        jlBraketSimulator.DensityMatrixSimulator(0, 0),
+        [circuit],
+        3,
+        100,
+        measured_qubits=[],
+    )
+
+
+if os.environ.get("BRAKET_SIMV2_PRECOMPILE", False):
+    precompile()
```

### Comparing `amazon_braket_simulator_v2-0.1.1.post0/src/braket/simulator_v2/state_vector_simulator_v2.py` & `amazon_braket_simulator_v2-0.1.2/src/braket/simulator_v2/state_vector_simulator_v2.py`

 * *Files identical despite different names*

