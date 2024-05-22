# Comparing `tmp/twinstop-0.1.2.tar.gz` & `tmp/twinstop-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twinstop-0.1.2.tar", last modified: Fri Aug  4 19:46:16 2023, max compression
+gzip compressed data, was "twinstop-0.1.3.tar", last modified: Wed May 22 09:27:45 2024, max compression
```

## Comparing `twinstop-0.1.2.tar` & `twinstop-0.1.3.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.2/LICENSE
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      745 2023-08-04 19:46:16.246145 twinstop-0.1.2/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      244 2023-07-28 19:58:25.000000 twinstop-0.1.2/README.md
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.2/pyproject.toml
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1054 2023-08-04 19:46:16.246145 twinstop-0.1.2/setup.cfg
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.2/setup.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.242145 twinstop-0.1.2/src/
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.2/src/twinstop/__init__.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2023-08-04 19:45:45.000000 twinstop-0.1.2/src/twinstop/_version.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4218 2023-07-28 21:23:19.000000 twinstop-0.1.2/src/twinstop/block_selection.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop/data_files/
--rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.def.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.pre.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.sen.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.2/src/twinstop/data_files/scaler.pkl
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp2.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   120533 2023-07-28 21:22:59.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   131351 2023-08-04 19:44:16.000000 twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.py
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6950 2023-07-28 21:23:28.000000 twinstop-0.1.2/src/twinstop/test_alignment_methods.py
-drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2023-08-04 19:46:16.246145 twinstop-0.1.2/src/twinstop.egg-info/
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      745 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/PKG-INFO
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      740 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/SOURCES.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/dependency_links.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      206 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/requires.txt
--rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2023-08-04 19:46:16.000000 twinstop-0.1.2/src/twinstop.egg-info/top_level.txt
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1071 2023-07-25 10:35:28.000000 twinstop-0.1.3/LICENSE
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1800 2024-05-22 09:27:45.622280 twinstop-0.1.3/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      928 2024-05-22 09:20:18.000000 twinstop-0.1.3/README.md
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      104 2021-06-11 14:00:42.000000 twinstop-0.1.3/pyproject.toml
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1054 2024-05-22 09:27:45.622280 twinstop-0.1.3/setup.cfg
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       69 2021-06-14 10:13:07.000000 twinstop-0.1.3/setup.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.614280 twinstop-0.1.3/src/
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.618280 twinstop-0.1.3/src/twinstop/
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       93 2023-07-25 10:19:10.000000 twinstop-0.1.3/src/twinstop/__init__.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)       20 2024-05-22 09:20:40.000000 twinstop-0.1.3/src/twinstop/_version.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4218 2023-07-28 21:23:19.000000 twinstop-0.1.3/src/twinstop/block_selection.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/src/twinstop/data_files/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     2003 2023-07-25 13:30:48.000000 twinstop-0.1.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.def.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1461 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.pre.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     1462 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.sen.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     4142 2023-07-25 14:46:08.000000 twinstop-0.1.3/src/twinstop/data_files/scaler.pkl
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   111812 2023-07-25 14:44:05.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   120533 2023-07-28 21:22:59.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)   141246 2024-05-22 09:14:30.000000 twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.py
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)     6950 2023-07-28 21:23:28.000000 twinstop-0.1.3/src/twinstop/test_alignment_methods.py
+drwxrwxr-x   0 mmariotti  (1000) mmariotti  (1000)        0 2024-05-22 09:27:45.622280 twinstop-0.1.3/src/twinstop.egg-info/
+-rw-r--r--   0 mmariotti  (1000) mmariotti  (1000)     1800 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/PKG-INFO
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      740 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/SOURCES.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        1 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/dependency_links.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)      206 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/requires.txt
+-rw-rw-r--   0 mmariotti  (1000) mmariotti  (1000)        9 2024-05-22 09:27:45.000000 twinstop-0.1.3/src/twinstop.egg-info/top_level.txt
```

### Comparing `twinstop-0.1.2/LICENSE` & `twinstop-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/setup.cfg` & `twinstop-0.1.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/block_selection.py` & `twinstop-0.1.3/src/twinstop/block_selection.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/data_files/Matrix_BLOSUM62sel.txt` & `twinstop-0.1.3/src/twinstop/data_files/Matrix_BLOSUM62sel.txt`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.def.pkl` & `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.def.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.pre.pkl` & `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.pre.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/data_files/logistic_regression_model.sen.pkl` & `twinstop-0.1.3/src/twinstop/data_files/logistic_regression_model.sen.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/data_files/scaler.pkl` & `twinstop-0.1.3/src/twinstop/data_files/scaler.pkl`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp2.py` & `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp2.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.bkp3.py` & `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.bkp3.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop/denovo_selenoproteins_h3.py` & `twinstop-0.1.3/src/twinstop/denovo_selenoproteins_h3.py`

 * *Files 2% similar despite different names*

```diff
@@ -87,15 +87,15 @@
 description_of_phases = {
     0: "Running tblastx between the transcriptomes",
     1: "Extracting CDS sequences and translating to get protein sequences",
     2: "Partitioning in UGA-containing ORFs, selecting best one per candidate",
     3: "Removing redundancy due to overlapping blast hits",
     4: "Extending to have complete ORFs, then removing duplicates and non-UGA containing ORFs",
     5: "Performing pairwise alignments between complete UGA-containing ORFs",
-    6: "Filtering out candidates that do not have UGA-UGA alignments",
+    6: "Filtering out candidates lacking UGA-UGA alignments, and keep one result per transcript",
     7: "Filtering candidates based on sequence conservation and other features",
     8: "Annotating candidates through blastp",
     9: "Producing output files",
 }
 
 m = max([len(i) for i in titles_of_phases.values()])
 phases_help = """\n### Description of phases\n""" + "\n".join(
@@ -1616,14 +1616,265 @@
     )
     # DataFrame is sorted by 'Density_Score' and saved.
     candidates.sort_values(by="Density_Score", inplace=True, ignore_index=True)
 
     return candidates
 
 
+def UGA_filter_each_row(row):
+    #write(row, how='green')
+    aligned = True
+    # first, we need to select the U responsible for readthrough
+    index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
+    # filters candidates with at least one aligned 'U'
+    if not index_u is None:
+        # counts the number of U's in both protein sequences
+        n_stops_subj = row["Subj_align_prot_seq"].count("U")
+        n_stops_query = row["Q_align_prot_seq"].count("U")
+        # selenoproteins sequences usually contains only one UGA responsible
+        # for readthrough. So, candidates with several U's will be trimmed.
+        if n_stops_subj >= 2 or n_stops_query >= 2:
+            # then the others Us (if any) indexes are stored in four lists
+            (
+                list_up_query,
+                list_down_query,
+                list_up_subj,
+                list_down_subj,
+            ) = list_UGAs(
+                row["Q_align_prot_seq"], row["Subj_align_prot_seq"], index_u
+            )
+            # cuts protein/nucleotide sequences from the closest up/downstream U to the selected 'U'.
+            # first, we cut downstream not to change the length of the sequences in case
+            # we need to cut upstream too. Trimmed parts are replaced with gaps.
+            if len(list_down_query) != 0:
+                query_cd = (
+                    len(
+                        row["Q_align_prot_seq"][list_down_query[0] + 1 :].replace(
+                            "-", ""
+                        )
+                    )
+                    * 3
+                )
+                row["Q_align_prot_seq"] = row["Q_align_prot_seq"][
+                    : list_down_query[0] + 1
+                ] + "-" * (len(row["Q_align_prot_seq"]) - list_down_query[0] - 1)
+                row["Query_CDS"] = row["Query_CDS"][
+                    : (
+                        list_down_query[0]
+                        + 1
+                        - row["Q_align_prot_seq"][: list_down_query[0] + 1].count(
+                            "-"
+                        )
+                    )
+                    * 3
+                ]
+                # print(f"row Query_CDS:\n {row['Query_CDS']}")
+            if len(list_up_query) != 0:
+                query_cu = (
+                    len(
+                        row["Q_align_prot_seq"][: list_up_query[-1]].replace(
+                            "-", ""
+                        )
+                    )
+                    + 1
+                ) * 3
+                # print('U upstream query')
+                # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
+                gaps_up = row["Q_align_prot_seq"][: list_up_query[-1] + 1].count(
+                    "-"
+                )
+                row["Q_align_prot_seq"] = (
+                    "-" * (list_up_query[-1] + 1)
+                    + row["Q_align_prot_seq"][list_up_query[-1] + 1 :]
+                )
+                # print(f"row Q_align_prot_seq:\n {row['Q_align_prot_seq']}")
+                # print(f"row Query_CDS:\n {row['Query_CDS']}")
+                row["Query_CDS"] = row["Query_CDS"][
+                    (list_up_query[-1] + 1 - gaps_up) * 3 :
+                ]
+                # print(f"row Query_CDS:\n {row['Query_CDS']}")
+            if len(list_down_subj) != 0:
+                subj_cd = (
+                    len(
+                        row["Subj_align_prot_seq"][list_down_subj[0] + 1 :].replace(
+                            "-", ""
+                        )
+                    )
+                    * 3
+                )
+                # print(f'subj_cd: {subj_cd}')
+                # print('U downstream subject')
+                # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
+                row["Subj_align_prot_seq"] = row["Subj_align_prot_seq"][
+                    : list_down_subj[0] + 1
+                ] + "-" * (len(row["Subj_align_prot_seq"]) - list_down_subj[0] - 1)
+                # print(f"row Subj_align_prot_seq:\n {row['Subj_align_prot_seq']}")
+                # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
+                row["Subj_CDS"] = row["Subj_CDS"][
+                    : (
+                        list_down_subj[0]
+                        + 1
+                        - row["Subj_align_prot_seq"][: list_down_subj[0] + 1].count(
+                            "-"
+                        )
+                    )
+                    * 3
+                ]
+                # print(f"row Subj_CDS:\n {row['Subj_CDS']}")
+            if len(list_up_subj) != 0:
+                subj_cu = (
+                    len(
+                        row["Subj_align_prot_seq"][: list_up_subj[-1]].replace(
+                            "-", ""
+                        )
+                    )
+                    + 1
+                ) * 3
+                gaps_up = row["Subj_align_prot_seq"][: list_up_subj[-1] + 1].count(
+                    "-"
+                )
+                row["Subj_align_prot_seq"] = (
+                    "-" * (list_up_subj[-1] + 1)
+                    + row["Subj_align_prot_seq"][list_up_subj[-1] + 1 :]
+                )
+                row["Subj_CDS"] = row["Subj_CDS"][
+                    (list_up_subj[-1] + 1 - gaps_up) * 3 :
+                ]
+
+            # updates the start/end positions according to strand value.
+            if len(list_up_subj) != 0:
+                # print('U upstream subject')
+                if row["Strand"] == "+":
+                    row["Start"] += subj_cu
+                else:
+                    row["End"] -= subj_cu
+            if len(list_down_subj) != 0:
+                if row["Strand"] == "+":
+                    row["End"] -= subj_cd
+                else:
+                    row["Start"] += subj_cd
+
+            if len(list_up_query) != 0:
+                # print('U upstream query')
+                if row["Q_Strand"] == "+":
+                    row["Q_align_s"] += query_cu
+                else:
+                    row["Q_align_e"] -= query_cu
+            if len(list_down_query) != 0:
+                # print('U downstream query')
+                if row["Q_Strand"] == "+":
+                    row["Q_align_e"] -= query_cd
+                else:
+                    row["Q_align_s"] += query_cd
+
+            prot_seq_query = ""
+            prot_seq_subj = ""
+            # deletes the non-sense gaps.
+            for idx, x in enumerate(row["Subj_align_prot_seq"]):
+                if x == "-" and row["Q_align_prot_seq"][idx] == "-":
+                    continue
+                else:
+                    prot_seq_query += row["Q_align_prot_seq"][idx]
+                    prot_seq_subj += x
+
+            row["Q_align_prot_seq"] = prot_seq_query
+            row["Subj_align_prot_seq"] = prot_seq_subj
+            index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
+
+        # counts the nº of gaps in both sequences.
+        n_gaps_subj = row["Subj_align_prot_seq"][:index_u].count("-")
+        n_gaps_query = row["Q_align_prot_seq"][:index_u].count("-")
+        # when using cds sequences we need to subtract the number of gaps and multiply by 3.
+        # (1 aa = 3 nucleotides).
+        index_3t_nucl_subj = (index_u - n_gaps_subj) * 3
+        index_3t_nucl_query = (index_u - n_gaps_query) * 3
+
+        # filters only when the selected 'U' = 'TGA'.
+        if not (
+            (row["Subj_CDS"][index_3t_nucl_subj : index_3t_nucl_subj + 3] == "TGA")
+            and (
+                row["Query_CDS"][index_3t_nucl_query : index_3t_nucl_query + 3]
+                == "TGA"
+            )
+        ):
+            raise SystemExit("Stop codon comparison did not match on:\n %s" % row)
+    else:
+        aligned = False
+    row['aligned']=aligned
+    return row
+
+def UGA_filter(df):
+    """ MM modified
+    Second filter of the script. During this filter, we will get only those hits
+    with aligned selenocysteines (U) and minimum values of conservation upstream
+    and downstream the in-frame-UGA.
+    Alignments with more than one aligned 'U' are cut to keep only one per hit.
+
+    Parameters
+    ----------
+    aligned_hits_df : <pd.DataFrame>
+        Dataframe with all the remaining hits.
+
+    Returns
+    -------
+    None
+        Modifies dataframe in place; also add column Aligned with boolean filter
+    """
+
+    df['aligned']=False
+    edited_columns='Q_align_s Q_align_e Start End Q_align_prot_seq Subj_align_prot_seq Query_CDS Subj_CDS'.split()
+    df[edited_columns]=df.apply(UGA_filter_each_row, axis=1)[edited_columns]
+    return df
+
+    if debugging:
+        pretty_out = pretty_output(filtered_out_candidates)
+        with open("filtered_out_candidates.txt", "w") as fw:
+            fw.write(pretty_out)
+
+    # updates the columns of the DataFrame.
+    candidates["Q_align_s"] = list_start_query
+    candidates["Q_align_e"] = list_end_query
+    candidates["Start"] = list_start_subj
+    candidates["End"] = list_end_subj
+    candidates["Q_align_prot_seq"] = list_prot_query
+    candidates["Subj_align_prot_seq"] = list_prot_subj
+    candidates["Query_CDS"] = list_cds_query
+    candidates["Subj_CDS"] = list_cds_subj
+    candidates["Score"] = list_score
+    candidates["Density_Score"] = list_density_score
+
+    candidates = candidates.reindex(
+        columns=[
+            "Density_Score",
+            "ID",
+            "Chromosome",
+            "Start",
+            "End",
+            "Subj_fr",
+            "Strand",
+            "Q_ID",
+            "Q_align_s",
+            "Q_align_e",
+            "Q_fr",
+            "Q_Strand",
+            "Score",
+            "Evalue",
+            "Subj_CDS",
+            "Query_CDS",
+            "Subj_align_prot_seq",
+            "Q_align_prot_seq",
+        ]
+    )
+    # DataFrame is sorted by 'Density_Score' and saved.
+    candidates.sort_values(by="Density_Score", inplace=True, ignore_index=True)
+
+    return candidates
+
+
+
 def find_sec_pos(row):
     # sec_annot_df = pd.DataFrame(columns=['ID', 'Chromosome', 'Start', 'End'])
     index_u = UGA(row["Q_align_prot_seq"], row["Subj_align_prot_seq"])
     if row["Strand"] == "+":
         sec_start = (
             index_u - row["Subj_align_prot_seq"][:index_u].count("-")
         ) * 3 + row["Start"]
@@ -2814,15 +3065,15 @@
 
     # first phase of the script is to run a tblastx between the query and subject transcriptomes to get the best
     # alignments among the transcripts.
     if not os.path.exists(path_tblastx_outfile) or n_section == 0:
 
         if not os.path.exists(subj_file+'.nin'):
             write('The subject file is not formatted for blast! Running makeblastdb')
-            cmd_makeblastdb = "makeblastdb -in " + subj_file+ + " -dbtype nucl"
+            cmd_makeblastdb = "makeblastdb -in " + subj_file + " -dbtype nucl"
             cmd_makeblastdb_list = shlex.split(cmd_makeblastdb)
             # subprocess.run allows to execute external programs inside a Python code
             y = subprocess.run(cmd_makeblastdb_list, capture_output=True)
             # controls that the subject transcriptome is nucleotide dtype, else raises Exception
             if y.returncode != 0:
                 write(y.stderr, y.stdout)
                 raise Exception()
```

### Comparing `twinstop-0.1.2/src/twinstop/test_alignment_methods.py` & `twinstop-0.1.3/src/twinstop/test_alignment_methods.py`

 * *Files identical despite different names*

### Comparing `twinstop-0.1.2/src/twinstop.egg-info/SOURCES.txt` & `twinstop-0.1.3/src/twinstop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

