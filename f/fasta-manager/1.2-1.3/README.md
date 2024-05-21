# Comparing `tmp/fasta-manager-1.2.tar.gz` & `tmp/fasta_manager-1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fasta-manager-1.2.tar", last modified: Mon Jan 22 15:25:24 2024, max compression
+gzip compressed data, was "fasta_manager-1.3.tar", last modified: Tue May 21 21:54:10 2024, max compression
```

## Comparing `fasta-manager-1.2.tar` & `fasta_manager-1.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.674956 fasta-manager-1.2/
--rw-rw-rw-   0        0        0     1084 2024-01-19 22:05:35.000000 fasta-manager-1.2/LICENSE
--rw-rw-rw-   0        0        0     2388 2024-01-22 15:25:24.674956 fasta-manager-1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1873 2024-01-22 15:24:53.000000 fasta-manager-1.2/README.md
--rw-rw-rw-   0        0        0      108 2024-01-19 22:05:35.000000 fasta-manager-1.2/pyproject.toml
--rw-rw-rw-   0        0        0      729 2024-01-22 15:25:24.674956 fasta-manager-1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.377821 fasta-manager-1.2/src/
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.674956 fasta-manager-1.2/src/fasta_manager.egg-info/
--rw-rw-rw-   0        0        0     2388 2024-01-22 15:25:24.000000 fasta-manager-1.2/src/fasta_manager.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      761 2024-01-22 15:25:24.000000 fasta-manager-1.2/src/fasta_manager.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-22 15:25:24.000000 fasta-manager-1.2/src/fasta_manager.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       45 2024-01-22 15:25:24.000000 fasta-manager-1.2/src/fasta_manager.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2024-01-22 15:25:24.000000 fasta-manager-1.2/src/fasta_manager.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.456230 fasta-manager-1.2/src/packages/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:05.000000 fasta-manager-1.2/src/packages/__init__.py
--rw-rw-rw-   0        0        0     4025 2024-01-21 23:22:05.000000 fasta-manager-1.2/src/packages/main.py
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.483569 fasta-manager-1.2/src/packages/plots/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/plots/__init__.py
--rw-rw-rw-   0        0        0     2969 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/plots/plot_generator.py
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.505477 fasta-manager-1.2/src/packages/sequences/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/sequences/__init__.py
--rw-rw-rw-   0        0        0      761 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/sequences/sequences.py
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.541814 fasta-manager-1.2/src/packages/stats/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/stats/__init__.py
--rw-rw-rw-   0        0        0     1699 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/stats/sequence_stats.py
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.628290 fasta-manager-1.2/src/packages/transformers/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/transformers/__init__.py
--rw-rw-rw-   0        0        0      347 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/transformers/abstract_transformer.py
--rw-rw-rw-   0        0        0     1584 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/transformers/duplicated_transformer.py
--rw-rw-rw-   0        0        0     1493 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/transformers/reverse_complement.py
-drwxrwxrwx   0        0        0        0 2024-01-22 15:25:24.672958 fasta-manager-1.2/src/packages/utils/
--rw-rw-rw-   0        0        0        0 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/utils/__init__.py
--rw-rw-rw-   0        0        0     2219 2024-01-21 23:22:10.000000 fasta-manager-1.2/src/packages/utils/seq_file_manager.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.357765 fasta_manager-1.3/
+-rw-rw-rw-   0        0        0     1084 2024-05-21 20:37:12.000000 fasta_manager-1.3/LICENSE
+-rw-rw-rw-   0        0        0     2359 2024-05-21 21:54:10.357264 fasta_manager-1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1844 2024-05-21 21:39:18.000000 fasta_manager-1.3/README.md
+-rw-rw-rw-   0        0        0      108 2024-05-21 21:46:37.000000 fasta_manager-1.3/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2024-05-21 21:54:10.358764 fasta_manager-1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.330264 fasta_manager-1.3/src/
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.356763 fasta_manager-1.3/src/fasta_manager.egg-info/
+-rw-rw-rw-   0        0        0     2359 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      761 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 21:54:10.000000 fasta_manager-1.3/src/fasta_manager.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.346766 fasta_manager-1.3/src/packages/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/__init__.py
+-rw-rw-rw-   0        0        0     4393 2024-05-21 21:36:14.000000 fasta_manager-1.3/src/packages/main.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.348263 fasta_manager-1.3/src/packages/plots/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/plots/__init__.py
+-rw-rw-rw-   0        0        0     3048 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/plots/plot_generator.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.349763 fasta_manager-1.3/src/packages/sequences/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/sequences/__init__.py
+-rw-rw-rw-   0        0        0      784 2024-05-21 21:34:56.000000 fasta_manager-1.3/src/packages/sequences/sequences.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.351263 fasta_manager-1.3/src/packages/stats/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/stats/__init__.py
+-rw-rw-rw-   0        0        0     1744 2024-05-21 21:13:57.000000 fasta_manager-1.3/src/packages/stats/sequence_stats.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.354263 fasta_manager-1.3/src/packages/transformers/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/__init__.py
+-rw-rw-rw-   0        0        0      356 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/abstract_transformer.py
+-rw-rw-rw-   0        0        0     1626 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/transformers/duplicated_transformer.py
+-rw-rw-rw-   0        0        0     1529 2024-05-21 21:35:49.000000 fasta_manager-1.3/src/packages/transformers/reverse_complement.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:54:10.355762 fasta_manager-1.3/src/packages/utils/
+-rw-rw-rw-   0        0        0        0 2024-05-21 20:37:12.000000 fasta_manager-1.3/src/packages/utils/__init__.py
+-rw-rw-rw-   0        0        0     2269 2024-05-21 21:36:04.000000 fasta_manager-1.3/src/packages/utils/seq_file_manager.py
```

### Comparing `fasta-manager-1.2/LICENSE` & `fasta_manager-1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fasta-manager-1.2/PKG-INFO` & `fasta_manager-1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fasta-manager
-Version: 1.2
+Name: fasta_manager
+Version: 1.3
 Summary: Manage your fasta files
 Home-page: https://github.com/santipvz/FASTA-manager
 Author: santipvz
 Author-email: santivzqzz@gmail.com
 Project-URL: Bug Tracker, https://github.com/santipvz/FASTA-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -54,15 +54,15 @@
 Example 3: Perform case transformation
 <pre><code>fasta --casefile upper</pre></code>
 
 You can also combine parameters where order doesn't matter.
 <pre><code>fasta --stats --plots --casefile lower --drename</pre></code>
 
 # Results
-The processed sequences will be stored in the `results` directory, and statistics (if computed) will be saved in the `stats` directory. Plots (if generated) will be saved in the `plots` directory
+The processed sequences will be stored in the `results` directory, and statistics will be saved in the `stats` directory. Plots will be saved in the `plots` directory
 
 # Input File Format
 The input files are expected to follow the format:
 
 <pre><code>>ID
 Sequence</pre></code>
```

### Comparing `fasta-manager-1.2/README.md` & `fasta_manager-1.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 Example 3: Perform case transformation
 <pre><code>fasta --casefile upper</pre></code>
 
 You can also combine parameters where order doesn't matter.
 <pre><code>fasta --stats --plots --casefile lower --drename</pre></code>
 
 # Results
-The processed sequences will be stored in the `results` directory, and statistics (if computed) will be saved in the `stats` directory. Plots (if generated) will be saved in the `plots` directory
+The processed sequences will be stored in the `results` directory, and statistics will be saved in the `stats` directory. Plots will be saved in the `plots` directory
 
 # Input File Format
 The input files are expected to follow the format:
 
 <pre><code>>ID
 Sequence</pre></code>
```

### Comparing `fasta-manager-1.2/setup.cfg` & `fasta_manager-1.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
-00000010: 203d 2066 6173 7461 2d6d 616e 6167 6572   = fasta-manager
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 320d  ..version = 1.2.
+00000010: 203d 2066 6173 7461 5f6d 616e 6167 6572   = fasta_manager
+00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 330d  ..version = 1.3.
 00000030: 0a61 7574 686f 7220 3d20 7361 6e74 6970  .author = santip
 00000040: 767a 0d0a 6175 7468 6f72 5f65 6d61 696c  vz..author_email
 00000050: 203d 2073 616e 7469 767a 717a 7a40 676d   = santivzqzz@gm
 00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
 00000070: 7469 6f6e 203d 204d 616e 6167 6520 796f  tion = Manage yo
 00000080: 7572 2066 6173 7461 2066 696c 6573 0d0a  ur fasta files..
 00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
```

### Comparing `fasta-manager-1.2/src/fasta_manager.egg-info/PKG-INFO` & `fasta_manager-1.3/src/fasta_manager.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: fasta-manager
-Version: 1.2
+Name: fasta_manager
+Version: 1.3
 Summary: Manage your fasta files
 Home-page: https://github.com/santipvz/FASTA-manager
 Author: santipvz
 Author-email: santivzqzz@gmail.com
 Project-URL: Bug Tracker, https://github.com/santipvz/FASTA-manager/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -54,15 +54,15 @@
 Example 3: Perform case transformation
 <pre><code>fasta --casefile upper</pre></code>
 
 You can also combine parameters where order doesn't matter.
 <pre><code>fasta --stats --plots --casefile lower --drename</pre></code>
 
 # Results
-The processed sequences will be stored in the `results` directory, and statistics (if computed) will be saved in the `stats` directory. Plots (if generated) will be saved in the `plots` directory
+The processed sequences will be stored in the `results` directory, and statistics will be saved in the `stats` directory. Plots will be saved in the `plots` directory
 
 # Input File Format
 The input files are expected to follow the format:
 
 <pre><code>>ID
 Sequence</pre></code>
```

### Comparing `fasta-manager-1.2/src/fasta_manager.egg-info/SOURCES.txt` & `fasta_manager-1.3/src/fasta_manager.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fasta-manager-1.2/src/packages/main.py` & `fasta_manager-1.3/src/packages/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,93 +1,106 @@
-'''Main module for the FASTA file processing tool'''
-import argparse
-import os
-
-from packages.utils.seq_file_manager import SeqFileManager
-from packages.plots.plot_generator import PlotGenerator
-from packages.sequences.sequences import Sequence
-from packages.transformers.duplicated_transformer import DuplicatedTransformer
-from packages.transformers.reverse_complement import ReverseComplement
-from packages.stats.sequence_stats import SequenceStats
-
-def apply_case_transformation(args, sequences):
-    '''Applies a case transformation to the sequences'''
-    if args.casefile == 'upper':
-        return [Sequence(seq.id, seq.seq.upper(), seq.file_name) for seq in sequences]
-    if args.casefile == 'lower':
-        return [Sequence(seq.id, seq.seq.lower(), seq.file_name) for seq in sequences]
-    return sequences
-
-def apply_duplicate_transformation(args, sequences):
-    '''Applies a duplicate transformation to the sequences'''
-    if args.dremove:
-        return DuplicatedTransformer(style='remove').transform(sequences)
-    if args.drename:
-        return DuplicatedTransformer(style='rename').transform(sequences)
-    return sequences
-
-def apply_sequence_transformation(args, sequences):
-    '''Applies a sequence transformation to the sequences'''
-    if args.reverse:
-        return ReverseComplement(style='reverse').transform(sequences)
-    if args.complement:
-        return ReverseComplement(style='complement').transform(sequences)
-    if args.rc:
-        return ReverseComplement(style='both').transform(sequences)
-    return sequences
-
-def main():
-    '''Main function'''
-    parser = argparse.ArgumentParser(description='FASTA file processing tool')
-    parser.add_argument('--dremove', action='store_true', help='Remove duplicates')
-    parser.add_argument('--drename', action='store_true', help='Rename duplicates')
-    parser.add_argument('--reverse', action='store_true', help='Reverse sequences')
-    parser.add_argument('--complement', action='store_true', help='Complement sequences')
-    parser.add_argument('--rc', action='store_true', help='Reverse complement sequences')
-    parser.add_argument('--stats', help='Compute stats', action='store_true')
-    parser.add_argument('--casefile', help='Case transformation (original, upper, lower)')
-    parser.add_argument('--plots', help='Generate plots', action='store_true')
-    args = parser.parse_args()
-
-
-    # Get the FASTA files in the current directory
-    current_directory = os.getcwd()
-    fasta_files = [file for file in os.listdir(current_directory) if file.endswith('.fasta')]
-
-    # Verify that there are FASTA files in the current directory
-    if not any([args.casefile, args.dremove, args.drename, args.reverse,
-                args.complement, args.rc, args.stats, args.plots]):
-        print('No transformation specified')
-        return
-
-    if not fasta_files:
-        print('No FASTA files found in the current directory')
-        return
-
-    stats_directory = os.path.join(current_directory, 'result_stats')
-
-    for filename in fasta_files:
-        seq_file_manager = SeqFileManager(input_filename=filename)
-        sequences = seq_file_manager.load_fasta(filename)
-
-        sequences = apply_case_transformation(args, sequences)
-
-        sequences = apply_duplicate_transformation(args, sequences)
-
-        sequences = apply_sequence_transformation(args, sequences)
-
-        if args.plots:
-            plot_generator = PlotGenerator(sequences, filename, 'result_plots')
-            plot_generator.generate_plots()
-
-        if args.stats:
-            sequence_stats = SequenceStats()
-            sequence_stats.generate_stats(sequences, stats_directory, filename)
-
-
-        # Process the sequences if any transformation was specified
-        if any([args.casefile, args.dremove, args.drename, args.reverse, args.complement, args.rc]):
-            output_directory = os.path.join(current_directory, 'result_formatted')
-            seq_file_manager.write_fasta(sequences, output_directory)
-
-if __name__ == '__main__':
-    main()
+'''Main module for the FASTA file processing tool'''
+import argparse
+import os
+
+from packages.utils.seq_file_manager import SeqFileManager
+from packages.plots.plot_generator import PlotGenerator
+from packages.sequences.sequences import Sequence
+from packages.transformers.duplicated_transformer import DuplicatedTransformer
+from packages.transformers.reverse_complement import ReverseComplement
+from packages.stats.sequence_stats import SequenceStats
+
+def apply_case_transformation(args, sequences):
+    '''Applies a case transformation to the sequences'''
+    if args.casefile == 'upper':
+        return [Sequence(seq.id, seq.seq.upper(), seq.file_name) for seq in sequences]
+    if args.casefile == 'lower':
+        return [Sequence(seq.id, seq.seq.lower(), seq.file_name) for seq in sequences]
+    return sequences
+
+def apply_duplicate_transformation(args, sequences):
+    '''Applies a duplicate transformation to the sequences'''
+    if args.dremove:
+        return DuplicatedTransformer(style='remove').transform(sequences)
+    if args.drename:
+        return DuplicatedTransformer(style='rename').transform(sequences)
+    return sequences
+
+def apply_sequence_transformation(args, sequences):
+    '''Applies a sequence transformation to the sequences'''
+    if args.reverse:
+        return ReverseComplement(style='reverse').transform(sequences)
+    if args.complement:
+        return ReverseComplement(style='complement').transform(sequences)
+    if args.rc:
+        return ReverseComplement(style='both').transform(sequences)
+    return sequences
+
+def main():
+    '''Main function'''
+    parser = argparse.ArgumentParser(description='FASTA file processing tool')
+    parser.add_argument('--dremove', action='store_true', help='Remove duplicates')
+    parser.add_argument('--drename', action='store_true', help='Rename duplicates')
+    parser.add_argument('--reverse', action='store_true', help='Reverse sequences')
+    parser.add_argument('--complement', action='store_true', help='Complement sequences')
+    parser.add_argument('--rc', action='store_true', help='Reverse complement sequences')
+    parser.add_argument('--stats', help='Compute stats', action='store_true')
+    parser.add_argument('--casefile', help='Case transformation (original, upper, lower)')
+    parser.add_argument('--plots', help='Generate plots', action='store_true')
+    args = parser.parse_args()
+
+
+    # Get the FASTA files in the current directory
+    current_directory = os.getcwd()
+    fasta_files = [file for file in os.listdir(current_directory) if file.endswith('.fasta')]
+
+    # Verify that there are FASTA files in the current directory
+    if not any([args.casefile, args.dremove, args.drename, args.reverse,
+                args.complement, args.rc, args.stats, args.plots]):
+        print('No transformation specified')
+        return
+
+    if not fasta_files:
+        print('No FASTA files found in the current directory')
+        return
+
+    stats_directory = os.path.join(current_directory, 'result_stats')
+
+    
+    for filename in fasta_files:
+        seq_file_manager = SeqFileManager(input_filename=filename)
+        sequences = seq_file_manager.load_fasta(filename)
+
+        # Auxiliar sequence in uppercase for stats and plots
+        aux_seq = [seq.upper() for seq in sequences]
+
+        sequences = apply_duplicate_transformation(args, sequences)
+
+        sequences = apply_sequence_transformation(args, sequences)
+
+        sequences = apply_case_transformation(args, sequences)
+
+        sequence_stats = SequenceStats()
+        sequence_stats.generate_stats(aux_seq, stats_directory, filename)
+
+        plot_generator = PlotGenerator(aux_seq, filename, 'result_plots')
+        plot_generator.generate_plots()
+
+        
+
+
+        # Process the sequences if any transformation was specified
+        if any([args.casefile, args.dremove, args.drename, args.reverse, args.complement, args.rc]):
+            output_directory = os.path.join(current_directory, 'result_formatted')
+            seq_file_manager.write_fasta(sequences, output_directory)
+
+if __name__ == '__main__':
+    main()
+
+    list_of_sequences = [Sequence('seq1', 'atgc'), Sequence('seq2', 'atgc')]
+
+    a = Sequence('seq1', 'atgccc').upper()
+
+    print(a)
+
+    for seq in list_of_sequences:
+        print(seq.upper())
```

### Comparing `fasta-manager-1.2/src/packages/plots/plot_generator.py` & `fasta_manager-1.3/src/packages/plots/plot_generator.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,79 +1,79 @@
-'''Module for generating plots from sequences.'''
-import os
-import pandas as pd
-import matplotlib.pyplot as plt
-
-class PlotGenerator:
-    '''Class for generating plots from sequences.'''
-    def __init__(self, sequences, input_path, plots_dir):
-        self.sequences = sequences
-        self.input_path = input_path
-        self.plots_dir = plots_dir
-        self.df = self.create_dataframe()
-
-    def create_dataframe(self):
-        '''Creates a DataFrame from the sequences.'''
-        seq_ids = [seq.id for seq in self.sequences]
-        seq_lengths = [len(seq.seq) for seq in self.sequences]
-
-        base_counts = {'A': [], 'C': [], 'T': [], 'G': []}
-        for seq in self.sequences:
-            for base, count_list in base_counts.items():
-                count_list.append(seq.seq.count(base))
-
-        data = {
-            'seq_id': seq_ids,
-            'len': seq_lengths,
-            'A': base_counts['A'],
-            'C': base_counts['C'],
-            'T': base_counts['T'],
-            'G': base_counts['G']
-        }
-        return pd.DataFrame(data)
-
-    def generate_histogram(self):
-        '''Generates a histogram of sequence lengths.'''
-        sequence_lengths = self.df['len']
-        plt.hist(sequence_lengths, bins=10, color='#DDA0DD')
-        plt.xlabel('Sequence length')
-        plt.ylabel('Frequency')
-        plt.title('Histogram of sequence length distribution')
-        plt.grid(True)
-        input_file_name = os.path.splitext(os.path.basename(self.input_path))[0]
-        histogram_filename = input_file_name + '_histogram.png'
-        histogram_filepath = os.path.join(self.plots_dir, histogram_filename)
-        os.makedirs(self.plots_dir, exist_ok=True)
-        plt.savefig(histogram_filepath)
-        plt.close()
-
-    def generate_boxplot(self):
-        '''Generates a box plot of base percentages.'''
-        base_counts = ['A', 'C', 'T', 'G']
-        total_lengths = self.df['len']
-        for base in base_counts:
-            self.df[base] = self.df[base] / total_lengths
-
-        box_colors = ['#FFC0CB', '#ADD8E6', '#90EE90', '#FFFF66']
-        plt.boxplot(self.df[base_counts].values, labels=base_counts, patch_artist=True)
-
-        plt.xticks([])
-
-        for patch, color in zip(plt.boxplot(self.df[base_counts].values,patch_artist=True)['boxes'],
-                                box_colors):
-            patch.set_facecolor(color)
-
-        plt.xlabel('Bases')
-        plt.ylabel('Percentage')
-        plt.title('Relative percentage of bases in the total length of sequences')
-
-        plt.grid(True)
-        input_file_name = os.path.splitext(os.path.basename(self.input_path))[0]
-        boxplot_filename = input_file_name + '_boxplot.png'
-        boxplot_filepath = os.path.join(self.plots_dir, boxplot_filename)
-        plt.savefig(boxplot_filepath)
-        plt.close()
-
-    def generate_plots(self):
-        '''Generates plots from the sequences.'''
-        self.generate_histogram()
-        self.generate_boxplot()
+'''Module for generating plots from sequences.'''
+import os
+import pandas as pd
+import matplotlib.pyplot as plt
+
+class PlotGenerator:
+    '''Class for generating plots from sequences.'''
+    def __init__(self, sequences, input_path, plots_dir):
+        self.sequences = sequences
+        self.input_path = input_path
+        self.plots_dir = plots_dir
+        self.df = self.create_dataframe()
+
+    def create_dataframe(self):
+        '''Creates a DataFrame from the sequences.'''
+        seq_ids = [seq.id for seq in self.sequences]
+        seq_lengths = [len(seq.seq) for seq in self.sequences]
+
+        base_counts = {'A': [], 'C': [], 'T': [], 'G': []}
+        for seq in self.sequences:
+            for base, count_list in base_counts.items():
+                count_list.append(seq.seq.count(base))
+
+        data = {
+            'seq_id': seq_ids,
+            'len': seq_lengths,
+            'A': base_counts['A'],
+            'C': base_counts['C'],
+            'T': base_counts['T'],
+            'G': base_counts['G']
+        }
+        return pd.DataFrame(data)
+
+    def generate_histogram(self):
+        '''Generates a histogram of sequence lengths.'''
+        sequence_lengths = self.df['len']
+        plt.hist(sequence_lengths, bins=10, color='#DDA0DD')
+        plt.xlabel('Sequence length')
+        plt.ylabel('Frequency')
+        plt.title('Histogram of sequence length distribution')
+        plt.grid(True)
+        input_file_name = os.path.splitext(os.path.basename(self.input_path))[0]
+        histogram_filename = input_file_name + '_histogram.png'
+        histogram_filepath = os.path.join(self.plots_dir, histogram_filename)
+        os.makedirs(self.plots_dir, exist_ok=True)
+        plt.savefig(histogram_filepath)
+        plt.close()
+
+    def generate_boxplot(self):
+        '''Generates a box plot of base percentages.'''
+        base_counts = ['A', 'C', 'T', 'G']
+        total_lengths = self.df['len']
+        for base in base_counts:
+            self.df[base] = self.df[base] / total_lengths
+
+        box_colors = ['#FFC0CB', '#ADD8E6', '#90EE90', '#FFFF66']
+        plt.boxplot(self.df[base_counts].values, labels=base_counts, patch_artist=True)
+
+        plt.xticks([])
+
+        for patch, color in zip(plt.boxplot(self.df[base_counts].values,patch_artist=True)['boxes'],
+                                box_colors):
+            patch.set_facecolor(color)
+
+        plt.xlabel('Bases')
+        plt.ylabel('Percentage')
+        plt.title('Relative percentage of bases in the total length of sequences')
+
+        plt.grid(True)
+        input_file_name = os.path.splitext(os.path.basename(self.input_path))[0]
+        boxplot_filename = input_file_name + '_boxplot.png'
+        boxplot_filepath = os.path.join(self.plots_dir, boxplot_filename)
+        plt.savefig(boxplot_filepath)
+        plt.close()
+
+    def generate_plots(self):
+        '''Generates plots from the sequences.'''
+        self.generate_histogram()
+        self.generate_boxplot()
```

### Comparing `fasta-manager-1.2/src/packages/sequences/sequences.py` & `fasta_manager-1.3/src/packages/sequences/sequences.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-'''This module contains the Sequence class.'''
-## Definition of the Sequence class
-
-class Sequence:
-    '''This class represents a sequence.'''
-    def __init__(self, sequence_id, sequence, file_name=None):
-        self.id = sequence_id
-        self.seq = sequence
-        self.file_name = file_name
-
-    def __repr__(self):
-        return f'{self.id}: {self.seq}'
-
-    def __str__(self):
-        return f'{self.id}: {self.seq}\n'
-
-    def lower(self):
-        '''Returns a new Sequence object with the sequence in lowercase.'''
-        return Sequence(self.id, self.seq.lower(), self.file_name)
-
-    def upper(self):
-        '''Returns a new Sequence object with the sequence in uppercase.'''
-        return Sequence(self.id, self.seq.upper(), self.file_name)
+'''This module contains the Sequence class.'''
+## Definition of the Sequence class
+
+class Sequence:
+    '''This class represents a sequence.'''
+    def __init__(self, sequence_id, sequence, file_name=None):
+        self.id = sequence_id
+        self.seq = sequence
+        self.file_name = file_name
+
+    def __repr__(self):
+        return f'{self.id}: {self.seq}'
+
+    def __str__(self):
+        return f'{self.id}: {self.seq}\n'
+
+    def lower(self):
+        '''Returns a new Sequence object with the sequence in lowercase.'''
+        return Sequence(self.id, self.seq.lower(), self.file_name)
+
+    def upper(self):
+        '''Returns a new Sequence object with the sequence in uppercase.'''
+        return Sequence(self.id, self.seq.upper(), self.file_name)
```

### Comparing `fasta-manager-1.2/src/packages/transformers/duplicated_transformer.py` & `fasta_manager-1.3/src/packages/transformers/duplicated_transformer.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-'''Returns a list of Sequence objects with the specified transformation.'''
-# pylint: disable=too-few-public-methods
-from .abstract_transformer import AbstractTransformer
-
-class DuplicatedTransformer(AbstractTransformer):
-    '''Returns a list of Sequence objects with the specified transformation.'''
-    def __init__(self, style):
-        self.style = style
-
-    def transform(self, sequence):
-        new_seq_list = []
-
-        if self.style == 'rename':
-            id_dict = {}
-            duplicate_count = {}
-            for seq in sequence:
-                seq_id = seq.id
-                if seq_id in id_dict:
-                    if seq_id not in duplicate_count:
-                        duplicate_count[seq_id] = 1
-                        id_dict[seq_id].id = f'{seq_id}.{duplicate_count[seq_id]}'
-                        seq.id = f'{seq_id}.{duplicate_count[seq_id] + 1}'
-                        id_dict[seq.id] = seq
-                        duplicate_count[seq_id] += 1
-                    else:
-                        duplicate_count[seq_id] += 1
-                        seq.id = f'{seq_id}.{duplicate_count[seq_id]}'
-                        id_dict[seq.id] = seq
-                else:
-                    id_dict[seq_id] = seq
-            new_seq_list = list(id_dict.values())
-
-
-        elif self.style == 'remove':
-            id_dict = {}
-            for seq in sequence:
-                seq_id = seq.id
-                if seq_id not in id_dict:
-                    id_dict[seq_id] = seq
-            new_seq_list = list(id_dict.values())
-
-        return new_seq_list
+'''Returns a list of Sequence objects with the specified transformation.'''
+# pylint: disable=too-few-public-methods
+from .abstract_transformer import AbstractTransformer
+
+class DuplicatedTransformer(AbstractTransformer):
+    '''Returns a list of Sequence objects with the specified transformation.'''
+    def __init__(self, style):
+        self.style = style
+
+    def transform(self, sequence):
+        new_seq_list = []
+
+        if self.style == 'rename':
+            id_dict = {}
+            duplicate_count = {}
+            for seq in sequence:
+                seq_id = seq.id
+                if seq_id in id_dict:
+                    if seq_id not in duplicate_count:
+                        duplicate_count[seq_id] = 1
+                        id_dict[seq_id].id = f'{seq_id}.{duplicate_count[seq_id]}'
+                        seq.id = f'{seq_id}.{duplicate_count[seq_id] + 1}'
+                        id_dict[seq.id] = seq
+                        duplicate_count[seq_id] += 1
+                    else:
+                        duplicate_count[seq_id] += 1
+                        seq.id = f'{seq_id}.{duplicate_count[seq_id]}'
+                        id_dict[seq.id] = seq
+                else:
+                    id_dict[seq_id] = seq
+            new_seq_list = list(id_dict.values())
+
+
+        elif self.style == 'remove':
+            id_dict = {}
+            for seq in sequence:
+                seq_id = seq.id
+                if seq_id not in id_dict:
+                    id_dict[seq_id] = seq
+            new_seq_list = list(id_dict.values())
+
+        return new_seq_list
```

### Comparing `fasta-manager-1.2/src/packages/transformers/reverse_complement.py` & `fasta_manager-1.3/src/packages/transformers/reverse_complement.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,36 +1,36 @@
-'''Returns a list of Sequence objects with the reverse complement of the sequences.'''
-# pylint: disable=too-few-public-methods
-from packages.sequences.sequences import Sequence
-from .abstract_transformer import AbstractTransformer
-
-class ReverseComplement(AbstractTransformer):
-    '''Returns a list of Sequence objects with the reverse complement of the sequences.'''
-    def __init__(self, style):
-        self.style = style
-
-    def transform(self, sequence):
-        '''Returns a list of Sequence objects with the specified transformation.'''
-        toret = []
-        if self.style == 'reverse':
-            for seq in sequence:
-                toret.append(Sequence(seq.id, seq.seq[::-1], seq.file_name))
-
-        elif self.style == 'complement':
-            complements = {
-                'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A',
-                'a': 't', 'c': 'g', 'g': 'c', 't': 'a'
-            }
-            for seq in sequence:
-                toret.append(Sequence(seq.id, ''.join(complements[base] for base in seq.seq),
-                                      seq.file_name))
-
-        elif self.style == 'both':
-            complements = {
-                'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A',
-                'a': 't', 'c': 'g', 'g': 'c', 't': 'a'
-            }
-            for seq in sequence:
-                combined_seq = ''.join(complements[base] for base in seq.seq[::-1])
-                toret.append(Sequence(seq.id, combined_seq, seq.file_name))
-
-        return toret
+'''Returns a list of Sequence objects with the reverse complement of the sequences.'''
+# pylint: disable=too-few-public-methods
+from packages.sequences.sequences import Sequence
+from .abstract_transformer import AbstractTransformer
+
+class ReverseComplement(AbstractTransformer):
+    '''Returns a list of Sequence objects with the reverse complement of the sequences.'''
+    def __init__(self, style):
+        self.style = style
+
+    def transform(self, sequence):
+        '''Returns a list of Sequence objects with the specified transformation.'''
+        toret = []
+        if self.style == 'reverse':
+            for seq in sequence:
+                toret.append(Sequence(seq.id, seq.seq[::-1], seq.file_name))
+
+        elif self.style == 'complement':
+            complements = {
+                'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A',
+                'a': 't', 'c': 'g', 'g': 'c', 't': 'a'
+            }
+            for seq in sequence:
+                toret.append(Sequence(seq.id, ''.join(complements[base] for base in seq.seq),
+                                      seq.file_name))
+
+        elif self.style == 'both':
+            complements = {
+                'A': 'T', 'C': 'G', 'G': 'C', 'T': 'A',
+                'a': 't', 'c': 'g', 'g': 'c', 't': 'a'
+            }
+            for seq in sequence:
+                combined_seq = ''.join(complements[base] for base in seq.seq[::-1])
+                toret.append(Sequence(seq.id, combined_seq, seq.file_name))
+
+        return toret
```

### Comparing `fasta-manager-1.2/src/packages/utils/seq_file_manager.py` & `fasta_manager-1.3/src/packages/utils/seq_file_manager.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,49 @@
-'''Module for loading and writing fasta files.'''
-import os
-from packages.sequences.sequences import Sequence
-
-class SeqFileManager:
-    '''This class allows us to format sequences and load and write fasta files.'''
-    def __init__(self, input_filename=None):
-        self.input_filename = input_filename
-
-
-    def load_fasta(self, file_name):
-        '''Returns a list of Sequence objects from the fasta file.'''
-        sequences = []
-        with open(file_name, 'r', encoding='utf-8') as file:
-            current_id = None
-            current_seq = ''
-            for line in file:
-                line = line.strip()
-                if line.startswith('>'):
-                    if current_id is not None:
-                        # Provide the file_name parameter when creating Sequence objects
-                        sequences.append(Sequence(current_id, current_seq, file_name))
-                    current_id = line[1:]
-                    current_seq = ''
-                else:
-                    current_seq += line
-            if current_id is not None:
-                # Provide the file_name parameter when creating Sequence objects
-                sequences.append(Sequence(current_id, current_seq, file_name))
-        return sequences
-
-    # En la clase SeqFileManager en packages/Utils/seq_file_manager.py
-    def write_fasta(self, sequences, output_directory):
-        '''Writes all sequences to individual files in the output directory.'''
-        os.makedirs(output_directory, exist_ok=True)  # Ensure the output directory exists
-
-        for i, sequence in enumerate(sequences):
-            # Use the input file name (sequence.file_name) without extension for the output file
-            input_file_name = os.path.splitext(os.path.basename(sequence.file_name))[0]
-            output_filename = f"{input_file_name}_result.fasta"
-            output_file_path = os.path.join(output_directory, output_filename)
-
-            # Use 'w' mode for the first sequence, 'a' mode for subsequent sequences
-            mode = 'w' if i == 0 else 'a'
-
-            with open(output_file_path, mode, encoding='utf-8') as f:
-                f.write(f'>{sequence.id}\n')
-                f.write(f'{sequence.seq}\n')
+'''Module for loading and writing fasta files.'''
+import os
+from packages.sequences.sequences import Sequence
+
+class SeqFileManager:
+    '''This class allows us to format sequences and load and write fasta files.'''
+    def __init__(self, input_filename=None):
+        self.input_filename = input_filename
+
+
+    def load_fasta(self, file_name):
+        '''Returns a list of Sequence objects from the fasta file.'''
+        sequences = []
+        with open(file_name, 'r', encoding='utf-8') as file:
+            current_id = None
+            current_seq = ''
+            for line in file:
+                line = line.strip()
+                if line.startswith('>'):
+                    if current_id is not None:
+                        # Provide the file_name parameter when creating Sequence objects
+                        sequences.append(Sequence(current_id, current_seq, file_name))
+                    current_id = line[1:]
+                    current_seq = ''
+                else:
+                    current_seq += line
+            if current_id is not None:
+                # Provide the file_name parameter when creating Sequence objects
+                sequences.append(Sequence(current_id, current_seq, file_name))
+
+        return sequences
+
+    # En la clase SeqFileManager en packages/Utils/seq_file_manager.py
+    def write_fasta(self, sequences, output_directory):
+        '''Writes all sequences to individual files in the output directory.'''
+        os.makedirs(output_directory, exist_ok=True)  # Ensure the output directory exists
+
+        for i, sequence in enumerate(sequences):
+            # Use the input file name (sequence.file_name) without extension for the output file
+            input_file_name = os.path.splitext(os.path.basename(sequence.file_name))[0]
+            output_filename = f"{input_file_name}_result.fasta"
+            output_file_path = os.path.join(output_directory, output_filename)
+
+            # Use 'w' mode for the first sequence, 'a' mode for subsequent sequences
+            mode = 'w' if i == 0 else 'a'
+
+            with open(output_file_path, mode, encoding='utf-8') as f:
+                f.write(f'>{sequence.id}\n')
+                f.write(f'{sequence.seq}\n')
```

