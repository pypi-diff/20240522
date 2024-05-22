# Comparing `tmp/system_reliability-0.2.0.tar.gz` & `tmp/system_reliability-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_reliability-0.2.0.tar", max compression
+gzip compressed data, was "system_reliability-0.2.1.tar", max compression
```

## Comparing `system_reliability-0.2.0.tar` & `system_reliability-0.2.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.2.0/README.md
--rw-r--r--   0        0        0      273 2024-05-22 05:18:29.948936 system_reliability-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3670 2024-05-22 05:17:34.172666 system_reliability-0.2.0/system_reliability/components/block.py
--rw-r--r--   0        0        0      410 2024-05-22 04:59:53.429535 system_reliability-0.2.0/system_reliability/components/component.py
--rw-r--r--   0        0        0     1187 2024-05-22 05:04:26.214077 system_reliability-0.2.0/system_reliability/components/element.py
--rw-r--r--   0        0        0      556 2024-05-22 05:16:50.736446 system_reliability-0.2.0/system_reliability/date.py
--rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.2.0/system_reliability/enums.py
--rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.2.0/system_reliability/exceptions.py
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.2.1/README.md
+-rw-r--r--   0        0        0      273 2024-05-22 05:27:37.583075 system_reliability-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3763 2024-05-22 05:27:22.575025 system_reliability-0.2.1/system_reliability/components/block.py
+-rw-r--r--   0        0        0      410 2024-05-22 04:59:53.429535 system_reliability-0.2.1/system_reliability/components/component.py
+-rw-r--r--   0        0        0     1187 2024-05-22 05:04:26.214077 system_reliability-0.2.1/system_reliability/components/element.py
+-rw-r--r--   0        0        0      556 2024-05-22 05:16:50.736446 system_reliability-0.2.1/system_reliability/date.py
+-rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.2.1/system_reliability/enums.py
+-rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.2.1/system_reliability/exceptions.py
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.2.1/PKG-INFO
```

### Comparing `system_reliability-0.2.0/system_reliability/components/block.py` & `system_reliability-0.2.1/system_reliability/components/block.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,15 +71,18 @@
             components=[component.to_dict() for component in self.components],
         )
 
     def to_dict_analytical(self, mode: MethodConnection):
         # print(self.probability_analytical)
         # print(Block.get_formula_analytical(self.probability_analytical, mode))
 
-        return Block.get_formula_analytical(' * '.join([component.to_dict_analytical(self.connection) for component in self.components]), mode)
+        
+        formula = [component.to_dict_analytical(self.connection) for component in self.components]
+        
+        return Block.get_formula_analytical(' * '.join(formula), mode if len(formula) > 1 else MethodConnection.Serial)
         
     def get_formula_analytical(probability: int, mode: MethodConnection):
         match mode:
             case MethodConnection.Parallel:
                 return f'(1 - {probability})'
             case MethodConnection.Serial:
                 return f'{probability}'
```

### Comparing `system_reliability-0.2.0/system_reliability/components/element.py` & `system_reliability-0.2.1/system_reliability/components/element.py`

 * *Files identical despite different names*

### Comparing `system_reliability-0.2.0/system_reliability/date.py` & `system_reliability-0.2.1/system_reliability/date.py`

 * *Files identical despite different names*

