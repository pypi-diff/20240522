# Comparing `tmp/mapclassif_Iron-2.6.2.tar.gz` & `tmp/mapclassif_Iron-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapclassif_Iron-2.6.2.tar", last modified: Wed May 22 11:17:28 2024, max compression
+gzip compressed data, was "mapclassif_Iron-2.6.3.tar", last modified: Wed May 22 11:24:49 2024, max compression
```

## Comparing `mapclassif_Iron-2.6.2.tar` & `mapclassif_Iron-2.6.3.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 11:17:28.101940 mapclassif_Iron-2.6.2/
--rw-rw-rw-   0        0        0     1485 2023-12-13 18:11:42.000000 mapclassif_Iron-2.6.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1770 2024-05-22 11:17:28.093066 mapclassif_Iron-2.6.2/PKG-INFO
--rw-rw-rw-   0        0        0    10777 2024-05-20 21:57:54.000000 mapclassif_Iron-2.6.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-22 11:17:27.701702 mapclassif_Iron-2.6.2/mapclassif_Iron/
--rw-rw-rw-   0        0        0        2 2023-12-15 12:29:32.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/__init__.py
--rw-rw-rw-   0        0        0     2980 2023-12-15 13:50:35.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/classifiers.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:17:28.021271 mapclassif_Iron-2.6.2/mapclassif_Iron/datasets/
--rw-rw-rw-   0        0        0       51 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/datasets/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:17:28.088462 mapclassif_Iron-2.6.2/mapclassif_Iron/datasets/calemp/
--rw-rw-rw-   0        0        0       21 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/datasets/calemp/__init__.py
--rw-rw-rw-   0        0        0      450 2023-12-15 14:13:40.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/datasets/calemp/data.py
--rw-rw-rw-   0        0        0     3338 2024-05-20 21:34:52.000000 mapclassif_Iron-2.6.2/mapclassif_Iron/test_fisher_jenks_means.py
-drwxrwxrwx   0        0        0        0 2024-05-22 11:17:27.943874 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/
--rw-rw-rw-   0        0        0     1770 2024-05-22 11:17:27.000000 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      453 2024-05-22 11:17:27.000000 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 11:17:27.000000 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       22 2024-05-22 11:17:27.000000 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2024-05-22 11:17:27.000000 mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2999 2024-05-22 11:16:43.000000 mapclassif_Iron-2.6.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-22 11:17:28.102788 mapclassif_Iron-2.6.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:49.413422 mapclassif_Iron-2.6.3/
+-rw-rw-rw-   0        0        0     1485 2023-12-13 18:11:42.000000 mapclassif_Iron-2.6.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     1770 2024-05-22 11:24:49.413422 mapclassif_Iron-2.6.3/PKG-INFO
+-rw-rw-rw-   0        0        0    10777 2024-05-20 21:57:54.000000 mapclassif_Iron-2.6.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:49.258751 mapclassif_Iron-2.6.3/mapclassif_Iron/
+-rw-rw-rw-   0        0        0        2 2023-12-15 12:29:32.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/__init__.py
+-rw-rw-rw-   0        0        0     2980 2023-12-15 13:50:35.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/classifiers.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:49.345771 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/
+-rw-rw-rw-   0        0        0       51 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:49.397651 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/calemp/
+-rw-rw-rw-   0        0        0      319 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/calemp/README.md
+-rw-rw-rw-   0        0        0       21 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/calemp/__init__.py
+-rw-rw-rw-   0        0        0     7122 2023-12-15 11:44:14.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/calemp/calempdensity.csv
+-rw-rw-rw-   0        0        0      450 2023-12-15 14:13:40.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/datasets/calemp/data.py
+-rw-rw-rw-   0        0        0     3338 2024-05-20 21:34:52.000000 mapclassif_Iron-2.6.3/mapclassif_Iron/test_fisher_jenks_means.py
+drwxrwxrwx   0        0        0        0 2024-05-22 11:24:49.329172 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/
+-rw-rw-rw-   0        0        0     1770 2024-05-22 11:24:48.000000 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      545 2024-05-22 11:24:48.000000 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 11:24:48.000000 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       22 2024-05-22 11:24:48.000000 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2024-05-22 11:24:48.000000 mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2967 2024-05-22 11:24:33.000000 mapclassif_Iron-2.6.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-22 11:24:49.418424 mapclassif_Iron-2.6.3/setup.cfg
```

### Comparing `mapclassif_Iron-2.6.2/LICENSE.txt` & `mapclassif_Iron-2.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapclassif_Iron-2.6.2/PKG-INFO` & `mapclassif_Iron-2.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapclassif_Iron
-Version: 2.6.2
+Version: 2.6.3
 Summary: Classification Schemes for Choropleth Maps.
 Maintainer-email: James Parrott <james.parrott@proton.me>
 License: BSD 3-Clause
 Project-URL: Repository, https://github.com/JamesParrott/mapclassif-Iron
 Keywords: spatial statistics,geovisualizaiton
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mapclassif_Iron-2.6.2/README.md` & `mapclassif_Iron-2.6.3/README.md`

 * *Files identical despite different names*

### Comparing `mapclassif_Iron-2.6.2/mapclassif_Iron/classifiers.py` & `mapclassif_Iron-2.6.3/mapclassif_Iron/classifiers.py`

 * *Files identical despite different names*

### Comparing `mapclassif_Iron-2.6.2/mapclassif_Iron/test_fisher_jenks_means.py` & `mapclassif_Iron-2.6.3/mapclassif_Iron/test_fisher_jenks_means.py`

 * *Files identical despite different names*

### Comparing `mapclassif_Iron-2.6.2/mapclassif_Iron.egg-info/PKG-INFO` & `mapclassif_Iron-2.6.3/mapclassif_Iron.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapclassif-Iron
-Version: 2.6.2
+Version: 2.6.3
 Summary: Classification Schemes for Choropleth Maps.
 Maintainer-email: James Parrott <james.parrott@proton.me>
 License: BSD 3-Clause
 Project-URL: Repository, https://github.com/JamesParrott/mapclassif-Iron
 Keywords: spatial statistics,geovisualizaiton
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
```

### Comparing `mapclassif_Iron-2.6.2/pyproject.toml` & `mapclassif_Iron-2.6.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapclassif_Iron"
-version="2.6.2"
+version="2.6.3"
 maintainers = [
     {name = "James Parrott", email = "james.parrott@proton.me"},
 ]
 license = {text = "BSD 3-Clause"}
 description = "Classification Schemes for Choropleth Maps."
 keywords = ["spatial statistics", "geovisualizaiton"]
 readme = {text = """\
@@ -56,16 +56,16 @@
 include = [
     "mapclassif_Iron",
     "mapclassif_Iron.*",
 ]
 
 [tool.setuptools.package-data]
 mapclassif_Iron = [
-    "mapclassif_Iron/datasets/calemp/calempdensity.csv",
-    "mapclassif_Iron/datasets/calemp/README.md",
+    "datasets/calemp/calempdensity.csv",
+    "datasets/calemp/README.md",
 ]
 
 [tool.black]
 line-length = 88
 extend-exclude = '''
 (
   docs/conf.py
```

