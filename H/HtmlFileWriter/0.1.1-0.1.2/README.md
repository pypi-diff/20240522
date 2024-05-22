# Comparing `tmp/htmlfilewriter-0.1.1.tar.gz` & `tmp/htmlfilewriter-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "htmlfilewriter-0.1.1.tar", last modified: Wed May 22 07:11:47 2024, max compression
+gzip compressed data, was "htmlfilewriter-0.1.2.tar", last modified: Wed May 22 07:43:47 2024, max compression
```

## Comparing `htmlfilewriter-0.1.1.tar` & `htmlfilewriter-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-22 07:11:47.406308 htmlfilewriter-0.1.1/
-drwxrwxrwx   0        0        0        0 2024-05-22 07:11:47.401943 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/
--rw-rw-rw-   0        0        0     1025 2024-05-22 07:11:47.000000 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      257 2024-05-22 07:11:47.000000 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-22 07:11:47.000000 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-22 07:11:47.000000 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-05-22 07:11:47.000000 htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 htmlfilewriter-0.1.1/LICENCE
--rw-rw-rw-   0        0        0     1025 2024-05-22 07:11:47.401943 htmlfilewriter-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0      334 2024-05-22 06:40:28.000000 htmlfilewriter-0.1.1/README.md
--rw-rw-rw-   0        0        0      379 2024-05-22 06:35:49.000000 htmlfilewriter-0.1.1/run.sh
--rw-rw-rw-   0        0        0       42 2024-05-22 07:11:47.407312 htmlfilewriter-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1364 2024-05-22 06:32:55.000000 htmlfilewriter-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-22 07:11:47.395695 htmlfilewriter-0.1.1/src/
--rw-rw-rw-   0        0        0       41 2024-05-22 06:20:25.000000 htmlfilewriter-0.1.1/src/__init__.py
--rw-rw-rw-   0        0        0      687 2024-05-22 06:18:03.000000 htmlfilewriter-0.1.1/src/html_writer.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:43:47.692322 htmlfilewriter-0.1.2/
+drwxrwxrwx   0        0        0        0 2024-05-22 07:43:47.681645 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/
+-rw-rw-rw-   0        0        0     1025 2024-05-22 07:43:46.000000 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      257 2024-05-22 07:43:47.000000 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-22 07:43:46.000000 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-22 07:43:46.000000 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-22 07:43:47.000000 htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1083 2024-05-18 13:06:21.000000 htmlfilewriter-0.1.2/LICENCE
+-rw-rw-rw-   0        0        0     1025 2024-05-22 07:43:47.686828 htmlfilewriter-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-05-22 06:40:28.000000 htmlfilewriter-0.1.2/README.md
+-rw-rw-rw-   0        0        0      379 2024-05-22 06:35:49.000000 htmlfilewriter-0.1.2/run.sh
+-rw-rw-rw-   0        0        0       42 2024-05-22 07:43:47.693813 htmlfilewriter-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1364 2024-05-22 07:41:39.000000 htmlfilewriter-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-22 07:43:47.675184 htmlfilewriter-0.1.2/src/
+-rw-rw-rw-   0        0        0       41 2024-05-22 06:20:25.000000 htmlfilewriter-0.1.2/src/__init__.py
+-rw-rw-rw-   0        0        0     1086 2024-05-22 07:38:13.000000 htmlfilewriter-0.1.2/src/html_writer.py
```

### Comparing `htmlfilewriter-0.1.1/HtmlFileWriter.egg-info/PKG-INFO` & `htmlfilewriter-0.1.2/HtmlFileWriter.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HtmlFileWriter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sets up and writes an HTML File using a filewriter.
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,FileWriter,App,HTML,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htmlfilewriter-0.1.1/LICENCE` & `htmlfilewriter-0.1.2/LICENCE`

 * *Files identical despite different names*

### Comparing `htmlfilewriter-0.1.1/PKG-INFO` & `htmlfilewriter-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HtmlFileWriter
-Version: 0.1.1
+Version: 0.1.2
 Summary: Sets up and writes an HTML File using a filewriter.
 Author: kunaalg
 Author-email: <kunaal@runcode.in>
 Keywords: python,FileWriter,App,HTML,Function,math
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `htmlfilewriter-0.1.1/setup.py` & `htmlfilewriter-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Sets up and writes an HTML File using a filewriter.'
 LONG_DESCRIPTION = 'A package that sets up a basic filewriter to write a HTML File in the current directory.'
 
 # Setting up
 setup(
     name="HtmlFileWriter",
     version=VERSION,
```

