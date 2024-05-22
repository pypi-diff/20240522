# Comparing `tmp/firspackage-0.0.1.tar.gz` & `tmp/firspackage-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "firspackage-0.0.1.tar", last modified: Wed May 22 02:47:11 2024, max compression
+gzip compressed data, was "firspackage-0.0.2.tar", last modified: Wed May 22 03:06:37 2024, max compression
```

## Comparing `firspackage-0.0.1.tar` & `firspackage-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 02:47:11.530422 firspackage-0.0.1/
--rw-r--r--   0 xhxa053    (503) staff       (20)      578 2024-05-22 02:47:11.530103 firspackage-0.0.1/PKG-INFO
--rw-r--r--   0 xhxa053    (503) staff       (20)       20 2024-05-22 02:47:09.000000 firspackage-0.0.1/README.md
-drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 02:47:11.529776 firspackage-0.0.1/firspackage.egg-info/
--rw-r--r--   0 xhxa053    (503) staff       (20)      578 2024-05-22 02:47:11.000000 firspackage-0.0.1/firspackage.egg-info/PKG-INFO
--rw-r--r--   0 xhxa053    (503) staff       (20)      221 2024-05-22 02:47:11.000000 firspackage-0.0.1/firspackage.egg-info/SOURCES.txt
--rw-r--r--   0 xhxa053    (503) staff       (20)        1 2024-05-22 02:47:11.000000 firspackage-0.0.1/firspackage.egg-info/dependency_links.txt
--rw-r--r--   0 xhxa053    (503) staff       (20)       32 2024-05-22 02:47:11.000000 firspackage-0.0.1/firspackage.egg-info/requires.txt
--rw-r--r--   0 xhxa053    (503) staff       (20)        4 2024-05-22 02:47:11.000000 firspackage-0.0.1/firspackage.egg-info/top_level.txt
--rw-r--r--   0 xhxa053    (503) staff       (20)       38 2024-05-22 02:47:11.530494 firspackage-0.0.1/setup.cfg
--rw-r--r--   0 xhxa053    (503) staff       (20)     1054 2024-05-22 02:40:53.000000 firspackage-0.0.1/setup.py
-drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 02:47:11.529182 firspackage-0.0.1/src/
--rw-r--r--   0 xhxa053    (503) staff       (20)       28 2024-05-22 02:39:45.000000 firspackage-0.0.1/src/__init__.py
--rw-r--r--   0 xhxa053    (503) staff       (20)       42 2024-05-22 02:38:35.000000 firspackage-0.0.1/src/hello.py
+drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 03:06:37.152620 firspackage-0.0.2/
+-rw-r--r--   0 xhxa053    (503) staff       (20)      521 2024-05-22 03:06:37.152329 firspackage-0.0.2/PKG-INFO
+-rw-r--r--   0 xhxa053    (503) staff       (20)       20 2024-05-22 02:47:09.000000 firspackage-0.0.2/README.md
+drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 03:06:37.151966 firspackage-0.0.2/firspackage.egg-info/
+-rw-r--r--   0 xhxa053    (503) staff       (20)      521 2024-05-22 03:06:37.000000 firspackage-0.0.2/firspackage.egg-info/PKG-INFO
+-rw-r--r--   0 xhxa053    (503) staff       (20)      221 2024-05-22 03:06:37.000000 firspackage-0.0.2/firspackage.egg-info/SOURCES.txt
+-rw-r--r--   0 xhxa053    (503) staff       (20)        1 2024-05-22 03:06:37.000000 firspackage-0.0.2/firspackage.egg-info/dependency_links.txt
+-rw-r--r--   0 xhxa053    (503) staff       (20)        5 2024-05-22 03:06:37.000000 firspackage-0.0.2/firspackage.egg-info/requires.txt
+-rw-r--r--   0 xhxa053    (503) staff       (20)        4 2024-05-22 03:06:37.000000 firspackage-0.0.2/firspackage.egg-info/top_level.txt
+-rw-r--r--   0 xhxa053    (503) staff       (20)       38 2024-05-22 03:06:37.152701 firspackage-0.0.2/setup.cfg
+-rw-r--r--   0 xhxa053    (503) staff       (20)     1021 2024-05-22 03:05:14.000000 firspackage-0.0.2/setup.py
+drwxr-xr-x   0 xhxa053    (503) staff       (20)        0 2024-05-22 03:06:37.151427 firspackage-0.0.2/src/
+-rw-r--r--   0 xhxa053    (503) staff       (20)       28 2024-05-22 02:39:45.000000 firspackage-0.0.2/src/__init__.py
+-rw-r--r--   0 xhxa053    (503) staff       (20)       42 2024-05-22 02:38:35.000000 firspackage-0.0.2/src/hello.py
```

### Comparing `firspackage-0.0.1/PKG-INFO` & `firspackage-0.0.2/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: firspackage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Haitham Alnajdawi
 Author-email: <mail@neuralnine.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
-Requires-Dist: pyautogui
-Requires-Dist: pyaudio
+Requires-Dist: time
 
 
 First python package
```

### Comparing `firspackage-0.0.1/firspackage.egg-info/PKG-INFO` & `firspackage-0.0.2/firspackage.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 Metadata-Version: 2.1
 Name: firspackage
-Version: 0.0.1
+Version: 0.0.2
 Summary: Streaming video data via networks
 Author: Haitham Alnajdawi
 Author-email: <mail@neuralnine.com>
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: Unix
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Description-Content-Type: text/markdown
-Requires-Dist: opencv-python
-Requires-Dist: pyautogui
-Requires-Dist: pyaudio
+Requires-Dist: time
 
 
 First python package
```

### Comparing `firspackage-0.0.1/setup.py` & `firspackage-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,29 +3,29 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Streaming video data via networks'
 LONG_DESCRIPTION = 'A package that allows to build simple streams of video, audio and camera data.'
 
 # Setting up
 setup(
     name="firspackage",
     version=VERSION,
     author="Haitham Alnajdawi",
     author_email="<mail@neuralnine.com>",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=long_description,
     packages=find_packages(),
-    install_requires=['opencv-python', 'pyautogui', 'pyaudio'],
+    install_requires=['time'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
```

