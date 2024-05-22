# Comparing `tmp/elements-3.6.1.tar.gz` & `tmp/elements-3.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elements-3.6.1.tar", last modified: Wed May 22 05:36:19 2024, max compression
+gzip compressed data, was "elements-3.6.3.tar", last modified: Wed May 22 05:55:28 2024, max compression
```

## Comparing `elements-3.6.1.tar` & `elements-3.6.3.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.1/LICENSE
--rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.1/MANIFEST.in
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:36:19.486392 elements-3.6.1/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.1/README.md
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/elements/
--rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 05:36:08.000000 elements-3.6.1/elements/__init__.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.1/elements/agg.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 05:36:04.000000 elements-3.6.1/elements/checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.1/elements/config.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.1/elements/counter.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.1/elements/flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.1/elements/fps.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.1/elements/logger.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)    11483 2024-05-22 05:36:01.000000 elements-3.6.1/elements/path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.1/elements/plotting.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.1/elements/printing.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.1/elements/rwlock.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.1/elements/timer.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.1/elements/tree.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.1/elements/usage.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.1/elements/utils.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.1/elements/uuid.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.1/elements/when.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/elements.egg-info/
--rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/PKG-INFO
--rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/SOURCES.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/dependency_links.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/requires.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 05:36:19.000000 elements-3.6.1/elements.egg-info/top_level.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.1/requirements-optional.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.1/requirements.txt
--rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 05:36:19.486392 elements-3.6.1/setup.cfg
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.1/setup.py
-drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:36:19.486392 elements-3.6.1/tests/
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.1/tests/test_basics.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.1/tests/test_checkpoint.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.1/tests/test_flags.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-22 05:33:39.000000 elements-3.6.1/tests/test_path.py
--rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.1/tests/test_tree.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:55:28.017465 elements-3.6.3/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1058 2023-12-10 19:43:58.000000 elements-3.6.3/LICENSE
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       59 2023-12-10 19:43:58.000000 elements-3.6.3/MANIFEST.in
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:55:28.017465 elements-3.6.3/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10443 2024-05-10 21:35:11.000000 elements-3.6.3/README.md
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:55:28.013466 elements-3.6.3/elements/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      551 2024-05-22 05:55:19.000000 elements-3.6.3/elements/__init__.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3540 2024-02-05 03:02:13.000000 elements-3.6.3/elements/agg.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3993 2024-05-22 05:55:14.000000 elements-3.6.3/elements/checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     5998 2024-02-05 02:06:54.000000 elements-3.6.3/elements/config.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      916 2023-12-10 19:47:36.000000 elements-3.6.3/elements/counter.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4211 2023-12-13 01:50:18.000000 elements-3.6.3/elements/flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      320 2023-12-10 19:43:58.000000 elements-3.6.3/elements/fps.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    12996 2024-02-06 00:22:22.000000 elements-3.6.3/elements/logger.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    11853 2024-05-22 05:55:12.000000 elements-3.6.3/elements/path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     6052 2023-12-10 19:43:58.000000 elements-3.6.3/elements/plotting.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     3169 2023-12-10 19:52:49.000000 elements-3.6.3/elements/printing.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1630 2023-12-10 19:47:10.000000 elements-3.6.3/elements/rwlock.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2847 2023-12-10 19:47:13.000000 elements-3.6.3/elements/timer.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1443 2024-05-10 21:58:03.000000 elements-3.6.3/elements/tree.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     7666 2023-12-10 19:47:25.000000 elements-3.6.3/elements/usage.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      228 2024-02-26 02:12:34.000000 elements-3.6.3/elements/utils.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2199 2023-12-10 19:54:08.000000 elements-3.6.3/elements/uuid.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1671 2023-12-10 19:47:30.000000 elements-3.6.3/elements/when.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:55:28.017465 elements-3.6.3/elements.egg-info/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)    10803 2024-05-22 05:55:27.000000 elements-3.6.3/elements.egg-info/PKG-INFO
+-rw-r-----   0 danijar  (322066) primarygroup (89939)      679 2024-05-22 05:55:27.000000 elements-3.6.3/elements.egg-info/SOURCES.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        1 2024-05-22 05:55:27.000000 elements-3.6.3/elements.egg-info/dependency_links.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-22 05:55:27.000000 elements-3.6.3/elements.egg-info/requires.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)        9 2024-05-22 05:55:27.000000 elements-3.6.3/elements.egg-info/top_level.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       53 2024-05-13 22:39:18.000000 elements-3.6.3/requirements-optional.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       66 2024-05-14 17:34:25.000000 elements-3.6.3/requirements.txt
+-rw-r-----   0 danijar  (322066) primarygroup (89939)       38 2024-05-22 05:55:28.017465 elements-3.6.3/setup.cfg
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1095 2023-12-10 20:02:30.000000 elements-3.6.3/setup.py
+drwxr-x---   0 danijar  (322066) primarygroup (89939)        0 2024-05-22 05:55:28.017465 elements-3.6.3/tests/
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2112 2024-05-20 18:51:09.000000 elements-3.6.3/tests/test_basics.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1889 2024-05-20 19:03:28.000000 elements-3.6.3/tests/test_checkpoint.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     4454 2023-12-13 01:48:36.000000 elements-3.6.3/tests/test_flags.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     1505 2024-05-22 05:33:39.000000 elements-3.6.3/tests/test_path.py
+-rw-r-----   0 danijar  (322066) primarygroup (89939)     2331 2024-05-10 22:02:36.000000 elements-3.6.3/tests/test_tree.py
```

### Comparing `elements-3.6.1/LICENSE` & `elements-3.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/PKG-INFO` & `elements-3.6.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.1
+Version: 3.6.3
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.1/README.md` & `elements-3.6.3/README.md`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/__init__.py` & `elements-3.6.3/elements/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '3.6.1'
+__version__ = '3.6.3'
 
 from .agg import Agg
 from .checkpoint import Checkpoint, Saveable
 from .config import Config
 from .counter import Counter
 from .flags import Flags
 from .fps import FPS
```

### Comparing `elements-3.6.1/elements/agg.py` & `elements-3.6.3/elements/agg.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/checkpoint.py` & `elements-3.6.3/elements/checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/config.py` & `elements-3.6.3/elements/config.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/counter.py` & `elements-3.6.3/elements/counter.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/flags.py` & `elements-3.6.3/elements/flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/logger.py` & `elements-3.6.3/elements/logger.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/path.py` & `elements-3.6.3/elements/path.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,27 +144,27 @@
 
   def isdir(self):
     return os.path.isdir(str(self))
 
   def mkdirs(self):
     os.makedirs(str(self), exist_ok=True)
 
-  def remove(self, recursive=True):
+  def remove(self, recursive=False):
     if recursive:
       shutil.rmtree(self)
     else:
       os.rmdir(str(self)) if self.isdir() else os.remove(str(self))
 
-  def copy(self, dest, recursive=True):
+  def copy(self, dest, recursive=False):
     if recursive:
       shutil.copytree(self, type(self)(dest), dirs_exist_ok=True)
     else:
       shutil.copy(self, type(self)(dest))
 
-  def move(self, dest, recursive=True):
+  def move(self, dest, recursive=False):
     shutil.move(self, dest)
 
 
 class TFPath(Path):
 
   __slots__ = ('_path',)
 
@@ -383,30 +383,42 @@
     if recursive:
       for child in self.glob('**'):
         child.remove()
     else:
       self.blob.delete(self.client)
 
   def move(self, dest, recursive=False):
+    dest = Path(dest)
+    notgcs = not str(dest).startswith('gs://')
     if recursive:
+      notgcs and dest.mkdirs()
       for child in self.glob('**'):
-        name = str(child).removeprefix(str(self))
-        child.move(dest / name)
+        name = str(child).removeprefix(str(self) + '/')
+        if child.isdir():
+          notgcs and dest.mkdirs()
+        else:
+          child.move(dest / name)
     elif self._bucket(dest) == self.bucket.name:
       dest = type(self)(dest)
       self.bucket.rename_blob(self.blob, dest.blob.name)
     else:
       self.copy(dest)
       self.remove()
 
-  def copy(self, dest, recursive=True):
+  def copy(self, dest, recursive=False):
+    dest = Path(dest)
+    notgcs = not str(dest).startswith('gs://')
     if recursive:
+      notgcs and dest.mkdirs()
       for child in self.glob('**'):
-        name = str(child).removeprefix(str(self))
-        child.copy(dest / name)
+        name = str(child).removeprefix(str(self) + '/')
+        if child.isdir():
+          notgcs and dest.mkdirs()
+        else:
+          child.copy(dest / name)
     elif str(dest).startswith('gs://'):
       dest = type(self)(dest)
       self.bucket.copy_blob(self.blob, dest.bucket, dest.blob.name)
     else:
       data = self.read('rb')
       Path(dest).write(data, 'wb')
```

### Comparing `elements-3.6.1/elements/plotting.py` & `elements-3.6.3/elements/plotting.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/printing.py` & `elements-3.6.3/elements/printing.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/rwlock.py` & `elements-3.6.3/elements/rwlock.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/timer.py` & `elements-3.6.3/elements/timer.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/tree.py` & `elements-3.6.3/elements/tree.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/usage.py` & `elements-3.6.3/elements/usage.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/uuid.py` & `elements-3.6.3/elements/uuid.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements/when.py` & `elements-3.6.3/elements/when.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/elements.egg-info/PKG-INFO` & `elements-3.6.3/elements.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elements
-Version: 3.6.1
+Version: 3.6.3
 Summary: Building blocks for productive research.
 Home-page: http://github.com/danijar/elements
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `elements-3.6.1/elements.egg-info/SOURCES.txt` & `elements-3.6.3/elements.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/setup.py` & `elements-3.6.3/setup.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/tests/test_basics.py` & `elements-3.6.3/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/tests/test_checkpoint.py` & `elements-3.6.3/tests/test_checkpoint.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/tests/test_flags.py` & `elements-3.6.3/tests/test_flags.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/tests/test_path.py` & `elements-3.6.3/tests/test_path.py`

 * *Files identical despite different names*

### Comparing `elements-3.6.1/tests/test_tree.py` & `elements-3.6.3/tests/test_tree.py`

 * *Files identical despite different names*

