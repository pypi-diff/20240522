# Comparing `tmp/code_diff_review-1.0.0.tar.gz` & `tmp/code_diff_review-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "code_diff_review-1.0.0.tar", last modified: Wed May 22 16:38:24 2024, max compression
+gzip compressed data, was "code_diff_review-1.2.0.tar", last modified: Wed May 22 16:52:09 2024, max compression
```

## Comparing `code_diff_review-1.0.0.tar` & `code_diff_review-1.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:38:24.449857 code_diff_review-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:38:24.445857 code_diff_review-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:38:24.445857 code_diff_review-1.0.0/code_diff_review.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 16:38:24.000000 code_diff_review-1.0.0/code_diff_review.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:38:24.449857 code_diff_review-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:38:24.445857 code_diff_review-1.0.0/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/src/publishers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3192 2024-05-22 16:38:19.000000 code_diff_review-1.0.0/src/script.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4047 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/code_diff_review.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4739 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      358 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-05-22 16:52:09.000000 code_diff_review-1.2.0/code_diff_review.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:09.233385 code_diff_review-1.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3548 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/publishers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3193 2024-05-22 16:52:04.000000 code_diff_review-1.2.0/src/script.py
```

### Comparing `code_diff_review-1.0.0/LICENSE` & `code_diff_review-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.0.0/PKG-INFO` & `code_diff_review-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.0.0
+Version: 1.2.0
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.0.0/README.md` & `code_diff_review-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.0.0/code_diff_review.egg-info/PKG-INFO` & `code_diff_review-1.2.0/code_diff_review.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: code-diff-review
-Version: 1.0.0
+Version: 1.2.0
 Summary: Review your code diff.
 Author: Agustin Rios
 Author-email: arios6@uc.cl
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `code_diff_review-1.0.0/setup.py` & `code_diff_review-1.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='code-diff-review',
-    version='1.0.0',
+    version='1.2.0',
     author='Agustin Rios',
     author_email='arios6@uc.cl',
     description='Review your code diff.',
     long_description=open('README.md').read() + '\n\n' + open('CHANGELOG.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=open("./requirements.txt").read().splitlines(),
```

### Comparing `code_diff_review-1.0.0/src/publishers.py` & `code_diff_review-1.2.0/src/publishers.py`

 * *Files identical despite different names*

### Comparing `code_diff_review-1.0.0/src/script.py` & `code_diff_review-1.2.0/src/script.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 import json
 import subprocess
 import argparse
-from publishers import GitIssuePublisher, WebPublisher
+from .publishers import GitIssuePublisher, WebPublisher
 
 def extract_message(text):
     pattern = r'\[C:START\](.*?)\[C:END\]'
     matcher = re.search(pattern, text, re.DOTALL)
     if matcher:
         return matcher.group(1)
     return None
```

