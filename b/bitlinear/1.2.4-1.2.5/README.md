# Comparing `tmp/bitlinear-1.2.4.tar.gz` & `tmp/bitlinear-1.2.5.tar.gz`

## Comparing `bitlinear-1.2.4.tar` & `bitlinear-1.2.5.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.4/bitlinear/__init__.py
--rw-r--r--   0        0        0     2982 2020-02-02 00:00:00.000000 bitlinear-1.2.4/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.4/bitlinear/kernels.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.4/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.4/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.4/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.4/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.4/PKG-INFO
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/__init__.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-1.2.5/bitlinear/kernels.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-1.2.5/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-1.2.5/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-1.2.5/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-1.2.5/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-1.2.5/PKG-INFO
```

### Comparing `bitlinear-1.2.4/bitlinear/bitlinear.py` & `bitlinear-1.2.5/bitlinear/bitlinear.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from math import ceil
+import re
 import torch
 import torch.nn as nn
 
 from .kernels import TorchLinear
 
 def round_clamp(input, min, max):
     return (input.round().clamp(min, max) - input).detach() + input
@@ -51,22 +52,23 @@
         x_quant = round_clamp(x_norm * x_scale, self.x_min, self.x_max)
         w_scale = 1 / self.measure(self.weight.detach().abs()).clamp_(min=self.eps)
         w_quant = round_clamp(self.weight * w_scale, self.w_min, self.w_max)
         y_quant = self.kernel(x_quant, w_quant, self.bias)
         y = y_quant / (w_scale * x_scale)
         return y
 
-def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}):
+def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}, match_name=None, prefix=""):
     for name, module in model.named_children():
-        if isinstance(module, old_class):
+        qual_name = prefix + "." + name
+        if isinstance(module, old_class) and (match_name is None or re.search(match_name, qual_name) is not None):
             kwargs = dict(new_class_kwargs)
             kwargs["in_features"] = module.in_features
             kwargs["out_features"] = module.out_features
             bias = getattr(module, "bias", None) is not None
             kwargs["bias"] = bias
             new_module = new_class(**kwargs)
             new_module.weight.data = module.weight.data
             if bias:
                 new_module.bias.data = module.bias.data
             setattr(model, name, new_module)
         else:
-            replace_modules(module, old_class, new_class, new_class_kwargs)
+            replace_modules(module, old_class, new_class, new_class_kwargs, match_name, prefix=qual_name)
```

### Comparing `bitlinear-1.2.4/bitlinear/kernels.py` & `bitlinear-1.2.5/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.4/LICENSE` & `bitlinear-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.4/README.md` & `bitlinear-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-1.2.4/pyproject.toml` & `bitlinear-1.2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "1.2.4"
+version = "1.2.5"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-1.2.4/PKG-INFO` & `bitlinear-1.2.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 1.2.4
+Version: 1.2.5
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

