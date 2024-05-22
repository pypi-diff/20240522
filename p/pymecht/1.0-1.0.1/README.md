# Comparing `tmp/pymecht-1.0.tar.gz` & `tmp/pymecht-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymecht-1.0.tar", last modified: Tue Dec 12 11:59:07 2023, max compression
+gzip compressed data, was "pymecht-1.0.1.tar", last modified: Wed May 22 08:56:08 2024, max compression
```

## Comparing `pymecht-1.0.tar` & `pymecht-1.0.1.tar`

### file list

```diff
@@ -1,61 +1,61 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.973371 pymecht-1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.953371 pymecht-1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.961371 pymecht-1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2023-12-12 11:58:57.000000 pymecht-1.0/.github/workflows/ci-tests.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2023-12-12 11:58:57.000000 pymecht-1.0/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       88 2023-12-12 11:58:57.000000 pymecht-1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-12 11:58:57.000000 pymecht-1.0/.readthedocs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.961371 pymecht-1.0/Examples/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9656 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/biax-data.npz
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/biax-fitting.py
--rw-r--r--   0 runner    (1001) docker     (127)     3578 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/biax-model-prob.py
--rw-r--r--   0 runner    (1001) docker     (127)     5642 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/examples.py
--rw-r--r--   0 runner    (1001) docker     (127)     2091 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/test2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2246 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/tube-model-prob.py
--rw-r--r--   0 runner    (1001) docker     (127)    78167 2023-12-12 11:58:57.000000 pymecht-1.0/Examples/tutorial.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2023-12-12 11:58:57.000000 pymecht-1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-12-12 11:59:07.973371 pymecht-1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3353 2023-12-12 11:58:57.000000 pymecht-1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.961371 pymecht-1.0/Tests/
--rw-r--r--   0 runner    (1001) docker     (127)     8086 2023-12-12 11:58:57.000000 pymecht-1.0/Tests/test_examples.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.965371 pymecht-1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      638 2023-12-12 11:58:57.000000 pymecht-1.0/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      804 2023-12-12 11:58:57.000000 pymecht-1.0/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      503 2023-12-12 11:58:57.000000 pymecht-1.0/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.969371 pymecht-1.0/docs/source/
--rw-r--r--   0 runner    (1001) docker     (127)    21044 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/biax.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2153 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      118 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/matmodel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      125 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/mcmc.rst
--rw-r--r--   0 runner    (1001) docker     (127)      140 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/paramdict.rst
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/paramfitter.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/randomparameters.rst
--rw-r--r--   0 runner    (1001) docker     (127)      142 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/sampleexperiment.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/theory_biax.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/theory_matmodel.rst
--rw-r--r--   0 runner    (1001) docker     (127)      739 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/theory_spring.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/theory_tube.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2197 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/theory_uniaxial.rst
--rw-r--r--   0 runner    (1001) docker     (127)    42563 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/tube.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14316 2023-12-12 11:58:57.000000 pymecht-1.0/docs/source/uniax.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8870 2023-12-12 11:58:57.000000 pymecht-1.0/examples_CR.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.969371 pymecht-1.0/pymecht/
--rw-r--r--   0 runner    (1001) docker     (127)     3655 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/MCMC.py
--rw-r--r--   0 runner    (1001) docker     (127)    39283 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/MatModel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/ParamDict.py
--rw-r--r--   0 runner    (1001) docker     (127)     1870 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/ParamFitter.py
--rw-r--r--   0 runner    (1001) docker     (127)    11536 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/RandomParameters.py
--rw-r--r--   0 runner    (1001) docker     (127)    46056 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/SampleExperiment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1117 2023-12-12 11:58:57.000000 pymecht-1.0/pymecht/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-12 11:59:07.973371 pymecht-1.0/pymecht.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4064 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2023-12-12 11:59:07.000000 pymecht-1.0/pymecht.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2023-12-12 11:58:57.000000 pymecht-1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-12 11:59:07.973371 pymecht-1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       96 2023-12-12 11:58:57.000000 pymecht-1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.773103 pymecht-1.0.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.761103 pymecht-1.0.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.765103 pymecht-1.0.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-22 08:56:04.000000 pymecht-1.0.1/.github/workflows/ci-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-22 08:56:04.000000 pymecht-1.0.1/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       88 2024-05-22 08:56:04.000000 pymecht-1.0.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-22 08:56:04.000000 pymecht-1.0.1/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.765103 pymecht-1.0.1/Examples/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9656 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/biax-data.npz
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/biax-fitting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3578 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/biax-model-prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5642 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/examples.py
+-rw-r--r--   0 runner    (1001) docker     (127)    94075 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/examples_CR.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     2091 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/test2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2246 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/tube-model-prob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    78167 2024-05-22 08:56:04.000000 pymecht-1.0.1/Examples/tutorial.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-22 08:56:04.000000 pymecht-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-22 08:56:08.773103 pymecht-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3353 2024-05-22 08:56:04.000000 pymecht-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.765103 pymecht-1.0.1/Tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     8086 2024-05-22 08:56:04.000000 pymecht-1.0.1/Tests/test_examples.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.765103 pymecht-1.0.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      638 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.769103 pymecht-1.0.1/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (127)    21044 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/biax.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2153 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/matmodel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/mcmc.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/paramdict.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/paramfitter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/randomparameters.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/sampleexperiment.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/theory_biax.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/theory_matmodel.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/theory_spring.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4179 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/theory_tube.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2197 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/theory_uniaxial.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    42563 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/tube.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14316 2024-05-22 08:56:04.000000 pymecht-1.0.1/docs/source/uniax.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.769103 pymecht-1.0.1/pymecht/
+-rw-r--r--   0 runner    (1001) docker     (127)     3655 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/MCMC.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39283 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/MatModel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/ParamDict.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1870 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/ParamFitter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11536 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/RandomParameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46076 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/SampleExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1117 2024-05-22 08:56:04.000000 pymecht-1.0.1/pymecht/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 08:56:08.773103 pymecht-1.0.1/pymecht.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4066 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-22 08:56:08.000000 pymecht-1.0.1/pymecht.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-22 08:56:04.000000 pymecht-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 08:56:08.773103 pymecht-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       96 2024-05-22 08:56:04.000000 pymecht-1.0.1/setup.py
```

### Comparing `pymecht-1.0/.github/workflows/ci-tests.yml` & `pymecht-1.0.1/.github/workflows/ci-tests.yml`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,17 @@
       matrix:
         python-version: [3.8, 3.9, "3.10"]
         os: [ubuntu-latest, windows-latest, macos-latest]
     
     runs-on: ${{ matrix.os }}
 
     steps:
-    - uses: actions/checkout@v3
+    - uses: actions/checkout@v4
     - name: Set up Python ${{ matrix.python-version }}
-      uses: actions/setup-python@v1
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python-version }}
     
     # Yes we have to explictly install pytest. In a "real" example this could be included in a 
     # requirement.txt or environment.yml to setup your environment
     - name: Install pymecht
       run: |
```

### Comparing `pymecht-1.0/.github/workflows/python-publish.yml` & `pymecht-1.0.1/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/.readthedocs.yaml` & `pymecht-1.0.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/biax-data.npz` & `pymecht-1.0.1/Examples/biax-data.npz`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/biax-fitting.py` & `pymecht-1.0.1/Examples/biax-fitting.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/biax-model-prob.py` & `pymecht-1.0.1/Examples/biax-model-prob.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/examples.py` & `pymecht-1.0.1/Examples/examples.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/test2.py` & `pymecht-1.0.1/Examples/test2.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/tube-model-prob.py` & `pymecht-1.0.1/Examples/tube-model-prob.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Examples/tutorial.ipynb` & `pymecht-1.0.1/Examples/tutorial.ipynb`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/LICENSE` & `pymecht-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/PKG-INFO` & `pymecht-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymecht
-Version: 1.0
+Version: 1.0.1
 Summary: This is PYthon-based repository is for MECHanics of Tissue mechanics. The focus is on flexibility of adding new constitutive models and varying their parameters.
 Author-email: Ankush Aggarwal <ankush.aggarwal@glasgow.ac.uk>, Ross Williams <ross.williams@glasgow.ac.uk>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: numpy>=1.22.2
```

### Comparing `pymecht-1.0/README.md` & `pymecht-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/Tests/test_examples.py` & `pymecht-1.0.1/Tests/test_examples.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/Makefile` & `pymecht-1.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/make.bat` & `pymecht-1.0.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/biax.svg` & `pymecht-1.0.1/docs/source/biax.svg`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/conf.py` & `pymecht-1.0.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/index.rst` & `pymecht-1.0.1/docs/source/index.rst`

 * *Files 14% similar despite different names*

```diff
@@ -19,14 +19,21 @@
    :caption: Tutorials:
 
    Examples/tutorial.ipynb
 
 .. toctree::
    :glob:
    :maxdepth: 1
+   :caption: Examples:
+
+   Examples/examples_CR.ipynb
+
+.. toctree::
+   :glob:
+   :maxdepth: 1
    :caption: Theory:
 
    theory_matmodel
    theory_uniaxial
    theory_biax
    theory_tube
    theory_spring
```

### Comparing `pymecht-1.0/docs/source/theory_biax.rst` & `pymecht-1.0.1/docs/source/theory_biax.rst`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/theory_matmodel.rst` & `pymecht-1.0.1/docs/source/theory_matmodel.rst`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/theory_spring.rst` & `pymecht-1.0.1/docs/source/theory_spring.rst`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/theory_tube.rst` & `pymecht-1.0.1/docs/source/theory_tube.rst`

 * *Files 10% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 As a result, the Cauchy stress tensor can be calculated at any point
 (without the Lagrange multiplier :math:`p` term). The pressure
 difference between inside and outside of the artery can then be written
 as:
 
 .. math::
 
-   \Delta p = -\int\limits_{R_i}^{R_i+H}\frac{R}{\lambda_Z r^2} \left( \bar{\sigma}_{rr} - \bar{\sigma}_{\theta\theta} \right){\textrm{d}R}.
+   \Delta p = -\int\limits_{R_i}^{R_i+H}\frac{1}{\lambda_{\theta} \lambda_Z r} \left( \lambda_r \frac{\partial \Psi}{\partial {\lambda_r}} - \lambda_{\theta}\frac{\partial \Psi}{\partial {\lambda_{\theta}}} \right){\textrm{d}R}  = -\int\limits_{R_i}^{R_i+H}\frac{R}{\kappa\lambda_Z r^2} \left( \bar{\sigma}_{rr} - \bar{\sigma}_{\theta\theta} \right){\textrm{d}R}.
    \label{main-eq}
 
 This integral is evaluated numerically. If the fiber directions are not
 symmetric about the length of the cylinder, there could be shear stress
 components. However, these are neglected. Lastly, from the pressure
 difference :math:`\Delta p`, force acting on the cylinder can be
 calculated as :math:`f = 2\pi r_i L_0 \lambda_Z`. The deformation can be
```

### Comparing `pymecht-1.0/docs/source/theory_uniaxial.rst` & `pymecht-1.0.1/docs/source/theory_uniaxial.rst`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/tube.svg` & `pymecht-1.0.1/docs/source/tube.svg`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/docs/source/uniax.svg` & `pymecht-1.0.1/docs/source/uniax.svg`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/MCMC.py` & `pymecht-1.0.1/pymecht/MCMC.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/MatModel.py` & `pymecht-1.0.1/pymecht/MatModel.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/ParamDict.py` & `pymecht-1.0.1/pymecht/ParamDict.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/ParamFitter.py` & `pymecht-1.0.1/pymecht/ParamFitter.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/RandomParameters.py` & `pymecht-1.0.1/pymecht/RandomParameters.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht/SampleExperiment.py` & `pymecht-1.0.1/pymecht/SampleExperiment.py`

 * *Files 0% similar despite different names*

```diff
@@ -579,15 +579,15 @@
             raise ValueError("Input to disp_controlled should be a scalar, a list, or a numpy array")
 
         def integrand(xi,ri,params):
             R = self._Ri+xi*self._thick
             r = sqrt((R**2-self._Ri**2)/self._k/self._lambdaZ+ri**2)
             F = self._defGrad(r,R)
             sigma = self._compute(F,params) 
-            return R/self._lambdaZ/r**2*self._thick*(sigma[1,1]-sigma[0,0])
+            return R/(self._k*self._lambdaZ*r**2)*self._thick*(sigma[1,1]-sigma[0,0])
         
         if self._output=='pressure':
             output = [quad(integrand,0,1,args=(ri,params))[0] for ri in self._stretch(inp)]
         elif self._output =='force':
             output = [quad(integrand,0,1,args=(ri,params))[0]*self._L0*self._lambdaZ*pi*ri*2 for ri in self._stretch(inp)]
         if output_scalar:
             return output[0]
@@ -692,15 +692,15 @@
             ri = ri[0]
 
         def integrand(xi,ri,params):
             R = self._Ri+xi*self._thick
             r = sqrt((R**2-self._Ri**2)/self._k/self._lambdaZ+ri**2)
             F = self._defGrad(r,R)
             sigma = self._compute(F,params) 
-            return R/self._lambdaZ/r**2*self._thick*(sigma[1,1]-sigma[0,0])
+            return R/(self._k*self._lambdaZ*r**2)*self._thick*(sigma[1,1]-sigma[0,0])
 
         Stresses = []
         if pressure is None:
             pressure = quad(integrand,0,1,args=(ri,params))[0]
         xi = np.linspace(0,1,n)
         for xii in xi:
             R = self._Ri+xii*self._thick
```

### Comparing `pymecht-1.0/pymecht/__init__.py` & `pymecht-1.0.1/pymecht/__init__.py`

 * *Files identical despite different names*

### Comparing `pymecht-1.0/pymecht.egg-info/PKG-INFO` & `pymecht-1.0.1/pymecht.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymecht
-Version: 1.0
+Version: 1.0.1
 Summary: This is PYthon-based repository is for MECHanics of Tissue mechanics. The focus is on flexibility of adding new constitutive models and varying their parameters.
 Author-email: Ankush Aggarwal <ankush.aggarwal@glasgow.ac.uk>, Ross Williams <ross.williams@glasgow.ac.uk>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: matplotlib>=3.4.1
 Requires-Dist: numpy>=1.22.2
```

### Comparing `pymecht-1.0/pymecht.egg-info/SOURCES.txt` & `pymecht-1.0.1/pymecht.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 .gitignore
 .readthedocs.yaml
 LICENSE
 README.md
-examples_CR.ipynb
 pyproject.toml
 setup.py
 .github/workflows/ci-tests.yml
 .github/workflows/python-publish.yml
 Examples/__init__.py
 Examples/biax-data.npz
 Examples/biax-fitting.py
 Examples/biax-model-prob.py
 Examples/examples.py
+Examples/examples_CR.ipynb
 Examples/test2.py
 Examples/tube-model-prob.py
 Examples/tutorial.ipynb
 Tests/test_examples.py
 docs/Makefile
 docs/make.bat
 docs/requirements.txt
```

### Comparing `pymecht-1.0/pyproject.toml` & `pymecht-1.0.1/pyproject.toml`

 * *Files identical despite different names*

