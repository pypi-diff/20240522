# Comparing `tmp/scprel-1.1.8.tar.gz` & `tmp/scprel-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/scprel-1.1.8.tar", last modified: Thu Nov 16 10:21:19 2023, max compression
+gzip compressed data, was "dist/scprel-1.1.9.tar", last modified: Thu Nov 16 11:01:04 2023, max compression
```

## Comparing `scprel-1.1.8.tar` & `scprel-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 10:21:19.000000 scprel-1.1.8/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1084 2023-11-14 15:25:46.000000 scprel-1.1.8/LICENSE.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2776 2023-11-16 10:21:19.000000 scprel-1.1.8/PKG-INFO
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1623 2023-11-16 10:16:11.000000 scprel-1.1.8/README.md
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 10:21:19.000000 scprel-1.1.8/scprel/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       36 2023-11-15 13:33:12.000000 scprel-1.1.8/scprel/__init__.py
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)    12383 2023-11-15 15:31:41.000000 scprel-1.1.8/scprel/functions.py
-drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 10:21:19.000000 scprel-1.1.8/scprel.egg-info/
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2776 2023-11-16 10:21:17.000000 scprel-1.1.8/scprel.egg-info/PKG-INFO
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)      218 2023-11-16 10:21:17.000000 scprel-1.1.8/scprel.egg-info/SOURCES.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        1 2023-11-16 10:21:17.000000 scprel-1.1.8/scprel.egg-info/dependency_links.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       81 2023-11-16 10:21:17.000000 scprel-1.1.8/scprel.egg-info/requires.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        7 2023-11-16 10:21:17.000000 scprel-1.1.8/scprel.egg-info/top_level.txt
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       38 2023-11-16 10:21:19.000000 scprel-1.1.8/setup.cfg
--rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1739 2023-11-16 10:20:53.000000 scprel-1.1.8/setup.py
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 11:01:04.000000 scprel-1.1.9/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1084 2023-11-14 15:25:46.000000 scprel-1.1.9/LICENSE.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2872 2023-11-16 11:01:04.000000 scprel-1.1.9/PKG-INFO
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1719 2023-11-16 11:00:22.000000 scprel-1.1.9/README.md
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 11:01:04.000000 scprel-1.1.9/scprel/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       36 2023-11-15 13:33:12.000000 scprel-1.1.9/scprel/__init__.py
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)    12377 2023-11-16 10:52:15.000000 scprel-1.1.9/scprel/functions.py
+drwxr-xr-x   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        0 2023-11-16 11:01:04.000000 scprel-1.1.9/scprel.egg-info/
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     2872 2023-11-16 11:01:02.000000 scprel-1.1.9/scprel.egg-info/PKG-INFO
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)      218 2023-11-16 11:01:02.000000 scprel-1.1.9/scprel.egg-info/SOURCES.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        1 2023-11-16 11:01:02.000000 scprel-1.1.9/scprel.egg-info/dependency_links.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       81 2023-11-16 11:01:02.000000 scprel-1.1.9/scprel.egg-info/requires.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)        7 2023-11-16 11:01:02.000000 scprel-1.1.9/scprel.egg-info/top_level.txt
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)       38 2023-11-16 11:01:04.000000 scprel-1.1.9/setup.cfg
+-rw-r--r--   0 g_puzanov (800697380) gs_hpc_u981 (800677181)     1739 2023-11-16 11:00:28.000000 scprel-1.1.9/setup.py
```

### Comparing `scprel-1.1.8/LICENSE.txt` & `scprel-1.1.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `scprel-1.1.8/PKG-INFO` & `scprel-1.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: scprel
-Version: 1.1.8
+Version: 1.1.9
 Summary: Single-cell data preprocessing for multiple samples.
 Home-page: https://pypi.org/project/scprel/
 Author: GPuzanov (Grigory Puzanov)
 Author-email: <grigorypuzanov@gmail.com>
 License: UNKNOWN
 Description: ## Scprel - Single-Cell Data Preprocessing in Python
         
         ### Import scprel as:
         
             import scprel
         
-        This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization, leiden clustering and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
+        This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization with `target_sum=1e4`, leiden clustering, annotation of cell types with [PanglaoDB](https://panglaodb.se/) database and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
         
         ### Example of usage:
         
             scprel.scrun(names = ['sample1', 'sample2'], path = '/content/drive/MyDrive/MyDirectory/')
         
         * *names - list of sample names in your directory (.h5 format);* 
         * *path - path to the directory with samples*
         
-        The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations. The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
+        The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations.
         
         ![The obs table for resulting adata file](https://raw.githubusercontent.com/ronnaug/1/Genomic_data_analysis/Example_table.png)
         
-        
+        The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
 Keywords: python,jupyter notebook,single-cell,scRNA-seq,single-cell quality control,single-cell data preparation,single-cell multiple samples,samples concatenation
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `scprel-1.1.8/README.md` & `scprel-1.1.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 ## Scprel - Single-Cell Data Preprocessing in Python
 
 ### Import scprel as:
 
     import scprel
 
-This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization, leiden clustering and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
+This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization with `target_sum=1e4`, leiden clustering, annotation of cell types with [PanglaoDB](https://panglaodb.se/) database and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
 
 ### Example of usage:
 
     scprel.scrun(names = ['sample1', 'sample2'], path = '/content/drive/MyDrive/MyDirectory/')
 
 * *names - list of sample names in your directory (.h5 format);* 
 * *path - path to the directory with samples*
 
-The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations. The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
+The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations.
 
 ![The obs table for resulting adata file](https://raw.githubusercontent.com/ronnaug/1/Genomic_data_analysis/Example_table.png)
 
+The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
```

### Comparing `scprel-1.1.8/scprel/functions.py` & `scprel-1.1.9/scprel/functions.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,15 +183,15 @@
             l = tuple(adata.var.index.tolist())
             l1 = lis(l)
         
             adata.var['chromosome'].loc[l1] = chro(tuple(l1))
             adata.var['start'].loc[l1] = sta(tuple(l1))
             adata.var['end'].loc[l1] = en(tuple(l1))
           
-        print('Infercnc calculations...')
+        print('Infercnv calculations...')
           
         
         for i in samr:
             adata = i
             reference_cat = []
             
             for j in adata.obs['cell_type'].unique():
@@ -227,15 +227,15 @@
                 ax=ax1,
                show=False,
             #save = 'firi_R_'+str(i)'cnvscore.png'
             )
             cnv.pl.umap(adata, color="cnv_score", ax=ax2, show=False)
             cnv.pl.umap(adata, color="cell_type", ax=ax3)
         
-            fig.savefig(path++str(names[k])+'cnvscore.png', dpi=300,  facecolor ='w')
+            fig.savefig(path+str(names[k])+'cnv.png', dpi=300,  facecolor ='w')
         
             k = k+1
             
         k = 0
           
         for i in samr:
             adata = i
```

### Comparing `scprel-1.1.8/scprel.egg-info/PKG-INFO` & `scprel-1.1.9/scprel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,35 @@
 Metadata-Version: 2.1
 Name: scprel
-Version: 1.1.8
+Version: 1.1.9
 Summary: Single-cell data preprocessing for multiple samples.
 Home-page: https://pypi.org/project/scprel/
 Author: GPuzanov (Grigory Puzanov)
 Author-email: <grigorypuzanov@gmail.com>
 License: UNKNOWN
 Description: ## Scprel - Single-Cell Data Preprocessing in Python
         
         ### Import scprel as:
         
             import scprel
         
-        This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization, leiden clustering and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
+        This package allows to perform basic preprocessing steps for single-cell analysis of multiple samples. It includes scrublets detection, quality control, normalization with `target_sum=1e4`, leiden clustering, annotation of cell types with [PanglaoDB](https://panglaodb.se/) database and infercnv calculations. It integrates some of the [Scanpy](https://scanpy.readthedocs.io/en/stable/), [Decoupler](https://decoupler-py.readthedocs.io/en/latest/), [Infercnvpy](https://infercnvpy.readthedocs.io/en/latest/infercnv.html) and [Anndata](https://anndata.readthedocs.io/en/latest/concatenation.html) functions. It is designed to facilitate workflow when analyzing multiple samples.
         
         ### Example of usage:
         
             scprel.scrun(names = ['sample1', 'sample2'], path = '/content/drive/MyDrive/MyDirectory/')
         
         * *names - list of sample names in your directory (.h5 format);* 
         * *path - path to the directory with samples*
         
-        The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations. The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
+        The result of this function is the [anndata.AnnData](https://anndata.readthedocs.io/en/stable/generated/anndata.AnnData.html#anndata.AnnData) object, compressed with [hdf5plugin](https://pypi.org/project/hdf5plugin/), with concatenated samples, filtered by 'mt' and 'ribo' genes, with annotated gene locations and annotated tumor cells based on cnv score. All immune cells in the sample are considered reference cells for infercnv calculations.
         
         ![The obs table for resulting adata file](https://raw.githubusercontent.com/ronnaug/1/Genomic_data_analysis/Example_table.png)
         
-        
+        The resulting file will be saved in your default home directory and is ready for batch correction and further analysis.
 Keywords: python,jupyter notebook,single-cell,scRNA-seq,single-cell quality control,single-cell data preparation,single-cell multiple samples,samples concatenation
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `scprel-1.1.8/setup.py` & `scprel-1.1.9/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 #import codecs
 
-VERSION = '1.1.8'
+VERSION = '1.1.9'
 DESCRIPTION = 'Single-cell data preprocessing for multiple samples.'
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 #with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
```

