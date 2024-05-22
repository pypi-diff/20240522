# Comparing `tmp/VeriFact-0.0.1.tar.gz` & `tmp/verifact-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/VeriFact-0.0.1.tar", last modified: Tue May 21 18:29:27 2024, max compression
+gzip compressed data, was "verifact-0.0.2.tar", last modified: Wed May 22 17:59:10 2024, max compression
```

## Comparing `VeriFact-0.0.1.tar` & `verifact-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-21 18:29:27.000000 VeriFact-0.0.1/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 VeriFact-0.0.1/LICENSE
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      430 2024-05-21 18:29:27.000000 VeriFact-0.0.1/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 VeriFact-0.0.1/README.md
-drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-21 18:29:27.000000 VeriFact-0.0.1/VeriFact.egg-info/
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      430 2024-05-21 18:29:27.000000 VeriFact-0.0.1/VeriFact.egg-info/PKG-INFO
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      154 2024-05-21 18:29:27.000000 VeriFact-0.0.1/VeriFact.egg-info/SOURCES.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-21 18:29:27.000000 VeriFact-0.0.1/VeriFact.egg-info/dependency_links.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-21 18:29:27.000000 VeriFact-0.0.1/VeriFact.egg-info/top_level.txt
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-21 18:29:27.000000 VeriFact-0.0.1/setup.cfg
--rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      618 2024-05-21 17:56:52.000000 VeriFact-0.0.1/setup.py
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 17:59:10.262805 verifact-0.0.2/
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)     1068 2024-05-21 17:48:27.000000 verifact-0.0.2/LICENSE
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 17:59:10.262805 verifact-0.0.2/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       11 2024-05-21 17:48:27.000000 verifact-0.0.2/README.md
+drwxrwxr-x   0 yekyungkim (32790) yekyungkim (32790)        0 2024-05-22 17:59:10.262805 verifact-0.0.2/VeriFact.egg-info/
+-rw-r--r--   0 yekyungkim (32790) yekyungkim (32790)      521 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/PKG-INFO
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      185 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/SOURCES.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/dependency_links.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       31 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/requires.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)        1 2024-05-22 17:59:10.000000 verifact-0.0.2/VeriFact.egg-info/top_level.txt
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)       38 2024-05-22 17:59:10.262805 verifact-0.0.2/setup.cfg
+-rw-rw-r--   0 yekyungkim (32790) yekyungkim (32790)      684 2024-05-22 17:57:47.000000 verifact-0.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `VeriFact-0.0.1/LICENSE` & `verifact-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `VeriFact-0.0.1/setup.py` & `verifact-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 from setuptools import setup, find_packages
 
 setup(
    name="VeriFact",
-   version="0.0.1",
+   version="0.0.2",
    packages=find_packages(),
    install_requires=[
        #'requests', 'numpy'
+      'openai',
+      'anthropic',
+      'tiktoken',
+      'tqdm'
    ],
    author="Yixio Song",
    author_email="yixiaosong@umass.edu",
    description="Pip package for Verifact",
    long_description=open('README.md').read(),
    long_description_content_type="text/markdown",
    url="https://github.com/mungg/VeriScore",
```

