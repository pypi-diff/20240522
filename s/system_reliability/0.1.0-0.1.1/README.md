# Comparing `tmp/system_reliability-0.1.0.tar.gz` & `tmp/system_reliability-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "system_reliability-0.1.0.tar", max compression
+gzip compressed data, was "system_reliability-0.1.1.tar", max compression
```

## Comparing `system_reliability-0.1.0.tar` & `system_reliability-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.1.0/README.md
--rw-r--r--   0        0        0      273 2024-05-20 15:18:41.436859 system_reliability-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2929 2024-05-20 15:11:49.770508 system_reliability-0.1.0/system_reliability/components/block.py
--rw-r--r--   0        0        0      251 2024-05-18 15:49:00.741340 system_reliability-0.1.0/system_reliability/components/component.py
--rw-r--r--   0        0        0      932 2024-05-20 15:10:25.104953 system_reliability-0.1.0/system_reliability/components/element.py
--rw-r--r--   0        0        0      528 2024-05-20 15:09:55.634029 system_reliability-0.1.0/system_reliability/date.py
--rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.1.0/system_reliability/enums.py
--rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.1.0/system_reliability/exceptions.py
--rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-05-20 15:16:37.753854 system_reliability-0.1.1/README.md
+-rw-r--r--   0        0        0      273 2024-05-21 08:00:51.369407 system_reliability-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     2926 2024-05-21 08:00:40.893280 system_reliability-0.1.1/system_reliability/components/block.py
+-rw-r--r--   0        0        0      251 2024-05-18 15:49:00.741340 system_reliability-0.1.1/system_reliability/components/component.py
+-rw-r--r--   0        0        0      932 2024-05-20 15:10:25.104953 system_reliability-0.1.1/system_reliability/components/element.py
+-rw-r--r--   0        0        0      528 2024-05-20 15:09:55.634029 system_reliability-0.1.1/system_reliability/date.py
+-rw-r--r--   0        0        0      101 2024-05-18 15:45:03.716083 system_reliability-0.1.1/system_reliability/enums.py
+-rw-r--r--   0        0        0       95 2024-05-18 15:44:52.624116 system_reliability-0.1.1/system_reliability/exceptions.py
+-rw-r--r--   0        0        0      292 1970-01-01 00:00:00.000000 system_reliability-0.1.1/PKG-INFO
```

### Comparing `system_reliability-0.1.0/system_reliability/components/block.py` & `system_reliability-0.1.1/system_reliability/components/block.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,12 +72,12 @@
             connection=self.connection.value,
             probability=self.probability_simulated,
             components=[component.to_dict() for component in self.components],
         )
 
     
     def calculate(self):
-        simulated = self.simulated_probability(num_trials=10000)
+        simulated = self.simulated_probability(num_trials=50)
         
         return CulculateResult(
             simulated_results=simulated
         )
```

### Comparing `system_reliability-0.1.0/system_reliability/components/element.py` & `system_reliability-0.1.1/system_reliability/components/element.py`

 * *Files identical despite different names*

### Comparing `system_reliability-0.1.0/system_reliability/date.py` & `system_reliability-0.1.1/system_reliability/date.py`

 * *Files identical despite different names*

