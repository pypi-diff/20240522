# Comparing `tmp/insolver-0.4.dev3.tar.gz` & `tmp/insolver-0.4.dev4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/insolver-0.4.dev3.tar", last modified: Fri Dec 25 13:16:38 2020, max compression
+gzip compressed data, was "dist/insolver-0.4.dev4.tar", last modified: Fri Dec 25 17:19:20 2020, max compression
```

## Comparing `insolver-0.4.dev3.tar` & `insolver-0.4.dev4.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.407201 insolver-0.4.dev3/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2278 2020-12-25 13:16:38.407201 insolver-0.4.dev3/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1263 2020-12-21 16:16:21.000000 insolver-0.4.dev3/README.md
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.403199 insolver-0.4.dev3/insolver/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     9009 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/InsolverGeoTransforms.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3142 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/InsolverPlotsGBM.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1793 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/InsolverUtils.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    11466 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/InsuranceDFCreator.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       45 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/__init__.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.403199 insolver-0.4.dev3/insolver/frame/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       37 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/frame/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1212 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/frame/frame.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.407201 insolver-0.4.dev3/insolver/model_tools/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      155 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/model_tools/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     6162 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/model_tools/model_comparison.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     3585 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/model_tools/model_utils.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.407201 insolver-0.4.dev3/insolver/serving/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2020-12-10 15:15:30.000000 insolver-0.4.dev3/insolver/serving/__main__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     1160 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/serving/fastapi_app.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2549 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/serving/flask_app.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      922 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/serving/run_service.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.407201 insolver-0.4.dev3/insolver/transforms/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     4043 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/transforms/InsolverTransformMain.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    27016 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/transforms/InsolverTransforms.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      104 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/transforms/__init__.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.407201 insolver-0.4.dev3/insolver/wrappers/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      113 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/wrappers/__init__.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    15072 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/wrappers/base.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    12580 2020-12-21 16:16:21.000000 insolver-0.4.dev3/insolver/wrappers/gbm.py
--rw-rw-r--   0 andrey    (1000) andrey    (1000)    12871 2020-12-23 12:45:55.000000 insolver-0.4.dev3/insolver/wrappers/glm.py
-drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 13:16:38.403199 insolver-0.4.dev3/insolver.egg-info/
--rw-rw-r--   0 andrey    (1000) andrey    (1000)     2278 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/PKG-INFO
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      893 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/SOURCES.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/dependency_links.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       71 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/entry_points.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2020-12-24 11:15:40.000000 insolver-0.4.dev3/insolver.egg-info/not-zip-safe
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      180 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/requires.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)        9 2020-12-25 13:16:38.000000 insolver-0.4.dev3/insolver.egg-info/top_level.txt
--rw-rw-r--   0 andrey    (1000) andrey    (1000)       38 2020-12-25 13:16:38.407201 insolver-0.4.dev3/setup.cfg
--rw-rw-r--   0 andrey    (1000) andrey    (1000)      996 2020-12-25 13:04:44.000000 insolver-0.4.dev3/setup.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.731058 insolver-0.4.dev4/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2173 2020-12-25 17:19:20.731058 insolver-0.4.dev4/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1174 2020-12-25 13:30:52.000000 insolver-0.4.dev4/README.md
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.723058 insolver-0.4.dev4/insolver/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     9009 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/InsolverGeoTransforms.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3142 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/InsolverPlotsGBM.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1793 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/InsolverUtils.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    11466 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/InsuranceDFCreator.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       45 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/__init__.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.723058 insolver-0.4.dev4/insolver/frame/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       37 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/frame/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1212 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/frame/frame.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.727058 insolver-0.4.dev4/insolver/model_tools/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      155 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/model_tools/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     6162 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/model_tools/model_comparison.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     3585 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/model_tools/model_utils.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.727058 insolver-0.4.dev4/insolver/serving/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        0 2020-12-10 15:15:30.000000 insolver-0.4.dev4/insolver/serving/__main__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     1160 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/serving/fastapi_app.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2549 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/serving/flask_app.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      922 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/serving/run_service.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.727058 insolver-0.4.dev4/insolver/transforms/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     4043 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/transforms/InsolverTransformMain.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    27016 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/transforms/InsolverTransforms.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      104 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/transforms/__init__.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.731058 insolver-0.4.dev4/insolver/wrappers/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      113 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/wrappers/__init__.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    15072 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/wrappers/base.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    12580 2020-12-21 16:16:21.000000 insolver-0.4.dev4/insolver/wrappers/gbm.py
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)    12871 2020-12-23 12:45:55.000000 insolver-0.4.dev4/insolver/wrappers/glm.py
+drwxrwxr-x   0 andrey    (1000) andrey    (1000)        0 2020-12-25 17:19:20.723058 insolver-0.4.dev4/insolver.egg-info/
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)     2173 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/PKG-INFO
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      893 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       71 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/entry_points.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        1 2020-12-24 11:15:40.000000 insolver-0.4.dev4/insolver.egg-info/not-zip-safe
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      180 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/requires.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)        9 2020-12-25 17:19:20.000000 insolver-0.4.dev4/insolver.egg-info/top_level.txt
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)       38 2020-12-25 17:19:20.731058 insolver-0.4.dev4/setup.cfg
+-rw-rw-r--   0 andrey    (1000) andrey    (1000)      996 2020-12-25 13:32:22.000000 insolver-0.4.dev4/setup.py
```

### Comparing `insolver-0.4.dev3/PKG-INFO` & `insolver-0.4.dev4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: insolver
-Version: 0.4.dev3
+Version: 0.4.dev4
 Summary: Mindset insurance scoring
 Home-page: https://github.com/MindSetLib/MS-InsuranceScoring
 Author: Mindset
 Author-email: request@mind-set.ru
 License: MIT
 Description: # Insolver
         
         Mindset insurance scoring - product repository
         
         ## Installation:
         
         ```shell
-        pip install "git+ssh://git@github.com/MindSetLib/MS-InsuranceScoring.git"
+        pip install insolver
         ```
-        ### Post-install cavets:
+        ### Post-install:
         
         To fix displaying plotly figs in jyputerlab install:
         ```shell
         jupyter labextension install jupyterlab-plotly
         ```
         
         In case of problem with `pyodbc` you may need to install:
@@ -73,15 +73,13 @@
         ```
         
         
         ## Contributing to Insolver:
         
         Please, feel free to open an issue or/and suggest PR, if you find any bugs or any enhancements.
         
-        [link to CONTRIBUTING.md]()
-        
 Keywords: ML insurance scoring
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `insolver-0.4.dev3/README.md` & `insolver-0.4.dev4/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Insolver
 
 Mindset insurance scoring - product repository
 
 ## Installation:
 
 ```shell
-pip install "git+ssh://git@github.com/MindSetLib/MS-InsuranceScoring.git"
+pip install insolver
 ```
-### Post-install cavets:
+### Post-install:
 
 To fix displaying plotly figs in jyputerlab install:
 ```shell
 jupyter labextension install jupyterlab-plotly
 ```
 
 In case of problem with `pyodbc` you may need to install:
@@ -64,9 +64,7 @@
 python -m pytest --cov=insolver; coverage html; xdg-open htmlcov/index.html
 ```
 
 
 ## Contributing to Insolver:
 
 Please, feel free to open an issue or/and suggest PR, if you find any bugs or any enhancements.
-
-[link to CONTRIBUTING.md]()
```

### Comparing `insolver-0.4.dev3/insolver/InsolverGeoTransforms.py` & `insolver-0.4.dev4/insolver/InsolverGeoTransforms.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/InsolverPlotsGBM.py` & `insolver-0.4.dev4/insolver/InsolverPlotsGBM.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/InsolverUtils.py` & `insolver-0.4.dev4/insolver/InsolverUtils.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/InsuranceDFCreator.py` & `insolver-0.4.dev4/insolver/InsuranceDFCreator.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/frame/frame.py` & `insolver-0.4.dev4/insolver/frame/frame.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/model_tools/model_comparison.py` & `insolver-0.4.dev4/insolver/model_tools/model_comparison.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/model_tools/model_utils.py` & `insolver-0.4.dev4/insolver/model_tools/model_utils.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/serving/fastapi_app.py` & `insolver-0.4.dev4/insolver/serving/fastapi_app.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/serving/flask_app.py` & `insolver-0.4.dev4/insolver/serving/flask_app.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/serving/run_service.py` & `insolver-0.4.dev4/insolver/serving/run_service.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/transforms/InsolverTransformMain.py` & `insolver-0.4.dev4/insolver/transforms/InsolverTransformMain.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/transforms/InsolverTransforms.py` & `insolver-0.4.dev4/insolver/transforms/InsolverTransforms.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/wrappers/base.py` & `insolver-0.4.dev4/insolver/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/wrappers/gbm.py` & `insolver-0.4.dev4/insolver/wrappers/gbm.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver/wrappers/glm.py` & `insolver-0.4.dev4/insolver/wrappers/glm.py`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/insolver.egg-info/PKG-INFO` & `insolver-0.4.dev4/insolver.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: insolver
-Version: 0.4.dev3
+Version: 0.4.dev4
 Summary: Mindset insurance scoring
 Home-page: https://github.com/MindSetLib/MS-InsuranceScoring
 Author: Mindset
 Author-email: request@mind-set.ru
 License: MIT
 Description: # Insolver
         
         Mindset insurance scoring - product repository
         
         ## Installation:
         
         ```shell
-        pip install "git+ssh://git@github.com/MindSetLib/MS-InsuranceScoring.git"
+        pip install insolver
         ```
-        ### Post-install cavets:
+        ### Post-install:
         
         To fix displaying plotly figs in jyputerlab install:
         ```shell
         jupyter labextension install jupyterlab-plotly
         ```
         
         In case of problem with `pyodbc` you may need to install:
@@ -73,15 +73,13 @@
         ```
         
         
         ## Contributing to Insolver:
         
         Please, feel free to open an issue or/and suggest PR, if you find any bugs or any enhancements.
         
-        [link to CONTRIBUTING.md]()
-        
 Keywords: ML insurance scoring
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `insolver-0.4.dev3/insolver.egg-info/SOURCES.txt` & `insolver-0.4.dev4/insolver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `insolver-0.4.dev3/setup.py` & `insolver-0.4.dev4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     required = f.read().splitlines()
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 
 setup(name='insolver',
-      version='0.4.dev3',
+      version='0.4.dev4',
       description='Mindset insurance scoring',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/MindSetLib/MS-InsuranceScoring',
       keywords='ML insurance scoring',
       author='Mindset',
       author_email='request@mind-set.ru',
```

