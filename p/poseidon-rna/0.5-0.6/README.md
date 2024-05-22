# Comparing `tmp/poseidon_rna-0.5.tar.gz` & `tmp/poseidon_rna-0.6.tar.gz`

## Comparing `poseidon_rna-0.5.tar` & `poseidon_rna-0.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.5/src/poseidonrna/__init__.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 poseidon_rna-0.5/src/poseidonrna/poseidonrna.py
--rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average.ct
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average.db
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average__varna-color.txt
--rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/Structures/a580__full.png
--rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/Structures/a580__full.svg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.5/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 poseidon_rna-0.5/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 poseidon_rna-0.5/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.6/src/poseidonrna/__init__.py
+-rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 poseidon_rna-0.6/src/poseidonrna/poseidonrna.py
+-rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average.ct
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average.db
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average__varna-color.txt
+-rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/Structures/a580__full.png
+-rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/Structures/a580__full.svg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.6/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 poseidon_rna-0.6/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 poseidon_rna-0.6/PKG-INFO
```

### Comparing `poseidon_rna-0.5/src/poseidonrna/poseidonrna.py` & `poseidon_rna-0.6/src/poseidonrna/poseidonrna.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import networkx as nx
 import os
 import matplotlib.pyplot as plt
 import seaborn as sns
 import numpy as np
+
 def read_db_structures(filename):
     #only reads first structure
     # Open the .db file
     with open(filename, 'r') as file:
         # Read the lines
         lines = file.readlines()
 
@@ -249,19 +250,24 @@
 
     elif filename[-2:] == 'ct':
 
         if num_strucs == 'all':
             num_strucs = len(seqs)
         
         for x in range(num_strucs):
-            G = create_ct_graph(seqs[x],'',newcolors)
-            graphs.append(G)
+
+            try:
+                G = create_ct_graph(seqs[x],'',newcolors)
+                graphs.append(G)
+
+            except:
+                break
 
     
     positions = []
-    for x in range(num_strucs):
+    for x in range(len(graphs)):
 
         pos = plotGraph(graphs[x],names[x],color,node_size,bases,view)
         
         positions.append(pos)
 
     return
```

### Comparing `poseidon_rna-0.5/test/full__average.ct` & `poseidon_rna-0.6/test/full__average.ct`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/test/full__average.db` & `poseidon_rna-0.6/test/full__average.db`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/test/full__average__varna-color.txt` & `poseidon_rna-0.6/test/full__average__varna-color.txt`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/test/Structures/a580__full.png` & `poseidon_rna-0.6/test/Structures/a580__full.png`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/test/Structures/a580__full.svg` & `poseidon_rna-0.6/test/Structures/a580__full.svg`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/pyproject.toml` & `poseidon_rna-0.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.5/PKG-INFO` & `poseidon_rna-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: poseidon-rna
-Version: 0.5
+Version: 0.6
 Summary: Plotting RNA using Kamada-Kawai Graph Plotting Algorithm
 Project-URL: Homepage, https://github.com/rouskinlab/poseidon-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/poseidon-rna/issues
 Author: Adam Sychla
 License: GPL-3.0-only
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

