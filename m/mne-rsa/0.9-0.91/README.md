# Comparing `tmp/mne-rsa-0.9.tar.gz` & `tmp/mne_rsa-0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mne-rsa-0.9.tar", last modified: Tue Oct 10 11:49:07 2023, max compression
+gzip compressed data, was "mne_rsa-0.91.tar", last modified: Wed May 22 11:52:47 2024, max compression
```

## Comparing `mne-rsa-0.9.tar` & `mne_rsa-0.91.tar`

### file list

```diff
@@ -1,27 +1,26 @@
-drwxrwxrwx   0        0        0        0 2023-10-10 11:49:07.209715 mne-rsa-0.9/
--rw-rw-rw-   0        0        0     1524 2022-10-24 08:52:09.000000 mne-rsa-0.9/LICENSE
--rw-rw-rw-   0        0        0     6251 2023-10-10 11:49:07.209715 mne-rsa-0.9/PKG-INFO
--rw-rw-rw-   0        0        0     4956 2023-10-10 10:35:33.000000 mne-rsa-0.9/README.rst
-drwxrwxrwx   0        0        0        0 2023-10-10 11:49:07.183284 mne-rsa-0.9/mne_rsa/
--rw-rw-rw-   0        0        0      488 2023-10-10 11:46:10.000000 mne-rsa-0.9/mne_rsa/__init__.py
--rw-rw-rw-   0        0        0     3832 2023-09-28 07:45:53.000000 mne-rsa-0.9/mne_rsa/folds.py
--rw-rw-rw-   0        0        0    10164 2023-10-10 10:28:18.000000 mne-rsa-0.9/mne_rsa/rdm.py
--rw-rw-rw-   0        0        0    15676 2023-10-10 10:28:18.000000 mne-rsa-0.9/mne_rsa/rsa.py
--rw-rw-rw-   0        0        0    15249 2023-09-27 13:04:23.000000 mne-rsa-0.9/mne_rsa/searchlight.py
--rw-rw-rw-   0        0        0    32676 2023-10-10 10:28:18.000000 mne-rsa-0.9/mne_rsa/sensor_level.py
--rw-rw-rw-   0        0        0    53252 2023-10-10 11:20:10.000000 mne-rsa-0.9/mne_rsa/source_level.py
--rw-rw-rw-   0        0        0    11909 2023-10-10 10:28:18.000000 mne-rsa-0.9/mne_rsa/viz.py
-drwxrwxrwx   0        0        0        0 2023-10-10 11:49:07.205063 mne-rsa-0.9/mne_rsa.egg-info/
--rw-rw-rw-   0        0        0     6251 2023-10-10 11:49:07.000000 mne-rsa-0.9/mne_rsa.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      441 2023-10-10 11:49:07.000000 mne-rsa-0.9/mne_rsa.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-10-10 11:49:07.000000 mne-rsa-0.9/mne_rsa.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-10-10 11:49:07.000000 mne-rsa-0.9/mne_rsa.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-10-10 11:49:07.000000 mne-rsa-0.9/mne_rsa.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      922 2023-07-19 06:05:35.000000 mne-rsa-0.9/pyproject.toml
--rw-rw-rw-   0        0        0      351 2023-10-10 11:49:07.210720 mne-rsa-0.9/setup.cfg
--rw-rw-rw-   0        0        0     1930 2023-09-27 12:40:50.000000 mne-rsa-0.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-10-10 11:49:07.208346 mne-rsa-0.9/tests/
--rw-rw-rw-   0        0        0     2557 2023-05-22 06:17:00.000000 mne-rsa-0.9/tests/test_folds.py
--rw-rw-rw-   0        0        0     6593 2023-10-10 10:28:18.000000 mne-rsa-0.9/tests/test_rdm.py
--rw-rw-rw-   0        0        0    13522 2023-10-10 10:28:18.000000 mne-rsa-0.9/tests/test_rsa.py
--rw-rw-rw-   0        0        0     6940 2023-05-22 06:17:01.000000 mne-rsa-0.9/tests/test_searchlight.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:52:47.126838 mne_rsa-0.91/
+-rw-rw-rw-   0        0        0     1524 2022-10-24 08:52:09.000000 mne_rsa-0.91/LICENSE
+-rw-rw-rw-   0        0        0      780 2024-05-22 11:52:47.124818 mne_rsa-0.91/PKG-INFO
+-rw-rw-rw-   0        0        0     4950 2024-05-22 11:47:57.000000 mne_rsa-0.91/README.rst
+drwxrwxrwx   0        0        0        0 2024-05-22 11:52:47.079370 mne_rsa-0.91/mne_rsa/
+-rw-rw-rw-   0        0        0      500 2024-05-22 11:48:43.000000 mne_rsa-0.91/mne_rsa/__init__.py
+-rw-rw-rw-   0        0        0     3884 2024-05-22 11:47:30.000000 mne_rsa-0.91/mne_rsa/folds.py
+-rw-rw-rw-   0        0        0    11056 2024-05-22 11:47:30.000000 mne_rsa-0.91/mne_rsa/rdm.py
+-rw-rw-rw-   0        0        0    16848 2024-05-22 11:47:30.000000 mne_rsa-0.91/mne_rsa/rsa.py
+-rw-rw-rw-   0        0        0    15253 2024-05-06 18:37:20.000000 mne_rsa-0.91/mne_rsa/searchlight.py
+-rw-rw-rw-   0        0        0    32716 2024-05-22 11:47:30.000000 mne_rsa-0.91/mne_rsa/sensor_level.py
+-rw-rw-rw-   0        0        0    52123 2024-05-22 11:47:30.000000 mne_rsa-0.91/mne_rsa/source_level.py
+-rw-rw-rw-   0        0        0    11876 2024-05-22 08:05:30.000000 mne_rsa-0.91/mne_rsa/viz.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:52:47.123017 mne_rsa-0.91/mne_rsa.egg-info/
+-rw-rw-rw-   0        0        0      780 2024-05-22 11:52:46.000000 mne_rsa-0.91/mne_rsa.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      422 2024-05-22 11:52:47.000000 mne_rsa-0.91/mne_rsa.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:52:46.000000 mne_rsa-0.91/mne_rsa.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 11:52:46.000000 mne_rsa-0.91/mne_rsa.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 11:52:46.000000 mne_rsa-0.91/mne_rsa.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1540 2024-05-06 18:37:20.000000 mne_rsa-0.91/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:52:47.126838 mne_rsa-0.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 11:52:47.119493 mne_rsa-0.91/tests/
+-rw-rw-rw-   0        0        0     2618 2024-05-22 11:47:30.000000 mne_rsa-0.91/tests/test_folds.py
+-rw-rw-rw-   0        0        0     8099 2024-05-06 18:37:20.000000 mne_rsa-0.91/tests/test_rdm.py
+-rw-rw-rw-   0        0        0    13681 2024-05-07 05:23:14.000000 mne_rsa-0.91/tests/test_rsa.py
+-rw-rw-rw-   0        0        0     6996 2024-05-06 18:37:20.000000 mne_rsa-0.91/tests/test_searchlight.py
```

### Comparing `mne-rsa-0.9/LICENSE` & `mne_rsa-0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `mne-rsa-0.9/PKG-INFO` & `mne_rsa-0.91/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,175 +1,149 @@
-Metadata-Version: 2.1
-Name: mne-rsa
-Version: 0.9
-Summary: Code for performing Representational Similarity Analysis on MNE-Python data structures.
-Home-page: https://github.com/wmvanvliet/mne-rsa
-Download-URL: https://github.com/wmvanvliet/mne-rsa/archive/master.zip
-Author-email: Marijn van Vliet <w.m.vanvliet@gmail.com>
-Maintainer: Marijn van Vliet
-Maintainer-email: w.m.vanvliet@gmail.com
-License: BSD-3-Clause
-Keywords: rsa,meg,eeg,neuroimaging,mne-python
-Platform: any
-Classifier: Intended Audience :: Science/Research
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved
-Classifier: Programming Language :: Python
-Classifier: Topic :: Software Development
-Classifier: Topic :: Scientific/Engineering
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS
-Requires-Python: >=3.7
-Description-Content-Type: text/x-rst
-License-File: LICENSE
-Requires-Dist: numpy
-Requires-Dist: scipy
-Requires-Dist: scikit-learn
-Requires-Dist: nibabel
-Requires-Dist: matplotlib
-Requires-Dist: mne
-
-Representational Similarity Analysis
-------------------------------------
-
-|unit_tests|_ |build_docs|_
-
-.. |unit_tests| image:: https://github.com/wmvanvliet/mne-rsa/workflows/unit%20tests/badge.svg
-.. _unit_tests: https://github.com/wmvanvliet/mne-rsa/actions?query=workflow%3A%22unit+tests%22
-
-.. |build_docs| image:: https://github.com/wmvanvliet/mne-rsa/workflows/build-docs/badge.svg
-.. _build_docs: https://github.com/wmvanvliet/mne-rsa/actions?query=workflow%3Abuild-docs
-
-This is a Python package for performing representational similarity
-analysis (RSA) using
-`MNE-Python <https://martinos.org/mne/stable/index.html>`__ data
-structures. The RSA is computed using a “searchlight” approach.
-
-Read more on RSA in the paper that introduced the technique:
-
-Nikolaus Kriegeskorte, Marieke Mur and Peter Bandettini (2008).
-Representational similarity analysis - connecting the branches of
-systems neuroscience. Frontiers in Systems Neuroscience, 2(4).
-https://doi.org/10.3389/neuro.06.004.2008
-
-.. image:: https://raw.githubusercontent.com/wmvanvliet/mne-rsa/main/doc/rsa.png
-
-
-Installation
-------------
-
-The package can be installed either through PIP:  
-``pip install mne-rsa``  
-or through conda using the conda-forge channel:  
-``conda install -c conda-forge mne-rsa``
-
-
-Use cases
----------
-
-This is what the package can do for you:
-
--  Compute RDMs on arbitrary data
--  Compute RDMs in a searchlight across:
-
-   -  vertices/voxels and samples (source level)
-   -  sensors and samples (sensor level)
-   -  vertices/voxels only (source level)
-   -  sensors only (sensor level)
-   -  samples only (source and sensor level)
-
--  Use cross-validated distance metrics when computing RDMs
--  And of course: compute RSA between RDMs
-
-Supported metrics for comparing RDMs:
-
--  Spearman correlation (the default)
--  Pearson correlation
--  Kendall’s Tau-A
--  Linear regression (when comparing multiple RDMs at once)
--  Partial correlation (when comparing multiple RDMs at once)
-
-Juicy bits of the API
----------------------
-
-.. code:: python
-
-   def compute_rdm(data, metric='correlation', **kwargs)
-
-   def rsa_stcs(stcs, rdm_model, src, spatial_radius=0.04, temporal_radius=0.1,
-                stc_rdm_metric='correlation', stc_rdm_params=dict(),
-                rsa_metric='spearman', y=None, n_folds=1, sel_vertices=None,
-                tmin=None, tmax=None, n_jobs=1, verbose=False):
-
-   def rsa_evokeds(evokeds, rdm_model, noise_cov=None, spatial_radius=0.04,
-                   temporal_radius=0.1, evoked_rdm_metric='correlation',
-                   evoked_rdm_params=dict(), rsa_metric='spearman', y=None,
-                   n_folds=1, picks=None, tmin=None, tmax=None, n_jobs=1,
-                   verbose=False):
-
-   def rsa_epochs(epochs, rdm_model, noise_cov=None, spatial_radius=0.04,
-                  temporal_radius=0.1, epochs_rdm_metric='correlation',
-                  epochs_rdm_params=dict(), rsa_metric='spearman', y=None,
-                  n_folds=1, picks=None, tmin=None, tmax=None, n_jobs=1,
-                  verbose=False):
-
-   def rsa_nifti(image, rdm_model, spatial_radius=0.01,
-                 image_rdm_metric='correlation', image_rdm_params=dict(),
-                 rsa_metric='spearman', y=None, n_folds=1, roi_mask=None,
-                 brain_mask=None, n_jobs=1, verbose=False):
-
-Example usage
--------------
-
-Basic example on the EEG “kiloword” data:
-
-.. code:: python
-
-   import mne
-   import rsa
-   data_path = mne.datasets.kiloword.data_path(verbose=True)
-   epochs = mne.read_epochs(data_path + '/kword_metadata-epo.fif')
-   # Compute the model RDM using all word properties
-   rdm_model = rsa.compute_rdm(epochs.metadata.iloc[:, 1:].values)
-   evoked_rsa = rsa.rsa_epochs(epochs, rdm_model,
-                               spatial_radius=0.04, temporal_radius=0.01,
-                               verbose=True)
-
-Documentation
--------------
-
-For quick guides on how to do specific things, see the
-`examples <https://users.aalto.fi/~vanvlm1/mne-rsa/auto_examples/index.html>`__.
-
-Finally, there is the
-`API reference <https://users.aalto.fi/~vanvlm1/mne-rsa/api.html>`__
-documentation.
-
-Integration with other packages
--------------------------------
-
-I mainly wrote this package to perform RSA analysis on MEG data. Hence,
-integration functions with `MNE-Python <https://mne.tools>`__ are
-provided. There is also some integration with `nipy <https://nipy.org>`__ for
-fMRI.
-
-Performance
------------
-
-This package aims to be fast and memory efficient. An important design
-feature is that under the hood, everything operates on generators. The
-searchlight routines produce a generator of RDMs which are consumed by a
-generator of RSA values. Parallel processing is also supported, so you
-can use all of your CPU cores.
-
-Development
------------
-
-Here is how to set up the package as a developer:
-
-.. code:: bash
-
-   git clone git@github.com:wmvanvliet/mne-rsa.git
-   cd mne-rsa
-   python setup.py develop --user
+Representational Similarity Analysis
+------------------------------------
+
+|unit_tests| |build_docs|
+
+.. |unit_tests| image:: https://github.com/wmvanvliet/mne-rsa/workflows/unit%20tests/badge.svg
+   :target: https://github.com/wmvanvliet/mne-rsa/actions?query=workflow%3A%22unit+tests%22
+
+.. |build_docs| image:: https://github.com/wmvanvliet/mne-rsa/workflows/build-docs/badge.svg
+   :target: https://github.com/wmvanvliet/mne-rsa/actions?query=workflow%3Abuild-docs
+
+This is a Python package for performing representational similarity
+analysis (RSA) using
+`MNE-Python <https://martinos.org/mne/stable/index.html>`__ data
+structures. The RSA is computed using a “searchlight” approach.
+
+Read more on RSA in the paper that introduced the technique:
+
+Nikolaus Kriegeskorte, Marieke Mur and Peter Bandettini (2008).
+Representational similarity analysis - connecting the branches of
+systems neuroscience. Frontiers in Systems Neuroscience, 2(4).
+https://doi.org/10.3389/neuro.06.004.2008
+
+.. image:: https://raw.githubusercontent.com/wmvanvliet/mne-rsa/main/doc/rsa.png
+
+
+Installation
+------------
+
+The package can be installed either through PIP:  
+``pip install mne-rsa``  
+or through conda using the conda-forge channel:  
+``conda install -c conda-forge mne-rsa``
+
+
+Use cases
+---------
+
+This is what the package can do for you:
+
+-  Compute RDMs on arbitrary data
+-  Compute RDMs in a searchlight across:
+
+   -  vertices/voxels and samples (source level)
+   -  sensors and samples (sensor level)
+   -  vertices/voxels only (source level)
+   -  sensors only (sensor level)
+   -  samples only (source and sensor level)
+
+-  Use cross-validated distance metrics when computing RDMs
+-  And of course: compute RSA between RDMs
+
+Supported metrics for comparing RDMs:
+
+-  Spearman correlation (the default)
+-  Pearson correlation
+-  Kendall’s Tau-A
+-  Linear regression (when comparing multiple RDMs at once)
+-  Partial correlation (when comparing multiple RDMs at once)
+
+Juicy bits of the API
+---------------------
+
+.. code:: python
+
+   compute_rdm(data, metric='correlation', **kwargs)
+
+   rsa_stcs(stcs, rdm_model, src, spatial_radius=0.04, temporal_radius=0.1,
+            stc_rdm_metric='correlation', stc_rdm_params=dict(),
+            rsa_metric='spearman', y=None, n_folds=1, sel_vertices=None,
+            tmin=None, tmax=None, n_jobs=1, verbose=False)
+
+   rsa_evokeds(evokeds, rdm_model, noise_cov=None, spatial_radius=0.04,
+               temporal_radius=0.1, evoked_rdm_metric='correlation',
+               evoked_rdm_params=dict(), rsa_metric='spearman', y=None,
+               n_folds=1, picks=None, tmin=None, tmax=None, n_jobs=1,
+               verbose=False)
+
+   rsa_epochs(epochs, rdm_model, noise_cov=None, spatial_radius=0.04,
+              temporal_radius=0.1, epochs_rdm_metric='correlation',
+              epochs_rdm_params=dict(), rsa_metric='spearman', y=None,
+              n_folds=1, picks=None, tmin=None, tmax=None, n_jobs=1,
+              verbose=False)
+
+   rsa_nifti(image, rdm_model, spatial_radius=0.01,
+             image_rdm_metric='correlation', image_rdm_params=dict(),
+             rsa_metric='spearman', y=None, n_folds=1, roi_mask=None,
+             brain_mask=None, n_jobs=1, verbose=False)
+
+Example usage
+-------------
+
+Basic example on the EEG “kiloword” data:
+
+.. code:: python
+
+   import mne
+   import rsa
+   data_path = mne.datasets.kiloword.data_path(verbose=True)
+   epochs = mne.read_epochs(data_path + '/kword_metadata-epo.fif')
+   # Compute the model RDM using all word properties
+   rdm_model = rsa.compute_rdm(epochs.metadata.iloc[:, 1:].values)
+   evoked_rsa = rsa.rsa_epochs(epochs, rdm_model,
+                               spatial_radius=0.04, temporal_radius=0.01,
+                               verbose=True)
+
+Documentation
+-------------
+
+For quick guides on how to do specific things, see the
+`examples <https://users.aalto.fi/~vanvlm1/mne-rsa/auto_examples/index.html>`__.
+
+Finally, there is the
+`API reference <https://users.aalto.fi/~vanvlm1/mne-rsa/api.html>`__
+documentation.
+
+Integration with other packages
+-------------------------------
+
+I mainly wrote this package to perform RSA analysis on MEG data. Hence,
+integration functions with `MNE-Python <https://mne.tools>`__ are
+provided. There is also some integration with `nipy <https://nipy.org>`__ for
+fMRI.
+
+Performance
+-----------
+
+This package aims to be fast and memory efficient. An important design
+feature is that under the hood, everything operates on generators. The
+searchlight routines produce a generator of RDMs which are consumed by a
+generator of RSA values. Parallel processing is also supported, so you
+can use all of your CPU cores.
+
+Development
+-----------
+
+Here is how to set up the package as a developer:
+
+.. code:: bash
+
+   git clone git@github.com:wmvanvliet/mne-rsa.git
+   cd mne-rsa
+   python setup.py develop --user
+
+.. toctree::
+   :hidden:
+
+   Examples <auto_examples/index>
+   API Reference <api>
```

### Comparing `mne-rsa-0.9/mne_rsa/folds.py` & `mne_rsa-0.91/mne_rsa/folds.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-from mne.utils import logger
+"""Functions concerning the creation of cross-validation folds."""
+
 import numpy as np
+from mne.utils import logger
 from sklearn.model_selection import StratifiedKFold
 from sklearn.preprocessing import OneHotEncoder
 
 
 def create_folds(X, y=None, n_folds=None):
     """Group individual items into folds suitable for cross-validation.
 
-    The ``y`` list should contain an integer label for each item in ``X``.
-    Repetitions of the same item have the same integer label. Repeated items
-    are distributed evenly across the folds, and averaged within a fold.
+    The ``y`` list should contain an integer label for each item in ``X``. Repetitions
+    of the same item have the same integer label. Repeated items are distributed evenly
+    across the folds, and averaged within a fold.
 
     Parameters
     ----------
     X : ndarray, shape (n_items, ...)
-        For each item, all the features. The first dimension are the items and
-        all other dimensions will be flattened and treated as features.
+        For each item, all the features. The first dimension are the items and all other
+        dimensions will be flattened and treated as features.
     y : ndarray of int, shape (n_items,) | None
-        For each item, a number indicating the class to which the item belongs.
-        When ``None``, each item is assumed to belong to a different class.
-        Defaults to ``None``.
+        For each item, a number indicating the class to which the item belongs. When
+        ``None``, each item is assumed to belong to a different class. Defaults to
+        ``None``.
     n_folds : int | sklearn.BaseCrossValidator | None
-        Number of cross-validation folds to use when computing the distance
-        metric. Folds are created based on the ``y`` parameter. Specify
-        ``None`` to use the maximum number of folds possible, given the data.
-        Alternatively, you can pass a Scikit-Learn cross validator object (e.g.
-        ``sklearn.model_selection.KFold``) to assert fine-grained control over
-        how folds are created.
-        Defaults to ``None``.
+        Number of cross-validation folds to use when computing the distance metric.
+        Folds are created based on the ``y`` parameter. Specify ``None`` to use the
+        maximum number of folds possible, given the data. Alternatively, you can pass a
+        Scikit-Learn cross validator object (e.g. ``sklearn.model_selection.KFold``) to
+        assert fine-grained control over how folds are created. Defaults to ``None``.
 
     Returns
     -------
     folds : ndarray, shape (n_folds, n_items, ...)
         The folded data.
 
     """
```

### Comparing `mne-rsa-0.9/mne_rsa/rdm.py` & `mne_rsa-0.91/mne_rsa/rdm.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,47 +1,45 @@
 # encoding: utf-8
 """Methods to compute dissimilarity matrices (RDMs)."""
 
 import numpy as np
-from scipy.spatial import distance
 from joblib import Parallel, delayed
+from scipy.spatial import distance
 
 from .folds import create_folds
 from .searchlight import searchlight
 
 
 def compute_rdm(data, metric="correlation", **kwargs):
     """Compute a dissimilarity matrix (RDM).
 
     Parameters
     ----------
     data : ndarray, shape (n_items, ...)
-        For each item, all the features. The first dimension are the items and
-        all other dimensions will be flattened and treated as features.
+        For each item, all the features. The first dimension are the items and all other
+        dimensions will be flattened and treated as features.
     metric : str | function
-        The distance metric to use to compute the RDM. Can be any metric
-        supported by :func:`scipy.spatial.distance.pdist`. When a function is
-        specified, it needs to take in two vectors and output a single number.
-        See also the ``dist_params`` parameter to specify and additional
-        parameter for the distance function.
+        The distance metric to use to compute the RDM. Can be any metric supported by
+        :func:`scipy.spatial.distance.pdist`. When a function is specified, it needs to
+        take in two vectors and output a single number. See also the ``dist_params``
+        parameter to specify and additional parameter for the distance function.
         Defaults to 'correlation'.
     **kwargs : dict, optional
-        Extra arguments for the distance metric. Refer to
-        :mod:`scipy.spatial.distance` for a list of all other metrics and their
-        arguments.
+        Extra arguments for the distance metric. Refer to :mod:`scipy.spatial.distance`
+        for a list of all other metrics and their arguments.
 
     Returns
     -------
     rdm : ndarray, shape (n_classes * n_classes-1,)
-        The RDM, in condensed form.
-        See :func:`scipy.spatial.distance.squareform`.
+        The RDM, in condensed form. See :func:`scipy.spatial.distance.squareform`.
 
     See Also
     --------
     compute_rdm_cv
+
     """
     X = np.reshape(np.asarray(data), (len(data), -1))
     n_items, n_features = X.shape
 
     # Be careful with certain metrics
     if n_features == 1 and metric in ["correlation", "cosine"]:
         raise ValueError(
@@ -53,46 +51,45 @@
 
     return distance.pdist(X, metric, **kwargs)
 
 
 def compute_rdm_cv(folds, metric="correlation", **kwargs):
     """Compute a dissimilarity matrix (RDM) using cross-validation.
 
-    The distance computation is performed from the average of
-    all-but-one "training" folds to the remaining "test" fold. This is repeated
-    with each fold acting as the "test" fold once. The resulting distances are
-    averaged and the result used in the final RDM.
+    The distance computation is performed from the average of all-but-one "training"
+    folds to the remaining "test" fold. This is repeated with each fold acting as the
+    "test" fold once. The resulting distances are averaged and the result used in the
+    final RDM.
 
     Parameters
     ----------
     folds : ndarray, shape (n_folds, n_items, ...)
-        For each item, all the features. The first dimension are the folds used
-        for cross-validation, items are along the second dimension, and all
-        other dimensions will be flattened and treated as features.
+        For each item, all the features. The first dimension are the folds used for
+        cross-validation, items are along the second dimension, and all other dimensions
+        will be flattened and treated as features.
     metric : str | function
-        The distance metric to use to compute the RDM. Can be any metric
-        supported by :func:`scipy.spatial.distance.pdist`. When a function is
-        specified, it needs to take in two vectors and output a single number.
-        See also the ``dist_params`` parameter to specify and additional
-        parameter for the distance function.
+        The distance metric to use to compute the RDM. Can be any metric supported by
+        :func:`scipy.spatial.distance.pdist`. When a function is specified, it needs to
+        take in two vectors and output a single number. See also the ``dist_params``
+        parameter to specify and additional parameter for the distance function.
         Defaults to 'correlation'.
     **kwargs : dict, optional
-        Extra arguments for the distance metric. Refer to
-        :mod:`scipy.spatial.distance` for a list of all other metrics and their
-        arguments.
+        Extra arguments for the distance metric. Refer to :mod:`scipy.spatial.distance`
+        for a list of all other metrics and their arguments.
 
     Returns
     -------
     rdm : ndarray, shape (n_classes * n_classes-1,)
         The cross-validated RDM, in condensed form.
         See :func:`scipy.spatial.distance.squareform`.
 
     See Also
     --------
     compute_rdm
+
     """
     X = np.reshape(folds, (folds.shape[0], folds.shape[1], -1))
     n_folds, n_items, n_features = X.shape[:3]
 
     # Be careful with certain metrics
     if n_features == 1 and metric in ["correlation", "cosine"]:
         raise ValueError(
@@ -115,15 +112,15 @@
         rdm += dist[np.triu_indices_from(dist, 1)]
 
     return rdm / n_folds
 
 
 def _ensure_condensed(rdm, var_name):
     """Convert a RDM to condensed form if needed."""
-    if type(rdm) is list:
+    if isinstance(rdm, list):
         return [_ensure_condensed(d, var_name) for d in rdm]
 
     if not isinstance(rdm, np.ndarray):
         raise TypeError(
             "A single RDM should be a NumPy array. "
             "Multiple RDMs should be a list of NumPy arrays."
         )
@@ -148,83 +145,110 @@
 
 def _n_items_from_rdm(rdm):
     """Get the number of items, given a RDM."""
     if rdm.ndim == 2:
         return rdm.shape[0]
     elif rdm.ndim == 1:
         return distance.squareform(rdm).shape[0]
+    else:
+        raise ValueError(f"Wrong number of dimensions for RDM ({rdm.ndim})")
+
+
+def pick_rdm(rdm, sel):
+    """Select items from an RDM.
+
+    Parameters
+    ----------
+    rdm : ndarray, shape (n, n) | (n * (n - 1) // 2,)
+        The RDM to pick items from.
+    sel : int | list of int | boolean mask | slice
+        The items to pick. These items will be selected from both rows and columns of
+        the RDM.
+
+    Returns
+    -------
+    rdm : ndarray, shape (n, n) | (n * (n - 1) // 2,)
+        A new RDM with only the selected items. If the original RDM was in condensed
+        form, the returned RDM will be as well.
+
+    """
+    if np.isscalar(sel):
+        sel = [sel]  # to avoid dropping a dimension
+    if rdm.ndim == 2:
+        return rdm[sel, :][:, sel]
+    elif rdm.ndim == 1:
+        return distance.squareform(distance.squareform(rdm)[sel, :][:, sel])
+    else:
+        raise ValueError(f"Wrong number of dimensions for RDM ({rdm.ndim})")
 
 
 class rdm_array:
     """Generate RDMs from an array of data, possibly in a searchlight pattern.
 
-    First use :class:`searchlight` to compute the searchlight patches.
-    Then you can use this function to compute RDMs for each searchlight patch.
+    First use :class:`searchlight` to compute the searchlight patches. Then you can use
+    this function to compute RDMs for each searchlight patch.
 
     Parameters
     ----------
     X : ndarray, shape (n_items, n_series, n_times)
         An array containing the data.
     patches : generator of tuples | None
-        Searchlight patches as generated by :class:`searchlight`. If ``None``,
-        no searchlight is used. Defaults to ``None``.
+        Searchlight patches as generated by :class:`searchlight`. If ``None``, no
+        searchlight is used. Defaults to ``None``.
     dist_metric : str | function
-        The distance metric to use to compute the RDMs. Can be any metric
-        supported by :func:`scipy.spatial.distance.pdist`. When a function is
-        specified, it needs to take in two vectors and output a single number.
-        See also the ``dist_params`` parameter to specify and additional
-        parameter for the distance function.
+        The distance metric to use to compute the RDMs. Can be any metric supported by
+        :func:`scipy.spatial.distance.pdist`. When a function is specified, it needs to
+        take in two vectors and output a single number. See also the ``dist_params``
+        parameter to specify and additional parameter for the distance function.
         Defaults to 'correlation'.
     dist_params : dict
-        Extra arguments for the distance metric used to compute the RDMs.
-        Refer to :mod:`scipy.spatial.distance` for a list of all other metrics
-        and their arguments. Defaults to an empty dictionary.
+        Extra arguments for the distance metric used to compute the RDMs. Refer to
+        :mod:`scipy.spatial.distance` for a list of all other metrics and their
+        arguments. Defaults to an empty dictionary.
     y : ndarray of int, shape (n_items,) | None
-        For each item, a number indicating the class to which the item belongs.
-        When ``None``, each item is assumed to belong to a different class.
+        For each item, a number indicating the class to which the item belongs. When
+        ``None``, each item is assumed to belong to a different class.
         Defaults to ``None``.
     n_folds : int | sklearn.model_selection.BaseCrollValidator | None
-        Number of cross-validation folds to use when computing the distance
-        metric. Folds are created based on the ``y`` parameter. Specify
-        ``None`` to use the maximum number of folds possible, given the data.
-        Alternatively, you can pass a Scikit-Learn cross validator object (e.g.
-        ``sklearn.model_selection.KFold``) to assert fine-grained control over
-        how folds are created.
+        Number of cross-validation folds to use when computing the distance metric.
+        Folds are created based on the ``y`` parameter. Specify ``None`` to use the
+        maximum number of folds possible, given the data. Alternatively, you can pass a
+        Scikit-Learn cross validator object (e.g. ``sklearn.model_selection.KFold``) to
+        assert fine-grained control over how folds are created.
         Defaults to 1 (no cross-validation).
 
     Yields
     ------
     rdm : ndarray, shape (n_patches, n_items * (n_items - 1))
         A RDM (in condensed form) for each searchlight patch.
 
     Attributes
     ----------
     shape : tuple of int
         Multidimensional shape of the generted RDMs.
 
-        This is useful for re-shaping the result obtained after consuming the
-        this generator.
+        This is useful for re-shaping the result obtained after consuming the this
+        generator.
 
         For a spatio-temporal searchlight:
-            Three elements: the number of time-series, number of time
-            samples and length of a consensed RDM.
+            Three elements: the number of time-series, number of time samples and length
+            of a consensed RDM.
         For a spatial searchlight:
-            Two element: the number of time-series and length of a condensed
-            RDM.
+            Two element: the number of time-series and length of a condensed RDM.
         For a temporal searchlight:
-            Two elements: the number of time-samples and length of a condensed
-            RDM.
+            Two elements: the number of time-samples and length of a condensed RDM.
         For no searchlight:
             One element: the length of a condensed RDM.
 
     See Also
     --------
     rdm
     rsa
     searchlight
+
     """
 
     def __init__(
         self,
         X,
         patches=None,
         dist_metric="correlation",
```

### Comparing `mne-rsa-0.9/mne_rsa/rsa.py` & `mne_rsa-0.91/mne_rsa/rsa.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # encoding: utf-8
-"""
-Methods to compute representational similarity analysis (RSA).
-"""
+"""Methods to compute representational similarity analysis (RSA)."""
 
 import numpy as np
-from scipy import stats
 from joblib import Parallel, delayed
+from scipy import stats
 
 from .folds import create_folds
 from .rdm import _ensure_condensed, compute_rdm, compute_rdm_cv
 from .searchlight import searchlight
 
 try:
     # Version 1.8.0 and up
@@ -130,31 +128,32 @@
         * 'kendall-tau-a' for Kendall's Tau (alpha variant)
         * 'partial' for partial Pearson correlations
         * 'partial-spearman' for partial Spearman correlations
         * 'regression' for linear regression weights
 
         Defaults to 'spearman'.
     ignore_nan : bool
-        Whether to treat NaN's as missing values and ignore them when computing
-        the distance metric. Defaults to ``False``.
+        Whether to treat NaN's as missing values and ignore them when computing the
+        distance metric. Defaults to ``False``.
 
         .. versionadded:: 0.8
 
     Yields
     ------
     rsa_val : float | ndarray, shape (len(rdm_model),)
-        For each data RDM, the representational similarity with the model RDM.
-        When multiple model RDMs are specified, this will be a 1D array of
-        similarities, comparing the data RDM with each model RDM.
+        For each data RDM, the representational similarity with the model RDM. When
+        multiple model RDMs are specified, this will be a 1D array of similarities,
+        comparing the data RDM with each model RDM.
 
-    See also
+    See Also
     --------
     rsa
+
     """
-    if type(rdm_model) == list:
+    if isinstance(rdm_model, list):
         return_array = True
         rdm_model = [_ensure_condensed(rdm, "rdm_model") for rdm in rdm_model]
     else:
         return_array = False
         rdm_model = [_ensure_condensed(rdm_model, "rdm_model")]
 
     if ignore_nan:
@@ -242,39 +241,39 @@
         Defaults to 'spearman'.
     ignore_nan : bool
         Whether to treat NaN's as missing values and ignore them when computing
         the distance metric. Defaults to ``False``.
 
         .. versionadded:: 0.8
     n_data_rdms : int | None
-        The number of data RDMs. This is useful when displaying a progress bar,
-        so an estimate can be made of the computation time remaining. This
-        information is available if ``rdm_data`` is an array or a list, but if
-        it is a generator, this information is not available and you may want
-        to set it explicitly.
+        The number of data RDMs. This is useful when displaying a progress bar, so an
+        estimate can be made of the computation time remaining. This information is
+        available if ``rdm_data`` is an array or a list, but if it is a generator, this
+        information is not available and you may want to set it explicitly.
     n_jobs : int
-        The number of processes (=number of CPU cores) to use. Specify -1 to
-        use all available cores. Defaults to 1.
+        The number of processes (=number of CPU cores) to use. Specify -1 to use all
+        available cores. Defaults to 1.
     verbose : bool
-        Whether to display a progress bar. In order for this to work, you need
-        the tqdm python module installed. Defaults to False.
+        Whether to display a progress bar. In order for this to work, you need the tqdm
+        python module installed. Defaults to False.
 
     Returns
     -------
     rsa_val : float | ndarray, shape (len(rdm_data), len(rdm_model))
-        Depending on whether one or more data and model RDMs were specified, a
-        single similarity value or a 2D array of similarity values for each
-        data RDM versus each model RDM.
+        Depending on whether one or more data and model RDMs were specified, a single
+        similarity value or a 2D array of similarity values for each data RDM versus
+        each model RDM.
 
-    See also
+    See Also
     --------
     rsa_gen
+
     """
     return_array = False
-    if type(rdm_data) == list or hasattr(rdm_data, "__next__"):
+    if isinstance(rdm_data, list) or hasattr(rdm_data, "__next__"):
         return_array = True
     else:
         rdm_data = [rdm_data]
 
     if verbose:
         from tqdm import tqdm
 
@@ -318,89 +317,107 @@
     """Perform RSA on an array of data, possibly in a searchlight pattern.
 
     Parameters
     ----------
     X : ndarray, shape (n_items, n_series, n_times)
         An array containing the data.
     rdm_model : ndarray, shape (n, n) | (n * (n - 1) // 2,) | list of ndarray
-        The model RDM, see :func:`compute_rdm`. For efficiency, you can give it
-        in condensed form, meaning only the upper triangle of the matrix as a
-        vector. See :func:`scipy.spatial.distance.squareform`. To perform RSA
-        against multiple models at the same time, supply a list of model RDMs.
+        The model RDM, see :func:`compute_rdm`. For efficiency, you can give it in
+        condensed form, meaning only the upper triangle of the matrix as a vector. See
+        :func:`scipy.spatial.distance.squareform`. To perform RSA against multiple
+        models at the same time, supply a list of model RDMs.
 
         Use :func:`compute_rdm` to compute RDMs.
     patches : generator of tuples | None
-        Searchlight patches as generated by :class:`searchlight`. If ``None``,
-        no searchlight is used. Defaults to ``None``.
+        Searchlight patches as generated by :class:`searchlight`. If ``None``, no
+        searchlight is used. Defaults to ``None``.
     data_rdm_metric : str
-        The metric to use to compute the data RDMs. This can be any metric
-        supported by the scipy.distance.pdist function. Defaults to
-        'correlation'.
+        The metric to use to compute the data RDMs. This can be any metric supported by
+        the scipy.distance.pdist function. Defaults to 'correlation'.
     data_rdm_params : dict
-        Extra arguments for the distance metric used to compute the RDMs.
-        Refer to :mod:`scipy.spatial.distance` for a list of all other metrics
-        and their arguments. Defaults to an empty dictionary.
+        Extra arguments for the distance metric used to compute the RDMs. Refer to
+        :mod:`scipy.spatial.distance` for a list of all other metrics and their
+        arguments. Defaults to an empty dictionary.
     rsa_metric : str
         The RSA metric to use to compare the RDMs. Valid options are:
 
         * 'spearman' for Spearman's correlation (the default)
         * 'pearson' for Pearson's correlation
         * 'kendall-tau-a' for Kendall's Tau (alpha variant)
         * 'partial' for partial Pearson correlations
         * 'partial-spearman' for partial Spearman correlations
         * 'regression' for linear regression weights
 
         Defaults to 'spearman'.
     ignore_nan : bool
-        Whether to treat NaN's as missing values and ignore them when computing
-        the distance metric. Defaults to ``False``.
+        Whether to treat NaN's as missing values and ignore them when computing the
+        distance metric. Defaults to ``False``.
 
         .. versionadded:: 0.8
     y : ndarray of int, shape (n_items,) | None
-        For each item, a number indicating the class to which the item belongs.
-        When ``None``, each item is assumed to belong to a different class.
+        (Deprecated) For each item, a number indicating the class to which the item
+        belongs.  When ``None``, each item is assumed to belong to a different class.
         Defaults to ``None``.
+    labels_rdm_model: list | None
+        For each row in ``rdm_model``, a label that identifies the item to which it
+        corresponds. This is used in combination with ``labels_X`` to align the data and
+        model RDMs before comparing them. Each row should have a unique label. Labels
+        may be of any python type that can be compared with ``==`` (int, float, string,
+        tuple, etc). By default (``None``), the integers ``0:n_rows`` are used as
+        labels.
+
+        .. versionadded:: 0.10
+    labels_X : list | None
+        For each element in ``X`` (=the first dimension), a label that identifies the
+        item to which it corresponds. This is used in combination with
+        ``labels_rdm_model`` to align the data and model RDMs before comparing them.
+        Multiple elements in ``X`` may correspond to the same item, in which case they
+        should have the same label and will be averaged when computing the data RDM.
+        Labels may be of any python type that can be compared with ``==`` (int, float,
+        string, tuple, etc). By default (``None``), the integers ``0:len(X)`` are used
+        as labels.
+
+        .. versionadded:: 0.10
     n_folds : int | sklearn.model_selection.BaseCrollValidator | None
-        Number of cross-validation folds to use when computing the distance
-        metric. Folds are created based on the ``y`` parameter. Specify
-        ``None`` to use the maximum number of folds possible, given the data.
-        Alternatively, you can pass a Scikit-Learn cross validator object (e.g.
-        ``sklearn.model_selection.KFold``) to assert fine-grained control over
-        how folds are created.
+        Number of cross-validation folds to use when computing the distance metric.
+        Folds are created based on the ``y`` parameter. Specify ``None`` to use the
+        maximum number of folds possible, given the data. Alternatively, you can pass a
+        Scikit-Learn cross validator object (e.g. ``sklearn.model_selection.KFold``) to
+        assert fine-grained control over how folds are created.
         Defaults to 1 (no cross-validation).
     n_jobs : int
-        The number of processes (=number of CPU cores) to use. Specify -1 to
-        use all available cores. Defaults to 1.
+        The number of processes (=number of CPU cores) to use. Specify -1 to use all
+        available cores. Defaults to 1.
     verbose : bool
-        Whether to display a progress bar. In order for this to work, you need
-        the tqdm python module installed. Defaults to False.
+        Whether to display a progress bar. In order for this to work, you need the tqdm
+        python module installed. Defaults to False.
 
     Returns
     -------
     rsa_vals : ndarray, shape ([n_series,] [n_times,] [n_model_rdms])
-        The RSA value for each searchlight patch. When ``spatial_radius`` is
-        set to ``None``, there will only be no ``n_series`` dimension. When
-        ``temporal_radius`` is set to ``None``, there will be no time
-        dimension. When multiple models have been supplied, the last dimension
-        will contain RSA results for each model.
+        The RSA value for each searchlight patch. When ``spatial_radius`` is set to
+        ``None``, there will only be no ``n_series`` dimension. When ``temporal_radius``
+        is set to ``None``, there will be no time dimension. When multiple models have
+        been supplied, the last dimension will contain RSA results for each model.
 
     See Also
     --------
     searchlight
     compute_rdm
     rdm_array
+
     """
     if patches is None:
         patches = searchlight(X.shape)  # One big searchlight patch
 
     # Create folds for cross-validated RDM metrics
     X = create_folds(X, y, n_folds)
     # The data is now folds x items x n_series x n_times
 
-    if type(rdm_model) == list:
+    if isinstance(rdm_model, list):
         rdm_model = [_ensure_condensed(rdm, "rdm_model") for rdm in rdm_model]
     else:
         rdm_model = [_ensure_condensed(rdm_model, "rdm_model")]
 
     if ignore_nan:
         masks = [~np.isnan(rdm) for rdm in rdm_model]
     else:
```

### Comparing `mne-rsa-0.9/mne_rsa/searchlight.py` & `mne_rsa-0.91/mne_rsa/searchlight.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Classes and functions having to do with creating searchlights."""
+
 import numpy as np
 from mne.utils import logger
 
 
 class searchlight:
     """Generate indices for searchlight patches.
 
@@ -88,14 +89,15 @@
         A single searchlight patch. Each element of the tuple corresponds to a
         dimension of the data array and can be used to index along this
         dimension to extract the searchlight patch.
 
     Attributes
     ----------
     shape
+
     """
 
     def __init__(
         self,
         shape,
         dist=None,
         spatial_radius=None,
@@ -320,14 +322,15 @@
                 One element: the number of time-series for which patches are
                 generated.
             For a temporal searchlight:
                 One element: the number of time-samples for which patches are
                 generated.
             For no searchlight:
                 Zero elements.
+
         """
         if self.spatial_radius is not None and self.temporal_radius is not None:
             return (len(self.sel_series), len(self.time_centers))
         elif self.spatial_radius is not None:
             return (len(self.sel_series),)
         elif self.temporal_radius is not None:
             return (len(self.time_centers),)
@@ -356,14 +359,15 @@
     radius : float
         The maximum distance that points can be to be included.
 
     Returns
     -------
     ind : ndarray, shape (n_points_in_radius,)
         Indices of all points in the given radius from the seed point.
+
     """
     from scipy.sparse import issparse
 
     if issparse(dist):
         # Treat all zero distances as missing data
         ind = dist[seed].nonzero()[1]
         # Find indices for points within the radius
```

### Comparing `mne-rsa-0.9/mne_rsa/sensor_level.py` & `mne_rsa-0.91/mne_rsa/sensor_level.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-"""
-Module implementing representational similarity analysis (RSA) at the sensor level.
+"""Module implementing representational similarity analysis (RSA) at the sensor level.
 
 Kriegeskorte, N., Mur, M., & Bandettini, P. A. (2008). Representational similarity
 analysis - connecting the branches of systems neuroscience. Frontiers in Systems
 Neuroscience, 2(November), 4. https://doi.org/10.3389/neuro.06.004.2008
 
 Authors
 -------
 Marijn van Vliet <w.m.vanvliet@gmail.com>
 """
+
 import numpy as np
 from scipy.spatial import distance
 import mne
 from mne.utils import logger
 from mne.cov import compute_whitener
 
 from .rdm import _n_items_from_rdm, rdm_array
@@ -133,16 +133,17 @@
         None, there will only be one virtual sensor. When temporal_radius is set to
         None, there will only be one time point. When multiple models have been
         supplied, a list will be returned containing the RSA results for each model.
 
     See Also
     --------
     compute_rdm
+
     """
-    one_model = type(rdm_model) != list
+    one_model = isinstance(rdm_model, list)
     if one_model:
         rdm_model = [rdm_model]
 
     logger.info(f"Performing RSA between Evokeds and {len(rdm_model)} model RDM(s)")
 
     # Check for compatibility of the evokeds and the model features
     for rdm in rdm_model:
@@ -372,14 +373,15 @@
         None, there will only be one virtual sensor. When temporal_radius is set to
         None, there will only be one time point. When multiple models have been
         supplied, a list will be returned containing the RSA results for each model.
 
     See Also
     --------
     compute_rdm
+
     """
     one_model = type(rdm_model) is np.ndarray
     if one_model:
         rdm_model = [rdm_model]
 
     logger.info(f"Performing RSA between Epochs and {len(rdm_model)} model RDM(s)")
 
@@ -415,15 +417,15 @@
                 "    Using diagonal values of the covariance matrix to whiten "
                 "the data."
             )
             noise_cov = noise_cov.as_diag()
         else:
             logger.info("    Using covariance matrix to whiten the data.")
         W, _ = compute_whitener(noise_cov, epochs.info, picks=picks)
-        epochs._data[picks] = W @ epochs._data[picks]
+        epochs._data[:, picks] = (W @ epochs._data[:, picks].T).T
 
     if spatial_radius is not None:
         logger.info(f"    Spatial radius: {spatial_radius} meters")
         logger.info(f"    Using {len(picks)} sensors")
 
         # Compute the distances between the sensors
         locs = np.vstack([ch["loc"][:3] for ch in epochs.info["chs"]])
@@ -432,15 +434,15 @@
         dist = None
 
     if temporal_radius is not None:
         logger.info(f"    Temporal radius: {temporal_radius} samples")
         logger.info(f"    Time interval: {tmin}-{tmax} seconds")
 
     # Perform the RSA
-    X = epochs.get_data()
+    X = epochs.get_data(copy=False)
     patches = searchlight(
         X.shape,
         dist=dist,
         spatial_radius=spatial_radius,
         temporal_radius=temporal_radius,
         sel_series=picks,
         samples_from=samples_from,
@@ -555,14 +557,15 @@
         time point. This value is given in seconds. Defaults to ``None``, in which case
         patches are generated up to and including the last time point.
 
     Yields
     ------
     rdm : ndarray, shape (n_items, n_items)
         A RDM for each searchlight patch.
+
     """
     times = evokeds[0].times
     for evoked in evokeds:
         if np.any(evoked.times != times):
             raise ValueError("Not all evokeds have the same time points.")
 
     # Convert the temporal radius to samples
@@ -683,14 +686,15 @@
 
         .. versionadded:: 0.8
 
     Yields
     ------
     rdm : ndarray, shape (n_items, n_items)
         A RDM for each searchlight patch.
+
     """
     if y is None:
         y = epochs.events[:, 2]
 
     # Convert the temporal radius to samples
     if temporal_radius is not None:
         temporal_radius = round(epochs.info["sfreq"] * temporal_radius)
@@ -717,15 +721,15 @@
         # Compute the distances between the sensors
         locs = np.vstack([ch["loc"][:3] for ch in epochs.info["chs"]])
         dist = distance.squareform(distance.pdist(locs))
     else:
         dist = None
 
     # Compute the RDMs
-    X = epochs.get_data()
+    X = epochs.get_data(copy=False)
     patches = searchlight(
         X.shape,
         dist=dist,
         spatial_radius=spatial_radius,
         temporal_radius=temporal_radius,
         sel_series=picks,
         samples_from=samples_from,
```

### Comparing `mne-rsa-0.9/mne_rsa/source_level.py` & `mne_rsa-0.91/mne_rsa/source_level.py`

 * *Files 2% similar despite different names*

```diff
@@ -207,17 +207,15 @@
         f"Performing RSA between SourceEstimates and {len(rdm_model)} model RDM(s)"
     )
     if spatial_radius is not None:
         logger.info(f"    Spatial radius: {spatial_radius} meters")
     if sel_vertices is not None:
         logger.info(f"    Using {len(sel_series)} vertices")
     else:
-        logger.info(
-            f"    Using {sum(len(v) for v in stcs[0].vertices)} vertices"
-        )
+        logger.info(f"    Using {sum(len(v) for v in stcs[0].vertices)} vertices")
     if temporal_radius is not None:
         logger.info(f"    Temporal radius: {temporal_radius} samples")
     if tmin is not None or tmax is not None:
         logger.info(f"    Time interval: {tmin}-{tmax} seconds")
 
     # Perform the RSA
     X = np.array([stc.data for stc in stcs])
@@ -379,14 +377,15 @@
         Whether to display a progress bar. In order for this to work, you need
         the tqdm python module installed. Defaults to False.
 
     Yields
     ------
     rdm : ndarray, shape (n_items, n_items)
         A RDM for each searchlight patch.
+
     """
     src = _check_stcs_compatibility(stcs, src)
     if spatial_radius is not None:
         dist = _get_distance_matrix(src, dist_lim=spatial_radius, n_jobs=n_jobs)
     else:
         dist = None
 
@@ -732,14 +731,15 @@
         The correlation values for each searchlight patch. When multiple models
         have been supplied, a list will be returned containing the RSA results
         for each model.
 
     See Also
     --------
     compute_rdm
+
     """
     # Check for compatibility of the source estimates and the model features
     one_model = type(rdm_model) is np.ndarray
     if one_model:
         rdm_model = [rdm_model]
 
     if (
@@ -914,14 +914,15 @@
         Whether to display a progress bar. In order for this to work, you need
         the tqdm python module installed. Defaults to False.
 
     Yields
     ------
     rdm : ndarray, shape (n_items, n_items)
         A RDM for each searchlight patch.
+
     """
     if (
         not isinstance(image, tuple(nib.imageclasses.all_image_classes))
         or image.ndim != 4
     ):
         raise ValueError("The image data must be 4-dimensional Nifti-like " "images")
 
@@ -1034,14 +1035,15 @@
         Number of CPU cores to use if distance computation is necessary.
         Defaults to 1.
 
     Returns
     -------
     dist : ndarray (n_vertices, n_vertices)
         The vertex-to-vertex distance matrix.
+
     """
     dist = []
 
     # Check if distances have been pre-computed in the given source space. Give
     # a warning if the pre-computed distances may have had a too limited
     # dist_lim setting.
     needs_distance_computation = False
@@ -1095,14 +1097,15 @@
         reduce computation time.
 
     Returns
     -------
     src : instance of mne.SourceSpaces
         The volume source space, now with the 'dist' and 'dist_limit' fields
         set.
+
     """
     # Lazy import to not have to load the huge scipy module every time mne_rsa
     # get's loaded.
     from scipy.sparse import csr_matrix
 
     assert src.kind == "volume"
     n_sources = src[0]["np"]
@@ -1121,40 +1124,14 @@
     i = i.ravel()[idx]
     j = j.ravel()[idx]
     src[0]["dist"] = csr_matrix((d, (i, j)), shape=(n_sources, n_sources))
     src[0]["dist_limit"] = np.array([dist_limit], "float32")
     return src
 
 
-def make_mri_con_matrix(img):
-    from scipy.sparse import csr_matrix
-
-    # Create 3 x 3 x 3 cube of (ijk) indices, centered around (0, 0, 0)
-    cube = np.array(list(np.ndindex(3, 3, 3))) - [1, 1, 1]
-    # Remove center of the cube
-    cube = np.delete(cube, len(cube) // 2, axis=0)
-    # Compute distance from all points in the cube to the center
-    dist = np.linalg.norm(cube @ img.affine[:3, :3], axis=1)
-    # Copy the cube, centering it around each voxel
-    voxels = np.array(list(np.ndindex(*img.shape[:3])))
-    neighbours = voxels[:, :, np.newaxis] + cube.T[np.newaxis, :, :]
-    assert neighbours.shape == (len(voxels), 3, len(cube))
-    # Convert ijk coordinates to voxel numbers
-    neighbours = np.ravel_multi_index(
-        (neighbours[:, 0, :], neighbours[:, 1, :], neighbours[:, 2, :]),
-        img.shape[:3],
-        mode="clip",
-    )
-    rows = np.repeat(np.arange(neighbours.shape[0]), neighbours.shape[1])
-    cols = neighbours.ravel()
-    dist = np.tile(dist, neighbours.shape[0])
-    con_matrix = csr_matrix((dist, (rows, cols)), shape=(len(voxels), len(voxels)))
-    return con_matrix
-
-
 def backfill_stc_from_rois(values, rois, src, tmin=0, tstep=1, subject=None):
     """Backfill the ROI values into a full mne.SourceEstimate object.
 
     Each vertex belonging to the same region of interest (ROI) will have the
     sample value.
 
     Parameters
@@ -1175,14 +1152,15 @@
     subject : str | None
         The name of the FreeSurfer subject.
 
     Returns
     -------
     stc : mne.SourceEstimate
         The backfilled source estimate object.
+
     """
     values = np.asarray(values)
     if values.ndim == 1:
         n_samples = 1
     else:
         n_samples = values.shape[1]
     data = np.zeros((src[0]["nuse"] + src[1]["nuse"], n_samples))
@@ -1279,14 +1257,15 @@
         If not None, override default verbose level (see :func:`mne.verbose`
         and :ref:`Logging documentation <tut_logging>` for more).
 
     Returns
     -------
     src_out : instance of SourceSpaces
         The restricted source space.
+
     """
     src_out = deepcopy(src)
 
     vert_no_lh, vert_no_rh = vertno
     if not (
         np.all(np.in1d(vert_no_lh, src[0]["vertno"]))
         and np.all(np.in1d(vert_no_rh, src[1]["vertno"]))
```

### Comparing `mne-rsa-0.9/mne_rsa/viz.py` & `mne_rsa-0.91/mne_rsa/viz.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,46 @@
-from functools import partial
+"""Functions related to visualization of RDMs."""
+
 import types
+from functools import partial
+
 import matplotlib.pyplot as plt
-from matplotlib.cm import get_cmap
+import numpy as np
 from mne.viz import Brain
 from mne.viz.topo import _iter_topography
-import numpy as np
 from scipy.spatial import distance
 
 
 def plot_rdms(rdms, names=None, items=None, n_rows=1, cmap="viridis", title=None):
-    """Plot one or more RDMs
+    """Plot one or more RDMs.
 
     Parameters
     ----------
     rdms : ndarray | list of ndarray
-        The RDM or list of RDMs to plot. The RDMs can either be two-dimensional
-        (n_items x n_items) matrices or be in condensed form.
+        The RDM or list of RDMs to plot. The RDMs can either be two-dimensional (n_items
+        x n_items) matrices or be in condensed form.
     names : str | list of str | None
         For each given RDM, a name to show above it. Defaults to no names.
     items : list of str | None
-        The each item (row/col) in the RDM, a string description. This will be
-        displayed along the axes. Defaults to None which means the items will
-        be numbered.
+        The each item (row/col) in the RDM, a string description. This will be displayed
+        along the axes. Defaults to None which means the items will be numbered.
     n_rows : int
-        Number of rows to use when plotting multiple RDMs at once. Defaults to
-        1.
+        Number of rows to use when plotting multiple RDMs at once. Defaults to 1.
     cmap : str
         Matplotlib colormap to use. See
         https://matplotlib.org/gallery/color/colormap_reference.html
         for all possibilities. Defaults to 'viridis'.
     title : str | None
         Title for the entire figure. Defaults to no title.
 
     Returns
     -------
     fig : matplotlib figure
         The figure produced by matplotlib
+
     """
     if not isinstance(rdms, list):
         rdms = [rdms]
 
     if isinstance(names, str):
         names = [names]
     if names is not None and len(names) != len(rdms):
@@ -77,27 +78,27 @@
     plt.colorbar(im, ax=ax)
     if title is not None:
         plt.suptitle(title)
     return fig
 
 
 def _click_func(ax, ch_idx, rdms, cmap):
-    """Function used to plot a single RDM interactively.
+    """Plot a single RDM interactively.
 
     Parameters
     ----------
     ax: matplotlib.Axes.axes
         Axes.axes object on which a new single RDM is plotted.
     ch_idx: int
         Index of a channel.
     rdms: ndarray, shape (n_sensors, n_rdm_datapoint)
         RDMs of MEG recordings; there's one RDM for each sensor.
     cmap: str
-        Colormap used for plotting RDMs.
-        Check matplotlib.pyplot.imshow for details.
+        Colormap used for plotting RDMs. Check ``matplotlib.pyplot.imshow`` for details.
+
     """
     rdm = rdms[ch_idx]
     rdm = distance.squareform(rdm)
     ax.imshow(rdm, cmap=cmap)
 
 
 def _plot_rdms_topo_timepoint(
@@ -114,28 +115,28 @@
     show=False,
 ):
     """Plot RDMs on 2D MEG topography.
 
     Parameters
     ----------
     rdms: ndarray, shape (n_sensors, n_rdm_datapoints) | generator
-        RDMs of MEG recordings; one RDM for each sensor.
-        Can also be a generator of RDMs as produced by the :func:`rdm_epochs`,
+        RDMs of MEG recordings; one RDM for each sensor. Can also be a generator of RDMs
+        as produced by the :func:`rdm_epochs`,
         :func:`rdm_evokeds` or :func:`rdm_array` functions.
     info: mne.io.meas_info.Info
         Info object that contains meta data of MEG recordings.
     layout: mne.channels.layout.Layout | None
-        Layout objects containing sensor layout info.
-        The default (``None``) will figure out layout based on info.
+        Layout objects containing sensor layout info. The default (``None``) will figure
+        out layout based on info.
     fig: matplotlib.pyplot.Figure | None
-        Figure object on which RDMs on 2D MEG topography are plotted.
-        The default (``None``) creates a new Figure object.
+        Figure object on which RDMs on 2D MEG topography are plotted. The default
+        (``None``) creates a new Figure object.
     title: str | None
-        Title of the plot, used only when ``fig=None``.
-        The default (``None``) puts no title in the figure.
+        Title of the plot, used only when ``fig=None``. The default (``None``) puts no
+        title in the figure.
     axis_facecolor: str
         Face color of the each RDM. Defaults to 'w', white.
     axis_spinecolor: str
         Spine color of each RDM. Defaults to 'w', white.
     fig_facecolor: str
         Face color of the entire topography. Defaults to 'w', white.
     figsize: tuple of float
@@ -147,14 +148,15 @@
     show: bool
         Whether to display the generated figure. Defaults to False.
 
     Returns
     -------
     fig: matplotlib.pyplot.Figure
         Figure object in which RDMs are plotted on 2D MEG topography.
+
     """
     on_pick = partial(_click_func, rdms=rdms, cmap=cmap)
 
     if fig is None:
         fig = plt.figure(figsize=figsize)
         if title is not None:
             fig.suptitle(title, x=0.98, horizontalalignment="right")
@@ -192,35 +194,33 @@
     axis_facecolor="w",
     axis_spinecolor="w",
     fig_facecolor="w",
     figsize=(6.4, 4.8),
     cmap="viridis",
     show=True,
 ):
-    """Plot RDMs on 2D sensor topography
+    """Plot RDMs on 2D sensor topography.
 
     Parameters
     ----------
     rdms: ndarray | numpy.memmap, shape (n_sensors,[ n_times,] n_rdm_datapts)
         RDMs of MEG/EEG recordings; one RDM for each sensor and time point.
     info: mne.io.meas_info.Info
         Info object that contains meta data of MEG/EEG recordings.
     time: int | [int, int] | None
-        A time point (int) or time window ([int, int]) for which RDMs are
-        plotted. When a time window is given, averge RDMs for the window are
-        plotted. The default (``None``) plots the average RDMs of all the time
-        points. Start of the time window is inclusive, while the end is
-        exclusive.
+        A time point (int) or time window ([int, int]) for which RDMs are plotted. When
+        a time window is given, averge RDMs for the window are plotted. The default
+        (``None``) plots the average RDMs of all the time points. Start of the time
+        window is inclusive, while the end is exclusive.
     layout: mne.channels.layout.Layout, optional
-        Layout objects containing sensor layout info.
-        The default, ``layout=None``, will figure out layout based on info.
+        Layout objects containing sensor layout info. The default, ``layout=None``, will
+        figure out layout based on info.
     fig: matplotlib.pyplot.Figure | None, optional
-        Figure object on which RDMs on 2D sensor topography are plotted.
-        The default (``None``) creates a new Figure object
-        with a title based on time parameter.
+        Figure object on which RDMs on 2D sensor topography are plotted. The default
+        (``None``) creates a new Figure object with a title based on time parameter.
     axis_facecolor: str, optional
         Face color of the each RDM. Defaults to 'w', white.
     axis_spinecolor: str, optional
         Spine color of each RDM. Defaults to 'w', white.
     fig_facecolor: str, optional
         Face color of the entire topography. Defaults to 'w', white.
     figsize: tuple of float, optional
@@ -232,14 +232,15 @@
     show: bool, optional
         Whether to display the generated figure. Defaults to ``True``.
 
     Returns
     -------
     fig: matplotlib.pyplot.Figure
         Figure object in which RDMs are plotted on 2D sensor topography.
+
     """
     if isinstance(rdms, types.GeneratorType):
         rdms = np.array(list(rdms))
 
     if rdms.ndim != 2 and rdms.ndim != 3:
         raise ValueError(
             "rdms have to be a 2D or 3D ndarray or numpy.memmap, "
@@ -300,30 +301,30 @@
     values : array-like, shape (n_rois,)
         The values to plot. One value per ROI.
     rois : list of mne.Label
         The labels corrsponding to the ROIs.
     subject : str
         The name of the FreeSurfer subject to plot the brain for.
     subjects_dir : str
-        The folder in which the FreeSurfer subject data is kept. Inside this
-        folder should be a folder with the same name as the `subject`
-        parameter.
+        The folder in which the FreeSurfer subject data is kept. Inside this folder
+        should be a folder with the same name as the `subject` parameter.
     cmap : str
         The name of the matplotlib colormap to use. Defaults to 'plasma'.
     alpha : float
-        The alpha (opacity, 1.0 is fully opaque, 0.0 is fully transparant) of
-        the data being plotted on top of the brain.
+        The alpha (opacity, 1.0 is fully opaque, 0.0 is fully transparant) of the data
+        being plotted on top of the brain.
 
     Returns
     -------
     brain : mne.viz.Brain
         The MNE-Python brain plotting object that was created and currently
         being shown. You can use this to modify the plot.
+
     """
-    cmap = get_cmap(cmap)
+    cmap = plt.get_cmap(cmap)
     max_val = np.max(values)
     brain = Brain(
         subject=subject, subjects_dir=subjects_dir, surf="inflated", hemi="both"
     )
     labels_lh = np.zeros(len(brain.geo["lh"].coords), dtype=int)
     labels_rh = np.zeros(len(brain.geo["rh"].coords), dtype=int)
     ctab_lh = list()
```

### Comparing `mne-rsa-0.9/tests/test_folds.py` & `mne_rsa-0.91/tests/test_folds.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-import pytest
+"""Unit tests for the creation of cross-validation folds."""
+
 import numpy as np
+import pytest
+from mne_rsa.folds import _compute_item_means, _convert_to_one_hot, create_folds
 from numpy.testing import assert_equal
 
-from mne_rsa.folds import create_folds, _convert_to_one_hot, _compute_item_means
-
 
 class TestCreateFolds:
     """Test the create_folds function."""
 
     def test_basic(self):
         """Test basic invocation of create_folds."""
         data = np.array([1, 1, 1, 2, 2, 2, 3, 3, 3])
```

### Comparing `mne-rsa-0.9/tests/test_rsa.py` & `mne_rsa-0.91/tests/test_rsa.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,62 +1,65 @@
-import pytest
+"""Unit tests for comparing RDMs (which is called RSA)."""
+
 from types import GeneratorType
+
 import numpy as np
-from numpy.testing import assert_allclose, assert_equal
-from mne_rsa import searchlight, rsa, rsa_gen, rsa_array
+import pytest
+from mne_rsa import rsa, rsa_array, rsa_gen, searchlight
 from mne_rsa.rsa import _kendall_tau_a, _partial_correlation
+from numpy.testing import assert_allclose, assert_equal
 
 
 def rdm():
-    """Create an example RDM"""
+    """Create an example RDM."""
     return np.array([1, 2, 3, 4, 5, 6])
 
 
 def rdm_gen(rdms):
-    """Generator for RDMs"""
+    """Generate RDMs."""
     for rdm in rdms:
         yield np.asarray(rdm)
 
 
 class TestRSAGen:
-    """Test the rsa_gen function"""
+    """Test the rsa_gen function."""
 
     def test_return_type(self):
-        """Test return type of rsa_gen"""
+        """Test return type of rsa_gen."""
         assert isinstance(rsa_gen(rdm_gen([rdm()]), rdm()), GeneratorType)
         assert next(rsa_gen(rdm_gen([rdm()]), rdm())).shape == tuple()
         assert next(rsa_gen(rdm_gen([rdm()]), [rdm()])).shape == (1,)
 
     def test_spearman(self):
-        """Test computing RSA with Spearman correlation"""
+        """Test computing RSA with Spearman correlation."""
         data_rdm = rdm_gen([[1, 2, 3]])
         model_rdm = np.array([2, 3, 3.5])
         assert next(rsa_gen(data_rdm, model_rdm, metric="spearman")) == 1.0
 
         data_rdm = rdm_gen([[np.NaN, 2, 3, 4, 5]])
         model_rdm = np.array([2, np.NaN, 3.5, 4, 5])
         assert (
             next(rsa_gen(data_rdm, model_rdm, metric="spearman", ignore_nan=True))
             == 1.0
         )
 
     def test_pearson(self):
-        """Test computing RSA with Pearson correlation"""
+        """Test computing RSA with Pearson correlation."""
         data_rdm = rdm_gen([[1, 2, 3]])
         model_rdm = np.array([2, 3, 3.5])
         assert next(rsa_gen(data_rdm, model_rdm, metric="pearson")) < 1.0
 
         data_rdm = rdm_gen([[np.NaN, 2, 3, 4, 5]])
         model_rdm = np.array([2, np.NaN, 3.5, 4, 5])
         assert (
             next(rsa_gen(data_rdm, model_rdm, metric="pearson", ignore_nan=True)) < 1.0
         )
 
     def test_kendall_tau_a(self):
-        """Test computing RSA with Kendall's Tau Alpha"""
+        """Test computing RSA with Kendall's Tau Alpha."""
         data_rdm = rdm_gen([[1, 2, 3]])
         model_rdm = np.array([1, 3, 3])  # This metric deals well with ties
         rsa_val = next(rsa_gen(data_rdm, model_rdm, metric="kendall-tau-a"))
         assert rsa_val == 2 / 3
 
         data_rdm = rdm_gen([[1, np.NaN, 2, 3, 4]])
         model_rdm = np.array([1, 2, 3, 3, np.NaN])
@@ -144,25 +147,25 @@
             next(rsa_gen(rdm_gen([[1, 2, np.NaN, 4, 5, 6]]), rdm(), ignore_nan=True)),
             1,
             atol=1e-15,
         )
 
 
 class TestRSA:
-    """Test the main RSA function"""
+    """Test the main RSA function."""
 
     # Most of the functionality is already tested in TestRSAGen
     def test_return_type(self):
-        """Test return type of rsa_gen"""
+        """Test return type of rsa_gen."""
         assert isinstance(rsa([rdm()], rdm()), np.ndarray)
         assert rsa(rdm(), rdm()).shape == tuple()
         assert rsa(rdm(), [rdm()]).shape == (1,)
 
     def test_progress_bar(self):
-        """Test showing a progress bar for rsa"""
+        """Test showing a progress bar for rsa."""
         assert rsa([rdm()], rdm(), verbose=True) == [1.0]
         assert rsa([rdm()], rdm(), verbose=True, n_data_rdms=1) == [1.0]
         assert rsa(rdm_gen([rdm()]), rdm(), verbose=True) == [1.0]
 
     def test_parallel_processing(self):
         """Test running rsa with multiple cores."""
         assert_equal(rsa([rdm(), rdm()], rdm(), n_jobs=2), [1.0, 1.0])
@@ -293,16 +296,18 @@
             data, [model_rdm, model_rdm], patches, data_rdm_metric="euclidean", n_jobs=2
         )
         assert rsa_result.shape == (2, 1, 2)
         assert_equal(rsa_result, 1)
 
 
 class TestKendallTau:
+    """Test computing Kendall's Tau Alpha metric."""
+
     def test_basic(self):
-        """Test computing Kendall's Tau Alpha"""
+        """Test computing Kendall's Tau Alpha."""
         # This metric deals well with ties
         assert _kendall_tau_a([1, 2, 3], [1, 3, 3]) == 2 / 3
 
         # Test taken from scipy
         assert _kendall_tau_a([9, 2, 5, 6], [4, 7, 9, 11]) == 0
 
     def test_sizes(self):
@@ -316,14 +321,16 @@
 
     def test_only_ties(self):
         """Test Kendall's Tau Alpha where every value is a tie."""
         assert np.isnan(_kendall_tau_a([1, 1, 1], [2, 2, 2]))
 
 
 class TestPartialCorrelation:
+    """Test partial correlations."""
+
     def test_basic(self):
         """Test computing partial correlations."""
         data_rdm = [2, 4, 15, 20]
         model_rdms = [[1, 2, 3, 4], [0, 0, 1, 1]]
         assert_allclose(
             _partial_correlation(data_rdm, model_rdms, type="pearson"),
             [0.919145, 0.912871],
```

### Comparing `mne-rsa-0.9/tests/test_searchlight.py` & `mne_rsa-0.91/tests/test_searchlight.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
+"""Unit tests for the searchlight patch generator."""
+
 import pytest
 import numpy as np
 from numpy.testing import assert_equal
 from scipy import sparse
 
 from mne_rsa import searchlight
 
 
 class TestSearchLight:
-    """Test the searchlight generator class"""
+    """Test the searchlight generator class."""
 
     def test_iter_spatio_temporal(self):
         """Test generating spatio-temporal searchlight patches."""
         dist = np.array([[0, 1, 2], [1, 0, 1], [2, 1, 0]])
         s = searchlight((10, 3, 4), dist, spatial_radius=2, temporal_radius=1)
         assert len(s) == 6
         assert s.shape == (3, 2)
```

