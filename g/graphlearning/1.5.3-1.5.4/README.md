# Comparing `tmp/graphlearning-1.5.3.tar.gz` & `tmp/graphlearning-1.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphlearning-1.5.3.tar", last modified: Fri May  3 02:14:02 2024, max compression
+gzip compressed data, was "graphlearning-1.5.4.tar", last modified: Wed May 22 01:43:23 2024, max compression
```

## Comparing `graphlearning-1.5.3.tar` & `graphlearning-1.5.4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-03 02:13:47.000000 graphlearning-1.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-03 02:13:47.000000 graphlearning-1.5.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-03 02:14:02.119960 graphlearning-1.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-03 02:13:47.000000 graphlearning-1.5.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.115960 graphlearning-1.5.3/c_code/
--rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/cextensions.c
--rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/hjsolvers.c
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/hjsolvers.h
--rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/lp_iterate.c
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/lp_iterate.h
--rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_dijkstra.h
--rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/maj_simple_implicit_heap.h
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mbo_convolution.h
--rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mbo_speedy_volume_preserving.c
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/memory_allocation.c
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/memory_allocation.h
--rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mnist_benchmark.c
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/mnist_benchmark.h
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-03 02:13:47.000000 graphlearning-1.5.3/c_code/vector_operations.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/graphlearning/
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23417 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/active_learning.py
--rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/clustering.py
--rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/datasets.py
--rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)    77849 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/trainsets.py
--rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    22463 2024-05-03 02:13:47.000000 graphlearning-1.5.3/graphlearning/weightmatrix.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-03 02:14:02.119960 graphlearning-1.5.3/graphlearning.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-03 02:14:02.000000 graphlearning-1.5.3/graphlearning.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-03 02:13:48.000000 graphlearning-1.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-03 02:14:02.119960 graphlearning-1.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-03 02:13:48.000000 graphlearning-1.5.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.698391 graphlearning-1.5.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-22 01:43:06.000000 graphlearning-1.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-22 01:43:06.000000 graphlearning-1.5.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 01:43:23.698391 graphlearning-1.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3511 2024-05-22 01:43:06.000000 graphlearning-1.5.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.694391 graphlearning-1.5.4/c_code/
+-rw-r--r--   0 runner    (1001) docker     (127)    11644 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/cextensions.c
+-rw-r--r--   0 runner    (1001) docker     (127)    11735 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/hjsolvers.c
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/hjsolvers.h
+-rw-r--r--   0 runner    (1001) docker     (127)     6877 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/lp_iterate.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/lp_iterate.h
+-rw-r--r--   0 runner    (1001) docker     (127)     7003 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_dijkstra.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3765 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/maj_simple_implicit_heap.h
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mbo_convolution.h
+-rw-r--r--   0 runner    (1001) docker     (127)    37180 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mbo_speedy_volume_preserving.c
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/memory_allocation.c
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/memory_allocation.h
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mnist_benchmark.c
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/mnist_benchmark.h
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-05-22 01:43:06.000000 graphlearning-1.5.4/c_code/vector_operations.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.694391 graphlearning-1.5.4/graphlearning/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23418 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/active_learning.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16061 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9682 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50782 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78178 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/trainsets.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29768 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22468 2024-05-22 01:43:06.000000 graphlearning-1.5.4/graphlearning/weightmatrix.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 01:43:23.698391 graphlearning-1.5.4/graphlearning.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-22 01:43:23.000000 graphlearning-1.5.4/graphlearning.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-05-22 01:43:07.000000 graphlearning-1.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 01:43:23.698391 graphlearning-1.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2024-05-22 01:43:07.000000 graphlearning-1.5.4/setup.py
```

### Comparing `graphlearning-1.5.3/LICENSE` & `graphlearning-1.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/PKG-INFO` & `graphlearning-1.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.3/README.md` & `graphlearning-1.5.4/README.md`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/cextensions.c` & `graphlearning-1.5.4/c_code/cextensions.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/hjsolvers.c` & `graphlearning-1.5.4/c_code/hjsolvers.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/hjsolvers.h` & `graphlearning-1.5.4/c_code/hjsolvers.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/lp_iterate.c` & `graphlearning-1.5.4/c_code/lp_iterate.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/lp_iterate.h` & `graphlearning-1.5.4/c_code/lp_iterate.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/maj_dijkstra.h` & `graphlearning-1.5.4/c_code/maj_dijkstra.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/maj_implicit_heap.h` & `graphlearning-1.5.4/c_code/maj_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/maj_simple_implicit_heap.h` & `graphlearning-1.5.4/c_code/maj_simple_implicit_heap.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/mbo_convolution.h` & `graphlearning-1.5.4/c_code/mbo_convolution.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/mbo_speedy_volume_preserving.c` & `graphlearning-1.5.4/c_code/mbo_speedy_volume_preserving.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/memory_allocation.c` & `graphlearning-1.5.4/c_code/memory_allocation.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/mnist_benchmark.c` & `graphlearning-1.5.4/c_code/mnist_benchmark.c`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/mnist_benchmark.h` & `graphlearning-1.5.4/c_code/mnist_benchmark.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/c_code/vector_operations.h` & `graphlearning-1.5.4/c_code/vector_operations.h`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/active_learning.py` & `graphlearning-1.5.4/graphlearning/active_learning.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 ```
 
 Some clarification of terms:
 - ``acquisition function``: a function that quantifies "how useful" it would be to label a currently unlabeled node. Oftentimes, this is reflected in the "uncertainty" of the current classifier's output for each node. 
 - __NOTE:__ users can provide their own acquisition functions that inherit from the ``acquisition_function`` class, being sure to implement it so that __larger values__ of the acquisition function correspond to __more desirable__ nodes to be labeled.
 - ``policy``: the active learning policy determines which node(s) will be selected as query points, given the set of acquisition function values evaluated on the unlabeled nodes. 
 - The default value ``max`` indicates that query points will be the maximizers of the acquisition function on the unlabeled nodes. The policy ``prop`` selects the query points proportional to the ''softmax'' of the acquisition function values; namely, 
-\\[\mathbb{P}(X = x) \\propto e^{\\gamma \\mathcal{A}(x)}\\]
+\\[\\mathbb{P}(X = x) \\propto e^{\\gamma \\mathcal{A}(x)}\\]
 """
 
 import numpy as np
 from scipy.special import softmax
 from abc import ABCMeta, abstractmethod
 import matplotlib.pyplot as plt
```

### Comparing `graphlearning-1.5.3/graphlearning/clustering.py` & `graphlearning-1.5.4/graphlearning/clustering.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/datasets.py` & `graphlearning-1.5.4/graphlearning/datasets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/graph.py` & `graphlearning-1.5.4/graphlearning/graph.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/ssl.py` & `graphlearning-1.5.4/graphlearning/ssl.py`

 * *Files 0% similar despite different names*

```diff
@@ -453,15 +453,15 @@
             Training labels as integers \\(0,1,\\dots,k-1\\) for \\(k\\) classes.
         all_labels : numpy array, int (optional)
             True labels for all datapoints.
 
         Returns
         -------
         u : (n,k) numpy array, float
-            Probabilities computed by graph-based learning for each node and each class.
+            Per-class scores computed by graph-based learning for each node and each class. For some methods these are probabilities (i.e., for Laplace learning), while for others they can take on negative values (e.g., Poisson learning). The class label prediction is either the argmax or argmin over the rows of u (most methods are argmax, except distance-function based methods like nearest neighbor and peikonal).
         """
 
         if self.graph is None:
             sys.exit('SSL object has no graph. Use graph.set_graph() to provide a graph for SSL.')
 
         self.fitted = True
```

### Comparing `graphlearning-1.5.3/graphlearning/trainsets.py` & `graphlearning-1.5.4/graphlearning/trainsets.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/utils.py` & `graphlearning-1.5.4/graphlearning/utils.py`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/graphlearning/weightmatrix.py` & `graphlearning-1.5.4/graphlearning/weightmatrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -342,20 +342,20 @@
         if method == 'kdtree':
 
             Xtree = spatial.cKDTree(X)
             knn_dist, knn_ind = Xtree.query(X,k=k)
 
         else: #Brute force knn search
 
-            knn_ind = np.array((n,k),dtype=int)
-            knn_dist = np.array((n,k))
+            knn_ind = np.zeros((n,k),dtype=int)
+            knn_dist = np.zeros((n,k))
             for i in range(n):
                 dist  = np.linalg.norm(X - X[i,:],axis=1) 
                 knn_ind[i,:] = np.argsort(dist)[:k]
-                knn_dist[i,:] = dist[knn_ind]
+                knn_dist[i,:] = dist[knn_ind[i,:]]
 
     elif method == 'annoy':
 
         if not similarity in ['euclidean','angular','manhattan','hamming','dot']:
             sys.exit('Invalid choice of similarity ' + similarity)
 
         from annoy import AnnoyIndex
```

### Comparing `graphlearning-1.5.3/graphlearning.egg-info/PKG-INFO` & `graphlearning-1.5.4/graphlearning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphlearning
-Version: 1.5.3
+Version: 1.5.4
 Summary: Python package for graph-based clustering and semi-supervised learning
 Author-email: Jeff Calder <jwcalder@umn.edu>
 License: MIT
 Project-URL: Homepage, https://github.com/jwcalder/GraphLearning
 Project-URL: Bug Tracker, https://github.com/jwcalder/GraphLearning/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `graphlearning-1.5.3/graphlearning.egg-info/SOURCES.txt` & `graphlearning-1.5.4/graphlearning.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphlearning-1.5.3/pyproject.toml` & `graphlearning-1.5.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [tool.setuptools]
 packages = ['graphlearning']
 
 
 [project]
 name = "graphlearning"
-version = "1.5.3"
+version = "1.5.4"
 authors = [
   { name="Jeff Calder", email="jwcalder@umn.edu" },
 ]
 description = "Python package for graph-based clustering and semi-supervised learning"
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.6"
```

### Comparing `graphlearning-1.5.3/setup.py` & `graphlearning-1.5.4/setup.py`

 * *Files identical despite different names*

