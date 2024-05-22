# Comparing `tmp/lam-cli-0.0.5.tar.gz` & `tmp/lam_cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lam-cli-0.0.5.tar", last modified: Sun Mar 10 14:59:39 2024, max compression
+gzip compressed data, was "lam_cli-0.0.6.tar", last modified: Wed May 22 21:01:58 2024, max compression
```

## Comparing `lam-cli-0.0.5.tar` & `lam_cli-0.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:59:39.399495 lam-cli-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-03-10 14:59:32.000000 lam-cli-0.0.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-10 14:59:39.399495 lam-cli-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-03-10 14:59:32.000000 lam-cli-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:59:39.395494 lam-cli-0.0.5/lam/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-10 14:59:32.000000 lam-cli-0.0.5/lam/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5843 2024-03-10 14:59:32.000000 lam-cli-0.0.5/lam/lam.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 14:59:39.395494 lam-cli-0.0.5/lam_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      374 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-10 14:59:39.000000 lam-cli-0.0.5/lam_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-10 14:59:39.399495 lam-cli-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-03-10 14:59:32.000000 lam-cli-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (127)    35148 2024-05-22 21:01:54.000000 lam_cli-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 21:01:58.058709 lam_cli-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1844 2024-05-22 21:01:54.000000 lam_cli-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/lam/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:54.000000 lam_cli-0.0.6/lam/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     7269 2024-05-22 21:01:54.000000 lam_cli-0.0.6/lam/lam.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 21:01:58.058709 lam_cli-0.0.6/lam_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 21:01:58.000000 lam_cli-0.0.6/lam_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 21:01:58.058709 lam_cli-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-05-22 21:01:54.000000 lam_cli-0.0.6/setup.py
```

### Comparing `lam-cli-0.0.5/LICENSE` & `lam_cli-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lam-cli-0.0.5/setup.py` & `lam_cli-0.0.6/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import find_packages, setup
 
 setup(
     name='lam-cli',
-    version='0.0.5',
+    version='0.0.6',
     packages=find_packages(),
     install_requires=[
         'click',
         'posthog',
+        'logtail-python',
     ],
     entry_points={
         'console_scripts': [
             'lam=lam.lam:lam',
         ],
     },
     license='GPLv3',
```

