# Comparing `tmp/poseidon_rna-0.4.tar.gz` & `tmp/poseidon_rna-0.5.tar.gz`

## Comparing `poseidon_rna-0.4.tar` & `poseidon_rna-0.5.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.4/src/poseidonrna/__init__.py
--rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 poseidon_rna-0.4/src/poseidonrna/poseidonrna.py
--rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average.ct
--rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average.db
--rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/full__average__varna-color.txt
--rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/Structures/a580__full.png
--rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.4/test/Structures/a580__full.svg
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.4/README.md
--rw-r--r--   0        0        0      862 2020-02-02 00:00:00.000000 poseidon_rna-0.4/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 poseidon_rna-0.4/PKG-INFO
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 poseidon_rna-0.5/src/poseidonrna/__init__.py
+-rw-r--r--   0        0        0     6398 2020-02-02 00:00:00.000000 poseidon_rna-0.5/src/poseidonrna/poseidonrna.py
+-rw-r--r--   0        0        0    76580 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average.ct
+-rw-r--r--   0        0        0     4291 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average.db
+-rw-r--r--   0        0        0     6584 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/full__average__varna-color.txt
+-rw-r--r--   0        0        0   158756 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/Structures/a580__full.png
+-rw-r--r--   0        0        0   227302 2020-02-02 00:00:00.000000 poseidon_rna-0.5/test/Structures/a580__full.svg
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 poseidon_rna-0.5/README.md
+-rw-r--r--   0        0        0      883 2020-02-02 00:00:00.000000 poseidon_rna-0.5/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 poseidon_rna-0.5/PKG-INFO
```

### Comparing `poseidon_rna-0.4/src/poseidonrna/poseidonrna.py` & `poseidon_rna-0.5/src/poseidonrna/poseidonrna.py`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/test/full__average.ct` & `poseidon_rna-0.5/test/full__average.ct`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/test/full__average.db` & `poseidon_rna-0.5/test/full__average.db`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/test/full__average__varna-color.txt` & `poseidon_rna-0.5/test/full__average__varna-color.txt`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/test/Structures/a580__full.png` & `poseidon_rna-0.5/test/Structures/a580__full.png`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/test/Structures/a580__full.svg` & `poseidon_rna-0.5/test/Structures/a580__full.svg`

 * *Files identical despite different names*

### Comparing `poseidon_rna-0.4/pyproject.toml` & `poseidon_rna-0.5/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,14 +16,15 @@
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "networkx>=3.3",
     "matplotlib>=3.8.4",
     "seaborn>=0.13.2",
     "numpy>=1.26.4",
+    "scipy>=1.13.0",
 ]
 dynamic = ["version"]
 
 [tool.hatch.build.targets.sdist]
 exclude = [
   "/.test",
 ]
```

### Comparing `poseidon_rna-0.4/PKG-INFO` & `poseidon_rna-0.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.3
 Name: poseidon-rna
-Version: 0.4
+Version: 0.5
 Summary: Plotting RNA using Kamada-Kawai Graph Plotting Algorithm
 Project-URL: Homepage, https://github.com/rouskinlab/poseidon-rna
 Project-URL: Bug Tracker, https://github.com/rouskinlab/poseidon-rna/issues
 Author: Adam Sychla
 License: GPL-3.0-only
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
 Requires-Dist: matplotlib>=3.8.4
 Requires-Dist: networkx>=3.3
 Requires-Dist: numpy>=1.26.4
+Requires-Dist: scipy>=1.13.0
 Requires-Dist: seaborn>=0.13.2
 Description-Content-Type: text/markdown
 
 Functions
 
 	poseidonrna.graph(filename,**kwargs)
```

