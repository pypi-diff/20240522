# Comparing `tmp/sitesyncro-0.9.5.tar.gz` & `tmp/sitesyncro-0.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sitesyncro-0.9.5.tar", last modified: Thu May 16 12:15:58 2024, max compression
+gzip compressed data, was "sitesyncro-0.9.6.tar", last modified: Wed May 22 13:08:53 2024, max compression
```

## Comparing `sitesyncro-0.9.5.tar` & `sitesyncro-0.9.6.tar`

### file list

```diff
@@ -1,35 +1,45 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.449489 sitesyncro-0.9.5/
--rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.5/LICENSE
--rw-rw-rw-   0        0        0    11779 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/PKG-INFO
--rw-rw-rw-   0        0        0    10770 2024-05-15 15:34:33.000000 sitesyncro-0.9.5/README.md
--rw-rw-rw-   0        0        0       42 2024-05-16 12:15:58.449489 sitesyncro-0.9.5/setup.cfg
--rw-rw-rw-   0        0        0     1968 2024-05-15 06:17:47.000000 sitesyncro-0.9.5/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.396111 sitesyncro-0.9.5/src/
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.411747 sitesyncro-0.9.5/src/sitesyncro/
--rw-rw-rw-   0        0        0    38904 2024-05-16 11:41:57.000000 sitesyncro-0.9.5/src/sitesyncro/Model.py
--rw-rw-rw-   0        0        0    19732 2024-05-15 14:36:11.000000 sitesyncro-0.9.5/src/sitesyncro/Sample.py
--rw-rw-rw-   0        0        0      202 2024-05-15 08:39:18.000000 sitesyncro-0.9.5/src/sitesyncro/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.427354 sitesyncro-0.9.5/src/sitesyncro/mhelpers/
--rw-rw-rw-   0        0        0    11338 2024-05-16 11:07:38.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MCluster.py
--rw-rw-rw-   0        0        0     1808 2024-05-16 09:19:33.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MOxCal.py
--rw-rw-rw-   0        0        0    12885 2024-05-16 11:02:34.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPhasing.py
--rw-rw-rw-   0        0        0     6286 2024-05-16 10:24:18.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPlot.py
--rw-rw-rw-   0        0        0     3909 2024-05-16 09:31:19.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/MRandomization.py
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.5/src/sitesyncro/mhelpers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/src/sitesyncro/utils/
--rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.5/src/sitesyncro/utils/__init__.py
--rw-rw-rw-   0        0        0     5766 2024-05-16 10:31:01.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_cluster.py
--rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_data.py
--rw-rw-rw-   0        0        0     8268 2024-05-16 10:50:52.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_load.py
--rw-rw-rw-   0        0        0     3689 2024-05-04 21:29:14.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_mp.py
--rw-rw-rw-   0        0        0     9981 2024-05-16 09:14:45.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_oxcal.py
--rw-rw-rw-   0        0        0     5593 2024-05-16 10:35:51.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_phase.py
--rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_radiocarbon.py
--rw-rw-rw-   0        0        0     5107 2024-05-16 09:27:30.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_simulate.py
--rw-rw-rw-   0        0        0     7720 2024-05-04 12:22:34.000000 sitesyncro-0.9.5/src/sitesyncro/utils/fnc_stat.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:15:58.433860 sitesyncro-0.9.5/src/sitesyncro.egg-info/
--rw-rw-rw-   0        0        0    11779 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      852 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      176 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 12:15:58.000000 sitesyncro-0.9.5/src/sitesyncro.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.496835 sitesyncro-0.9.6/
+-rw-rw-rw-   0        0        0    35821 2022-11-10 14:20:31.000000 sitesyncro-0.9.6/LICENSE
+-rw-rw-rw-   0        0        0    12788 2024-05-22 13:08:53.495837 sitesyncro-0.9.6/PKG-INFO
+-rw-rw-rw-   0        0        0    11779 2024-05-22 12:56:46.000000 sitesyncro-0.9.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 13:08:53.496835 sitesyncro-0.9.6/setup.cfg
+-rw-rw-rw-   0        0        0     1968 2024-05-15 06:17:47.000000 sitesyncro-0.9.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.430932 sitesyncro-0.9.6/src/
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.450010 sitesyncro-0.9.6/src/sitesyncro/
+-rw-rw-rw-   0        0        0    39647 2024-05-22 12:30:42.000000 sitesyncro-0.9.6/src/sitesyncro/Model.py
+-rw-rw-rw-   0        0        0     3798 2024-05-22 12:13:46.000000 sitesyncro-0.9.6/src/sitesyncro/Phase.py
+-rw-rw-rw-   0        0        0    19732 2024-05-15 14:36:11.000000 sitesyncro-0.9.6/src/sitesyncro/Sample.py
+-rw-rw-rw-   0        0        0      202 2024-05-22 13:06:33.000000 sitesyncro-0.9.6/src/sitesyncro/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.460486 sitesyncro-0.9.6/src/sitesyncro/graphviz/
+-rw-rw-rw-   0        0        0        0 2024-02-29 11:43:21.000000 sitesyncro-0.9.6/src/sitesyncro/graphviz/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.468769 sitesyncro-0.9.6/src/sitesyncro/mhelpers/
+-rw-rw-rw-   0        0        0    10872 2024-05-21 13:50:42.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/MCluster.py
+-rw-rw-rw-   0        0        0     1808 2024-05-16 09:19:33.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/MOxCal.py
+-rw-rw-rw-   0        0        0    13302 2024-05-21 18:13:26.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/MPhasing.py
+-rw-rw-rw-   0        0        0     7369 2024-05-22 12:39:54.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/MPlot.py
+-rw-rw-rw-   0        0        0     3909 2024-05-16 09:31:19.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/MRandomization.py
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.6/src/sitesyncro/mhelpers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.475981 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/
+-rw-rw-rw-   0        0        0      946 2024-05-16 19:16:50.000000 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/__init__.py
+-rw-rw-rw-   0        0        0    72363 2024-05-16 19:17:17.000000 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/agraph.py
+-rw-rw-rw-   0        0        0     7202 2024-02-29 11:43:21.000000 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/graphviz.py
+-rw-rw-rw-   0        0        0     2861 2024-02-29 11:43:21.000000 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/scraper.py
+-rw-rw-rw-   0        0        0      609 2024-02-29 11:43:21.000000 sitesyncro-0.9.6/src/sitesyncro/pygraphviz/testing.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.492643 sitesyncro-0.9.6/src/sitesyncro/utils/
+-rw-rw-rw-   0        0        0        0 2024-03-20 16:40:04.000000 sitesyncro-0.9.6/src/sitesyncro/utils/__init__.py
+-rw-rw-rw-   0        0        0     5505 2024-05-21 13:39:26.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_cluster.py
+-rw-rw-rw-   0        0        0     2425 2024-05-02 14:21:12.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_data.py
+-rw-rw-rw-   0        0        0     8268 2024-05-16 10:50:52.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_load.py
+-rw-rw-rw-   0        0        0     5926 2024-05-20 15:59:11.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_mp.py
+-rw-rw-rw-   0        0        0     9981 2024-05-16 09:14:45.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_oxcal.py
+-rw-rw-rw-   0        0        0    10329 2024-05-21 09:33:44.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_phase.py
+-rw-rw-rw-   0        0        0     2572 2024-05-02 14:41:27.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_radiocarbon.py
+-rw-rw-rw-   0        0        0     5107 2024-05-16 09:27:30.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_simulate.py
+-rw-rw-rw-   0        0        0     7720 2024-05-04 12:22:34.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_stat.py
+-rw-rw-rw-   0        0        0     1633 2024-05-21 09:02:33.000000 sitesyncro-0.9.6/src/sitesyncro/utils/fnc_visualize.py
+drwxrwxrwx   0        0        0        0 2024-05-22 13:08:53.493737 sitesyncro-0.9.6/src/sitesyncro.egg-info/
+-rw-rw-rw-   0        0        0    12788 2024-05-22 13:08:53.000000 sitesyncro-0.9.6/src/sitesyncro.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1136 2024-05-22 13:08:53.000000 sitesyncro-0.9.6/src/sitesyncro.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 13:08:53.000000 sitesyncro-0.9.6/src/sitesyncro.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      176 2024-05-22 13:08:53.000000 sitesyncro-0.9.6/src/sitesyncro.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 13:08:53.000000 sitesyncro-0.9.6/src/sitesyncro.egg-info/top_level.txt
```

### Comparing `sitesyncro-0.9.5/LICENSE` & `sitesyncro-0.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/PKG-INFO` & `sitesyncro-0.9.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-Metadata-Version: 2.1
-Name: sitesyncro
-Version: 0.9.5
-Summary: SiteSyncro - Site-specific chronological modeling and synchronization
-Home-page: https://github.com/demjanp/SiteSyncro
-Author: Peter Demjan
-Author-email: peter.demjan@gmail.com
-Keywords: archaeology,radiocarbon,chronology,stratigraphy
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
-Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.10, <3.11
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: numpy<2,>=1.26.4
-Requires-Dist: scipy<2,>=1.13.0
-Requires-Dist: matplotlib<4,>=3.8.4
-Requires-Dist: scikit-learn<2,>=1.4.2
-Requires-Dist: tqdm<5,>=4.66.0
-Requires-Dist: requests<3,>=2.31.0
-Requires-Dist: networkx<4,>=2.8.0
-Requires-Dist: sphinx<7.4,>=7.3.7
-Requires-Dist: myst-parser<3.1,>=3.0.1
-
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
 Project homepage: [https://github.com/demjanp/SiteSyncro](https://github.com/demjanp/SiteSyncro)
 
@@ -37,14 +11,15 @@
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
    * [Sample Class](#sample_class)
+   * [Phase Class](#phase_class)
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
@@ -85,20 +60,20 @@
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
 - `-h`, `--help`: Show help message and exit.
-- `-directory`: Working directory for model data (default is "model").
+- `-directory`: Working directory for model data (default is 'model').
 - `-input`: The path to the input file in semicolon-separated CSV format.
-- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is 'intcal20.14c').
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is 'sequence').
 - `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
-- `-min_years_per_cluster`: Minimum number of years per cluster. (default is 25).
+- `-cluster_selection`: Cluster selection method ('silhouette' or 'mcst'; default is 'silhouette').
 - `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-by_dates`: Flag indicating whether to update the phasing by comparing sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
 - `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
@@ -147,24 +122,26 @@
     
     # Plot the randomization test result
     model.plot_randomized()
     
     # Plot the clustering result
     model.plot_clusters()
     
-    # Save the results to a CSV file
-    model.save_csv()
+    # Save the results to a CSV files
+    model.save_csv_samples()
+    model.save_csv_phases()
 ```
 This will create the default directory `model` and generate the following files:
 `model.json.gz`
 `model.oxcal`
 `model.js`, `model.log`, `model.txt`
 `randomized.pdf`
 `silhouette.pdf`
-`results.csv`
+`results_samples.csv`
+`results_phases.csv`
 
 See [Model Class](https://sitesyncro.readthedocs.io/en/latest/model.html) documentation for more information.
 
 ### Sample Class <a name="sample_class"></a>
 The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
 
 ```python
@@ -177,14 +154,37 @@
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
+### Phase Class <a name="phase_class"></a>
+The `Phase` class represents a modeled chronological phase. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+    
+    # Initialize the Model object and load data from the directory 'model'
+    model = Model(directory='model')
+    
+    # Print information on phasing (if model has been processed)
+    for group, phase in model.phases:
+        phase = model.phases[(group, phase)]
+        start_from, start_to = phase.start_range
+        end_from, end_to = phase.end_range
+        
+        # Print the group, phase, and start and end ranges
+        print(f'Group: {group}, Phase: {phase}, Start: {start_from}-{start_to}, End: {end_from}-{end_to}')
+```
+
+See [Phase Class](https://sitesyncro.readthedocs.io/en/latest/phase.html) documentation for more information.
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
@@ -240,8 +240,8 @@
 * [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
 * [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
```

### Comparing `sitesyncro-0.9.5/README.md` & `sitesyncro-0.9.6/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,33 @@
+Metadata-Version: 2.1
+Name: sitesyncro
+Version: 0.9.6
+Summary: SiteSyncro - Site-specific chronological modeling and synchronization
+Home-page: https://github.com/demjanp/SiteSyncro
+Author: Peter Demjan
+Author-email: peter.demjan@gmail.com
+Keywords: archaeology,radiocarbon,chronology,stratigraphy
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python :: 3.10
+Requires-Python: >=3.10, <3.11
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: numpy<2,>=1.26.4
+Requires-Dist: scipy<2,>=1.13.0
+Requires-Dist: matplotlib<4,>=3.8.4
+Requires-Dist: scikit-learn<2,>=1.4.2
+Requires-Dist: tqdm<5,>=4.66.0
+Requires-Dist: requests<3,>=2.31.0
+Requires-Dist: networkx<4,>=2.8.0
+Requires-Dist: sphinx<7.4,>=7.3.7
+Requires-Dist: myst-parser<3.1,>=3.0.1
+
 # SiteSyncro
 Site-specific chronological modeling and synchronization
 
 Created on 10.4.2024
 
 Project homepage: [https://github.com/demjanp/SiteSyncro](https://github.com/demjanp/SiteSyncro)
 
@@ -11,14 +37,15 @@
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
    * [Sample Class](#sample_class)
+   * [Phase Class](#phase_class)
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
@@ -59,20 +86,20 @@
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
 - `-h`, `--help`: Show help message and exit.
-- `-directory`: Working directory for model data (default is "model").
+- `-directory`: Working directory for model data (default is 'model').
 - `-input`: The path to the input file in semicolon-separated CSV format.
-- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is 'intcal20.14c').
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is 'sequence').
 - `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
-- `-min_years_per_cluster`: Minimum number of years per cluster. (default is 25).
+- `-cluster_selection`: Cluster selection method ('silhouette' or 'mcst'; default is 'silhouette').
 - `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-by_dates`: Flag indicating whether to update the phasing by comparing sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
 - `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
@@ -121,24 +148,26 @@
     
     # Plot the randomization test result
     model.plot_randomized()
     
     # Plot the clustering result
     model.plot_clusters()
     
-    # Save the results to a CSV file
-    model.save_csv()
+    # Save the results to a CSV files
+    model.save_csv_samples()
+    model.save_csv_phases()
 ```
 This will create the default directory `model` and generate the following files:
 `model.json.gz`
 `model.oxcal`
 `model.js`, `model.log`, `model.txt`
 `randomized.pdf`
 `silhouette.pdf`
-`results.csv`
+`results_samples.csv`
+`results_phases.csv`
 
 See [Model Class](https://sitesyncro.readthedocs.io/en/latest/model.html) documentation for more information.
 
 ### Sample Class <a name="sample_class"></a>
 The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
 
 ```python
@@ -151,14 +180,37 @@
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
+### Phase Class <a name="phase_class"></a>
+The `Phase` class represents a modeled chronological phase. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+    
+    # Initialize the Model object and load data from the directory 'model'
+    model = Model(directory='model')
+    
+    # Print information on phasing (if model has been processed)
+    for group, phase in model.phases:
+        phase = model.phases[(group, phase)]
+        start_from, start_to = phase.start_range
+        end_from, end_to = phase.end_range
+        
+        # Print the group, phase, and start and end ranges
+        print(f'Group: {group}, Phase: {phase}, Start: {start_from}-{start_to}, End: {end_from}-{end_to}')
+```
+
+See [Phase Class](https://sitesyncro.readthedocs.io/en/latest/phase.html) documentation for more information.
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
@@ -214,8 +266,8 @@
 * [Requests](https://requests.readthedocs.io/)
 * [Scikit-learn](https://scikit-learn.org/)
 * [SciPy](https://scipy.org/)
 * [tqdm](https://tqdm.github.io/)
 
 ## License <a name="license"></a>
 
-This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
+This code is licensed under the [GNU GENERAL PUBLIC LICENSE](https://www.gnu.org/licenses/gpl-3.0.en.html) - see the [LICENSE](https://github.com/demjanp/SiteSyncro/blob/main/LICENSE) file for details
```

### Comparing `sitesyncro-0.9.5/setup.py` & `sitesyncro-0.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/Model.py` & `sitesyncro-0.9.6/src/sitesyncro/Model.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import subprocess
 from collections import defaultdict
 from typing import List, Dict, Any
 
 import numpy as np
 
 from sitesyncro.Sample import Sample
+from sitesyncro.Phase import Phase
 
 from sitesyncro.mhelpers.MPhasing import MPhasing
 from sitesyncro.mhelpers.MOxCal import MOxCal
 from sitesyncro.mhelpers.MRandomization import MRandomization
 from sitesyncro.mhelpers.MCluster import MCluster
 from sitesyncro.mhelpers.MPlot import MPlot
 
@@ -40,17 +41,14 @@
 
 	:param cluster_n: Number of clusters to form (-1 = automatic; default is -1).
 	:type cluster_n: int
 	
 	:param cluster_selection: The method used to select the optimal number of clusters. Can be 'silhouette' or 'mcst' (default is 'silhouette').
 	:type cluster_selection: str
 	
-	:param min_years_per_cluster: The minimum number of years per cluster.
-	:type min_years_per_cluster: int
-
 	:param uniform: Flag indicating whether to use uniform randomization (default is False).
 	:type uniform: bool
 
 	:param p_value: The P-value for statistical tests (default is 0.05).
 	:type p_value: float
 
 	:param uncertainty_base: The base uncertainty for randomization (default is 15).
@@ -74,15 +72,14 @@
 		defaults = dict(
 			directory='model',
 			samples=[],
 			curve_name='intcal20.14c',
 			phase_model='sequence',
 			cluster_n=-1,
 			cluster_selection='silhouette',
-			min_years_per_cluster=25,
 			uniform=False,
 			p_value=0.05,
 			uncertainty_base=15,
 			npass=100,
 			convergence=0.99,
 			oxcal_url='https://c14.arch.ox.ac.uk/OxCalDistribution.zip',
 			overwrite=False,
@@ -103,14 +100,20 @@
 		
 		if kwargs.get('phase_model', 'sequence') not in ['sequence', 'contiguous', 'overlapping', 'none']:
 			raise Exception("Invalid phase model specified")
 		
 		if not download_oxcal(url=kwargs.get('oxcal_url', defaults['oxcal_url'])):
 			raise Exception("OxCal not found")
 		
+		self.mphasing = MPhasing(self)
+		self.moxcal = MOxCal(self)
+		self.mrandomization = MRandomization(self)
+		self.mcluster = MCluster(self)
+		self.mplot = MPlot(self)
+		
 		self._data = self._assigned()
 		self._data.update(self._calculated())
 		
 		# Attempt to load data from directory
 		if ('directory' in kwargs) and (not overwrite) and ('samples' not in kwargs):
 			if self.load(kwargs['directory']):
 				del kwargs['directory']
@@ -124,29 +127,22 @@
 		kwargs['samples'] = dict([(sample.name, sample) for sample in kwargs['samples']])
 		
 		self._data.update(kwargs)
 		
 		# Create model directory if needed
 		self._data['directory'] = self._create_dir(self.directory, overwrite)
 		
-		self._mphasing = MPhasing(self)
-		self._moxcal = MOxCal(self)
-		self._mrandomization = MRandomization(self)
-		self._mcluster = MCluster(self)
-		self._mplot = MPlot(self)
-	
 	def _assigned(self) -> Dict[str, Any]:
 		return dict(
 			directory=None,
 			samples=None,
 			curve_name=None,
 			phase_model=None,
 			cluster_n=None,
 			cluster_selection=None,
-			min_years_per_cluster=None,
 			uniform=None,
 			p_value=None,
 			uncertainty_base=None,
 			npass=None,
 			convergence=None,
 			oxcal_url=None,
 		)
@@ -155,14 +151,16 @@
 		return dict(
 			years=None,
 			curve=None,
 			oxcal_data=None,
 			
 			outlier_candidates=None,
 			
+			phases=None,
+			
 			summed=None,
 			random_p=None,
 			random_lower=None,
 			random_upper=None,
 			
 			clusters=None,
 			cluster_means=None,
@@ -197,14 +195,25 @@
 					pass
 		if n is not None:
 			n += 1
 			directory = os.path.join(parent_dir, os.path.basename(directory) + "_" + str(n))
 		os.makedirs(directory)
 		return directory
 	
+	def _populate_phases(self):
+		keys = set()
+		for name in self.samples:
+			keys.add((self.samples[name].group, self.samples[name].phase))
+		self._data['phases'] = {}
+		for key in keys:
+			group, phase = key
+			phase = Phase(group, phase)
+			if phase.populate(self):
+				self._data['phases'][key] = phase
+	
 	# Assigned properties
 	
 	@property
 	def directory(self) -> str:
 		"""
 		The directory where the model data is stored.
 		
@@ -262,24 +271,14 @@
 		
 		:return: The method used to select the optimal number of clusters. Can be 'silhouette' or 'mcst'.
 		:rtype: str
 		"""
 		return self._data['cluster_selection']
 	
 	@property
-	def min_years_per_cluster(self) -> int:
-		"""
-		The minimum number of years per cluster.
-		
-		:return: The minimum number of years per cluster.
-		:rtype: int
-		"""
-		return self._data['min_years_per_cluster']
-	
-	@property
 	def uniform(self) -> bool:
 		"""
 		Flag indicating whether the model tests for a uniform distribution of the calendar ages.
 
 		:return: True if a uniform distribution is used, False otherwise.
 		:rtype: bool
 		"""
@@ -508,14 +507,24 @@
 		
 		groups = defaultdict(list)
 		for name in self.samples:
 			groups[self.samples[name].group].append(name)
 		return dict(groups)
 	
 	@property
+	def phases(self) -> List[Phase]:
+		"""
+		:return: A dictionary where the keys are (group, phase) and the values are Phase objects.
+		:rtype: Dict[tuple, Phase]
+		"""
+		if self._data['phases'] is None:
+			self._populate_phases()
+		return self._data['phases']
+	
+	@property
 	def clusters(self) -> Dict[int, Dict[int, List[str]]]:
 		"""
 		Clusters of samples based on the similarity of their probability distributions.
 
 		:return: {clusters_n: [cluster: [sample name, ...], ...}, ...}; clusters_n = number of clusters
 		:rtype: Dict[int, Dict[int, List[str]]]
 		"""
@@ -688,15 +697,17 @@
 		
 		:param zipped: If True, the model is saved as a zipped JSON file. Defaults to False.
 		:type zipped: bool
 		:return: None
 		"""
 		
 		fname = os.path.join(self.directory, 'model.json.gz' if zipped else 'model.json')
-		data = dict_np_to_list(copy.deepcopy(self._data))
+		data = copy.deepcopy(self._data)
+		data['phases'] = None
+		data = dict_np_to_list(data)
 		for name in self.samples:
 			data['samples'][name] = self.samples[name].to_dict()
 		
 		if zipped:
 			with gzip.open(fname, 'wt') as file:
 				json.dump(data, file)
 		else:
@@ -720,15 +731,14 @@
 		model = Model(
 			directory = directory,
 			samples = [self.samples[name].copy() for name in self.samples],
 			curve_name = self.curve_name,
 			phase_model = self.phase_model,
 			cluster_n = self.cluster_n,
 			cluster_selection = self.cluster_selection,
-			min_years_per_cluster = self.min_years_per_cluster,
 			uniform = self.uniform,
 			p_value = self.p_value,
 			uncertainty_base = self.uncertainty_base,
 			npass = self.npass,
 			convergence = self.convergence,
 			oxcal_url = self.oxcal_url
 		)
@@ -848,15 +858,15 @@
 			print("\nNo randomization data to plot")
 			return None
 		
 		# Determine the file path for the plot
 		if fname is None:
 			fname = os.path.join(self.directory, "randomized.pdf")
 		
-		self._mplot.plot_randomized(fname, show)
+		self.mplot.plot_randomized(fname, show)
 		return fname
 	
 	def plot_clusters(self, fname: str = None, show: bool = False) -> str:
 		"""
 		Plots the clustering results.
 
 		The plot can either be saved to a file or displayed.
@@ -874,38 +884,60 @@
 			return None
 		
 		# Determine the file path for the plot
 		if fname is None:
 			fname = os.path.join(self.directory, "silhouette.pdf")
 		
 		# Plot the clustering data
-		self._mplot.plot_clusters(fname, show)
+		self.mplot.plot_clusters(fname, show)
 		return fname
 	
-	def save_csv(self, fcsv: str = None) -> str:
+	def save_csv_samples(self, fcsv: str = None) -> str:
 		"""
-		Saves the results to a CSV file.
+		Saves the results for samples to a CSV file.
 
 		:param fcsv: The file path for the CSV file. If None, a default file name and path are used. Defaults to None.
 		:type fcsv: str, optional
 		:return: The file path the results were saved to.
 		:rtype: str
 		"""
 		
 		# Check if there are any results
 		if not self.has_data:
 			print("\nNo data available")
 			return None
 		
 		# Determine the file path for the CSV file
 		if fcsv is None:
-			fcsv = os.path.join(self.directory, "results.csv")
+			fcsv = os.path.join(self.directory, "results_samples.csv")
+		
+		# Save the results to the CSV file
+		self.mplot.save_results_samples_csv(fcsv)
+		return fcsv
+	
+	def save_csv_phases(self, fcsv: str = None) -> str:
+		"""
+		Saves the results for phases to a CSV file.
+
+		:param fcsv: The file path for the CSV file. If None, a default file name and path are used. Defaults to None.
+		:type fcsv: str, optional
+		:return: The file path the results were saved to.
+		:rtype: str
+		"""
+		# Check if there are any results
+		if not self.is_modeled:
+			print("\nNo data available")
+			return None
+		
+		# Determine the file path for the CSV file
+		if fcsv is None:
+			fcsv = os.path.join(self.directory, "results_phases.csv")
 		
 		# Save the results to the CSV file
-		self._mplot.save_results_csv(fcsv)
+		self.mplot.save_results_phases_csv(fcsv)
 		return fcsv
 	
 	def save_outliers(self, fname: str = None) -> str:
 		"""
 		Saves a list of outliers to a text file.
 
 		:param fname: The file name to save the outliers to. If None, a default file name is used. Defaults to None.
@@ -913,15 +945,15 @@
 		:return: The file name the outliers were saved to.
 		:rtype: str
 		"""
 		
 		if fname is None:
 			fname = os.path.join(self.directory, "outliers.txt")
 		
-		self._mplot.save_outliers(fname)
+		self.mplot.save_outliers(fname)
 		return fname
 	
 	def to_oxcal(self, fname: str = None) -> str:
 		"""
 		Exports the model to an OxCal file.
 
 		Generates an OxCal file from the current model. The OxCal file can be used for further analysis in the OxCal software.
@@ -937,15 +969,15 @@
 		if not self.has_data:
 			print("\nNo data available")
 			return None
 		
 		if fname is None:
 			fname = os.path.join(self.directory, "model.oxcal")
 		
-		txt = self._moxcal.gen_oxcal_model()
+		txt = self.moxcal.gen_oxcal_model()
 		with open(fname, "w", encoding="utf-8") as file:
 			file.write(txt)
 		return fname
 	
 	def load_oxcal_data(self) -> None:
 		"""
 		Loads the OxCal data associated with the model.
@@ -1000,15 +1032,15 @@
 			reset_assigned: {parameter: [old value, new value], ...}; parameters and their values that have been updated;
 			reset_calculated: {attribute, ...}; calculated attributes that have been reset
 		:rtype: (Dict[str, List], set)
 		"""
 		
 		assigned_full = ['samples', 'curve_name', 'phase_model']
 		assigned_randomization = ['uniform', 'p_value', 'uncertainty_base', 'npass', 'convergence']
-		assigned_clustering = ['cluster_n', 'cluster_selection', 'min_years_per_cluster']
+		assigned_clustering = ['cluster_n', 'cluster_selection']
 		
 		def _get_n_samples(value):
 			if isinstance(value, dict):
 				return len(value)
 			return 0
 		
 		reset_assigned = {}
@@ -1076,28 +1108,28 @@
 		:type by_clusters: bool, optional
 		:param by_dates: If True, update the phasing by comparing sample dates. Defaults to False.
 		:type by_dates: bool, optional
 		:return: True if phasing has changed, False otherwise.
 		:rtype: bool
 		"""
 		
-		return self._mphasing.process(by_clusters, by_dates)
+		return self.mphasing.process(by_clusters, by_dates)
 	
 	def process_outliers(self) -> None:
 		"""
 		Identifies and marks dating outliers among the samples in the model.
 
 		Finds dating outliers among the samples which need to be removed for the model to be valid.
 		The outliers are identified based on conflicts between their dating ranges and stratigraphic relationships with other samples.
 		The identified outliers can be retrieved via the attributes Model.outliers and Model.outlier_candidates.
 
 		:return: None
 		"""
 		
-		outliers, self._data['outlier_candidates'] = self._mphasing.find_dating_outliers()
+		outliers, self._data['outlier_candidates'] = self.mphasing.find_dating_outliers()
 		for name in outliers:
 			self.samples[name].set_outlier(True)
 	
 	def process_dates(self) -> None:
 		"""
 		Calculates the posterior probabilities of sample dates based on phasing using Bayesian modeling in OxCal.
 
@@ -1128,15 +1160,15 @@
 		:type max_cpus: int, optional
 		:param max_queue_size: Maximum queue size for parallel processing. If -1, the queue size is unlimited. Defaults to -1.
 		:type max_queue_size: int, optional
 		:return: None
 		"""
 		
 		self._data['summed'], self._data['random_lower'], self._data['random_upper'], self._data[
-			'random_p'] = self._mrandomization.test_distributions(max_cpus=max_cpus, max_queue_size=max_queue_size)
+			'random_p'] = self.mrandomization.test_distributions(max_cpus=max_cpus, max_queue_size=max_queue_size)
 	
 	def process_clustering(self, max_cpus=-1, max_queue_size=-1) -> None:
 		"""
 		Performs clustering on the sample dates.
 
 		Clusters the sample dates and uses randomization testing to find the optimal clustering solution.
 		
@@ -1144,21 +1176,19 @@
 		:type max_cpus: int, optional
 		:param max_queue_size: Maximum queue size for parallel processing. If -1, the queue size is unlimited. Defaults to -1.
 		:type max_queue_size: int, optional
 		:return: None
 		"""
 		
 		self._data['clusters'], self._data['cluster_means'], self._data['cluster_sils'], self._data['cluster_ps'], \
-			self._data['cluster_opt_n'] = self._mcluster.process(max_cpus=max_cpus, max_queue_size=max_queue_size)
+			self._data['cluster_opt_n'] = self.mcluster.process(max_cpus=max_cpus, max_queue_size=max_queue_size)
 	
-	def process(self, by_clusters: bool = False, by_dates: bool = False, max_cpus: int = -1, max_queue_size: int = -1,
+	def process(self, by_clusters: bool = False, by_dates: bool = False, 
+				max_cpus: int = -1, max_queue_size: int = -1, 
 				save: bool = False) -> None:
-		# Process the complete model
-		# by_clusters: if True, update the phasing by clustering sample dates
-		# by_dates: if True, update the phasing by comparing sample dates
 		"""
 		Processes the complete model.
 
 		Performs the following steps:
 		1. Modeling stratigraphy to determine phasing
 		2. Finding outliers
 		3. Bayesian modeling of C-14 dates
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro/Sample.py` & `sitesyncro-0.9.6/src/sitesyncro/Sample.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MCluster.py` & `sitesyncro-0.9.6/src/sitesyncro/mhelpers/MCluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,33 +61,19 @@
 		distributions_n = len(samples)
 		
 		if distributions_n < 3:
 			raise Exception("Insufficient number samples for testing of clustering.")
 		
 		t_mean, t_std = get_params(distributions, self.model.curve, self.model.uniform)
 		
-		# Get dating range of all samples
-		rng_min, rng_max = np.inf, -np.inf
-		for name in self.model.samples:
-			rng = self.model.samples[name].get_range()
-			if None in rng:
-				continue
-			rng_min = min(rng_min, min(rng))
-			rng_max = max(rng_max, max(rng))
-		rng = (rng_max - rng_min)
-		if abs(rng) == np.inf:
-			raise Exception("Invalid dating range")
-		
-		clu_max = min(max(2, int(round(rng / self.model.min_years_per_cluster))), distributions_n - 1)
-		
 		clusters = {}  # {cluster_n: {label: [idx, ...], ...}, ...}; idx = index in samples
 		sils = {}  # {cluster_n: silhouette_score, ...}
 		means = {}  # {cluster_n: {label: mean, ...}, ...}
 		D = calc_distance_matrix(distributions)
-		for cluster_n in range(2, clu_max + 1):
+		for cluster_n in range(2, distributions_n):
 			clusters[cluster_n] = calc_clusters_hca(D, cluster_n)
 			sils[cluster_n] = calc_silhouette(D, clusters[cluster_n])
 			means[cluster_n] = {}
 			for label in clusters[cluster_n]:
 				means[cluster_n][label] = np.average(
 					self.model.years,
 					weights=calc_sum([distributions[idx] for idx in clusters[cluster_n][label]])
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MOxCal.py` & `sitesyncro-0.9.6/src/sitesyncro/mhelpers/MOxCal.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPhasing.py` & `sitesyncro-0.9.6/src/sitesyncro/mhelpers/MPhasing.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,17 +3,17 @@
 from typing import List, Dict
 
 import matplotlib.pyplot as plt
 import networkx as nx
 import numpy as np
 from tqdm import tqdm
 
-from sitesyncro.utils.fnc_stat import (samples_to_distributions)
+from sitesyncro.utils.fnc_stat import (samples_to_distributions, calc_range)
 from sitesyncro.utils.fnc_phase import (check_circular_relationships, visualize_earlier_than, extend_earlier_than,
-                                        eap_to_int, get_groups_and_phases, prob_earlier_than)
+                                        eap_to_int, get_groups_and_phases)
 
 class MPhasing(object):
 	"""
 	A class implementing phasing functionality
 	
 	:param model: The parent Model object
 	:type model: Model
@@ -85,18 +85,15 @@
 					continue
 				if self.model.samples[s1].group != self.model.samples[s2].group:
 					continue
 				if self.model.samples[s1].phase < self.model.samples[s2].phase:
 					earlier_than[i][j] = True
 		
 		# Check if earlier_than has circular relationships
-		if not check_circular_relationships(earlier_than, samples):
-			# Visualize earlier_than as a DAG
-			visualize_earlier_than(earlier_than, samples)
-			raise Exception("Circular relationships detected")
+		check_circular_relationships(earlier_than, samples)
 		
 		# Extend the earlier_than matrix to include computed relations
 		earlier_than = extend_earlier_than(earlier_than)
 		# earlier_than: matrix[n_samples x n_samples] = [True/False, ...]; sample in row is earlier than sample in column based on stratigraphy
 		return earlier_than, samples
 	
 	def update_earlier_than_by_dating(self, earlier_than: np.ndarray, samples: List[str]) -> np.ndarray:
@@ -109,14 +106,15 @@
 		earlier_than: matrix[n_samples x n_samples] = [True/False, ...]; sample in row is earlier than sample in column based on stratigraphy
 		samples: The list of sample names.
 
 		Returns:
 		np.ndarray: The updated "earlier than" matrix.
 		"""
 		
+		earlier_than = earlier_than.copy()
 		distributions, names_dist, joined = samples_to_distributions(self.model.samples.values())
 		
 		# distributions = [[p, ...], ...]
 		# names_dist = [combined_name, ...] ordered by distributions
 		# joined = {combined_name: [sample name, ...], ...}
 		
 		def _get_combined(name, joined):
@@ -131,26 +129,30 @@
 			if name in names_dist:
 				idx_lookup[name] = names_dist.index(name)
 			else:
 				combined_name = _get_combined(name, joined)
 				if combined_name is not None:
 					idx_lookup[name] = names_dist.index(combined_name)
 		
+		ranges = {}
+		for i in range(len(distributions)):
+			ranges[i] = calc_range(self.model.years, distributions[i])
+		
 		# Update earlier_than based on probability distributions
 		for i, s1 in enumerate(samples):
 			d_i = idx_lookup[s1]
 			if d_i is None:
 				continue
 			for j, s2 in enumerate(samples):
 				if i == j:
 					continue
 				d_j = idx_lookup[s2]
 				if d_j is None:
 					continue
-				if prob_earlier_than(distributions[d_i], distributions[d_j]) >= (1 - self.model.p_value):
+				if ranges[d_i][1] > ranges[d_j][0]:
 					earlier_than[i][j] = True
 		
 		# Extend the earlier_than matrix to include computed relations
 		earlier_than = extend_earlier_than(earlier_than)
 		
 		return earlier_than
 	
@@ -168,55 +170,62 @@
 		np.ndarray: The updated "earlier than" matrix.
 		"""
 		# Update earlier_than based on temporal clustering of the samples
 		
 		if self.model.cluster_opt_n is None:
 			raise Exception("No clustering found")
 		
+		earlier_than = earlier_than.copy()
 		clusters = self.model.clusters[self.model.cluster_opt_n]
 		means = self.model.cluster_means[self.model.cluster_opt_n]
 		
 		if len(clusters) < 2:
 			return earlier_than
 		
 		# Sort clusters from oldest to youngest
 		labels = sorted(clusters.keys(), key=lambda label: means[label], reverse=True)
 		
-		phases_clu = dict((label, idx + 1) for idx, label in enumerate(labels))
-		# phases_clu = {label: phase, ...}; lower phase = earlier
+		# Assign phase numbers to clusters
+		phases_clu = dict([(label, n+1) for n, label in enumerate(labels)])
 		
 		collect = {}
 		for label in phases_clu:
 			for sample in clusters[label]:
 				collect[sample] = phases_clu[label]
 		phases_clu = collect
 		# phases_clu = {sample: phase, ...}
 		
+		# Eliminate cluster pairs which violate chronological relations given by stratigraphy
+		invalid = set()
+		for i, s1 in enumerate(samples):
+			if phases_clu[s1] is None:
+				continue
+			for j, s2 in enumerate(samples):
+				if phases_clu[s2] is None:
+					continue
+				if phases_clu[s1] < phases_clu[s2]:
+					if ((self.model.samples[s1].group == self.model.samples[s2].group) and (self.model.samples[s1].phase is not None) and (
+							self.model.samples[s2].phase is not None) and (self.model.samples[s1].phase > self.model.samples[s2].phase)):
+						invalid.add((phases_clu[s1], phases_clu[s2]))
+						invalid.add((phases_clu[s2], phases_clu[s1]))
+		
 		# Update earlier-than relationships based on phases derived from clustering
-		errors = []
 		for i, s1 in enumerate(samples):
+			if phases_clu[s1] is None:
+				continue
 			for j, s2 in enumerate(samples):
+				if phases_clu[s2] is None:
+					continue
+				if (phases_clu[s1], phases_clu[s2]) in invalid:
+					continue
 				if phases_clu[s1] < phases_clu[s2]:
 					earlier_than[i][j] = True
-					if (self.model.samples[s1].group == self.model.samples[s2].group) and (self.model.samples[s1].phase is not None) and (
-							self.model.samples[s2].phase is not None) and (self.model.samples[s1].phase > self.model.samples[s2].phase):
-						errors.append(
-							[s1, s2, phases_clu[s1], phases_clu[s2], self.model.samples[s1].phase, self.model.samples[s2].phase])
-		if errors:
-			print("Warning, collisions detected between stratigraphic phasing and clustering:")
-			for s1, s2, clu1, clu2, ph1, ph2 in errors:
-				print("%s (Strat. phase %s, Clu. phase %s), %s (Strat. phase %s, Clu. phase %s)" % (
-					s1, ph1, clu1, s2, ph2, clu2))
-			print()
 		
 		# Check if earlier_than has circular relationships
-		if not check_circular_relationships(earlier_than, samples):
-			# Visualize earlier_than as a DAG
-			visualize_earlier_than(earlier_than, samples)
-			raise Exception("Circular relationships detected")
+		check_circular_relationships(earlier_than, samples)
 		
 		# Extend the earlier_than matrix to include computed relations
 		earlier_than = extend_earlier_than(earlier_than)
 		
 		return earlier_than
 	
 	def find_dating_outliers(self) -> (List[str], List[str]):
@@ -315,35 +324,45 @@
 		Updates the phasing of samples based on stratigraphic relations.
 
 		Updates the groups and phases of samples based on their stratigraphic relations.
 
 		:param by_clusters: If True, update the phasing by clustering sample dates. Defaults to False.
 		:type by_clusters: bool, optional
 		:param by_dates: If True, update the phasing by comparing sample dates. Defaults to False.
-		:type by_dates: bool, optional
+		:type by_dates: bool, optional		
 		:return: True if phasing has changed, False otherwise.
 		:rtype: bool
 		"""
 		
+		phasing0 = set([(name, self.model.samples[name].group, self.model.samples[name].phase) for name in self.model.samples])
+		
 		earlier_than, samples = self.create_earlier_than_matrix()
 		if by_clusters and self.model.is_clustered:
 			earlier_than = self.update_earlier_than_by_clustering(earlier_than, samples)
 		
 		if by_dates and self.model.is_modeled:
 			earlier_than = self.update_earlier_than_by_dating(earlier_than, samples)
 		
-		groups_phases = get_groups_and_phases(earlier_than, samples)
+		ranges = [self.model.samples[name].get_range() for name in self.model.samples]		
+		groups_phases, phasing_multi = get_groups_and_phases(earlier_than, samples, ranges)
 		# groups_phases = {sample: [group, phase], ...}
+		# phasing_multi = {sample: [phase, ...], ...}
+		
+		if phasing_multi:
+			print("Warning! Some samples can be assigned to multiple phases:")
+			for name in phasing_multi:
+				print("%s: Phases %s" % (name, ", ".join([str(ph) for ph in phasing_multi[name]])))
+		
 		for name in self.model.samples:
 			if name in groups_phases:
 				group, phase = groups_phases[name]
 				self.model.samples[name].set_group(group)
 				self.model.samples[name].set_phase(phase)
 			else:
 				self.model.samples[name].set_group(None)
 				self.model.samples[name].set_phase(None)
 		
-		earlier_than_1, samples_1 = self.create_earlier_than_matrix()
-		if not ((earlier_than.shape == earlier_than.shape) and np.allclose(earlier_than, earlier_than_1) and (
-				samples == samples_1)):
+		phasing1 = set([(name, self.model.samples[name].group, self.model.samples[name].phase) for name in self.model.samples])
+		
+		if phasing0 != phasing1:
 			return True
 		return False
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MPlot.py` & `sitesyncro-0.9.6/src/sitesyncro/mhelpers/MPlot.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,14 +9,27 @@
 	:param model: The parent Model object
 	:type model: Model
 	"""
 	def __init__(self, model: 'Model'):
 		
 		self.model = model
 	
+	@staticmethod
+	def _format_year(value):
+		
+		if value is None:
+			return "None"
+		return "%0.2f" % (-(value - 1950))
+	
+	@staticmethod
+	def _sum_range(rng):
+		if None in rng:
+			return -1
+		return sum(rng)
+	
 	def plot_randomized(self, fname: str, show: bool = False) -> None:
 		"""
 		Plots the randomization test results.
 
 		Parameters:
 		fname (str): The filename where the plot will be saved.
 		show (bool): If True, the plot will be displayed. Default is False.
@@ -76,30 +89,37 @@
 		
 		ax1.set_xlabel("Clusters")
 		ax1.set_ylabel("Mean Silhouette Coefficient", color=color1)
 		ax1.plot(clu_ns, sils_plot, color=color1)
 		ax1.plot(clu_ns, sils_plot, ".", color=color1)
 		ax1.tick_params(axis="y", labelcolor=color1)
 		
-		ax2 = ax1.twinx()
-		ax2.set_ylabel("p", color=color2)
-		ax2.plot(clu_ns, ps_plot, color=color2)
-		ax2.plot(clu_ns, ps_plot, ".", color=color2)
+		if self.model.cluster_selection == 'mcst':
+			ax2 = ax1.twinx()
+			ax2.set_ylabel("p", color=color2)
+			ax2.plot(clu_ns, ps_plot, color=color2)
+			ax2.plot(clu_ns, ps_plot, ".", color=color2)
+			if self.model.p_value is not None:
+				ax2.plot([clu_ns[0], clu_ns[-1]], [self.model.p_value, self.model.p_value], "--", color=color2, linewidth=0.7)
+				ax2.annotate("p = %0.3f" % (self.model.p_value), xy=(clu_ns.mean(), self.model.p_value), xytext=(0, -3),
+							 textcoords="offset pixels", va="top", ha="center", color=color2)
+			ax2.tick_params(axis="y", labelcolor=color2)
+		
+		pyplot.xticks(clu_ns, clu_ns)
+		
 		if self.model.cluster_opt_n is not None:
-			ax2.plot([self.model.cluster_opt_n, self.model.cluster_opt_n], [0, max(ps_plot.max(), sils_plot.max())], color=color3,
+			ymin, ymax = ax1.get_ylim()
+			if self.model.cluster_selection == 'mcst':
+				ymin2, ymax2 = ax2.get_ylim()
+				ymin, ymax = min(ymin, ymin2), max(ymax, ymax2)
+			ax1.plot([self.model.cluster_opt_n, self.model.cluster_opt_n], [ymin, ymax], color=color3,
 					 linewidth=0.7, label="Optimal no. of clusters")
-		if self.model.p_value is not None:
-			ax2.plot([clu_ns[0], clu_ns[-1]], [self.model.p_value, self.model.p_value], "--", color=color2, linewidth=0.7)
-			ax2.annotate("p = %0.3f" % (self.model.p_value), xy=(clu_ns.mean(), self.model.p_value), xytext=(0, -3),
-						 textcoords="offset pixels", va="top", ha="center", color=color2)
-		ax2.tick_params(axis="y", labelcolor=color2)
+			ax1.set_ylim(ymin, ymax)
 		
-		pyplot.xticks(clu_ns, clu_ns)
 		pyplot.legend()
-		
 		fig.tight_layout()
 		pyplot.savefig(fname)
 		if show:
 			pyplot.show()
 		pyplot.close()
 	
 	def save_outliers(self, fname: str) -> None:
@@ -124,42 +144,29 @@
 			txt += "%s\n" % (", ".join(candidates))
 		else:
 			txt += "None\n"
 		
 		with open(fname, "w", encoding="utf-8") as file:
 			file.write(txt)
 	
-	def save_results_csv(self, fcsv: str) -> None:
+	def save_results_samples_csv(self, fcsv: str) -> None:
 		"""
-		Saves the results to a CSV file.
+		Saves the results for samples to a CSV file.
 
 		Parameters:
 		fcsv (str): The filename where the results will be saved.
 
 		Returns:
 		None
 		"""
-		
-		def _format_year(value):
-			
-			if value is None:
-				return "None"
-			return "%0.2f" % (-(value - 1950))
-		
 		samples = list(self.model.samples.keys())
-		
-		def _sum_range(rng):
-			if None in rng:
-				return -1
-			return sum(rng)
-		
 		samples = sorted(samples, key=lambda name: [
 			self.model.samples[name].group,
 			self.model.samples[name].phase,
-			_sum_range(self.model.samples[name].likelihood_range)
+			self._sum_range(self.model.samples[name].likelihood_range)
 		])
 		
 		cluster = dict([(name, None) for name in samples])
 		if self.model.is_clustered:
 			m_clusters = self.model.clusters[self.model.cluster_opt_n]
 			for clu in m_clusters:
 				for name in m_clusters[clu]:
@@ -173,11 +180,35 @@
 				posterior_min, posterior_max = self.model.samples[name].posterior_range
 				file.write('''"%s";"%s";"%s";%0.2f;%0.2f;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s;%s\n''' % (
 					name, self.model.samples[name].context, self.model.samples[name].area,
 					self.model.samples[name].age, self.model.samples[name].uncertainty,
 					int(self.model.samples[name].long_lived), int(self.model.samples[name].redeposited),
 					int(self.model.samples[name].outlier), self.model.samples[name].excavation_area_phase,
 					self.model.samples[name].group, self.model.samples[name].phase, cluster[name],
-					_format_year(likelihood_min), _format_year(likelihood_max),
-					_format_year(posterior_min), _format_year(posterior_max)
+					self._format_year(likelihood_min), self._format_year(likelihood_max),
+					self._format_year(posterior_min), self._format_year(posterior_max)
 				))
 
+	def save_results_phases_csv(self, fcsv: str) -> None:
+		"""
+		Saves the results for phases to a CSV file.
+
+		Parameters:
+		fcsv (str): The filename where the results will be saved.
+
+		Returns:
+		None
+		"""
+		phases = sorted(list(self.model.phases.keys()))
+		
+		with codecs.open(fcsv, "w", encoding="utf-8-sig") as file:
+			file.write(
+				"Group;Phase;Start From (CE);Start To (CE);End From (CE);End To (CE)\n")
+			for key in phases:
+				group, phase = key
+				start_from, start_to = self.model.phases[key].start_range
+				end_from, end_to = self.model.phases[key].end_range
+				file.write('''%d;%d;%s;%s;%s;%s\n''' % (
+					group, phase, 
+					self._format_year(start_from), self._format_year(start_to), 
+					self._format_year(end_from), self._format_year(end_to)
+				))
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro/mhelpers/MRandomization.py` & `sitesyncro-0.9.6/src/sitesyncro/mhelpers/MRandomization.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_cluster.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -91,18 +91,14 @@
 	D (np.ndarray): A distance matrix. If D is a 1-d condensed distance matrix, it will be converted to a 2-d form.
 	n (int): The desired number of clusters.
 	method (str, optional): The method to use for HCA. Default is "average".
 
 	Returns:
 		clusters = {label: [idx, ...], ...}; idx = index D
 	
-	Example:
-	If we have a distance matrix for three distributions and we want to cluster them into two groups, the function
-	might return {1: [0, 2], 2: [1]}. This means that distributions 0 and 2 are in one cluster and distribution 1 is
-	in another cluster.
 	"""
 	if D.ndim == 1:
 		D = squareform(D)
 	d = calc_distances_pca(D)
 	if d.shape[0] == d.shape[1]:
 		d = squareform(d)
 	clusters_l = fcluster(linkage(d, method=method, metric="euclidean"), n, criterion="maxclust")
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_data.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_data.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_load.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_load.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_oxcal.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_oxcal.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_radiocarbon.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_radiocarbon.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_simulate.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_simulate.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro/utils/fnc_stat.py` & `sitesyncro-0.9.6/src/sitesyncro/utils/fnc_stat.py`

 * *Files identical despite different names*

### Comparing `sitesyncro-0.9.5/src/sitesyncro.egg-info/PKG-INFO` & `sitesyncro-0.9.6/src/sitesyncro.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sitesyncro
-Version: 0.9.5
+Version: 0.9.6
 Summary: SiteSyncro - Site-specific chronological modeling and synchronization
 Home-page: https://github.com/demjanp/SiteSyncro
 Author: Peter Demjan
 Author-email: peter.demjan@gmail.com
 Keywords: archaeology,radiocarbon,chronology,stratigraphy
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
@@ -37,14 +37,15 @@
 
 1. [About SiteSyncro](#about)
 2. [Installation](#installation)
 3. [Usage](#usage)
    * [Input File Format](#input_file)
    * [Model Class](#model_class)
    * [Sample Class](#sample_class)
+   * [Phase Class](#phase_class)
 4. [Developer Notes](#developer)
 	* [Preparing the Virtual Environment](#venv)
 	* [Building a Windows Executable](#build)
 5. [Contact](#contact)
 6. [Acknowledgements](#acknowledgements)
 7. [License](#license)
 
@@ -85,20 +86,20 @@
 ```
 or
 ```
 sitesyncro.exe -input data_sample.csv
 ```
 `process.py` & `sitesyncro.exe` accepts the following command-line arguments:
 - `-h`, `--help`: Show help message and exit.
-- `-directory`: Working directory for model data (default is "model").
+- `-directory`: Working directory for model data (default is 'model').
 - `-input`: The path to the input file in semicolon-separated CSV format.
-- `-curve_name`: File name of the radiocarbon age calibration curve (default is "intcal20.14c").
-- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is "sequence").
+- `-curve_name`: File name of the radiocarbon age calibration curve (default is 'intcal20.14c').
+- `-phase_model`: OxCal phase model type (can be 'sequence', 'contiguous', 'overlapping', or 'none'; default is 'sequence').
 - `-cluster_n`: Number of clusters to form (-1 = automatic; default is -1).
-- `-min_years_per_cluster`: Minimum number of years per cluster. (default is 25).
+- `-cluster_selection`: Cluster selection method ('silhouette' or 'mcst'; default is 'silhouette').
 - `-by_clusters`: Flag indicating whether to update the phasing by clustering sample dates (default is 0).
 - `-by_dates`: Flag indicating whether to update the phasing by comparing sample dates (default is 0).
 - `-uniform`: Flag indicating whether to use a uniform distribution for the calendar ages (default is 0).
 - `-p_value`: P-value for the randomization tests (default is 0.05).
 - `-uncertainty_base`: Base uncertainty for the radiocarbon dates for the randomization tests (default is 15).
 - `-npass`: Minimum number of passes for the randomization tests (default is 100).
 - `-convergence`: Convergence threshold for the randomization tests (default is 0.99).
@@ -147,24 +148,26 @@
     
     # Plot the randomization test result
     model.plot_randomized()
     
     # Plot the clustering result
     model.plot_clusters()
     
-    # Save the results to a CSV file
-    model.save_csv()
+    # Save the results to a CSV files
+    model.save_csv_samples()
+    model.save_csv_phases()
 ```
 This will create the default directory `model` and generate the following files:
 `model.json.gz`
 `model.oxcal`
 `model.js`, `model.log`, `model.txt`
 `randomized.pdf`
 `silhouette.pdf`
-`results.csv`
+`results_samples.csv`
+`results_phases.csv`
 
 See [Model Class](https://sitesyncro.readthedocs.io/en/latest/model.html) documentation for more information.
 
 ### Sample Class <a name="sample_class"></a>
 The `Sample` class represents a single radiocarbon sample. Here is a basic example of how to use it:
 
 ```python
@@ -177,14 +180,37 @@
 	
 	# Print the sample data
 	print(sample)
 ```
 
 See [Sample Class](https://sitesyncro.readthedocs.io/en/latest/sample.html) documentation for more information.
 
+### Phase Class <a name="phase_class"></a>
+The `Phase` class represents a modeled chronological phase. Here is a basic example of how to use it:
+
+```python
+from sitesyncro import Model
+
+if __name__ == '__main__':
+    
+    # Initialize the Model object and load data from the directory 'model'
+    model = Model(directory='model')
+    
+    # Print information on phasing (if model has been processed)
+    for group, phase in model.phases:
+        phase = model.phases[(group, phase)]
+        start_from, start_to = phase.start_range
+        end_from, end_to = phase.end_range
+        
+        # Print the group, phase, and start and end ranges
+        print(f'Group: {group}, Phase: {phase}, Start: {start_from}-{start_to}, End: {end_from}-{end_to}')
+```
+
+See [Phase Class](https://sitesyncro.readthedocs.io/en/latest/phase.html) documentation for more information.
+
 ## Developer Notes <a name="developer"></a>
 ### Preparing the Virtual Environment <a name="venv"></a>
 SiteSyncro requires [Python 3.10](https://www.python.org/downloads/).
 
 To prepare a Python virtual environment open a terminal or command prompt window and type the following commands:
 
 ```
```

### Comparing `sitesyncro-0.9.5/src/sitesyncro.egg-info/SOURCES.txt` & `sitesyncro-0.9.6/src/sitesyncro.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -1,27 +1,35 @@
 LICENSE
 README.md
 setup.py
 src/sitesyncro/Model.py
+src/sitesyncro/Phase.py
 src/sitesyncro/Sample.py
 src/sitesyncro/__init__.py
 src/sitesyncro.egg-info/PKG-INFO
 src/sitesyncro.egg-info/SOURCES.txt
 src/sitesyncro.egg-info/dependency_links.txt
 src/sitesyncro.egg-info/requires.txt
 src/sitesyncro.egg-info/top_level.txt
+src/sitesyncro/graphviz/__init__.py
 src/sitesyncro/mhelpers/MCluster.py
 src/sitesyncro/mhelpers/MOxCal.py
 src/sitesyncro/mhelpers/MPhasing.py
 src/sitesyncro/mhelpers/MPlot.py
 src/sitesyncro/mhelpers/MRandomization.py
 src/sitesyncro/mhelpers/__init__.py
+src/sitesyncro/pygraphviz/__init__.py
+src/sitesyncro/pygraphviz/agraph.py
+src/sitesyncro/pygraphviz/graphviz.py
+src/sitesyncro/pygraphviz/scraper.py
+src/sitesyncro/pygraphviz/testing.py
 src/sitesyncro/utils/__init__.py
 src/sitesyncro/utils/fnc_cluster.py
 src/sitesyncro/utils/fnc_data.py
 src/sitesyncro/utils/fnc_load.py
 src/sitesyncro/utils/fnc_mp.py
 src/sitesyncro/utils/fnc_oxcal.py
 src/sitesyncro/utils/fnc_phase.py
 src/sitesyncro/utils/fnc_radiocarbon.py
 src/sitesyncro/utils/fnc_simulate.py
-src/sitesyncro/utils/fnc_stat.py
+src/sitesyncro/utils/fnc_stat.py
+src/sitesyncro/utils/fnc_visualize.py
```

