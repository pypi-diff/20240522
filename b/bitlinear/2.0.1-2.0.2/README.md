# Comparing `tmp/bitlinear-2.0.1.tar.gz` & `tmp/bitlinear-2.0.2.tar.gz`

## Comparing `bitlinear-2.0.1.tar` & `bitlinear-2.0.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/__init__.py
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/kernels.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/measures.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.1/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.1/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.1/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/__init__.py
+-rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/kernels.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/measures.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.2/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.2/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.2/PKG-INFO
```

### Comparing `bitlinear-2.0.1/bitlinear/bitlinear.py` & `bitlinear-2.0.2/bitlinear/bitlinear.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from collections.abc import Sequence
 from math import ceil
 import re
 import torch
 import torch.nn as nn
 
 from .kernels import TorchLinear
-from .measures import AbsMax, AbsMedian
+from .measures import AbsMax, AbsMedian, AbsMean
 
 def round_clamp(input, range):
     return (input.round().clamp(range[0], range[1]) - input).detach() + input
 
 def scale(input, range, measure, keepdim, eps):
     return max(abs(k) for k in range) / measure(input.detach(), keepdim=keepdim).clamp_(min=eps)
 
@@ -22,32 +22,32 @@
             in_features,
             out_features,
             bias=True,
             device=None,
             dtype=None,
             eps=1e-5,
             weight_range=1.58,
-            weight_measure=AbsMedian(),
+            weight_measure="AbsMedian",
             activation_range=8,
-            activation_measure=AbsMax(),
-            kernel=TorchLinear(),
+            activation_measure="AbsMax",
+            kernel="TorchLinear",
         ):
         super(BitLinear, self).__init__(
             in_features=in_features,
             out_features=out_features,
             bias=bias,
             device=device,
             dtype=dtype,
         )
         self.eps = eps
-        self.kernel = kernel
-        self.weight_measure = weight_measure
-        self.activation_measure = activation_measure
-        self.activation_range = activation_range if isinstance(activation_range, Sequence) else range_from_bits(activation_range)
         self.weight_range = weight_range if isinstance(weight_range, Sequence) else range_from_bits(weight_range)
+        self.weight_measure = eval(weight_measure) if isinstance(weight_measure, str) else weight_measure
+        self.activation_range = activation_range if isinstance(activation_range, Sequence) else range_from_bits(activation_range)
+        self.activation_measure = eval(activation_measure) if isinstance(activation_measure, str) else activation_measure
+        self.kernel = eval(kernel) if isinstance(kernel, str) else kernel
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_range={self.weight_range}, weight_measure={self.weight_measure}, activation_range={self.activation_range}, activation_measure={self.activation_measure}, kernel={self.kernel})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
         x_scale = scale(x_norm, self.activation_range, self.activation_measure, True, self.eps)
```

### Comparing `bitlinear-2.0.1/bitlinear/kernels.py` & `bitlinear-2.0.2/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.1/bitlinear/measures.py` & `bitlinear-2.0.2/bitlinear/measures.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.1/LICENSE` & `bitlinear-2.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.1/README.md` & `bitlinear-2.0.2/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.1/pyproject.toml` & `bitlinear-2.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "2.0.1"
+version = "2.0.2"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-2.0.1/PKG-INFO` & `bitlinear-2.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 2.0.1
+Version: 2.0.2
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

