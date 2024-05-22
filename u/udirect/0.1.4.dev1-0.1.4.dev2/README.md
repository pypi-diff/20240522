# Comparing `tmp/udirect-0.1.4.dev1.tar.gz` & `tmp/udirect-0.1.4.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "udirect-0.1.4.dev1.tar", last modified: Tue May 21 14:58:12 2024, max compression
+gzip compressed data, was "udirect-0.1.4.dev2.tar", last modified: Tue May 21 15:02:34 2024, max compression
```

## Comparing `udirect-0.1.4.dev1.tar` & `udirect-0.1.4.dev2.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:58:12.423828 udirect-0.1.4.dev1/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.4.dev1/LICENSE.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:58:12.423828 udirect-0.1.4.dev1/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/README.md
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-21 14:58:12.423828 udirect-0.1.4.dev1/setup.cfg
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1748 2024-05-21 14:58:01.000000 udirect-0.1.4.dev1/setup.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:58:12.419827 udirect-0.1.4.dev1/udirect/
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:58:12.423828 udirect-0.1.4.dev1/udirect/directivity_model/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:42.000000 udirect-0.1.4.dev1/udirect/directivity_model/__init.py__
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   100360 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/udirect/directivity_model/keras_metadata.pb
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   582224 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/udirect/directivity_model/saved_model.pb
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/udirect/directivity_model/xmax.npy
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/udirect/directivity_model/xmin.npy
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1564 2024-05-21 12:47:16.000000 udirect-0.1.4.dev1/udirect/predictiveModel.py
-drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:58:12.423828 udirect-0.1.4.dev1/udirect.egg-info/
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 14:58:12.000000 udirect-0.1.4.dev1/udirect.egg-info/PKG-INFO
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      414 2024-05-21 14:58:12.000000 udirect-0.1.4.dev1/udirect.egg-info/SOURCES.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-21 14:58:12.000000 udirect-0.1.4.dev1/udirect.egg-info/dependency_links.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-21 14:58:12.000000 udirect-0.1.4.dev1/udirect.egg-info/requires.txt
--rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-21 14:58:12.000000 udirect-0.1.4.dev1/udirect.egg-info/top_level.txt
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1074 2024-05-21 13:48:20.000000 udirect-0.1.4.dev2/LICENSE.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        9 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/README.md
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       79 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/setup.cfg
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1781 2024-05-21 15:01:32.000000 udirect-0.1.4.dev2/setup.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.753684 udirect-0.1.4.dev2/udirect/
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.757684 udirect-0.1.4.dev2/udirect/directivity_model/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:42.000000 udirect-0.1.4.dev2/udirect/directivity_model/__init.py__
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   100360 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/keras_metadata.pb
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)   582224 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/saved_model.pb
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.761684 udirect-0.1.4.dev2/udirect/directivity_model/variables/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 14:57:50.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/__init.py__
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)  6469009 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.data-00000-of-00001
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     8147 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/variables/variables.index
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/xmax.npy
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      216 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/directivity_model/xmin.npy
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)     1564 2024-05-21 12:47:16.000000 udirect-0.1.4.dev2/udirect/predictiveModel.py
+drwxrwxr-x   0 lilienka  (1000) lilienka  (1000)        0 2024-05-21 15:02:34.753684 udirect-0.1.4.dev2/udirect.egg-info/
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      743 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/PKG-INFO
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)      580 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/SOURCES.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        1 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/dependency_links.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)       17 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/requires.txt
+-rw-rw-r--   0 lilienka  (1000) lilienka  (1000)        8 2024-05-21 15:02:34.000000 udirect-0.1.4.dev2/udirect.egg-info/top_level.txt
```

### Comparing `udirect-0.1.4.dev1/LICENSE.txt` & `udirect-0.1.4.dev2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev1/PKG-INFO` & `udirect-0.1.4.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

### Comparing `udirect-0.1.4.dev1/setup.py` & `udirect-0.1.4.dev2/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'udirect',         # How you named your package folder (MyLib)
   packages = ['udirect'],   # Chose the same as "name"
-  version = '0.1.4-dev.1',      # Start with a small number and increase it with every change you make
+  version = '0.1.4-dev.2',      # Start with a small number and increase it with every change you make
   license='MIT',        # Chose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Deep learning tools for modeling rupture forward directivity',   # Give a short description about your library
   author = 'Henning Lilienkamp',                   # Type in your name
   author_email = 'henninglilienkamp@gmx.de',      # Type in your E-Mail
   url = 'https://github.com/HenningLilienkamp/udirect',   # Provide either the link to your github or to your website
   download_url = 'https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz',    # I explain this later on
   keywords = ['Deep learning', 'Rupture forward directivity', 'Modifier of moments'],   # Keywords that define your package best
@@ -21,10 +21,10 @@
     'Topic :: Software Development :: Build Tools',
 
     'License :: OSI Approved :: MIT License',   # Again, pick a license
 
     'Programming Language :: Python :: 3',      #Specify which pyhton versions that you want to support
     'Programming Language :: Python :: 3.9',
   ],
-  package_data={'udirect' :['directivity_model/*']},
+  package_data={'udirect' :['directivity_model/*', 'directivity_model/variables/*']},
   include_package_data=True,
 )
```

### Comparing `udirect-0.1.4.dev1/udirect/directivity_model/keras_metadata.pb` & `udirect-0.1.4.dev2/udirect/directivity_model/keras_metadata.pb`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev1/udirect/directivity_model/saved_model.pb` & `udirect-0.1.4.dev2/udirect/directivity_model/saved_model.pb`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev1/udirect/predictiveModel.py` & `udirect-0.1.4.dev2/udirect/predictiveModel.py`

 * *Files identical despite different names*

### Comparing `udirect-0.1.4.dev1/udirect.egg-info/PKG-INFO` & `udirect-0.1.4.dev2/udirect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: udirect
-Version: 0.1.4.dev1
+Version: 0.1.4.dev2
 Summary: Deep learning tools for modeling rupture forward directivity
 Home-page: https://github.com/HenningLilienkamp/udirect
 Download-URL: https://github.com/HenningLilienkamp/udirect/archive/refs/tags/v.0.1.tar.gz
 Author: Henning Lilienkamp
 Author-email: henninglilienkamp@gmx.de
 License: MIT
 Keywords: Deep learning,Rupture forward directivity,Modifier of moments
```

