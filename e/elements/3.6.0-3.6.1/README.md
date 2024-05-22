# Comparing `tmp/elements-3.6.0.tar.gz` & `tmp/elements-3.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.6.0.tar", last modified: Wed May 22 05:34:49 2024, max compression
+gzip compressed data, was "elements-3.6.1.tar", last modified: Wed May 22 05:36:19 2024, max compression
```

## Comparing `elements-3.6.0.tar` & `elements-3.6.1.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.0/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.0/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:34:49.930481 elements-3.6.0/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.0/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 05:34:10.000000 elements-3.6.0/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.0/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3992 2024-05-22 05:34:03.000000 elements-3.6.0/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.0/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.0/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.0/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.0/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.0/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    11477 2024-05-22 05:34:20.000000 elements-3.6.0/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.0/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.0/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.0/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.0/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.0/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.0/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.0/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.0/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.0/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 05:34:49.000000 elements-3.6.0/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.0/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.0/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 05:34:49.930481 elements-3.6.0/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.0/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:34:49.930481 elements-3.6.0/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.0/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.0/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.0/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-22 05:33:39.000000 elements-3.6.0/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.0/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.1/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.1/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:36:19.486392 elements-3.6.1/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.1/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 05:36:08.000000 elements-3.6.1/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.1/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 05:36:04.000000 elements-3.6.1/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.1/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.1/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.1/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.1/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.1/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11483 2024-05-22 05:36:01.000000 elements-3.6.1/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.1/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.1/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.1/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.1/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.1/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.1/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.1/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.1/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.1/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.1/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.1/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 05:36:19.486392 elements-3.6.1/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.1/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.1/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.1/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.1/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-22 05:33:39.000000 elements-3.6.1/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.1/tests/test_tree.py
```

### Comparing `elements-3.6.0/LICENSE` & `elements-3.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/PKG-INFO` & `elements-3.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.0
+Version: 3.6.1
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.0/README.md` & `elements-3.6.1/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/__init__.py` & `elements-3.6.1/elements/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.6.0'
+__version__ = '3.6.1'
 
 from .agg import Agg
 from .checkpoint import Checkpoint, Saveable
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.6.0/elements/agg.py` & `elements-3.6.1/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/checkpoint.py` & `elements-3.6.1/elements/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -85,15 +85,15 @@
       self._promise = self._worker.submit(self._save, filename, data)
     else:
       self._save(filename, data)
 
   @timer.section('checkpoint_save')
   def _save(self, filename, data):
     data['_timestamp'] = time.time()
-    filename.parent.mkdir()
+    filename.parent.mkdirs()
     content = pickle.dumps(data)
     if str(filename).startswith('gs://'):
       filename.write(content, mode='wb')
     else:
       # Write to a temporary file and then atomically rename, so that the file
       # either contains a complete write or not update at all if writing was
       # interrupted.
```

### Comparing `elements-3.6.0/elements/config.py` & `elements-3.6.1/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/counter.py` & `elements-3.6.1/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/flags.py` & `elements-3.6.1/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/logger.py` & `elements-3.6.1/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/path.py` & `elements-3.6.1/elements/path.py`

 * *Files 1% similar despite different names*

```diff
@@ -99,15 +99,15 @@
 
   def isfile(self):
     raise NotImplementedError
 
   def isdir(self):
     raise NotImplementedError
 
-  def mkdir(self):
+  def mkdirs(self):
     raise NotImplementedError
 
   def remove(self, recursive=False):
     raise NotImplementedError
 
   def copy(self, dest, recursive=False):
     raise NotImplementedError
@@ -141,15 +141,15 @@
 
   def isfile(self):
     return os.path.isfile(str(self))
 
   def isdir(self):
     return os.path.isdir(str(self))
 
-  def mkdir(self):
+  def mkdirs(self):
     os.makedirs(str(self), exist_ok=True)
 
   def remove(self, recursive=True):
     if recursive:
       shutil.rmtree(self)
     else:
       os.rmdir(str(self)) if self.isdir() else os.remove(str(self))
@@ -204,15 +204,15 @@
 
   def isfile(self):
     return self.exists() and not self.isdir()
 
   def isdir(self):
     return self.gfile.isdir(str(self))
 
-  def mkdir(self):
+  def mkdirs(self):
     self.gfile.makedirs(str(self))
 
   def remove(self, recursive=False):
     if recursive:
       self.gfile.rmtree(str(self))
     else:
       self.gfile.remove(str(self))
@@ -220,26 +220,26 @@
   def copy(self, dest, recursive=False):
     dest = Path(dest)
     if not recursive:
       self.gfile.copy(str(self), str(dest), overwrite=True)
       return
     for folder, subdirs, files in self.gfile.walk(str(self)):
       target = type(self)(folder.replace(str(self), str(dest)))
-      target.exists() or target.mkdir()
+      target.exists() or target.mkdirs()
       for file in files:
         (type(self)(folder) / file).copy(target / file)
 
   def move(self, dest, recursive=False):
     dest = Path(dest)
     if recursive:
       self.gfile.rename(self, str(dest), overwrite=True)
       return
     for folder, subdirs, files in self.gfile.walk(str(self)):
       target = type(self)(folder.replace(str(self), str(dest)))
-      target.exists() or target.mkdir()
+      target.exists() or target.mkdirs()
       for file in files:
         (type(self)(folder) / file).move(target / file)
 
 
 class GCSPath(Path):
 
   __slots__ = ('_path', '_blob')
@@ -366,15 +366,15 @@
       return True
     try:
       next(iter(self.glob('*')))
       return True
     except StopIteration:
       return False
 
-  def mkdir(self):
+  def mkdirs(self):
     from google.cloud import storage
     if not self.blob:
       return
     if self.exists():
       return
     folder = storage.Blob(self.blob.name + '/', self.bucket)
     folder.upload_from_string(b'')
```

### Comparing `elements-3.6.0/elements/plotting.py` & `elements-3.6.1/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/printing.py` & `elements-3.6.1/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/rwlock.py` & `elements-3.6.1/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/timer.py` & `elements-3.6.1/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/tree.py` & `elements-3.6.1/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/usage.py` & `elements-3.6.1/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/uuid.py` & `elements-3.6.1/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements/when.py` & `elements-3.6.1/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/elements.egg-info/PKG-INFO` & `elements-3.6.1/elements.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.0
+Version: 3.6.1
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.0/elements.egg-info/SOURCES.txt` & `elements-3.6.1/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/setup.py` & `elements-3.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/tests/test_basics.py` & `elements-3.6.1/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/tests/test_checkpoint.py` & `elements-3.6.1/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/tests/test_flags.py` & `elements-3.6.1/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/tests/test_path.py` & `elements-3.6.1/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.0/tests/test_tree.py` & `elements-3.6.1/tests/test_tree.py`

 * *Files identical despite different names*

