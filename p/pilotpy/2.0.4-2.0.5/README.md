# Comparing `tmp/pilotpy-2.0.4.tar.gz` & `tmp/pilotpy-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pilotpy-2.0.4.tar", max compression
+gzip compressed data, was "pilotpy-2.0.5.tar", max compression
```

## Comparing `pilotpy-2.0.4.tar` & `pilotpy-2.0.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1098 2024-05-02 06:16:17.000000 pilotpy-2.0.4/LICENSE
--rw-r--r--   0        0        0     3374 2024-05-17 12:26:52.755763 pilotpy-2.0.4/README.md
--rw-r--r--   0        0        0      810 2024-05-17 12:19:38.785901 pilotpy-2.0.4/pyproject.toml
--rw-r--r--   0        0        0      139 2024-05-17 12:13:45.796641 pilotpy-2.0.4/src/pilotpy/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0      139 2024-05-17 12:13:45.796641 pilotpy-2.0.4/src/pilotpy/__init__.py
--rw-r--r--   0        0        0       20 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/pl.py
--rw-r--r--   0        0        0      131 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/plot/__init__.py
--rw-r--r--   0        0        0      334 2024-05-06 14:07:55.719657 pilotpy-2.0.4/src/pilotpy/plot/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4347 2024-05-06 14:07:55.931656 pilotpy-2.0.4/src/pilotpy/plot/__pycache__/curve_activity.cpython-311.pyc
--rw-r--r--   0        0        0    64363 2024-05-06 14:07:55.937656 pilotpy-2.0.4/src/pilotpy/plot/__pycache__/gene_selection_analysis.cpython-311.pyc
--rw-r--r--   0        0        0   112825 2024-05-06 14:07:55.731657 pilotpy-2.0.4/src/pilotpy/plot/__pycache__/ploting.cpython-311.pyc
--rw-r--r--   0        0        0    31410 2024-05-06 14:07:55.941656 pilotpy-2.0.4/src/pilotpy/plot/__pycache__/pseudobulk_DE_analysis.cpython-311.pyc
--rw-r--r--   0        0        0     2782 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/plot/curve_activity.py
--rw-r--r--   0        0        0    54721 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/plot/gene_selection_analysis.py
--rw-r--r--   0        0        0    87552 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/plot/ploting.py
--rw-r--r--   0        0        0    25134 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/plot/pseudobulk_DE_analysis.py
--rw-r--r--   0        0        0       21 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tl.py
--rw-r--r--   0        0        0      184 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0    29801 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/Cell_gene_selection.py
--rw-r--r--   0        0        0    11338 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/Gene_cluster_specific.py
--rw-r--r--   0        0        0    29947 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/Gene_cluster_specific_functions.py
--rw-r--r--   0        0        0    65958 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/Trajectory.py
--rw-r--r--   0        0        0      184 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/__init__.py
--rw-r--r--   0        0        0    44031 2024-05-06 14:07:56.648652 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Cell_gene_selection.cpython-311.pyc
--rw-r--r--   0        0        0    13816 2024-05-06 14:07:56.954650 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Gene_cluster_specific.cpython-311.pyc
--rw-r--r--   0        0        0    40748 2024-05-06 14:07:55.927656 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Gene_cluster_specific_functions.cpython-311.pyc
--rw-r--r--   0        0        0    80194 2024-05-06 14:07:53.945667 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Trajectory.cpython-311.pyc
--rw-r--r--   0        0        0      395 2024-05-06 14:07:53.937667 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0    12257 2024-05-06 14:07:57.034650 pilotpy-2.0.4/src/pilotpy/tools/__pycache__/patients_sub_clustering.cpython-311.pyc
--rw-r--r--   0        0        0    10982 2024-05-02 06:16:17.000000 pilotpy-2.0.4/src/pilotpy/tools/patients_sub_clustering.py
--rw-r--r--   0        0        0     4604 1970-01-01 00:00:00.000000 pilotpy-2.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-02 06:16:17.000000 pilotpy-2.0.5/LICENSE
+-rw-r--r--   0        0        0     3318 2024-05-22 09:46:32.655923 pilotpy-2.0.5/README.md
+-rw-r--r--   0        0        0      824 2024-05-22 09:46:11.686030 pilotpy-2.0.5/pyproject.toml
+-rw-r--r--   0        0        0      139 2024-05-22 09:47:15.529703 pilotpy-2.0.5/src/pilotpy/__init__.py
+-rw-r--r--   0        0        0       20 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/pl.py
+-rw-r--r--   0        0        0    54721 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/.ipynb_checkpoints/gene_selection_analysis-checkpoint.py
+-rw-r--r--   0        0        0      131 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/__init__.py
+-rw-r--r--   0        0        0      334 2024-05-06 14:07:55.719657 pilotpy-2.0.5/src/pilotpy/plot/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     4347 2024-05-06 14:07:55.931656 pilotpy-2.0.5/src/pilotpy/plot/__pycache__/curve_activity.cpython-311.pyc
+-rw-r--r--   0        0        0    64363 2024-05-06 14:07:55.937656 pilotpy-2.0.5/src/pilotpy/plot/__pycache__/gene_selection_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0   112825 2024-05-06 14:07:55.731657 pilotpy-2.0.5/src/pilotpy/plot/__pycache__/ploting.cpython-311.pyc
+-rw-r--r--   0        0        0    31410 2024-05-06 14:07:55.941656 pilotpy-2.0.5/src/pilotpy/plot/__pycache__/pseudobulk_DE_analysis.cpython-311.pyc
+-rw-r--r--   0        0        0     2782 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/curve_activity.py
+-rw-r--r--   0        0        0    54721 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/gene_selection_analysis.py
+-rw-r--r--   0        0        0    87552 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/ploting.py
+-rw-r--r--   0        0        0    25134 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/plot/pseudobulk_DE_analysis.py
+-rw-r--r--   0        0        0       21 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tl.py
+-rw-r--r--   0        0        0      184 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0    29801 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/Cell_gene_selection.py
+-rw-r--r--   0        0        0    11338 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/Gene_cluster_specific.py
+-rw-r--r--   0        0        0    29947 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/Gene_cluster_specific_functions.py
+-rw-r--r--   0        0        0    65958 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/Trajectory.py
+-rw-r--r--   0        0        0      184 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/__init__.py
+-rw-r--r--   0        0        0    44031 2024-05-06 14:07:56.648652 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Cell_gene_selection.cpython-311.pyc
+-rw-r--r--   0        0        0    13816 2024-05-06 14:07:56.954650 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Gene_cluster_specific.cpython-311.pyc
+-rw-r--r--   0        0        0    40748 2024-05-06 14:07:55.927656 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Gene_cluster_specific_functions.cpython-311.pyc
+-rw-r--r--   0        0        0    80194 2024-05-06 14:07:53.945667 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Trajectory.cpython-311.pyc
+-rw-r--r--   0        0        0      395 2024-05-06 14:07:53.937667 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0    12257 2024-05-06 14:07:57.034650 pilotpy-2.0.5/src/pilotpy/tools/__pycache__/patients_sub_clustering.cpython-311.pyc
+-rw-r--r--   0        0        0    10982 2024-05-02 06:16:17.000000 pilotpy-2.0.5/src/pilotpy/tools/patients_sub_clustering.py
+-rw-r--r--   0        0        0     4586 1970-01-01 00:00:00.000000 pilotpy-2.0.5/PKG-INFO
```

### Comparing `pilotpy-2.0.4/LICENSE` & `pilotpy-2.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/README.md` & `pilotpy-2.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -28,24 +28,22 @@
 - [4] Department of Internal Medicine, Nephrology and Transplantation, Erasmus Medical Center
 - [5] Department of Nephrology, $1^{st}$ Faculty of Medicine and General University Hospital, Charles University, Prague, Czech Republic
 - [6] John Walls Renal Unit, University Hospital of Leicester National Health Service Trust, Leicester, United Kingdom
 - [7] Department of Cardiovascular Sciences, University of Leicester, Leicester, United Kingdom
 - [8] Department of Cellular Pathology, Oxford University Hospitals National Health Services Foundation Trust, Oxford, United Kingdom
 - [9] Fondazione Ricerca Molinette. Regina Margherita Children's University Hospital, Torino, Italy
   
-Current version for PILOT is 2.0.4
+Current version for PILOT is 2.0.5
 
 ## Installation
 The easiest way to install PILOT and the required packages is using the following way:
 
 ```terminal
 conda create --name PILOT python=3.11.5 r-base
 conda activate PILOT
-conda install -c conda-forge rpy2
-conda install jupyter
 pip install pilotpy
 ```
 
 ## [Tutorial&Data sets](https://pilot.readthedocs.io/en/latest/index.html)
 There are five tutorials, one for [Myocardial Infarction (single cell data)](https://pilot.readthedocs.io/en/latest/Myocardial_infarction.html), and the second tutorial for [pathomics data, the combination of Kidney IgAN(G) & Kidney IgAN(T)](https://pilot.readthedocs.io/en/latest/Combination_Kidney_IgAN.html), and the third one  for [Patients sub-group detection and then ranking cells/genes (Pancreas data)](https://pilot.readthedocs.io/en/latest/Patients_sub_group_detection.html) and the forth one for 
 [evaluation of the presence of batch effects in Trajectory](https://pilot.readthedocs.io/en/latest/Kidney_trajectory.html) and the last one for [evaluation of the presence of batch effects in detected sub-groups](https://pilot.readthedocs.io/en/latest/Kidney_clusters.html).
```

### Comparing `pilotpy-2.0.4/pyproject.toml` & `pilotpy-2.0.5/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pilotpy"
-version = "2.0.4"
+version = "2.0.5"
 description = "PILOT: Detection of PatIent-Level distances from single cell genomics and pathomics data with Optimal Transport (PILOT)"
 authors = ["Mehdi Joodaki"]
 license = "MIT license"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "3.11.5"
@@ -24,12 +24,12 @@
 scipy = "^1.11.2"
 seaborn = "^0.12.2"
 shap = "^0.42.1"
 statsmodels = "^0.14.0"
 elpigraph-python = "^0.3.1"
 adjustText = "^0.8"
 gprofiler-official = "^1.0.0"
-
+rpy2="^3.5.11"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/__pycache__/curve_activity.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/plot/__pycache__/curve_activity.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/__pycache__/gene_selection_analysis.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/plot/__pycache__/gene_selection_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/__pycache__/ploting.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/plot/__pycache__/ploting.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/__pycache__/pseudobulk_DE_analysis.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/plot/__pycache__/pseudobulk_DE_analysis.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/curve_activity.py` & `pilotpy-2.0.5/src/pilotpy/plot/curve_activity.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/gene_selection_analysis.py` & `pilotpy-2.0.5/src/pilotpy/plot/.ipynb_checkpoints/gene_selection_analysis-checkpoint.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/ploting.py` & `pilotpy-2.0.5/src/pilotpy/plot/ploting.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/plot/pseudobulk_DE_analysis.py` & `pilotpy-2.0.5/src/pilotpy/plot/pseudobulk_DE_analysis.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/Cell_gene_selection.py` & `pilotpy-2.0.5/src/pilotpy/tools/Cell_gene_selection.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/Gene_cluster_specific.py` & `pilotpy-2.0.5/src/pilotpy/tools/Gene_cluster_specific.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/Gene_cluster_specific_functions.py` & `pilotpy-2.0.5/src/pilotpy/tools/Gene_cluster_specific_functions.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/Trajectory.py` & `pilotpy-2.0.5/src/pilotpy/tools/Trajectory.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Cell_gene_selection.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Cell_gene_selection.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Gene_cluster_specific.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Gene_cluster_specific.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Gene_cluster_specific_functions.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Gene_cluster_specific_functions.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/__pycache__/Trajectory.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/tools/__pycache__/Trajectory.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/__pycache__/patients_sub_clustering.cpython-311.pyc` & `pilotpy-2.0.5/src/pilotpy/tools/__pycache__/patients_sub_clustering.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/src/pilotpy/tools/patients_sub_clustering.py` & `pilotpy-2.0.5/src/pilotpy/tools/patients_sub_clustering.py`

 * *Files identical despite different names*

### Comparing `pilotpy-2.0.4/PKG-INFO` & `pilotpy-2.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pilotpy
-Version: 2.0.4
+Version: 2.0.5
 Summary: PILOT: Detection of PatIent-Level distances from single cell genomics and pathomics data with Optimal Transport (PILOT)
 License: MIT
 Author: Mehdi Joodaki
 Requires-Python: ==3.11.5
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: POT (>=0.9.1,<0.10.0)
@@ -16,14 +16,15 @@
 Requires-Dist: leidenalg (>=0.10.1,<0.11.0)
 Requires-Dist: matplotlib (>=3.8.0,<4.0.0)
 Requires-Dist: numpy (>=1.24.4,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
 Requires-Dist: plotly (>=5.22.0,<6.0.0)
 Requires-Dist: plotnine (>=0.12.3,<0.13.0)
 Requires-Dist: pydiffmap (>=0.2.0.1,<0.3.0.0)
+Requires-Dist: rpy2 (>=3.5.11,<4.0.0)
 Requires-Dist: scanpy (>=1.9.5,<2.0.0)
 Requires-Dist: scikit-learn (>=1.3.0,<2.0.0)
 Requires-Dist: scikit-network (>=0.31.0,<0.32.0)
 Requires-Dist: scipy (>=1.11.2,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: shap (>=0.42.1,<0.43.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
@@ -59,24 +60,22 @@
 - [4] Department of Internal Medicine, Nephrology and Transplantation, Erasmus Medical Center
 - [5] Department of Nephrology, $1^{st}$ Faculty of Medicine and General University Hospital, Charles University, Prague, Czech Republic
 - [6] John Walls Renal Unit, University Hospital of Leicester National Health Service Trust, Leicester, United Kingdom
 - [7] Department of Cardiovascular Sciences, University of Leicester, Leicester, United Kingdom
 - [8] Department of Cellular Pathology, Oxford University Hospitals National Health Services Foundation Trust, Oxford, United Kingdom
 - [9] Fondazione Ricerca Molinette. Regina Margherita Children's University Hospital, Torino, Italy
   
-Current version for PILOT is 2.0.4
+Current version for PILOT is 2.0.5
 
 ## Installation
 The easiest way to install PILOT and the required packages is using the following way:
 
 ```terminal
 conda create --name PILOT python=3.11.5 r-base
 conda activate PILOT
-conda install -c conda-forge rpy2
-conda install jupyter
 pip install pilotpy
 ```
 
 ## [Tutorial&Data sets](https://pilot.readthedocs.io/en/latest/index.html)
 There are five tutorials, one for [Myocardial Infarction (single cell data)](https://pilot.readthedocs.io/en/latest/Myocardial_infarction.html), and the second tutorial for [pathomics data, the combination of Kidney IgAN(G) & Kidney IgAN(T)](https://pilot.readthedocs.io/en/latest/Combination_Kidney_IgAN.html), and the third one  for [Patients sub-group detection and then ranking cells/genes (Pancreas data)](https://pilot.readthedocs.io/en/latest/Patients_sub_group_detection.html) and the forth one for 
 [evaluation of the presence of batch effects in Trajectory](https://pilot.readthedocs.io/en/latest/Kidney_trajectory.html) and the last one for [evaluation of the presence of batch effects in detected sub-groups](https://pilot.readthedocs.io/en/latest/Kidney_clusters.html).
```

