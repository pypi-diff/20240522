# Comparing `tmp/bnlearn-0.8.7.tar.gz` & `tmp/bnlearn-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bnlearn-0.8.7.tar", last modified: Fri Apr 12 20:57:24 2024, max compression
+gzip compressed data, was "bnlearn-0.8.8.tar", last modified: Wed May 22 16:02:22 2024, max compression
```

## Comparing `bnlearn-0.8.7.tar` & `bnlearn-0.8.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.777326 bnlearn-0.8.7/
--rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.7/LICENSE
--rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.7/MANIFEST.in
--rw-rw-rw-   0        0        0    12768 2024-04-12 20:57:24.777326 bnlearn-0.8.7/PKG-INFO
--rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.7/README.md
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.698762 bnlearn-0.8.7/bnlearn/
--rw-rw-rw-   0        0        0     4729 2024-04-12 20:43:39.000000 bnlearn-0.8.7/bnlearn/__init__.py
--rw-rw-rw-   0        0        0    72952 2024-04-12 20:42:15.000000 bnlearn-0.8.7/bnlearn/bnlearn.py
--rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/confmatrix.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.745638 bnlearn-0.8.7/bnlearn/data/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/data/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.763303 bnlearn-0.8.7/bnlearn/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/discretize/__init__.py
--rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.7/bnlearn/discretize/discretize.py
--rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.7/bnlearn/discretize/learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    53337 2024-04-12 20:21:18.000000 bnlearn-0.8.7/bnlearn/examples.py
--rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/examples_discretize.py
--rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/inference.py
--rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/network.py
--rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/parameter_learning.py
--rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.7/bnlearn/structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.763303 bnlearn-0.8.7/bnlearn/tests/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.777326 bnlearn-0.8.7/bnlearn/tests/discretize/
--rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/__init__.py
--rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/test_discretize.py
--rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
--rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.7/bnlearn/tests/test_bnlearn.py
--rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.7/bnlearn/tests/test_structure_learning.py
-drwxrwxrwx   0        0        0        0 2024-04-12 20:57:24.745638 bnlearn-0.8.7/bnlearn.egg-info/
--rw-rw-rw-   0        0        0    12768 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      776 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      204 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-12 20:57:24.000000 bnlearn-0.8.7/bnlearn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-12 20:57:24.777326 bnlearn-0.8.7/setup.cfg
--rw-rw-rw-   0        0        0     2088 2024-04-09 19:29:59.000000 bnlearn-0.8.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.905151 bnlearn-0.8.8/
+-rw-rw-rw-   0        0        0     1231 2023-10-22 19:58:12.000000 bnlearn-0.8.8/LICENSE
+-rw-rw-rw-   0        0        0      643 2023-10-22 19:58:12.000000 bnlearn-0.8.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    12276 2024-05-22 16:02:22.905151 bnlearn-0.8.8/PKG-INFO
+-rw-rw-rw-   0        0        0    11670 2023-10-22 19:58:12.000000 bnlearn-0.8.8/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.873151 bnlearn-0.8.8/bnlearn/
+-rw-rw-rw-   0        0        0     4735 2024-05-22 15:52:06.000000 bnlearn-0.8.8/bnlearn/__init__.py
+-rw-rw-rw-   0        0        0    72952 2024-04-12 20:42:15.000000 bnlearn-0.8.8/bnlearn/bnlearn.py
+-rw-rw-rw-   0        0        0     1745 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/confmatrix.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.891371 bnlearn-0.8.8/bnlearn/data/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/data/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.905151 bnlearn-0.8.8/bnlearn/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/discretize/__init__.py
+-rw-rw-rw-   0        0        0     3935 2023-11-15 21:42:47.000000 bnlearn-0.8.8/bnlearn/discretize/discretize.py
+-rw-rw-rw-   0        0        0    19245 2023-11-10 19:55:44.000000 bnlearn-0.8.8/bnlearn/discretize/learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    53521 2024-04-13 07:42:32.000000 bnlearn-0.8.8/bnlearn/examples.py
+-rw-rw-rw-   0        0        0     1330 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/examples_discretize.py
+-rw-rw-rw-   0        0        0     4847 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/inference.py
+-rw-rw-rw-   0        0        0    16904 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/network.py
+-rw-rw-rw-   0        0        0     7419 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/parameter_learning.py
+-rw-rw-rw-   0        0        0    27065 2023-11-11 20:55:02.000000 bnlearn-0.8.8/bnlearn/structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.905151 bnlearn-0.8.8/bnlearn/tests/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.905151 bnlearn-0.8.8/bnlearn/tests/discretize/
+-rw-rw-rw-   0        0        0        0 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/tests/discretize/__init__.py
+-rw-rw-rw-   0        0        0     2293 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/tests/discretize/test_discretize.py
+-rw-rw-rw-   0        0        0     9366 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py
+-rw-rw-rw-   0        0        0    13368 2023-11-10 22:07:11.000000 bnlearn-0.8.8/bnlearn/tests/test_bnlearn.py
+-rw-rw-rw-   0        0        0     8222 2023-10-22 19:58:12.000000 bnlearn-0.8.8/bnlearn/tests/test_structure_learning.py
+drwxrwxrwx   0        0        0        0 2024-05-22 16:02:22.891371 bnlearn-0.8.8/bnlearn.egg-info/
+-rw-rw-rw-   0        0        0    12276 2024-05-22 16:02:22.000000 bnlearn-0.8.8/bnlearn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      776 2024-05-22 16:02:22.000000 bnlearn-0.8.8/bnlearn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 16:02:22.000000 bnlearn-0.8.8/bnlearn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      197 2024-05-22 16:02:22.000000 bnlearn-0.8.8/bnlearn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-22 16:02:22.000000 bnlearn-0.8.8/bnlearn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 16:02:22.905151 bnlearn-0.8.8/setup.cfg
+-rw-rw-rw-   0        0        0     2081 2024-05-22 15:47:39.000000 bnlearn-0.8.8/setup.py
```

### Comparing `bnlearn-0.8.7/LICENSE` & `bnlearn-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/MANIFEST.in` & `bnlearn-0.8.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/PKG-INFO` & `bnlearn-0.8.8/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,7 @@
-Metadata-Version: 2.1
-Name: bnlearn
-Version: 0.8.7
-Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
-Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz
-Author: Erdogan Taskesen
-Author-email: erdogant@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pgmpy>=0.1.18
-Requires-Dist: networkx>=2.7.1
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas==1.5.3
-Requires-Dist: tqdm
-Requires-Dist: ismember
-Requires-Dist: scikit-learn
-Requires-Dist: funcsigs
-Requires-Dist: statsmodels
-Requires-Dist: python-louvain
-Requires-Dist: packaging
-Requires-Dist: df2onehot
-Requires-Dist: fsspec
-Requires-Dist: pypickle
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: datazets
-
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,31 +1,17 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.7 Summary: Python package for
-learning the graphical structure of Bayesian networks, parameter learning,
-inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz Author:
-Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist: tqdm
-Requires-Dist: ismember Requires-Dist: scikit-learn Requires-Dist: funcsigs
-Requires-Dist: statsmodels Requires-Dist: python-louvain Requires-Dist:
-packaging Requires-Dist: df2onehot Requires-Dist: fsspec Requires-Dist:
-pypickle Requires-Dist: tabulate Requires-Dist: ipywidgets Requires-Dist:
-datazets # bnlearn - Library for Bayesian network learning and inference [!
-[Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
-img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
-Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
-(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
-forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
-[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
-(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+# bnlearn - Library for Bayesian network learning and inference [![Python]
+(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.7/README.md` & `bnlearn-0.8.8/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: bnlearn
+Version: 0.8.8
+Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
+Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.8.tar.gz
+Author: Erdogan Taskesen
+Author-email: erdogant@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
 [![Forks](https://img.shields.io/github/forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network)
```

#### html2text {}

```diff
@@ -1,9 +1,17 @@
-# bnlearn - Library for Bayesian network learning and inference [![Python]
-(https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.8 Summary: Python package for
+learning the graphical structure of Bayesian networks, parameter learning,
+inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.8.tar.gz Author:
+Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent Requires-Python: >=3
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
 pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
 (https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
 img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
 img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
 bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
 erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
 Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
```

### Comparing `bnlearn-0.8.7/bnlearn/__init__.py` & `bnlearn-0.8.8/bnlearn/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 import bnlearn.network as network
 import bnlearn.confmatrix as confmatrix
 from bnlearn.discretize.discretize import discretize, discretize_value
 from packaging import version
 
 __author__ = 'Erdogan Tasksen'
 __email__ = 'erdogant@gmail.com'
-__version__ = '0.8.7'
+__version__ = '0.8.8'
 
 import pgmpy
 # Check version pgmpy
 if version.parse(pgmpy.__version__) < version.parse("0.1.18"):
     raise ImportError('[bnlearn] >Error: This release requires pgmpy to be version >= 0.1.18. Try to: <pip install -U pgmpy>=0.1.18>')
 
 # Version check
@@ -54,17 +54,17 @@
 if version.parse(nx.__version__) < version.parse("2.7.1"):
     raise ImportError('[bnlearn] >Error: networkx version should be > 2.7.1\nTry to: pip install -U networkx')
 
 import numpy as np
 if version.parse(np.__version__) < version.parse("1.24.1"):
     raise ImportError('[bnlearn] >Error: numpy version should be > 1.24.1\nTry to: pip install -U numpy')
 
-import pandas as pd
-if version.parse(pd.__version__) > version.parse("1.5.3"):
-    raise ImportError('[bnlearn] >Error: pands version should be <= 1.5.3')
+# import pandas as pd
+# if version.parse(pd.__version__) > version.parse("1.5.3"):
+#     raise ImportError('[bnlearn] >Error: pands version should be <= 1.5.3')
 
 # This one is moved towards the interactive plot function because it is not required in the setup.
 # import d3blocks as d3
 # if version.parse(d3.__version__) < version.parse("1.4.9"):
 #     raise ImportError('[bnlearn] >Error: d3blocks version should be >= 1.4.9')
 
 # module level doc-string
```

### Comparing `bnlearn-0.8.7/bnlearn/bnlearn.py` & `bnlearn-0.8.8/bnlearn/bnlearn.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/confmatrix.py` & `bnlearn-0.8.8/bnlearn/confmatrix.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/discretize/discretize.py` & `bnlearn-0.8.8/bnlearn/discretize/discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/discretize/learn_discrete_bayes_net.py` & `bnlearn-0.8.8/bnlearn/discretize/learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/examples.py` & `bnlearn-0.8.8/bnlearn/examples.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,21 +34,24 @@
 # print(df)
 
 # Structure learning
 model = bn.structure_learning.fit(df, verbose=0, scoretype='bic', methodtype='hc')
 model = bn.structure_learning.fit(df, verbose=0, scoretype='k2', methodtype='hc')
 
 # Plot the DAG
+DAG = bn.plot(model, verbose=0, interactive=False)
 bn.plot(model, verbose=0, interactive=True, node_color='#000000')
 
 # Test for independence
 model = bn.independence_test(model, df, prune=False)
 
 # Plot the DAG
+bn.plot(model, verbose=0, interactive=False, pos=DAG['pos'])
 bn.plot(model, verbose=0, interactive=True, node_color='#000000')
+
 # Print the CPDs
 bn.print_CPD(model)
 # Comparison
 
 # Learn its parameters from data and perform the inference.
 model_with_CPD = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
 model = bn.parameter_learning.fit(model, df, methodtype='bayes', verbose=0)
@@ -100,19 +103,25 @@
 # Constrained based
 # DAG = bn.structure_learning.fit(df, methodtype='cs')
 
 # Set class node (endpoint)
 df = df.dropna()
 DAG = bn.structure_learning.fit(df, methodtype='tan', class_node='threat_type')
 
+# Plot
+G = bn.plot(DAG)
+G = bn.plot(DAG, interactive=True)
+
 # Structure learning
 DAG = bn.independence_test(DAG, df, prune=True)
+
 # Plot
 G = bn.plot(DAG)
 G = bn.plot(DAG, interactive=True)
+
 # Parameter learning
 model = bn.parameter_learning.fit(DAG, df)
 # Make inference
 q1 = bn.inference.fit(model, variables=['threat_type'], evidence={'flee_status': 'foot'})
 q1 = bn.inference.fit(model, variables=['gender'], evidence={'threat_type': 'accident', 'armed_with': 'gun'})
 
 # No connection in the DAG, thus the evidence should not influence the outcome
```

### Comparing `bnlearn-0.8.7/bnlearn/examples_discretize.py` & `bnlearn-0.8.8/bnlearn/examples_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/inference.py` & `bnlearn-0.8.8/bnlearn/inference.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/network.py` & `bnlearn-0.8.8/bnlearn/network.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/parameter_learning.py` & `bnlearn-0.8.8/bnlearn/parameter_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/structure_learning.py` & `bnlearn-0.8.8/bnlearn/structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/tests/discretize/test_discretize.py` & `bnlearn-0.8.8/bnlearn/tests/discretize/test_discretize.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py` & `bnlearn-0.8.8/bnlearn/tests/discretize/test_learn_discrete_bayes_net.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/tests/test_bnlearn.py` & `bnlearn-0.8.8/bnlearn/tests/test_bnlearn.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn/tests/test_structure_learning.py` & `bnlearn-0.8.8/bnlearn/tests/test_structure_learning.py`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/bnlearn.egg-info/PKG-INFO` & `bnlearn-0.8.8/bnlearn.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,21 @@
 Metadata-Version: 2.1
 Name: bnlearn
-Version: 0.8.7
+Version: 0.8.8
 Summary: Python package for learning the graphical structure of Bayesian networks, parameter learning, inference and sampling methods.
 Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.8.tar.gz
 Author: Erdogan Taskesen
 Author-email: erdogant@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pgmpy>=0.1.18
-Requires-Dist: networkx>=2.7.1
-Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1
-Requires-Dist: pandas==1.5.3
-Requires-Dist: tqdm
-Requires-Dist: ismember
-Requires-Dist: scikit-learn
-Requires-Dist: funcsigs
-Requires-Dist: statsmodels
-Requires-Dist: python-louvain
-Requires-Dist: packaging
-Requires-Dist: df2onehot
-Requires-Dist: fsspec
-Requires-Dist: pypickle
-Requires-Dist: tabulate
-Requires-Dist: ipywidgets
-Requires-Dist: datazets
 
 # bnlearn - Library for Bayesian network learning and inference
 
 [![Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/pyversions/bnlearn)
 [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/)
 ![GitHub Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn)
 [![License](https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/bnlearn/blob/master/LICENSE)
```

#### html2text {}

```diff
@@ -1,31 +1,25 @@
-Metadata-Version: 2.1 Name: bnlearn Version: 0.8.7 Summary: Python package for
+Metadata-Version: 2.1 Name: bnlearn Version: 0.8.8 Summary: Python package for
 learning the graphical structure of Bayesian networks, parameter learning,
 inference and sampling methods. Home-page: https://erdogant.github.io/bnlearn
-Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.7.tar.gz Author:
+Download-URL: https://github.com/erdogant/bnlearn/archive/0.8.8.tar.gz Author:
 Erdogan Taskesen Author-email: erdogant@gmail.com Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent Requires-Python: >=3
-Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
-pgmpy>=0.1.18 Requires-Dist: networkx>=2.7.1 Requires-Dist: matplotlib>=3.3.4
-Requires-Dist: numpy>=1.24.1 Requires-Dist: pandas==1.5.3 Requires-Dist: tqdm
-Requires-Dist: ismember Requires-Dist: scikit-learn Requires-Dist: funcsigs
-Requires-Dist: statsmodels Requires-Dist: python-louvain Requires-Dist:
-packaging Requires-Dist: df2onehot Requires-Dist: fsspec Requires-Dist:
-pypickle Requires-Dist: tabulate Requires-Dist: ipywidgets Requires-Dist:
-datazets # bnlearn - Library for Bayesian network learning and inference [!
-[Python](https://img.shields.io/pypi/pyversions/bnlearn)](https://
-img.shields.io/pypi/pyversions/bnlearn) [![PyPI Version](https://
-img.shields.io/pypi/v/bnlearn)](https://pypi.org/project/bnlearn/) ![GitHub
-Repo stars](https://img.shields.io/github/stars/erdogant/bnlearn) [![License]
-(https://img.shields.io/badge/license-MIT-green.svg)](https://github.com/
-erdogant/bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/
-forks/erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [!
-[Open Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)]
-(https://github.com/erdogant/bnlearn/issues) [![Project Status](http://
+Description-Content-Type: text/markdown License-File: LICENSE # bnlearn -
+Library for Bayesian network learning and inference [![Python](https://
+img.shields.io/pypi/pyversions/bnlearn)](https://img.shields.io/pypi/
+pyversions/bnlearn) [![PyPI Version](https://img.shields.io/pypi/v/bnlearn)]
+(https://pypi.org/project/bnlearn/) ![GitHub Repo stars](https://
+img.shields.io/github/stars/erdogant/bnlearn) [![License](https://
+img.shields.io/badge/license-MIT-green.svg)](https://github.com/erdogant/
+bnlearn/blob/master/LICENSE) [![Forks](https://img.shields.io/github/forks/
+erdogant/bnlearn.svg)](https://github.com/erdogant/bnlearn/network) [![Open
+Issues](https://img.shields.io/github/issues/erdogant/bnlearn.svg)](https://
+github.com/erdogant/bnlearn/issues) [![Project Status](http://
 www.repostatus.org/badges/latest/active.svg)](http://www.repostatus.org/
 #active) [![Downloads](https://pepy.tech/badge/bnlearn/month)](https://
 pepy.tech/project/bnlearn/) [![Downloads](https://pepy.tech/badge/bnlearn)]
 (https://pepy.tech/project/bnlearn) [![DOI](https://zenodo.org/badge/
 231263493.svg)](https://zenodo.org/badge/latestdoi/231263493) [![Docs](https://
 img.shields.io/badge/Sphinx-Docs-Green)](https://erdogant.github.io/bnlearn/)
 [![Medium](https://img.shields.io/badge/Medium-Blog-black)](https://
```

### Comparing `bnlearn-0.8.7/bnlearn.egg-info/SOURCES.txt` & `bnlearn-0.8.8/bnlearn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bnlearn-0.8.7/setup.py` & `bnlearn-0.8.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 with open("README.md", "r", encoding='utf8') as fh:
     long_description = fh.read()
 setuptools.setup(
      install_requires=["pgmpy>=0.1.18",
                        "networkx>=2.7.1",
                        "matplotlib>=3.3.4",
                        "numpy>=1.24.1",
-                       'pandas==1.5.3',
+                       'pandas',
                        'tqdm',
                        'ismember',
                        'scikit-learn',
                        'funcsigs',
                        'statsmodels',
                        'python-louvain',
                        'packaging',
```

