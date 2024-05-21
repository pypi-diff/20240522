# Comparing `tmp/multidim_indexing-0.9.2.tar.gz` & `tmp/multidim_indexing-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidim_indexing-0.9.2.tar", last modified: Tue May 21 01:12:50 2024, max compression
+gzip compressed data, was "multidim_indexing-0.9.3.tar", last modified: Tue May 21 02:35:05 2024, max compression
```

## Comparing `multidim_indexing-0.9.2.tar` & `multidim_indexing-0.9.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1056 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/LICENSE.txt
--rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/PKG-INFO
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6744 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/README.md
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4172 2024-05-17 02:36:21.000000 multidim_indexing-0.9.2/pyproject.toml
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-21 01:12:50.772292 multidim_indexing-0.9.2/setup.cfg
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/multidim_indexing/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        0 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/src/multidim_indexing/__init__.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1547 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/src/multidim_indexing/numpy_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2851 2024-05-17 02:30:54.000000 multidim_indexing-0.9.2/src/multidim_indexing/torch_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    11208 2024-05-17 02:35:21.000000 multidim_indexing-0.9.2/src/multidim_indexing/view.py
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/
--rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      472 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       64 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       18 2024-05-21 01:12:50.000000 multidim_indexing-0.9.2/src/multidim_indexing.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 01:12:50.768292 multidim_indexing-0.9.2/tests/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6859 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/tests/test_numpy_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      893 2024-05-17 01:24:04.000000 multidim_indexing-0.9.2/tests/test_performance.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9498 2024-05-01 20:02:46.000000 multidim_indexing-0.9.2/tests/test_torch_view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 02:35:05.616328 multidim_indexing-0.9.3/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1056 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/LICENSE.txt
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 02:35:05.616328 multidim_indexing-0.9.3/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6744 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/README.md
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4172 2024-05-21 02:34:47.000000 multidim_indexing-0.9.3/pyproject.toml
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-21 02:35:05.616328 multidim_indexing-0.9.3/setup.cfg
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 02:35:05.612328 multidim_indexing-0.9.3/src/
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 02:35:05.612328 multidim_indexing-0.9.3/src/multidim_indexing/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        0 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/src/multidim_indexing/__init__.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1547 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/src/multidim_indexing/numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2851 2024-05-17 02:30:54.000000 multidim_indexing-0.9.3/src/multidim_indexing/torch_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    11233 2024-05-21 01:49:15.000000 multidim_indexing-0.9.3/src/multidim_indexing/view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 02:35:05.616328 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 02:35:05.000000 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      472 2024-05-21 02:35:05.000000 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-21 02:35:05.000000 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       64 2024-05-21 02:35:05.000000 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       18 2024-05-21 02:35:05.000000 multidim_indexing-0.9.3/src/multidim_indexing.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 02:35:05.612328 multidim_indexing-0.9.3/tests/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6859 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/tests/test_numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      893 2024-05-17 01:24:04.000000 multidim_indexing-0.9.3/tests/test_performance.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9498 2024-05-01 20:02:46.000000 multidim_indexing-0.9.3/tests/test_torch_view.py
```

### Comparing `multidim_indexing-0.9.2/LICENSE.txt` & `multidim_indexing-0.9.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/PKG-INFO` & `multidim_indexing-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidim_indexing
-Version: 0.9.2
+Version: 0.9.3
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-0.9.2/README.md` & `multidim_indexing-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/pyproject.toml` & `multidim_indexing-0.9.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multidim_indexing"
-version = "0.9.2"
+version = "0.9.3"
 description = "Multidimensional batch indexing of pytorch tensors and numpy arrays"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `multidim_indexing-0.9.2/src/multidim_indexing/numpy_view.py` & `multidim_indexing-0.9.3/src/multidim_indexing/numpy_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/src/multidim_indexing/torch_view.py` & `multidim_indexing-0.9.3/src/multidim_indexing/torch_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/src/multidim_indexing/view.py` & `multidim_indexing-0.9.3/src/multidim_indexing/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,17 @@
     def __init__(self, f):
         self.f = f
 
     def __get__(self, obj, owner):
         return self.f(owner)
 
 
+eps = 1e-8
+
+
 class MultidimView(abc.ABC):
     def __init__(self, source, value_ranges=None, invalid_value=-1, check_safety=True, method='nearest',
                  coord_dtype=None):
         """
         View into a tensor or numpy array that is convenient to index using a batch of indices.
         Intended for use on a cache of a function that needs to be indexed into with coordinates
         rather than integer indices.
@@ -33,16 +36,16 @@
         self.dim = len(source.shape)
         self.invalid_value = invalid_value
         self.check_safety = check_safety
         self.method = method
         self.coordinate_dtype = coord_dtype or self.default_coordinate_dtype
 
         if value_ranges is not None:
-            self._min = self.arr([min(range) for range in value_ranges])
-            self._max = self.arr([max(range) for range in value_ranges])
+            self._min = self.arr([min(range) for range in value_ranges]) - eps
+            self._max = self.arr([max(range) for range in value_ranges]) + eps
             self._is_value_range = True
             # want an inclusive range on the min and max, so indexing with max should be valid
             shape = self.arr(self.shape)
             self._resolution = (self._max - self._min) / (shape - 1)
             # if some dim of shape is 1, then resolution for it is undefined
             invalid_resolution = self.lib.isnan(self._resolution)
             valid_resolution_val = self._resolution[~invalid_resolution]
```

### Comparing `multidim_indexing-0.9.2/src/multidim_indexing.egg-info/PKG-INFO` & `multidim_indexing-0.9.3/src/multidim_indexing.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidim_indexing
-Version: 0.9.2
+Version: 0.9.3
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-0.9.2/tests/test_numpy_view.py` & `multidim_indexing-0.9.3/tests/test_numpy_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/tests/test_performance.py` & `multidim_indexing-0.9.3/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-0.9.2/tests/test_torch_view.py` & `multidim_indexing-0.9.3/tests/test_torch_view.py`

 * *Files identical despite different names*

