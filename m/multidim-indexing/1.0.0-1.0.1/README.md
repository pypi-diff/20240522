# Comparing `tmp/multidim_indexing-1.0.0.tar.gz` & `tmp/multidim_indexing-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multidim_indexing-1.0.0.tar", last modified: Tue May 21 23:55:12 2024, max compression
+gzip compressed data, was "multidim_indexing-1.0.1.tar", last modified: Wed May 22 00:56:49 2024, max compression
```

## Comparing `multidim_indexing-1.0.0.tar` & `multidim_indexing-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1056 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/LICENSE.txt
--rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/PKG-INFO
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6744 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/README.md
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4172 2024-05-21 23:54:40.000000 multidim_indexing-1.0.0/pyproject.toml
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/setup.cfg
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/src/
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/src/multidim_indexing/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        0 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/src/multidim_indexing/__init__.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1547 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/src/multidim_indexing/numpy_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2851 2024-05-17 02:30:54.000000 multidim_indexing-1.0.0/src/multidim_indexing/torch_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    11699 2024-05-21 23:53:08.000000 multidim_indexing-1.0.0/src/multidim_indexing/view.py
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/
--rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-21 23:55:12.000000 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/PKG-INFO
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      472 2024-05-21 23:55:12.000000 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/SOURCES.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-21 23:55:12.000000 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/dependency_links.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       64 2024-05-21 23:55:12.000000 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/requires.txt
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       18 2024-05-21 23:55:12.000000 multidim_indexing-1.0.0/src/multidim_indexing.egg-info/top_level.txt
-drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-21 23:55:12.123419 multidim_indexing-1.0.0/tests/
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6859 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/tests/test_numpy_view.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2389 2024-05-21 23:22:42.000000 multidim_indexing-1.0.0/tests/test_performance.py
--rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9498 2024-05-01 20:02:46.000000 multidim_indexing-1.0.0/tests/test_torch_view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-22 00:56:49.905022 multidim_indexing-1.0.1/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1056 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/LICENSE.txt
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-22 00:56:49.905022 multidim_indexing-1.0.1/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6744 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/README.md
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     4172 2024-05-22 00:56:18.000000 multidim_indexing-1.0.1/pyproject.toml
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       38 2024-05-22 00:56:49.905022 multidim_indexing-1.0.1/setup.cfg
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-22 00:56:49.901023 multidim_indexing-1.0.1/src/
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-22 00:56:49.901023 multidim_indexing-1.0.1/src/multidim_indexing/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        0 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/src/multidim_indexing/__init__.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     1547 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/src/multidim_indexing/numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2851 2024-05-17 02:30:54.000000 multidim_indexing-1.0.1/src/multidim_indexing/torch_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)    11705 2024-05-22 00:54:57.000000 multidim_indexing-1.0.1/src/multidim_indexing/view.py
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-22 00:56:49.901023 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/
+-rw-r--r--   0 zhsh      (1002) zhsh      (1002)     9051 2024-05-22 00:56:49.000000 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/PKG-INFO
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)      472 2024-05-22 00:56:49.000000 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)        1 2024-05-22 00:56:49.000000 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       64 2024-05-22 00:56:49.000000 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/requires.txt
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)       18 2024-05-22 00:56:49.000000 multidim_indexing-1.0.1/src/multidim_indexing.egg-info/top_level.txt
+drwxrwxr-x   0 zhsh      (1002) zhsh      (1002)        0 2024-05-22 00:56:49.901023 multidim_indexing-1.0.1/tests/
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     6859 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/tests/test_numpy_view.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     2389 2024-05-21 23:22:42.000000 multidim_indexing-1.0.1/tests/test_performance.py
+-rw-rw-r--   0 zhsh      (1002) zhsh      (1002)     9498 2024-05-01 20:02:46.000000 multidim_indexing-1.0.1/tests/test_torch_view.py
```

### Comparing `multidim_indexing-1.0.0/LICENSE.txt` & `multidim_indexing-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/PKG-INFO` & `multidim_indexing-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidim_indexing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-1.0.0/README.md` & `multidim_indexing-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/pyproject.toml` & `multidim_indexing-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "multidim_indexing"
-version = "1.0.0"
+version = "1.0.1"
 description = "Multidimensional batch indexing of pytorch tensors and numpy arrays"
 readme = "README.md" # Optional
 
 # Specify which Python versions you support. In contrast to the
 # 'Programming Language' classifiers above, 'pip install' will check this
 # and refuse to install the project if the version does not match. See
 # https://packaging.python.org/guides/distributing-packages-using-setuptools/#python-requires
```

### Comparing `multidim_indexing-1.0.0/src/multidim_indexing/numpy_view.py` & `multidim_indexing-1.0.1/src/multidim_indexing/numpy_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/src/multidim_indexing/torch_view.py` & `multidim_indexing-1.0.1/src/multidim_indexing/torch_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/src/multidim_indexing/view.py` & `multidim_indexing-1.0.1/src/multidim_indexing/view.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,18 +245,17 @@
 
             # Calculate the indices for the vertices of the 3D cube surrounding the interpolation point
             offsets = self.arr(tuple(itertools.product([0, 1], repeat=self.dim)), dtype=self.int)
             # All combinations of idx_left with [0, 1] offsets in 3 dimensions
             corner_indices = idx_left[:, None, :] + offsets
 
             # Compute ravel indices for all corners in one step
-            flat_corner_indices = self.ravel_multi_index(corner_indices.view(-1, 3), self.shape)
+            flat_corner_indices = self.ravel_multi_index(corner_indices.view(-1, self.dim), self.shape)
             flat_corner_indices = flat_corner_indices.view(-1,
                                                            2 ** self.dim)  # Reshape back to the number of points and corners
-
             # Compute distances for interpolation only once
             dist_left = idx_raw - idx_left
             dist_right = 1 - dist_left
             # Calculate the interpolation weights for all corners
             weights = dist_left[:, None, :] ** offsets * dist_right[:, None, :] ** (1 - offsets)
             weights = weights.prod(dim=2)  # Weights for each corner
```

### Comparing `multidim_indexing-1.0.0/src/multidim_indexing.egg-info/PKG-INFO` & `multidim_indexing-1.0.1/src/multidim_indexing.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multidim_indexing
-Version: 1.0.0
+Version: 1.0.1
 Summary: Multidimensional batch indexing of pytorch tensors and numpy arrays
 Author-email: Sheng Zhong <zhsh@umich.edu>
 Maintainer-email: Sheng Zhong <zhsh@umich.edu>
 License: Copyright (c) 2023 Sheng Zhong
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
```

### Comparing `multidim_indexing-1.0.0/tests/test_numpy_view.py` & `multidim_indexing-1.0.1/tests/test_numpy_view.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/tests/test_performance.py` & `multidim_indexing-1.0.1/tests/test_performance.py`

 * *Files identical despite different names*

### Comparing `multidim_indexing-1.0.0/tests/test_torch_view.py` & `multidim_indexing-1.0.1/tests/test_torch_view.py`

 * *Files identical despite different names*

