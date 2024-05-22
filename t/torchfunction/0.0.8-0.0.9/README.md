# Comparing `tmp/torchfunction-0.0.8-py3-none-any.whl.zip` & `tmp/torchfunction-0.0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 5702 bytes, number of entries: 11
--rw-r--r--  2.0 unx       17 b- defN 21-Jun-03 16:14 torchfunction/__init__.py
--rw-r--r--  2.0 unx      516 b- defN 21-Jun-03 16:14 torchfunction/createtensor.py
--rw-r--r--  2.0 unx      656 b- defN 21-Jun-03 16:14 torchfunction/functional.py
--rw-r--r--  2.0 unx      903 b- defN 21-Jun-03 16:14 torchfunction/inspect.py
--rw-r--r--  2.0 unx     1649 b- defN 21-Jun-03 16:14 torchfunction/lossfunc.py
--rw-r--r--  2.0 unx       27 b- defN 21-Jun-03 16:14 torchfunction/nn/__init__.py
--rw-r--r--  2.0 unx     1811 b- defN 21-Jun-03 16:14 torchfunction/nn/linear.py
--rw-r--r--  2.0 unx     3611 b- defN 21-Jun-03 16:14 torchfunction-0.0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 21-Jun-03 16:14 torchfunction-0.0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 21-Jun-03 16:14 torchfunction-0.0.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      898 b- defN 21-Jun-03 16:14 torchfunction-0.0.8.dist-info/RECORD
-11 files, 10194 bytes uncompressed, 4172 bytes compressed:  59.1%
+Zip file size: 5912 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       17 b- defN 21-Jun-04 04:11 torchfunction/__init__.py
+-rw-r--r--  2.0 unx      516 b- defN 21-Jun-04 04:11 torchfunction/createtensor.py
+-rw-r--r--  2.0 unx      656 b- defN 21-Jun-04 04:11 torchfunction/functional.py
+-rw-r--r--  2.0 unx      903 b- defN 21-Jun-04 04:11 torchfunction/inspect.py
+-rw-r--r--  2.0 unx     1649 b- defN 21-Jun-04 04:11 torchfunction/lossfunc.py
+-rw-r--r--  2.0 unx       27 b- defN 21-Jun-04 04:11 torchfunction/nn/__init__.py
+-rw-r--r--  2.0 unx     3100 b- defN 21-Jun-04 04:11 torchfunction/nn/linear.py
+-rw-r--r--  2.0 unx     3611 b- defN 21-Jun-04 04:11 torchfunction-0.0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 21-Jun-04 04:11 torchfunction-0.0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 21-Jun-04 04:11 torchfunction-0.0.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      898 b- defN 21-Jun-04 04:11 torchfunction-0.0.9.dist-info/RECORD
+11 files, 11483 bytes uncompressed, 4382 bytes compressed:  61.8%
```

## zipnote {}

```diff
@@ -15,20 +15,20 @@
 
 Filename: torchfunction/nn/__init__.py
 Comment: 
 
 Filename: torchfunction/nn/linear.py
 Comment: 
 
-Filename: torchfunction-0.0.8.dist-info/METADATA
+Filename: torchfunction-0.0.9.dist-info/METADATA
 Comment: 
 
-Filename: torchfunction-0.0.8.dist-info/WHEEL
+Filename: torchfunction-0.0.9.dist-info/WHEEL
 Comment: 
 
-Filename: torchfunction-0.0.8.dist-info/top_level.txt
+Filename: torchfunction-0.0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: torchfunction-0.0.8.dist-info/RECORD
+Filename: torchfunction-0.0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## torchfunction/nn/linear.py

```diff
@@ -1,48 +1,76 @@
 from torch import nn
 from torch.nn.parameter import Parameter
 import torch
 from torch import Tensor
 import torch.nn.init as init
 import torch.nn.functional as F
+from pyctlib import vector
 
 class Linear(nn.Module):
 
     __constants__ = ['in_features', 'out_features']
     in_features: int
     out_features: int
     weight: Tensor
 
-    def __init__(self, in_features: int, out_features: int, bias: bool = True, activation="ReLU") -> None:
+    def __init__(self, in_features: int, out_features: int, bias: bool = True, activation="ReLU", hidden_dim=None) -> None:
         super(Linear, self).__init__()
         self.in_features = in_features
         self.out_features = out_features
-        self.weight = Parameter(torch.zeros(out_features, in_features))
-        if bias:
-            self.bias = Parameter(torch.zeros(out_features))
+        self.hidden_dim = hidden_dim
+        if hidden_dim is None:
+            self.weight = Parameter(torch.zeros(out_features, in_features))
+            if bias:
+                self.bias = Parameter(torch.zeros(out_features))
+            else:
+                self.register_parameter('bias', None)
         else:
-            self.register_parameter('bias', None)
+            temp_dim = vector(in_features, *vector(hidden_dim), out_features)
+            self.weight = nn.ParameterList(temp_dim.map_k(lambda in_dim, out_dim: Parameter(torch.zeros(out_dim, in_dim)), 2))
+            if bias:
+                self.bias = nn.ParameterList(temp_dim.map_k(lambda in_dim, out_dim: Parameter(torch.zeros(out_dim)), 2))
+            else:
+                self.register_parameter('bias', None)
         # print(self.weight)
         if activation == "ReLU":
             self.activation = nn.ReLU()
         else:
             self.activation = activation
         self.reset_parameters()
         # print(self.weight)
 
     def reset_parameters(self) -> None:
-        if isinstance(self.activation, torch.nn.ReLU):
-            init.kaiming_normal_(self.weight, a=0, mode='fan_in', nonlinearity='relu')
+        if self.hidden_dim is None:
+            if isinstance(self.activation, torch.nn.ReLU):
+                init.kaiming_normal_(self.weight, a=0, mode='fan_in', nonlinearity='relu')
+            else:
+                init.xavier_normal_(self.weight)
         else:
-            init.xavier_normal_(self.weight)
+            if isinstance(self.activation, torch.nn.ReLU):
+                for w in self.weight:
+                    init.kaiming_normal_(w, a=0, mode='fan_in', nonlinearity='relu')
+            else:
+                for w in self.weight:
+                    init.xavier_normal_(w)
 
     def forward(self, input: Tensor) -> Tensor:
-        if self.activation is None:
-            return F.linear(input, self.weight, self.bias)
+        if self.hidden_dim is None:
+            if self.activation is None:
+                return F.linear(input, self.weight, self.bias)
+            else:
+                return self.activation(F.linear(input, self.weight, self.bias))
         else:
-            return self.activation(F.linear(input, self.weight, self.bias))
+            h = input
+            if self.bias is None:
+                for w in self.weight:
+                    h = self.activation(F.linear(h, w, None))
+            else:
+                for w, b in zip(self.weight, self.bias):
+                    h = self.activation(F.linear(h, w, b))
+            return h
 
     def extra_repr(self) -> str:
         if self.activation is None:
             return 'in_features={}, out_features={}, bias={}'.format(self.in_features, self.out_features, self.bias is not None)
         else:
             return 'in_features={}, out_features={}, bias={}, activation={}'.format(self.in_features, self.out_features, self.bias is not None, self.activation)
```

## Comparing `torchfunction-0.0.8.dist-info/METADATA` & `torchfunction-0.0.9.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchfunction
-Version: 0.0.8
+Version: 0.0.9
 Summary: This package is based on pytorch and try to provide a more user-friendly interface for pytorch. 
 Home-page: https://github.com/Bertie97/pyctlib/tree/main/torchplus
 Author: Yiteng Zhang
 Author-email: zytfdu@icloud.com
 License: MIT Licence
 Keywords: pip,pyctlib,pytorch
 Platform: any
```

## Comparing `torchfunction-0.0.8.dist-info/RECORD` & `torchfunction-0.0.9.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 torchfunction/__init__.py,sha256=00k0VmDJ4bh2hx9-7CG42Gzt9O5uIKiAaqe9J8NeFv8,17
 torchfunction/createtensor.py,sha256=QVlcOWsxJKXvGtdMyHxIqleNAAvT7390p_g7a-5q7x8,516
 torchfunction/functional.py,sha256=LTVHc69cHDkLLtVJNpEOwBkVuv_IeeJ4occakq_VzMI,656
 torchfunction/inspect.py,sha256=2-SrrNAR_gYG8xs3Uv9G4GsiiE_MqF-wEQP4i6BVETM,903
 torchfunction/lossfunc.py,sha256=T0kdgX_Fi5_NwvS8Jv5V23N8Lr7YcGEaQGxRfTZehjY,1649
 torchfunction/nn/__init__.py,sha256=5RlQ4iRCXMFStVngkGIGKnVn1SWLjpSQlu-aQiv2rCQ,27
-torchfunction/nn/linear.py,sha256=-jJRosRpiVcuuiDa7ilRPzsgMKZVcrqMIipWVAeYW1s,1811
-torchfunction-0.0.8.dist-info/METADATA,sha256=JCLCue_TXMdrl1F_ENmH5mVukDUGVHCs1cUd4upfKK8,3611
-torchfunction-0.0.8.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-torchfunction-0.0.8.dist-info/top_level.txt,sha256=S1oGrUz-aOKGsUhmfdOKpVoU6ZnohbHuQpCnjasyZVg,14
-torchfunction-0.0.8.dist-info/RECORD,,
+torchfunction/nn/linear.py,sha256=newa7C7UVUCglVKPJQAeHslPRXOixSMFVaXI4YhwZHM,3100
+torchfunction-0.0.9.dist-info/METADATA,sha256=CrbJ9O_aNAnzWCrwxnZXbaEVccz9DEiXpwd_2wJkD8E,3611
+torchfunction-0.0.9.dist-info/WHEEL,sha256=OqRkF0eY5GHssMorFjlbTIq072vpHpF60fIQA6lS9xA,92
+torchfunction-0.0.9.dist-info/top_level.txt,sha256=S1oGrUz-aOKGsUhmfdOKpVoU6ZnohbHuQpCnjasyZVg,14
+torchfunction-0.0.9.dist-info/RECORD,,
```

