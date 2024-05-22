# Comparing `tmp/mysmallutils-2.0.8.tar.gz` & `tmp/mysmallutils-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mysmallutils-2.0.8.tar", last modified: Thu Jun  8 14:20:22 2023, max compression
+gzip compressed data, was "mysmallutils-2.0.9.tar", last modified: Wed Jun 28 12:15:40 2023, max compression
```

## Comparing `mysmallutils-2.0.8.tar` & `mysmallutils-2.0.9.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/
--rw-rw-rw-   0        0        0    60363 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    59881 2023-06-08 14:18:49.000000 mysmallutils-2.0.8/README.md
-drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.540732 mysmallutils-2.0.8/mysmallutils.egg-info/
--rw-rw-rw-   0        0        0    60363 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-06-08 14:20:22.000000 mysmallutils-2.0.8/mysmallutils.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-08 14:20:22.701259 mysmallutils-2.0.8/mysutils/
--rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/__init__.py
--rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.8/mysutils/collections.py
--rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/command.py
--rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/config.py
--rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/fastapi.py
--rw-rw-rw-   0        0        0    26268 2023-06-03 12:41:08.000000 mysmallutils-2.0.8/mysutils/file.py
--rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/logging.py
--rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/method.py
--rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/misc.py
--rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/request.py
--rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/service.py
--rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.8/mysutils/tar.py
--rw-rw-rw-   0        0        0    11276 2023-06-08 12:19:58.000000 mysmallutils-2.0.8/mysutils/text.py
--rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.8/mysutils/tmp.py
--rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/unittest.py
--rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.8/mysutils/web.py
--rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.8/mysutils/yaml.py
--rw-rw-rw-   0        0        0       42 2023-06-08 14:20:22.704259 mysmallutils-2.0.8/setup.cfg
--rw-rw-rw-   0        0        0     1711 2023-06-03 12:59:04.000000 mysmallutils-2.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-28 12:15:40.321153 mysmallutils-2.0.9/
+-rw-rw-rw-   0        0        0    60363 2023-06-28 12:15:40.321153 mysmallutils-2.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    59881 2023-06-08 14:18:49.000000 mysmallutils-2.0.9/README.md
+drwxrwxrwx   0        0        0        0 2023-06-28 12:15:40.280126 mysmallutils-2.0.9/mysmallutils.egg-info/
+-rw-rw-rw-   0        0        0    60363 2023-06-28 12:15:40.000000 mysmallutils-2.0.9/mysmallutils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-06-28 12:15:40.000000 mysmallutils-2.0.9/mysmallutils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-28 12:15:40.000000 mysmallutils-2.0.9/mysmallutils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-28 12:15:40.000000 mysmallutils-2.0.9/mysmallutils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-28 12:15:40.317803 mysmallutils-2.0.9/mysutils/
+-rw-rw-rw-   0        0        0        0 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/__init__.py
+-rw-rw-rw-   0        0        0    22982 2023-02-07 14:39:08.000000 mysmallutils-2.0.9/mysutils/collections.py
+-rw-rw-rw-   0        0        0     1533 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/command.py
+-rw-rw-rw-   0        0        0     1753 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/config.py
+-rw-rw-rw-   0        0        0     8540 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/fastapi.py
+-rw-rw-rw-   0        0        0    26406 2023-06-28 11:57:39.000000 mysmallutils-2.0.9/mysutils/file.py
+-rw-rw-rw-   0        0        0     2649 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/logging.py
+-rw-rw-rw-   0        0        0      639 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/method.py
+-rw-rw-rw-   0        0        0      467 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/misc.py
+-rw-rw-rw-   0        0        0      820 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/request.py
+-rw-rw-rw-   0        0        0     1861 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/service.py
+-rw-rw-rw-   0        0        0    12420 2023-02-10 08:55:00.000000 mysmallutils-2.0.9/mysutils/tar.py
+-rw-rw-rw-   0        0        0    11276 2023-06-08 12:19:58.000000 mysmallutils-2.0.9/mysutils/text.py
+-rw-rw-rw-   0        0        0     6479 2023-02-10 13:25:04.000000 mysmallutils-2.0.9/mysutils/tmp.py
+-rw-rw-rw-   0        0        0     1974 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/unittest.py
+-rw-rw-rw-   0        0        0     1175 2023-02-06 15:28:27.000000 mysmallutils-2.0.9/mysutils/web.py
+-rw-rw-rw-   0        0        0     3082 2023-02-07 14:39:08.000000 mysmallutils-2.0.9/mysutils/yaml.py
+-rw-rw-rw-   0        0        0       42 2023-06-28 12:15:40.322152 mysmallutils-2.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1306 2023-06-28 12:14:57.000000 mysmallutils-2.0.9/setup.py
```

### Comparing `mysmallutils-2.0.8/PKG-INFO` & `mysmallutils-2.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysmallutils-2.0.8/README.md` & `mysmallutils-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysmallutils.egg-info/PKG-INFO` & `mysmallutils-2.0.9/mysmallutils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mysmallutils
-Version: 2.0.8
+Version: 2.0.9
 Summary: Small Python utils to do life easier.
 Home-page: https://github.com/jmgomezsoriano/mysmallutils
 Author: José Manuel Gómez Soriano
 Author-email: jmgomez.soriano@gmail.com
 License: LGPL2
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mysmallutils-2.0.8/mysutils/collections.py` & `mysmallutils-2.0.9/mysutils/collections.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/command.py` & `mysmallutils-2.0.9/mysutils/command.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/config.py` & `mysmallutils-2.0.9/mysutils/config.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/fastapi.py` & `mysmallutils-2.0.9/mysutils/fastapi.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/file.py` & `mysmallutils-2.0.9/mysutils/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,18 +243,22 @@
     :param files: The list of files or empty directories to remove. To remove directories with files or subdirectories,
       please, use shutil.rmtree().
     :param ignore_errors: If True, ignore the error if the file or directory does not exist.
     :param recursive: If True, delete the folder recursively with all its content.
     """
     for file in expand_wildcards(*files):
         if isdir(file):
-            if recursive:
-                rmtree(file)
-            else:
-                rmdir(file)
+            try:
+                if recursive:
+                    rmtree(file)
+                else:
+                    rmdir(file)
+            except Exception as e:
+                if not ignore_errors:
+                    raise e
         elif not ignore_errors or exists(file):
             remove(file)
 
 
 def first_line(filename: Union[PathLike, str, bytes]) -> str:
     """ Read the first line of a file removing the final \n if it exists.
```

### Comparing `mysmallutils-2.0.8/mysutils/logging.py` & `mysmallutils-2.0.9/mysutils/logging.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/method.py` & `mysmallutils-2.0.9/mysutils/method.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/request.py` & `mysmallutils-2.0.9/mysutils/request.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/service.py` & `mysmallutils-2.0.9/mysutils/service.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/tar.py` & `mysmallutils-2.0.9/mysutils/tar.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/text.py` & `mysmallutils-2.0.9/mysutils/text.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/tmp.py` & `mysmallutils-2.0.9/mysutils/tmp.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/unittest.py` & `mysmallutils-2.0.9/mysutils/unittest.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/web.py` & `mysmallutils-2.0.9/mysutils/web.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/mysutils/yaml.py` & `mysmallutils-2.0.9/mysutils/yaml.py`

 * *Files identical despite different names*

### Comparing `mysmallutils-2.0.8/setup.py` & `mysmallutils-2.0.9/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import glob
-import os
 from shutil import rmtree
 
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
@@ -21,36 +20,18 @@
     def run(self):
         rmtree('build', ignore_errors=True)
         rmtree('dist', ignore_errors=True)
         for file in glob.glob('*.egg-info'):
             rmtree(file)
 
 
-class PrepublishCommand(setuptools.Command):
-    """ Custom prepublish command. """
-    user_options = []
-
-    def initialize_options(self):
-        pass
-
-    def finalize_options(self):
-        pass
-
-    def run(self):
-        os.system('python setup.py clean')
-        os.system('python setup.py sdist bdist_wheel')
-
-
 setuptools.setup(
-    cmdclass={
-        'clean': CleanCommand,
-        'prepublish': PrepublishCommand,
-    },
+    cmdclass={'clean': CleanCommand},
     name='mysmallutils',
-    version='2.0.8',
+    version='2.0.9',
     url='https://github.com/jmgomezsoriano/mysmallutils',
     license='LGPL2',
     author='José Manuel Gómez Soriano',
     author_email='jmgomez.soriano@gmail.com',
     long_description=long_description,
     long_description_content_type='text/markdown',
     description='Small Python utils to do life easier.',
```

