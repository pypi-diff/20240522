# Comparing `tmp/pixmclass-0.1.1.tar.gz` & `tmp/pixmclass-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pixmclass-0.1.1.tar", last modified: Thu May 16 15:32:30 2024, max compression
+gzip compressed data, was "pixmclass-0.1.2.tar", last modified: Wed May 22 20:39:22 2024, max compression
```

## Comparing `pixmclass-0.1.1.tar` & `pixmclass-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.429533 pixmclass-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-16 15:32:25.000000 pixmclass-0.1.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-16 15:32:30.425533 pixmclass-0.1.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.425533 pixmclass-0.1.1/PixMClass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-16 15:32:30.000000 pixmclass-0.1.1/PixMClass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 15:32:25.000000 pixmclass-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:32:30.425533 pixmclass-0.1.1/pix_mclass/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/callbacks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/training.py
--rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/unet.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-16 15:32:25.000000 pixmclass-0.1.1/pix_mclass/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:32:30.429533 pixmclass-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-16 15:32:25.000000 pixmclass-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:39:22.469031 pixmclass-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-05-22 20:39:19.000000 pixmclass-0.1.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-22 20:39:22.469031 pixmclass-0.1.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:39:22.469031 pixmclass-0.1.2/PixMClass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1559 2024-05-22 20:39:22.000000 pixmclass-0.1.2/PixMClass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      300 2024-05-22 20:39:22.000000 pixmclass-0.1.2/PixMClass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 20:39:22.000000 pixmclass-0.1.2/PixMClass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-22 20:39:22.000000 pixmclass-0.1.2/PixMClass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-22 20:39:22.000000 pixmclass-0.1.2/PixMClass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-22 20:39:19.000000 pixmclass-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 20:39:22.469031 pixmclass-0.1.2/pix_mclass/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-05-22 20:39:19.000000 pixmclass-0.1.2/pix_mclass/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2513 2024-05-22 20:39:19.000000 pixmclass-0.1.2/pix_mclass/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2024-05-22 20:39:19.000000 pixmclass-0.1.2/pix_mclass/training.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4483 2024-05-22 20:39:19.000000 pixmclass-0.1.2/pix_mclass/unet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-22 20:39:19.000000 pixmclass-0.1.2/pix_mclass/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 20:39:22.469031 pixmclass-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-05-22 20:39:19.000000 pixmclass-0.1.2/setup.py
```

### Comparing `pixmclass-0.1.1/LICENSE.txt` & `pixmclass-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pixmclass-0.1.1/PKG-INFO` & `pixmclass-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PixMClass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multiclass pixel classification
 Home-page: https://github.com/jeanollion/pix_mclass
-Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz
+Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.2/pix_mclass-0.1.2.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Classification,Microscopy,Cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
-Requires-Dist: dataset_iterator>=0.4.0
+Requires-Dist: dataset_iterator>=0.4.5
 Requires-Dist: elasticdeform
 
 # Multiclass pixel classifier
 Deep learning segmentation method with very low annotation requirement.
 
 Similar to [Ilastik pixel classification](https://www.ilastik.org/documentation/pixelclassification/pixelclassification) procedure, but based on a deep neural network.
```

### Comparing `pixmclass-0.1.1/PixMClass.egg-info/PKG-INFO` & `pixmclass-0.1.2/PixMClass.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: PixMClass
-Version: 0.1.1
+Version: 0.1.2
 Summary: Multiclass pixel classification
 Home-page: https://github.com/jeanollion/pix_mclass
-Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz
+Download-URL: https://github.com/jeanollion/pix_mclass/releases/download/v0.1.2/pix_mclass-0.1.2.tar.gz
 Author: Jean Ollion
 Author-email: jean.ollion@polytechnique.org
 Keywords: Segmentation,Classification,Microscopy,Cell
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Image Processing
@@ -15,15 +15,15 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: numpy
 Requires-Dist: scipy
 Requires-Dist: tensorflow>=2.7.1
-Requires-Dist: dataset_iterator>=0.4.0
+Requires-Dist: dataset_iterator>=0.4.5
 Requires-Dist: elasticdeform
 
 # Multiclass pixel classifier
 Deep learning segmentation method with very low annotation requirement.
 
 Similar to [Ilastik pixel classification](https://www.ilastik.org/documentation/pixelclassification/pixelclassification) procedure, but based on a deep neural network.
```

### Comparing `pixmclass-0.1.1/README.md` & `pixmclass-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pixmclass-0.1.1/pix_mclass/losses.py` & `pixmclass-0.1.2/pix_mclass/losses.py`

 * *Files identical despite different names*

### Comparing `pixmclass-0.1.1/pix_mclass/training.py` & `pixmclass-0.1.2/pix_mclass/training.py`

 * *Files identical despite different names*

### Comparing `pixmclass-0.1.1/pix_mclass/unet.py` & `pixmclass-0.1.2/pix_mclass/unet.py`

 * *Files identical despite different names*

### Comparing `pixmclass-0.1.1/setup.py` & `pixmclass-0.1.2/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PixMClass",
-    version="0.1.1",
+    version="0.1.2",
     author="Jean Ollion",
     author_email="jean.ollion@polytechnique.org",
     description="Multiclass pixel classification",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jeanollion/pix_mclass",
-    download_url='https://github.com/jeanollion/pix_mclass/releases/download/v0.1.1/pix_mclass-0.1.1.tar.gz',
+    download_url='https://github.com/jeanollion/pix_mclass/releases/download/v0.1.2/pix_mclass-0.1.2.tar.gz',
     packages=setuptools.find_packages(),
     keywords = ['Segmentation', 'Classification', 'Microscopy', 'Cell'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Science/Research',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Processing',
         'License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)',
         'Programming Language :: Python :: 3',
     ],
     python_requires='>=3',
-    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'dataset_iterator>=0.4.0', 'elasticdeform']
+    install_requires=['numpy', 'scipy', 'tensorflow>=2.7.1', 'dataset_iterator>=0.4.5', 'elasticdeform']
 )
```

