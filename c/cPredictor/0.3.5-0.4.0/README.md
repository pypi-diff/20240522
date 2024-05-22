# Comparing `tmp/cPredictor-0.3.5-py3-none-any.whl.zip` & `tmp/cPredictor-0.4.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 22411 bytes, number of entries: 11
--rw-r--r--  2.0 unx    43185 b- defN 24-May-16 08:09 cPredictor/SVM_prediction.py
--rw-r--r--  2.0 unx      354 b- defN 24-May-16 08:09 cPredictor/__init__.py
--rw-r--r--  2.0 unx     6922 b- defN 24-May-16 08:09 cPredictor/tests/SVM_prediction_test.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-16 08:09 cPredictor/tests/__init__.py
--rw-r--r--  2.0 unx     8174 b- defN 24-May-16 08:09 cPredictor/tests/cPredictor_test_model.py
--rw-r--r--  2.0 unx    11357 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/LICENSE
--rw-r--r--  2.0 unx     3361 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/WHEEL
--rw-r--r--  2.0 unx      227 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      941 b- defN 24-May-16 08:10 cPredictor-0.3.5.dist-info/RECORD
-11 files, 74624 bytes uncompressed, 20803 bytes compressed:  72.1%
+Zip file size: 22416 bytes, number of entries: 11
+-rw-r--r--  2.0 unx    43233 b- defN 24-May-22 06:40 cPredictor/SVM_prediction.py
+-rw-r--r--  2.0 unx      354 b- defN 24-May-22 06:40 cPredictor/__init__.py
+-rw-r--r--  2.0 unx     6922 b- defN 24-May-22 06:40 cPredictor/tests/SVM_prediction_test.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-22 06:40 cPredictor/tests/__init__.py
+-rw-r--r--  2.0 unx     8174 b- defN 24-May-22 06:40 cPredictor/tests/cPredictor_test_model.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3361 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      227 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      941 b- defN 24-May-22 06:40 cPredictor-0.4.0.dist-info/RECORD
+11 files, 74672 bytes uncompressed, 20808 bytes compressed:  72.1%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: cPredictor/tests/__init__.py
 Comment: 
 
 Filename: cPredictor/tests/cPredictor_test_model.py
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/LICENSE
+Filename: cPredictor-0.4.0.dist-info/LICENSE
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/METADATA
+Filename: cPredictor-0.4.0.dist-info/METADATA
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/WHEEL
+Filename: cPredictor-0.4.0.dist-info/WHEEL
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/entry_points.txt
+Filename: cPredictor-0.4.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/top_level.txt
+Filename: cPredictor-0.4.0.dist-info/top_level.txt
 Comment: 
 
-Filename: cPredictor-0.3.5.dist-info/RECORD
+Filename: cPredictor-0.4.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cPredictor/SVM_prediction.py

```diff
@@ -233,14 +233,15 @@
             matrix_test = matrix_test.reindex(col_one_list, axis=1)
 
         new_col_values = np.full(len(matrix_test), 0)
         for col in missing_cols:
             matrix_test[col] = new_col_values
 
         matrix_test = matrix_test[matrix_test.columns.intersection(col_one_list)]
+        matrix_test = matrix_test[col_one_list]
         data_test = matrix_test.to_numpy(dtype="float16")
 
         logging.info('Processing test data')
         data_test = cpredictor.preprocess_data_test(data_test)
 
         if rejected is True:
             cpredictor.predict_only_svmrejection(Threshold_rej, OutputDir, data_test)
```

## cPredictor/__init__.py

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.3.5"
+__version__ = "0.4.0"
 
 from .SVM_prediction import SVM_predict
 from .SVM_prediction import SVM_import
 from .SVM_prediction import SVM_performance
 from .SVM_prediction import SVM_pseudobulk
 from .SVM_prediction import predpars
 from .SVM_prediction import importpars
```

## cPredictor/tests/cPredictor_test_model.py

```diff
@@ -172,15 +172,15 @@
 os.environ["GIT_PYTHON_REFRESH"] = "quiet"
 import git
 
 # Specify data types and output dirs
 reference = "test/cma_meta_atlas_rfe.h5ad"
 labels = "data/training_labels_meta.csv"
 outdir = "test_output/"
-cPredictor_version = "0.3.5"
+cPredictor_version = "0.4.0"
 
 print("Setup tokens")
 # Set environments and passwords
 DAGSHUB_USER_NAME = 'Arts-of-coding'
 DAGSHUB_TOKEN =  os.environ['DH_key']
 DAGSHUB_REPO_OWNER = 'Arts-of-coding'
 MLFLOW_EXPERIMENT_NAME = 'Cornea'
```

## Comparing `cPredictor-0.3.5.dist-info/LICENSE` & `cPredictor-0.4.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cPredictor-0.3.5.dist-info/METADATA` & `cPredictor-0.4.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cPredictor
-Version: 0.3.5
+Version: 0.4.0
 Summary: Cell command line predictor
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools ==68.2.2
 Requires-Dist: wheel
 Requires-Dist: python-build
 Requires-Dist: pytest-cov
```

## Comparing `cPredictor-0.3.5.dist-info/RECORD` & `cPredictor-0.4.0.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-cPredictor/SVM_prediction.py,sha256=8972cpamcVDflAcqAz3ocjNenIo13QRlpThMH34Zjm8,43185
-cPredictor/__init__.py,sha256=ye20bcsMXJLCNLdmqzTzjDgan2OaAgQ8wT00WD-cNDo,354
+cPredictor/SVM_prediction.py,sha256=GfXuomCub9FuKxY_VE8fdrh1qrqu3hx4PZrzozB4vfc,43233
+cPredictor/__init__.py,sha256=Iw_eeTRVY8gSFIhThkr54pUmtDID-f9v-whl_WjhKxs,354
 cPredictor/tests/SVM_prediction_test.py,sha256=sKJF3SHRSY6Njt1XD6ty-D_CkHcE4n1O57J5IMJkKak,6922
 cPredictor/tests/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-cPredictor/tests/cPredictor_test_model.py,sha256=NWA9XGx6_f78E3dMs3PVXUJKiAcGxFWAak-TIX0hVPM,8174
-cPredictor-0.3.5.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-cPredictor-0.3.5.dist-info/METADATA,sha256=O9B4NHihtm5UgymUp1AFS_Ci8O6K0HP8nhVxbbpH7cU,3361
-cPredictor-0.3.5.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-cPredictor-0.3.5.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
-cPredictor-0.3.5.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
-cPredictor-0.3.5.dist-info/RECORD,,
+cPredictor/tests/cPredictor_test_model.py,sha256=_Kk7tUIZO1Sv_k-dchETqZ7Gq9n6TqoN0i1L-Hq3VDA,8174
+cPredictor-0.4.0.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+cPredictor-0.4.0.dist-info/METADATA,sha256=jUaFTr10wir3NRvPNYac05wEeFafdIazNQ7o-P9TDhU,3361
+cPredictor-0.4.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+cPredictor-0.4.0.dist-info/entry_points.txt,sha256=jWviDlyXk8UTuVRVDXW5ihbZ7xWbKSt3uKRwjx2pvJw,227
+cPredictor-0.4.0.dist-info/top_level.txt,sha256=NXWRMFJ_ywM9zoRGffXs1j38bnAtf-odfECMfsNtJV4,11
+cPredictor-0.4.0.dist-info/RECORD,,
```

