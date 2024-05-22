# Comparing `tmp/pyiter-0.9.0.tar.gz` & `tmp/pyiter-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiter-0.9.0.tar", last modified: Fri Apr 19 23:28:31 2024, max compression
+gzip compressed data, was "pyiter-0.9.1.tar", last modified: Wed May 22 12:13:59 2024, max compression
```

## Comparing `pyiter-0.9.0.tar` & `pyiter-0.9.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 23:28:31.710628 pyiter-0.9.0/
--rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.9.0/LICENSE-APACHE
--rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.9.0/LICENSE-MIT
--rw-r--r--   0 yish      (1000) yish      (1000)     2896 2024-04-19 23:28:31.710628 pyiter-0.9.0/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)     2342 2024-04-19 23:28:01.000000 pyiter-0.9.0/README.md
--rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.9.0/pyproject.toml
--rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-19 23:28:31.710628 pyiter-0.9.0/setup.cfg
--rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-19 23:27:04.000000 pyiter-0.9.0/setup.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 23:28:31.710628 pyiter-0.9.0/src/
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 23:28:31.710628 pyiter-0.9.0/src/pyiter/
--rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.9.0/src/pyiter/__init__.py
--rw-r--r--   0 yish      (1000) yish      (1000)   103216 2024-04-19 23:25:19.000000 pyiter-0.9.0/src/pyiter/sequence.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-19 23:28:31.710628 pyiter-0.9.0/src/pyiter.egg-info/
--rw-r--r--   0 yish      (1000) yish      (1000)     2896 2024-04-19 23:28:31.000000 pyiter-0.9.0/src/pyiter.egg-info/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-19 23:28:31.000000 pyiter-0.9.0/src/pyiter.egg-info/SOURCES.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-19 23:28:31.000000 pyiter-0.9.0/src/pyiter.egg-info/dependency_links.txt
--rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-19 23:28:31.000000 pyiter-0.9.0/src/pyiter.egg-info/requires.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-19 23:28:31.000000 pyiter-0.9.0/src/pyiter.egg-info/top_level.txt
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-05-22 12:13:58.987802 pyiter-0.9.1/
+-rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.9.1/LICENSE-APACHE
+-rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.9.1/LICENSE-MIT
+-rw-r--r--   0 yish      (1000) yish      (1000)     2896 2024-05-22 12:13:58.987802 pyiter-0.9.1/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)     2342 2024-04-19 23:28:01.000000 pyiter-0.9.1/README.md
+-rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.9.1/pyproject.toml
+-rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-05-22 12:13:58.987802 pyiter-0.9.1/setup.cfg
+-rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-05-22 12:13:32.000000 pyiter-0.9.1/setup.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-05-22 12:13:58.987802 pyiter-0.9.1/src/
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-05-22 12:13:58.987802 pyiter-0.9.1/src/pyiter/
+-rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.9.1/src/pyiter/__init__.py
+-rw-r--r--   0 yish      (1000) yish      (1000)   104362 2024-05-22 12:11:26.000000 pyiter-0.9.1/src/pyiter/sequence.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-05-22 12:13:58.987802 pyiter-0.9.1/src/pyiter.egg-info/
+-rw-r--r--   0 yish      (1000) yish      (1000)     2896 2024-05-22 12:13:58.000000 pyiter-0.9.1/src/pyiter.egg-info/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-05-22 12:13:58.000000 pyiter-0.9.1/src/pyiter.egg-info/SOURCES.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-05-22 12:13:58.000000 pyiter-0.9.1/src/pyiter.egg-info/dependency_links.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-05-22 12:13:58.000000 pyiter-0.9.1/src/pyiter.egg-info/requires.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-05-22 12:13:58.000000 pyiter-0.9.1/src/pyiter.egg-info/top_level.txt
```

### Comparing `pyiter-0.9.0/LICENSE-APACHE` & `pyiter-0.9.1/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pyiter-0.9.0/LICENSE-MIT` & `pyiter-0.9.1/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyiter-0.9.0/PKG-INFO` & `pyiter-0.9.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.9.0
+Version: 0.9.1
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

### Comparing `pyiter-0.9.0/README.md` & `pyiter-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pyiter-0.9.0/setup.py` & `pyiter-0.9.1/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyiter',
-    version='0.9.0',
+    version='0.9.1',
     keywords=['linq', 'iterator', 'typing', 'lazy evaluation', 'type inference'],
     description='PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt '
                 'and Rust . Enables strong typing and type inference for iterative operations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='YISH',
     author_email="mokeyish@hotmail.com",
```

### Comparing `pyiter-0.9.0/src/pyiter/__init__.py` & `pyiter-0.9.1/src/pyiter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiter-0.9.0/src/pyiter/sequence.py` & `pyiter-0.9.1/src/pyiter/sequence.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,14 +101,20 @@
         >>> lst = [ 'a1', 'a2', 'b1', 'b2']
         >>> it(lst).filter_not(lambda x, i: x.startswith('a') and i % 2 == 0 ).to_list()
         ['a2', 'b1', 'b2']
         """
         predicate = self._callback_overload_warpper(predicate)
         return self.filter(lambda x: not predicate(x))
 
+    @overload
+    def filter_not_none(self: Sequence[Optional[R]]) -> Sequence[R]:
+        ...
+    @overload
+    def filter_not_none(self: Sequence[T]) -> Sequence[T]:
+        ...
     def filter_not_none(self: Sequence[Optional[R]]) -> Sequence[R]:
         """
         Returns a Sequence containing all elements that are not `None`.
 
         Example 1:
         >>> lst = [ 'a', None, 'b']
         >>> it(lst).filter_not_none().to_list()
@@ -2613,14 +2619,17 @@
         return self.__do_iter()
     
     def __do_iter(self) -> Iterator[T]:
         yield from self._iter
 
     def __len__(self):
         return len(self._iter)
+    
+    def __repr__(self):
+        return repr(self.to_list())
 
     def __getitem__(self, key: int):
         """
         Returns the element at the specified [index] in the Sequence.
 
         Example 1:
         >>> lst = [1, 2, 3]
@@ -3051,18 +3060,43 @@
             data = json.load(f, **kwargs) # type: ignore
             return self(data)
     
     def csv(self, filepath: str):
         """
         Reads and parses the input of a csv file.
         """
+        return self.read_csv(filepath)
+    
+    def read_csv(self, filepath: str, header: Optional[int]=0):
+        """
+        Reads and parses the input of a csv file.
+
+        Example 1:
+        >>> it.read_csv('tests/data/a.csv')
+        [{'a': 'a1', 'b': '1'}, {'a': 'a2', 'b': '2'}]
+        """
         import csv
+        it = self
         with open(filepath) as f:
-            r = csv.reader(f)
-            return it(r)
+            reader = csv.reader(f)
+            iter = it(*reader)
+            if header is None or header < 0:
+                return iter
+            
+            headers = iter.element_at_or_none(header)
+            if headers is not None:
+                if header == 0:
+                    iter = iter.skip(1)
+                else:
+                    iter = iter.filter(lambda _, i: i != header)
+                
+                return iter.map(lambda row: it(row).associate_by(
+                    lambda _, ordinal: headers[ordinal] if ordinal < len(headers) else f'undefined_{ordinal}')
+                )
+            return iter
 
 
 sequence = SequenceProducer()
 """
     Creates an iterator from a list of elements or given Iterable.
 
     Example 1:
```

### Comparing `pyiter-0.9.0/src/pyiter.egg-info/PKG-INFO` & `pyiter-0.9.1/src/pyiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.9.0
+Version: 0.9.1
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

