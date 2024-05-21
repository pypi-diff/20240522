# Comparing `tmp/positional_vectorizer-0.0.7.tar.gz` & `tmp/positional_vectorizer-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "positional_vectorizer-0.0.7.tar", last modified: Wed May  1 23:27:37 2024, max compression
+gzip compressed data, was "positional_vectorizer-0.0.9.tar", last modified: Tue May 21 23:41:20 2024, max compression
```

## Comparing `positional_vectorizer-0.0.7.tar` & `positional_vectorizer-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.724475 positional_vectorizer-0.0.7/.mypy_cache/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.724475 positional_vectorizer-0.0.7/.mypy_cache/3.11/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/.mypy_cache/3.11/positional_vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)    13140 2024-05-01 23:27:33.000000 positional_vectorizer-0.0.7/.mypy_cache/3.11/positional_vectorizer/__init__.data.json
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-05-01 23:27:33.000000 positional_vectorizer-0.0.7/.mypy_cache/3.11/positional_vectorizer/__init__.meta.json
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-01 23:27:36.000000 positional_vectorizer-0.0.7/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/positional_vectorizer/
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/positional_vectorizer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/positional_vectorizer/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (127)     6009 2024-05-01 23:27:34.000000 positional_vectorizer-0.0.7/positional_vectorizer/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-01 23:27:37.000000 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-01 23:27:37.000000 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-01 23:27:37.000000 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-01 23:27:37.000000 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-01 23:27:37.000000 positional_vectorizer-0.0.7/positional_vectorizer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-01 23:27:37.728476 positional_vectorizer-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-01 23:27:18.000000 positional_vectorizer-0.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:41:20.254705 positional_vectorizer-0.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-21 23:41:20.254705 positional_vectorizer-0.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-21 23:41:18.000000 positional_vectorizer-0.0.9/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:41:20.254705 positional_vectorizer-0.0.9/positional_vectorizer/
+-rw-r--r--   0 runner    (1001) docker     (127)     4466 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/positional_vectorizer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-21 23:41:20.254705 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2024-05-21 23:41:20.000000 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-21 23:41:20.000000 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-21 23:41:20.000000 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-21 23:41:20.000000 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-21 23:41:20.000000 positional_vectorizer-0.0.9/positional_vectorizer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-21 23:41:20.254705 positional_vectorizer-0.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-05-21 23:41:03.000000 positional_vectorizer-0.0.9/setup.py
```

### Comparing `positional_vectorizer-0.0.7/LICENSE` & `positional_vectorizer-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.7/PKG-INFO` & `positional_vectorizer-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.7
+Version: 0.0.9
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
-Requires-Python: >=3.11, <3.12
+Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: typing-extensions>=4.11.0
 
 # Positional Vectorizer
 
 The Positional Vectorizer is a transformer in scikit-learn designed to transform text into a bag of words vector using a positional ranking algorithm to assign scores. Similar to scikit-learn's CountVectorizer and TFIDFVectorizer, it assigns a value to each dimension based on the term's position in the original text.
 
 ## How to use
```

### Comparing `positional_vectorizer-0.0.7/README.md` & `positional_vectorizer-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `positional_vectorizer-0.0.7/positional_vectorizer/__init__.py` & `positional_vectorizer-0.0.9/positional_vectorizer/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 from sklearn.feature_extraction.text import _VectorizerMixin
 from sklearn.base import BaseEstimator
-from typing import Self, List
+from typing import List
 from scipy.sparse._csr import csr_matrix
 import math
 
+# Python 3.10 has no Self on typing module
+try:
+    from typing import Self  # type: ignore[attr-defined]
+except Exception:
+    from typing_extensions import Self
+
 
 class PositionalVectorizer(_VectorizerMixin, BaseEstimator):
 
     def __init__(
         self,
         *,
         input="content",
```

### Comparing `positional_vectorizer-0.0.7/positional_vectorizer.egg-info/PKG-INFO` & `positional_vectorizer-0.0.9/positional_vectorizer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: positional-vectorizer
-Version: 0.0.7
+Version: 0.0.9
 Summary: Positional Vectorizer is a scikit-learn transformer that converts text to bag of words vector using a positional ranking algorithm as score
 Home-page: https://github.com/timotta/positional-vectorizer
 Author: Tiago Albineli Motta
 Author-email: timotta@gmail.com
 License: new BSD
 Keywords: machine learning,embedding,vectorizer,scikit-learn,text,NLP
-Requires-Python: >=3.11, <3.12
+Requires-Python: >=3.10, <3.12
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: scikit-learn>=1.4.2
+Requires-Dist: typing-extensions>=4.11.0
 
 # Positional Vectorizer
 
 The Positional Vectorizer is a transformer in scikit-learn designed to transform text into a bag of words vector using a positional ranking algorithm to assign scores. Similar to scikit-learn's CountVectorizer and TFIDFVectorizer, it assigns a value to each dimension based on the term's position in the original text.
 
 ## How to use
```

### Comparing `positional_vectorizer-0.0.7/setup.py` & `positional_vectorizer-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,10 +31,10 @@
     include_package_data=True,
     keywords="machine learning, embedding, vectorizer, scikit-learn, text, NLP",
     entry_points={
         "console_scripts": [
             # '',
         ],
     },
-    python_requires=">=3.11, <3.12",
+    python_requires=">=3.10, <3.12",
     install_requires=requirements,
 )
```

