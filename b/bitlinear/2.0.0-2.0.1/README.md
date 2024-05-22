# Comparing `tmp/bitlinear-2.0.0.tar.gz` & `tmp/bitlinear-2.0.1.tar.gz`

## Comparing `bitlinear-2.0.0.tar` & `bitlinear-2.0.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/__init__.py
--rw-r--r--   0        0        0     3239 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/kernels.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.0/bitlinear/measures.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.0/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.0/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.0/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.0/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/__init__.py
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/kernels.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.1/bitlinear/measures.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.1/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.1/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.1/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.1/PKG-INFO
```

### Comparing `bitlinear-2.0.0/bitlinear/bitlinear.py` & `bitlinear-2.0.1/bitlinear/bitlinear.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,21 +1,25 @@
+from collections.abc import Sequence
 from math import ceil
 import re
 import torch
 import torch.nn as nn
 
 from .kernels import TorchLinear
 from .measures import AbsMax, AbsMedian
 
 def round_clamp(input, range):
     return (input.round().clamp(range[0], range[1]) - input).detach() + input
 
 def scale(input, range, measure, keepdim, eps):
     return max(abs(k) for k in range) / measure(input.detach(), keepdim=keepdim).clamp_(min=eps)
 
+def range_from_bits(bits):
+    return (ceil(-2**(bits-1)), ceil(2**(bits-1)-1))
+
 class BitLinear(nn.Linear):
     def __init__(
             self,
             in_features,
             out_features,
             bias=True,
             device=None,
@@ -34,16 +38,16 @@
             device=device,
             dtype=dtype,
         )
         self.eps = eps
         self.kernel = kernel
         self.weight_measure = weight_measure
         self.activation_measure = activation_measure
-        self.activation_range = activation_range if isinstance(activation_range, tuple) else (ceil(-2**(activation_range-1)), ceil(2**(activation_range-1)-1))
-        self.weight_range = weight_range if isinstance(weight_range, tuple) else (ceil(-2**(weight_range-1)), ceil(2**(weight_range-1)-1))
+        self.activation_range = activation_range if isinstance(activation_range, Sequence) else range_from_bits(activation_range)
+        self.weight_range = weight_range if isinstance(weight_range, Sequence) else range_from_bits(weight_range)
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_range={self.weight_range}, weight_measure={self.weight_measure}, activation_range={self.activation_range}, activation_measure={self.activation_measure}, kernel={self.kernel})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
         x_scale = scale(x_norm, self.activation_range, self.activation_measure, True, self.eps)
```

### Comparing `bitlinear-2.0.0/bitlinear/kernels.py` & `bitlinear-2.0.1/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.0/bitlinear/measures.py` & `bitlinear-2.0.1/bitlinear/measures.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.0/LICENSE` & `bitlinear-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.0/README.md` & `bitlinear-2.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.0/pyproject.toml` & `bitlinear-2.0.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "2.0.0"
+version = "2.0.1"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-2.0.0/PKG-INFO` & `bitlinear-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 2.0.0
+Version: 2.0.1
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

