# Comparing `tmp/bitlinear-2.0.2.tar.gz` & `tmp/bitlinear-2.0.3.tar.gz`

## Comparing `bitlinear-2.0.2.tar` & `bitlinear-2.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/__init__.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/bitlinear.py
--rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/kernels.py
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.2/bitlinear/measures.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.2/.gitignore
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.2/LICENSE
--rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.2/README.md
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.2/pyproject.toml
--rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 bitlinear-2.0.3/bitlinear/__init__.py
+-rw-r--r--   0        0        0     3905 2020-02-02 00:00:00.000000 bitlinear-2.0.3/bitlinear/bitlinear.py
+-rw-r--r--   0        0        0     2509 2020-02-02 00:00:00.000000 bitlinear-2.0.3/bitlinear/kernels.py
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 bitlinear-2.0.3/bitlinear/measures.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 bitlinear-2.0.3/.gitignore
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 bitlinear-2.0.3/LICENSE
+-rw-r--r--   0        0        0     1853 2020-02-02 00:00:00.000000 bitlinear-2.0.3/README.md
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 bitlinear-2.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2436 2020-02-02 00:00:00.000000 bitlinear-2.0.3/PKG-INFO
```

### Comparing `bitlinear-2.0.2/bitlinear/bitlinear.py` & `bitlinear-2.0.3/bitlinear/bitlinear.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,41 +36,54 @@
             out_features=out_features,
             bias=bias,
             device=device,
             dtype=dtype,
         )
         self.eps = eps
         self.weight_range = weight_range if isinstance(weight_range, Sequence) else range_from_bits(weight_range)
-        self.weight_measure = eval(weight_measure) if isinstance(weight_measure, str) else weight_measure
+        self.weight_measure = eval(weight_measure)() if isinstance(weight_measure, str) else weight_measure
         self.activation_range = activation_range if isinstance(activation_range, Sequence) else range_from_bits(activation_range)
-        self.activation_measure = eval(activation_measure) if isinstance(activation_measure, str) else activation_measure
-        self.kernel = eval(kernel) if isinstance(kernel, str) else kernel
+        self.activation_measure = eval(activation_measure)() if isinstance(activation_measure, str) else activation_measure
+        self.kernel = eval(kernel)() if isinstance(kernel, str) else kernel
 
     def __repr__(self):
         return f"BitLinear(in_features={self.in_features}, out_features={self.out_features}, bias={self.bias is not None}, eps={self.eps}, weight_range={self.weight_range}, weight_measure={self.weight_measure}, activation_range={self.activation_range}, activation_measure={self.activation_measure}, kernel={self.kernel})"
 
     def forward(self, x):
         x_norm = torch.layer_norm(x, x.size()[1:])
         x_scale = scale(x_norm, self.activation_range, self.activation_measure, True, self.eps)
         x_quant = round_clamp(x_norm * x_scale, self.activation_range)
         w_scale = scale(self.weight, self.weight_range, self.weight_measure, False, self.eps)
         w_quant = round_clamp(self.weight * w_scale, self.weight_range)
         y_quant = self.kernel(x_quant, w_quant, self.bias)
         y = y_quant / (w_scale * x_scale)
         return y
 
-def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}, match_name=None, prefix=""):
+def replace_modules(model, old_class=nn.Linear, new_class=BitLinear, new_class_kwargs={}, match_name="", prefix=""):
     for name, module in model.named_children():
         qual_name = prefix + "." + name
-        if isinstance(module, old_class) and (match_name is None or re.search(match_name, qual_name) is not None):
+        if isinstance(module, old_class) and re.search(match_name, qual_name) is not None:
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
             replace_modules(module, old_class, new_class, new_class_kwargs, match_name, prefix=qual_name)
+
+def bitlinearize(model, old_class=nn.Linear, new_class=BitLinear, replacements=[{}]):
+    for replacement in replacements:
+        replacement = dict(replacement)
+        match_name = replacement.pop("match_name", "")
+        replace_modules(
+            model=model,
+            old_class=old_class,
+            new_class=new_class,
+            new_class_kwargs=replacement,
+            match_name=match_name,
+        )
+    return model
```

### Comparing `bitlinear-2.0.2/bitlinear/kernels.py` & `bitlinear-2.0.3/bitlinear/kernels.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.2/bitlinear/measures.py` & `bitlinear-2.0.3/bitlinear/measures.py`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.2/LICENSE` & `bitlinear-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.2/README.md` & `bitlinear-2.0.3/README.md`

 * *Files identical despite different names*

### Comparing `bitlinear-2.0.2/pyproject.toml` & `bitlinear-2.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "bitlinear"
-version = "2.0.2"
+version = "2.0.3"
 authors = [
   { name = "Peter Schneider-Kamp" }
 ]
 
 description = "An production-ready implementation of 1.58 bit quantization-aware training and inference."
 readme = "README.md"
 requires-python = ">=3.10"
```

### Comparing `bitlinear-2.0.2/PKG-INFO` & `bitlinear-2.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: bitlinear
-Version: 2.0.2
+Version: 2.0.3
 Summary: An production-ready implementation of 1.58 bit quantization-aware training and inference.
 Project-URL: Homepage, https://github.com/schneiderkamplab/bitlinear
 Project-URL: Bug Tracker, https://github.com/schneiderkamplab/bitlinear/issues
 Author: Peter Schneider-Kamp
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

