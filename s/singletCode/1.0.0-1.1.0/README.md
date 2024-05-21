# Comparing `tmp/singletCode-1.0.0.tar.gz` & `tmp/singletcode-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "singletCode-1.0.0.tar", last modified: Mon Mar 25 17:21:40 2024, max compression
+gzip compressed data, was "singletcode-1.1.0.tar", last modified: Tue May 21 22:22:53 2024, max compression
```

## Comparing `singletCode-1.0.0.tar` & `singletcode-1.1.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-03-25 17:21:40.880124 singletCode-1.0.0/
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1507 2024-03-22 22:07:35.000000 singletCode-1.0.0/LICENSE
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4456 2024-03-25 17:21:40.880124 singletCode-1.0.0/PKG-INFO
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1752 2024-03-25 17:01:22.000000 singletCode-1.0.0/README.md
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)        6 2024-03-25 17:21:30.000000 singletCode-1.0.0/__version__
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1145 2024-03-25 16:59:07.000000 singletCode-1.0.0/pyproject.toml
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)       38 2024-03-25 17:21:40.880124 singletCode-1.0.0/setup.cfg
-drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-03-25 17:21:40.880124 singletCode-1.0.0/singletCode/
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)       98 2024-03-23 00:26:57.000000 singletCode-1.0.0/singletCode/__init__.py
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)    17050 2024-03-25 16:13:27.000000 singletCode-1.0.0/singletCode/count_doublets_utils_copy.py
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1902 2024-03-23 00:10:44.000000 singletCode-1.0.0/singletCode/general_utility_functions.py
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4131 2024-03-23 00:12:36.000000 singletCode-1.0.0/singletCode/get_singlets.py
-drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-03-25 17:21:40.880124 singletCode-1.0.0/singletCode.egg-info/
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4456 2024-03-25 17:21:40.000000 singletCode-1.0.0/singletCode.egg-info/PKG-INFO
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)      352 2024-03-25 17:21:40.000000 singletCode-1.0.0/singletCode.egg-info/SOURCES.txt
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)        1 2024-03-25 17:21:40.000000 singletCode-1.0.0/singletCode.egg-info/dependency_links.txt
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)       59 2024-03-25 17:21:40.000000 singletCode-1.0.0/singletCode.egg-info/requires.txt
--rw-r--r--   0 keerthana  (1000) keerthana  (1000)       12 2024-03-25 17:21:40.000000 singletCode-1.0.0/singletCode.egg-info/top_level.txt
+drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-05-21 22:22:53.967182 singletcode-1.1.0/
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1507 2024-03-23 02:30:11.000000 singletcode-1.1.0/LICENSE
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4289 2024-05-21 22:22:53.967182 singletcode-1.1.0/PKG-INFO
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1623 2024-03-23 02:30:11.000000 singletcode-1.1.0/README.md
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)        6 2024-05-21 21:32:16.000000 singletcode-1.1.0/__version__
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     1106 2024-03-23 02:30:11.000000 singletcode-1.1.0/pyproject.toml
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)       38 2024-05-21 22:22:53.967182 singletcode-1.1.0/setup.cfg
+drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-05-21 22:22:53.967182 singletcode-1.1.0/singletCode/
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)       98 2024-03-23 02:30:11.000000 singletcode-1.1.0/singletCode/__init__.py
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)    16552 2024-05-21 21:23:13.000000 singletcode-1.1.0/singletCode/count_doublets_utils_copy.py
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     2136 2024-05-21 21:23:49.000000 singletcode-1.1.0/singletCode/general_utility_functions.py
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4322 2024-05-21 22:16:58.000000 singletcode-1.1.0/singletCode/get_singlets.py
+drwxr-xr-x   0 keerthana  (1000) keerthana  (1000)        0 2024-05-21 22:22:53.967182 singletcode-1.1.0/singletCode.egg-info/
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)     4289 2024-05-21 22:22:53.000000 singletcode-1.1.0/singletCode.egg-info/PKG-INFO
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)      352 2024-05-21 22:22:53.000000 singletcode-1.1.0/singletCode.egg-info/SOURCES.txt
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)        1 2024-05-21 22:22:53.000000 singletcode-1.1.0/singletCode.egg-info/dependency_links.txt
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)       59 2024-05-21 22:22:53.000000 singletcode-1.1.0/singletCode.egg-info/requires.txt
+-rw-r--r--   0 keerthana  (1000) keerthana  (1000)       12 2024-05-21 22:22:53.000000 singletcode-1.1.0/singletCode.egg-info/top_level.txt
```

### Comparing `singletCode-1.0.0/LICENSE` & `singletcode-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `singletCode-1.0.0/PKG-INFO` & `singletcode-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: singletCode
-Version: 1.0.0
+Version: 1.1.0
 Summary: singletCode is a package to identify true singlets in lineage-barcoded sequencing data.
-Author-email: Ziyang Zhang <ziyang.zhang1@northwestern.edu>
-Maintainer-email: Keerthana M Arun <keerthana.melekotearun@northwestern.edu>
+Author-email: Keerthana M Arun <keerthana.melekotearun@northwestern.edu>, Ziyang Zhang <ziyang.zhang1@northwestern.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023 Goyal Lab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -30,15 +29,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Homepage, https://goyallab.github.io/SingletCodeWebsite/
-Project-URL: Documentation, https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/
+Project-URL: Documentation, https://goyallab.github.io/SingletCodeWebsite/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
@@ -51,32 +50,32 @@
 
 # singletCode 
 
 singletCode is a framework designed to identify true singlets in barcoded sequencing datasets. It utilizes a CSV file containing cell ID, barcode, and sample name to detect singlets within the dataset.
 
 ## Getting Started
 
-For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Features
 
 - **Singlet Identification**: Efficiently identifies true singlets from barcoded sequencing data.
 - **Easy Input**: Works with a simple CSV file format that includes cell ID, barcode, and sample name.
 - **Comprehensive Documentation**: Detailed guides and usage instructions available.
 
 ## Installation
 
-To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Usage
 
-After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Contributing
 
 We welcome contributions to the SingletCode project! If you have suggestions, bug reports, or contributions, please visit our repository's issues section or submit a pull request.
 
 ## License
 
 SingletCode is made available under a standard open-source license. For more details, see the LICENSE file in the repository.
 
-For more information about how singletCode works and using it for your sequencing data, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
+For more information, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
```

### Comparing `singletCode-1.0.0/README.md` & `singletcode-1.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 # singletCode 
 
 singletCode is a framework designed to identify true singlets in barcoded sequencing datasets. It utilizes a CSV file containing cell ID, barcode, and sample name to detect singlets within the dataset.
 
 ## Getting Started
 
-For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Features
 
 - **Singlet Identification**: Efficiently identifies true singlets from barcoded sequencing data.
 - **Easy Input**: Works with a simple CSV file format that includes cell ID, barcode, and sample name.
 - **Comprehensive Documentation**: Detailed guides and usage instructions available.
 
 ## Installation
 
-To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Usage
 
-After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Contributing
 
 We welcome contributions to the SingletCode project! If you have suggestions, bug reports, or contributions, please visit our repository's issues section or submit a pull request.
 
 ## License
 
 SingletCode is made available under a standard open-source license. For more details, see the LICENSE file in the repository.
 
-For more information about how singletCode works and using it for your sequencing data, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
+For more information, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
```

### Comparing `singletCode-1.0.0/pyproject.toml` & `singletcode-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "singletCode"
 dynamic = ["version"]
 requires-python = ">=3.7"
 authors = [
-    { name = "Ziyang Zhang", email = "ziyang.zhang1@northwestern.edu" }
-]
-maintainers = [
     { name = "Keerthana M Arun", email = "keerthana.melekotearun@northwestern.edu" },
+    { name = "Ziyang Zhang", email = "ziyang.zhang1@northwestern.edu" }
 ]
 description = "singletCode is a package to identify true singlets in lineage-barcoded sequencing data."
 readme = "README.md"
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: BSD License",
@@ -28,11 +26,11 @@
     "pandas >= 0.23.4",
     "tqdm >= 4.28.1",
     "matplotlib >= 3.0.2"
 ]
 
 [project.urls]
 "Homepage" = "https://goyallab.github.io/SingletCodeWebsite/"
-"Documentation" = "https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/"
+"Documentation" = "https://goyallab.github.io/SingletCodeWebsite/"
 
 [tool.setuptools.dynamic]
 version = {file = ["__version__"]}
```

### Comparing `singletCode-1.0.0/singletCode/count_doublets_utils_copy.py` & `singletcode-1.1.0/singletCode/count_doublets_utils_copy.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,20 @@
 from itertools import combinations
 import random
 import math
 import matplotlib.pyplot as plt
 from .general_utility_functions import check_input
 random.seed(2022)
 
-def count_doublets(df, output_prefix = None, dataset_name = None, sample_type = "RNA", 
+def count_doublets(df, output_prefix = None, dataset_name = None,
                    save_all_singlet_categories = False, save_plot_umi = False,
                    umi_cutoff_method = "ratio", umi_cutoff_ratio=3 / 4e5, umi_cutoff_percentile = None, min_umi_good_data_cutoff=2,
                    umi_diff_threshold=50, dominant_threshold=10):
     # TODO: write check_input function
     check_input(df, output_path = output_prefix, dataset_name = dataset_name,
-                sample_type = sample_type, 
                 save_all_singlet_categories = save_all_singlet_categories,
                 save_plot_umi = save_plot_umi,
                 umi_cutoff_method = umi_cutoff_method)
     if(output_prefix == None):
         print("Note: None of the output files will be saved since no output path was provided.")
     else:
         output_prefix = os.path.join(output_prefix)
@@ -48,25 +47,16 @@
         cur_sample_df = df[df["sample"] == cur_sample_num]
         total_cells = len(cur_sample_df["cellID"].unique())
         print("Total cells for sample {}: {}".format(cur_sample_num, total_cells))
 
         #Counting nUMI for each barcode, cell ID combination
         cur_freq_df = cur_sample_df.groupby(['cellID', 'barcode', 'sample']).size().reset_index()
         cur_freq_df.columns = ['cellID', "barcode", 'sample', "nUMI"]
-
-
-        # If sample_type is ATAC, we remove all barcodes with greater than 2 UMI
-        if sample_type == "ATAC":
-            print("INFO: the barcodes are from ATACseq data and the UMI cutoff is 2 for all barcodes.")
-            print(cur_sample_num)
-            cur_freq_df = cur_freq_df[cur_freq_df['nUMI'] <= 2].reset_index(drop=True)
-            calculated_umi_cutoff = 1
-            cur_umi_adjusted_cutoff = 1
         
-        elif umi_cutoff_method == "percentile":
+        if umi_cutoff_method == "percentile":
             print("INFO: Using percentile filtering by choosing barcodes whose UMI counts is in top {} percentile".format(umi_cutoff_percentile))
             calculated_umi_cutoff = math.ceil(np.percentile(cur_freq_df["nUMI"], umi_cutoff_percentile))
             cur_umi_adjusted_cutoff = max(calculated_umi_cutoff, min_umi_good_data_cutoff)
         
         elif umi_cutoff_method == "ratio":
             print("INFO: Using ratio based filtering.")
             calculated_umi_cutoff = round(umi_cutoff_ratio * cur_sample_df.shape[0])
```

### Comparing `singletCode-1.0.0/singletCode/general_utility_functions.py` & `singletcode-1.1.0/singletCode/general_utility_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,30 @@
 #Module to define the general utility functions.
 import pandas as pd
 import os
 def check_sample_sheet(data_frame):
-    #Function to check if the dataframe can be used as input to get_singlets function. It checks if the three columns needed are present.
+    '''
+    Function to check if the dataframe can be used as input to get_singlets function. It checks if the three columns - cellID, barcode, sample needed are present and in same order. If this dataframe can be used for get_singlets function, then a statement will be printed to confirm that
+    
+    Args: 
+        sample_sheet: A dataframe that contains your sample sheet.
+    
+    Returns:
+        None
+    '''
     column_names = data_frame.columns
     column_names = column_names.tolist()
     required_columns = ["cellID","barcode", "sample"]
     if column_names != required_columns:
         #Test
         raise ValueError("The column names of the sample sheet must be cellID, barcode and sample, in that order.")
     print("The sample sheet provided can be used as input to get_singlets to get a list of singlets identified.")
     return
 
-def check_input(sample_sheet, output_path = None, dataset_name = None, sample_type = None, 
+def check_input(sample_sheet, output_path = None, dataset_name = None, 
                 save_all_singlet_categories = None, save_plot_umi = None,
                 umi_cutoff_method = None):
                 
 
     if(output_path):
         flag = os.path.exists(output_path)
         if(not flag):
@@ -29,10 +37,10 @@
         raise ValueError("The column names of the sample sheet must be cellID, barcode and sample, in that order.")
     
     #checking if output_prefix is provided if save is true
     if (save_plot_umi or save_all_singlet_categories):
         if(not output_path):
             raise ValueError("The option to save files has been set to true, but no output_path has been provided.")
         
-    if (umi_cutoff_method != "ratio" and umi_cutoff_method != "percentile" and sample_type == "RNA"):
+    if (umi_cutoff_method != "ratio" and umi_cutoff_method != "percentile"):
         raise ValueError("Please choose either ratio or percentile method to determine UMI cutoff for you RNAseq dataset.")
     return
```

### Comparing `singletCode-1.0.0/singletCode/get_singlets.py` & `singletcode-1.1.0/singletCode/get_singlets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,41 +1,61 @@
 #Module which has the the main functions
 from .count_doublets_utils_copy import count_doublets
 
-def get_singlets(sample_sheet, output_path = None, dataset_name = None, sample_type = "RNA",
+def get_singlets(sample_sheet, output_path = None, dataset_name = None,
                 save_all_singlet_categories = False, save_plot_umi = False, 
                 umi_cutoff_method = "ratio", umi_cutoff_ratio = 3/4e5, 
                 umi_cutoff_percentile= None,  min_umi_cutoff =2, umi_diff_threshold = 50,
                 umi_dominant_threshold = 10):
     """
-    Function that inputs the sample sheet and other parameters and runs it through count_doublets to get a list of singlets in the sample.
-    :param: sample_sheet: a dataframe that contains 3 columns: cellID, barcode, sample and if a row is repeated, it is assumed to reflect the UMI associated with a barcode in this cell (identified by the cellID). 
-    :dataset_name: This is the name of the dataset being analysed. It will be in the name of all saved files and be a column in the singlet_stats sheet returned
-    :param: output_path: the path to store any output files, including plots to show UMI distribution and what the umi_cutoff used is, csv files containing singlets of different categories. If None, then the list of singlets will be returned but it won't contain information about what category of singlet each cell is.
-    :param: sample_type: specify if the barcodes are from RNAseq or ATACseq data. If it is from ATACseq data, any barcode with more than 2 UMI will be filtered out since there can be atmost 2 copies of the barcode in the genome and hence, atmost 2 UMI associated with it. Also, please ensure the input_sheet contains UMI information, and not reads.  
-    :param: save_all_singlet_categories: If true, then singlets of each category are saved separately in csv files along with all singlets and all non-singlets - a total of 5 files - at the path inputted in output_prefix
-    :param: save_plot_umi: If true, then plots showing UMI distribution indicating the UMI cutoff used will be saved for each sample in the path inputted in output_prefix.
-    :param: umi_cutoff_method: Specify if quality control for barcodes using UMI counts should be based on "ratio" or "percentile". If it is ratio, then the umi_cutoff will be calculated by multiplying umi_cutoff_ratio (default: 3/4e5) with the total UMI count for sample. If it is percentile, the umi_cutoff_percentile will be used to determine the umi_cutoff.
-    :param: umi_cutoff_ratio: this is the ratio used to determine the umi_cutoff if umi_cutoff_method is "ratio"
-    :param: umi_cutoff_percentile: If umi_cutoff_method is "percentile", then the umi_cutoff will be the minimum UMI count required to be in top umi_cutoff_percentile'th percentile. 
-    :param: min_umi_cutoff: This is the absolute minimum number of UMIs that need to be associated with a barcode for it to be considered a barcode. However, the actual umi_cutoff used will be the greater of min_umi_cutoff and the cutoff calculated using umi_cutoff_method.    
-    :param: umi_dominant_threshold: The minimum UMI count to be associated with a barcode for it to be considered to be a potential dominant barcode in a cell.
-    :param: umi_diff_threshold: This is the minimum difference between UMI counts associated with a potential dominant barcode present within a cell and the median UMI count of all barcodes associated with the cell. If a cell has only one dominant barcode, it will be counted as a singlet.
+    Function that inputs the sample sheet and other parameters and runs it through count_doublets to get a list of 
+    singlets in the sample. If a row is repeated, it is assumed to reflect the UMI associated with a barcode in 
+    this cell (identified by the cellID).
 
+    Args:
+        sample_sheet (DataFrame): A dataframe that contains 3 columns: cellID, barcode, sample.
+        dataset_name (str): The name of the dataset being analysed. It will be in the name of all saved files 
+            and be a column in the singlet_stats sheet returned.
+        output_path (str, optional): The path to store any output files, including plots to show UMI distribution 
+            and what the umi_cutoff used is, csv files containing singlets of different categories. If None, 
+            then the list of singlets will be returned but it won’t contain information about what category of 
+            singlet each cell is. Defaults to None.
+        save_all_singlet_categories (bool, optional): If true, then singlets of each category are saved separately 
+            in csv files along with all singlets and all non-singlets. Defaults to False.
+        save_plot_umi (bool, optional): If true, then plots showing UMI distribution indicating the UMI cutoff used 
+            will be saved for each sample. Defaults to False.
+        umi_cutoff_method (str, optional): Specify if quality control for barcodes using UMI counts should be based 
+            on "ratio" or "percentile". Defaults to 'ratio'.
+        umi_cutoff_ratio (float, optional): The ratio used to determine the umi_cutoff if umi_cutoff_method is 
+            "ratio". Defaults to 3/4e5.
+        umi_cutoff_percentile (float, optional): If umi_cutoff_method is "percentile", then the umi_cutoff will be 
+            the minimum UMI count required to be in the top umi_cutoff_percentile'th percentile. There is no default and if umi_cutoff_method is set to "percentile", then manually set this parameter.
+        min_umi_cutoff (int, optional): This is the absolute minimum number of UMIs that need to be associated with 
+            a barcode for it to be considered a barcode. However, the actual umi_cutoff used will be the greater 
+            of min_umi_cutoff and the cutoff calculated using umi_cutoff_method. Defaults to 2.
+        umi_dominant_threshold (int, optional): The minimum UMI count to be associated with a barcode for it to be 
+            considered to be a potential dominant barcode in a cell. Defaults to 10.
+        umi_diff_threshold (int, optional): This is the minimum difference between UMI counts associated with a 
+            potential dominant barcode present within a cell and the median UMI count of all barcodes associated 
+            with the cell. If a cell has only one dominant barcode, it will be counted. Defaults to 50.
+
+    Returns:
+        tuple: A 2-tuple containing:
+            - pandas.DataFrame: A dataframe which contains all unique cell ID and barcode combinations in the data along with singlet assignment to each cell ID.
+            - pandas.DataFrame: A dataframe which contains the statistics for total singlets, different categories of singlets, and cells removed due to low UMI counts.
     """
     singlet_list, singlet_stats = count_doublets(
             sample_sheet,
             output_prefix=output_path,
             save_all_singlet_categories = save_all_singlet_categories,
             save_plot_umi = save_plot_umi,
             umi_cutoff_ratio=umi_cutoff_ratio,
             umi_cutoff_percentile = umi_cutoff_percentile,
             umi_diff_threshold=umi_diff_threshold,
             dominant_threshold=umi_dominant_threshold,
             min_umi_good_data_cutoff=min_umi_cutoff,
-            sample_type = sample_type, 
             umi_cutoff_method = umi_cutoff_method,
             dataset_name = dataset_name
     )
     
     return singlet_list, singlet_stats
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `singletCode-1.0.0/singletCode.egg-info/PKG-INFO` & `singletcode-1.1.0/singletCode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: singletCode
-Version: 1.0.0
+Version: 1.1.0
 Summary: singletCode is a package to identify true singlets in lineage-barcoded sequencing data.
-Author-email: Ziyang Zhang <ziyang.zhang1@northwestern.edu>
-Maintainer-email: Keerthana M Arun <keerthana.melekotearun@northwestern.edu>
+Author-email: Keerthana M Arun <keerthana.melekotearun@northwestern.edu>, Ziyang Zhang <ziyang.zhang1@northwestern.edu>
 License: BSD 3-Clause License
         
         Copyright (c) 2023 Goyal Lab
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
@@ -30,15 +29,15 @@
         FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
         DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 Project-URL: Homepage, https://goyallab.github.io/SingletCodeWebsite/
-Project-URL: Documentation, https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/
+Project-URL: Documentation, https://goyallab.github.io/SingletCodeWebsite/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Science/Research
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Requires-Python: >=3.7
@@ -51,32 +50,32 @@
 
 # singletCode 
 
 singletCode is a framework designed to identify true singlets in barcoded sequencing datasets. It utilizes a CSV file containing cell ID, barcode, and sample name to detect singlets within the dataset.
 
 ## Getting Started
 
-For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+For detailed instructions on how to use SingletCode, including setup, input file formats, and execution commands, please visit our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Features
 
 - **Singlet Identification**: Efficiently identifies true singlets from barcoded sequencing data.
 - **Easy Input**: Works with a simple CSV file format that includes cell ID, barcode, and sample name.
 - **Comprehensive Documentation**: Detailed guides and usage instructions available.
 
 ## Installation
 
-To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+To install SingletCode, ensure that you have a compatible Python environment. For installation instructions, dependencies, and more, refer to the [SingletCode documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Usage
 
-After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/packageDocumentation/).
+After installation, you can run SingletCode with your dataset by following the detailed usage instructions available in our [documentation](https://goyallab.github.io/SingletCodeWebsite/).
 
 ## Contributing
 
 We welcome contributions to the SingletCode project! If you have suggestions, bug reports, or contributions, please visit our repository's issues section or submit a pull request.
 
 ## License
 
 SingletCode is made available under a standard open-source license. For more details, see the LICENSE file in the repository.
 
-For more information about how singletCode works and using it for your sequencing data, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
+For more information, please visit [SingletCode's homepage](https://goyallab.github.io/SingletCodeWebsite/).
```

