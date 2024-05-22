# Comparing `tmp/udirect-0.1.4.dev2.tar.gz` & `tmp/udirect-0.1.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udirect-0.1.4.dev2.tar", last modified: Tue May 21 15:02:34 2024, max compression
+gzip compressed data, was "udirect-0.1.4.dev3.tar", last modified: Wed May 22 08:37:00 2024, max compression
```

## Comparing `udirect-0.1.4.dev2.tar` & `udirect-0.1.4.dev3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.4.dev2/LICENSE.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/README.md
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/setup.cfg
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1781 2024-05-21 15:01:32.000000 udirect-0.1.4.dev2/setup.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.753684 udirect-0.1.4.dev2/udirect/
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.757684 udirect-0.1.4.dev2/udirect/directivity_model/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:42.000000 udirect-0.1.4.dev2/udirect/directivity_model/__init.py__
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   100360 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/keras_metadata.pb
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   582224 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/saved_model.pb
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/udirect/directivity_model/variables/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:50.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/__init.py__
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)  6469009 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.data-00000-of-00001
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     8147 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.index
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/xmax.npy
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/xmin.npy
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1564 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/predictiveModel.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.753684 udirect-0.1.4.dev2/udirect.egg-info/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      580 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/SOURCES.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/dependency_links.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/requires.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/top_level.txt
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-22 08:37:00.248945 udirect-0.1.4.dev3/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.4.dev3/LICENSE.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-22 08:37:00.248945 udirect-0.1.4.dev3/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/README.md
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-22 08:37:00.248945 udirect-0.1.4.dev3/setup.cfg
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1781 2024-05-22 08:36:50.000000 udirect-0.1.4.dev3/setup.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-22 08:37:00.240945 udirect-0.1.4.dev3/udirect/
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-22 08:37:00.240945 udirect-0.1.4.dev3/udirect/directivity_model/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:42.000000 udirect-0.1.4.dev3/udirect/directivity_model/__init.py__
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   100360 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/keras_metadata.pb
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   582224 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/saved_model.pb
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-22 08:37:00.248945 udirect-0.1.4.dev3/udirect/directivity_model/variables/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:50.000000 udirect-0.1.4.dev3/udirect/directivity_model/variables/__init.py__
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)  6469009 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/variables/variables.data-00000-of-00001
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     8147 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/variables/variables.index
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/xmax.npy
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev3/udirect/directivity_model/xmin.npy
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1793 2024-05-22 08:36:21.000000 udirect-0.1.4.dev3/udirect/predictiveModel.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-22 08:37:00.240945 udirect-0.1.4.dev3/udirect.egg-info/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-22 08:37:00.000000 udirect-0.1.4.dev3/udirect.egg-info/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      580 2024-05-22 08:37:00.000000 udirect-0.1.4.dev3/udirect.egg-info/SOURCES.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-22 08:37:00.000000 udirect-0.1.4.dev3/udirect.egg-info/dependency_links.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-22 08:37:00.000000 udirect-0.1.4.dev3/udirect.egg-info/requires.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-22 08:37:00.000000 udirect-0.1.4.dev3/udirect.egg-info/top_level.txt
```

### Comparing `udirect-0.1.4.dev2/LICENSE.txt` & `udirect-0.1.4.dev3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev2/PKG-INFO` & `udirect-0.1.4.dev3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.4.dev2
+Version: 0.1.4.dev3
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

### Comparing `udirect-0.1.4.dev2/setup.py` & `udirect-0.1.4.dev3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'udirect',         # How you named your package folder (MyLib)
   packages = ['udirect'],   # Chose the same as "name"
-  version = '0.1.4-dev.2',      # Start with a small number and increase it with every change you make
+  version = '0.1.4-dev.3',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Deep learning tools for modeling rupture forward directivity',   # Give a short description about your library
   author = 'Henning Lilienkamp',                   # Type in your name
   author_email = 'henninglilienkamp@gmx.de',      # Type in your E-Mail
   url = 'https://github.com/HenningLilienkamp/udirect',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz',    # I explain this later on
   keywords = ['Deep learning', 'Rupture forward directivity', 'Modifier of moments'],   # Keywords that define your package best
```

### Comparing `udirect-0.1.4.dev2/udirect/directivity_model/keras_metadata.pb` & `udirect-0.1.4.dev3/udirect/directivity_model/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev2/udirect/directivity_model/saved_model.pb` & `udirect-0.1.4.dev3/udirect/directivity_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.data-00000-of-00001` & `udirect-0.1.4.dev3/udirect/directivity_model/variables/variables.data-00000-of-00001`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.index` & `udirect-0.1.4.dev3/udirect/directivity_model/variables/variables.index`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev2/udirect/predictiveModel.py` & `udirect-0.1.4.dev3/udirect/predictiveModel.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 import numpy as np
 from tensorflow.keras.models import load_model
-
+from importlib.resources import files
 
 class predictiveModel:
-    def __init__(self, model_dir='directivity_model/'):
-        self.model = load_model(model_dir, compile=False)
-        self.xmin = np.load(model_dir+'xmin.npy')[np.array([0, 1, 6, 5, 2, 8, 7, 9])]
-        self.xmax = np.load(model_dir + 'xmax.npy')[np.array([0, 1, 6, 5, 2, 8, 7, 9])]
+    def __init__(self, model_dir='directivity_model'):
+        self.model_path = str(files(model_dir).joinpath("/"))
+        self.model = load_model(self.model_path, compile=False)
+        self.xmin_file = str(files(model_dir).joinpath("xmin.npy"))
+        self.xmax_file = str(files(model_dir).joinpath("xmax.npy"))
+        self.xmin = np.load(self.xmin_file)[np.array([0, 1, 6, 5, 2, 8, 7, 9])]
+        self.xmax = np.load(self.xmax_file)[np.array([0, 1, 6, 5, 2, 8, 7, 9])]
         self.ymin = np.array([-0.73322594165802, 0])
         self.ymax = np.array([0.8272385001182556, 0.5207511782646179])
 
     def predict(self, input):
         '''
         input : array_like
                 Input array of shape (256, 256, 8), where the 8 channels provide:
@@ -30,7 +33,10 @@
         '''
         input_normed = ((input - self.xmin) / (self.xmax - self.xmin)).reshape(1, 256, 256, 8)
         output_normed = self.model.predict(input_normed)
         output = output_normed * (self.ymax - self.ymin) + self.ymin
 
         return output[0, ...]
         
+
+
+
```

### Comparing `udirect-0.1.4.dev2/udirect.egg-info/PKG-INFO` & `udirect-0.1.4.dev3/udirect.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.4.dev2
+Version: 0.1.4.dev3
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

### Comparing `udirect-0.1.4.dev2/udirect.egg-info/SOURCES.txt` & `udirect-0.1.4.dev3/udirect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

