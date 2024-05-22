# Comparing `tmp/nnz-0.0.1.tar.gz` & `tmp/nnz-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnz-0.0.1.tar", last modified: Sun Apr 28 15:49:55 2024, max compression
+gzip compressed data, was "nnz-0.0.2.tar", last modified: Wed May 22 07:37:43 2024, max compression
```

## Comparing `nnz-0.0.1.tar` & `nnz-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-28 15:49:55.973444 nnz-0.0.1/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2385 2024-04-28 15:42:33.000000 nnz-0.0.1/LICENCE
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      507 2024-04-28 15:49:55.973444 nnz-0.0.1/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       12 2024-04-28 15:43:16.000000 nnz-0.0.1/README.md
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      584 2024-04-28 15:45:49.000000 nnz-0.0.1/pyproject.toml
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-28 15:49:55.973444 nnz-0.0.1/setup.cfg
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-28 15:49:55.969444 nnz-0.0.1/src/
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-28 15:49:55.969444 nnz-0.0.1/src/nnz/
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       71 2024-04-28 15:36:58.000000 nnz-0.0.1/src/nnz/__init__.py
-drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-28 15:49:55.973444 nnz-0.0.1/src/nnz.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      507 2024-04-28 15:49:55.000000 nnz-0.0.1/src/nnz.egg-info/PKG-INFO
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      176 2024-04-28 15:49:55.000000 nnz-0.0.1/src/nnz.egg-info/SOURCES.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-28 15:49:55.000000 nnz-0.0.1/src/nnz.egg-info/dependency_links.txt
--rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        4 2024-04-28 15:49:55.000000 nnz-0.0.1/src/nnz.egg-info/top_level.txt
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-22 07:37:43.234638 nnz-0.0.2/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2385 2024-04-28 16:26:35.000000 nnz-0.0.2/LICENCE
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      645 2024-05-22 07:37:43.234638 nnz-0.0.2/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        9 2024-04-28 16:27:01.000000 nnz-0.0.2/README.md
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      653 2024-05-04 14:11:24.000000 nnz-0.0.2/pyproject.toml
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       38 2024-05-22 07:37:43.234638 nnz-0.0.2/setup.cfg
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-22 07:37:43.234638 nnz-0.0.2/src/
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-22 07:37:43.234638 nnz-0.0.2/src/nnz/
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     4064 2024-05-20 08:49:39.000000 nnz-0.0.2/src/nnz/__init__.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       43 2024-04-28 19:48:03.000000 nnz-0.0.2/src/nnz/config.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)    32888 2024-05-16 15:05:42.000000 nnz-0.0.2/src/nnz/dataset.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      117 2024-05-16 08:30:33.000000 nnz-0.0.2/src/nnz/modeling.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     2611 2024-05-07 12:00:06.000000 nnz-0.0.2/src/nnz/tools.py
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)     9449 2024-05-22 07:24:46.000000 nnz-0.0.2/src/nnz/workspace.py
+drwxrwxr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-05-22 07:37:43.234638 nnz-0.0.2/src/nnz.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      645 2024-05-22 07:37:43.000000 nnz-0.0.2/src/nnz.egg-info/PKG-INFO
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)      301 2024-05-22 07:37:43.000000 nnz-0.0.2/src/nnz.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        1 2024-05-22 07:37:43.000000 nnz-0.0.2/src/nnz.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)       51 2024-05-22 07:37:43.000000 nnz-0.0.2/src/nnz.egg-info/requires.txt
+-rw-rw-r--   0 jeremy    (1000) jeremy    (1000)        4 2024-05-22 07:37:43.000000 nnz-0.0.2/src/nnz.egg-info/top_level.txt
```

### Comparing `nnz-0.0.1/LICENCE` & `nnz-0.0.2/LICENCE`

 * *Files identical despite different names*

### Comparing `nnz-0.0.1/pyproject.toml` & `nnz-0.0.2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [build-system]
 requires = ["setuptools>=69.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "nnz"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="THULLIEZ Jeremy", email="j.thulliez@gmail.com" },
 ]
 description = "A small example package for datascience"
 readme = "README.md"
 requires-python = ">=3.12"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
-
+  "keras", "torch", "matplotlib", "scikit-learn", "pandas", "seaborn"
 ]
 
 [project.urls]
 Homepage = "https://github.com/JeremZed/NN"
 Issues = "https://github.com/JeremZed/NN/issues"
```

