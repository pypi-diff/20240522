# Comparing `tmp/neurocaps-0.9.0.post4.tar.gz` & `tmp/neurocaps-0.9.0.post5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neurocaps-0.9.0.post4.tar", last modified: Sat May 18 21:41:13 2024, max compression
+gzip compressed data, was "neurocaps-0.9.0.post5.tar", last modified: Wed May 22 01:30:58 2024, max compression
```

## Comparing `neurocaps-0.9.0.post4.tar` & `neurocaps-0.9.0.post5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1077 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/LICENSE.md
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15139 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    14181 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/README.md
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       78 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/_utils/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      352 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/__init__.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       87 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2492 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/_capgetter.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      179 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2825 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_check_confound_names.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      178 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     5578 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     8043 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     2637 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/analysis/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      137 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    57051 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/cap.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     4716 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/merge.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1564 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/analysis/standardize.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:12.000000 neurocaps-0.9.0.post4/neurocaps/extraction/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       86 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/extraction/__init__.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    29824 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/neurocaps/extraction/timeseriesextractor.py
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)    15139 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/PKG-INFO
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1061 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/SOURCES.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)        1 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/dependency_links.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      121 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/requires.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       10 2024-05-18 21:41:11.000000 neurocaps-0.9.0.post4/neurocaps.egg-info/top_level.txt
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1324 2024-05-18 21:40:19.000000 neurocaps-0.9.0.post4/pyproject.toml
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)       38 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/setup.cfg
-drwxr-xr-x   0 dsmit216 (351141) hpc_nbc    (147)        0 2024-05-18 21:41:13.000000 neurocaps-0.9.0.post4/tests/
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     6365 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_CAP.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     3685 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1053 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor_additional.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)     1906 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_merge_dicts.py
--rw-r--r--   0 dsmit216 (351141) hpc_nbc    (147)      678 2024-05-18 21:40:20.000000 neurocaps-0.9.0.post4/tests/test_standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.826772 neurocaps-0.9.0.post5/
+-rw-rw-rw-   0        0        0     1077 2024-04-28 16:38:21.000000 neurocaps-0.9.0.post5/LICENSE.md
+-rw-rw-rw-   0        0        0    15505 2024-05-22 01:30:58.825775 neurocaps-0.9.0.post5/PKG-INFO
+-rw-rw-rw-   0        0        0    14181 2024-05-18 21:20:48.000000 neurocaps-0.9.0.post5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.726299 neurocaps-0.9.0.post5/neurocaps/
+-rw-rw-rw-   0        0        0       78 2024-04-28 16:38:21.000000 neurocaps-0.9.0.post5/neurocaps/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.774561 neurocaps-0.9.0.post5/neurocaps/_utils/
+-rw-rw-rw-   0        0        0      369 2024-05-22 01:20:59.000000 neurocaps-0.9.0.post5/neurocaps/_utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.787210 neurocaps-0.9.0.post5/neurocaps/_utils/_cap_internals/
+-rw-rw-rw-   0        0        0       88 2024-04-28 16:38:21.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_cap_internals/__init__.py
+-rw-rw-rw-   0        0        0     2591 2024-05-09 19:38:42.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_cap_internals/_capgetter.py
+-rw-rw-rw-   0        0        0      186 2024-04-28 16:38:21.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_cap_internals/_pickle_to_dict.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.802749 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/
+-rw-rw-rw-   0        0        0      238 2024-05-22 01:24:25.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+-rw-rw-rw-   0        0        0     2863 2024-05-22 01:09:57.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
+-rw-rw-rw-   0        0        0     5777 2024-05-22 00:26:07.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
+-rw-rw-rw-   0        0        0     8190 2024-05-18 21:30:36.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
+-rw-rw-rw-   0        0        0     2701 2024-05-22 00:17:25.000000 neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.809651 neurocaps-0.9.0.post5/neurocaps/analysis/
+-rw-rw-rw-   0        0        0      143 2024-05-14 02:35:32.000000 neurocaps-0.9.0.post5/neurocaps/analysis/__init__.py
+-rw-rw-rw-   0        0        0    58768 2024-05-22 00:26:07.000000 neurocaps-0.9.0.post5/neurocaps/analysis/cap.py
+-rw-rw-rw-   0        0        0     4811 2024-05-14 02:35:32.000000 neurocaps-0.9.0.post5/neurocaps/analysis/merge.py
+-rw-rw-rw-   0        0        0     1598 2024-05-14 02:35:32.000000 neurocaps-0.9.0.post5/neurocaps/analysis/standardize.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.809651 neurocaps-0.9.0.post5/neurocaps/extraction/
+-rw-rw-rw-   0        0        0       89 2024-04-28 16:38:21.000000 neurocaps-0.9.0.post5/neurocaps/extraction/__init__.py
+-rw-rw-rw-   0        0        0    30304 2024-05-22 00:26:07.000000 neurocaps-0.9.0.post5/neurocaps/extraction/timeseriesextractor.py
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.824775 neurocaps-0.9.0.post5/neurocaps.egg-info/
+-rw-rw-rw-   0        0        0    15505 2024-05-22 01:30:58.000000 neurocaps-0.9.0.post5/neurocaps.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1092 2024-05-22 01:30:58.000000 neurocaps-0.9.0.post5/neurocaps.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 01:30:58.000000 neurocaps-0.9.0.post5/neurocaps.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      121 2024-05-22 01:30:58.000000 neurocaps-0.9.0.post5/neurocaps.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-05-22 01:30:58.000000 neurocaps-0.9.0.post5/neurocaps.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1496 2024-05-22 01:29:50.000000 neurocaps-0.9.0.post5/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 01:30:58.827781 neurocaps-0.9.0.post5/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 01:30:58.822779 neurocaps-0.9.0.post5/tests/
+-rw-rw-rw-   0        0        0     6471 2024-05-02 14:49:04.000000 neurocaps-0.9.0.post5/tests/test_CAP.py
+-rw-rw-rw-   0        0        0     3767 2024-05-09 19:38:42.000000 neurocaps-0.9.0.post5/tests/test_TimeseriesExtractor.py
+-rw-rw-rw-   0        0        0     1077 2024-05-18 21:37:50.000000 neurocaps-0.9.0.post5/tests/test_TimeseriesExtractor_additional.py
+-rw-rw-rw-   0        0        0     1931 2024-05-02 14:49:04.000000 neurocaps-0.9.0.post5/tests/test_merge_dicts.py
+-rw-rw-rw-   0        0        0      691 2024-05-14 02:35:32.000000 neurocaps-0.9.0.post5/tests/test_standardize.py
```

### Comparing `neurocaps-0.9.0.post4/LICENSE.md` & `neurocaps-0.9.0.post5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neurocaps-0.9.0.post4/PKG-INFO` & `neurocaps-0.9.0.post5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,218 +1,188 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.9.0.post4
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nibabel
-Requires-Dist: nilearn==0.10.2
-Requires-Dist: surfplot
-Requires-Dist: neuromaps
-Requires-Dist: pybids; platform_system != "Windows"
-
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
-**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
-
-If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
-
-Custom Key Structure:
-- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
-Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
-visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
-        
-Example 
-The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
-
-```Python
-parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                             "regions": {"Vis" : {"lh": [0,1],
-                                                  "rh": [3,4]},
-                                         "Hippocampus": {"lh": [2],
-                                                         "rh": [5]}}}}
- ```
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-# Examples use randomized data
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-```python
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-```
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-```python
-# If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=2)
-```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
-
-# Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
-
-Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
-
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
-[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
-
-[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
-
-[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+Custom Key Structure:
+- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+        
+Example 
+The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+```Python
+parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+ ```
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+# Examples use randomized data
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+```python
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+```
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+```python
+# If you experience coverage issues, usually smoothing helps to mitigate these issues
+cap_analysis.caps2surf(fwhm=2)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+
+[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
+
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.9.0.post4/README.md` & `neurocaps-0.9.0.post5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,40 @@
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.9.0.post5
+Summary: Co-activation patterns Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nibabel
+Requires-Dist: nilearn==0.10.2
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
+Requires-Dist: pybids; platform_system != "Windows"
+
 # neurocaps
 This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
 
 **Still in beta but stable.**
 
 # Installation
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/_utils/_check_confound_names.py` & `neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,39 +1,39 @@
-import warnings
-def _check_confound_names(high_pass, specified_confound_names, n_acompcor_separate):
-    if specified_confound_names == None:
-        if high_pass:
-            # Do not use cosine or acompcor regressor if high pass filtering is not None. Acompcor regressors are estimated on high pass filtered version 
-            # of data form fmriprep
-            confound_names = [
-                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
-                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
-                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
-                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
-                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
-                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2"
-            ]
-        else:
-            confound_names = [
-                "cosine*",
-                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
-                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
-                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
-                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
-                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
-                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2", 
-                "a_comp_cor_00", "a_comp_cor_01", "a_comp_cor_02", "a_comp_cor_03", "a_comp_cor_04", "a_comp_cor_05"
-            ]
-    else:
-        assert type(specified_confound_names) == list and len(specified_confound_names) > 0 , "confound_names must be a non-empty list."
-        confound_names = specified_confound_names
-
-    if n_acompcor_separate:
-        check_confounds = [confound for confound in confound_names if "a_comp_cor" not in confound]
-        if len(confound_names) > len(check_confounds):
-            removed_confounds = [element for element in confound_names if element not in check_confounds]
-            if specified_confound_names: warnings.warn(f"Since `n_acompcor_separate` has been specified, specified acompcor components in `confound_names` will be disregarded and replaced with the first {n_acompcor_separate} components of the white matter and cerebrospinal fluid masks for each participant. The following components will not be used {removed_confounds}")
-            confound_names = check_confounds 
-    
-    print(f"List of confound regressors that will be used during timeseries extraction if available in confound dataframe: {confound_names}", flush=True)
-    
+import warnings
+def _check_confound_names(high_pass, specified_confound_names, n_acompcor_separate):
+    if specified_confound_names == None:
+        if high_pass:
+            # Do not use cosine or acompcor regressor if high pass filtering is not None. Acompcor regressors are estimated on high pass filtered version 
+            # of data form fmriprep
+            confound_names = [
+                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
+                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
+                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
+                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
+                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
+                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2"
+            ]
+        else:
+            confound_names = [
+                "cosine*",
+                "trans_x", "trans_x_derivative1", "trans_x_power2", "trans_x_derivative1_power2",
+                "trans_y", "trans_y_derivative1", "trans_y_derivative1_power2", "trans_y_power2",
+                "trans_z", "trans_z_derivative1", "trans_z_power2", "trans_z_derivative1_power2",
+                "rot_x", "rot_x_derivative1", "rot_x_power2", "rot_x_derivative1_power2",
+                "rot_y", "rot_y_derivative1", "rot_y_power2", "rot_y_derivative1_power2",
+                "rot_z", "rot_z_derivative1", "rot_z_derivative1_power2", "rot_z_power2", 
+                "a_comp_cor_00", "a_comp_cor_01", "a_comp_cor_02", "a_comp_cor_03", "a_comp_cor_04", "a_comp_cor_05"
+            ]
+    else:
+        assert type(specified_confound_names) == list and len(specified_confound_names) > 0 , "confound_names must be a non-empty list."
+        confound_names = specified_confound_names
+
+    if n_acompcor_separate:
+        check_confounds = [confound for confound in confound_names if "a_comp_cor" not in confound]
+        if len(confound_names) > len(check_confounds):
+            removed_confounds = [element for element in confound_names if element not in check_confounds]
+            if specified_confound_names: warnings.warn(f"Since `n_acompcor_separate` has been specified, specified acompcor components in `confound_names` will be disregarded and replaced with the first {n_acompcor_separate} components of the white matter and cerebrospinal fluid masks for each participant. The following components will not be used {removed_confounds}")
+            confound_names = check_confounds 
+    
+    print(f"List of confound regressors that will be used during timeseries extraction if available in confound dataframe: {confound_names}", flush=True)
+    
     return confound_names
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py` & `neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,72 +1,74 @@
-from nilearn import datasets
-import warnings, re, os
-
-def _check_parcel_approach(parcel_approach, call = "TimeseriesExtractor"):
-    valid_parcel_dict = {"Schaefer": {"n_rois" : 400, "yeo_networks": 7, "resolution_mm": 1},
-                         "AAL": {"version": "SPM12"},
-                         "Custom": {"maps": "/location/to/parcellation.nii.gz",
-                                    "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                                    "regions": {"Vis" : {"lh": [0,1],
-                                                          "rh": [3,4]},
-                                                 "Hippocampus": {"lh": [2],
-                                                                 "rh": [5]}}}}
-
-    if not isinstance(parcel_approach,dict) or isinstance(parcel_approach,dict) and len(parcel_approach.keys()) > 0 and not isinstance(parcel_approach[list(parcel_approach.keys())[0]],dict):
-        raise ValueError(f"Please include a valid `parcel_approach` in one of the following dictionary formats for 'Schaefer' or 'AAL' {valid_parcel_dict}")
-    
-    if len(parcel_approach.keys()) > 1:
-        raise ValueError(f"Only one parcellation approach can be selected from the following valid options: {valid_parcel_dict.keys()}.\n Example format of `parcel_approach`: {valid_parcel_dict}")
-    
-    if "Schaefer" not in parcel_approach.keys() and "AAL" not in parcel_approach.keys() and "Custom" not in parcel_approach.keys():
-        raise ValueError(f"Please include a valid `parcel_approach` in one of the following formats for 'Schaefer', 'AAL', or 'Custom': {valid_parcel_dict}")
-    
-    if "Schaefer" in parcel_approach.keys():
-        if "n_rois" not in parcel_approach["Schaefer"].keys():
-            warnings.warn("'n_rois' not specified in `parcel_approach`. Defaulting to 400 ROIs.")
-            parcel_approach["Schaefer"].update({"n_rois": 400})
-
-        if "yeo_networks" not in parcel_approach["Schaefer"].keys():
-            warnings.warn("'yeo_networks' not specified in `parcel_approach`. Defaulting to 7 networks.")
-            parcel_approach["Schaefer"].update({"yeo_networks": 7})
-        
-        if "resolution_mm" not in parcel_approach["Schaefer"].keys():
-            warnings.warn("'resolution_mm' not specified in `parcel_approach`. Defaulting to 1mm.")
-            parcel_approach["Schaefer"].update({"resolution_mm": 1})
-
-        # Get atlas
-        fetched_schaefer = datasets.fetch_atlas_schaefer_2018(n_rois=parcel_approach["Schaefer"]["n_rois"], yeo_networks=parcel_approach["Schaefer"]["yeo_networks"], resolution_mm=parcel_approach["Schaefer"]["resolution_mm"])
-        parcel_approach["Schaefer"].update({"maps": fetched_schaefer.maps})
-        parcel_approach["Schaefer"].update({"nodes": [label.decode().split("7Networks_")[-1]  for label in fetched_schaefer.labels]})
-        # Get node networks
-        parcel_approach["Schaefer"].update({"regions": list(dict.fromkeys([re.split("LH_|RH_", node)[-1].split("_")[0] for node in parcel_approach["Schaefer"]["nodes"]]))})
-
-    if "AAL" in parcel_approach.keys():
-        if "version" not in parcel_approach["AAL"].keys():
-            warnings.warn("'version' not specified in `parcel_approach`. Defaulting to 'SPM12'.")
-            parcel_approach["AAL"].update({"version": "SPM12"})
-
-        # Get atlas
-        fetched_aal = datasets.fetch_atlas_aal(version=parcel_approach["AAL"]["version"])
-        parcel_approach["AAL"].update({"maps": fetched_aal.maps})
-        parcel_approach["AAL"].update({"nodes": [label for label in fetched_aal.labels]})
-        # Get node networks
-        parcel_approach["AAL"].update({"regions": list(dict.fromkeys([node.split("_")[0] for node in parcel_approach["AAL"]["nodes"]]))})
-    
-    if "Custom" in parcel_approach.keys():
-        if call  == "TimeseriesExtractor" and "maps" not in parcel_approach["Custom"].keys():
-            raise ValueError(f"For `Custom` parcel_approach, a nested key-value pair containing the key 'maps' with the value being a string specifying the location of the parcellation is needed. Example: {{'Custom' : valid_parcel_dict['Custom']}}")
-        check_subkeys = ["nodes" in parcel_approach["Custom"].keys(), "regions" in parcel_approach["Custom"].keys()]
-        if not all(check_subkeys):
-            missing_subkeys = [["nodes", "regions"][x] for x,y in enumerate(check_subkeys) if y == False]
-            error_message = f"The following subkeys haven't been detected {missing_subkeys}."
-            if call == "TimeseriesExtractor": warnings.warn(error_message + " These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
-            else: 
-                custom_example = {"Custom": {"nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                                             "regions": {"Vis" : {"lh": [0,1],
-                                                                   "rh": [3,4]}},
-                                                                   "Hippocampus": {"lh": [2],"rh": [5]}}}
-                raise ValueError(error_message + f" These subkeys are needed for plotting. Please reassign `parcel_approach` using `self.parcel_approach` amd refer to the example structure: {custom_example}")
-        if call  == "TimeseriesExtractor" and not os.path.isfile(parcel_approach["Custom"]["maps"]):
-            raise ValueError("Please specify the location to the custom parcellation to be used.")
-
+from nilearn import datasets
+import warnings, re, os
+
+def _check_parcel_approach(parcel_approach, call = "TimeseriesExtractor"):
+    valid_parcel_dict = {"Schaefer": {"n_rois" : 400, "yeo_networks": 7, "resolution_mm": 1},
+                         "AAL": {"version": "SPM12"},
+                         "Custom": {"maps": "/location/to/parcellation.nii.gz",
+                                    "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                                    "regions": {"Vis" : {"lh": [0,1],
+                                                          "rh": [3,4]},
+                                                 "Hippocampus": {"lh": [2],
+                                                                 "rh": [5]}}}}
+
+    if not isinstance(parcel_approach,dict) or isinstance(parcel_approach,dict) and len(parcel_approach.keys()) > 0 and not isinstance(parcel_approach[list(parcel_approach.keys())[0]],dict):
+        raise ValueError(f"Please include a valid `parcel_approach` in one of the following dictionary formats for 'Schaefer' or 'AAL' {valid_parcel_dict}")
+    
+    if len(parcel_approach.keys()) > 1:
+        raise ValueError(f"Only one parcellation approach can be selected from the following valid options: {valid_parcel_dict.keys()}.\nExample format of `parcel_approach`: {valid_parcel_dict}")
+    
+    if "Schaefer" not in parcel_approach.keys() and "AAL" not in parcel_approach.keys() and "Custom" not in parcel_approach.keys():
+        raise ValueError(f"Please include a valid `parcel_approach` in one of the following formats for 'Schaefer', 'AAL', or 'Custom': {valid_parcel_dict}")
+    
+    if "Schaefer" in parcel_approach.keys():
+        if "n_rois" not in parcel_approach["Schaefer"].keys():
+            warnings.warn("'n_rois' not specified in `parcel_approach`. Defaulting to 400 ROIs.")
+            parcel_approach["Schaefer"].update({"n_rois": 400})
+
+        if "yeo_networks" not in parcel_approach["Schaefer"].keys():
+            warnings.warn("'yeo_networks' not specified in `parcel_approach`. Defaulting to 7 networks.")
+            parcel_approach["Schaefer"].update({"yeo_networks": 7})
+        
+        if "resolution_mm" not in parcel_approach["Schaefer"].keys():
+            warnings.warn("'resolution_mm' not specified in `parcel_approach`. Defaulting to 1mm.")
+            parcel_approach["Schaefer"].update({"resolution_mm": 1})
+
+        # Get atlas
+        fetched_schaefer = datasets.fetch_atlas_schaefer_2018(n_rois=parcel_approach["Schaefer"]["n_rois"], 
+                                                              yeo_networks=parcel_approach["Schaefer"]["yeo_networks"], 
+                                                              resolution_mm=parcel_approach["Schaefer"]["resolution_mm"])
+        parcel_approach["Schaefer"].update({"maps": fetched_schaefer.maps})
+        parcel_approach["Schaefer"].update({"nodes": [label.decode().split("7Networks_")[-1]  for label in fetched_schaefer.labels]})
+        # Get node networks
+        parcel_approach["Schaefer"].update({"regions": list(dict.fromkeys([re.split("LH_|RH_", node)[-1].split("_")[0] for node in parcel_approach["Schaefer"]["nodes"]]))})
+
+    if "AAL" in parcel_approach.keys():
+        if "version" not in parcel_approach["AAL"].keys():
+            warnings.warn("'version' not specified in `parcel_approach`. Defaulting to 'SPM12'.")
+            parcel_approach["AAL"].update({"version": "SPM12"})
+
+        # Get atlas
+        fetched_aal = datasets.fetch_atlas_aal(version=parcel_approach["AAL"]["version"])
+        parcel_approach["AAL"].update({"maps": fetched_aal.maps})
+        parcel_approach["AAL"].update({"nodes": [label for label in fetched_aal.labels]})
+        # Get node networks
+        parcel_approach["AAL"].update({"regions": list(dict.fromkeys([node.split("_")[0] for node in parcel_approach["AAL"]["nodes"]]))})
+    
+    if "Custom" in parcel_approach.keys():
+        if call  == "TimeseriesExtractor" and "maps" not in parcel_approach["Custom"].keys():
+            raise ValueError(f"For `Custom` parcel_approach, a nested key-value pair containing the key 'maps' with the value being a string specifying the location of the parcellation is needed.\nExample: {{'Custom' : valid_parcel_dict['Custom']}}")
+        check_subkeys = ["nodes" in parcel_approach["Custom"].keys(), "regions" in parcel_approach["Custom"].keys()]
+        if not all(check_subkeys):
+            missing_subkeys = [["nodes", "regions"][x] for x,y in enumerate(check_subkeys) if y == False]
+            error_message = f"The following subkeys haven't been detected {missing_subkeys}."
+            if call == "TimeseriesExtractor": warnings.warn(error_message + " These labels are not needed for timeseries extraction but are needed for future timeseries or CAPs plotting.")
+            else: 
+                custom_example = {"Custom": {"nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                                             "regions": {"Vis" : {"lh": [0,1],
+                                                                   "rh": [3,4]}},
+                                                                   "Hippocampus": {"lh": [2],"rh": [5]}}}
+                raise ValueError(error_message + f" These subkeys are needed for plotting. Please reassign `parcel_approach` using `self.parcel_approach` amd refer to the example structure: {custom_example}")
+        if call  == "TimeseriesExtractor" and not os.path.isfile(parcel_approach["Custom"]["maps"]):
+            raise ValueError("Please specify the location to the custom parcellation to be used.")
+
     return parcel_approach
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py` & `neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,148 +1,148 @@
-def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info, verbose, flush_print):
-
-    from nilearn.maskers import NiftiLabelsMasker
-    from nilearn.image import index_img, load_img
-    import copy, json, math, numpy as np, pandas as pd, warnings
-
-    # Intitialize subject dictionary
-    subject_timeseries = {subj_id: {}}
-    
-    for run in run_list:
-
-        run_id = "run-1" if run == None else run
-        run = run if run != None else ""
-
-        # Get files from specific run
-        nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file.split("/")[-1]]
-        if len(mask_files) != 0:
-            mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
-        else:
-            mask_file = []
-        confound_file = [confound_file for confound_file in confound_files if run in confound_file.split("/")[-1]] if signal_clean_info["use_confounds"] else None
-        confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file.split("/")[-1]] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
-
-        if verbose: print(f"Running subject: {subj_id}; run: {run_id}; \n {nifti_file}", flush=flush_print)
-
-        confound_df = pd.read_csv(confound_file[0], sep="\t") if signal_clean_info["use_confounds"] else None
-
-        event_file = None if len(event_files) == 0 else [event_file for event_file in event_files if run in event_file.split("/")[-1]]
-
-        # Extract confound information of interest and ensure confound file does not contain NAs
-        if signal_clean_info["use_confounds"]:
-            # Extract first "n" numbers of specified WM and CSF components
-            confound_names = copy.deepcopy(signal_clean_info["confound_names"])
-            if confound_metadata_file:
-                with open(confound_metadata_file[0]) as foo:
-                    confound_metadata = json.load(foo)
-            
-                acompcors = sorted([acompcor for acompcor in confound_metadata.keys() if "a_comp_cor" in acompcor])
-
-                acompcors_CSF = [acompcor_CSF for acompcor_CSF in acompcors if confound_metadata[acompcor_CSF]["Mask"] == "CSF"][0:signal_clean_info["n_acompcor_separate"]]
-                acompcor_WM = [acompcor_WM for acompcor_WM in acompcors if confound_metadata[acompcor_WM]["Mask"] == "WM"][0:signal_clean_info["n_acompcor_separate"]]
-                
-                confound_names.extend(acompcors_CSF + acompcor_WM)
-
-            valid_confounds = []
-            invalid_confounds = []
-            for confound_name in confound_names:
-                if "*" in confound_name:
-                    prefix = confound_name.split("*")[0]
-                    confounds_list = [col for col in confound_df.columns if col.startswith(prefix)]
-                else:
-                    confounds_list = [col for col in confound_df.columns if col == confound_name] 
-            
-                if len(confounds_list) > 0: valid_confounds.extend(confounds_list)
-                else: invalid_confounds.extend([confound_name])
-
-            if len(invalid_confounds) > 0: 
-                if verbose: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}", flush=flush_print)
-
-            confounds = confound_df[valid_confounds]
-            confounds = confounds.fillna(0)
-
-            if signal_clean_info["fd_threshold"]: 
-                censor = True
-                if "framewise_displacement" in confound_df.columns:
-                    fd_array = confound_df["framewise_displacement"].fillna(0).values
-                else:
-                    censor = False
-                    warnings.warn(f"For subject {subj_id}, `fd_threshold` specified but 'framewise_displacement' is not a column in the confound dataframe so removal of volumes after nuisance regression will not be done.")
-            else:
-                censor = False
-
-            if verbose: print(f"Confounds used for subject: {subj_id}; run: {run_id} - {confounds.columns}", flush=flush_print)
-
-        # Create the masker for extracting time series
-        if len(mask_file) !=0:
-            masker = NiftiLabelsMasker(
-                mask_img=mask_file[0],
-                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
-                resampling_target='data',
-                standardize=signal_clean_info["standardize"],
-                detrend=signal_clean_info["detrend"],
-                low_pass=signal_clean_info["low_pass"],
-                high_pass=signal_clean_info["high_pass"],
-                t_r=tr,
-                smoothing_fwhm=signal_clean_info["fwhm"]
-            )
-        else:
-            masker = NiftiLabelsMasker(
-                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
-                resampling_target='data',
-                standardize=signal_clean_info["standardize"],
-                detrend=signal_clean_info["detrend"],
-                low_pass=signal_clean_info["low_pass"],
-                high_pass=signal_clean_info["high_pass"],
-                t_r=tr,
-                smoothing_fwhm=signal_clean_info["fwhm"]
-            )
-        # Load and discard volumes if needed
-        nifti_img = load_img(nifti_file[0])
-        if signal_clean_info["dummy_scans"]: 
-            nifti_img = index_img(nifti_img, slice(signal_clean_info["dummy_scans"], None))
-            if signal_clean_info["use_confounds"]: 
-                confounds.drop(list(range(0,signal_clean_info["dummy_scans"])),axis=0,inplace=True)
-                # Truncate the fd_array also
-                if censor:
-                    fd_array = fd_array[signal_clean_info["dummy_scans"]:]
-            offset = signal_clean_info["dummy_scans"] 
-
-        # Extract timeseries
-        timeseries = masker.fit_transform(nifti_img, confounds=confounds) if signal_clean_info["use_confounds"] else masker.fit_transform(nifti_img)
-
-        if censor:
-            censor_volumes = list(np.where(fd_array > signal_clean_info["fd_threshold"])[0])
-
-        if event_file:
-            event_df = pd.read_csv(event_file[0], sep=None)
-            # Get specific timing information for specific condition
-            condition_df = event_df[event_df["trial_type"] == condition] 
-
-            # Empty list for scans
-            scan_list = []
-
-            # Convert times into scan numbers to obtain the scans taken when the participant was exposed to the condition of interest; include partial scans
-            for i in condition_df.index:
-                onset_scan, duration_scan = int(condition_df.loc[i,"onset"]/tr), math.ceil((condition_df.loc[i,"onset"] + condition_df.loc[i,"duration"])/tr)
-                if signal_clean_info["dummy_scans"]:
-                    scan_list.extend([scan - offset for scan in range(onset_scan, duration_scan + 1) if scan not in range(0, signal_clean_info["dummy_scans"])])
-                else:
-                    scan_list.extend(list(range(onset_scan, duration_scan + 1)))
-                if censor:
-                    scan_list = [volume for volume in scan_list if volume not in censor_volumes]
-
-            # Timeseries with the extracted scans corresponding to condition; set is used to remove overlapping TRs    
-            timeseries = timeseries[sorted(list(set(scan_list))),:]
-        else:
-            if censor:
-                timeseries = np.delete(timeseries, censor_volumes, axis=0)
-
-        if timeseries.shape[0] == 0:
-            warnings.warn(f"Subject {subj_id} timeseries is empty for {run}. Most likely due to condition not existing or TRs correspoonding to the condition being removed by `dummy_scans`.")
-        else:
-            subject_timeseries[subj_id].update({run_id: timeseries})
-    
-    if len(subject_timeseries[subj_id].keys()) == 0:
-        subject_timeseries = None
-
+def _extract_timeseries(subj_id, nifti_files, mask_files, event_files, confound_files, confound_metadata_files, run_list, tr, condition, parcel_approach, signal_clean_info, verbose, flush_print):
+
+    from nilearn.maskers import NiftiLabelsMasker
+    from nilearn.image import index_img, load_img
+    import copy, json, math, numpy as np, pandas as pd, warnings
+
+    # Intitialize subject dictionary
+    subject_timeseries = {subj_id: {}}
+    
+    for run in run_list:
+
+        run_id = "run-1" if run == None else run
+        run = run if run != None else ""
+
+        # Get files from specific run
+        nifti_file = [nifti_file for nifti_file in nifti_files if run in nifti_file.split("/")[-1]]
+        if len(mask_files) != 0:
+            mask_file = [mask_file for mask_file in mask_files if run in mask_file.split("/")[-1]]
+        else:
+            mask_file = []
+        confound_file = [confound_file for confound_file in confound_files if run in confound_file.split("/")[-1]] if signal_clean_info["use_confounds"] else None
+        confound_metadata_file = [confound_metadata_file for confound_metadata_file in confound_metadata_files if run in confound_metadata_file.split("/")[-1]] if signal_clean_info["use_confounds"] and signal_clean_info["n_acompcor_separate"] else None
+
+        if verbose: print(f"Running subject: {subj_id}; run: {run_id}; \n {nifti_file}", flush=flush_print)
+
+        confound_df = pd.read_csv(confound_file[0], sep="\t") if signal_clean_info["use_confounds"] else None
+
+        event_file = None if len(event_files) == 0 else [event_file for event_file in event_files if run in event_file.split("/")[-1]]
+
+        # Extract confound information of interest and ensure confound file does not contain NAs
+        if signal_clean_info["use_confounds"]:
+            # Extract first "n" numbers of specified WM and CSF components
+            confound_names = copy.deepcopy(signal_clean_info["confound_names"])
+            if confound_metadata_file:
+                with open(confound_metadata_file[0]) as foo:
+                    confound_metadata = json.load(foo)
+            
+                acompcors = sorted([acompcor for acompcor in confound_metadata.keys() if "a_comp_cor" in acompcor])
+
+                acompcors_CSF = [acompcor_CSF for acompcor_CSF in acompcors if confound_metadata[acompcor_CSF]["Mask"] == "CSF"][0:signal_clean_info["n_acompcor_separate"]]
+                acompcor_WM = [acompcor_WM for acompcor_WM in acompcors if confound_metadata[acompcor_WM]["Mask"] == "WM"][0:signal_clean_info["n_acompcor_separate"]]
+                
+                confound_names.extend(acompcors_CSF + acompcor_WM)
+
+            valid_confounds = []
+            invalid_confounds = []
+            for confound_name in confound_names:
+                if "*" in confound_name:
+                    prefix = confound_name.split("*")[0]
+                    confounds_list = [col for col in confound_df.columns if col.startswith(prefix)]
+                else:
+                    confounds_list = [col for col in confound_df.columns if col == confound_name] 
+            
+                if len(confounds_list) > 0: valid_confounds.extend(confounds_list)
+                else: invalid_confounds.extend([confound_name])
+
+            if len(invalid_confounds) > 0: 
+                if verbose: print(f"Subject {subj_id} did not have the following confounds: {invalid_confounds}", flush=flush_print)
+
+            confounds = confound_df[valid_confounds]
+            confounds = confounds.fillna(0)
+
+            if signal_clean_info["fd_threshold"]: 
+                censor = True
+                if "framewise_displacement" in confound_df.columns:
+                    fd_array = confound_df["framewise_displacement"].fillna(0).values
+                else:
+                    censor = False
+                    warnings.warn(f"For subject {subj_id}, `fd_threshold` specified but 'framewise_displacement' is not a column in the confound dataframe so removal of volumes after nuisance regression will not be done.")
+            else:
+                censor = False
+
+            if verbose: print(f"Confounds used for subject: {subj_id}; run: {run_id} - {confounds.columns}", flush=flush_print)
+
+        # Create the masker for extracting time series
+        if len(mask_file) !=0:
+            masker = NiftiLabelsMasker(
+                mask_img=mask_file[0],
+                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
+                resampling_target='data',
+                standardize=signal_clean_info["standardize"],
+                detrend=signal_clean_info["detrend"],
+                low_pass=signal_clean_info["low_pass"],
+                high_pass=signal_clean_info["high_pass"],
+                t_r=tr,
+                smoothing_fwhm=signal_clean_info["fwhm"]
+            )
+        else:
+            masker = NiftiLabelsMasker(
+                labels_img=parcel_approach[list(parcel_approach.keys())[0]]["maps"], 
+                resampling_target='data',
+                standardize=signal_clean_info["standardize"],
+                detrend=signal_clean_info["detrend"],
+                low_pass=signal_clean_info["low_pass"],
+                high_pass=signal_clean_info["high_pass"],
+                t_r=tr,
+                smoothing_fwhm=signal_clean_info["fwhm"]
+            )
+        # Load and discard volumes if needed
+        nifti_img = load_img(nifti_file[0])
+        if signal_clean_info["dummy_scans"]: 
+            nifti_img = index_img(nifti_img, slice(signal_clean_info["dummy_scans"], None))
+            if signal_clean_info["use_confounds"]: 
+                confounds.drop(list(range(0,signal_clean_info["dummy_scans"])),axis=0,inplace=True)
+                # Truncate the fd_array also
+                if censor:
+                    fd_array = fd_array[signal_clean_info["dummy_scans"]:]
+            offset = signal_clean_info["dummy_scans"] 
+
+        # Extract timeseries
+        timeseries = masker.fit_transform(nifti_img, confounds=confounds) if signal_clean_info["use_confounds"] else masker.fit_transform(nifti_img)
+
+        if censor:
+            censor_volumes = list(np.where(fd_array > signal_clean_info["fd_threshold"])[0])
+
+        if event_file:
+            event_df = pd.read_csv(event_file[0], sep=None)
+            # Get specific timing information for specific condition
+            condition_df = event_df[event_df["trial_type"] == condition] 
+
+            # Empty list for scans
+            scan_list = []
+
+            # Convert times into scan numbers to obtain the scans taken when the participant was exposed to the condition of interest; include partial scans
+            for i in condition_df.index:
+                onset_scan, duration_scan = int(condition_df.loc[i,"onset"]/tr), math.ceil((condition_df.loc[i,"onset"] + condition_df.loc[i,"duration"])/tr)
+                if signal_clean_info["dummy_scans"]:
+                    scan_list.extend([scan - offset for scan in range(onset_scan, duration_scan + 1) if scan not in range(0, signal_clean_info["dummy_scans"])])
+                else:
+                    scan_list.extend(list(range(onset_scan, duration_scan + 1)))
+                if censor:
+                    scan_list = [volume for volume in scan_list if volume not in censor_volumes]
+
+            # Timeseries with the extracted scans corresponding to condition; set is used to remove overlapping TRs    
+            timeseries = timeseries[sorted(list(set(scan_list))),:]
+        else:
+            if censor:
+                timeseries = np.delete(timeseries, censor_volumes, axis=0)
+
+        if timeseries.shape[0] == 0:
+            warnings.warn(f"Subject {subj_id} timeseries is empty for {run}. Most likely due to condition not existing or TRs correspoonding to the condition being removed by `dummy_scans`.")
+        else:
+            subject_timeseries[subj_id].update({run_id: timeseries})
+    
+    if len(subject_timeseries[subj_id].keys()) == 0:
+        subject_timeseries = None
+
     return subject_timeseries
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py` & `neurocaps-0.9.0.post5/neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,65 +1,65 @@
-import numpy as np
-from ._check_parcel_approach import _check_parcel_approach
-# A class which is responsible for acessing all TimeseriesExtractorGetter and to keep track of all attributes in TimeSeriesExtractor
-class _TimeseriesExtractorGetter:
-    def __init__(self):
-        pass
-    
-    #### Exists upon initialization of TimeseriesExtractor
-    @property
-    def space(self):
-        return self._space
-    
-    @property
-    def signal_clean_info(self):
-        return self._signal_clean_info
-    
-    @property
-    def parcel_approach(self):
-        return self._parcel_approach
-    
-    @parcel_approach.setter
-    def parcel_approach(self, parcel_dict):
-        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_dict, call="setter")
-
-    ### Does not exists upon initialization of Timeseries Extractor
-
-    # Exist when TimeSeriesExtractor.get_bold() used
-    @property
-    def task_info(self):
-        if hasattr(self, "_task_info"): return self._task_info
-        else: return None
-    
-    # Gets initialized and populated in TimeSeriesExtractor.get_bold(), 
-    @property
-    def subject_ids(self):
-        if hasattr(self, "_subject_ids"): return self._subject_ids
-        else: return None
-    
-    @property
-    def n_cores(self):
-        if hasattr(self, "_n_cores"): return self._n_cores
-        else: return None
-
-    # Gets initialized in TimeSeriesExtractor.get_bold(), gets populated when TimeseriesExtractor._timeseries_aggregator
-    # gets called in TimeseriesExtractor._extract_timeseries
-    @property
-    def subject_timeseries(self):
-        if hasattr(self, "_subject_timeseries"): return self._subject_timeseries
-        else: return None
-    
-    @subject_timeseries.setter
-    def subject_timeseries(self, subject_dict):
-        error_message = "Must be a nested dictionary where the first level is the subject id, second level is the run number in the form of 'run-#', and the final level is the timeseris as a numpy array."
-        if isinstance(subject_dict, dict): 
-            first_level_indx = list(subject_dict.keys())[0]
-            if isinstance(subject_dict[first_level_indx], dict) and len(subject_dict[first_level_indx].keys()) != 0 and "run" in list(subject_dict[first_level_indx].keys())[0]: 
-                run = list(subject_dict[first_level_indx].keys())[0]
-                if isinstance(subject_dict[first_level_indx][run],np.ndarray): 
-                    self._subject_timeseries = subject_dict
-                else: raise TypeError(error_message) 
-            else: raise TypeError(error_message) 
-        else: raise TypeError(error_message)
-    
-    
+import numpy as np
+from ._check_parcel_approach import _check_parcel_approach
+# A class which is responsible for acessing all TimeseriesExtractorGetter and to keep track of all attributes in TimeSeriesExtractor
+class _TimeseriesExtractorGetter:
+    def __init__(self):
+        pass
+    
+    #### Exists upon initialization of TimeseriesExtractor
+    @property
+    def space(self):
+        return self._space
+    
+    @property
+    def signal_clean_info(self):
+        return self._signal_clean_info
+    
+    @property
+    def parcel_approach(self):
+        return self._parcel_approach
+    
+    @parcel_approach.setter
+    def parcel_approach(self, parcel_dict):
+        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_dict, call="setter")
+
+    ### Does not exists upon initialization of Timeseries Extractor
+
+    # Exist when TimeSeriesExtractor.get_bold() used
+    @property
+    def task_info(self):
+        if hasattr(self, "_task_info"): return self._task_info
+        else: return None
+    
+    # Gets initialized and populated in TimeSeriesExtractor.get_bold(), 
+    @property
+    def subject_ids(self):
+        if hasattr(self, "_subject_ids"): return self._subject_ids
+        else: return None
+    
+    @property
+    def n_cores(self):
+        if hasattr(self, "_n_cores"): return self._n_cores
+        else: return None
+
+    # Gets initialized in TimeSeriesExtractor.get_bold(), gets populated when TimeseriesExtractor._timeseries_aggregator
+    # gets called in TimeseriesExtractor._extract_timeseries
+    @property
+    def subject_timeseries(self):
+        if hasattr(self, "_subject_timeseries"): return self._subject_timeseries
+        else: return None
+    
+    @subject_timeseries.setter
+    def subject_timeseries(self, subject_dict):
+        error_message = "Must be a nested dictionary where the first level is the subject id, second level is the run number in the form of 'run-#', and the final level is the timeseris as a numpy array."
+        if isinstance(subject_dict, dict): 
+            first_level_indx = list(subject_dict.keys())[0]
+            if isinstance(subject_dict[first_level_indx], dict) and len(subject_dict[first_level_indx].keys()) != 0 and "run" in list(subject_dict[first_level_indx].keys())[0]: 
+                run = list(subject_dict[first_level_indx].keys())[0]
+                if isinstance(subject_dict[first_level_indx][run],np.ndarray): 
+                    self._subject_timeseries = subject_dict
+                else: raise TypeError(error_message) 
+            else: raise TypeError(error_message) 
+        else: raise TypeError(error_message)
+    
+
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/analysis/cap.py` & `neurocaps-0.9.0.post5/neurocaps/analysis/cap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,883 +1,900 @@
-import numpy as np, re, warnings
-from kneed import KneeLocator
-from sklearn.cluster import KMeans
-from typing import Union
-from .._utils import _CAPGetter, _convert_pickle_to_dict, _check_parcel_approach
-
-
-class CAP(_CAPGetter):
-    def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
-        """
-        Initialize the CAP (Co-activation Patterns) analysis class.
-
-        Parameters
-        ----------
-        node_labels : list[str]
-            Decoded or non-decoded Schaefer Atlas labels for the nodes.
-        n_clusters : int or list[int], default=5
-            The number of clusters to use. Can be a single integer or a list of integers.
-        cluster_selection_method: str, default=None
-            Method to find the optimal number of clusters. Options are "silhouette" or "elbow".
-        groups : dict, default=None
-            A mapping of group names to subject IDs. Each group contains subject IDs for
-            separate CAP analysis. If None, CAPs are not separated by group.
-
-        Raises
-        ------
-        ValueError
-            If `cluster_selection_method` is none when `n_clusters` is a list.
-        ValueError
-            If `cluster_selection_method` is used when `n_clusters` is a single integer.
-        TypeError
-            If `groups` is provided but is not a dictionary.
-        AssertionError
-            If any group in `groups` has zero subject IDs.
-
-        Notes
-        -----
-        The initialization ensures unique values if `n_clusters` is a list and checks for 
-        valid input types and values.
-        """
-        # Ensure all unique values if n_clusters is a list
-        self._n_clusters = n_clusters if type(n_clusters) == int else sorted(list(set(n_clusters)))
-        self._cluster_selection_method = cluster_selection_method 
-
-        if type(n_clusters) == list:
-            self._n_clusters =  self._n_clusters[0] if all([type(self._n_clusters) == list, len(self._n_clusters) == 1]) else self._n_clusters
-            # Raise error if n_clusters is a list and no cluster selection method is specified
-            if all([len(n_clusters) > 1, self._cluster_selection_method== None]):
-                raise ValueError("`cluster_selection_method` cannot be None since n_clusters is a list.")
-
-        # Raise error if silhouette_method is requested when n_clusters is an integer
-        if all([self._cluster_selection_method != None, type(self._n_clusters) == int]):
-            raise ValueError("`cluster_selection_method` only valid if n_clusters is a range of unique integers.")
-       
-        self._groups = groups
-        # Raise error if self groups is not a dictionary 
-        if self._groups:
-            if type(self._groups) != dict:
-                raise TypeError("`groups` must be a dictionary where the keys are the group names and the items correspond to subject ids in the groups.")
-            
-            for group_name in self._groups.keys():
-                assert len(self._groups[group_name]) > 0, f"{group_name} has zero subject ids."
-            
-            # Convert ids to strings
-            for group in self._groups.keys():
-                self._groups[group] = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in self._groups[group]]
-        
-        valid_parcel_dict = {"Schaefer", "AAL", "Custom"}
-
-        if len(parcel_approach.keys()) > 1:
-            raise ValueError(f"Only one parcellation approach can be selected from the following valid options: {valid_parcel_dict.keys()}.\n Example format of `parcel_approach`: {valid_parcel_dict}")
-        
-        self._parcel_approach = parcel_approach 
-
-    def get_caps(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], runs: Union[int, list[int]]=None, random_state: int=None, show_figs: bool=True, standardize: bool=True, epsilon: Union[int,float]=0, **kwargs) -> None:
-        """"" Create CAPs
-
-        The purpose of this function is to concatenate the timeseries of each subject and perform kmeans clustering on the concatenated data.
-        
-        Parameters
-        ----------
-        subject_timeseries: dict or str
-            A pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
-            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-            must consist of the timeseries associated with that run.
-        runs: int or list[int], default=None
-            The run numbers to perform the CAPs analysis with. If None, all runs in the subject timeseries will be concatenated into a single dataframe.
-        random_state: int, default=None
-            The random state to use for scikits KMeans function.
-        show_figs: bool, default=True
-            Display the plots of inertia scores for all groups if `cluster_selection_method`="elbow".
-        standardize: bool, default=True
-            To z-score the features of the concatonated timeseries array.
-        epsilon: int or float, default=0
-            Small number to add to the denominator when z-scoring for numerical stabilty.
-        kwargs: dect
-            Dictionary to adjust the sensitivity, `S` parameter, of the elbow method. The elbow method uses the KneeLocator function from the  kneed package. If no `S` is inputted, `S` will be KneeLocator default.
-            Larger values of `S` are more conservative and less sensitive to small fluctuations.
-            
-        Raises
-        ------
-        ValueError
-            If both input_path and subject_timeseries are None.
-        """
-        
-        if runs:
-            if isinstance(runs,int): runs = list(runs)
-    
-        self._runs = runs if runs else "all"
-        self._standardize = standardize
-        self._epsilon = epsilon
-
-        if isinstance(subject_timeseries, str) and "pkl" in subject_timeseries: subject_timeseries = _convert_pickle_to_dict(pickle_file=subject_timeseries)
-
-        self._concatenated_timeseries = self._get_concatenated_timeseries(subject_timeseries=subject_timeseries, runs=runs)
-
-        if self._cluster_selection_method == "silhouette": 
-            self._perform_silhouette_method(random_state=random_state)
-        elif self._cluster_selection_method == "elbow":
-            self._perform_elbow_method(random_state=random_state, show_figs=show_figs, **kwargs)
-        else:
-            self._kmeans = {}
-            for group in self._groups.keys():
-                self._kmeans[group] = {}
-                self._kmeans[group] = KMeans(n_clusters=self._n_clusters,random_state=random_state).fit(self._concatenated_timeseries[group]) if random_state or random_state == 0 else KMeans(n_clusters=self._n_clusters).fit(self._concatenated_timeseries[group])
-            
-        # Create states dict   
-        self._create_caps_dict()
-    
-    def _perform_silhouette_method(self, random_state):
-        from sklearn.metrics import silhouette_score
-
-        # Initialize attribute
-        self._silhouette_scores = {}
-        self._optimal_n_clusters = {}
-        self._kmeans = {}
-
-        for group in self._groups.keys():
-            self._silhouette_scores[group] = {}
-            for n_cluster in self._n_clusters:
-                self._kmeans[group] = KMeans(n_clusters=n_cluster,random_state=random_state).fit(self._concatenated_timeseries[group]) if random_state or random_state == 0 else KMeans(n_clusters=n_cluster).fit(self._concatenated_timeseries[group])
-                cluster_labels = self._kmeans[group].predict(self._concatenated_timeseries[group])
-                self._silhouette_scores[group].update({n_cluster: silhouette_score(self._concatenated_timeseries[group], cluster_labels)})
-            self._optimal_n_clusters[group] = max(self._silhouette_scores[group], key=self._silhouette_scores[group].get)
-            if self._optimal_n_clusters[group] != self._n_clusters[-1]:
-                self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group],random_state=random_state).fit(self._concatenated_timeseries[group]) if random_state or random_state == 0 else KMeans(n_clusters=self._optimal_n_clusters[group]).fit(self._concatenated_timeseries[group])
-            print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.")
-        
-    
-    def _perform_elbow_method(self, random_state, show_figs, **kwargs):
-        # Initialize attribute
-        self._inertia = {}
-        self._optimal_n_clusters = {}
-        self._kmeans = {}
-
-        knee_dict = dict(S = kwargs["S"] if "S" in kwargs.keys() else 1)
-
-        for group in self._groups.keys():
-            self._inertia[group] = {}
-            for n_cluster in self._n_clusters:
-                self._kmeans[group] = KMeans(n_clusters=n_cluster,random_state=random_state).fit(self._concatenated_timeseries[group]) if random_state or random_state == 0 else KMeans(n_clusters=n_cluster).fit(self._concatenated_timeseries[group])
-                self._inertia[group].update({n_cluster: self._kmeans[group].inertia_}) 
-            
-            # Get optimal cluster size
-            kneedle = KneeLocator(x=list(self._inertia[group].keys()), 
-                                                        y=list(self._inertia[group].values()),
-                                                        curve='convex',
-                                                        direction='decreasing', S=knee_dict["S"])
-                
-            self._optimal_n_clusters[group] = kneedle.elbow
-            if not self._optimal_n_clusters[group]:
-                 warnings.warn("No elbow detected so optimal cluster size is None. Try adjusting the sensitivity parameter, `S`, to increase or decrease sensitivity (higher values are less sensitive), expanding the list of clusters to test, or setting `cluster_selection_method` to 'sillhouette'.")
-            else:
-                if self._optimal_n_clusters[group] != self._n_clusters[-1]:
-                    self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group],random_state=random_state).fit(self._concatenated_timeseries[group]) if random_state or random_state == 0 else KMeans(n_clusters=self._optimal_n_clusters[group]).fit(self._concatenated_timeseries[group])
-                print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.\n")
-
-                if show_figs:
-                    kneedle.plot_knee(title=group)
-                    kneedle.plot_knee_normalized(title=group)
-
-    def _create_caps_dict(self):
-        # Initialize dictionary
-        self._caps = {}
-        for group in self._groups.keys():
-                self._caps[group] = {}
-                self._caps[group].update({f"CAP-{state_number}": state_vector for state_number, state_vector in zip([num for num in range(1,len(self._kmeans[group].cluster_centers_)+1)],self._kmeans[group].cluster_centers_)})
-    
-    def _get_concatenated_timeseries(self, subject_timeseries, runs):
-        # Create dictionary for "All Subjects" if no groups are specified to reuse the same loop instead of having to create logic for grouped and non-grouped version of the same code
-        if not self._groups: self._groups = {"All Subjects": [subject for subject in subject_timeseries.keys()]}
-
-        concatenated_timeseries = {group: {} for group in self._groups.keys()}
-
-        self._generate_lookup_table()
-
-        self._mean_vec = {group: {} for group in self._groups.keys()}
-        self._stdev_vec = {group: {} for group in self._groups.keys()}
-
-        for subj_id, group in self._subject_table.items():
-            requested_runs = [f"run-{run}" for run in runs] if runs else subject_timeseries[subj_id].keys()
-            subject_runs = [subject_run for subject_run in subject_timeseries[subj_id].keys() if subject_run in requested_runs] 
-            if len(subject_runs) == 0:
-                warnings.warn(f"Skipping subject {subj_id} since they do not have the requested run numbers {','.join(requested_runs)}")
-                continue
-            for curr_run in subject_runs:
-                if len(concatenated_timeseries[group]) == 0:
-                    concatenated_timeseries[group] = subject_timeseries[subj_id][curr_run] if subj_id in list(set(self._groups[group])) else concatenated_timeseries[group]
-                else:
-                    concatenated_timeseries[group] = np.vstack([concatenated_timeseries[group], subject_timeseries[subj_id][curr_run]]) if subj_id in list(set(self._groups[group])) else concatenated_timeseries[group]
-        # Standardize
-        if self._standardize:
-            for group in self._groups.keys():
-                self._mean_vec[group], self._stdev_vec[group] = np.mean(concatenated_timeseries[group], axis=0), np.std(concatenated_timeseries[group], ddof=1, axis=0)
-                concatenated_timeseries[group] = (concatenated_timeseries[group] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon)
-
-        return concatenated_timeseries
-    
-    def _generate_lookup_table(self):
-        self._subject_table = {}
-        for group in self._groups:
-            for subj_id in self._groups[group]:
-                if subj_id in self._subject_table.keys():
-                    warnings.warn(f"Subject: {subj_id} appears more than once, only including the first instance of this subject in the analysis.") 
-                else:
-                    self._subject_table.update({subj_id : group})
-
-    def visualize_caps(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
-        """ Plotting CAPs
-
-        This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
-
-        Parameters
-        ----------
-        output_dir: str, default=None
-            Directory to save plots in. If None, plots will not be saved.
-        plot_options: str or list[str], default="outer product"
-            Type of plots to create. Options are "outer product" or "heatmap".
-        visual_scope: str or list[str], default="regions"
-            Determines whether plotting is done at the region level or node level. 
-            For region level, the value of each nodes in the same regions are averaged together them plotted.
-            Options are "regions" or "nodes".
-        task_title: str, default=None
-            Serves as the title of each plot as well as the name of the saved file if output_dir is given.
-        show_figs: bool, default=True
-            Display figures or not to display figures.
-        subplots: bool, default=True
-            Produce subplots for outer product plots.
-        kwargs: dict
-            Keyword arguments used when saving figures. Valid keywords include "dpi", "format", "figsize", "fontsize", "hspace", "wspace", "xticklabels_size", "yticklabels_size", "shrink", "nrow", "ncol", "suptitle_fontsize", "tight_layout", "rect", "sharey", "xlabel_rotation", "ylabel_rotation", "annot". 
-            If `output_dir` is not None and no inputs for dpi and format are given, dpi defaults to 300 and format defaults to "png". If no keywords, "figsize" defaults to (8,6), "fontsize", which adjusts the title size of the individual plots or subplots, defaults to 14, "hspace", which adjusts spacing for subplots, defaults to 0.4, 
-            "wspace", which adjusts spacing between subplots, defaults to 0.4, "xticklabels_size" defaults to 8, "yticklabels_size" defaults to 8, shrink, which adjusts the cbar size, defaults to 0.8, "nrow", which is the number of rows for subplot and varies, and "ncol", which is the number of columns for subplot, default varies but max is 5, "suptitle_fontsize", 
-            size of the main title when subplot is True, defaults to 0.7, "tight_layout", use tight layout for subplot, defaults to True, "rect", input for the `rect` parameter in tight layout when subplots is True to fix whitespace issues, default is [0, 0.03, 1, 0.95], "sharey", which shares y axis labela for subplots, defaults to True, 
-            "xlabel_rotation", which rotates the labels on the x-axis, defaults to 0, "ylabel_rotation", which rotates the labels on the y-axis, defaults to 0, "annot", which adds values to cells on the outer product heatmap at the region level only, defaults to False, "linewidths", which specifies the padding between each cell, defaults to 0,
-            and "cmap", which specifies the color pattern of the cells in the plot, defaults to "coolwarm".
-    
-         Notes
-        -----
-        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
-        the zero index should correspond the first id that is not zero.
-
-        Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
-        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
-          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
-          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
-        
-        Example 
-        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
-
-        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                             "regions": {"Vis" : {"lh": [0,1],
-                                                  "rh": [3,4]},
-                                         "Hippocampus": {"lh": [2],
-                                                         "rh": [5]}}}}
-        """
-        import itertools, os
-
-        # Check parcel approach
-
-        # Check if parcellation_approach is custom
-        if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
-            _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_caps")
-
-        # Check labels
-        check_caps = self._caps[list(self._caps.keys())[0]]
-        check_caps = check_caps[list(check_caps.keys())[0]]
-        if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]): 
-                raise ValueError("Number of rois/nodes used for CAPs does not equal the number of rois/nodes specified in `parcel_approach`.")
-
-        if output_dir:
-            if not os.path.exists(output_dir):
-                os.makedirs(output_dir)
-
-        # Convert to list
-        if type(plot_options) == str: plot_options = [plot_options]
-        if type(visual_scope) == str: visual_scope = [visual_scope]
-
-        # Check inputs for plot_options and visual_scope
-        if not any(["heatmap" in plot_options, "outer product" in plot_options]):
-            raise ValueError("Valid inputs for `plot_options` are 'heatmap' and 'outer product'.")
-        
-        if not any(["regions" in visual_scope, "nodes" in visual_scope]):
-            raise ValueError("Valid inputs for `visual_scope` are 'regions' and 'nodes'.")
-
-        if "regions" in visual_scope: self._create_regions()
-
-        # Create plot dictionary
-        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                        format = kwargs["format"] if kwargs and "format" in kwargs.keys() else "png",
-                        figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
-                        fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
-                        hspace = kwargs["hspace"] if kwargs and "hspace" in kwargs.keys() else 0.2,
-                        wspace = kwargs["wspace"] if kwargs and "wspace" in kwargs.keys() else 0.2,
-                        xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
-                        yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
-                        shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
-                        nrow = kwargs["nrow"] if kwargs and "nrow" in kwargs.keys() else None,
-                        ncol = kwargs["ncol"] if kwargs and "ncol" in kwargs.keys() else None,
-                        suptitle_fontsize = kwargs["suptitle_fontsize"] if kwargs and "suptitle_fontsize" in kwargs.keys() else 20,
-                        tight_layout = kwargs["tight_layout"] if kwargs and "tight_layout" in kwargs.keys() else True,
-                        rect = kwargs["rect"] if kwargs and "rect" in kwargs.keys() else [0, 0.03, 1, 0.95],
-                        sharey = kwargs["sharey"] if kwargs and "sharey" in kwargs.keys() else True,
-                        xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
-                        ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
-                        annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
-                        linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
-                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
-                        )
-        
-        if kwargs:
-            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
-            if len(invalid_kwargs.keys()) > 0:
-                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
-
-        # Ensure plot_options and visual_scope are lists
-        plot_options = plot_options if type(plot_options) == list else list(plot_options)
-        visual_scope = visual_scope if type(visual_scope) == list else list(visual_scope)
-        # Initialize outer product attribute
-        if "outer product" in plot_options: self._outer_product = {}
-
-        distributed_list = list(itertools.product(plot_options,visual_scope,self._groups.keys()))
-
-        for plot_option, scope, group in distributed_list:
-                # Get correct labels depending on scope
-                if scope == "regions": 
-                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
-                        cap_dict, columns = self._region_caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]
-                    else:
-                        cap_dict, columns = self._region_caps, list(self._parcel_approach["Custom"]["regions"].keys())
-                elif scope == "nodes": 
-                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
-                        cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]
-                    else:
-                        cap_dict, columns = self._caps , [x[0] + " " + x[1] for x in list(itertools.product(["LH", "RH"],self._parcel_approach["Custom"]["regions"].keys()))]
-
-                #  Generate plot for each group
-                if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
-                                                                                    output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
-                elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
-                                                                            output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
-            
-    def _create_regions(self):
-        self._region_caps = {group: {} for group in self._groups.keys()}
-        for group in self._groups.keys():
-            for cap in self._caps[group].keys():
-                region_caps = {}
-                if list(self._parcel_approach.keys())[0] != "Custom":
-                    for region in self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]:
-                        if len(region_caps) == 0:
-                            region_caps = np.array([np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
-                        else:
-                            region_caps = np.hstack([region_caps, np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
-                else:
-                    region_dict = self._parcel_approach["Custom"]["regions"]
-                    region_keys = region_dict.keys()
-                    for region in region_keys:
-                        roi_indxs = np.array(region_dict[region]["lh"] + region_dict[region]["rh"])
-
-                        if len(region_caps) == 0:
-                            region_caps= np.array([np.average(self._caps[group][cap][roi_indxs])])
-                        else:
-                            region_caps= np.hstack([region_caps, np.average(self._caps[group][cap][roi_indxs])])
-
-                self._region_caps[group].update({cap: region_caps})
-    
-    def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, task_title, show_figs, scope):
-        import matplotlib.pyplot as plt, os
-        from seaborn import heatmap
-
-        # Nested dictionary for group
-        self._outer_product[group] = {}
-
-        # Create base grid for subplots
-        if subplots:
-            # Max five subplots per row for default
-            default_col = len(cap_dict[group].keys()) if len(cap_dict[group].keys()) <= 5 else 5
-            ncol = plot_dict["ncol"] if plot_dict["ncol"] != None else default_col
-            # Pad nrow, since int will round down, padding is needed for cases where len(cap_dict[group].keys())/ncol is a float. This will add the extra row needed
-            x_pad = 0 if len(cap_dict[group].keys())/ncol <= 1 else 1
-            nrow = plot_dict["nrow"] if plot_dict["nrow"] != None else x_pad + int(len(cap_dict[group].keys())/ncol)
-
-            subplot_figsize = (8 * ncol, 6 * nrow) if plot_dict["figsize"] == (8,6) else plot_dict["figsize"] 
-
-            fig, axes = plt.subplots(nrow, ncol, sharex=False, sharey=plot_dict["sharey"], figsize=subplot_figsize)
-            suptitle = f"{group} {task_title}" if task_title else f"{group}"
-            fig.suptitle(suptitle, fontsize=plot_dict["suptitle_fontsize"])
-            fig.subplots_adjust(hspace=plot_dict["hspace"], wspace=plot_dict["wspace"])  
-            if plot_dict["tight_layout"]: fig.tight_layout(rect=plot_dict["rect"])  
-
-            # Current subplot
-            axes_x, axes_y = [0,0] 
-
-        # Iterate over CAPs
-        for cap in cap_dict[group].keys():
-            # Calculate outer product
-            self._outer_product[group].update({cap: np.outer(cap_dict[group][cap],cap_dict[group][cap])})
-            # Create labels if nodes requested for scope
-            if scope == "nodes":
-                import collections
-                
-                # Get frequency of each major hemisphere and region in Schaefer, AAL, or Custom atlas
-                if list(self._parcel_approach.keys())[0] == "Schaefer":
-                    frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
-                elif list(self._parcel_approach.keys())[0] == "AAL":
-                    frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
-                else:
-                    frequency_dict = {}
-                    for id in columns:
-                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
-                        region_id = re.split("LH |RH ", id)[-1]
-                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
-                # Get the names, which indicate the hemisphere and region
-                names_list = list(frequency_dict.keys())
-                # Create label list the same length as the labels dictionary and substitute each element with an empty string
-                labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
-
-                starting_value = 0
-
-                # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
-                for num, name in enumerate(names_list): 
-                    if num == 0:
-                        labels[0] = name
-                    else:
-                        # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
-                        starting_value += frequency_dict[names_list[num-1]] 
-                        labels[starting_value] = name
-
-            if subplots: 
-                ax = axes[axes_y] if nrow == 1 else axes[axes_x,axes_y]
-                # Modify tick labels based on scope
-                if scope == "regions":
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
-                else:
-                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={"shrink": plot_dict["shrink"]})
-
-                    ticks = [i for i, label in enumerate(labels) if label]  
-
-                    ax.set_xticks(ticks)  
-                    ax.set_xticklabels([label for label in labels if label]) 
-                    ax.set_yticks(ticks)  
-                    ax.set_yticklabels([label for label in labels if label]) 
-
-                # Modify label sizes
-                display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
-
-                if plot_dict["sharey"] == True:
-                    if axes_y == 0: display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
-                else:
-                    display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
-
-                # Set title of subplot
-                ax.set_title(cap, fontsize=plot_dict["fontsize"])
-
-                # If modulus is zero, move onto the new column back to zero
-                if (axes_y % ncol == 0 and axes_y != 0) or axes_y == ncol - 1: 
-                    axes_x += 1
-                    axes_y = 0
-                else:
-                    axes_y += 1
-
-            else:
-                # Create new plot for each iteration when not subplot
-                plt.figure(figsize=plot_dict["figsize"])
-
-                plot_title = f"{group} {cap} {task_title}" if task_title else f"{group} {cap}"
-                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
-                else: 
-                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
-                    ticks = [i for i, label in enumerate(labels) if label]  
-
-                    display.set_xticks(ticks)  
-                    display.set_xticklabels([label for label in labels if label]) 
-                    display.set_yticks(ticks)  
-                    display.set_yticklabels([label for label in labels if label]) 
-                
-                # Set title
-                display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
-
-                # Modify label sizes
-                display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
-                display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
-
-                # Save individual plots
-                if output_dir:
-                    partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
-                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
-                    display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
-        
-        # Remove subplots with no data
-        if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
-
-        # Save subplot
-        if subplots and output_dir: 
-            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
-            display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
-        
-        # Display figures
-        if not show_figs: plt.close()
-
-    def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
-        import matplotlib.pyplot as plt, os, pandas as pd
-        from seaborn import heatmap
-        
-        # Initialize new grid
-        plt.figure(figsize=plot_dict["figsize"])
-
-        if scope == "regions": 
-            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]}) 
-        else: 
-            # Create Labels
-            import collections
-            if list(self._parcel_approach.keys())[0] == "Schaefer":
-                frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
-            elif list(self._parcel_approach.keys())[0] == "AAL":
-                frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
-            else:
-                    frequency_dict = {}
-                    for id in columns:
-                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
-                        region_id = re.split("LH |RH ", id)[-1]
-                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
-            names_list = list(frequency_dict.keys())
-            labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
-
-            starting_value = 0
-
-            # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
-            for num, name in enumerate(names_list): 
-                if num == 0:
-                    labels[0] = name
-                else:
-                    # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
-                    starting_value += frequency_dict[names_list[num-1]] 
-                    labels[starting_value] = name
-
-            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]})
-
-            plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
-
-        # Modify label sizes
-        display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
-        display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
-
-        # Set plot name
-        plot_title = f"{group} CAPS {task_title}" if task_title else f"{group} CAPS" 
-        display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
-
-        # Save plots
-        if output_dir:
-            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
-            full_filename = f"{partial_filename}_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_heatmap-nodes.{plot_dict['format']}"
-            display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
-   
-        # Display figures
-        if not show_figs: plt.close()
-
-    def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, output_dir: str=None, file_name: str=None) -> dict:
-        """Get CAP metrics
-
-        Creates a single pandas Dataframe containing all participants containing CAP metrics as described in Liu et al., 2018 and Yang et al., 2021, where `temporal fraction` is the proportion of total volumes spent in a single CAP over all volumes in a run,
-        `persistence` is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and `counts` is the frequency of each CAP observed in a run, and `transition frequency` is the number of switches between
-        different CAPs across the entire run.
-
-        Parameters
-        ----------
-        subject_timeseries: dict or str
-            The absolute path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
-            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-            must consist of the timeseries associated with that run. This should be the same dictionary used for `get_caps()`.
-        tr: float, default=None
-            The repetition time. If given, persistence will be calculate as the average uninterrupted time spent in each CAP. If not give, persistence will be calculate
-            as the average uninterrupted volumes (TRs) spent in each state.
-        runs: int or list[int], default=None
-            The run numbers to calculate cap metrics for. If None, cap metrics will be calculated for each run.
-        continuous_runs: bool, default=False
-            If True, all runs will be treated as a single, uninterrupted run.
-        metrics : str or list[str], default=["temporal fraction", "persistence", "counts", "transition frequency"]
-            The metrics to calculate. Available options include `temporal fraction`, `persistence`, `counts`, and `transition frequency`.
-        return_df: str, default=True
-            If True, dataframe will be returned.
-        output_dir: str, default=None
-            Directory to save dataframe in. If None, dataframe will not be saved.
-        file_name: str, default=None
-            Name to save dataframe as if output_dir is not None.
-
-        Returns
-        -------
-        dictionary containing pandas dataframes - one for each metric requested.
-
-        Raises
-        ------
-        ValueError
-            No valid metrics are detected in `metrics` parameter.
-
-        Notes
-        -----
-        The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
-        a specific CAP.
-
-        References
-        -----
-        Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-        Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
-        NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-        """
-        import collections, os, pandas as pd
-
-        metrics = [metrics] if isinstance(metrics, str) else metrics
-
-        valid_metrics = ["temporal fraction", "persistence", "counts", "transition frequency"]
-
-        boolean_list = [element in valid_metrics for element in metrics]
-
-        if any(boolean_list):
-            invalid_metrics = [metrics[indx] for indx,boolean in enumerate(boolean_list) if boolean == False]
-            if len(invalid_metrics) > 0:
-                warnings.warn(f"invalid metrics will be ignored: {' '.join(invalid_metrics)}")
-        else:
-            raise ValueError(f"No valid metrics in `metrics` list. Valid metrics are {', '.join(valid_metrics)}")
-        
-        if isinstance(subject_timeseries, str) and "pkl" in subject_timeseries: subject_timeseries = _convert_pickle_to_dict(pickle_file=subject_timeseries)
-
-        group_cap_dict = {}
-        # Get group with most CAPs
-        for group in self._groups.keys():
-            group_cap_dict.update({group: len(self._caps[group])})
-        
-        cap_names =  self._caps[max(group_cap_dict, key=group_cap_dict.get)].keys()
-        cap_numbers = [int(name.split("-")[-1]) for name in cap_names]
-
-        # Assign each subject TRs to CAP
-        predicted_subject_timeseries = {}
-
-        for subj_id, group in self._subject_table.items():
-            predicted_subject_timeseries[subj_id] = {}
-            requested_runs = [f"run-{run}" for run in runs] if runs else subject_timeseries[subj_id].keys()
-            subject_runs = [subject_run for subject_run in subject_timeseries[subj_id].keys() if subject_run in requested_runs] 
-            if len(subject_runs) == 0:
-                warnings.warn(f"Skipping subject {subj_id} since they do not have the requested run numbers {','.join(requested_runs)}")
-                continue
-            if not continuous_runs or len(requested_runs) == 1:
-                for curr_run in subject_runs:
-                        timeseries = (subject_timeseries[subj_id][curr_run] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon) if self._standardize else subject_timeseries[subj_id][curr_run] 
-                        predicted_subject_timeseries[subj_id].update({curr_run: self._kmeans[group].predict(timeseries) + 1})
-            else:
-                subject_runs = "Continuous Runs"
-                timeseries = {subject_runs: {}}
-                for curr_run in subject_timeseries[subj_id].keys():
-                    timeseries[subject_runs] = np.vstack([timeseries[subject_runs], subject_timeseries[subj_id][curr_run]]) if len(timeseries[subject_runs]) != 0 else subject_timeseries[subj_id][curr_run]
-                timeseries = (timeseries[subject_runs] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon) if self._standardize else timeseries[subject_runs]
-                predicted_subject_timeseries[subj_id].update({subject_runs: self._kmeans[group].predict(timeseries) + 1})
-
-        # Create pd.dataframe
-        df_dict = {}
-
-        for metric in metrics: 
-            if metric in valid_metrics:
-                if metric != "transition frequency":
-                    df_dict.update({metric: pd.DataFrame(columns=["Subject_ID", "Group","Run"] + list(cap_names))})
-                else:
-                    df_dict.update({metric: pd.DataFrame(columns=["Subject_ID", "Group","Run","Transition_Frequency"])})
-
-        distributed_list = []
-        for subj_id, group in self._subject_table.items():
-            for curr_run in predicted_subject_timeseries[subj_id].keys():
-                distributed_list.append([subj_id,group,curr_run])
-
-        for subj_id, group, curr_run in distributed_list:
-            if "temporal fraction" in metrics or "counts" in metrics:
-                frequency_dict = dict(collections.Counter(predicted_subject_timeseries[subj_id][curr_run]))
-                sorted_frequency_dict = {key: frequency_dict[key] for key in sorted(list(frequency_dict.keys()))}
-                if len(sorted_frequency_dict) != len(cap_numbers):
-                    sorted_frequency_dict = {cap_number: sorted_frequency_dict[cap_number] if cap_number in sorted_frequency_dict.keys() else 0 for cap_number in cap_numbers}
-                if "temporal fraction" in metrics: 
-                    proportion_dict = {key: item/(len(predicted_subject_timeseries[subj_id][curr_run])) for key, item in sorted_frequency_dict.items()}
-                    # Populate Dataframe
-                    df_dict["temporal fraction"].loc[len(df_dict["temporal fraction"])] = [subj_id, group, curr_run] + [items for _ , items in proportion_dict.items()]
-                if "counts" in metrics:
-                    # Populate Dataframe
-                    df_dict["counts"].loc[len(df_dict["counts"])] = [subj_id, group, curr_run] + [items for _ , items in sorted_frequency_dict.items()]
-            if "persistence" in metrics:
-                # Initialize variable
-                persistence_dict = {}
-                uninterrupted_volumes = []
-                count = 0
-
-                # Iterate through caps
-                for target in cap_numbers:
-                    # Iterate through each element and count uniterrupted volumes that equal target
-                    for index in range(0,len(predicted_subject_timeseries[subj_id][curr_run])):
-                        if predicted_subject_timeseries[subj_id][curr_run][index] == target:
-                            count +=1
-                        # Store count in list if interuptted and not zero an
-                        else:
-                            if count != 0:
-                                uninterrupted_volumes.append(count)
-                            # Reset counter 
-                            count = 0
-                    # In the event, a participant only occupies one CAP and to ensure final counts are added
-                    if count > 0:
-                        uninterrupted_volumes.append(count)
-                    # If uninterrupted_volumes not zero, multiply elements in the list by repetition time, sum and divide
-                    if len(uninterrupted_volumes) > 0:
-                        if tr:
-                            persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes)*tr)/(len(uninterrupted_volumes))})
-                        else:
-                            persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes))/(len(uninterrupted_volumes))})
-                    else:
-                        persistence_dict.update({target: 0})
-                    # Reset variables
-                    count = 0
-                    uninterrupted_volumes = []
-                # Populate Dataframe
-                df_dict["persistence"].loc[len(df_dict["persistence"])] = [subj_id, group, curr_run] + [items for _ , items in persistence_dict.items()]
-            if "transition frequency" in metrics:
-                count = 0
-                # Iterate through predicted values 
-                for index in range(0,len(predicted_subject_timeseries[subj_id][curr_run])):
-                    if index != 0:
-                        # If the subsequent element does not equal the previous element, this is considered a transition
-                        if predicted_subject_timeseries[subj_id][curr_run][index-1] != predicted_subject_timeseries[subj_id][curr_run][index]:
-                            count +=1
-                df_dict["transition frequency"].loc[len(df_dict["transition frequency"])] = [subj_id, group, curr_run, count]
-
-        if output_dir:
-            for metric in df_dict.keys():
-                filename = file_name + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
-                df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
-
-        if return_df:
-            return df_dict
-        
-    def caps2surf(self, output_dir: str=None, show_figs: bool = True, fwhm: float=None, 
-                  fslr_density: str="32k", method: str="linear", return_stat_map: bool = False, **kwargs):
-        """Project CAPs back onto atlas used for spatial dimensionality reduction for visualization
-        
-        Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
-        This function uses surfplot for surface plotting.
-
-        Parameters
-        ----------
-        output_dir: str, default=None
-            Directory to save plots in. If None, plots will not be saved.
-        show_figs: bool, default=True
-            Display figures or not to display figures.
-        fwhm: float, defualt=None
-            Strength of spatial smoothing to apply in millimeters.
-        fslr_density: str, default="32k"
-            Density of the fslr surface when converting from mni 152 space to fslr surface. Options are 
-            "32k" or "164k".
-        method: str, default="linear"
-            Interpolation method to use when converting from mni152 space to fslr surface. Options are "linear"
-            or "nearest".
-        return_stat_map: bool, default=FAlse
-            Returns the atlas as a stat map.
-        **kwargs: dict
-            Additional parameters to pass to modify certain plot parameters. Options include "dpi", defaults to 300, "title_pad", defaults to -3,
-            "cmap", defaults to "cold_hot", "cbar_location", defaults to "bottom", "cbar_draw_border", defaults to False, "cbar_aspect", defaults to 10, "cbar_shrink", defaults 
-            to 0.2, "cbar_decimals", defaults to 0, and "cbar_pad", defaults to 0.
-            
-        Returns
-        -------
-        Nifti Stat map
-
-        Notes
-        -----
-        Assumes that atlas background label is zero and atlas is in MNI space. Also assumes that the indices from the cluster centroids are related
-        to the atlas by an offset of one. For instance, index 0 of the cluster centroid vector is the first nonzero label, which is assumed to be at the 
-        first index of the array in sorted(np.unique(atlas_fdata)).
-
-        Using fwhm to adjust smooting may help coverage issues.
-
-        """
-
-        import nibabel as nib, numpy as np, os
-        from nilearn import image
-        from nilearn.plotting.cm import _cmap_d 
-        from neuromaps.transforms import mni152_to_fslr
-        from neuromaps.datasets import fetch_fslr
-        from surfplot import Plot
-
-        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                         title_pad = kwargs["title_pad"] if kwargs and "title_pad" in kwargs.keys() else -3,
-                         cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "cold_hot",
-                         cbar_location = kwargs["cbar_location"] if kwargs and "cbar_location" in kwargs.keys() else "bottom",
-                         cbar_draw_border = kwargs["cbar_draw_border"] if kwargs and "cbar_draw_border" in kwargs.keys() else False,
-                         cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 10,
-                         cbar_shrink = kwargs["cbar_shrink"] if kwargs and "cbar_shrink" in kwargs.keys() else 0.2,
-                         cbar_decimals = kwargs["cbar_decimals"] if kwargs and "cbar_decimals" in kwargs.keys() else 0,
-                         cbar_pad = kwargs["cbar_pad"] if kwargs and "cbar_pad" in kwargs.keys() else 0)
-        
-        if kwargs:
-            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
-            if len(invalid_kwargs.keys()) > 0:
-                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
-
-        for group in self._caps.keys():
-            for cap in self._caps[group].keys():
-                atlas = nib.load(self._parcel_approach[list(self._parcel_approach.keys())[0]]["maps"])
-                atlas_fdata = atlas.get_fdata()
-                # Get array containing all labels in atlas to avoid issue if atlas labels dont start at 1, like Nilearn's AAL map
-                target_array = sorted(np.unique(atlas_fdata))
-                for indx, value in enumerate(self._caps[group][cap]):
-                    actual_indx = indx + 1
-                    atlas_fdata[np.where(atlas_fdata == target_array[actual_indx])] = value
-                stat_map = nib.Nifti1Image(atlas_fdata, atlas.affine, atlas.header)
-                # Add smoothing to stat map to help mitigate potential coverage issues 
-                if fwhm != None:
-                    stat_map = image.smooth_img(stat_map, fwhm=fwhm)
-
-                # Code slightly adapted from surfplot example 2
-                gii_lh, gii_rh = mni152_to_fslr(stat_map, method=method, fslr_density=fslr_density)
-                surfaces = fetch_fslr()
-                lh, rh = surfaces['inflated']
-                lh = str(lh) if not isinstance(lh, str) else lh
-                rh = str(rh) if not isinstance(rh, str) else rh
-                sulc_lh, sulc_rh = surfaces['sulc']
-                sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
-                sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
-                p = Plot(lh, rh)
-
-                # Add base layer
-                p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
-
-                plot_min = -1 if round(atlas_fdata.min()) == 0 else round(atlas_fdata.min())
-                plot_max = 1 if round(atlas_fdata.max()) == 0 else round(atlas_fdata.max())
-
-                # Add stat map layer
-                p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
-                            color_range=(plot_min,plot_max))
-
-                # Color bar
-                kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
-                        decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"])
-                fig = p.build(cbar_kws=kws)
-                fig_name = f"{group} - {cap}"
-                fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])      
-                
-                if show_figs:
-                    fig.show()
-                
-                if output_dir:
-                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}"
-                    fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
-
-        if return_stat_map:
-            return stat_map
-
-
-
-                    
-
-
-
-
+import numpy as np, re, warnings
+from kneed import KneeLocator
+from sklearn.cluster import KMeans
+from typing import Union
+from .._utils import _CAPGetter, _convert_pickle_to_dict, _check_parcel_approach
+
+
+class CAP(_CAPGetter):
+    def __init__(self, parcel_approach: dict[dict], n_clusters: Union[int, list[int]]=5, cluster_selection_method: str=None, groups: dict=None):
+        """
+        Initialize the CAP (Co-activation Patterns) analysis class.
+
+        Parameters
+        ----------
+        node_labels : list[str]
+            Decoded or non-decoded Schaefer Atlas labels for the nodes.
+        n_clusters : int or list[int], default=5
+            The number of clusters to use. Can be a single integer or a list of integers.
+        cluster_selection_method: str, default=None
+            Method to find the optimal number of clusters. Options are "silhouette" or "elbow".
+        groups : dict, default=None
+            A mapping of group names to subject IDs. Each group contains subject IDs for
+            separate CAP analysis. If None, CAPs are not separated by group.
+
+        Raises
+        ------
+        ValueError
+            If `cluster_selection_method` is none when `n_clusters` is a list.
+        ValueError
+            If `cluster_selection_method` is used when `n_clusters` is a single integer.
+        TypeError
+            If `groups` is provided but is not a dictionary.
+        AssertionError
+            If any group in `groups` has zero subject IDs.
+
+        Notes
+        -----
+        The initialization ensures unique values if `n_clusters` is a list and checks for 
+        valid input types and values.
+        """
+        # Ensure all unique values if n_clusters is a list
+        self._n_clusters = n_clusters if type(n_clusters) == int else sorted(list(set(n_clusters)))
+        self._cluster_selection_method = cluster_selection_method 
+
+        if type(n_clusters) == list:
+            self._n_clusters =  self._n_clusters[0] if all([type(self._n_clusters) == list, len(self._n_clusters) == 1]) else self._n_clusters
+            # Raise error if n_clusters is a list and no cluster selection method is specified
+            if all([len(n_clusters) > 1, self._cluster_selection_method== None]):
+                raise ValueError("`cluster_selection_method` cannot be None since n_clusters is a list.")
+
+        # Raise error if silhouette_method is requested when n_clusters is an integer
+        if all([self._cluster_selection_method != None, type(self._n_clusters) == int]):
+            raise ValueError("`cluster_selection_method` only valid if n_clusters is a range of unique integers.")
+       
+        self._groups = groups
+        # Raise error if self groups is not a dictionary 
+        if self._groups:
+            if type(self._groups) != dict:
+                raise TypeError("`groups` must be a dictionary where the keys are the group names and the items correspond to subject ids in the groups.")
+            
+            for group_name in self._groups.keys():
+                assert len(self._groups[group_name]) > 0, f"{group_name} has zero subject ids."
+            
+            # Convert ids to strings
+            for group in self._groups.keys():
+                self._groups[group] = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in self._groups[group]]
+        
+        valid_parcel_dict = {"Schaefer", "AAL", "Custom"}
+
+        if len(parcel_approach.keys()) > 1:
+            raise ValueError(f"Only one parcellation approach can be selected from the following valid options: {valid_parcel_dict.keys()}.\nExample format of `parcel_approach`: {valid_parcel_dict}")
+        
+        self._parcel_approach = parcel_approach 
+
+    def get_caps(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], runs: Union[int, list[int]]=None, random_state: int=None, 
+                 show_figs: bool=False, output_dir: str=None, standardize: bool=True, epsilon: Union[int,float]=0, **kwargs) -> None:
+        """"" Create CAPs
+
+        The purpose of this function is to concatenate the timeseries of each subject and perform kmeans clustering on the concatenated data.
+        
+        Parameters
+        ----------
+        subject_timeseries: dict or str
+            A pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
+            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
+            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
+            must consist of the timeseries associated with that run.
+        runs: int or list[int], default=None
+            The run numbers to perform the CAPs analysis with. If None, all runs in the subject timeseries will be concatenated into a single dataframe.
+        random_state: int, default=None
+            The random state to use for scikit's KMeans function.
+        show_figs: bool, default=False
+            Display the plots of inertia scores for all groups if `cluster_selection_method`="elbow".
+        output_dir: str, default=None
+            Directory to save plot in if `cluster_selection_method`="elbow".
+        standardize: bool, default=True
+            To z-score the features of the concatonated timeseries array.
+        epsilon: int or float, default=0
+            Small number to add to the denominator when z-scoring for numerical stabilty.
+        kwargs: dict
+            Dictionary to adjust certain parameters related to `cluster_selection_method`="elbow". Additional parameters includes "S", which adjust the sensitivity of finding the elbow 
+            (Larger values of `S` are more conservative and less sensitive to small fluctuations; this package uses KneeLocator from the kneed package to identify the elbow), defaults to 1, 
+            "dpi", to adjust the dpi of the elbow plot, defaults to 300, and "figsize", which adjust the size of the elbow plots.
+            
+        Raises
+        ------
+        ValueError
+            If both input_path and subject_timeseries are None.
+        """
+        
+        if runs:
+            if isinstance(runs,int): runs = list(runs)
+    
+        self._runs = runs if runs else "all"
+        self._standardize = standardize
+        self._epsilon = epsilon
+
+        if isinstance(subject_timeseries, str) and "pkl" in subject_timeseries: subject_timeseries = _convert_pickle_to_dict(pickle_file=subject_timeseries)
+
+        self._concatenated_timeseries = self._get_concatenated_timeseries(subject_timeseries=subject_timeseries, runs=runs)
+
+        if self._cluster_selection_method == "silhouette": 
+            self._perform_silhouette_method(random_state=random_state)
+        elif self._cluster_selection_method == "elbow":
+            self._perform_elbow_method(random_state=random_state, show_figs=show_figs, output_dir=output_dir, **kwargs)
+        else:
+            self._kmeans = {}
+            for group in self._groups.keys():
+                self._kmeans[group] = {}
+                self._kmeans[group] = KMeans(n_clusters=self._n_clusters,random_state=random_state).fit(self._concatenated_timeseries[group]) 
+            
+        # Create states dict   
+        self._create_caps_dict()
+    
+    def _perform_silhouette_method(self, random_state):
+        from sklearn.metrics import silhouette_score
+
+        # Initialize attribute
+        self._silhouette_scores = {}
+        self._optimal_n_clusters = {}
+        self._kmeans = {}
+
+        for group in self._groups.keys():
+            self._silhouette_scores[group] = {}
+            for n_cluster in self._n_clusters:
+                self._kmeans[group] = KMeans(n_clusters=n_cluster,random_state=random_state).fit(self._concatenated_timeseries[group])
+                cluster_labels = self._kmeans[group].predict(self._concatenated_timeseries[group])
+                self._silhouette_scores[group].update({n_cluster: silhouette_score(self._concatenated_timeseries[group], cluster_labels)})
+            self._optimal_n_clusters[group] = max(self._silhouette_scores[group], key=self._silhouette_scores[group].get)
+            if self._optimal_n_clusters[group] != self._n_clusters[-1]:
+                self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group],random_state=random_state).fit(self._concatenated_timeseries[group]) 
+            print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.")
+        
+    
+    def _perform_elbow_method(self, random_state, show_figs, output_dir, **kwargs):
+        # Initialize attribute
+        self._inertia = {}
+        self._optimal_n_clusters = {}
+        self._kmeans = {}
+
+        knee_dict = dict(S = kwargs["S"] if "S" in kwargs.keys() else 1)
+
+        for group in self._groups.keys():
+            self._inertia[group] = {}
+            for n_cluster in self._n_clusters:
+                self._kmeans[group] = KMeans(n_clusters=n_cluster,random_state=random_state).fit(self._concatenated_timeseries[group])
+                self._inertia[group].update({n_cluster: self._kmeans[group].inertia_}) 
+            
+            # Get optimal cluster size
+            kneedle = KneeLocator(x=list(self._inertia[group].keys()), 
+                                                        y=list(self._inertia[group].values()),
+                                                        curve='convex',
+                                                        direction='decreasing', S=knee_dict["S"])
+                
+            self._optimal_n_clusters[group] = kneedle.elbow
+            if not self._optimal_n_clusters[group]:
+                 warnings.warn("No elbow detected so optimal cluster size is None. Try adjusting the sensitivity parameter, `S`, to increase or decrease sensitivity (higher values are less sensitive), expanding the list of clusters to test, or setting `cluster_selection_method` to 'sillhouette'.")
+            else:
+                if self._optimal_n_clusters[group] != self._n_clusters[-1]:
+                    self._kmeans[group] = KMeans(n_clusters=self._optimal_n_clusters[group],random_state=random_state).fit(self._concatenated_timeseries[group])
+                print(f"Optimal cluster size for {group} is {self._optimal_n_clusters[group]}.\n")
+
+                if show_figs or output_dir != None:
+                    import matplotlib.pyplot as plt, os
+
+                    plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                                     figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6))
+                    
+                    plt.figure(figsize=plot_dict["figsize"])
+                    inertia_values = [y for x,y in self._inertia[group].items()]
+                    plt.plot(self._n_clusters, inertia_values)
+                    plt.vlines(self._optimal_n_clusters[group], plt.ylim()[0], plt.ylim()[1], 
+                               linestyles="--", label="elbow")
+                    plt.legend(loc="best")
+                    plt.xlabel("K")
+                    plt.ylabel("Inertia")
+                    plt.title(group)
+
+                    if output_dir:
+                        plt.savefig(os.path.join(output_dir,f"{group.replace(' ','_')}_elbow.png"), dpi=plot_dict["dpi"])
+                    
+                    if show_figs == False:
+                        plt.close()
+                    else:
+                        plt.show()
+
+    def _create_caps_dict(self):
+        # Initialize dictionary
+        self._caps = {}
+        for group in self._groups.keys():
+                self._caps[group] = {}
+                self._caps[group].update({f"CAP-{state_number}": state_vector for state_number, state_vector in zip([num for num in range(1,len(self._kmeans[group].cluster_centers_)+1)],self._kmeans[group].cluster_centers_)})
+    
+    def _get_concatenated_timeseries(self, subject_timeseries, runs):
+        # Create dictionary for "All Subjects" if no groups are specified to reuse the same loop instead of having to create logic for grouped and non-grouped version of the same code
+        if not self._groups: self._groups = {"All Subjects": [subject for subject in subject_timeseries.keys()]}
+
+        concatenated_timeseries = {group: {} for group in self._groups.keys()}
+
+        self._generate_lookup_table()
+
+        self._mean_vec = {group: {} for group in self._groups.keys()}
+        self._stdev_vec = {group: {} for group in self._groups.keys()}
+
+        for subj_id, group in self._subject_table.items():
+            requested_runs = [f"run-{run}" for run in runs] if runs else subject_timeseries[subj_id].keys()
+            subject_runs = [subject_run for subject_run in subject_timeseries[subj_id].keys() if subject_run in requested_runs] 
+            if len(subject_runs) == 0:
+                warnings.warn(f"Skipping subject {subj_id} since they do not have the requested run numbers {','.join(requested_runs)}")
+                continue
+            for curr_run in subject_runs:
+                if len(concatenated_timeseries[group]) == 0:
+                    concatenated_timeseries[group] = subject_timeseries[subj_id][curr_run] if subj_id in list(set(self._groups[group])) else concatenated_timeseries[group]
+                else:
+                    concatenated_timeseries[group] = np.vstack([concatenated_timeseries[group], subject_timeseries[subj_id][curr_run]]) if subj_id in list(set(self._groups[group])) else concatenated_timeseries[group]
+        # Standardize
+        if self._standardize:
+            for group in self._groups.keys():
+                self._mean_vec[group], self._stdev_vec[group] = np.mean(concatenated_timeseries[group], axis=0), np.std(concatenated_timeseries[group], ddof=1, axis=0)
+                concatenated_timeseries[group] = (concatenated_timeseries[group] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon)
+
+        return concatenated_timeseries
+    
+    def _generate_lookup_table(self):
+        self._subject_table = {}
+        for group in self._groups:
+            for subj_id in self._groups[group]:
+                if subj_id in self._subject_table.keys():
+                    warnings.warn(f"Subject: {subj_id} appears more than once, only including the first instance of this subject in the analysis.") 
+                else:
+                    self._subject_table.update({subj_id : group})
+
+    def visualize_caps(self, output_dir: str=None, plot_options: Union[str, list[str]]="outer product", visual_scope: list[str]="regions", 
+                       task_title: str=None, show_figs: bool=True, subplots: bool=False, **kwargs):
+        """ Plotting CAPs
+
+        This function produces seaborn heatmaps for each CAP. If groups were given when the CAP class was initialized, plotting will be done for all CAPs for all groups.
+
+        Parameters
+        ----------
+        output_dir: str, default=None
+            Directory to save plots in. If None, plots will not be saved.
+        plot_options: str or list[str], default="outer product"
+            Type of plots to create. Options are "outer product" or "heatmap".
+        visual_scope: str or list[str], default="regions"
+            Determines whether plotting is done at the region level or node level. 
+            For region level, the value of each nodes in the same regions are averaged together them plotted.
+            Options are "regions" or "nodes".
+        task_title: str, default=None
+            Serves as the title of each plot as well as the name of the saved file if output_dir is given.
+        show_figs: bool, default=True
+            Display figures or not to display figures.
+        subplots: bool, default=True
+            Produce subplots for outer product plots.
+        kwargs: dict
+            Keyword arguments used when saving figures. Valid keywords include "dpi", "format", "figsize", "fontsize", "hspace", "wspace", "xticklabels_size", "yticklabels_size", "shrink", "nrow", "ncol", "suptitle_fontsize", "tight_layout", "rect", "sharey", "xlabel_rotation", "ylabel_rotation", "annot". 
+            If `output_dir` is not None and no inputs for dpi and format are given, dpi defaults to 300 and format defaults to "png". If no keywords, "figsize" defaults to (8,6), "fontsize", which adjusts the title size of the individual plots or subplots, defaults to 14, "hspace", which adjusts spacing for subplots, defaults to 0.4, 
+            "wspace", which adjusts spacing between subplots, defaults to 0.4, "xticklabels_size" defaults to 8, "yticklabels_size" defaults to 8, shrink, which adjusts the cbar size, defaults to 0.8, "nrow", which is the number of rows for subplot and varies, and "ncol", which is the number of columns for subplot, default varies but max is 5, "suptitle_fontsize", 
+            size of the main title when subplot is True, defaults to 0.7, "tight_layout", use tight layout for subplot, defaults to True, "rect", input for the `rect` parameter in tight layout when subplots is True to fix whitespace issues, default is [0, 0.03, 1, 0.95], "sharey", which shares y axis labela for subplots, defaults to True, 
+            "xlabel_rotation", which rotates the labels on the x-axis, defaults to 0, "ylabel_rotation", which rotates the labels on the y-axis, defaults to 0, "annot", which adds values to cells on the outer product heatmap at the region level only, defaults to False, "linewidths", which specifies the padding between each cell, defaults to 0,
+            and "cmap", which specifies the color pattern of the cells in the plot, defaults to "coolwarm".
+    
+         Notes
+        -----
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
+        the zero index should correspond the first id that is not zero.
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
+        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+        """
+        import itertools, os
+
+        # Check parcel approach
+
+        # Check if parcellation_approach is custom
+        if "Custom" in self.parcel_approach.keys() and ("nodes" not in self.parcel_approach["Custom"].keys() or "regions" not in self.parcel_approach["Custom"].keys()):
+            _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_caps")
+
+        # Check labels
+        check_caps = self._caps[list(self._caps.keys())[0]]
+        check_caps = check_caps[list(check_caps.keys())[0]]
+        if check_caps.shape[0] != len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]): 
+                raise ValueError("Number of rois/nodes used for CAPs does not equal the number of rois/nodes specified in `parcel_approach`.")
+
+        if output_dir:
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
+
+        # Convert to list
+        if type(plot_options) == str: plot_options = [plot_options]
+        if type(visual_scope) == str: visual_scope = [visual_scope]
+
+        # Check inputs for plot_options and visual_scope
+        if not any(["heatmap" in plot_options, "outer product" in plot_options]):
+            raise ValueError("Valid inputs for `plot_options` are 'heatmap' and 'outer product'.")
+        
+        if not any(["regions" in visual_scope, "nodes" in visual_scope]):
+            raise ValueError("Valid inputs for `visual_scope` are 'regions' and 'nodes'.")
+
+        if "regions" in visual_scope: self._create_regions()
+
+        # Create plot dictionary
+        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                        format = kwargs["format"] if kwargs and "format" in kwargs.keys() else "png",
+                        figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (8,6),
+                        fontsize = kwargs["fontsize"] if kwargs and "fontsize" in kwargs.keys() else 14,
+                        hspace = kwargs["hspace"] if kwargs and "hspace" in kwargs.keys() else 0.2,
+                        wspace = kwargs["wspace"] if kwargs and "wspace" in kwargs.keys() else 0.2,
+                        xticklabels_size = kwargs["xticklabels_size"] if kwargs and "xticklabels_size" in kwargs.keys() else 8,
+                        yticklabels_size = kwargs["yticklabels_size"] if kwargs and "yticklabels_size" in kwargs.keys() else 8,
+                        shrink = kwargs["shrink"] if kwargs and "shrink" in kwargs.keys() else 0.8,
+                        nrow = kwargs["nrow"] if kwargs and "nrow" in kwargs.keys() else None,
+                        ncol = kwargs["ncol"] if kwargs and "ncol" in kwargs.keys() else None,
+                        suptitle_fontsize = kwargs["suptitle_fontsize"] if kwargs and "suptitle_fontsize" in kwargs.keys() else 20,
+                        tight_layout = kwargs["tight_layout"] if kwargs and "tight_layout" in kwargs.keys() else True,
+                        rect = kwargs["rect"] if kwargs and "rect" in kwargs.keys() else [0, 0.03, 1, 0.95],
+                        sharey = kwargs["sharey"] if kwargs and "sharey" in kwargs.keys() else True,
+                        xlabel_rotation = kwargs["xlabel_rotation"] if kwargs and "xlabel_rotation" in kwargs.keys() else 0,
+                        ylabel_rotation = kwargs["ylabel_rotation"] if kwargs and "ylabel_rotation" in kwargs.keys() else 0,
+                        annot = kwargs["annot"] if kwargs and "annot" in kwargs.keys() else False,
+                        linewidths = kwargs["linewidths"] if kwargs and "linewidths" in kwargs.keys() else 0,
+                        cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "coolwarm"
+                        )
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
+
+        # Ensure plot_options and visual_scope are lists
+        plot_options = plot_options if type(plot_options) == list else list(plot_options)
+        visual_scope = visual_scope if type(visual_scope) == list else list(visual_scope)
+        # Initialize outer product attribute
+        if "outer product" in plot_options: self._outer_product = {}
+
+        distributed_list = list(itertools.product(plot_options,visual_scope,self._groups.keys()))
+
+        for plot_option, scope, group in distributed_list:
+                # Get correct labels depending on scope
+                if scope == "regions": 
+                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
+                        cap_dict, columns = self._region_caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]
+                    else:
+                        cap_dict, columns = self._region_caps, list(self._parcel_approach["Custom"]["regions"].keys())
+                elif scope == "nodes": 
+                    if list(self._parcel_approach.keys())[0] in ["Schaefer", "AAL"]:
+                        cap_dict, columns = self._caps, self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]
+                    else:
+                        cap_dict, columns = self._caps , [x[0] + " " + x[1] for x in list(itertools.product(["LH", "RH"],self._parcel_approach["Custom"]["regions"].keys()))]
+
+                #  Generate plot for each group
+                if plot_option == "outer product": self._generate_outer_product_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns, subplots=subplots,
+                                                                                    output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
+                elif plot_option == "heatmap": self._generate_heatmap_plots(group=group, plot_dict=plot_dict, cap_dict=cap_dict, columns=columns,
+                                                                            output_dir=output_dir, task_title=task_title, show_figs=show_figs, scope=scope)
+            
+    def _create_regions(self):
+        self._region_caps = {group: {} for group in self._groups.keys()}
+        for group in self._groups.keys():
+            for cap in self._caps[group].keys():
+                region_caps = {}
+                if list(self._parcel_approach.keys())[0] != "Custom":
+                    for region in self._parcel_approach[list(self._parcel_approach.keys())[0]]["regions"]:
+                        if len(region_caps) == 0:
+                            region_caps = np.array([np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
+                        else:
+                            region_caps = np.hstack([region_caps, np.average(self._caps[group][cap][np.array([index for index, node in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in node])])])
+                else:
+                    region_dict = self._parcel_approach["Custom"]["regions"]
+                    region_keys = region_dict.keys()
+                    for region in region_keys:
+                        roi_indxs = np.array(region_dict[region]["lh"] + region_dict[region]["rh"])
+
+                        if len(region_caps) == 0:
+                            region_caps= np.array([np.average(self._caps[group][cap][roi_indxs])])
+                        else:
+                            region_caps= np.hstack([region_caps, np.average(self._caps[group][cap][roi_indxs])])
+
+                self._region_caps[group].update({cap: region_caps})
+    
+    def _generate_outer_product_plots(self, group, plot_dict, cap_dict, columns, subplots, output_dir, task_title, show_figs, scope):
+        import matplotlib.pyplot as plt, os
+        from seaborn import heatmap
+
+        # Nested dictionary for group
+        self._outer_product[group] = {}
+
+        # Create base grid for subplots
+        if subplots:
+            # Max five subplots per row for default
+            default_col = len(cap_dict[group].keys()) if len(cap_dict[group].keys()) <= 5 else 5
+            ncol = plot_dict["ncol"] if plot_dict["ncol"] != None else default_col
+            # Pad nrow, since int will round down, padding is needed for cases where len(cap_dict[group].keys())/ncol is a float. This will add the extra row needed
+            x_pad = 0 if len(cap_dict[group].keys())/ncol <= 1 else 1
+            nrow = plot_dict["nrow"] if plot_dict["nrow"] != None else x_pad + int(len(cap_dict[group].keys())/ncol)
+
+            subplot_figsize = (8 * ncol, 6 * nrow) if plot_dict["figsize"] == (8,6) else plot_dict["figsize"] 
+
+            fig, axes = plt.subplots(nrow, ncol, sharex=False, sharey=plot_dict["sharey"], figsize=subplot_figsize)
+            suptitle = f"{group} {task_title}" if task_title else f"{group}"
+            fig.suptitle(suptitle, fontsize=plot_dict["suptitle_fontsize"])
+            fig.subplots_adjust(hspace=plot_dict["hspace"], wspace=plot_dict["wspace"])  
+            if plot_dict["tight_layout"]: fig.tight_layout(rect=plot_dict["rect"])  
+
+            # Current subplot
+            axes_x, axes_y = [0,0] 
+
+        # Iterate over CAPs
+        for cap in cap_dict[group].keys():
+            # Calculate outer product
+            self._outer_product[group].update({cap: np.outer(cap_dict[group][cap],cap_dict[group][cap])})
+            # Create labels if nodes requested for scope
+            if scope == "nodes":
+                import collections
+                
+                # Get frequency of each major hemisphere and region in Schaefer, AAL, or Custom atlas
+                if list(self._parcel_approach.keys())[0] == "Schaefer":
+                    frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
+                elif list(self._parcel_approach.keys())[0] == "AAL":
+                    frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
+                else:
+                    frequency_dict = {}
+                    for id in columns:
+                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
+                        region_id = re.split("LH |RH ", id)[-1]
+                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
+                # Get the names, which indicate the hemisphere and region
+                names_list = list(frequency_dict.keys())
+                # Create label list the same length as the labels dictionary and substitute each element with an empty string
+                labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
+
+                starting_value = 0
+
+                # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
+                for num, name in enumerate(names_list): 
+                    if num == 0:
+                        labels[0] = name
+                    else:
+                        # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
+                        starting_value += frequency_dict[names_list[num-1]] 
+                        labels[starting_value] = name
+
+            if subplots: 
+                ax = axes[axes_y] if nrow == 1 else axes[axes_x,axes_y]
+                # Modify tick labels based on scope
+                if scope == "regions":
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={"shrink": plot_dict["shrink"]}, annot=plot_dict["annot"])
+                else:
+                    display = heatmap(ax=ax, data=self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={"shrink": plot_dict["shrink"]})
+
+                    ticks = [i for i, label in enumerate(labels) if label]  
+
+                    ax.set_xticks(ticks)  
+                    ax.set_xticklabels([label for label in labels if label]) 
+                    ax.set_yticks(ticks)  
+                    ax.set_yticklabels([label for label in labels if label]) 
+
+                # Modify label sizes
+                display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
+
+                if plot_dict["sharey"] == True:
+                    if axes_y == 0: display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
+                else:
+                    display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
+
+                # Set title of subplot
+                ax.set_title(cap, fontsize=plot_dict["fontsize"])
+
+                # If modulus is zero, move onto the new column back to zero
+                if (axes_y % ncol == 0 and axes_y != 0) or axes_y == ncol - 1: 
+                    axes_x += 1
+                    axes_y = 0
+                else:
+                    axes_y += 1
+
+            else:
+                # Create new plot for each iteration when not subplot
+                plt.figure(figsize=plot_dict["figsize"])
+
+                plot_title = f"{group} {cap} {task_title}" if task_title else f"{group} {cap}"
+                if scope == "regions": display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=columns, yticklabels=columns, cbar_kws={'shrink': plot_dict["shrink"]})
+                else: 
+                    display = heatmap(self._outer_product[group][cap], cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], xticklabels=[], yticklabels=[], cbar_kws={'shrink': plot_dict["shrink"]})
+                    ticks = [i for i, label in enumerate(labels) if label]  
+
+                    display.set_xticks(ticks)  
+                    display.set_xticklabels([label for label in labels if label]) 
+                    display.set_yticks(ticks)  
+                    display.set_yticklabels([label for label in labels if label]) 
+                
+                # Set title
+                display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
+
+                # Modify label sizes
+                display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
+                display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
+
+                # Save individual plots
+                if output_dir:
+                    partial_filename = f"{group}_{cap}_{task_title}" if task_title else f"{group}_{cap}"
+                    full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+                    display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')
+        
+        # Remove subplots with no data
+        if subplots: [fig.delaxes(ax) for ax in axes.flatten() if not ax.has_data()]
+
+        # Save subplot
+        if subplots and output_dir: 
+            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
+            full_filename = f"{partial_filename}_outer_product_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_outer_product_heatmap-nodes.{plot_dict['format']}"
+            display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
+        
+        # Display figures
+        if not show_figs: plt.close()
+
+    def _generate_heatmap_plots(self, group, plot_dict, cap_dict, columns, output_dir, task_title, show_figs, scope):
+        import matplotlib.pyplot as plt, os, pandas as pd
+        from seaborn import heatmap
+        
+        # Initialize new grid
+        plt.figure(figsize=plot_dict["figsize"])
+
+        if scope == "regions": 
+            display = heatmap(pd.DataFrame(cap_dict[group], index=columns), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]}) 
+        else: 
+            # Create Labels
+            import collections
+            if list(self._parcel_approach.keys())[0] == "Schaefer":
+                frequency_dict = dict(collections.Counter([names[0] + " " + names[1] for names in [name.split("_")[0:2] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]]]))
+            elif list(self._parcel_approach.keys())[0] == "AAL":
+                frequency_dict = collections.Counter([name.split("_")[0] for name in self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]])
+            else:
+                    frequency_dict = {}
+                    for id in columns:
+                        hemisphere_id = "LH" if id.startswith("LH ") else "RH"
+                        region_id = re.split("LH |RH ", id)[-1]
+                        frequency_dict.update({id: len(self._parcel_approach["Custom"]["regions"][region_id][hemisphere_id.lower()])})
+            names_list = list(frequency_dict.keys())
+            labels = ["" for _ in range(0,len(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]))]
+
+            starting_value = 0
+
+            # Iterate through names_list and assign the starting indices corresponding to unique region and hemisphere key
+            for num, name in enumerate(names_list): 
+                if num == 0:
+                    labels[0] = name
+                else:
+                    # Shifting to previous frequency of the preceding netwerk to obtain the new starting value of the subsequent region and hemosphere pair
+                    starting_value += frequency_dict[names_list[num-1]] 
+                    labels[starting_value] = name
+
+            display = heatmap(pd.DataFrame(cap_dict[group], columns=cap_dict[group].keys()), xticklabels=True, yticklabels=True, cmap=plot_dict["cmap"], linewidths=plot_dict["linewidths"], cbar_kws={'shrink': plot_dict["shrink"]})
+
+            plt.yticks(ticks=[pos for pos, label in enumerate(labels) if label], labels=names_list)  
+
+        # Modify label sizes
+        display.set_xticklabels(display.get_xticklabels(), size = plot_dict["xticklabels_size"], rotation=plot_dict["xlabel_rotation"])
+        display.set_yticklabels(display.get_yticklabels(), size = plot_dict["yticklabels_size"], rotation=plot_dict["ylabel_rotation"])
+
+        # Set plot name
+        plot_title = f"{group} CAPS {task_title}" if task_title else f"{group} CAPS" 
+        display.set_title(plot_title, fontdict= {'fontsize': plot_dict["fontsize"]})
+
+        # Save plots
+        if output_dir:
+            partial_filename = f"{group}_CAPS_{task_title}" if task_title else f"{group}_CAPS"
+            full_filename = f"{partial_filename}_heatmap-regions.{plot_dict['format']}" if scope == "regions" else f"{partial_filename}_heatmap-nodes.{plot_dict['format']}"
+            display.get_figure().savefig(os.path.join(output_dir,full_filename), dpi=plot_dict["dpi"], bbox_inches='tight')    
+   
+        # Display figures
+        if not show_figs: plt.close()
+
+    def calculate_metrics(self, subject_timeseries: Union[dict[dict[np.ndarray]], str], tr: float=None, runs: Union[int]=None, continuous_runs: bool=False, metrics: Union[str, list[str]]=["temporal fraction", "persistence", "counts", "transition frequency"], return_df: bool=True, output_dir: str=None, file_name: str=None) -> dict:
+        """Get CAP metrics
+
+        Creates a single pandas Dataframe containing all participants containing CAP metrics as described in Liu et al., 2018 and Yang et al., 2021, where `temporal fraction` is the proportion of total volumes spent in a single CAP over all volumes in a run,
+        `persistence` is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and `counts` is the frequency of each CAP observed in a run, and `transition frequency` is the number of switches between
+        different CAPs across the entire run.
+
+        Parameters
+        ----------
+        subject_timeseries: dict or str
+            The absolute path of the pickle file containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or
+            the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
+            ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
+            must consist of the timeseries associated with that run. This should be the same dictionary used for `get_caps()`.
+        tr: float, default=None
+            The repetition time. If given, persistence will be calculate as the average uninterrupted time spent in each CAP. If not give, persistence will be calculate
+            as the average uninterrupted volumes (TRs) spent in each state.
+        runs: int or list[int], default=None
+            The run numbers to calculate cap metrics for. If None, cap metrics will be calculated for each run.
+        continuous_runs: bool, default=False
+            If True, all runs will be treated as a single, uninterrupted run.
+        metrics : str or list[str], default=["temporal fraction", "persistence", "counts", "transition frequency"]
+            The metrics to calculate. Available options include `temporal fraction`, `persistence`, `counts`, and `transition frequency`.
+        return_df: str, default=True
+            If True, dataframe will be returned.
+        output_dir: str, default=None
+            Directory to save dataframe in. If None, dataframe will not be saved.
+        file_name: str, default=None
+            Name to save dataframe as if output_dir is not None.
+
+        Returns
+        -------
+        dictionary containing pandas dataframes - one for each metric requested.
+
+        Raises
+        ------
+        ValueError
+            No valid metrics are detected in `metrics` parameter.
+
+        Notes
+        -----
+        The presence of 0 for specific CAPs in the "temporal fraction", "persistence", or "counts" dataframes, indicates that the participant had zero instances of 
+        a specific CAP.
+
+        References
+        -----
+        Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+        Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. 
+        NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+        """
+        import collections, os, pandas as pd
+
+        metrics = [metrics] if isinstance(metrics, str) else metrics
+
+        valid_metrics = ["temporal fraction", "persistence", "counts", "transition frequency"]
+
+        boolean_list = [element in valid_metrics for element in metrics]
+
+        if any(boolean_list):
+            invalid_metrics = [metrics[indx] for indx,boolean in enumerate(boolean_list) if boolean == False]
+            if len(invalid_metrics) > 0:
+                warnings.warn(f"invalid metrics will be ignored: {' '.join(invalid_metrics)}")
+        else:
+            raise ValueError(f"No valid metrics in `metrics` list. Valid metrics are {', '.join(valid_metrics)}")
+        
+        if isinstance(subject_timeseries, str) and "pkl" in subject_timeseries: subject_timeseries = _convert_pickle_to_dict(pickle_file=subject_timeseries)
+
+        group_cap_dict = {}
+        # Get group with most CAPs
+        for group in self._groups.keys():
+            group_cap_dict.update({group: len(self._caps[group])})
+        
+        cap_names =  self._caps[max(group_cap_dict, key=group_cap_dict.get)].keys()
+        cap_numbers = [int(name.split("-")[-1]) for name in cap_names]
+
+        # Assign each subject TRs to CAP
+        predicted_subject_timeseries = {}
+
+        for subj_id, group in self._subject_table.items():
+            predicted_subject_timeseries[subj_id] = {}
+            requested_runs = [f"run-{run}" for run in runs] if runs else subject_timeseries[subj_id].keys()
+            subject_runs = [subject_run for subject_run in subject_timeseries[subj_id].keys() if subject_run in requested_runs] 
+            if len(subject_runs) == 0:
+                warnings.warn(f"Skipping subject {subj_id} since they do not have the requested run numbers {','.join(requested_runs)}")
+                continue
+            if not continuous_runs or len(requested_runs) == 1:
+                for curr_run in subject_runs:
+                        timeseries = (subject_timeseries[subj_id][curr_run] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon) if self._standardize else subject_timeseries[subj_id][curr_run] 
+                        predicted_subject_timeseries[subj_id].update({curr_run: self._kmeans[group].predict(timeseries) + 1})
+            else:
+                subject_runs = "Continuous Runs"
+                timeseries = {subject_runs: {}}
+                for curr_run in subject_timeseries[subj_id].keys():
+                    timeseries[subject_runs] = np.vstack([timeseries[subject_runs], subject_timeseries[subj_id][curr_run]]) if len(timeseries[subject_runs]) != 0 else subject_timeseries[subj_id][curr_run]
+                timeseries = (timeseries[subject_runs] - self._mean_vec[group])/(self._stdev_vec[group] + self._epsilon) if self._standardize else timeseries[subject_runs]
+                predicted_subject_timeseries[subj_id].update({subject_runs: self._kmeans[group].predict(timeseries) + 1})
+
+        # Create pd.dataframe
+        df_dict = {}
+
+        for metric in metrics: 
+            if metric in valid_metrics:
+                if metric != "transition frequency":
+                    df_dict.update({metric: pd.DataFrame(columns=["Subject_ID", "Group","Run"] + list(cap_names))})
+                else:
+                    df_dict.update({metric: pd.DataFrame(columns=["Subject_ID", "Group","Run","Transition_Frequency"])})
+
+        distributed_list = []
+        for subj_id, group in self._subject_table.items():
+            for curr_run in predicted_subject_timeseries[subj_id].keys():
+                distributed_list.append([subj_id,group,curr_run])
+
+        for subj_id, group, curr_run in distributed_list:
+            if "temporal fraction" in metrics or "counts" in metrics:
+                frequency_dict = dict(collections.Counter(predicted_subject_timeseries[subj_id][curr_run]))
+                sorted_frequency_dict = {key: frequency_dict[key] for key in sorted(list(frequency_dict.keys()))}
+                if len(sorted_frequency_dict) != len(cap_numbers):
+                    sorted_frequency_dict = {cap_number: sorted_frequency_dict[cap_number] if cap_number in sorted_frequency_dict.keys() else 0 for cap_number in cap_numbers}
+                if "temporal fraction" in metrics: 
+                    proportion_dict = {key: item/(len(predicted_subject_timeseries[subj_id][curr_run])) for key, item in sorted_frequency_dict.items()}
+                    # Populate Dataframe
+                    df_dict["temporal fraction"].loc[len(df_dict["temporal fraction"])] = [subj_id, group, curr_run] + [items for _ , items in proportion_dict.items()]
+                if "counts" in metrics:
+                    # Populate Dataframe
+                    df_dict["counts"].loc[len(df_dict["counts"])] = [subj_id, group, curr_run] + [items for _ , items in sorted_frequency_dict.items()]
+            if "persistence" in metrics:
+                # Initialize variable
+                persistence_dict = {}
+                uninterrupted_volumes = []
+                count = 0
+
+                # Iterate through caps
+                for target in cap_numbers:
+                    # Iterate through each element and count uniterrupted volumes that equal target
+                    for index in range(0,len(predicted_subject_timeseries[subj_id][curr_run])):
+                        if predicted_subject_timeseries[subj_id][curr_run][index] == target:
+                            count +=1
+                        # Store count in list if interuptted and not zero an
+                        else:
+                            if count != 0:
+                                uninterrupted_volumes.append(count)
+                            # Reset counter 
+                            count = 0
+                    # In the event, a participant only occupies one CAP and to ensure final counts are added
+                    if count > 0:
+                        uninterrupted_volumes.append(count)
+                    # If uninterrupted_volumes not zero, multiply elements in the list by repetition time, sum and divide
+                    if len(uninterrupted_volumes) > 0:
+                        if tr:
+                            persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes)*tr)/(len(uninterrupted_volumes))})
+                        else:
+                            persistence_dict.update({target: np.sum(np.array(uninterrupted_volumes))/(len(uninterrupted_volumes))})
+                    else:
+                        persistence_dict.update({target: 0})
+                    # Reset variables
+                    count = 0
+                    uninterrupted_volumes = []
+                # Populate Dataframe
+                df_dict["persistence"].loc[len(df_dict["persistence"])] = [subj_id, group, curr_run] + [items for _ , items in persistence_dict.items()]
+            if "transition frequency" in metrics:
+                count = 0
+                # Iterate through predicted values 
+                for index in range(0,len(predicted_subject_timeseries[subj_id][curr_run])):
+                    if index != 0:
+                        # If the subsequent element does not equal the previous element, this is considered a transition
+                        if predicted_subject_timeseries[subj_id][curr_run][index-1] != predicted_subject_timeseries[subj_id][curr_run][index]:
+                            count +=1
+                df_dict["transition frequency"].loc[len(df_dict["transition frequency"])] = [subj_id, group, curr_run, count]
+
+        if output_dir:
+            for metric in df_dict.keys():
+                filename = file_name + f"-{metric.replace(' ','_')}" if file_name else f"{metric.replace(' ','_')}"
+                df_dict[f"{metric}"].to_csv(path_or_buf=os.path.join(output_dir,filename + ".csv"), sep=",", index=False)
+
+        if return_df:
+            return df_dict
+        
+    def caps2surf(self, output_dir: str=None, show_figs: bool = True, fwhm: float=None, 
+                  fslr_density: str="32k", method: str="linear", return_stat_map: bool = False, **kwargs):
+        """Project CAPs back onto atlas used for spatial dimensionality reduction for visualization
+        
+        Converts atlas into a stat map by replacing labels with the corresponding from the cluster centroids then plots on a surface plot.
+        This function uses surfplot for surface plotting.
+
+        Parameters
+        ----------
+        output_dir: str, default=None
+            Directory to save plots in. If None, plots will not be saved.
+        show_figs: bool, default=True
+            Display figures or not to display figures.
+        fwhm: float, defualt=None
+            Strength of spatial smoothing to apply in millimeters.
+        fslr_density: str, default="32k"
+            Density of the fslr surface when converting from mni 152 space to fslr surface. Options are 
+            "32k" or "164k".
+        method: str, default="linear"
+            Interpolation method to use when converting from mni152 space to fslr surface. Options are "linear"
+            or "nearest".
+        return_stat_map: bool, default=FAlse
+            Returns the atlas as a stat map.
+        **kwargs: dict
+            Additional parameters to pass to modify certain plot parameters. Options include "dpi", defaults to 300, "title_pad", defaults to -3,
+            "cmap", defaults to "cold_hot", "cbar_location", defaults to "bottom", "cbar_draw_border", defaults to False, "cbar_aspect", defaults to 10, "cbar_shrink", defaults 
+            to 0.2, "cbar_decimals", defaults to 0, and "cbar_pad", defaults to 0.
+            
+        Returns
+        -------
+        Nifti Stat map
+
+        Notes
+        -----
+        Assumes that atlas background label is zero and atlas is in MNI space. Also assumes that the indices from the cluster centroids are related
+        to the atlas by an offset of one. For instance, index 0 of the cluster centroid vector is the first nonzero label, which is assumed to be at the 
+        first index of the array in sorted(np.unique(atlas_fdata)).
+
+        Using fwhm to adjust smooting may help coverage issues.
+
+        """
+
+        import nibabel as nib, numpy as np, os
+        from nilearn import image
+        from nilearn.plotting.cm import _cmap_d 
+        from neuromaps.transforms import mni152_to_fslr
+        from neuromaps.datasets import fetch_fslr
+        from surfplot import Plot
+
+        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                         title_pad = kwargs["title_pad"] if kwargs and "title_pad" in kwargs.keys() else -3,
+                         cmap = kwargs["cmap"] if kwargs and "cmap" in kwargs.keys() else "cold_hot",
+                         cbar_location = kwargs["cbar_location"] if kwargs and "cbar_location" in kwargs.keys() else "bottom",
+                         cbar_draw_border = kwargs["cbar_draw_border"] if kwargs and "cbar_draw_border" in kwargs.keys() else False,
+                         cbar_aspect = kwargs["cbar_aspect"] if kwargs and "cbar_aspect" in kwargs.keys() else 10,
+                         cbar_shrink = kwargs["cbar_shrink"] if kwargs and "cbar_shrink" in kwargs.keys() else 0.2,
+                         cbar_decimals = kwargs["cbar_decimals"] if kwargs and "cbar_decimals" in kwargs.keys() else 0,
+                         cbar_pad = kwargs["cbar_pad"] if kwargs and "cbar_pad" in kwargs.keys() else 0)
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
+
+        for group in self._caps.keys():
+            for cap in self._caps[group].keys():
+                atlas = nib.load(self._parcel_approach[list(self._parcel_approach.keys())[0]]["maps"])
+                atlas_fdata = atlas.get_fdata()
+                # Get array containing all labels in atlas to avoid issue if atlas labels dont start at 1, like Nilearn's AAL map
+                target_array = sorted(np.unique(atlas_fdata))
+                for indx, value in enumerate(self._caps[group][cap]):
+                    actual_indx = indx + 1
+                    atlas_fdata[np.where(atlas_fdata == target_array[actual_indx])] = value
+                stat_map = nib.Nifti1Image(atlas_fdata, atlas.affine, atlas.header)
+                # Add smoothing to stat map to help mitigate potential coverage issues 
+                if fwhm != None:
+                    stat_map = image.smooth_img(stat_map, fwhm=fwhm)
+
+                # Code slightly adapted from surfplot example 2
+                gii_lh, gii_rh = mni152_to_fslr(stat_map, method=method, fslr_density=fslr_density)
+                surfaces = fetch_fslr()
+                lh, rh = surfaces['inflated']
+                lh = str(lh) if not isinstance(lh, str) else lh
+                rh = str(rh) if not isinstance(rh, str) else rh
+                sulc_lh, sulc_rh = surfaces['sulc']
+                sulc_lh = str(sulc_lh) if not isinstance(sulc_lh, str) else sulc_lh
+                sulc_rh = str(sulc_rh) if not isinstance(sulc_rh, str) else sulc_rh
+                p = Plot(lh, rh)
+
+                # Add base layer
+                p.add_layer({"left": sulc_lh, "right": sulc_rh}, cmap="binary_r", cbar=False)
+
+                plot_min = -1 if round(atlas_fdata.min()) == 0 else round(atlas_fdata.min())
+                plot_max = 1 if round(atlas_fdata.max()) == 0 else round(atlas_fdata.max())
+
+                # Add stat map layer
+                p.add_layer({"left": gii_lh, "right": gii_rh}, cmap=_cmap_d[plot_dict["cmap"]], 
+                            color_range=(plot_min,plot_max))
+
+                # Color bar
+                kws = dict(location=plot_dict["cbar_location"], draw_border=plot_dict["cbar_draw_border"], aspect=plot_dict["cbar_aspect"], shrink=plot_dict["cbar_shrink"],
+                        decimals=plot_dict["cbar_decimals"], pad=plot_dict["cbar_pad"])
+                fig = p.build(cbar_kws=kws)
+                fig_name = f"{group} - {cap}"
+                fig.axes[0].set_title(fig_name, pad=plot_dict["title_pad"])      
+                
+                if show_figs:
+                    fig.show()
+                
+                if output_dir:
+                    save_name = f"{group.replace(' ', '_')}_{cap.replace('-', '_')}"
+                    fig.savefig(os.path.join(output_dir, save_name), dpi=plot_dict["dpi"])
+
+        if return_stat_map:
+            return stat_map
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/analysis/merge.py` & `neurocaps-0.9.0.post5/neurocaps/analysis/merge.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,96 +1,96 @@
-import numpy as np
-from typing import Union
-from .._utils import _convert_pickle_to_dict
-
-def merge_dicts(subject_timeseries_list: Union[list[dict], list[str]], return_combined_dict: bool=True, return_reduced_dicts: bool=False, output_dir: str=None, file_name: str=None) -> dict:
-    """Merge subject timeseries
-
-    Merge subject timeseries dictionaries or pickle files to the first dictionary or pickle file in the list.
-    Repetition times from the same subject and run are merged together. The combined dicitonary will only include subjects
-    that are present in all dictionaries.
-
-    Parameters
-    ----------
-
-    subject_timeseries_list: list[dict] or list[str]
-        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
-        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-        must consist of the timeseries associated with that run.
-    return_combined_dict: bool, default=True,
-        Returns the merged dictionaries if True
-    return_reduced_dicts: bool, default=False
-        Returns the list of dictionaries provided with only the subjects present in the combined dictionary. Returns dictionaries in the same order
-        they are listed in the `subject_timeseries_list` parameter.
-    output_dir: str, default=None
-        Directory to save the merged dictionary to. Will be saved as a pickle file.
-    file_name: str, default=None
-        Name to save merged dictionary as.
-
-    Raises
-    ------
-    AssertionError
-        If the length of `subject_timeseries_list` is less than two.
-
-    Returns
-    -------
-    dict
-    
-    """
-    assert len(subject_timeseries_list) > 1, "Merging cannot be done with less than two dictionaries or files."
-
-    if isinstance(subject_timeseries_list[0],dict): subject_timeseries_combined = subject_timeseries_list[0] 
-    else: subject_timeseries_combined = _convert_pickle_to_dict(pickle_file=subject_timeseries_list[0])
-
-    # Get common subject ids
-    subject_set = {}
-
-    for curr_dict in subject_timeseries_list:      
-        if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
-        if len(subject_set) == 0: subject_set = set(curr_dict.keys())    
-        subject_set = subject_set.intersection(list(curr_dict.keys()))
-
-    # Order subjects
-    intersect_subjects = sorted(list(subject_set))
-
-    subject_timeseries_combined = {}
-
-    for curr_dict in subject_timeseries_list:
-        if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
-        for subj_id in intersect_subjects:
-            if subj_id not in subject_timeseries_combined.keys(): subject_timeseries_combined.update({subj_id: {}})
-            # Get run names in the current iteration
-            subject_runs = curr_dict[subj_id].keys()
-            for curr_run in subject_runs:
-                # If run is in combined dict, stack. If not, add
-                if curr_run in subject_timeseries_combined[subj_id].keys():
-                    subject_timeseries_combined[subj_id][curr_run] = np.vstack([subject_timeseries_combined[subj_id][curr_run], curr_dict[subj_id][curr_run]])
-                else:
-                    subject_timeseries_combined[subj_id].update({curr_run: curr_dict[subj_id][curr_run]})
-                
-    if output_dir:
-        import pickle, os
-        if not os.path.exists(output_dir):
-            os.makedirs(output_dir)
-    
-        with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
-            pickle.dump(subject_timeseries_combined,f)
-    
-    if return_reduced_dicts:
-        all_dicts = {}
-        count = 1
-        for curr_dict in subject_timeseries_list:
-            if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
-            if any([elem in subject_timeseries_combined.keys() for elem in curr_dict.keys()]):
-                all_dicts[f"dict_{count}"] = {}
-                for subj_id in subject_timeseries_combined.keys():
-                    if subj_id in curr_dict.keys():
-                        all_dicts[f"dict_{count}"].update({subj_id : curr_dict[subj_id]})
-                count += 1
-        if not return_combined_dict: return all_dicts
-            
-    if return_combined_dict:
-        if not return_reduced_dicts: return subject_timeseries_combined
-        else: 
-            all_dicts["combined"] = subject_timeseries_combined
+import numpy as np
+from typing import Union
+from .._utils import _convert_pickle_to_dict
+
+def merge_dicts(subject_timeseries_list: Union[list[dict], list[str]], return_combined_dict: bool=True, return_reduced_dicts: bool=False, output_dir: str=None, file_name: str=None) -> dict:
+    """Merge subject timeseries
+
+    Merge subject timeseries dictionaries or pickle files to the first dictionary or pickle file in the list.
+    Repetition times from the same subject and run are merged together. The combined dicitonary will only include subjects
+    that are present in all dictionaries.
+
+    Parameters
+    ----------
+
+    subject_timeseries_list: list[dict] or list[str]
+        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
+        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
+        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
+        must consist of the timeseries associated with that run.
+    return_combined_dict: bool, default=True,
+        Returns the merged dictionaries if True
+    return_reduced_dicts: bool, default=False
+        Returns the list of dictionaries provided with only the subjects present in the combined dictionary. Returns dictionaries in the same order
+        they are listed in the `subject_timeseries_list` parameter.
+    output_dir: str, default=None
+        Directory to save the merged dictionary to. Will be saved as a pickle file.
+    file_name: str, default=None
+        Name to save merged dictionary as.
+
+    Raises
+    ------
+    AssertionError
+        If the length of `subject_timeseries_list` is less than two.
+
+    Returns
+    -------
+    dict
+    
+    """
+    assert len(subject_timeseries_list) > 1, "Merging cannot be done with less than two dictionaries or files."
+
+    if isinstance(subject_timeseries_list[0],dict): subject_timeseries_combined = subject_timeseries_list[0] 
+    else: subject_timeseries_combined = _convert_pickle_to_dict(pickle_file=subject_timeseries_list[0])
+
+    # Get common subject ids
+    subject_set = {}
+
+    for curr_dict in subject_timeseries_list:      
+        if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
+        if len(subject_set) == 0: subject_set = set(curr_dict.keys())    
+        subject_set = subject_set.intersection(list(curr_dict.keys()))
+
+    # Order subjects
+    intersect_subjects = sorted(list(subject_set))
+
+    subject_timeseries_combined = {}
+
+    for curr_dict in subject_timeseries_list:
+        if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
+        for subj_id in intersect_subjects:
+            if subj_id not in subject_timeseries_combined.keys(): subject_timeseries_combined.update({subj_id: {}})
+            # Get run names in the current iteration
+            subject_runs = curr_dict[subj_id].keys()
+            for curr_run in subject_runs:
+                # If run is in combined dict, stack. If not, add
+                if curr_run in subject_timeseries_combined[subj_id].keys():
+                    subject_timeseries_combined[subj_id][curr_run] = np.vstack([subject_timeseries_combined[subj_id][curr_run], curr_dict[subj_id][curr_run]])
+                else:
+                    subject_timeseries_combined[subj_id].update({curr_run: curr_dict[subj_id][curr_run]})
+                
+    if output_dir:
+        import pickle, os
+        if not os.path.exists(output_dir):
+            os.makedirs(output_dir)
+    
+        with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
+            pickle.dump(subject_timeseries_combined,f)
+    
+    if return_reduced_dicts:
+        all_dicts = {}
+        count = 1
+        for curr_dict in subject_timeseries_list:
+            if "pkl" in curr_dict: curr_dict = _convert_pickle_to_dict(pickle_file=curr_dict)
+            if any([elem in subject_timeseries_combined.keys() for elem in curr_dict.keys()]):
+                all_dicts[f"dict_{count}"] = {}
+                for subj_id in subject_timeseries_combined.keys():
+                    if subj_id in curr_dict.keys():
+                        all_dicts[f"dict_{count}"].update({subj_id : curr_dict[subj_id]})
+                count += 1
+        if not return_combined_dict: return all_dicts
+            
+    if return_combined_dict:
+        if not return_reduced_dicts: return subject_timeseries_combined
+        else: 
+            all_dicts["combined"] = subject_timeseries_combined
             return all_dicts
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/analysis/standardize.py` & `neurocaps-0.9.0.post5/neurocaps/analysis/standardize.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,35 @@
-import numpy as np, pickle
-from typing import Union
-
-def standardize(subject_timeseries: Union[dict,str]) -> dict:
-    """Standardize subject timeseries 
-    
-    Standardizes each run independently for all subjects in the subject timeseries.
-
-    Parameters
-    ----------
-
-    subject_timeseries_list: dict or str
-        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
-        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
-        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
-        must consist of the timeseries associated with that run.
-
-     Returns
-    -------
-    dict
-    """
-
-    if ".pkl" in subject_timeseries:
-        with open(subject_timeseries, "rb") as foo:
-            subject_timeseries = pickle.load(foo)
-
-    for subject in subject_timeseries.keys():
-        for run in subject_timeseries[subject].keys():
-            subject_timeseries[subject][run] -= subject_timeseries[subject][run].mean(axis=0)
-            std = subject_timeseries[subject][run].std(axis=0, ddof=1)
-            # Taken from nilearn pipeline, used for numerical stability purposes to avoide numpy division error
-            std[std < np.finfo(np.float64).eps] = 1.0             
-            subject_timeseries[subject][run] /= std
-
+import numpy as np, pickle
+from typing import Union
+
+def standardize(subject_timeseries: Union[dict,str]) -> dict:
+    """Standardize subject timeseries 
+    
+    Standardizes each run independently for all subjects in the subject timeseries.
+
+    Parameters
+    ----------
+
+    subject_timeseries_list: dict or str
+        The list of pickle files containing the nested subject timeseries dictionary saved by the TimeSeriesExtractor class or a liist of the
+        the nested subject timeseries dictionary produced by the TimeseriesExtractor class. The first level of the nested dictionary must consist of the subject
+        ID as a string, the second level must consist of the the run numbers in the form of 'run-#', where # is the corresponding number of the run, and the last level 
+        must consist of the timeseries associated with that run.
+
+     Returns
+    -------
+    dict
+    """
+
+    if ".pkl" in subject_timeseries:
+        with open(subject_timeseries, "rb") as foo:
+            subject_timeseries = pickle.load(foo)
+
+    for subject in subject_timeseries.keys():
+        for run in subject_timeseries[subject].keys():
+            subject_timeseries[subject][run] -= subject_timeseries[subject][run].mean(axis=0)
+            std = subject_timeseries[subject][run].std(axis=0, ddof=1)
+            # Taken from nilearn pipeline, used for numerical stability purposes to avoide numpy division error
+            std[std < np.finfo(np.float64).eps] = 1.0             
+            subject_timeseries[subject][run] /= std
+
     return subject_timeseries
```

### Comparing `neurocaps-0.9.0.post4/neurocaps/extraction/timeseriesextractor.py` & `neurocaps-0.9.0.post5/neurocaps/extraction/timeseriesextractor.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,440 +1,442 @@
-import json, os, re, sys, warnings
-from typing import Union
-from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
-
-class TimeseriesExtractor(_TimeseriesExtractorGetter):
-    def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
-                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, fwhm: float=None, fd_threshold: float=None,
-                 n_acompcor_separate: int=None, dummy_scans: int=None):
-        """Timeseries Extractor Class
-        
-        Initializes a TimeseriesExtractor to prepare for Co-activation Patterns (CAPs) analysis.
-
-        Parameters
-        ----------
-        space : str, default="MNI152NLin2009cAsym"
-            The brain template space data is in. 
-        standardize : bool, default=True
-            Determines whether to standardize the timeseries. Refer to Nilearn's NiftiLabelsMasker for available options. 
-        detrend : bool, default=True
-            Detrends timeseries during extraction.
-        low_pass : bool, default=None
-            Signals above cutoff frequency will be filtered out.
-        high_pass : float, default=None
-            Signals below cutoff frequency will be filtered out.
-        parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
-            Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
-            Currently only "Schaefer", "AAL", and "Custom" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois", "yeo_networks", and "resolution_mm".
-            Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
-            is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
-            and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
-            - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
-        use_confounds : bool, default=True
-            To use confounds when extracting timeseries.
-        confound_names : List[str], default=None
-            Names of confounds to use in confound files. If None, default confounds are used.
-        fwhm : float, default=None
-            Parameter for spatial smoothing.
-        fd_threshold : float, default=None
-            Threshold criteria to remove volume after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
-            in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
-        n_acompcor_separate : int, default = None
-            The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
-            then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
-            used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
-            masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
-            `confound_names` parameter.
-        dummy_scans : float, default=None
-            Removes the first `n` number of volumes before extracting timeseries.
-        
-        Notes for `confounds_names`
-        --------------------------
-        For the `confound_names` parameter, an asterisk ("*") can be used to find the name of confounds that starts with the term preceding the asterisk.
-        For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
-
-        Notes for `parcel_approach`
-        ---------------------------
-        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
-        the zero index should correspond the first id that is not zero.
-
-        Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-        - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
-          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
-          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
-          For timeseries extraction, this key is not required.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
-        
-        Example 
-        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
-
-        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                             "regions": {"Vis" : {"lh": [0,1],
-                                                  "rh": [3,4]},
-                                         "Hippocampus": {"lh": [2],
-                                                         "rh": [5]}}}}
-        """
-        self._space = space
-        self._signal_clean_info = {"standardize": standardize, "detrend": detrend, "low_pass": low_pass, "high_pass": high_pass, "fwhm": fwhm, 
-                                   "dummy_scans": dummy_scans, "use_confounds": use_confounds,  "n_acompcor_separate": n_acompcor_separate,
-                                   "fd_threshold": None}   
-
-        # Check parcel_apprach
-        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_approach)
-
-        if self._signal_clean_info["use_confounds"]:
-            self._signal_clean_info["confound_names"] = _check_confound_names(high_pass=high_pass, specified_confound_names=confound_names, n_acompcor_separate=n_acompcor_separate)
-            self._signal_clean_info["fd_threshold"] = fd_threshold
-
-    def get_bold(self, bids_dir: str, task: str, session: Union[int,str]=None, runs: list[int]=None, condition: str=None, tr: Union[int, float]=None, 
-                 run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False,
-                 exclude_niftis: list[str]=None) -> None: 
-        """Get Bold Data
-
-        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
-
-        Parameters
-        ----------
-        bids_dir : str
-            Path to a BIDS compliant directory. 
-        task : str, default="rest"
-            Task name.
-        session : int, default=None
-            Session to extract timeseries from. Only a single session can be extracted at a time. 
-        runs : list[int], default=None
-            Run number to extract timeseries data from. Extracts all runs if unspecified.
-        condition : str, default=None
-            Specific condition in the task to extract from. Only a single condition can be extracted at a time.
-        tr : int or float, default=None
-            Repetition time.
-        run_subjects : list[str], default=None
-            List of subject IDs to process. Processes all subjects if None.
-        exclude_subjects : list[str], default=None
-            List of subject IDs to exclude.  
-        pipeline_name: str, default=None
-            The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
-            should be used if their are multiple pipelines in the derivatives folder.
-        n_cores: bool or int, default=None
-            The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
-        verbose: bool, default=True
-            Print subject specific information such as confounds being extracted and id and run of subject being processed during timeseries extraction.
-        flush_print: bool, default=False
-            Flush the printed subject specific infomation produced during the timeseries extraction process.
-        exclude_niftis: list[str], default=None
-            Exclude certain preprocessed nifti files to prevent the timeseries of that file from being extracted. Used if there are specific runs across differnt participants that need to be
-            excluded.
-        """
-        import bids, multiprocessing
-
-        if sys.platform == "win32":
-            raise SystemError("Cannot use this method on Windows devices since it relies on the `pybids` module which is only compatable with POSIX systems.")
-
-        # Update attributes
-        self._task_info = {"task": task, "condition": condition, "session": session, "runs": runs, "tr": tr}
-
-        # Intiialize new attributes
-        self._subject_ids = []
-        self._subject_timeseries = {}
-        self._subject_info = {}
-
-        if pipeline_name:
-            layout = bids.BIDSLayout(bids_dir, derivatives=os.path.join(bids_dir, "derivatives", pipeline_name))
-        else:
-            layout = bids.BIDSLayout(bids_dir, derivatives=True)
-
-        print(f"Bids layout collected.", flush=True)
-        print(layout, flush=True)
-        subj_id_list = sorted(layout.get(return_type="id", target="subject", task=task, space=self._space, suffix="bold")) 
-
-        if exclude_subjects: 
-            exclude_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in exclude_subjects]
-            subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id not in exclude_subjects])
-
-        if run_subjects: 
-            run_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in run_subjects]
-            subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id in run_subjects])
-
-        # Setup extraction
-        self._setup_extraction(layout=layout, subj_id_list=subj_id_list, exclude_niftis=exclude_niftis)
-
-        if n_cores:
-            if n_cores == True:
-                self._n_cores = multiprocessing.cpu_count()
-            else:
-                if n_cores > multiprocessing.cpu_count():
-                    raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {multiprocessing.cpu_count()}.")
-                else:
-                    self._n_cores = n_cores
-            
-            # Generate list of tuples for each subject
-            args_list = [(subj_id, self._subject_info[subj_id]["nifti_files"],self._subject_info[subj_id]["mask_files"],self._subject_info[subj_id]["event_files"],
-                          self._subject_info[subj_id]["confound_files"], self._subject_info[subj_id]["confound_metadata_files"], self._subject_info[subj_id]["run_list"],
-                          self._subject_info[subj_id]["tr"], condition, self._parcel_approach, self._signal_clean_info, verbose, flush_print
-                          ) for subj_id in self._subject_ids]
-
-            with multiprocessing.Pool(processes=self._n_cores) as pool:
-                outputs = pool.starmap(_extract_timeseries, args_list)
-            
-            for output in outputs:
-                if isinstance(output, dict):
-                    self._subject_timeseries.update(output)
-
-            # Ensure subjects are sorted
-            self._subject_timeseries = dict(sorted(self._subject_timeseries.items()))
-
-            # Ensure processes close
-            pool.close()
-        else:
-            for subj_id in self._subject_ids:
-
-                subject_timeseries=_extract_timeseries(subj_id=subj_id, nifti_files=self._subject_info[subj_id]["nifti_files"], mask_files=self._subject_info[subj_id]["mask_files"], 
-                                                       event_files=self._subject_info[subj_id]["event_files"], confound_files=self._subject_info[subj_id]["confound_files"],
-                                                       confound_metadata_files=self._subject_info[subj_id]["confound_metadata_files"], run_list=self._subject_info[subj_id]["run_list"], 
-                                                       tr=self._subject_info[subj_id]["tr"], condition=condition, parcel_approach=self._parcel_approach, signal_clean_info=self._signal_clean_info,
-                                                       verbose=verbose, flush_print=flush_print)
-            
-                # Aggregate new timeseries
-                if isinstance(subject_timeseries, dict): self._subject_timeseries.update(subject_timeseries)
-        
-    # Get valid subjects to iterate through
-    def _setup_extraction(self, layout, subj_id_list, exclude_niftis):
-       for subj_id in subj_id_list:
-            if self._task_info["session"]:
-                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"],extension = "nii.gz", subject=subj_id))
-                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "json", subject=subj_id))
-                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
-                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject=subj_id))
-                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "json", subject=subj_id))
-                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "nii.gz", subject=subj_id))
-            else:
-                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
-                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "json", subject=subj_id))
-                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
-                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "tsv", subject=subj_id))
-                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "json", subject=subj_id))
-                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
-            
-            # Remove excluded file from the nifti_files list, which will prevent it from being processed
-            if exclude_niftis and len(nifti_files) != 0:
-                nifti_files = [nifti_file for nifti_file in nifti_files if os.path.basename(nifti_file) not in exclude_niftis]
-
-            # Generate a list of runs to iterate through based on runs in nifti_files
-            if self._task_info["runs"]:
-                check_runs = [f"run-{run}" for run in self._task_info["runs"]] 
-            elif len(nifti_files) != 0:
-                if "run-" in os.path.basename(nifti_files[0]):
-                    check_runs = [re.search("run-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
-                else:
-                   check_runs = [] 
-            else:
-                check_runs = []
-
-            # Generate a list of runs to iterate through based on runs in nifti_files
-            if not self._task_info["session"] and len(nifti_files) != 0:
-                if "ses-" in os.path.basename(nifti_files[0]):
-                    check_sessions = [re.search("ses-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
-                    if len(list(set(check_sessions))) > 1:
-                        raise ValueError(f"`session` not specified but subject {subj_id} has more than one session : {sorted(list(set(check_sessions)))}. In order to continue timeseries extraction, the specific session to extract must be specified.")
-
-            if len(nifti_files) == 0:
-                warnings.warn(f"Skipping subject: {subj_id} due to missing nifti files.")
-                continue
-            
-            if len(mask_files) == 0:
-                warnings.warn(f"Subject: {subj_id} is missing mask file but timeseries extraction will continue.")
-                
-            if self._signal_clean_info["use_confounds"]:
-                if len(confound_files) == 0:
-                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound files.")
-                    continue
-                if len(confound_metadata_files) == 0 and self._signal_clean_info["n_acompcor_separate"]:
-                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks seperately.")
-                    continue
-            
-            if self._task_info["condition"] and len(event_files) == 0:
-                warnings.warn(f"Skipping subject: {subj_id} due to having no event files.")
-                continue
-                
-            if len(check_runs) != 0:
-                run_list = []
-                # Check if at least one run has all files present
-                for run in check_runs:
-                    curr_list = []
-                    # Assess is any of these returns True
-                    curr_list.append(any([run in file for file in nifti_files]))
-                    if self._task_info["condition"]: curr_list.append(any([run in file for file in event_files]))
-                    if self._signal_clean_info["use_confounds"]:
-                        curr_list.append(any([run in file for file in confound_files]))
-                        if self._signal_clean_info["n_acompcor_separate"]: curr_list.append(any([run in file for file in confound_metadata_files]))
-                    if len(mask_files) != 0: curr_list.append(any([run in file for file in mask_files]))
-                    # Append runs that contain all needed files
-                    if all(curr_list): run_list.append(run)
-                
-                # Skip subject if no run has all needed files present
-                if len(run_list) != len(check_runs) or len(run_list) == 0:
-                    if len(run_list) == 0:
-                        if self._task_info["condition"]: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, confound tsv file, confound json file being from the same run.")
-                        else: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, event file, confound tsv file, confound json file being from the same run.")
-                        continue
-                    else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}.")
-            else:
-                run_list = [None]
-            # Add subject list to subject attribute. These are subjects that will be ran
-            self._subject_ids.append(subj_id)
-
-            # Get repetition time for the subject
-            tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
-
-            # Store subject specific information
-            self._subject_info[subj_id] = {"nifti_files": nifti_files, "event_files": event_files, "confound_files": confound_files, "confound_metadata_files": confound_metadata_files, "mask_files": mask_files,
-                                           "tr": tr, "run_list": run_list}
-
-    def timeseries_to_pickle(self, output_dir: str, file_name: str):
-        """Save Bold Data
-
-        Saves the timeseries dictionary as a pickle file where columns are the subject ID and indices are the runs. Each cell contains the timeseries array.
-
-        Parameters
-        ----------
-        output_dir : str
-            Directory to save the file to.
-        file_name : str
-            Name of the file without the "pkl" extension.
-        """
-        import pickle
-
-        if output_dir:
-            if not os.path.exists(output_dir):
-                os.makedirs(output_dir)
-        
-        with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
-            pickle.dump(self._subject_timeseries,f)
-
-    def visualize_bold(self, subj_id: Union[int,str], run: int, roi_indx: Union[int, list[int]]=None, region: str=None, show_figs: bool=True, output_dir: str=None, file_name: str=None, **kwargs):
-        """Plot Bold Data
-
-        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
-
-        Parameters
-        ----------
-        subj_id: str
-            Subject ID, as a string, to plot.
-        run: int
-            The run to plot.
-        roi_indx: int or list[int], default=None
-            The indices of the Schaefer nodes to plot. See self.node_indices for valid node names and indices.
-        region: str, default=None
-            The region of the parcellation to plot. If not None, all nodes in the specified region will be averaged then plotted. See `regions` in self.parcel_approach 
-            for valid regions names.
-        show_figs: bool, defaults=True
-            Whether to show figires or not to show figures
-        output_dir : str
-            Directory to save the file to.
-        file_name : str
-            Name of the file with the extension to signify the file type.
-        kwargs: dict
-            Keyword arguments used when saving figures. Valid keywords include "dpi" and "figsize". If output_dir is not None and no inputs for dpi and format are given,
-            dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (11,5).
-
-        Raises
-        ------
-        ValueError
-            If both `roi_indx` and `region` are specified.
-        AssertionError
-            If `file_name` does not contain an extension to signify the file type.
-
-        Notes
-        -----
-        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
-        the zero index should correspond the first id that is not zero.
-
-        Custom Key Structure:
-        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
-        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
-          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
-          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
-        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
-        
-        Example 
-        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
-
-        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                             "regions": {"Vis" : {"lh": [0,1],
-                                                  "rh": [3,4]},
-                                         "Hippocampus": {"lh": [2],
-                                                         "rh": [5]}}}}
-        """
-    
-        import matplotlib.pyplot as plt, numpy as np
-
-        if isinstance(subj_id,int): subj_id = str(subj_id)
-
-        if roi_indx !=None and region != None:
-            raise ValueError("`roi_indx` and `region` can not be used simultaneously.")
-        
-        if output_dir:
-            if not os.path.exists(output_dir):
-                os.makedirs(output_dir)
-            assert "." in file_name, "`file_name` must be specified if `output_dir` is specified and it must contain an extension to signify the file type."
-
-        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
-                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (11, 5))
-        
-        if kwargs:
-            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
-            if len(invalid_kwargs.keys()) > 0:
-                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
-
-        # Obtain the column indices associated with the rois; add logic for roi_indx == 0 since it would be recognized as False
-        if roi_indx or roi_indx == 0:
-            if type(roi_indx) == int:
-                plot_indxs = roi_indx
-            
-            elif type(roi_indx) == str:
-                # Check if parcellation_approach is custom
-                if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
-                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
-                plot_indxs = self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(roi_indx)
-            
-            elif type(roi_indx) == list:
-                if all([isinstance(indx,int) for indx in roi_indx]):
-                    plot_indxs = np.array(roi_indx)
-                elif all([isinstance(indx,str) for indx in roi_indx]):
-                    # Check if parcellation_approach is custom
-                    if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
-                        _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
-                    plot_indxs = np.array([self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(index) for index in roi_indx])
-                else:
-                    raise ValueError("All elements in `roi_indx` need to be all strings or all integers.")
-                
-        elif region:
-            if "Custom" in self.parcel_approach.keys():
-                if "regions" not in self.parcel_approach["Custom"].keys():
-                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
-                else:
-                    plot_indxs =  np.array(self.parcel_approach["Custom"]["regions"][region]["lh"] + self.parcel_approach["Custom"]["regions"][region]["rh"])
-            else:
-                plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in label])
-        
-        plt.figure(figsize=plot_dict["figsize"])
-
-        if roi_indx or roi_indx == 0: 
-            plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs])
-        elif region:  
-            plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), np.mean(self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs], axis=1))
-            plt.title(region)
-        plt.xlabel("TR")
-
-        if output_dir:
-            plt.savefig(os.path.join(output_dir,file_name), dpi=plot_dict["dpi"])
-
-        if show_figs == False:
-            plt.close()
-
-
-
-        
-        
-        
+import json, os, re, sys, warnings
+from typing import Union
+from .._utils import _TimeseriesExtractorGetter, _check_confound_names, _check_parcel_approach, _extract_timeseries
+
+class TimeseriesExtractor(_TimeseriesExtractorGetter):
+    def __init__(self, space: str="MNI152NLin2009cAsym", standardize: Union[bool,str]="zscore_sample", detrend: bool=False , low_pass: float=None, high_pass: float=None, 
+                 parcel_approach : dict={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}, use_confounds: bool=True, confound_names: list[str]=None, 
+                 fwhm: float=None, fd_threshold: float=None, n_acompcor_separate: int=None, dummy_scans: int=None):
+        """Timeseries Extractor Class
+        
+        Initializes a TimeseriesExtractor to prepare for Co-activation Patterns (CAPs) analysis.
+
+        Parameters
+        ----------
+        space : str, default="MNI152NLin2009cAsym"
+            The brain template space data is in. 
+        standardize : bool, default=True
+            Determines whether to standardize the timeseries. Refer to Nilearn's NiftiLabelsMasker for available options. 
+        detrend : bool, default=True
+            Detrends timeseries during extraction.
+        low_pass : bool, default=None
+            Signals above cutoff frequency will be filtered out.
+        high_pass : float, default=None
+            Signals below cutoff frequency will be filtered out.
+        parcel_approach : dict, default={"Schaefer": {"n_rois": 400, "yeo_networks": 7, "resolution_mm": 1}}
+            Approach to use to parcellate bold images. Should be in the form of a nested dictionary where the first key is the atlas.
+            Currently only "Schaefer", "AAL", and "Custom" is supported. For the sub-dictionary for "Schaefer", available options includes "n_rois", "yeo_networks", and "resolution_mm".
+            Please refer to the documentation for Nilearn's `datasets.fetch_atlas_schaefer_2018` for valid inputs. For the subdictionary for "AAL" only "version"
+            is an option. Please refer to the documentation for Nilearn's `datasets.fetch_atlas_aal` for valid inputs. As of version 0.8.9, you can replace "Schaefer"
+            and "AAL" with "Custom". At minimum, if "Custom" is specified, a subkey, called "maps" specifying the directory location of the parcellation as a Nifti (e.g .nii or .nii.gz)
+            - {"Custom": {"maps": "/location/to/parcellation.nii.gz"}}.
+        use_confounds : bool, default=True
+            To use confounds when extracting timeseries.
+        confound_names : List[str], default=None
+            Names of confounds to use in confound files. If None, default confounds are used.
+        fwhm : float, default=None
+            Parameter for spatial smoothing.
+        fd_threshold : float, default=None
+            Threshold criteria to remove volume after nuisance regression and timeseries extraction. For this to work, a column named "framewise_displacement" must be
+            in the confounds dataframe and `use_confounds` must be true. Additionally, 'framewise_displacemnt' does not need to be specified in the `confound_names` for this to work.
+        n_acompcor_separate : int, default = None
+            The number of seperate acompcor components derived from the white-matter (WM) and cerebrospinal (CSF) masks to use. For instance if '5' is assigned to this parameter
+            then the first five components derived from the WM mask and the first five components derived from the CSF mask will be used, resulting in ten acompcor components being
+            used. If this parameter is not none any acompcor components listed in the confound names will be disregarded in order to locate the first 'n' components derived from the 
+            masks. To use the acompcor components derived from the combined masks (WM & CSF) leave this parameter as 'None' and list the specific acompcors of interest in the 
+            `confound_names` parameter.
+        dummy_scans : float, default=None
+            Removes the first `n` number of volumes before extracting timeseries.
+        
+        Notes for `confounds_names`
+        --------------------------
+        For the `confound_names` parameter, an asterisk ("*") can be used to find the name of confounds that starts with the term preceding the asterisk.
+        For instance, "cosine*" will find all confound names in the confound files starting with "cosine".
+
+        Notes for `parcel_approach`
+        ---------------------------
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
+        the zero index should correspond the first id that is not zero.
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+        - nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+          For timeseries extraction, this key is not required.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For timeseries extraction, this key is not required.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+        """
+        self._space = space
+        self._signal_clean_info = {"standardize": standardize, "detrend": detrend, "low_pass": low_pass, "high_pass": high_pass, "fwhm": fwhm, 
+                                   "dummy_scans": dummy_scans, "use_confounds": use_confounds,  "n_acompcor_separate": n_acompcor_separate,
+                                   "fd_threshold": None}   
+
+        # Check parcel_apprach
+        self._parcel_approach = _check_parcel_approach(parcel_approach=parcel_approach)
+
+        if self._signal_clean_info["use_confounds"]:
+            self._signal_clean_info["confound_names"] = _check_confound_names(high_pass=high_pass, specified_confound_names=confound_names, n_acompcor_separate=n_acompcor_separate)
+            self._signal_clean_info["fd_threshold"] = fd_threshold
+
+    def get_bold(self, bids_dir: str, task: str, session: Union[int,str]=None, runs: list[int]=None, condition: str=None, tr: Union[int, float]=None, 
+                 run_subjects: list[str]=None, exclude_subjects: list[str]= None, pipeline_name: str=None, n_cores: Union[bool, int]=None, verbose: bool=True, flush_print: bool=False,
+                 exclude_niftis: list[str]=None) -> None: 
+        """Get Bold Data
+
+        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
+
+        Parameters
+        ----------
+        bids_dir : str
+            Path to a BIDS compliant directory. 
+        task : str, default="rest"
+            Task name.
+        session : int, default=None
+            Session to extract timeseries from. Only a single session can be extracted at a time. 
+        runs : list[int], default=None
+            Run number to extract timeseries data from. Extracts all runs if unspecified.
+        condition : str, default=None
+            Specific condition in the task to extract from. Only a single condition can be extracted at a time.
+        tr : int or float, default=None
+            Repetition time.
+        run_subjects : list[str], default=None
+            List of subject IDs to process. Processes all subjects if None.
+        exclude_subjects : list[str], default=None
+            List of subject IDs to exclude.  
+        pipeline_name: str, default=None
+            The name of the pipeline folder in the derivatives folder containing the preprocessed data. If None, BIDSLayout will use the name of dset_dir with derivatives=True. This parameter
+            should be used if their are multiple pipelines in the derivatives folder.
+        n_cores: bool or int, default=None
+            The number of CPU cores to use for multiprocessing. If true, all available cores will be used.
+        verbose: bool, default=True
+            Print subject specific information such as confounds being extracted and id and run of subject being processed during timeseries extraction.
+        flush_print: bool, default=False
+            Flush the printed subject specific infomation produced during the timeseries extraction process.
+        exclude_niftis: list[str], default=None
+            Exclude certain preprocessed nifti files to prevent the timeseries of that file from being extracted. Used if there are specific runs across differnt participants that need to be
+            excluded.
+        """
+        import bids, multiprocessing
+
+        if sys.platform == "win32":
+            raise SystemError("Cannot use this method on Windows devices since it relies on the `pybids` module which is only compatable with POSIX systems.")
+
+        # Update attributes
+        self._task_info = {"task": task, "condition": condition, "session": session, "runs": runs, "tr": tr}
+
+        # Intiialize new attributes
+        self._subject_ids = []
+        self._subject_timeseries = {}
+        self._subject_info = {}
+
+        if pipeline_name:
+            layout = bids.BIDSLayout(bids_dir, derivatives=os.path.join(bids_dir, "derivatives", pipeline_name))
+        else:
+            layout = bids.BIDSLayout(bids_dir, derivatives=True)
+
+        print(f"Bids layout collected.", flush=True)
+        print(layout, flush=True)
+        subj_id_list = sorted(layout.get(return_type="id", target="subject", task=task, space=self._space, suffix="bold")) 
+
+        if exclude_subjects: 
+            exclude_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in exclude_subjects]
+            subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id not in exclude_subjects])
+
+        if run_subjects: 
+            run_subjects = [str(subj_id) if not isinstance(subj_id,str) else subj_id for subj_id in run_subjects]
+            subj_id_list = sorted([subj_id for subj_id in subj_id_list if subj_id in run_subjects])
+
+        # Setup extraction
+        self._setup_extraction(layout=layout, subj_id_list=subj_id_list, exclude_niftis=exclude_niftis)
+
+        if n_cores:
+            if n_cores == True:
+                self._n_cores = multiprocessing.cpu_count()
+            else:
+                if n_cores > multiprocessing.cpu_count():
+                    raise ValueError(f"More cores specified than available - Number of cores specified: {n_cores}; Max cores available: {multiprocessing.cpu_count()}.")
+                else:
+                    self._n_cores = n_cores
+            
+            # Generate list of tuples for each subject
+            args_list = [(subj_id, self._subject_info[subj_id]["nifti_files"],self._subject_info[subj_id]["mask_files"],self._subject_info[subj_id]["event_files"],
+                          self._subject_info[subj_id]["confound_files"], self._subject_info[subj_id]["confound_metadata_files"], self._subject_info[subj_id]["run_list"],
+                          self._subject_info[subj_id]["tr"], condition, self._parcel_approach, self._signal_clean_info, verbose, flush_print
+                          ) for subj_id in self._subject_ids]
+
+            with multiprocessing.Pool(processes=self._n_cores) as pool:
+                outputs = pool.starmap(_extract_timeseries, args_list)
+            
+            for output in outputs:
+                if isinstance(output, dict):
+                    self._subject_timeseries.update(output)
+
+            # Ensure subjects are sorted
+            self._subject_timeseries = dict(sorted(self._subject_timeseries.items()))
+
+            # Ensure processes close
+            pool.close()
+        else:
+            for subj_id in self._subject_ids:
+
+                subject_timeseries=_extract_timeseries(subj_id=subj_id, nifti_files=self._subject_info[subj_id]["nifti_files"], mask_files=self._subject_info[subj_id]["mask_files"], 
+                                                       event_files=self._subject_info[subj_id]["event_files"], confound_files=self._subject_info[subj_id]["confound_files"],
+                                                       confound_metadata_files=self._subject_info[subj_id]["confound_metadata_files"], run_list=self._subject_info[subj_id]["run_list"], 
+                                                       tr=self._subject_info[subj_id]["tr"], condition=condition, parcel_approach=self._parcel_approach, signal_clean_info=self._signal_clean_info,
+                                                       verbose=verbose, flush_print=flush_print)
+            
+                # Aggregate new timeseries
+                if isinstance(subject_timeseries, dict): self._subject_timeseries.update(subject_timeseries)
+        
+    # Get valid subjects to iterate through
+    def _setup_extraction(self, layout, subj_id_list, exclude_niftis):
+       for subj_id in subj_id_list:
+            if self._task_info["session"]:
+                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"],extension = "nii.gz", subject=subj_id))
+                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "json", subject=subj_id))
+                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
+                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "tsv", subject=subj_id))
+                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], session=self._task_info["session"],extension = "json", subject=subj_id))
+                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, session=self._task_info["session"], extension = "nii.gz", subject=subj_id))
+            else:
+                nifti_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
+                bold_metadata_files = sorted(layout.get(scope="derivatives", return_type="file",suffix="bold", task=self._task_info["task"], space=self._space, extension = "json", subject=subj_id))
+                event_files = sorted([file for file in sorted(layout.get(return_type="filename",suffix="events", task=self._task_info["task"], extension = "tsv", subject = subj_id))]) if self._task_info["condition"] else []
+                confound_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "tsv", subject=subj_id))
+                confound_metadata_files = sorted(layout.get(scope='derivatives', return_type='file', desc='confounds', task=self._task_info["task"], extension = "json", subject=subj_id))
+                mask_files = sorted(layout.get(scope='derivatives', return_type='file', suffix='mask', task=self._task_info["task"], space=self._space, extension = "nii.gz", subject=subj_id))
+            
+            # Remove excluded file from the nifti_files list, which will prevent it from being processed
+            if exclude_niftis and len(nifti_files) != 0:
+                nifti_files = [nifti_file for nifti_file in nifti_files if os.path.basename(nifti_file) not in exclude_niftis]
+
+            # Generate a list of runs to iterate through based on runs in nifti_files
+            if self._task_info["runs"]:
+                check_runs = [f"run-{run}" for run in self._task_info["runs"]] 
+            elif len(nifti_files) != 0:
+                if "run-" in os.path.basename(nifti_files[0]):
+                    check_runs = [re.search("run-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
+                else:
+                   check_runs = [] 
+            else:
+                check_runs = []
+
+            # Generate a list of runs to iterate through based on runs in nifti_files
+            if not self._task_info["session"] and len(nifti_files) != 0:
+                if "ses-" in os.path.basename(nifti_files[0]):
+                    check_sessions = [re.search("ses-(\\S+?)[-_]",os.path.basename(x))[0][:-1] for x in nifti_files]
+                    if len(list(set(check_sessions))) > 1:
+                        raise ValueError(f"`session` not specified but subject {subj_id} has more than one session : {sorted(list(set(check_sessions)))}. In order to continue timeseries extraction, the specific session to extract must be specified.")
+
+            if len(nifti_files) == 0:
+                warnings.warn(f"Skipping subject: {subj_id} due to missing nifti files.")
+                continue
+            
+            if len(mask_files) == 0:
+                warnings.warn(f"Subject: {subj_id} is missing mask file but timeseries extraction will continue.")
+                
+            if self._signal_clean_info["use_confounds"]:
+                if len(confound_files) == 0:
+                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound files.")
+                    continue
+                if len(confound_metadata_files) == 0 and self._signal_clean_info["n_acompcor_separate"]:
+                    warnings.warn(f"Skipping subject: {subj_id} due to missing confound metadata to locate the first six components of the white-matter and cerobrospinal fluid masks seperately.")
+                    continue
+            
+            if self._task_info["condition"] and len(event_files) == 0:
+                warnings.warn(f"Skipping subject: {subj_id} due to having no event files.")
+                continue
+                
+            if len(check_runs) != 0:
+                run_list = []
+                # Check if at least one run has all files present
+                for run in check_runs:
+                    curr_list = []
+                    # Assess is any of these returns True
+                    curr_list.append(any([run in file for file in nifti_files]))
+                    if self._task_info["condition"]: curr_list.append(any([run in file for file in event_files]))
+                    if self._signal_clean_info["use_confounds"]:
+                        curr_list.append(any([run in file for file in confound_files]))
+                        if self._signal_clean_info["n_acompcor_separate"]: curr_list.append(any([run in file for file in confound_metadata_files]))
+                    if len(mask_files) != 0: curr_list.append(any([run in file for file in mask_files]))
+                    # Append runs that contain all needed files
+                    if all(curr_list): run_list.append(run)
+                
+                # Skip subject if no run has all needed files present
+                if len(run_list) != len(check_runs) or len(run_list) == 0:
+                    if len(run_list) == 0:
+                        if self._task_info["condition"]: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, confound tsv file, confound json file being from the same run.")
+                        else: warnings.warn(f"Skipping subject: {subj_id} due to no nifti file, mask file, event file, confound tsv file, confound json file being from the same run.")
+                        continue
+                    else: warnings.warn(f"Subject: {subj_id} only has the following runs available: {', '.join(run_list)}.")
+            else:
+                run_list = [None]
+            # Add subject list to subject attribute. These are subjects that will be ran
+            self._subject_ids.append(subj_id)
+
+            # Get repetition time for the subject
+            tr = self._task_info["tr"] if self._task_info["tr"] else json.load(open(bold_metadata_files[0]))["RepetitionTime"]
+
+            # Store subject specific information
+            self._subject_info[subj_id] = {"nifti_files": nifti_files, "event_files": event_files, "confound_files": confound_files, "confound_metadata_files": confound_metadata_files, "mask_files": mask_files,
+                                           "tr": tr, "run_list": run_list}
+
+    def timeseries_to_pickle(self, output_dir: str, file_name: str):
+        """Save Bold Data
+
+        Saves the timeseries dictionary as a pickle file where columns are the subject ID and indices are the runs. Each cell contains the timeseries array.
+
+        Parameters
+        ----------
+        output_dir : str
+            Directory to save the file to.
+        file_name : str
+            Name of the file without the "pkl" extension.
+        """
+        import pickle
+
+        if output_dir:
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
+        
+        with open(os.path.join(output_dir,file_name + ".pkl"), "wb") as f:
+            pickle.dump(self._subject_timeseries,f)
+
+    def visualize_bold(self, subj_id: Union[int,str], run: int, roi_indx: Union[int, list[int]]=None, region: str=None, show_figs: bool=True, output_dir: str=None, file_name: str=None, **kwargs):
+        """Plot Bold Data
+
+        Collects files needed to extract timeseries data from NIfTI files for BIDS-compliant datasets.
+
+        Parameters
+        ----------
+        subj_id: str
+            Subject ID, as a string, to plot.
+        run: int
+            The run to plot.
+        roi_indx: int or list[int], default=None
+            The indices of the Schaefer nodes to plot. See self.node_indices for valid node names and indices.
+        region: str, default=None
+            The region of the parcellation to plot. If not None, all nodes in the specified region will be averaged then plotted. See `regions` in self.parcel_approach 
+            for valid regions names.
+        show_figs: bool, defaults=True
+            Whether to show figires or not to show figures
+        output_dir : str
+            Directory to save the file to.
+        file_name : str
+            Name of the file with the extension to signify the file type.
+        kwargs: dict
+            Keyword arguments used when saving figures. Valid keywords include "dpi" and "figsize". If output_dir is not None and no inputs for dpi and format are given,
+            dpi defaults to 300. If "figsize" has no input, figure sizes defaults to (11,5).
+
+        Raises
+        ------
+        ValueError
+            If both `roi_indx` and `region` are specified.
+        AssertionError
+            If `file_name` does not contain an extension to signify the file type.
+
+        Notes
+        -----
+        If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. Also, this function assumes that the background label is "zero". Do not add a a background label, in the "nodes" or "networks" key,
+        the zero index should correspond the first id that is not zero.
+
+        Custom Key Structure:
+        - maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this label is not required.
+        - nodes: A list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+          Each label should match the parcellation index it represents. For example, if the parcellation label "1" corresponds to the left hemisphere 
+          visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended.
+        - regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes.
+        
+        Example 
+        The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+        parcel_approach = {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+        """
+    
+        import matplotlib.pyplot as plt, numpy as np
+
+        if isinstance(subj_id,int): subj_id = str(subj_id)
+
+        if roi_indx !=None and region != None:
+            raise ValueError("`roi_indx` and `region` can not be used simultaneously.")
+        
+        if output_dir:
+            if not os.path.exists(output_dir):
+                os.makedirs(output_dir)
+            assert "." in file_name, "`file_name` must be specified if `output_dir` is specified and it must contain an extension to signify the file type."
+
+        plot_dict = dict(dpi = kwargs["dpi"] if kwargs and "dpi" in kwargs.keys() else 300,
+                         figsize = kwargs["figsize"] if kwargs and "figsize" in kwargs.keys() else (11, 5))
+        
+        if kwargs:
+            invalid_kwargs = {key : value for key, value in kwargs.items() if key not in plot_dict.keys()}
+            if len(invalid_kwargs.keys()) > 0:
+                print(f"Invalid kwargs arguments used and will be ignored {invalid_kwargs}.")
+
+        # Obtain the column indices associated with the rois; add logic for roi_indx == 0 since it would be recognized as False
+        if roi_indx or roi_indx == 0:
+            if type(roi_indx) == int:
+                plot_indxs = roi_indx
+            
+            elif type(roi_indx) == str:
+                # Check if parcellation_approach is custom
+                if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                plot_indxs = self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(roi_indx)
+            
+            elif type(roi_indx) == list:
+                if all([isinstance(indx,int) for indx in roi_indx]):
+                    plot_indxs = np.array(roi_indx)
+                elif all([isinstance(indx,str) for indx in roi_indx]):
+                    # Check if parcellation_approach is custom
+                    if "Custom" in self.parcel_approach.keys() and "nodes" not in self.parcel_approach["Custom"].keys():
+                        _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                    plot_indxs = np.array([self._parcel_approach[self._parcel_approach.keys[0]]["nodes"].index(index) for index in roi_indx])
+                else:
+                    raise ValueError("All elements in `roi_indx` need to be all strings or all integers.")
+                
+        elif region:
+            if "Custom" in self.parcel_approach.keys():
+                if "regions" not in self.parcel_approach["Custom"].keys():
+                    _check_parcel_approach(parcel_approach=self._parcel_approach, call="visualize_bold")
+                else:
+                    plot_indxs =  np.array(self.parcel_approach["Custom"]["regions"][region]["lh"] + self.parcel_approach["Custom"]["regions"][region]["rh"])
+            else:
+                plot_indxs = np.array([index for index, label in enumerate(self._parcel_approach[list(self._parcel_approach.keys())[0]]["nodes"]) if region in label])
+        
+        plt.figure(figsize=plot_dict["figsize"])
+
+        if roi_indx or roi_indx == 0: 
+            plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs])
+        elif region:  
+            plt.plot(range(1, self._subject_timeseries[subj_id][f"run-{run}"].shape[0] + 1), np.mean(self._subject_timeseries[subj_id][f"run-{run}"][:,plot_indxs], axis=1))
+            plt.title(region)
+        plt.xlabel("TR")
+
+        if output_dir:
+            plt.savefig(os.path.join(output_dir,file_name), dpi=plot_dict["dpi"])
+
+        if show_figs == False:
+            plt.close()
+        else:
+            plt.show()
+
+
+
+        
+        
+
```

### Comparing `neurocaps-0.9.0.post4/neurocaps.egg-info/PKG-INFO` & `neurocaps-0.9.0.post5/neurocaps.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,218 +1,221 @@
-Metadata-Version: 2.1
-Name: neurocaps
-Version: 0.9.0.post4
-Summary: Co-activation patterns Python package
-Author-email: Donisha Smith <donishasmith@outlook.com>
-Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
-Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
-Classifier: Intended Audience :: Education
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.12
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: Microsoft :: Windows :: Windows 11
-Classifier: Development Status :: 4 - Beta
-Requires-Python: >=3.9.0
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-Requires-Dist: numpy
-Requires-Dist: pandas
-Requires-Dist: matplotlib
-Requires-Dist: seaborn
-Requires-Dist: kneed
-Requires-Dist: nibabel
-Requires-Dist: nilearn==0.10.2
-Requires-Dist: surfplot
-Requires-Dist: neuromaps
-Requires-Dist: pybids; platform_system != "Windows"
-
-# neurocaps
-This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
-
-**Still in beta but stable.**
-
-# Installation
-
-**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
-
-To install, using your preferred terminal:
-
-**Installation with pip:**
-
-```bash
-
-pip install neurocaps
-
-```
-
-**From source (Development version):**
-
-```bash
-pip install git+https://github.com/donishadsmith/neurocaps.git
-```
-
-or
-
-```bash
-
-git clone https://github.com/donishadsmith/neurocaps/
-cd neurocaps
-pip install -e .
-
-```
-
-# Usage
-**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
-
-**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
-
-If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
-
-Custom Key Structure:
-- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
-- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
-Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
-visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
-- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
-        
-Example 
-The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
-
-```Python
-parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
-                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
-                             "regions": {"Vis" : {"lh": [0,1],
-                                                  "rh": [3,4]},
-                                         "Hippocampus": {"lh": [2],
-                                                         "rh": [5]}}}}
- ```
-
-**Main features for `TimeseriesExtractor` includes:**
-
-- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
-- Saving the nested dictionary containing timeseries as a pickle file.
-- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
-- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
-
-**Main features for `CAP` includes:**
-
-- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
-- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
-- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
-- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
-different CAPs across the entire run.
-
-**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
-
-Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
-
-Quick code example:
-
-```python
-# Examples use randomized data
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-"""If an asterisk '*' is after a name, all confounds starting with the 
-term preceding the parameter will be used. in this case, all parameters 
-starting with cosine will be used."""
-confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
-             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
-             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
-             "rot_z","rot_z_derivative1"]
-
-"""If use_confounds is True but no confound_names provided, there are hardcoded 
-confound names that will extract the data from the confound files outputted by fMRIPrep
-`n_acompcor_separate` will use the first 'n' components derived from the separate 
-white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
-combined mask, list them in the `confound_names` parameter"""
-parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
-
-extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
-                                 confound_names=confounds, n_acompcor_separate=6)
-
-bids_dir = "/path/to/bids/dir"
-
-# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
-pipeline_name = "fmriprep-1.4.0"
-
-# Resting State
-# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
-
-# Task; use parallel processing with `n_cores`
-extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
-                   pipeline_name=pipeline_name, n_cores=10)
-
-cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
-                    n_clusters=6)
-
-cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
-                      standardize = True)
-
-# Visualize CAPs
-cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3, sharey=True, 
-                            subplots=True)
-
-cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
-                            task_title="- Positive Valence", ncol=3,sharey=True, 
-                            subplots=True, xlabel_rotation=90, tight_layout=False, 
-                            hspace = 0.4)
-
-```
-**Graph Outputs:**
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
-
-```python
-
-# Get CAP metrics
-outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
-                                         return_df=True, output_dir=output_dir,
-                                         metrics=["temporal fraction", "persistence"],
-                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
-
-print(outputs["temporal fraction"])
-```
-**DataFrame Output:**
-| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
-| --- | --- | --- | --- | --- | --- | --- | --- | --- |
-| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
-| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
-| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
-| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
-| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
-| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
-| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
-| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
-| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
-| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
-
-```python
-# If you experience coverage issues, usually smoothing helps to mitigate these issues
-cap_analysis.caps2surf(fwhm=2)
-```
-![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
-
-# Testing 
-This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
-
-Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
-
-
-# References
-[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
-
-[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
-
-[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
-
-[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
-
-[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
-
-[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
+Metadata-Version: 2.1
+Name: neurocaps
+Version: 0.9.0.post5
+Summary: Co-activation patterns Python package
+Author-email: Donisha Smith <donishasmith@outlook.com>
+Project-URL: Homepage, https://github.com/donishadsmith/neurocaps
+Keywords: python,Co-Activation Patterns,CAPs,neuroimaging,fmri,dfc,dynamic functional connectivity,fMRIPrep
+Classifier: Intended Audience :: Education
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: Microsoft :: Windows :: Windows 11
+Classifier: Development Status :: 4 - Beta
+Requires-Python: >=3.9.0
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+Requires-Dist: numpy
+Requires-Dist: pandas
+Requires-Dist: matplotlib
+Requires-Dist: seaborn
+Requires-Dist: kneed
+Requires-Dist: nibabel
+Requires-Dist: nilearn==0.10.2
+Requires-Dist: surfplot
+Requires-Dist: neuromaps
+Requires-Dist: pybids; platform_system != "Windows"
+
+# neurocaps
+This is a Python package to perform Co-activation Patterns (CAPs) analyses, which involves using kmeans clustering to group timepoints (TR's) into brain states, on both resting-state or task data. It is compatible with data preprocessed with **fMRIPrep** and assumes your directory is BIDS-compliant and contains a derivatives folder with a pipeline folder, such as fMRIPrep, containing preprocessed BOLD data.
+
+**Still in beta but stable.**
+
+# Installation
+
+**Note**: The `.get_bold()` method in the `TimeseriesExtractor` class in this package uses pybids, which is only functional on POSIX operating system and Mac OS. Assuming you have a pickled timeseries dictionary in the proper nested form, this package can be used on windows to visualize the bold timeseries, use the `CAP` class, and the `merge_dicts()` fuction. 
+
+To install, using your preferred terminal:
+
+**Installation with pip:**
+
+```bash
+
+pip install neurocaps
+
+```
+
+**From source (Development version):**
+
+```bash
+pip install git+https://github.com/donishadsmith/neurocaps.git
+```
+
+or
+
+```bash
+
+git clone https://github.com/donishadsmith/neurocaps/
+cd neurocaps
+pip install -e .
+
+```
+
+# Usage
+**This package contains two main classes - `TimeseriesExtractor`, for extracting the timeseries, and `CAP`, for performing the CAPs analysis.**
+
+**Note**: When extracting the timeseries, **this package uses the Schaefer atlas, the Automated Anatomical Labeling (AAL) atlas, or a custom parcellation where all nodes has a left and right version**. The number of ROIs and networks for the Schaefer atlas can be modified with the `parcel_approach` parameter when initializing the main `TimeseriesExtractor` class. To modify it, you must use a nested dictionary, where the primary key is "Schaefer" and the sub-keys are "n_rois" and "yeo_networks". Example: `parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm: 1}}`. Similary, the version of the AAL atlas can be modified using `parcel_approach = {"AAL": {"version": "SPM12"}}`. 
+
+If using a "Custom" parcellation approach, ensure each node in your dataset includes both left (lh) and right (rh) hemisphere versions. 
+
+Custom Key Structure:
+- maps: Directory path containing necessary parcellation files. Ensure files are in a supported format (e.g., .nii for NIfTI files). For plotting purposes, this key is not required.
+- nodes:  list of all node labels used in your study, arranged in the exact order they correspond to indices in your parcellation files. 
+Each label should match the parcellation index it represents. For example, if the parcellation label "0" corresponds to the left hemisphere 
+visual cortex area 1, then "LH_Vis1" should occupy the 0th index in this list. This ensures that data extraction and analysis accurately reflect the anatomical regions intended. For timeseries extraction, this key is not required.
+- regions: Dictionary defining major brain regions. Each region should list node indices under "lh" and "rh" to specify left and right hemisphere nodes. For    timeseries extraction, this key is not required.
+        
+Example 
+The provided example demonstrates setting up a custom parcellation containing nodes for the visual network (Vis) and hippocampus regions:
+
+```Python
+parcel_approach= {"Custom": {"maps": "/location/to/parcellation.nii.gz",
+                             "nodes": ["LH_Vis1", "LH_Vis2", "LH_Hippocampus", "RH_Vis1", "RH_Vis2", "RH_Hippocampus"],
+                             "regions": {"Vis" : {"lh": [0,1],
+                                                  "rh": [3,4]},
+                                         "Hippocampus": {"lh": [2],
+                                                         "rh": [5]}}}}
+ ```
+
+**Main features for `TimeseriesExtractor` includes:**
+
+- Timeseries extraction for resting state or task data and creating a nested dictionary containing the subject ID, run number, and associated timeseries. This is used as input for the `get_caps()` method in the `CAP` class.
+- Saving the nested dictionary containing timeseries as a pickle file.
+- Visualizing the timeseries of a Schaefer or AAL node or network subject's run. Also includes the ability to save plots.
+- Ability to use parallel processing by specifiying the number of CPU cores to use in the `n_cores` parameter in the `get_bold()` method. Testing on an HPC using a loop with `TimeseriesExtractor.get_bold()` to extract the session 1 and 2 bold timeries from 105 subjects from resting-state data (single-run containing 360 volumes) and two task datasets (three-runs containing 200 volumes each and two-runs containing 200 volumes) reduced processing time from 5 hrs 48 mins to 1 hr 26 mins (using 10 cores).
+
+**Main features for `CAP` includes:**
+
+- Performing the silhouette or elbow method to identify the optimal cluster size. When the optimal cluster size is identified, the optimal model is saved as an attribute.
+- Visualizing the CAPs identified as an outer product or regular heatmap. For outer products, you also have the ability to use subplots to reduce the number of individual plots. You can also save the plots and use them. Please refer to the docstring for the `visualize_caps()` method in the `CAP` class to see the list of available kwargs arguments to modify plots.
+- Grouping feature to perform CAPs independently on groups of subject IDs. When grouping is specified, k-means clustering, silhouette and elbow methods, as well as plotting, are done for each independent group.
+- Calculating CAP metrics as described in [Liu et al., 2018](https://doi.org/10.1016/j.neuroimage.2018.01.041)[^1] and [Yang et al., 2021](https://doi.org/10.1016/j.neuroimage.2021.118193)[^2], where *temporal fraction* is the proportion of total volumes spent in a single CAP over all volumes in a run, *persistence* is the average time spent in a single CAP before transitioning to another CAP (average consecutive/uninterrupted time), and *counts* is the frequency of each CAP observed in a run, and *transition frequency* is the number of switches between
+different CAPs across the entire run.
+
+**Additionally, the `neurocaps.analysis` submodule contains the `merge_dicts` function, which allows you to merge the subject_timeseries dictionaries (merged dictionary will be returned and can be saved as a pickle file) for overlapping subjects across tasks in order to identify similar CAPs across different tasks[^3].**
+
+Please refer to [demo.ipynb](https://github.com/donishadsmith/neurocaps/blob/main/demo.ipynb) to see a more extensive demonstration of the features included in this package. 
+
+Quick code example:
+
+```python
+# Examples use randomized data
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+"""If an asterisk '*' is after a name, all confounds starting with the 
+term preceding the parameter will be used. in this case, all parameters 
+starting with cosine will be used."""
+confounds = ["cosine*", "trans_x", "trans_x_derivative1", "trans_y", 
+             "trans_y_derivative1", "trans_z","trans_z_derivative1", 
+             "rot_x", "rot_x_derivative1", "rot_y", "rot_y_derivative1", 
+             "rot_z","rot_z_derivative1"]
+
+"""If use_confounds is True but no confound_names provided, there are hardcoded 
+confound names that will extract the data from the confound files outputted by fMRIPrep
+`n_acompcor_separate` will use the first 'n' components derived from the separate 
+white-matter (WM) and cerebrospinal fluid (CSF). To use the acompcor components from the 
+combined mask, list them in the `confound_names` parameter"""
+parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7, "resolution_mm": 2}}
+
+extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                 use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01, 
+                                 confound_names=confounds, n_acompcor_separate=6)
+
+bids_dir = "/path/to/bids/dir"
+
+# If there are multiple pipelines in the derivatives folder, you can specify a specific pipeline
+pipeline_name = "fmriprep-1.4.0"
+
+# Resting State
+# extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name)
+
+# Task; use parallel processing with `n_cores`
+extractor.get_bold(bids_dir=bids_dir, task="emo", condition="positive", 
+                   pipeline_name=pipeline_name, n_cores=10)
+
+cap_analysis = CAP(parcel_approach=extractor.parcel_approach,
+                    n_clusters=6)
+
+cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries, 
+                      standardize = True)
+
+# Visualize CAPs
+cap_analysis.visualize_caps(visual_scope="regions", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3, sharey=True, 
+                            subplots=True)
+
+cap_analysis.visualize_caps(visual_scope="nodes", plot_options="outer product", 
+                            task_title="- Positive Valence", ncol=3,sharey=True, 
+                            subplots=True, xlabel_rotation=90, tight_layout=False, 
+                            hspace = 0.4)
+
+```
+**Graph Outputs:**
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/4699bbd9-1f55-462b-9d9e-4ef17da79ad4)
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/506c5be5-540d-43a9-8a61-c02062f5c6f9)
+
+```python
+
+# Get CAP metrics
+outputs = cap_analysis.calculate_metrics(subject_timeseries=extractor.subject_timeseries, tr=2.0, 
+                                         return_df=True, output_dir=output_dir,
+                                         metrics=["temporal fraction", "persistence"],
+                                         continuous_runs=True, file_name="All_Subjects_CAPs_metrics")
+
+print(outputs["temporal fraction"])
+```
+**DataFrame Output:**
+| Subject_ID | Group | Run | CAP-1 | CAP-2 | CAP-3 | CAP-4 | CAP-5 | CAP-6 |
+| --- | --- | --- | --- | --- | --- | --- | --- | --- |
+| 1 | All Subjects | Continuous Runs | 0.14 | 0.17 | 0.14 | 0.2 | 0.15 | 0.19 |
+| 2 | All Subjects | Continuous Runs | 0.17 | 0.17 | 0.16 | 0.16 | 0.15 | 0.19 |
+| 3 | All Subjects | Continuous Runs | 0.15 | 0.2 | 0.14 | 0.18 | 0.17 | 0.17 |
+| 4 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.18 | 0.17 | 0.1 | 0.16 |
+| 5 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.16 | 0.2 | 0.18 |
+| 6 | All Subjects | Continuous Runs | 0.16 | 0.21 | 0.16 | 0.18 | 0.16 | 0.13 |
+| 7 | All Subjects | Continuous Runs | 0.16 | 0.16 | 0.17 | 0.15 | 0.19 | 0.17 |
+| 8 | All Subjects | Continuous Runs | 0.17 | 0.21 | 0.13 | 0.14 | 0.17 | 0.18 |
+| 9 | All Subjects | Continuous Runs | 0.18 | 0.1 | 0.17 | 0.18 | 0.16 | 0.2 |
+| 10 | All Subjects | Continuous Runs | 0.14 | 0.19 | 0.14 | 0.17 | 0.19 | 0.16 |
+
+```python
+# If you experience coverage issues, usually smoothing helps to mitigate these issues
+cap_analysis.caps2surf(fwhm=2)
+```
+![image](https://github.com/donishadsmith/neurocaps/assets/112973674/46ea5174-0ded-4640-a1f9-c21e798e0459)
+
+# Testing 
+This package was tested using a closed dataset as well as a modified version of a single subject open dataset to test the TimeseriesExtractor function on Github Actions. Furthermore, the open dataset provided by [Laumann & Poldrack](https://openfmri.org/dataset/ds000031/) and used in [Laumann et al., 2015](https://doi.org/10.1016/j.neuron.2015.06.037)[^4]. Additionally, this data was obtained from the OpenfMRI database. Its accession number is ds000031. Modifications to the data consist of truncating the preprocessed bold data and confounds form 448 timepoints to 34 timepoints, only including session 002 data, adding a dataset_description.json file to the fmriprep folder, excluding the nii.gz file in the root bids folder, only retaining the mask, truncated preprocessed bold file, and truncated confounds file in the fmriprep folder, and slighly changing the naming style of the mask, preprocessed bold file, and confounds file in the fmriprep folder to conform with the naming conventions of modern fmriprep outputs.
+
+Testing with custom parcellations was done with the HCPex parcellation, an extension of the HCP (Human Connectome Project) parcellation, which adds 66 subcortical areas [^5], [^6]. This original atlas can be downloaded from https://github.com/wayalan/HCPex.
+
+
+# References
+[^1]: Liu, X., Zhang, N., Chang, C., & Duyn, J. H. (2018). Co-activation patterns in resting-state fMRI signals. NeuroImage, 180, 485–494. https://doi.org/10.1016/j.neuroimage.2018.01.041
+
+[^2]: Yang, H., Zhang, H., Di, X., Wang, S., Meng, C., Tian, L., & Biswal, B. (2021). Reproducible coactivation patterns of functional brain networks reveal the aberrant dynamic state transition in schizophrenia. NeuroImage, 237, 118193. https://doi.org/10.1016/j.neuroimage.2021.118193
+
+[^3]: Kupis, L., Romero, C., Dirks, B., Hoang, S., Parladé, M. V., Beaumont, A. L., Cardona, S. M., Alessandri, M., Chang, C., Nomi, J. S., & Uddin, L. Q. (2020). Evoked and intrinsic brain network dynamics in children with autism spectrum disorder. NeuroImage: Clinical, 28, 102396. https://doi.org/10.1016/j.nicl.2020.102396
+
+[^4]: Laumann, T. O., Gordon, E. M., Adeyemo, B., Snyder, A. Z., Joo, S. J., Chen, M. Y., Gilmore, A. W., McDermott, K. B., Nelson, S. M., Dosenbach, N. U., Schlaggar, B. L., Mumford, J. A., Poldrack, R. A., & Petersen, S. E. (2015). Functional system and areal organization of a highly sampled individual human brain. Neuron, 87(3), 657–670. https://doi.org/10.1016/j.neuron.2015.06.037
+
+[^5]: Huang CC, Rolls ET, Feng J, Lin CP. An extended Human Connectome Project multimodal parcellation atlas of the human cortex and subcortical areas. Brain Struct Funct. 2022 Apr;227(3):763-778. Epub 2021 Nov 17. doi: 10.1007/s00429-021-02421-6
+
+[^6]: Huang CC, Rolls ET, Hsu CH, Feng J, Lin CP. Extensive Cortical Connectivity of the Human Hippocampal Memory System: Beyond the "What" and "Where" Dual Stream Model. Cerebral Cortex. 2021 May 19;bhab113. doi: 10.1093/cercor/bhab113.
```

### Comparing `neurocaps-0.9.0.post4/neurocaps.egg-info/SOURCES.txt` & `neurocaps-0.9.0.post5/neurocaps.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 neurocaps/__init__.py
 neurocaps.egg-info/PKG-INFO
 neurocaps.egg-info/SOURCES.txt
 neurocaps.egg-info/dependency_links.txt
 neurocaps.egg-info/requires.txt
 neurocaps.egg-info/top_level.txt
 neurocaps/_utils/__init__.py
-neurocaps/_utils/_check_confound_names.py
 neurocaps/_utils/_cap_internals/__init__.py
 neurocaps/_utils/_cap_internals/_capgetter.py
 neurocaps/_utils/_cap_internals/_pickle_to_dict.py
 neurocaps/_utils/_timeseriesextractor_internals/__init__.py
+neurocaps/_utils/_timeseriesextractor_internals/_check_confound_names.py
 neurocaps/_utils/_timeseriesextractor_internals/_check_parcel_approach.py
 neurocaps/_utils/_timeseriesextractor_internals/_extract_timeseries.py
 neurocaps/_utils/_timeseriesextractor_internals/_timeseriesextractorgetter.py
 neurocaps/analysis/__init__.py
 neurocaps/analysis/cap.py
 neurocaps/analysis/merge.py
 neurocaps/analysis/standardize.py
```

### Comparing `neurocaps-0.9.0.post4/tests/test_CAP.py` & `neurocaps-0.9.0.post5/tests/test_CAP.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import os, numpy as np, pickle, pytest, warnings
-
-from neurocaps.extraction import TimeseriesExtractor
-from neurocaps.analysis import CAP
-
-def test_CAP_get_caps_no_groups():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=2)
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
-    
-def test_CAP_get_caps_with_groups():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=2)
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
-
-def test_CAP_get_caps_with_no_groups_and_silhouette_method():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
-
-
-def test_CAP_get_caps_with_groups_and_silhouette_method():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
-
-def test_CAP_get_caps_no_groups_pkl():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    with open("sample_timeseries.pkl", "rb") as f:
-        subject_timeseries = pickle.load(f)
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=2)
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
-    
-def test_CAP_get_caps_with_groups_pkl():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    with open("sample_timeseries.pkl", "rb") as f:
-        subject_timeseries = pickle.load(f)
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=2)
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
-
-def test_CAP_get_caps_with_no_groups_and_silhouette_method_pkl():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    with open("sample_timeseries.pkl", "rb") as f:
-        subject_timeseries = pickle.load(f)
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
-
-
-def test_CAP_get_caps_with_groups_and_silhouette_method_pkl():
-    warnings.simplefilter('ignore')
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
-    with open("sample_timeseries.pkl", "rb") as f:
-        subject_timeseries = pickle.load(f)
-    extractor.subject_timeseries = subject_timeseries
-    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
-    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
-    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
-    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
+import os, numpy as np, pickle, pytest, warnings
+
+from neurocaps.extraction import TimeseriesExtractor
+from neurocaps.analysis import CAP
+
+def test_CAP_get_caps_no_groups():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=2)
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
+    
+def test_CAP_get_caps_with_groups():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=2)
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
+
+def test_CAP_get_caps_with_no_groups_and_silhouette_method():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
+
+
+def test_CAP_get_caps_with_groups_and_silhouette_method():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
+
+def test_CAP_get_caps_no_groups_pkl():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    with open("sample_timeseries.pkl", "rb") as f:
+        subject_timeseries = pickle.load(f)
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=2)
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
+    
+def test_CAP_get_caps_with_groups_pkl():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    with open("sample_timeseries.pkl", "rb") as f:
+        subject_timeseries = pickle.load(f)
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=2)
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
+
+def test_CAP_get_caps_with_no_groups_and_silhouette_method_pkl():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    with open("sample_timeseries.pkl", "rb") as f:
+        subject_timeseries = pickle.load(f)
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["All Subjects"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["All Subjects"]["CAP-2"].shape == (100,)
+
+
+def test_CAP_get_caps_with_groups_and_silhouette_method_pkl():
+    warnings.simplefilter('ignore')
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach)
+    with open("sample_timeseries.pkl", "rb") as f:
+        subject_timeseries = pickle.load(f)
+    extractor.subject_timeseries = subject_timeseries
+    cap_analysis = CAP(parcel_approach=extractor.parcel_approach, groups={"A": [1,2,3,5], "B": [4,6,7,8,9,10,7]}, n_clusters=[2,3,4,5], cluster_selection_method="silhouette")
+    cap_analysis.get_caps(subject_timeseries=extractor.subject_timeseries)
+    assert cap_analysis.caps["A"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["A"]["CAP-2"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-1"].shape == (100,)
+    assert cap_analysis.caps["B"]["CAP-2"].shape == (100,)
```

### Comparing `neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor.py` & `neurocaps-0.9.0.post5/tests/test_TimeseriesExtractor.py`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import os, pytest
-from neurocaps.extraction import TimeseriesExtractor
-
-def test_TimeseriesExtractor_no_parallel():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds)
-
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, session='002', task="rest", pipeline_name=pipeline_name, tr=1.2)
-    
-    print(extractor.subject_timeseries, flush=True)
-
-    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
-
-def test_TimeseriesExtractor_no_parallel_no_session_w_custom():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds)
-
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
-    
-    print(extractor.subject_timeseries, flush=True)
-
-    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
-
-def test_TimeseriesExtractor_no_parallel_no_session_w_custom_and_censoring():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds, fd_threshold=0.35)
-
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
-    
-    print(extractor.subject_timeseries, flush=True)
-
-    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
-    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 39
-
-def test_TimeseriesExtractor_check_exclusion():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds, fd_threshold=0.35)
-
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2, exclude_niftis=["sub-01_ses-002_task-rest_run-001_space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"])
-    assert len(extractor.subject_timeseries) == 0
+import os, pytest
+from neurocaps.extraction import TimeseriesExtractor
+
+def test_TimeseriesExtractor_no_parallel():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, session='002', task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 100
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
+
+def test_TimeseriesExtractor_no_parallel_no_session_w_custom():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 40
+
+def test_TimeseriesExtractor_no_parallel_no_session_w_custom_and_censoring():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds, fd_threshold=0.35)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-001"].shape[-1] == 426
+    assert extractor.subject_timeseries["01"]["run-001"].shape[0] == 39
+
+def test_TimeseriesExtractor_check_exclusion():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Custom": {"maps": os.path.join(dir, "HCPex.nii.gz")}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds, fd_threshold=0.35)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2, exclude_niftis=["sub-01_ses-002_task-rest_run-001_space-MNI152NLin2009cAsym_desc-preproc_bold.nii.gz"])
+    assert len(extractor.subject_timeseries) == 0
```

### Comparing `neurocaps-0.9.0.post4/tests/test_TimeseriesExtractor_additional.py` & `neurocaps-0.9.0.post5/tests/test_TimeseriesExtractor_additional.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-import os, pytest
-from neurocaps.extraction import TimeseriesExtractor
-
-# Changing file name in github actions to test different file naming configurations
-
-def test_TimeseriesExtractor_no_parallel_additional():
-    dir = os.path.dirname(__file__)
-
-    confounds=["Cosine*", "aComp*", "Rot*"]
-
-    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
-
-    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
-                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
-                                    confound_names=confounds, fwhm=2)
-
-    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
-
-    pipeline_name = "fmriprep_1.0.0/fmriprep"
-    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
-    
-    print(extractor.subject_timeseries, flush=True)
-
-    assert extractor.subject_timeseries["01"]["run-1"].shape[-1] == 100
+import os, pytest
+from neurocaps.extraction import TimeseriesExtractor
+
+# Changing file name in github actions to test different file naming configurations
+
+def test_TimeseriesExtractor_no_parallel_additional():
+    dir = os.path.dirname(__file__)
+
+    confounds=["Cosine*", "aComp*", "Rot*"]
+
+    parcel_approach = {"Schaefer": {"n_rois": 100, "yeo_networks": 7}}
+
+    extractor = TimeseriesExtractor(parcel_approach=parcel_approach, standardize="zscore_sample",
+                                    use_confounds=True, detrend=True, low_pass=0.15, high_pass=0.01,
+                                    confound_names=confounds, fwhm=2)
+
+    bids_dir = os.path.join(dir, "ds000031_R1.0.4_ses001-022/ds000031_R1.0.4")
+
+    pipeline_name = "fmriprep_1.0.0/fmriprep"
+    extractor.get_bold(bids_dir=bids_dir, task="rest", pipeline_name=pipeline_name, tr=1.2)
+    
+    print(extractor.subject_timeseries, flush=True)
+
+    assert extractor.subject_timeseries["01"]["run-1"].shape[-1] == 100
     assert extractor.subject_timeseries["01"]["run-1"].shape[0] == 40
```

### Comparing `neurocaps-0.9.0.post4/tests/test_merge_dicts.py` & `neurocaps-0.9.0.post5/tests/test_merge_dicts.py`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import numpy as np, pickle, pandas as pytest
-
-from neurocaps.analysis import merge_dicts
-
-def test_merge_dicts():
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    subject_timeseries_combined = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= False, return_combined_dict=True)
-    assert subject_timeseries_combined["1"]["run-1"].shape == (200,100)
-    assert subject_timeseries_combined["1"]["run-2"].shape == (200,100)
-    assert subject_timeseries_combined["1"]["run-3"].shape == (200,100)
-    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=True)
-    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() == all_dicts["combined"].keys()
-    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=False)
-    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() 
-
-def test_merge_dicts_pkl():
-    with open("sample_timeseries.pkl", "rb") as f:
-        subject_timeseries = pickle.load(f)
-    subject_timeseries_combined = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= False, return_combined_dict=True)
-    assert subject_timeseries_combined["1"]["run-1"].shape == (100,100)
-    assert subject_timeseries_combined["1"]["run-2"].shape == (100,100)
-    assert subject_timeseries_combined["1"]["run-3"].shape == (100,100)
-    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=True)
-    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() == all_dicts["combined"].keys()
-    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=False)
+import numpy as np, pickle, pandas as pytest
+
+from neurocaps.analysis import merge_dicts
+
+def test_merge_dicts():
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    subject_timeseries_combined = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= False, return_combined_dict=True)
+    assert subject_timeseries_combined["1"]["run-1"].shape == (200,100)
+    assert subject_timeseries_combined["1"]["run-2"].shape == (200,100)
+    assert subject_timeseries_combined["1"]["run-3"].shape == (200,100)
+    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=True)
+    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() == all_dicts["combined"].keys()
+    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=False)
+    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() 
+
+def test_merge_dicts_pkl():
+    with open("sample_timeseries.pkl", "rb") as f:
+        subject_timeseries = pickle.load(f)
+    subject_timeseries_combined = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= False, return_combined_dict=True)
+    assert subject_timeseries_combined["1"]["run-1"].shape == (100,100)
+    assert subject_timeseries_combined["1"]["run-2"].shape == (100,100)
+    assert subject_timeseries_combined["1"]["run-3"].shape == (100,100)
+    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=True)
+    assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys() == all_dicts["combined"].keys()
+    all_dicts = merge_dicts([subject_timeseries,subject_timeseries], return_reduced_dicts= True, return_combined_dict=False)
     assert all_dicts["dict_1"].keys() == all_dicts["dict_2"].keys()
```

### Comparing `neurocaps-0.9.0.post4/tests/test_standardize.py` & `neurocaps-0.9.0.post5/tests/test_standardize.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-import numpy as np, os, pandas as pytest
-
-from neurocaps.analysis import standardize
-
-def test_standardize():
-    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
-    subject_timeseries = standardize(subject_timeseries=subject_timeseries)
-    assert subject_timeseries["1"]["run-1"].mean() == 0
-    assert subject_timeseries["1"]["run-1"].std() == 1
-
-def test_standardize_w_pickle():
-    subject_timeseries = standardize(subject_timeseries=os.path.join(os.path.dirname(__file__), "sample_timeseries.pkl"))
-    assert subject_timeseries["1"]["run-1"].mean() == 0
+import numpy as np, os, pandas as pytest
+
+from neurocaps.analysis import standardize
+
+def test_standardize():
+    subject_timeseries = {str(x) : {f"run-{y}": np.random.rand(100,100) for y in range(1,4)} for x in range(1,11)}
+    subject_timeseries = standardize(subject_timeseries=subject_timeseries)
+    assert subject_timeseries["1"]["run-1"].mean() == 0
+    assert subject_timeseries["1"]["run-1"].std() == 1
+
+def test_standardize_w_pickle():
+    subject_timeseries = standardize(subject_timeseries=os.path.join(os.path.dirname(__file__), "sample_timeseries.pkl"))
+    assert subject_timeseries["1"]["run-1"].mean() == 0
     assert subject_timeseries["1"]["run-1"].std() == 1
```

