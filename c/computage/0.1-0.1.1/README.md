# Comparing `tmp/computage-0.1.tar.gz` & `tmp/computage-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "computage-0.1.tar", last modified: Wed May 22 12:56:11 2024, max compression
+gzip compressed data, was "computage-0.1.1.tar", last modified: Wed May 22 15:50:28 2024, max compression
```

## Comparing `computage-0.1.tar` & `computage-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 12:56:11.792827 computage-0.1/
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)    20137 2024-05-22 11:06:16.000000 computage-0.1/LICENSE
--rw-r--r--   0 dkriukov  (1013) dkriukov  (1013)      382 2024-05-22 12:56:11.792827 computage-0.1/PKG-INFO
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)     2683 2024-05-22 11:52:30.000000 computage-0.1/README.md
-drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 12:56:11.792827 computage-0.1/computage/
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       60 2024-05-22 12:45:05.000000 computage-0.1/computage/__init__.py
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       45 2024-05-22 10:56:40.000000 computage-0.1/computage/settings.py
-drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 12:56:11.792827 computage-0.1/computage.egg-info/
--rw-r--r--   0 dkriukov  (1013) dkriukov  (1013)      382 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/PKG-INFO
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)      276 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/SOURCES.txt
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)        1 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/dependency_links.txt
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)        1 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/not-zip-safe
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       76 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/requires.txt
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       10 2024-05-22 12:56:11.000000 computage-0.1/computage.egg-info/top_level.txt
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       38 2024-05-22 12:56:11.792827 computage-0.1/setup.cfg
--rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)      450 2024-05-22 12:21:13.000000 computage-0.1/setup.py
+drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 15:50:28.758072 computage-0.1.1/
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)    20137 2024-05-22 11:06:16.000000 computage-0.1.1/LICENSE
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)      233 2024-05-22 15:50:28.758072 computage-0.1.1/PKG-INFO
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)     2716 2024-05-22 13:30:55.000000 computage-0.1.1/README.md
+drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 15:50:28.758072 computage-0.1.1/computage/
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       60 2024-05-22 12:45:05.000000 computage-0.1.1/computage/__init__.py
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       45 2024-05-22 10:56:40.000000 computage-0.1.1/computage/settings.py
+drwxrwxr-x   0 dkriukov  (1013) dkriukov  (1013)        0 2024-05-22 15:50:28.758072 computage-0.1.1/computage.egg-info/
+-rw-r--r--   0 dkriukov  (1013) dkriukov  (1013)      233 2024-05-22 15:50:28.000000 computage-0.1.1/computage.egg-info/PKG-INFO
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)      276 2024-05-22 15:50:28.000000 computage-0.1.1/computage.egg-info/SOURCES.txt
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)        1 2024-05-22 15:50:28.000000 computage-0.1.1/computage.egg-info/dependency_links.txt
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)        1 2024-05-22 12:56:11.000000 computage-0.1.1/computage.egg-info/not-zip-safe
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       94 2024-05-22 15:50:28.000000 computage-0.1.1/computage.egg-info/requires.txt
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       10 2024-05-22 15:50:28.000000 computage-0.1.1/computage.egg-info/top_level.txt
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)       38 2024-05-22 15:50:28.758072 computage-0.1.1/setup.cfg
+-rw-rw-r--   0 dkriukov  (1013) dkriukov  (1013)      493 2024-05-22 15:50:18.000000 computage-0.1.1/setup.py
```

### Comparing `computage-0.1/LICENSE` & `computage-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `computage-0.1/README.md` & `computage-0.1.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # ComputAge
-A library for fullstack aging clocks design and benchmarking.
+A library for full-stack aging clocks design and benchmarking.
 
 *The full release version of the package is currently developing. Only bechmarking module is released and ready for use. Please see below.*
 
 ## Installation
 
 
 
@@ -35,14 +35,18 @@
 <em>ComputAgeBench epigenetic clock construction overview.</em>
 </p>
 
 ## Usage (benchmarking)
 
 
 
+## Reproducing paper results
+
+
+
 ## Cite us
 
 
 
 ## Contact
 
 For any questions or clarifications, please reach out to: dmitrii.kriukov@skoltech.ru
```

