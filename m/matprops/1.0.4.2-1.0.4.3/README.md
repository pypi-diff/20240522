# Comparing `tmp/matprops-1.0.4.2.tar.gz` & `tmp/matprops-1.0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matprops-1.0.4.2.tar", last modified: Mon May 20 00:42:51 2024, max compression
+gzip compressed data, was "matprops-1.0.4.3.tar", last modified: Wed May 22 21:25:32 2024, max compression
```

## Comparing `matprops-1.0.4.2.tar` & `matprops-1.0.4.3.tar`

### file list

```diff
@@ -1,16 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:42:51.407963 matprops-1.0.4.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-20 00:42:47.000000 matprops-1.0.4.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-20 00:42:51.407963 matprops-1.0.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-20 00:42:47.000000 matprops-1.0.4.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-20 00:42:51.407963 matprops-1.0.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-20 00:42:47.000000 matprops-1.0.4.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:42:51.403963 matprops-1.0.4.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:42:51.407963 matprops-1.0.4.2/src/matprops/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-20 00:42:47.000000 matprops-1.0.4.2/src/matprops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5321 2024-05-20 00:42:47.000000 matprops-1.0.4.2/src/matprops/props.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-20 00:42:51.407963 matprops-1.0.4.2/src/matprops.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-20 00:42:51.000000 matprops-1.0.4.2/src/matprops.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-20 00:42:51.000000 matprops-1.0.4.2/src/matprops.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-20 00:42:51.000000 matprops-1.0.4.2/src/matprops.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-20 00:42:51.000000 matprops-1.0.4.2/src/matprops.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-20 00:42:51.000000 matprops-1.0.4.2/src/matprops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.827463 matprops-1.0.4.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-05-22 21:25:28.000000 matprops-1.0.4.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-22 21:25:32.827463 matprops-1.0.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-22 21:25:28.000000 matprops-1.0.4.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:25:32.827463 matprops-1.0.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-05-22 21:25:28.000000 matprops-1.0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.819463 matprops-1.0.4.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/matprops/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/matprops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5318 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/matprops/props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/matprops.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2024-05-22 21:25:32.000000 matprops-1.0.4.3/src/matprops.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-22 21:25:32.000000 matprops-1.0.4.3/src/matprops.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:25:32.000000 matprops-1.0.4.3/src/matprops.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-22 21:25:32.000000 matprops-1.0.4.3/src/matprops.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-22 21:25:32.000000 matprops-1.0.4.3/src/matprops.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/resources/configs/
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2478 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/configs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4808 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/configs/props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/resources/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/utils/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/resources/utils/props.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:32.823463 matprops-1.0.4.3/src/validation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/validation/pil.py
+-rw-r--r--   0 runner    (1001) docker     (127)      249 2024-05-22 21:25:28.000000 matprops-1.0.4.3/src/validation/prop_test.py
```

### Comparing `matprops-1.0.4.2/LICENSE` & `matprops-1.0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `matprops-1.0.4.2/PKG-INFO` & `matprops-1.0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.4.2
+Version: 1.0.4.3
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `matprops-1.0.4.2/README.md` & `matprops-1.0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `matprops-1.0.4.2/setup.py` & `matprops-1.0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setup(
     name='matprops',
-    version='1.0.4.2',
+    version='1.0.4.3',
     packages=find_packages(where="src"),
     package_dir={'': 'src'},
     classifiers=[
         "Programming Language :: Python :: 3",
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
```

### Comparing `matprops-1.0.4.2/src/matprops/props.py` & `matprops-1.0.4.3/src/matprops/props.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import matplotlib
 
-from ...resources.configs.props import *
-from ...resources.utils.props import *
-from ...resources.utils.figure import *
+from ..resources.configs.props import *
+from ..resources.utils.props import *
+from ..resources.utils.figure import *
 
 
 def AreaProp(dataset, col, cols=8, labels=True, label_loc="inc", labelcolor="blue", title=None, title_loc="tl",
              facecolor="blue", bgcolor="#707070", description=None):
     """
     Square area proportional chart
     This function is used to create and customize almost everything in basic square area proportional chart
```

### Comparing `matprops-1.0.4.2/src/matprops.egg-info/PKG-INFO` & `matprops-1.0.4.3/src/matprops.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matprops
-Version: 1.0.4.2
+Version: 1.0.4.3
 Summary: Python library written on top of matplotlib library for customizable proportional charts
 Home-page: https://github.com/shammeer-s/matprops
 Author: Mohammed Shammeer
 Author-email: mohammedshammeer.s@gmail.com
 Keywords: matplotlib,visualization,proportional charts
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
```

