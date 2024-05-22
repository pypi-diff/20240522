# Comparing `tmp/apeer-ometiff-library-1.8.3.tar.gz` & `tmp/apeer-ometiff-library-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/apeer-ometiff-library-1.8.3.tar", last modified: Fri May 13 07:52:23 2022, max compression
+gzip compressed data, was "dist/apeer-ometiff-library-1.9.0.tar", last modified: Thu May 19 10:42:17 2022, max compression
```

## Comparing `apeer-ometiff-library-1.8.3.tar` & `apeer-ometiff-library-1.9.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/
--rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library/__init__.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)     6063 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library/io.py
--rwxr-xr-x   0 vsts      (1001) docker     (121)    52721 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library/omexmlClass.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library/processing.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-05-13 07:52:22.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)      420 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-13 07:52:22.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-13 07:52:22.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-05-13 07:52:22.000000 apeer-ometiff-library-1.8.3/apeer_ometiff_library.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)      550 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-13 07:52:23.000000 apeer-ometiff-library-1.8.3/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-05-13 07:51:58.000000 apeer-ometiff-library-1.8.3/tests/test_processing.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      537 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library/__init__.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     7532 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library/io.py
+-rwxr-xr-x   0 vsts      (1001) docker     (121)    52721 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library/omexmlClass.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1473 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library/processing.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)      419 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)      437 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       15 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       28 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/apeer_ometiff_library.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)       38 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (121)      550 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-05-19 10:42:17.000000 apeer-ometiff-library-1.9.0/tests/
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5056 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/tests/test_io.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      379 2022-05-19 10:41:58.000000 apeer-ometiff-library-1.9.0/tests/test_processing.py
```

### Comparing `apeer-ometiff-library-1.8.3/README.md` & `apeer-ometiff-library-1.9.0/README.md`

 * *Files identical despite different names*

### Comparing `apeer-ometiff-library-1.8.3/apeer_ometiff_library/omexmlClass.py` & `apeer-ometiff-library-1.9.0/apeer_ometiff_library/omexmlClass.py`

 * *Files identical despite different names*

### Comparing `apeer-ometiff-library-1.8.3/apeer_ometiff_library/processing.py` & `apeer-ometiff-library-1.9.0/apeer_ometiff_library/processing.py`

 * *Files identical despite different names*

### Comparing `apeer-ometiff-library-1.8.3/setup.py` & `apeer-ometiff-library-1.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 from setuptools import setup
 
 setup(name='apeer-ometiff-library',
-      version='1.8.3',
+      version='1.9.0',
       description='Library to read and write ometiff images',
       url='https://github.com/apeer-micro/apeer-ometiff-library',
       author='apeer-micro',
       packages=setuptools.find_packages(),
       install_requires=['numpy','tifffile'],
       license='MIT',
       classifiers=[
```

