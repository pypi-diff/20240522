# Comparing `tmp/elements-3.5.0.tar.gz` & `tmp/elements-3.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.5.0.tar", last modified: Mon May 20 19:05:33 2024, max compression
+gzip compressed data, was "elements-3.6.0.tar", last modified: Wed May 22 05:34:49 2024, max compression
```

## Comparing `elements-3.5.0.tar` & `elements-3.6.0.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.913949 elements-3.5.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.5.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.5.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-20 19:05:33.913949 elements-3.5.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.5.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.909949 elements-3.5.0/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-20 19:03:34.000000 elements-3.5.0/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.5.0/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-20 19:03:19.000000 elements-3.5.0/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.5.0/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.5.0/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.5.0/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.5.0/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.5.0/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7702 2024-05-16 00:32:50.000000 elements-3.5.0/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.5.0/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.5.0/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.5.0/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.5.0/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.5.0/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.5.0/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.5.0/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.5.0/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.5.0/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.909949 elements-3.5.0/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-20 19:05:33.000000 elements-3.5.0/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.5.0/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.5.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-20 19:05:33.913949 elements-3.5.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.5.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-20 19:05:33.913949 elements-3.5.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.5.0/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.5.0/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.5.0/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-14 17:33:06.000000 elements-3.5.0/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.5.0/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.0/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.0/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:34:49.930481 elements-3.6.0/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.0/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 05:34:10.000000 elements-3.6.0/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.0/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3992 2024-05-22 05:34:03.000000 elements-3.6.0/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.0/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.0/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.0/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.0/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.0/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11477 2024-05-22 05:34:20.000000 elements-3.6.0/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.0/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.0/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.0/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.0/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.0/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.0/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.0/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.0/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.0/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.0/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.0/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 05:34:49.930481 elements-3.6.0/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.0/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.0/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.0/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.0/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-22 05:33:39.000000 elements-3.6.0/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.0/tests/test_tree.py
```

### Comparing `elements-3.5.0/LICENSE` & `elements-3.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/PKG-INFO` & `elements-3.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.5.0
+Version: 3.6.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.5.0/README.md` & `elements-3.6.0/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/agg.py` & `elements-3.6.0/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/checkpoint.py` & `elements-3.6.0/elements/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
       self._promise = self._worker.submit(self._save, filename, data)
     else:
       self._save(filename, data)
 
   @timer.section('checkpoint_save')
   def _save(self, filename, data):
     data['_timestamp'] = time.time()
-    filename.parent.mkdirs()
+    filename.parent.mkdir()
     content = pickle.dumps(data)
     if str(filename).startswith('gs://'):
       filename.write(content, mode='wb')
     else:
       # Write to a temporary file and then atomically rename, so that the file
       # either contains a complete write or not update at all if writing was
       # interrupted.
```

### Comparing `elements-3.5.0/elements/config.py` & `elements-3.6.0/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/counter.py` & `elements-3.6.0/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/flags.py` & `elements-3.6.0/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/logger.py` & `elements-3.6.0/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/plotting.py` & `elements-3.6.0/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/printing.py` & `elements-3.6.0/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/rwlock.py` & `elements-3.6.0/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/timer.py` & `elements-3.6.0/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/tree.py` & `elements-3.6.0/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/usage.py` & `elements-3.6.0/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/uuid.py` & `elements-3.6.0/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements/when.py` & `elements-3.6.0/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/elements.egg-info/PKG-INFO` & `elements-3.6.0/elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.5.0
+Version: 3.6.0
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.5.0/elements.egg-info/SOURCES.txt` & `elements-3.6.0/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/setup.py` & `elements-3.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/tests/test_basics.py` & `elements-3.6.0/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/tests/test_checkpoint.py` & `elements-3.6.0/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/tests/test_flags.py` & `elements-3.6.0/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/tests/test_path.py` & `elements-3.6.0/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.5.0/tests/test_tree.py` & `elements-3.6.0/tests/test_tree.py`

 * *Files identical despite different names*

