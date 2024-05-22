# Comparing `tmp/xai_feature_selection-0.1.tar.gz` & `tmp/xai_feature_selection-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xai_feature_selection-0.1.tar", last modified: Wed May 22 17:49:54 2024, max compression
+gzip compressed data, was "xai_feature_selection-0.2.tar", last modified: Wed May 22 17:23:40 2024, max compression
```

## Comparing `xai_feature_selection-0.1.tar` & `xai_feature_selection-0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 17:49:54.808628 xai_feature_selection-0.1/
--rw-rw-rw-   0        0        0     1067 2024-05-20 18:12:40.000000 xai_feature_selection-0.1/LICENSE.txt
--rw-rw-rw-   0        0        0      788 2024-05-22 17:49:54.805423 xai_feature_selection-0.1/PKG-INFO
--rw-rw-rw-   0        0        0      158 2024-05-22 16:59:01.000000 xai_feature_selection-0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-05-22 17:49:54.809125 xai_feature_selection-0.1/setup.cfg
--rw-rw-rw-   0        0        0     1187 2024-05-22 17:48:07.000000 xai_feature_selection-0.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:49:54.774373 xai_feature_selection-0.1/xai_feature_selection/
--rw-rw-rw-   0        0        0        0 2024-05-20 17:52:08.000000 xai_feature_selection-0.1/xai_feature_selection/__init__.py
--rw-rw-rw-   0        0        0     4218 2024-05-22 12:40:20.000000 xai_feature_selection-0.1/xai_feature_selection/feature_selection.py
--rw-rw-rw-   0        0        0     5703 2024-05-22 12:40:22.000000 xai_feature_selection-0.1/xai_feature_selection/model_prediction.py
-drwxrwxrwx   0        0        0        0 2024-05-22 17:49:54.802649 xai_feature_selection-0.1/xai_feature_selection.egg-info/
--rw-rw-rw-   0        0        0      788 2024-05-22 17:49:54.000000 xai_feature_selection-0.1/xai_feature_selection.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      373 2024-05-22 17:49:54.000000 xai_feature_selection-0.1/xai_feature_selection.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 17:49:54.000000 xai_feature_selection-0.1/xai_feature_selection.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2024-05-22 17:49:54.000000 xai_feature_selection-0.1/xai_feature_selection.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2024-05-22 17:49:54.000000 xai_feature_selection-0.1/xai_feature_selection.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-22 17:23:40.676195 xai_feature_selection-0.2/
+-rw-rw-rw-   0        0        0     1067 2024-05-20 18:12:40.000000 xai_feature_selection-0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0      788 2024-05-22 17:23:40.676195 xai_feature_selection-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      158 2024-05-22 16:59:01.000000 xai_feature_selection-0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-05-22 17:23:40.677209 xai_feature_selection-0.2/setup.cfg
+-rw-rw-rw-   0        0        0     1187 2024-05-22 17:00:05.000000 xai_feature_selection-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:23:40.653459 xai_feature_selection-0.2/xai_feature_selection/
+-rw-rw-rw-   0        0        0        0 2024-05-20 17:52:08.000000 xai_feature_selection-0.2/xai_feature_selection/__init__.py
+-rw-rw-rw-   0        0        0     4218 2024-05-22 12:40:20.000000 xai_feature_selection-0.2/xai_feature_selection/feature_selection.py
+-rw-rw-rw-   0        0        0     5703 2024-05-22 12:40:22.000000 xai_feature_selection-0.2/xai_feature_selection/model_prediction.py
+drwxrwxrwx   0        0        0        0 2024-05-22 17:23:40.673288 xai_feature_selection-0.2/xai_feature_selection.egg-info/
+-rw-rw-rw-   0        0        0      788 2024-05-22 17:23:40.000000 xai_feature_selection-0.2/xai_feature_selection.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      373 2024-05-22 17:23:40.000000 xai_feature_selection-0.2/xai_feature_selection.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 17:23:40.000000 xai_feature_selection-0.2/xai_feature_selection.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2024-05-22 17:23:40.000000 xai_feature_selection-0.2/xai_feature_selection.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2024-05-22 17:23:40.000000 xai_feature_selection-0.2/xai_feature_selection.egg-info/top_level.txt
```

### Comparing `xai_feature_selection-0.1/LICENSE.txt` & `xai_feature_selection-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `xai_feature_selection-0.1/PKG-INFO` & `xai_feature_selection-0.2/xai_feature_selection.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xai_feature_selection
-Version: 0.1
+Name: xai-feature-selection
+Version: 0.2
 Summary: Feature selection using XAI
 Author: Yaganteeswarudu Akkem
 Author-email: yaganteeswaritexpert@gmail.com
 Keywords: machine learning,feature selection,explainable artificial intelligence,XAI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `xai_feature_selection-0.1/setup.py` & `xai_feature_selection-0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 DESCRIPTION = 'Feature selection using XAI'
 LONG_DESCRIPTION = 'allows to select best features using XAI by combining with local and global importance'
 
 # Setting up
 setup(
     name="xai_feature_selection",
-    version="0.1",
+    version="0.2",
     author="Yaganteeswarudu Akkem",
     author_email="yaganteeswaritexpert@gmail.com",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
     install_requires=[ 'pandas==2.0.*','lime', 'shap'],
```

### Comparing `xai_feature_selection-0.1/xai_feature_selection/feature_selection.py` & `xai_feature_selection-0.2/xai_feature_selection/feature_selection.py`

 * *Files identical despite different names*

### Comparing `xai_feature_selection-0.1/xai_feature_selection/model_prediction.py` & `xai_feature_selection-0.2/xai_feature_selection/model_prediction.py`

 * *Files identical despite different names*

### Comparing `xai_feature_selection-0.1/xai_feature_selection.egg-info/PKG-INFO` & `xai_feature_selection-0.2/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: xai-feature-selection
-Version: 0.1
+Name: xai_feature_selection
+Version: 0.2
 Summary: Feature selection using XAI
 Author: Yaganteeswarudu Akkem
 Author-email: yaganteeswaritexpert@gmail.com
 Keywords: machine learning,feature selection,explainable artificial intelligence,XAI
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

