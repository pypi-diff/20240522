# Comparing `tmp/sumonet-0.1.6.tar.gz` & `tmp/sumonet-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumonet-0.1.6.tar", last modified: Sun Feb 25 15:53:43 2024, max compression
+gzip compressed data, was "sumonet-0.1.7.tar", last modified: Wed May 22 15:50:51 2024, max compression
```

## Comparing `sumonet-0.1.6.tar` & `sumonet-0.1.7.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.817727 sumonet-0.1.6/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)    10312 2023-08-26 11:09:19.000000 sumonet-0.1.6/LICENSE.rst
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1474 2024-02-25 15:53:43.817610 sumonet-0.1.6/PKG-INFO
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1003 2024-02-25 15:30:22.000000 sumonet-0.1.6/README.md
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)       38 2024-02-25 15:53:43.817777 sumonet-0.1.6/setup.cfg
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1112 2024-02-25 15:51:08.000000 sumonet-0.1.6/setup.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.808497 sumonet-0.1.6/sumonet/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:20.000000 sumonet-0.1.6/sumonet/__init__.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.810010 sumonet-0.1.6/sumonet/data/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.6/sumonet/data/__init__.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.810523 sumonet-0.1.6/sumonet/data/hard_test_samples/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.6/sumonet/data/hard_test_samples/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     2490 2023-08-26 11:09:19.000000 sumonet-0.1.6/sumonet/data/hard_test_samples/hard_samples_negative.fasta
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     6290 2023-08-26 11:09:19.000000 sumonet-0.1.6/sumonet/data/hard_test_samples/hard_samples_positive.fasta
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.811538 sumonet-0.1.6/sumonet/data/test/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)    62106 2023-08-26 11:09:19.000000 sumonet-0.1.6/sumonet/data/test/Sumoylation_neg_Test.fasta
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)    20002 2023-08-26 11:09:19.000000 sumonet-0.1.6/sumonet/data/test/Sumoylation_pos_Test.fasta
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.6/sumonet/data/test/__init__.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.814010 sumonet-0.1.6/sumonet/data/train/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)   558746 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/data/train/Sumoylation_neg_Train.fasta
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)   180383 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/data/train/Sumoylation_pos_Train.fasta
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.6/sumonet/data/train/__init__.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.814192 sumonet-0.1.6/sumonet/evaluation/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:52.000000 sumonet-0.1.6/sumonet/evaluation/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1972 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/evaluation/metrics.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.814521 sumonet-0.1.6/sumonet/model/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/model/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     2791 2023-08-26 17:22:42.000000 sumonet-0.1.6/sumonet/model/architecture.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.815508 sumonet-0.1.6/sumonet/model/pretrained/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 19:12:18.000000 sumonet-0.1.6/sumonet/model/pretrained/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)   226272 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/model/pretrained/sumonet3.h5
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)   225992 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/model/pretrained/sumonet3_partial.h5
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.816419 sumonet-0.1.6/sumonet/utils/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:20.000000 sumonet-0.1.6/sumonet/utils/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     9810 2023-08-28 17:37:10.000000 sumonet-0.1.6/sumonet/utils/data_pipe.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.816727 sumonet-0.1.6/sumonet/utils/encoding_matrix/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:26:14.000000 sumonet-0.1.6/sumonet/utils/encoding_matrix/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1624 2024-02-25 14:00:19.000000 sumonet-0.1.6/sumonet/utils/encoding_matrix/blosum62.csv
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     4216 2024-02-25 15:29:18.000000 sumonet-0.1.6/sumonet/utils/encodings.py
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.817023 sumonet-0.1.6/sumonet/utils/scaler/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 17:41:00.000000 sumonet-0.1.6/sumonet/utils/scaler/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)      867 2023-08-26 11:09:20.000000 sumonet-0.1.6/sumonet/utils/scaler/minmax_scaler.gz
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.809297 sumonet-0.1.6/sumonet.egg-info/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1474 2024-02-25 15:53:43.000000 sumonet-0.1.6/sumonet.egg-info/PKG-INFO
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1149 2024-02-25 15:53:43.000000 sumonet-0.1.6/sumonet.egg-info/SOURCES.txt
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        1 2024-02-25 15:53:43.000000 sumonet-0.1.6/sumonet.egg-info/dependency_links.txt
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)       76 2024-02-25 15:53:43.000000 sumonet-0.1.6/sumonet.egg-info/requires.txt
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)       14 2024-02-25 15:53:43.000000 sumonet-0.1.6/sumonet.egg-info/top_level.txt
-drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:53:43.817334 sumonet-0.1.6/tests/
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 14:38:18.000000 sumonet-0.1.6/tests/__init__.py
--rw-r--r--   0 berkedilekoglu   (501) staff       (20)      776 2024-02-25 14:56:22.000000 sumonet-0.1.6/tests/test_encodings.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.249286 sumonet-0.1.7/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)    10312 2023-08-26 11:09:19.000000 sumonet-0.1.7/LICENSE.rst
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1474 2024-05-22 15:50:51.249166 sumonet-0.1.7/PKG-INFO
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1003 2024-02-25 15:30:22.000000 sumonet-0.1.7/README.md
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)       38 2024-05-22 15:50:51.249329 sumonet-0.1.7/setup.cfg
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1127 2024-05-22 15:50:36.000000 sumonet-0.1.7/setup.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.234716 sumonet-0.1.7/sumonet/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:20.000000 sumonet-0.1.7/sumonet/__init__.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.235438 sumonet-0.1.7/sumonet/data/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.7/sumonet/data/__init__.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.235920 sumonet-0.1.7/sumonet/data/hard_test_samples/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.7/sumonet/data/hard_test_samples/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     2490 2023-08-26 11:09:19.000000 sumonet-0.1.7/sumonet/data/hard_test_samples/hard_samples_negative.fasta
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     6290 2023-08-26 11:09:19.000000 sumonet-0.1.7/sumonet/data/hard_test_samples/hard_samples_positive.fasta
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.236690 sumonet-0.1.7/sumonet/data/test/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)    62106 2023-08-26 11:09:19.000000 sumonet-0.1.7/sumonet/data/test/Sumoylation_neg_Test.fasta
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)    20002 2023-08-26 11:09:19.000000 sumonet-0.1.7/sumonet/data/test/Sumoylation_pos_Test.fasta
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.7/sumonet/data/test/__init__.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.242916 sumonet-0.1.7/sumonet/data/train/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)   558746 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/data/train/Sumoylation_neg_Train.fasta
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)   180383 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/data/train/Sumoylation_pos_Train.fasta
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 18:00:42.000000 sumonet-0.1.7/sumonet/data/train/__init__.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.243120 sumonet-0.1.7/sumonet/evaluation/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:52.000000 sumonet-0.1.7/sumonet/evaluation/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1972 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/evaluation/metrics.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.243637 sumonet-0.1.7/sumonet/model/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/model/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     2791 2023-08-26 17:22:42.000000 sumonet-0.1.7/sumonet/model/architecture.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.245515 sumonet-0.1.7/sumonet/model/pretrained/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 19:12:18.000000 sumonet-0.1.7/sumonet/model/pretrained/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)   226272 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/model/pretrained/sumonet3.h5
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)   225992 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/model/pretrained/sumonet3_partial.h5
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.247208 sumonet-0.1.7/sumonet/utils/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 16:49:20.000000 sumonet-0.1.7/sumonet/utils/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     9810 2023-08-28 17:37:10.000000 sumonet-0.1.7/sumonet/utils/data_pipe.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.248035 sumonet-0.1.7/sumonet/utils/encoding_matrix/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 15:26:14.000000 sumonet-0.1.7/sumonet/utils/encoding_matrix/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1624 2024-02-25 14:00:19.000000 sumonet-0.1.7/sumonet/utils/encoding_matrix/blosum62.csv
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     4216 2024-02-25 15:29:18.000000 sumonet-0.1.7/sumonet/utils/encodings.py
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.248455 sumonet-0.1.7/sumonet/utils/scaler/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2023-08-26 17:41:00.000000 sumonet-0.1.7/sumonet/utils/scaler/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)      867 2023-08-26 11:09:20.000000 sumonet-0.1.7/sumonet/utils/scaler/minmax_scaler.gz
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.235327 sumonet-0.1.7/sumonet.egg-info/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1474 2024-05-22 15:50:51.000000 sumonet-0.1.7/sumonet.egg-info/PKG-INFO
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)     1149 2024-05-22 15:50:51.000000 sumonet-0.1.7/sumonet.egg-info/SOURCES.txt
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        1 2024-05-22 15:50:51.000000 sumonet-0.1.7/sumonet.egg-info/dependency_links.txt
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)       92 2024-05-22 15:50:51.000000 sumonet-0.1.7/sumonet.egg-info/requires.txt
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)       14 2024-05-22 15:50:51.000000 sumonet-0.1.7/sumonet.egg-info/top_level.txt
+drwxr-xr-x   0 berkedilekoglu   (501) staff       (20)        0 2024-05-22 15:50:51.248789 sumonet-0.1.7/tests/
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)        0 2024-02-25 14:38:18.000000 sumonet-0.1.7/tests/__init__.py
+-rw-r--r--   0 berkedilekoglu   (501) staff       (20)      776 2024-02-25 14:56:22.000000 sumonet-0.1.7/tests/test_encodings.py
```

### Comparing `sumonet-0.1.6/LICENSE.rst` & `sumonet-0.1.7/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/PKG-INFO` & `sumonet-0.1.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumonet
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package Description
 Home-page: https://github.com/berkedilekoglu/SUMOnet
 Download-URL: https://github.com/berkedilekoglu/SUMOnet/archive/refs/tags/v0.1.6tar.gz
 Author: Berke Dilekoglu
 Author-email: berkedilekoglu@sabanciuniv.edu
 License: Academic Free License ("AFL") v. 3.0
 Keywords: sumoylation machine-learning deep-learning bioinformatics
```

### Comparing `sumonet-0.1.6/README.md` & `sumonet-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/setup.py` & `sumonet-0.1.7/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='sumonet',
-    version='0.1.6',
+    version='0.1.7',
     license='Academic Free License ("AFL") v. 3.0',
     description='Package Description',
     long_description=long_description,  # Use contents of README.md
     long_description_content_type='text/markdown',  # Specify content type
     author="Berke Dilekoglu",
     author_email='berkedilekoglu@sabanciuniv.edu',
     packages=find_packages(),
@@ -23,16 +23,15 @@
     download_url = 'https://github.com/berkedilekoglu/SUMOnet/archive/refs/tags/v0.1.6tar.gz', 
     keywords='sumoylation machine-learning deep-learning bioinformatics',
     install_requires=[
         'numpy',
         'scikit-learn',
         'joblib',
         'pandas',
-        'tensorflow',
-        'keras',
         'requests',
         'biopython',
         'loguru',
-
+        'tensorflow==2.15.0',
+        'keras==2.15.0'
       ],
 
-)
+)
```

### Comparing `sumonet-0.1.6/sumonet/data/hard_test_samples/hard_samples_negative.fasta` & `sumonet-0.1.7/sumonet/data/hard_test_samples/hard_samples_negative.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/data/hard_test_samples/hard_samples_positive.fasta` & `sumonet-0.1.7/sumonet/data/hard_test_samples/hard_samples_positive.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/data/test/Sumoylation_neg_Test.fasta` & `sumonet-0.1.7/sumonet/data/test/Sumoylation_neg_Test.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/data/test/Sumoylation_pos_Test.fasta` & `sumonet-0.1.7/sumonet/data/test/Sumoylation_pos_Test.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/data/train/Sumoylation_neg_Train.fasta` & `sumonet-0.1.7/sumonet/data/train/Sumoylation_neg_Train.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/data/train/Sumoylation_pos_Train.fasta` & `sumonet-0.1.7/sumonet/data/train/Sumoylation_pos_Train.fasta`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/evaluation/metrics.py` & `sumonet-0.1.7/sumonet/evaluation/metrics.py`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/model/architecture.py` & `sumonet-0.1.7/sumonet/model/architecture.py`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/model/pretrained/sumonet3.h5` & `sumonet-0.1.7/sumonet/model/pretrained/sumonet3.h5`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/model/pretrained/sumonet3_partial.h5` & `sumonet-0.1.7/sumonet/model/pretrained/sumonet3_partial.h5`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/utils/data_pipe.py` & `sumonet-0.1.7/sumonet/utils/data_pipe.py`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/utils/encoding_matrix/blosum62.csv` & `sumonet-0.1.7/sumonet/utils/encoding_matrix/blosum62.csv`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/utils/encodings.py` & `sumonet-0.1.7/sumonet/utils/encodings.py`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet/utils/scaler/minmax_scaler.gz` & `sumonet-0.1.7/sumonet/utils/scaler/minmax_scaler.gz`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/sumonet.egg-info/PKG-INFO` & `sumonet-0.1.7/sumonet.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumonet
-Version: 0.1.6
+Version: 0.1.7
 Summary: Package Description
 Home-page: https://github.com/berkedilekoglu/SUMOnet
 Download-URL: https://github.com/berkedilekoglu/SUMOnet/archive/refs/tags/v0.1.6tar.gz
 Author: Berke Dilekoglu
 Author-email: berkedilekoglu@sabanciuniv.edu
 License: Academic Free License ("AFL") v. 3.0
 Keywords: sumoylation machine-learning deep-learning bioinformatics
```

### Comparing `sumonet-0.1.6/sumonet.egg-info/SOURCES.txt` & `sumonet-0.1.7/sumonet.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sumonet-0.1.6/tests/test_encodings.py` & `sumonet-0.1.7/tests/test_encodings.py`

 * *Files identical despite different names*

