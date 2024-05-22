# Comparing `tmp/nanoCEM-0.0.6.0.tar.gz` & `tmp/nanoCEM-0.0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nanoCEM-0.0.6.0.tar", last modified: Tue May 21 03:07:43 2024, max compression
+gzip compressed data, was "nanoCEM-0.0.6.1.tar", last modified: Wed May 22 05:16:48 2024, max compression
```

## Comparing `nanoCEM-0.0.6.0.tar` & `nanoCEM-0.0.6.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.925960 nanoCEM-0.0.6.0/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.0/LICENSE
--rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.0/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15657 2024-04-30 05:57:13.000000 nanoCEM-0.0.6.0/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3973 2024-05-03 02:57:20.000000 nanoCEM-0.0.6.0/nanoCEM/alignment_magnifier
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    14865 2024-05-21 03:07:40.000000 nanoCEM-0.0.6.0/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10833 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3597 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.0/nanoCEM/read_tombo_resquiggle.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-21 03:07:43.924960 nanoCEM-0.0.6.0/nanoCEM.egg-info/
--rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      545 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-05-21 03:07:43.000000 nanoCEM-0.0.6.0/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-05-21 03:07:43.925960 nanoCEM-0.0.6.0/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-05-21 03:03:56.000000 nanoCEM-0.0.6.0/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-22 05:16:48.671349 nanoCEM-0.0.6.1/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.1/LICENSE
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-22 05:16:48.671349 nanoCEM-0.0.6.1/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-04-30 05:56:15.000000 nanoCEM-0.0.6.1/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-22 05:16:48.671349 nanoCEM-0.0.6.1/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15831 2024-05-21 03:32:19.000000 nanoCEM-0.0.6.1/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3973 2024-05-03 02:57:20.000000 nanoCEM-0.0.6.1/nanoCEM/alignment_magnifier
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    14932 2024-05-22 05:12:35.000000 nanoCEM-0.0.6.1/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    11119 2024-05-21 15:27:22.000000 nanoCEM-0.0.6.1/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3597 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10184 2024-05-21 13:58:55.000000 nanoCEM-0.0.6.1/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6734 2024-05-21 13:58:55.000000 nanoCEM-0.0.6.1/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-04-30 05:56:16.000000 nanoCEM-0.0.6.1/nanoCEM/read_tombo_resquiggle.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-05-22 05:16:48.671349 nanoCEM-0.0.6.1/nanoCEM.egg-info/
+-rw-r--r--   0 zhguo     (1000) zhguo     (1000)     3073 2024-05-22 05:16:48.000000 nanoCEM-0.0.6.1/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      545 2024-05-22 05:16:48.000000 nanoCEM-0.0.6.1/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-05-22 05:16:48.000000 nanoCEM-0.0.6.1/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-05-22 05:16:48.000000 nanoCEM-0.0.6.1/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-05-22 05:16:48.000000 nanoCEM-0.0.6.1/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-05-22 05:16:48.671349 nanoCEM-0.0.6.1/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-05-22 05:16:34.000000 nanoCEM-0.0.6.1/setup.py
```

### Comparing `nanoCEM-0.0.6.0/LICENSE` & `nanoCEM-0.0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/PKG-INFO` & `nanoCEM-0.0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.6.0
+Version: 0.0.6.1
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.0 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.1 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.6.0/README.md` & `nanoCEM-0.0.6.1/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.6.1/nanoCEM/CE_magnifier_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     #                     control='/hdd_data/download/23s_rRNA_A2030/ivt/file', output='f5c_result_rna_re_2524',
     #                     subsample_ratio=1,rna=True,
     #                     ref="../example/data/23S_rRNA.fasta", pore='r9')
     # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=8,norm=True,base_shift='auto',pore='r9',
     #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_re',
     #                     subsample_ratio=1,kmer_size=3,
     #                     ref="../example/data/reverse/23S_rRNA_re.fasta", rna=True)
-    parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
+    parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=2030, len=10, strand='+', cpu=8,norm=True,base_shift='-1',pore='r9',
                         input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_2030',kmer_size=3,
                         subsample_ratio=1,
                         ref="../example/data/23S_rRNA.fasta", rna=True)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
@@ -173,14 +173,16 @@
         except:
             single_mode = True
         if args.control_fast5 is None:
             single_mode = True
 
     elif args.function == 'f5c_ev':
         from nanoCEM.read_f5c_eventalign import read_blow5
+        if args.base_shift !='auto':
+            args.base_shift = int(args.base_shift)
         df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
                                                             subsample_ratio, args.base_shift, args.norm, str(args.cpu),args.rna)
         df_wt['Group'] = 'Sample'
         if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
@@ -208,17 +210,18 @@
         except Exception as e:
             print(e)
             single_mode = True
         if args.control is None:
             single_mode = True
     elif args.function == 'f5c_re':
         from nanoCEM.read_f5c_resquiggle import read_blow5
-
+        if args.base_shift !='auto':
+            args.base_shift = int(args.base_shift)
         df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
-                                                            subsample_ratio, args.base_shift, args.norm, str(args.cpu),args.rna)
+                                                            subsample_ratio, args.base_shift, args.norm, str(args.cpu), args.rna)
         df_wt['Group'] = 'Sample'
         if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
                                                             subsample_ratio, args.base_shift, args.norm, str(args.cpu),args.rna)
             df_ivt['Group'] = 'Control'
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM/alignment_magnifier` & `nanoCEM-0.0.6.1/nanoCEM/alignment_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/cem_utils.py` & `nanoCEM-0.0.6.1/nanoCEM/cem_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -382,15 +382,16 @@
         new_df = pd.concat([pd.DataFrame(new_df),label], axis =1)
         new_df.columns=['PC1','PC2','Group']
         if np.sum(new_df['Group']=='Sample') > 10 and np.sum(new_df['Group']=='Control') > 10:
             manova = MANOVA.from_formula('PC1 + PC2 ~ Group', data=new_df)
             # 执行多元方差分析
             results = manova.mv_test()
             pvalue = results.summary().tables[3].iloc[0,5]
-            mean_differ = feature[label[0]=='Sample'][4].median() - feature[label[0]=='Control'][4].median()
+            kmer_center = int((kmer -1)/2)
+            mean_differ = feature[label[0]=='Sample'][kmer_center*4].median() - feature[label[0]=='Control'][kmer_center*4].median()
             result_list.append([item,pvalue,mean_differ])
         else:
             result_list.append([item, None])
     new_df = pd.DataFrame(result_list)
     new_df[1] = np.log10(new_df[1]) * (-1)
     new_df.columns = ['Position', 'P value(-log10)','Norm_differ']
     return new_df
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.6.1/nanoCEM/current_events_magnifier`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         parser_input.add_argument("--strand", default="+", help="Strand of your interest")
         parser_input.add_argument('-r', "--ref", required=True, help="fasta file")
         parser_input.add_argument('-t', "--cpu", default=4, type=int, help="num of process")
         parser_input.add_argument('--norm', action='store_true', help='Turn on the normalization mode')
         parser_input.add_argument('-s', "--subsample_ratio", default=1, type=float,
                                   help="Subsample ratio to select reads")
         parser_input.add_argument('--rna', action='store_true', help='Turn on the RNA mode')
-        parser_input.add_argument('--kmer_size', choices=[3,5,7],default=3, help="kmer size for PCA and MANOVA analysis")
+        parser_input.add_argument('--kmer_size', choices=['1','3','5','7'],default='3', help="kmer size for PCA and MANOVA analysis")
         parser_input.add_argument('-o', "--output", default="nanoCEM_result", help="output_file")
 
     # Define the argument parser
     parser = argparse.ArgumentParser(
         description='A sample tool designed to visualize the features that distinguish between two groups of ONT data at the site level. It supports two re-squiggle pipeline(Tombo and f5c).')
     subparsers = parser.add_subparsers(dest='function')
 
@@ -48,24 +48,24 @@
 
     # f5c subparser
     parser_f5c = subparsers.add_parser('f5c_ev', help='tackle f5c eventalign')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                             help="control_blow5_path")
-    parser_f5c.add_argument('--base_shift',choices=['auto',0,-1,-2,-3,-4,-5,-6,-7,-8],default='auto', help='base shift option')
+    parser_f5c.add_argument('--base_shift',choices=['auto','0','-1','-2','-3','-4','-5','-6','-7','-8'],default='auto', help='base shift option')
     parser_f5c.add_argument('--pore', choices=['r9', 'r10','rna004'], help='Select pore type', default='r9')
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('f5c_re', help='tackle f5c re-squiggle')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
                             help="control_blow5_path")
-    parser_f5c.add_argument('--base_shift',choices=['auto',0,-1,-2,-3,-4,-5,-6,-7,-8],default='auto', help='base shift option')
+    parser_f5c.add_argument('--base_shift',choices=['auto','0','-1','-2','-3','-4','-5','-6','-7','-8'],default='auto', help='base shift option')
     parser_f5c.add_argument('--pore', choices=['r9', 'r10','rna004'], help='Select pore type', default='r9')
     add_public_argument(parser_f5c)
 
     parser_f5c = subparsers.add_parser('move_table', help='tackle move_table from basecaller')
     parser_f5c.add_argument("-i", "--input", required=True,
                             help="blow5_path")
     parser_f5c.add_argument('-c', "--control",
@@ -120,14 +120,16 @@
         except:
             single_mode = True
         if args.control_fast5 is None:
             single_mode = True
 
     elif args.function == 'f5c_ev':
         from nanoCEM.read_f5c_eventalign import read_blow5
+        if args.base_shift !='auto':
+            args.base_shift = int(args.base_shift)
         df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
                                                             subsample_ratio, args.base_shift, args.norm, str(args.cpu),args.rna)
         df_wt['Group'] = 'Sample'
         if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
@@ -155,15 +157,16 @@
         except Exception as e:
             print(e)
             single_mode = True
         if args.control is None:
             single_mode = True
     elif args.function == 'f5c_re':
         from nanoCEM.read_f5c_resquiggle import read_blow5
-
+        if args.base_shift !='auto':
+            args.base_shift = int(args.base_shift)
         df_wt, aligned_num_wt, nucleotide_type = read_blow5(args.input, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
                                                             subsample_ratio, args.base_shift, args.norm, str(args.cpu),args.rna)
         df_wt['Group'] = 'Sample'
         if nucleotide_type == 'RNA' and not args.rna:
             raise RuntimeError("You need to add --rna to turn on the rna mode")
         try:
             df_ivt, aligned_num_ivt, _ = read_blow5(args.control, args.pos,args.ref, args.len, args.chrom, args.strand, args.pore,
@@ -193,14 +196,16 @@
     df_copy.to_csv(results_path + '/current_feature.csv', index=None)
     print("Feature file saved  in " + results_path + '/current_feature.csv')
     # draw current feature
     current_plot(df, results_path, args.pos, base_list, title,filter=True)
     if not single_mode:
         if args.kmer_size is None:
             args.kmer_size = 3
+        else:
+            args.kmer_size = int(args.kmer_size)
         # draw PCA
         kmer_size = args.kmer_size
         # df_copy.loc[:, 'Position'] = df_copy['Position'].astype(int)
         feature_matrix, label = extract_kmer_feature(df_copy,kmer_size, args.pos + 1)
         plot_PCA(feature_matrix, label, results_path)
         # draw p_value
         new_df = calculate_MANOVA_result( args.pos+1,df_copy,args.len,500,args.len,kmer_size)
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.6.1/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.6.1/nanoCEM/machine_learning_trainer.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/normalization.py` & `nanoCEM-0.0.6.1/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/plot.py` & `nanoCEM-0.0.6.1/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.6.1/nanoCEM/read_f5c_eventalign.py`

 * *Files 2% similar despite different names*

```diff
@@ -159,16 +159,14 @@
         print('There are '+str(info_df.shape[0]-df.shape[0])+" reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
     df["feature"] = df.apply(extract_feature,base_shift=base_shift,strand=strand,position=position,windows_length=length,norm=norm,axis=1)
     pbar.close()
 
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
-    if subsample_ratio<1:
-        df=df.sample(frac=subsample_ratio)
     final_feature=[]
     for item in df["feature"]:
         final_feature.extend(item)
     final_feature=pd.DataFrame(final_feature)
     final_feature.columns=['Read ID','Mean','STD','Median','Dwell time','Position']
     # if rna_mode:
     #     if strand == '+':
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.6.1/nanoCEM/read_f5c_resquiggle.py`

 * *Files 1% similar despite different names*

```diff
@@ -150,16 +150,14 @@
         print('There are ' + str(info_df.shape[0] - df.shape[0]) + " reads not found in your paf file ...")
     pbar = tqdm(total=df.shape[0], position=0, leave=True)
     df["feature"] = df.apply(extract_feature,kmer_model=kmer_model, strand = strand,base_shift=base_shift, norm=norm, axis=1)
     pbar.close()
 
     df.dropna(inplace=True)
     num_aligned = df.shape[0]
-    if subsample_ratio < 1:
-        df = df.sample(frac=subsample_ratio)
     final_feature = []
     for item in df["feature"]:
         final_feature.extend(item)
     final_feature = pd.DataFrame(final_feature)
     final_feature.columns = ['Read ID', 'Mean', 'STD', 'Median', 'Dwell time', 'Position']
     final_feature = final_feature[
         (final_feature['Position'] >= position - length) & (final_feature['Position'] <= position + length)]
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM/read_move_table.py` & `nanoCEM-0.0.6.1/nanoCEM/read_move_table.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.6.1/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.6.1/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.6.0
+Version: 0.0.6.1
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.0 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.6.1 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.6.0/nanoCEM.egg-info/SOURCES.txt` & `nanoCEM-0.0.6.1/nanoCEM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.6.0/setup.py` & `nanoCEM-0.0.6.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.6.0",
+    version="0.0.6.1",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

