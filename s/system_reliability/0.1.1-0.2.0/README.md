# Comparing `tmp/system_reliability-0.1.1.tar.gz` & `tmp/system_reliability-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_reliability-0.1.1.tar", max compression
+gzip compressed data, was "system_reliability-0.2.0.tar", max compression
```

## Comparing `system_reliability-0.1.1.tar` & `system_reliability-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.1.1/README.md
--rw-r--r--   0        0        0      273 2024-05-21 08:00:51.369407 system_reliability-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2926 2024-05-21 08:00:40.893280 system_reliability-0.1.1/system_reliability/components/block.py
--rw-r--r--   0        0        0      251 2024-05-18 15:49:00.741340 system_reliability-0.1.1/system_reliability/components/component.py
--rw-r--r--   0        0        0      932 2024-05-20 15:10:25.104953 system_reliability-0.1.1/system_reliability/components/element.py
--rw-r--r--   0        0        0      528 2024-05-20 15:09:55.634029 system_reliability-0.1.1/system_reliability/date.py
--rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.1.1/system_reliability/enums.py
--rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.1.1/system_reliability/exceptions.py
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.2.0/README.md
+-rw-r--r--   0        0        0      273 2024-05-22 05:18:29.948936 system_reliability-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     3670 2024-05-22 05:17:34.172666 system_reliability-0.2.0/system_reliability/components/block.py
+-rw-r--r--   0        0        0      410 2024-05-22 04:59:53.429535 system_reliability-0.2.0/system_reliability/components/component.py
+-rw-r--r--   0        0        0     1187 2024-05-22 05:04:26.214077 system_reliability-0.2.0/system_reliability/components/element.py
+-rw-r--r--   0        0        0      556 2024-05-22 05:16:50.736446 system_reliability-0.2.0/system_reliability/date.py
+-rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.2.0/system_reliability/enums.py
+-rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.2.0/system_reliability/exceptions.py
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.2.0/PKG-INFO
```

### Comparing `system_reliability-0.1.1/system_reliability/components/block.py` & `system_reliability-0.2.0/system_reliability/components/block.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,19 +7,16 @@
 
 class Block(Component):
     
     def __init__(self, *components: Component, connection: MethodConnection):
         self.components = components
         self.connection = connection
         self.probability_analytical = self.calculate_probability_analytical()
-    
-    block_main = None
-    block_step: str = None  
-    simulated_step: int = None 
-    simulated_results = []
+        self.probability_simulated = None
+        self.simulated_results = []
        
     def calculate_probability_by_method_analytical(self, probability):
         match self.connection:
             case MethodConnection.Parallel:
                 return 1 - probability
             case MethodConnection.Serial:
                 return probability
@@ -70,14 +67,33 @@
         return BlockDict(
             type_component=self.__class__.__name__,
             connection=self.connection.value,
             probability=self.probability_simulated,
             components=[component.to_dict() for component in self.components],
         )
 
+    def to_dict_analytical(self, mode: MethodConnection):
+        # print(self.probability_analytical)
+        # print(Block.get_formula_analytical(self.probability_analytical, mode))
+
+        return Block.get_formula_analytical(' * '.join([component.to_dict_analytical(self.connection) for component in self.components]), mode)
+        
+    def get_formula_analytical(probability: int, mode: MethodConnection):
+        match mode:
+            case MethodConnection.Parallel:
+                return f'(1 - {probability})'
+            case MethodConnection.Serial:
+                return f'{probability}'
+        
+    
     
     def calculate(self):
         simulated = self.simulated_probability(num_trials=50)
         
+        
         return CulculateResult(
-            simulated_results=simulated
-        )
+            simulated_results=simulated,
+            analytical_results=self.to_dict_analytical(self.connection) + f' = {self.calculate_probability_analytical()}'
+            
+        )
+        
+
```

### Comparing `system_reliability-0.1.1/system_reliability/components/element.py` & `system_reliability-0.2.0/system_reliability/components/element.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,11 @@
 import random
+
+from system_reliability.components.block import Block
+from system_reliability.enums import MethodConnection
 from .component import Component
 from ..exceptions import ConstrainElementUp, ConstrainElementDown
 
 from ..date import ElementDict
 
 class Element(Component):
     
@@ -24,7 +27,10 @@
     def to_dict(self) -> ElementDict:
         return ElementDict(
             type_component=self.__class__.__name__,
             probability_analytical=self.probability_analytical,
             random_value=self.random_value,
             probability=self.random_value < self.probability_analytical
         )
+        
+    def to_dict_analytical(self, mode: MethodConnection):
+        return Block.get_formula_analytical(self.probability_analytical, mode)
```

### Comparing `system_reliability-0.1.1/system_reliability/date.py` & `system_reliability-0.2.0/system_reliability/date.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,8 +20,9 @@
     success_count: int
     num_trials: int
     probability: float
     details: List[ElementDict | BlockDict]
 
 @dataclass
 class CulculateResult:
-    simulated_results: SimulationResult
+    simulated_results: SimulationResult
+    analytical_results: str
```

