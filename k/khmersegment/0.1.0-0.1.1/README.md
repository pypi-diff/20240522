# Comparing `tmp/khmersegment-0.1.0.tar.gz` & `tmp/khmersegment-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "khmersegment-0.1.0.tar", last modified: Wed May 22 16:27:23 2024, max compression
+gzip compressed data, was "khmersegment-0.1.1.tar", last modified: Wed May 22 16:43:57 2024, max compression
```

## Comparing `khmersegment-0.1.0.tar` & `khmersegment-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:27:23.791329 khmersegment-0.1.0/
--rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-22 13:14:33.000000 khmersegment-0.1.0/LICENSE
--rw-r--r--   0 seanghay   (501) staff       (20)     1616 2024-05-22 16:27:23.791226 khmersegment-0.1.0/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      822 2024-05-22 16:25:28.000000 khmersegment-0.1.0/README.md
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:27:23.790604 khmersegment-0.1.0/khmersegment/
--rw-r--r--   0 seanghay   (501) staff       (20)     3227 2024-05-22 16:22:27.000000 khmersegment-0.1.0/khmersegment/__init__.py
-drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:27:23.791063 khmersegment-0.1.0/khmersegment.egg-info/
--rw-r--r--   0 seanghay   (501) staff       (20)     1616 2024-05-22 16:27:23.000000 khmersegment-0.1.0/khmersegment.egg-info/PKG-INFO
--rw-r--r--   0 seanghay   (501) staff       (20)      230 2024-05-22 16:27:23.000000 khmersegment-0.1.0/khmersegment.egg-info/SOURCES.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-22 16:27:23.000000 khmersegment-0.1.0/khmersegment.egg-info/dependency_links.txt
--rw-r--r--   0 seanghay   (501) staff       (20)        8 2024-05-22 16:27:23.000000 khmersegment-0.1.0/khmersegment.egg-info/requires.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       13 2024-05-22 16:27:23.000000 khmersegment-0.1.0/khmersegment.egg-info/top_level.txt
--rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-22 16:27:23.791363 khmersegment-0.1.0/setup.cfg
--rw-r--r--   0 seanghay   (501) staff       (20)      871 2024-05-22 16:23:19.000000 khmersegment-0.1.0/setup.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:43:57.160006 khmersegment-0.1.1/
+-rw-r--r--   0 seanghay   (501) staff       (20)    11343 2024-05-22 13:14:33.000000 khmersegment-0.1.1/LICENSE
+-rw-r--r--   0 seanghay   (501) staff       (20)     1616 2024-05-22 16:43:57.159891 khmersegment-0.1.1/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      822 2024-05-22 16:25:28.000000 khmersegment-0.1.1/README.md
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:43:57.159182 khmersegment-0.1.1/khmersegment/
+-rw-r--r--   0 seanghay   (501) staff       (20)     3228 2024-05-22 16:43:32.000000 khmersegment-0.1.1/khmersegment/__init__.py
+drwxr-xr-x   0 seanghay   (501) staff       (20)        0 2024-05-22 16:43:57.159730 khmersegment-0.1.1/khmersegment.egg-info/
+-rw-r--r--   0 seanghay   (501) staff       (20)     1616 2024-05-22 16:43:57.000000 khmersegment-0.1.1/khmersegment.egg-info/PKG-INFO
+-rw-r--r--   0 seanghay   (501) staff       (20)      230 2024-05-22 16:43:57.000000 khmersegment-0.1.1/khmersegment.egg-info/SOURCES.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        1 2024-05-22 16:43:57.000000 khmersegment-0.1.1/khmersegment.egg-info/dependency_links.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)        8 2024-05-22 16:43:57.000000 khmersegment-0.1.1/khmersegment.egg-info/requires.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       13 2024-05-22 16:43:57.000000 khmersegment-0.1.1/khmersegment.egg-info/top_level.txt
+-rw-r--r--   0 seanghay   (501) staff       (20)       38 2024-05-22 16:43:57.160061 khmersegment-0.1.1/setup.cfg
+-rw-r--r--   0 seanghay   (501) staff       (20)      871 2024-05-22 16:43:38.000000 khmersegment-0.1.1/setup.py
```

### Comparing `khmersegment-0.1.0/LICENSE` & `khmersegment-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `khmersegment-0.1.0/PKG-INFO` & `khmersegment-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khmersegment
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Khmer word segmentation tool built for NIPTICT Khmer Word Segmentation CRF model.
 Home-page: https://github.com/seanghay/khmersegment
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Khmer Segment
```

### Comparing `khmersegment-0.1.0/README.md` & `khmersegment-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `khmersegment-0.1.0/khmersegment/__init__.py` & `khmersegment-0.1.1/khmersegment/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     
     chunk += input_encodings[i][0]
     
     if tag == "0" or i == 0:
       continue
     
     if not deep:
-      if tag == "~":
+      if tag != "}{":
         continue
 
     yield chunk
     chunk = ""
 
   if chunk:
     yield chunk
```

### Comparing `khmersegment-0.1.0/khmersegment.egg-info/PKG-INFO` & `khmersegment-0.1.1/khmersegment.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: khmersegment
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Khmer word segmentation tool built for NIPTICT Khmer Word Segmentation CRF model.
 Home-page: https://github.com/seanghay/khmersegment
 Author: Seanghay Yath
 Author-email: seanghay.dev@gmail.com
 License: Apache License 2.0
 Description: ## Khmer Segment
```

### Comparing `khmersegment-0.1.0/setup.py` & `khmersegment-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="khmersegment",
-    version="0.1.0",
+    version="0.1.1",
     description="A Khmer word segmentation tool built for NIPTICT Khmer Word Segmentation CRF model.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/seanghay/khmersegment",
     author="Seanghay Yath",
     author_email="seanghay.dev@gmail.com",
     license="Apache License 2.0",
```

