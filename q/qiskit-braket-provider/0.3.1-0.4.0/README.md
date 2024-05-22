# Comparing `tmp/qiskit_braket_provider-0.3.1.tar.gz` & `tmp/qiskit_braket_provider-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_braket_provider-0.3.1.tar", last modified: Tue May  7 20:16:20 2024, max compression
+gzip compressed data, was "qiskit_braket_provider-0.4.0.tar", last modified: Wed May 22 21:55:16 2024, max compression
```

## Comparing `qiskit_braket_provider-0.3.1.tar` & `qiskit_braket_provider-0.4.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-07 20:16:20.152283 qiskit_braket_provider-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider/
--rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23041 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_quantum_task.py
--rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-07 20:16:20.000000 qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-07 20:16:20.152283 qiskit_braket_provider-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:20.148283 qiskit_braket_provider-0.3.1/tests/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/mocks.py
--rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-07 20:16:14.000000 qiskit_braket_provider-0.3.1/tests/providers/test_braket_quantum_task.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11416 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.343536 qiskit_braket_provider-0.4.0/qiskit_braket_provider/
+-rw-r--r--   0 runner    (1001) docker     (127)      262 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23230 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13449 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6873 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_quantum_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-22 21:55:16.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-05-22 21:55:16.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:55:16.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-05-22 21:55:16.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 21:55:16.000000 qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:16.347536 qiskit_braket_provider-0.4.0/tests/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4922 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/mocks.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25457 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/test_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12065 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/test_braket_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7076 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/test_braket_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-05-22 21:55:07.000000 qiskit_braket_provider-0.4.0/tests/providers/test_braket_quantum_task.py
```

### Comparing `qiskit_braket_provider-0.3.1/LICENSE.txt` & `qiskit_braket_provider-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/PKG-INFO` & `qiskit_braket_provider-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit_braket_provider
-Version: 0.3.1
+Version: 0.4.0
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.3.1/README.md` & `qiskit_braket_provider-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/__init__.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/adapter.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     FreeParameter,
     FreeParameterExpression,
     Instruction,
     measure,
 )
 from braket.device_schema import DeviceActionType, OpenQASMDeviceActionProperties
 from braket.device_schema.ionq import IonqDeviceCapabilities
+from braket.device_schema.iqm import IqmDeviceCapabilities
 from braket.device_schema.oqc import OqcDeviceCapabilities
 from braket.device_schema.rigetti import RigettiDeviceCapabilities
 from braket.device_schema.simulators import GateModelSimulatorDeviceCapabilities
 from braket.devices import LocalSimulator
 from braket.ir.openqasm.modifiers import Control
 from qiskit import QuantumCircuit, transpile
 from qiskit.circuit import ControlledGate
@@ -265,15 +266,20 @@
     properties = device.properties
     if isinstance(properties, GateModelSimulatorDeviceCapabilities):
         return _simulator_target(
             f"Target for Amazon Braket simulator: {device.name}", properties
         )
     elif isinstance(
         properties,
-        (IonqDeviceCapabilities, RigettiDeviceCapabilities, OqcDeviceCapabilities),
+        (
+            IonqDeviceCapabilities,
+            RigettiDeviceCapabilities,
+            OqcDeviceCapabilities,
+            IqmDeviceCapabilities,
+        ),
     ):
         return _qpu_target(f"Target for Amazon Braket QPU: {device.name}", properties)
 
     raise QiskitBraketException(
         f"Cannot convert to target. "
         f"{properties.__class__} device capabilities are not supported yet."
     )
@@ -295,15 +301,18 @@
     target.add_instruction(Measure())
     return target
 
 
 def _qpu_target(
     description: str,
     properties: Union[
-        IonqDeviceCapabilities, RigettiDeviceCapabilities, OqcDeviceCapabilities
+        IonqDeviceCapabilities,
+        RigettiDeviceCapabilities,
+        OqcDeviceCapabilities,
+        IqmDeviceCapabilities,
     ],
 ):
     qubit_count = properties.paradigm.qubitCount
     target = Target(description=description, num_qubits=qubit_count)
     action_properties = (
         properties.action.get(DeviceActionType.OPENQASM)
         if properties.action.get(DeviceActionType.OPENQASM)
```

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_backend.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_job.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_provider.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider/providers/braket_quantum_task.py` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider/providers/braket_quantum_task.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/PKG-INFO` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qiskit-braket-provider
-Version: 0.3.1
+Version: 0.4.0
 Summary: Qiskit-Braket provider to execute Qiskit programs on AWS quantum computing hardware devices through Amazon Braket.
 Home-page: UNKNOWN
 License: UNKNOWN
 Keywords: qiskit braket sdk quantum
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `qiskit_braket_provider-0.3.1/qiskit_braket_provider.egg-info/SOURCES.txt` & `qiskit_braket_provider-0.4.0/qiskit_braket_provider.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/setup.py` & `qiskit_braket_provider-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/tests/providers/mocks.py` & `qiskit_braket_provider-0.4.0/tests/providers/mocks.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/tests/providers/test_adapter.py` & `qiskit_braket_provider-0.4.0/tests/providers/test_adapter.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/tests/providers/test_braket_backend.py` & `qiskit_braket_provider-0.4.0/tests/providers/test_braket_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/tests/providers/test_braket_provider.py` & `qiskit_braket_provider-0.4.0/tests/providers/test_braket_provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_braket_provider-0.3.1/tests/providers/test_braket_quantum_task.py` & `qiskit_braket_provider-0.4.0/tests/providers/test_braket_quantum_task.py`

 * *Files identical despite different names*

