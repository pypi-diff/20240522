# Comparing `tmp/fspathtree-0.8.tar.gz` & `tmp/fspathtree-0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fspathtree-0.8.tar", max compression
+gzip compressed data, was "fspathtree-0.9.tar", max compression
```

## Comparing `fspathtree-0.8.tar` & `fspathtree-0.9.tar`

### file list

```diff
@@ -1,7 +1,6 @@
--rw-r--r--   0        0        0     1071 2022-11-27 14:10:28.294571 fspathtree-0.8/LICENSE.txt
--rw-r--r--   0        0        0     1806 2020-08-23 16:31:58.683439 fspathtree-0.8/README.md
--rw-r--r--   0        0        0       26 2020-08-23 16:16:57.157174 fspathtree-0.8/fspathtree/__init__.py
--rw-r--r--   0        0        0    16357 2023-03-08 13:11:23.660002 fspathtree-0.8/fspathtree/fspathtree.py
--rw-r--r--   0        0        0      495 2023-03-08 13:21:15.112423 fspathtree-0.8/pyproject.toml
--rw-r--r--   0        0        0     2540 1970-01-01 00:00:00.000000 fspathtree-0.8/setup.py
--rw-r--r--   0        0        0     2488 1970-01-01 00:00:00.000000 fspathtree-0.8/PKG-INFO
+-rw-r--r--   0        0        0     1071 2022-11-27 14:10:28.294571 fspathtree-0.9/LICENSE.txt
+-rw-r--r--   0        0        0     3051 2024-05-22 15:17:52.547266 fspathtree-0.9/README.md
+-rw-r--r--   0        0        0       26 2020-08-23 16:16:57.157174 fspathtree-0.9/fspathtree/__init__.py
+-rw-r--r--   0        0        0    19525 2024-05-22 15:07:49.882548 fspathtree-0.9/fspathtree/fspathtree.py
+-rw-r--r--   0        0        0      495 2024-05-22 15:20:21.179174 fspathtree-0.9/pyproject.toml
+-rw-r--r--   0        0        0     3784 1970-01-01 00:00:00.000000 fspathtree-0.9/PKG-INFO
```

### Comparing `fspathtree-0.8/LICENSE.txt` & `fspathtree-0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fspathtree-0.8/PKG-INFO` & `fspathtree-0.9/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: fspathtree
-Version: 0.8
-Summary: A small utility for wrapping trees (nested dict/list) that allows filesystem-like path access, including walking up with "../".
-License: MIT
-Author: CD Clark III
-Author-email: clifton.clark@gmail.com
-Requires-Python: >=3.7,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Description-Content-Type: text/markdown
-
 # FS Path Tree
 
 A simple class to allow filesystem-style path access to nested dict/list structures,
 including support for walking "up" the tree with '..'.
 
 Example:
 
@@ -50,24 +33,65 @@
   assert x['max'] == 0.5
   # but we can also access elements that are not in this branch.
   assert x['../y/max'] == 1.5
   # or reference elements from the root of the tree.
   assert x['/time/N'] == 50
 ```
 
+## API
+
+The `fspathtree` class can be default constructed, with a `dict`, or with another `fspathtree`
+```python
+t1 = fspathtree()
+t2 = fspathtree({'one':1})
+t3 = fspathtree(t2)
+```
+
+Elements in the tree can be tested for presense using the `in` operator. They can be accessed with the
+`__call__` operator or the `get(...)` method.
+```
+t = fspathtree({'one':{'two': 2}})
+
+assert '/one/two' in t
+assert t['/one/two'] == 2
+assert '/one/three' not in t
+
+t['/one/three'] = 3
+assert '/one/three' in t
+assert t['/one/three'] == 3
+
+assert t.get('/one/three', None) == 3
+assert t.get('/one/missing', None) is None
+```
+The `get_all_paths()` method returns a list of all paths in the tree (it actually returns a generator).
+`get_all_leaf_node_paths()` returns a list of only leaf node paths. Both accept a predicate that can
+be used to filer the paths that are returned.
+```python
+t = fspathtree({'one':{'two': 2}})
+
+paths = list( t.get_all_paths() ) # returns [PathType('/'), PathType('/one'), PathType('two')]
+paths = list( t.get_all_leafe_node_paths() ) # returns [PathType('two')]
+paths = list( t.get_all_paths(predicate p: p.name == 'one') ) # returns [ PathType('/one')]
+
+```
+
+
 ## Install
 
 You can install the latest release with `pip`.
 ```
 $ pip install fspathtree
 ```
 Or, even better, using `pipenv`
 ```
 $ pipenv install fspathtree
 ```
+Or, even better better, using `poetry`
+```
+$ poetry add fspathtree
+```
 
 ## Design
 
 The `fspathtree` is a small wrapper class that can wrap any nested tree data structure. The tree that is wrapped can be accessed with
 the `.tree` attribute. This is an improvement over the old `fspathdict.pdict` class, which stored nodes internally as `fspathdict.pdict` instances
 and required "converting" to and from the standard python dict and list types.
-
```

