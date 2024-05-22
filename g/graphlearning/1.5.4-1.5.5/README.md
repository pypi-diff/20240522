# Comparing `tmp/graphlearning-1.5.4.tar.gz` & `tmp/graphlearning-1.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlearning-1.5.4.tar", last modified: Wed May 22 01:43:23 2024, max compression
+gzip compressed data, was "graphlearning-1.5.5.tar", last modified: Wed May 22 13:10:14 2024, max compression
```

## Comparing `graphlearning-1.5.4.tar` & `graphlearning-1.5.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.698391 graphlearning-1.5.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 01:43:06.000000 graphlearning-1.5.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 01:43:06.000000 graphlearning-1.5.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 01:43:23.698391 graphlearning-1.5.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-22 01:43:06.000000 graphlearning-1.5.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.694391 graphlearning-1.5.4/c_code/
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/cextensions.c
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/hjsolvers.c
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/hjsolvers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/lp_iterate.c
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/lp_iterate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_simple_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mbo_convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mbo_speedy_volume_preserving.c
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/memory_allocation.c
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/memory_allocation.h
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mnist_benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mnist_benchmark.h
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/vector_operations.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.694391 graphlearning-1.5.4/graphlearning/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/trainsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/weightmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.698391 graphlearning-1.5.4/graphlearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-22 01:43:07.000000 graphlearning-1.5.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:43:23.698391 graphlearning-1.5.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-22 01:43:07.000000 graphlearning-1.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:10:14.240488 graphlearning-1.5.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 13:09:58.000000 graphlearning-1.5.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 13:09:58.000000 graphlearning-1.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 13:10:14.240488 graphlearning-1.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-22 13:09:58.000000 graphlearning-1.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:10:14.236488 graphlearning-1.5.5/c_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/cextensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/hjsolvers.c
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/hjsolvers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/lp_iterate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/lp_iterate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/maj_dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/maj_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/maj_simple_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/mbo_convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/mbo_speedy_volume_preserving.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/memory_allocation.c
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/memory_allocation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/mnist_benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/mnist_benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-22 13:09:58.000000 graphlearning-1.5.5/c_code/vector_operations.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:10:14.236488 graphlearning-1.5.5/graphlearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/trainsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23252 2024-05-22 13:09:58.000000 graphlearning-1.5.5/graphlearning/weightmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 13:10:14.240488 graphlearning-1.5.5/graphlearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 13:10:14.000000 graphlearning-1.5.5/graphlearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-22 13:10:14.000000 graphlearning-1.5.5/graphlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 13:10:14.000000 graphlearning-1.5.5/graphlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 13:10:14.000000 graphlearning-1.5.5/graphlearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 13:10:14.000000 graphlearning-1.5.5/graphlearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-22 13:09:59.000000 graphlearning-1.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 13:10:14.240488 graphlearning-1.5.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-22 13:09:59.000000 graphlearning-1.5.5/setup.py
```

### Comparing `graphlearning-1.5.4/LICENSE` & `graphlearning-1.5.5/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/PKG-INFO` & `graphlearning-1.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.4/README.md` & `graphlearning-1.5.5/README.md`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/cextensions.c` & `graphlearning-1.5.5/c_code/cextensions.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/hjsolvers.c` & `graphlearning-1.5.5/c_code/hjsolvers.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/hjsolvers.h` & `graphlearning-1.5.5/c_code/hjsolvers.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/lp_iterate.c` & `graphlearning-1.5.5/c_code/lp_iterate.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/lp_iterate.h` & `graphlearning-1.5.5/c_code/lp_iterate.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/maj_dijkstra.h` & `graphlearning-1.5.5/c_code/maj_dijkstra.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/maj_implicit_heap.h` & `graphlearning-1.5.5/c_code/maj_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/maj_simple_implicit_heap.h` & `graphlearning-1.5.5/c_code/maj_simple_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/mbo_convolution.h` & `graphlearning-1.5.5/c_code/mbo_convolution.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/mbo_speedy_volume_preserving.c` & `graphlearning-1.5.5/c_code/mbo_speedy_volume_preserving.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/memory_allocation.c` & `graphlearning-1.5.5/c_code/memory_allocation.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/mnist_benchmark.c` & `graphlearning-1.5.5/c_code/mnist_benchmark.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/mnist_benchmark.h` & `graphlearning-1.5.5/c_code/mnist_benchmark.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/c_code/vector_operations.h` & `graphlearning-1.5.5/c_code/vector_operations.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/active_learning.py` & `graphlearning-1.5.5/graphlearning/active_learning.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/clustering.py` & `graphlearning-1.5.5/graphlearning/clustering.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/datasets.py` & `graphlearning-1.5.5/graphlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/graph.py` & `graphlearning-1.5.5/graphlearning/graph.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/ssl.py` & `graphlearning-1.5.5/graphlearning/ssl.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/trainsets.py` & `graphlearning-1.5.5/graphlearning/trainsets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/utils.py` & `graphlearning-1.5.5/graphlearning/utils.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/graphlearning/weightmatrix.py` & `graphlearning-1.5.5/graphlearning/weightmatrix.py`

 * *Files 3% similar despite different names*

```diff
@@ -364,18 +364,37 @@
         for i in range(n):
             u.add_item(i, X[i,:])
 
         u.build(10)  #10 trees
         
         knn_dist = []
         knn_ind = []
+        eps = 1e-15
         for i in range(n):
             A = u.get_nns_by_item(i, k, include_distances=True, search_k=-1)
             knn_ind.append(A[0])
-            knn_dist.append(A[1])
+            #knn_dist.append(A[1]) #These distances are floating point (32-bit) precision
+            if similarity == 'euclidean':
+                dist = np.linalg.norm(X[i,:] - X[A[0],:],axis=1)
+            elif similarity == 'angular':
+                vi = X[i,:]/np.maximum(np.linalg.norm(X[i,:]),eps)
+                vj = X[A[0],:]/np.maximum(np.linalg.norm(X[A[0],:],axis=1)[:,None],eps)
+                dist = np.linalg.norm(vi-vj,axis=1)
+            elif similarity == 'manhattan':
+                dist = A[1]
+            elif similarity == 'hamming':
+                dist = A[1]
+            elif similarity == 'dot':
+                dist = A[1]
+            else:
+                dist = A[1]
+
+            print(np.max(np.absolute(dist - np.array(A[1]))))
+            knn_dist.append(dist)
+
 
         knn_ind = np.array(knn_ind)
         knn_dist = np.array(knn_dist)
 
     else:
         sys.exit('Invalid choice of knnsearch method ' + method)
```

### Comparing `graphlearning-1.5.4/graphlearning.egg-info/PKG-INFO` & `graphlearning-1.5.5/graphlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.4
+Version: 1.5.5
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.4/graphlearning.egg-info/SOURCES.txt` & `graphlearning-1.5.5/graphlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.4/pyproject.toml` & `graphlearning-1.5.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools]
 packages = ['graphlearning']
 
 
 [project]
 name = "graphlearning"
-version = "1.5.4"
+version = "1.5.5"
 authors = [
   { name="Jeff Calder", email="jwcalder@umn.edu" },
 ]
 description = "Python package for graph-based clustering and semi-supervised learning"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.6"
```

### Comparing `graphlearning-1.5.4/setup.py` & `graphlearning-1.5.5/setup.py`

 * *Files identical despite different names*

