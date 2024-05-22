# Comparing `tmp/poseidon_rna-0.6.tar.gz` & `tmp/poseidon_rna-0.7.tar.gz`

## Comparing `poseidon_rna-0.6.tar` & `poseidon_rna-0.7.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.6/src/poseidonrna/__init__.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 poseidon_rna-0.6/src/poseidonrna/poseidonrna.py
--rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average.ct
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average.db
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/full__average__varna-color.txt
--rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/Structures/a580__full.png
--rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.6/test/Structures/a580__full.svg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.6/README.md
--rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 poseidon_rna-0.6/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 poseidon_rna-0.6/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.7/src/poseidonrna/__init__.py
+-rw-r--r--   0        0        0     6545 2020-02-02 00:00:00.000000 poseidon_rna-0.7/src/poseidonrna/poseidonrna.py
+-rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.7/test/full__average.ct
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.7/test/full__average.db
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.7/test/full__average__varna-color.txt
+-rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.7/test/Structures/a580__full.png
+-rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.7/test/Structures/a580__full.svg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.7/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 poseidon_rna-0.7/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 poseidon_rna-0.7/PKG-INFO
```

### Comparing `poseidon_rna-0.6/src/poseidonrna/poseidonrna.py` & `poseidon_rna-0.7/src/poseidonrna/poseidonrna.py`

 * *Files 1% similar despite different names*

```diff
@@ -240,16 +240,19 @@
     
     if filename[-2:]=='db':
         
         if num_strucs == 'all':
             num_strucs = len(pairs)
             
         for x in range(num_strucs):
-            G = create_db_graph(seqs[x],pairs[x],newcolors)
-            graphs.append(G)
+            try:
+                G = create_db_graph(seqs[x],pairs[x],newcolors)
+                graphs.append(G)
+            except:
+                break
 
 
     elif filename[-2:] == 'ct':
 
         if num_strucs == 'all':
             num_strucs = len(seqs)
```

### Comparing `poseidon_rna-0.6/test/full__average.ct` & `poseidon_rna-0.7/test/full__average.ct`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/test/full__average.db` & `poseidon_rna-0.7/test/full__average.db`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/test/full__average__varna-color.txt` & `poseidon_rna-0.7/test/full__average__varna-color.txt`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/test/Structures/a580__full.png` & `poseidon_rna-0.7/test/Structures/a580__full.png`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/test/Structures/a580__full.svg` & `poseidon_rna-0.7/test/Structures/a580__full.svg`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/pyproject.toml` & `poseidon_rna-0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.6/PKG-INFO` & `poseidon_rna-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: poseidon-rna
-Version: 0.6
+Version: 0.7
 Summary: Plotting RNA using Kamada-Kawai Graph Plotting Algorithm
 Project-URL: Homepage, https://github.com/rouskinlab/poseidon-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/poseidon-rna/issues
 Author: Adam Sychla
 License: GPL-3.0-only
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

