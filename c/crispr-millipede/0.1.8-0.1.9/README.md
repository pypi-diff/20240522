# Comparing `tmp/crispr_millipede-0.1.8.tar.gz` & `tmp/crispr_millipede-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crispr_millipede-0.1.8.tar", max compression
+gzip compressed data, was "crispr_millipede-0.1.9.tar", max compression
```

## Comparing `crispr_millipede-0.1.8.tar` & `crispr_millipede-0.1.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      118 2023-12-18 11:55:32.094585 crispr_millipede-0.1.8/crispr_millipede/__init__.py
--rw-r--r--   0        0        0       38 2023-12-18 11:55:20.531424 crispr_millipede-0.1.8/crispr_millipede/encoding/__init__.py
--rw-r--r--   0        0        0    11308 2024-01-02 17:03:08.320850 crispr_millipede-0.1.8/crispr_millipede/encoding/CrisprMillipedeEncoding.py
--rw-r--r--   0        0        0       40 2023-12-18 11:55:25.108435 crispr_millipede-0.1.8/crispr_millipede/modelling/__init__.py
--rw-r--r--   0        0        0      283 2023-12-18 11:09:26.906267 crispr_millipede-0.1.8/crispr_millipede/modelling/CrisprMillipedeModelling.py
--rw-r--r--   0        0        0       43 2023-12-18 11:55:29.815853 crispr_millipede-0.1.8/crispr_millipede/visualization/__init__.py
--rw-r--r--   0        0        0        0 2023-12-18 11:26:57.377400 crispr_millipede-0.1.8/crispr_millipede/visualization/CrisprMillipedeVisualization.py
--rw-r--r--   0        0        0      521 2024-01-02 17:03:15.310134 crispr_millipede-0.1.8/pyproject.toml
--rw-r--r--   0        0        0        0 2023-10-24 13:31:13.358066 crispr_millipede-0.1.8/README.md
--rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 crispr_millipede-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0      118 2023-12-18 11:55:32.094585 crispr_millipede-0.1.9/crispr_millipede/__init__.py
+-rw-r--r--   0        0        0       38 2023-12-18 11:55:20.531424 crispr_millipede-0.1.9/crispr_millipede/encoding/__init__.py
+-rw-r--r--   0        0        0    11309 2024-01-02 17:04:20.838027 crispr_millipede-0.1.9/crispr_millipede/encoding/CrisprMillipedeEncoding.py
+-rw-r--r--   0        0        0       40 2023-12-18 11:55:25.108435 crispr_millipede-0.1.9/crispr_millipede/modelling/__init__.py
+-rw-r--r--   0        0        0      283 2023-12-18 11:09:26.906267 crispr_millipede-0.1.9/crispr_millipede/modelling/CrisprMillipedeModelling.py
+-rw-r--r--   0        0        0       43 2023-12-18 11:55:29.815853 crispr_millipede-0.1.9/crispr_millipede/visualization/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-18 11:26:57.377400 crispr_millipede-0.1.9/crispr_millipede/visualization/CrisprMillipedeVisualization.py
+-rw-r--r--   0        0        0      521 2024-01-02 17:04:29.018109 crispr_millipede-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-10-24 13:31:13.358066 crispr_millipede-0.1.9/README.md
+-rw-r--r--   0        0        0      780 1970-01-01 00:00:00.000000 crispr_millipede-0.1.9/PKG-INFO
```

### Comparing `crispr_millipede-0.1.8/crispr_millipede/encoding/CrisprMillipedeEncoding.py` & `crispr_millipede-0.1.9/crispr_millipede/encoding/CrisprMillipedeEncoding.py`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
     encodings_per_position_df.columns = list(original_seq)
     mismatch_mappings_per_position_df.columns = list(original_seq)
 
     mismatch_mappings_per_position_POS_list = np.arange(mismatch_mappings_per_position_df.shape[1]).repeat(mismatch_mappings_per_position_df.shape[0])
     mismatch_mappings_per_position_REF_list = np.asarray(list(original_seq)).repeat(mismatch_mappings_per_position_df.shape[0]).astype(np.object_)
     mismatch_mappings_per_position_ALT_list = mismatch_mappings_per_position_df.T.values.flatten()
-    mismatch_mappings_per_position_full_list = mismatch_mappings_per_position_POS_list.astype(np.str).astype(object)+mismatch_mappings_per_position_REF_list + np.repeat(">", len(mismatch_mappings_per_position_REF_list)) + mismatch_mappings_per_position_ALT_list
+    mismatch_mappings_per_position_full_list = mismatch_mappings_per_position_POS_list.astype(np.str_).astype(object)+mismatch_mappings_per_position_REF_list + np.repeat(">", len(mismatch_mappings_per_position_REF_list)) + mismatch_mappings_per_position_ALT_list
     encodings_per_position_list = encodings_per_position_df.T.values.flatten()
 
     
     # Encodings per position DF, mismatch mappings per position DF, encodings per position flattened, mismatch mappings per position flattened, mismatch mapping position in flattened list, mismatch mapping ref in flattened list, mismatch mapping alt in flattened list, all substitutions made
     
     index = pd.MultiIndex.from_tuples(zip(mismatch_mappings_per_position_full_list, mismatch_mappings_per_position_POS_list, mismatch_mappings_per_position_REF_list, mismatch_mappings_per_position_ALT_list), names=["FullChange", "Position","Ref", "Alt"])
```

### Comparing `crispr_millipede-0.1.8/pyproject.toml` & `crispr_millipede-0.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "crispr-millipede"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["Basheer Becerra <bbecerr@outlook.com>"]
 readme = "README.md"
 packages = [{include = "crispr_millipede"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
```

### Comparing `crispr_millipede-0.1.8/PKG-INFO` & `crispr_millipede-0.1.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crispr-millipede
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: Basheer Becerra
 Author-email: bbecerr@outlook.com
 Requires-Python: >=3.8,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

