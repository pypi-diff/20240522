# Comparing `tmp/ivers-0.1.tar.gz` & `tmp/ivers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ivers-0.1.tar", last modified: Sat May 18 21:08:19 2024, max compression
+gzip compressed data, was "ivers-0.1.1.tar", last modified: Wed May 22 12:56:15 2024, max compression
```

## Comparing `ivers-0.1.tar` & `ivers-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 21:08:19.494409 ivers-0.1/
--rw-rw-rw-   0        0        0     1098 2024-05-18 21:00:40.000000 ivers-0.1/LICENSE
--rw-rw-rw-   0        0        0      121 2024-05-18 21:07:31.000000 ivers-0.1/MANIFEST.in
--rw-rw-rw-   0        0        0     3057 2024-05-18 21:08:19.490355 ivers-0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2287 2024-05-18 21:00:40.000000 ivers-0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 21:08:19.384020 ivers-0.1/ivers/
--rw-rw-rw-   0        0        0       99 2024-05-18 21:07:46.000000 ivers-0.1/ivers/__init__.py
--rw-rw-rw-   0        0        0     4355 2024-05-18 21:00:40.000000 ivers-0.1/ivers/allforfree.py
--rw-rw-rw-   0        0        0     4130 2024-05-18 21:00:40.000000 ivers-0.1/ivers/leaky.py
--rw-rw-rw-   0        0        0     5726 2024-05-18 21:00:40.000000 ivers-0.1/ivers/stratify.py
--rw-rw-rw-   0        0        0     7245 2024-05-18 21:00:40.000000 ivers-0.1/ivers/temporal.py
-drwxrwxrwx   0        0        0        0 2024-05-18 21:08:19.470236 ivers-0.1/ivers.egg-info/
--rw-rw-rw-   0        0        0     3057 2024-05-18 21:08:17.000000 ivers-0.1/ivers.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2024-05-18 21:08:18.000000 ivers-0.1/ivers.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 21:08:17.000000 ivers-0.1/ivers.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       20 2024-05-18 21:08:17.000000 ivers-0.1/ivers.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-18 21:08:17.000000 ivers-0.1/ivers.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       64 2024-05-18 21:00:40.000000 ivers-0.1/requirements.txt
--rw-rw-rw-   0        0        0       42 2024-05-18 21:08:19.495415 ivers-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1042 2024-05-18 21:00:40.000000 ivers-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-18 21:08:19.484340 ivers-0.1/test/
--rw-rw-rw-   0        0        0        0 2024-05-18 21:00:40.000000 ivers-0.1/test/__init__.py
--rw-rw-rw-   0        0        0     3199 2024-05-18 21:00:40.000000 ivers-0.1/test/test_stratify.py
--rw-rw-rw-   0        0        0     2230 2024-05-18 21:00:40.000000 ivers-0.1/test/test_temporal_allforfree.py
--rw-rw-rw-   0        0        0     2304 2024-05-18 21:00:40.000000 ivers-0.1/test/test_temporal_leaky.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:56:15.914054 ivers-0.1.1/
+-rw-rw-rw-   0        0        0     1098 2024-05-22 10:51:31.000000 ivers-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      164 2024-05-22 12:52:25.000000 ivers-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     3309 2024-05-22 12:56:15.911210 ivers-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     2174 2024-05-22 10:51:31.000000 ivers-0.1.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 12:56:15.860966 ivers-0.1.1/ivers/
+-rw-rw-rw-   0        0        0       50 2024-05-22 12:32:02.000000 ivers-0.1.1/ivers/__init__.py
+-rw-rw-rw-   0        0        0    12622 2024-05-22 10:54:34.000000 ivers-0.1.1/ivers/stratify.py
+-rw-rw-rw-   0        0        0     9329 2024-05-22 12:41:19.000000 ivers-0.1.1/ivers/temporal.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:56:15.910122 ivers-0.1.1/ivers.egg-info/
+-rw-rw-rw-   0        0        0     3309 2024-05-22 12:56:15.000000 ivers-0.1.1/ivers.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      378 2024-05-22 12:56:15.000000 ivers-0.1.1/ivers.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 12:56:15.000000 ivers-0.1.1/ivers.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2024-05-22 12:56:15.000000 ivers-0.1.1/ivers.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-22 12:56:15.000000 ivers-0.1.1/ivers.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       64 2024-05-22 10:51:31.000000 ivers-0.1.1/requirements.txt
+-rw-rw-rw-   0        0        0       42 2024-05-22 12:56:15.914563 ivers-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1401 2024-05-22 12:52:44.000000 ivers-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 12:56:15.908714 ivers-0.1.1/test/
+-rw-rw-rw-   0        0        0        0 2024-05-22 10:51:31.000000 ivers-0.1.1/test/__init__.py
+-rw-rw-rw-   0        0        0     3199 2024-05-22 10:51:31.000000 ivers-0.1.1/test/test_stratify.py
+-rw-rw-rw-   0        0        0     3022 2024-05-22 10:51:31.000000 ivers-0.1.1/test/test_stratify_cv.py
+-rw-rw-rw-   0        0        0     2230 2024-05-22 10:51:31.000000 ivers-0.1.1/test/test_temporal_allforfree.py
+-rw-rw-rw-   0        0        0     3887 2024-05-22 10:54:04.000000 ivers-0.1.1/test/test_temporal_leaky.py
```

### Comparing `ivers-0.1/LICENSE` & `ivers-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ivers-0.1/PKG-INFO` & `ivers-0.1.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 Metadata-Version: 2.1
 Name: ivers
-Version: 0.1
-Summary: Python package to stratify split datasets based on endpoint distributions
+Version: 0.1.1
+Summary: Python package to stratify split datasets based on endpoint distributions, also 2 different temporal splits. Chemprop compatible.
 Home-page: http://github.com/iversohlsson/ivers
 Author: Philip Ivers Ohlsson
 Author-email: philip.iversohlsson@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Documentation, http://github.com/iversohlsson/ivers/docs/_build/html/index.html
+Project-URL: Source, http://github.com/iversohlsson/ivers
+Keywords: chemprop chemistry data science dataset splitting stratification temporal splits ivers
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # Ivers
 
-This project provides a robust library for managing data splits in machine learning projects with a focus on maintaining balanced distributions across various conditions. It is specifically designed to interface seamlessly with the Chemprop library, enhancing its capabilities for chemical property prediction.
 
-## Features
+This project offers tools for managing data splits, ensuring endpoint distributions are maintained, and presents two novel temporal split techniques: 'leaky' and 'all for free' splits. See the explanation below. 
+
+**Note**: This library was used in this paper [PlaceHolder](https://github.com/IversOhlsson/ivers) to generate data splits for the Chemprop library.
 
-- **Temporal Splits**: Supports two types of temporal data splits:
-  - **Leaky**: Allows for forward-leakage in your data to simulate real-world scenarios where future data might influence the model subtly.
-  - **AllForFree**: Provides a stricter temporal separation, ensuring that the training data is entirely independent of the test set, suitable for rigorous testing of model predictions over time.
-
-- **Num Fold Split**: Implements a novel approach to increasing the training set size successively across multiple folds. This feature allows for progressive training, where each subsequent fold includes the data from all previous folds, enhancing model robustness.
-
-- **Stratified Endpoint Split**: 
-  - **Main Feature**: Our library introduces a stratified endpoint split, crucial for maintaining a consistent distribution of data across different categories or endpoints in your datasets.
-  - **Utility**: Especially useful in scenarios where endpoint distributions are critical, such as in cheminformatics and bioinformatics.
+## Features
+  - **Temporal Leaky**: Allows for forward-leakage in your data to simulate real-world scenarios where future data might influence the model subtly.
+  - **Temporal AllForFree**: Provides a stricter temporal separation, ensuring that the training data is entirely independent of the test set, suitable for rigorous testing of model predictions over time.
+  - **Temporal Fold Split**: Implements a novel approach to increasing the training set size successively across multiple folds based on the temporal time sequence
+  - **Stratified Endpoint Split**: Our library introduces a stratified endpoint split, crucial for maintaining a consistent distribution of data across different categories or endpoints in your datasets. Especially useful in scenarios where endpoint distributions are critical, such as in cheminformatics and bioinformatics.
   - **Cross-Validation Support**: Integrates capabilities to ensure that each cross-validation split maintains endpoint distribution, ideal for developing models that are generalizable across varied data conditions.
 
 ## Integration with Chemprop
 
-- **Seamless Compatibility**: Designed to be used in conjunction with the Chemprop library, this feature allows users to leverage our data splitting strategies directly within their Chemprop workflows.
-- **Enhanced Data Handling**: By integrating our splitting mechanisms, users can ensure that their chemical property prediction models are trained on well-structured and strategically partitioned datasets.
+- By setting the `chemprop` variable to `true`, the library will generate splits compatible with the Chemprop library. This ensures that the features and train-test splits are generated in a way that can easily be used with Chemprop.
 
-## Getting Started
+## Getting Started or Contributing
 
 To get started with this library, clone the repository and install the required dependencies:
 
 ```bash
-git clone https://github.com/yourrepository/projectname.git
-cd projectname
+git clone https://github.com/IversOhlsson/ivers.git
+cd ivers
 pip install -r requirements.txt
 ```
+
+## Installation via pip
+You can also install the package via pip:
+```bash
+pip install ivers
+```
+We welcome contributions! Feel free to open issues or pull requests on our GitHub repository.
+
```

### Comparing `ivers-0.1/ivers.egg-info/PKG-INFO` & `ivers-0.1.1/ivers.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,50 +1,59 @@
 Metadata-Version: 2.1
 Name: ivers
-Version: 0.1
-Summary: Python package to stratify split datasets based on endpoint distributions
+Version: 0.1.1
+Summary: Python package to stratify split datasets based on endpoint distributions, also 2 different temporal splits. Chemprop compatible.
 Home-page: http://github.com/iversohlsson/ivers
 Author: Philip Ivers Ohlsson
 Author-email: philip.iversohlsson@gmail.com
-Classifier: Development Status :: 3 - Alpha
+Project-URL: Documentation, http://github.com/iversohlsson/ivers/docs/_build/html/index.html
+Project-URL: Source, http://github.com/iversohlsson/ivers
+Keywords: chemprop chemistry data science dataset splitting stratification temporal splits ivers
 Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: scikit-learn
 
 # Ivers
 
-This project provides a robust library for managing data splits in machine learning projects with a focus on maintaining balanced distributions across various conditions. It is specifically designed to interface seamlessly with the Chemprop library, enhancing its capabilities for chemical property prediction.
 
-## Features
+This project offers tools for managing data splits, ensuring endpoint distributions are maintained, and presents two novel temporal split techniques: 'leaky' and 'all for free' splits. See the explanation below. 
+
+**Note**: This library was used in this paper [PlaceHolder](https://github.com/IversOhlsson/ivers) to generate data splits for the Chemprop library.
 
-- **Temporal Splits**: Supports two types of temporal data splits:
-  - **Leaky**: Allows for forward-leakage in your data to simulate real-world scenarios where future data might influence the model subtly.
-  - **AllForFree**: Provides a stricter temporal separation, ensuring that the training data is entirely independent of the test set, suitable for rigorous testing of model predictions over time.
-
-- **Num Fold Split**: Implements a novel approach to increasing the training set size successively across multiple folds. This feature allows for progressive training, where each subsequent fold includes the data from all previous folds, enhancing model robustness.
-
-- **Stratified Endpoint Split**: 
-  - **Main Feature**: Our library introduces a stratified endpoint split, crucial for maintaining a consistent distribution of data across different categories or endpoints in your datasets.
-  - **Utility**: Especially useful in scenarios where endpoint distributions are critical, such as in cheminformatics and bioinformatics.
+## Features
+  - **Temporal Leaky**: Allows for forward-leakage in your data to simulate real-world scenarios where future data might influence the model subtly.
+  - **Temporal AllForFree**: Provides a stricter temporal separation, ensuring that the training data is entirely independent of the test set, suitable for rigorous testing of model predictions over time.
+  - **Temporal Fold Split**: Implements a novel approach to increasing the training set size successively across multiple folds based on the temporal time sequence
+  - **Stratified Endpoint Split**: Our library introduces a stratified endpoint split, crucial for maintaining a consistent distribution of data across different categories or endpoints in your datasets. Especially useful in scenarios where endpoint distributions are critical, such as in cheminformatics and bioinformatics.
   - **Cross-Validation Support**: Integrates capabilities to ensure that each cross-validation split maintains endpoint distribution, ideal for developing models that are generalizable across varied data conditions.
 
 ## Integration with Chemprop
 
-- **Seamless Compatibility**: Designed to be used in conjunction with the Chemprop library, this feature allows users to leverage our data splitting strategies directly within their Chemprop workflows.
-- **Enhanced Data Handling**: By integrating our splitting mechanisms, users can ensure that their chemical property prediction models are trained on well-structured and strategically partitioned datasets.
+- By setting the `chemprop` variable to `true`, the library will generate splits compatible with the Chemprop library. This ensures that the features and train-test splits are generated in a way that can easily be used with Chemprop.
 
-## Getting Started
+## Getting Started or Contributing
 
 To get started with this library, clone the repository and install the required dependencies:
 
 ```bash
-git clone https://github.com/yourrepository/projectname.git
-cd projectname
+git clone https://github.com/IversOhlsson/ivers.git
+cd ivers
 pip install -r requirements.txt
 ```
+
+## Installation via pip
+You can also install the package via pip:
+```bash
+pip install ivers
+```
+We welcome contributions! Feel free to open issues or pull requests on our GitHub repository.
+
```

### Comparing `ivers-0.1/setup.py` & `ivers-0.1.1/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ivers',
-    version='0.1',
+    version='0.1.1',
     packages=find_packages(),
-    description='Python package to stratify split datasets based on endpoint distributions',
+    description='Python package to stratify split datasets based on endpoint distributions, also 2 different temporal splits. Chemprop compatible.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     author='Philip Ivers Ohlsson',
     author_email='philip.iversohlsson@gmail.com',
     url='http://github.com/iversohlsson/ivers',
     install_requires=[
         'pandas',
         'scikit-learn'
     ],
     classifiers=[
-        'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
+                'Intended Audience :: Science/Research',
+
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
+    keywords='chemprop chemistry data science dataset splitting stratification temporal splits ivers',
+    project_urls={
+        'Documentation': 'http://github.com/iversohlsson/ivers/docs/_build/html/index.html',
+        'Source': 'http://github.com/iversohlsson/ivers',
+    },
 )
 from setuptools import setup, find_packages
```

### Comparing `ivers-0.1/test/test_stratify.py` & `ivers-0.1.1/test/test_stratify.py`

 * *Files identical despite different names*

### Comparing `ivers-0.1/test/test_temporal_allforfree.py` & `ivers-0.1.1/test/test_temporal_allforfree.py`

 * *Files identical despite different names*

