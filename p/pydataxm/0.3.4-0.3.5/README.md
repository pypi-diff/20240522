# Comparing `tmp/pydataxm-0.3.4.tar.gz` & `tmp/pydataxm-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydataxm-0.3.4.tar", last modified: Wed Feb 28 21:40:11 2024, max compression
+gzip compressed data, was "pydataxm-0.3.5.tar", last modified: Tue May 21 21:32:48 2024, max compression
```

## Comparing `pydataxm-0.3.4.tar` & `pydataxm-0.3.5.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-02-28 21:40:11.178753 pydataxm-0.3.4/
--rw-rw-rw-   0        0        0     1092 2024-02-28 21:35:31.000000 pydataxm-0.3.4/LICENSE
--rw-rw-rw-   0        0        0        0 2024-02-28 21:35:31.000000 pydataxm-0.3.4/MANIFEST.in
--rw-rw-rw-   0        0        0      739 2024-02-28 21:40:11.177680 pydataxm-0.3.4/PKG-INFO
--rw-rw-rw-   0        0        0    10324 2024-02-28 21:35:31.000000 pydataxm-0.3.4/README.md
-drwxrwxrwx   0        0        0        0 2024-02-28 21:40:11.153375 pydataxm-0.3.4/pydataxm/
--rw-rw-rw-   0        0        0       24 2024-02-28 21:35:31.000000 pydataxm-0.3.4/pydataxm/__init__.py
--rw-rw-rw-   0        0        0    10587 2024-02-28 21:35:31.000000 pydataxm-0.3.4/pydataxm/pydataxm.py
-drwxrwxrwx   0        0        0        0 2024-02-28 21:40:11.175678 pydataxm-0.3.4/pydataxm.egg-info/
--rw-rw-rw-   0        0        0      739 2024-02-28 21:40:10.000000 pydataxm-0.3.4/pydataxm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      249 2024-02-28 21:40:11.000000 pydataxm-0.3.4/pydataxm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-28 21:40:10.000000 pydataxm-0.3.4/pydataxm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2024-02-28 21:40:10.000000 pydataxm-0.3.4/pydataxm.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2024-02-28 21:40:10.000000 pydataxm-0.3.4/pydataxm.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2024-02-28 21:40:11.184773 pydataxm-0.3.4/setup.cfg
--rw-rw-rw-   0        0        0     1525 2024-02-28 21:35:59.000000 pydataxm-0.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:32:48.497964 pydataxm-0.3.5/
+-rw-rw-rw-   0        0        0     1092 2024-05-21 21:16:34.000000 pydataxm-0.3.5/LICENSE
+-rw-rw-rw-   0        0        0        0 2024-05-21 21:16:34.000000 pydataxm-0.3.5/MANIFEST.in
+-rw-rw-rw-   0        0        0      739 2024-05-21 21:32:48.497964 pydataxm-0.3.5/PKG-INFO
+-rw-rw-rw-   0        0        0    10324 2024-05-21 21:16:34.000000 pydataxm-0.3.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-21 21:32:48.497964 pydataxm-0.3.5/pydataxm/
+-rw-rw-rw-   0        0        0       24 2024-05-21 21:16:34.000000 pydataxm-0.3.5/pydataxm/__init__.py
+-rw-rw-rw-   0        0        0     5597 2024-05-21 21:16:22.000000 pydataxm-0.3.5/pydataxm/pydatasimem.py
+-rw-rw-rw-   0        0        0    10621 2024-05-21 21:16:37.000000 pydataxm-0.3.5/pydataxm/pydataxm.py
+drwxrwxrwx   0        0        0        0 2024-05-21 21:32:48.497964 pydataxm-0.3.5/pydataxm.egg-info/
+-rw-rw-rw-   0        0        0      739 2024-05-21 21:32:48.000000 pydataxm-0.3.5/pydataxm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      273 2024-05-21 21:32:48.000000 pydataxm-0.3.5/pydataxm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-21 21:32:48.000000 pydataxm-0.3.5/pydataxm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2024-05-21 21:32:48.000000 pydataxm-0.3.5/pydataxm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-21 21:32:48.000000 pydataxm-0.3.5/pydataxm.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2024-05-21 21:32:48.512481 pydataxm-0.3.5/setup.cfg
+-rw-rw-rw-   0        0        0     1525 2024-05-21 21:29:54.000000 pydataxm-0.3.5/setup.py
```

### Comparing `pydataxm-0.3.4/LICENSE` & `pydataxm-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pydataxm-0.3.4/PKG-INFO` & `pydataxm-0.3.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pydataxm
-Version: 0.3.4
+Version: 0.3.5
 Summary: Interface to play with the API XM
 Home-page: https://github.com/EquipoAnaliticaXM/API_XM
 Download-URL: https://raw.githubusercontent.com/EquipoAnaliticaXM/API_XM/master/pydataxm/pydataxm.py
 Author: Equipo Analitica XM
 Author-email: analitica@xm.com.co
 License: MIT
 Keywords: API interpreter,Mercado Energía Mayorista,XM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: datetime
```

### Comparing `pydataxm-0.3.4/README.md` & `pydataxm-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `pydataxm-0.3.4/pydataxm/pydataxm.py` & `pydataxm-0.3.5/pydataxm/pydataxm.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 import requests
 import json
 import pandas as pd
 import datetime as dt
 import time 
 # noinspection SpellCheckingInspection
-
+from pydataxm.pydatasimem import *
 
 class ReadDB(object):
 
     def __new__(cls):
         return super(ReadDB, cls).__new__(cls)
```

### Comparing `pydataxm-0.3.4/pydataxm.egg-info/PKG-INFO` & `pydataxm-0.3.5/pydataxm.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pydataxm
-Version: 0.3.4
+Version: 0.3.5
 Summary: Interface to play with the API XM
 Home-page: https://github.com/EquipoAnaliticaXM/API_XM
 Download-URL: https://raw.githubusercontent.com/EquipoAnaliticaXM/API_XM/master/pydataxm/pydataxm.py
 Author: Equipo Analitica XM
 Author-email: analitica@xm.com.co
 License: MIT
 Keywords: API interpreter,Mercado Energía Mayorista,XM
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.6
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: pandas
 Requires-Dist: datetime
```

### Comparing `pydataxm-0.3.4/setup.py` & `pydataxm-0.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from distutils.core import setup
 setup(
   name = 'pydataxm',         # How you named your package folder (MyLib)
   packages = ['pydataxm'],   # Chose the same as "name"
-  version = '0.3.4',      # Start with a small number and increase it with every change you make
+  version = '0.3.5',      # Start with a small number and increase it with every change you make
   license='MIT',        # Choose a license from here: https://help.github.com/articles/licensing-a-repository
   description = 'Interface to play with the API XM',   # Give a short description about your library
   author = 'Equipo Analitica XM',                   # Type in your name
   author_email = 'analitica@xm.com.co',      # Type in your E-Mail
   url = 'https://github.com/EquipoAnaliticaXM/API_XM',   # Provide either the link to your github or to your website
   download_url = 'https://raw.githubusercontent.com/EquipoAnaliticaXM/API_XM/master/pydataxm/pydataxm.py',    # I explain this later on
   keywords = ['API interpreter','Mercado Energía Mayorista', 'XM'],   # Keywords that define your package best
   install_requires=[            # I get to this in a second
           'requests', 'pandas','datetime'],
   classifiers=[
     'Development Status :: 3 - Alpha',      # Chose either "3 - Alpha", "4 - Beta" or "5 - Production/Stable" as the current state of your package
     'Intended Audience :: Developers',      # Define that your audience are developers
     'Topic :: Software Development :: Build Tools',
     'License :: OSI Approved :: MIT License',   # Again, pick a license
-    'Programming Language :: Python :: 3.9']
+    'Programming Language :: Python :: 3.6']
 )
```

